# Comparing `tmp/firemon-api-0.2.10.tar.gz` & `tmp/firemon-api-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firemon-api-0.2.10.tar", last modified: Mon Apr 17 16:32:59 2023, max compression
+gzip compressed data, was "firemon-api-0.2.9.tar", last modified: Mon Apr 17 03:18:42 2023, max compression
```

## Comparing `firemon-api-0.2.10.tar` & `firemon-api-0.2.9.tar`

### file list

```diff
@@ -1,85 +1,80 @@
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 16:32:59.327600 firemon-api-0.2.10/
--rw-r--r--   0 luke      (1000) luke      (1000)     1234 2023-04-17 02:35:30.000000 firemon-api-0.2.10/.gitignore
--rw-r--r--   0 luke      (1000) luke      (1000)      172 2022-12-23 15:19:15.000000 firemon-api-0.2.10/.pre-commit-config.yaml
--rw-r--r--   0 luke      (1000) luke      (1000)       39 2022-12-23 15:19:15.000000 firemon-api-0.2.10/Makefile
--rw-r--r--   0 luke      (1000) luke      (1000)     3313 2023-04-17 16:32:59.327600 firemon-api-0.2.10/PKG-INFO
--rw-r--r--   0 luke      (1000) luke      (1000)     2049 2023-04-17 15:30:32.000000 firemon-api-0.2.10/README.md
--rw-r--r--   0 luke      (1000) luke      (1000)     2474 2023-04-17 15:40:06.000000 firemon-api-0.2.10/README.rst
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 16:32:59.327600 firemon-api-0.2.10/docs/
--rw-r--r--   0 luke      (1000) luke      (1000)      634 2023-04-16 22:05:23.000000 firemon-api-0.2.10/docs/Makefile
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 16:32:59.327600 firemon-api-0.2.10/docs/_static/
--rwxrwxrwx   0 luke      (1000) luke      (1000)     3549 2023-04-16 23:50:10.000000 firemon-api-0.2.10/docs/_static/logo_firemon.png
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 16:32:59.327600 firemon-api-0.2.10/docs/_templates/
--rw-r--r--   0 luke      (1000) luke      (1000)      911 2023-04-17 14:52:52.000000 firemon-api-0.2.10/docs/_templates/sidebarintro.html
--rw-r--r--   0 luke      (1000) luke      (1000)      741 2023-04-17 14:52:57.000000 firemon-api-0.2.10/docs/_templates/sidebarlogo.html
--rw-r--r--   0 luke      (1000) luke      (1000)     1735 2023-04-17 15:54:54.000000 firemon-api-0.2.10/docs/conf.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1497 2023-04-17 15:08:19.000000 firemon-api-0.2.10/docs/index.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      800 2023-04-16 22:05:23.000000 firemon-api-0.2.10/docs/make.bat
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 16:32:59.327600 firemon-api-0.2.10/docs/securitymanager/
--rw-r--r--   0 luke      (1000) luke      (1000)     3658 2023-04-17 15:56:40.000000 firemon-api-0.2.10/docs/securitymanager/devicepacks.rst
--rw-r--r--   0 luke      (1000) luke      (1000)       43 2023-04-17 15:56:35.000000 firemon-api-0.2.10/docs/securitymanager/devices.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     1149 2023-04-17 14:31:50.000000 firemon-api-0.2.10/docs/securitymanager/siql.rst
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 16:32:59.327600 firemon-api-0.2.10/docs/user/
--rw-r--r--   0 luke      (1000) luke      (1000)     1590 2023-04-17 14:42:18.000000 firemon-api-0.2.10/docs/user/advanced.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      302 2023-04-17 14:54:23.000000 firemon-api-0.2.10/docs/user/install.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     4709 2023-04-17 15:21:27.000000 firemon-api-0.2.10/docs/user/quickstart.rst
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 16:32:59.327600 firemon-api-0.2.10/firemon_api/
--rw-r--r--   0 luke      (1000) luke      (1000)     2432 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/__init__.py
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 16:32:59.327600 firemon-api-0.2.10/firemon_api/apps/
--rw-r--r--   0 luke      (1000) luke      (1000)    12060 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/__init__.py
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 16:32:59.327600 firemon-api-0.2.10/firemon_api/apps/controlpanel/
--rw-r--r--   0 luke      (1000) luke      (1000)      301 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/controlpanel/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1594 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/controlpanel/certauth.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1028 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/controlpanel/cleanup.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2369 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/controlpanel/config.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1819 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/controlpanel/database.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1798 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/controlpanel/diagpkg.py
--rw-r--r--   0 luke      (1000) luke      (1000)       68 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/controlpanel/errors.py
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 16:32:59.327600 firemon-api-0.2.10/firemon_api/apps/globalpolicycontroller/
--rw-r--r--   0 luke      (1000) luke      (1000)      425 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/globalpolicycontroller/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1511 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/globalpolicycontroller/policycompute.py
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 16:32:59.327600 firemon-api-0.2.10/firemon_api/apps/policyoptimizer/
--rw-r--r--   0 luke      (1000) luke      (1000)      357 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/policyoptimizer/__init__.py
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 16:32:59.327600 firemon-api-0.2.10/firemon_api/apps/policyplanner/
--rw-r--r--   0 luke      (1000) luke      (1000)      519 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/policyplanner/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     9918 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/policyplanner/packets.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2106 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/policyplanner/siql.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5954 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/policyplanner/tasks.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3996 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/policyplanner/workflows.py
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 16:32:59.327600 firemon-api-0.2.10/firemon_api/apps/securitymanager/
--rw-r--r--   0 luke      (1000) luke      (1000)     1822 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2867 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/access_path.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1709 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/centralsyslogconfigs.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3166 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/centralsyslogs.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5881 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/collectionconfigs.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5863 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/collectors.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1922 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/deviceclusters.py
--rw-r--r--   0 luke      (1000) luke      (1000)    10457 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/devicepacks.py
--rw-r--r--   0 luke      (1000) luke      (1000)    25810 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/devices.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1416 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/elasticsearch.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1943 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/license.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5764 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/logging.py
--rw-r--r--   0 luke      (1000) luke      (1000)     3068 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/maps.py
--rw-r--r--   0 luke      (1000) luke      (1000)     8005 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/revisions.py
--rw-r--r--   0 luke      (1000) luke      (1000)     4368 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/routes.py
--rw-r--r--   0 luke      (1000) luke      (1000)     4511 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/siql.py
--rw-r--r--   0 luke      (1000) luke      (1000)     9120 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/users.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5322 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/apps/securitymanager/zones.py
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 16:32:59.327600 firemon-api-0.2.10/firemon_api/core/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/core/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     8567 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/core/api.py
--rw-r--r--   0 luke      (1000) luke      (1000)     6679 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/core/endpoint.py
--rw-r--r--   0 luke      (1000) luke      (1000)    11340 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/core/query.py
--rw-r--r--   0 luke      (1000) luke      (1000)    11776 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/core/response.py
--rw-r--r--   0 luke      (1000) luke      (1000)     4109 2022-12-23 15:19:15.000000 firemon-api-0.2.10/firemon_api/core/utils.py
-drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 16:32:59.327600 firemon-api-0.2.10/firemon_api.egg-info/
--rw-r--r--   0 luke      (1000) luke      (1000)     3313 2023-04-17 16:32:59.000000 firemon-api-0.2.10/firemon_api.egg-info/PKG-INFO
--rw-r--r--   0 luke      (1000) luke      (1000)     2350 2023-04-17 16:32:59.000000 firemon-api-0.2.10/firemon_api.egg-info/SOURCES.txt
--rw-r--r--   0 luke      (1000) luke      (1000)        1 2023-04-17 16:32:59.000000 firemon-api-0.2.10/firemon_api.egg-info/dependency_links.txt
--rw-r--r--   0 luke      (1000) luke      (1000)        1 2023-04-17 02:58:14.000000 firemon-api-0.2.10/firemon_api.egg-info/not-zip-safe
--rw-r--r--   0 luke      (1000) luke      (1000)       18 2023-04-17 16:32:59.000000 firemon-api-0.2.10/firemon_api.egg-info/requires.txt
--rw-r--r--   0 luke      (1000) luke      (1000)       12 2023-04-17 16:32:59.000000 firemon-api-0.2.10/firemon_api.egg-info/top_level.txt
--rw-r--r--   0 luke      (1000) luke      (1000)      167 2022-12-23 15:19:15.000000 firemon-api-0.2.10/pyproject.toml
--rw-r--r--   0 luke      (1000) luke      (1000)       43 2022-12-23 15:19:15.000000 firemon-api-0.2.10/requirements.txt
--rw-r--r--   0 luke      (1000) luke      (1000)      983 2023-04-17 16:32:59.327600 firemon-api-0.2.10/setup.cfg
--rw-r--r--   0 luke      (1000) luke      (1000)       91 2022-12-23 15:19:15.000000 firemon-api-0.2.10/setup.py
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 03:18:42.918214 firemon-api-0.2.9/
+-rw-r--r--   0 luke      (1000) luke      (1000)     1234 2023-04-17 02:35:30.000000 firemon-api-0.2.9/.gitignore
+-rw-r--r--   0 luke      (1000) luke      (1000)      172 2022-12-23 15:19:15.000000 firemon-api-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 luke      (1000) luke      (1000)       39 2022-12-23 15:19:15.000000 firemon-api-0.2.9/Makefile
+-rw-r--r--   0 luke      (1000) luke      (1000)      673 2023-04-17 03:18:42.918214 firemon-api-0.2.9/PKG-INFO
+-rw-r--r--   0 luke      (1000) luke      (1000)     3175 2023-04-16 21:16:41.000000 firemon-api-0.2.9/README.md
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 03:18:42.918214 firemon-api-0.2.9/docs/
+-rw-r--r--   0 luke      (1000) luke      (1000)      634 2023-04-16 22:05:23.000000 firemon-api-0.2.9/docs/Makefile
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 03:18:42.918214 firemon-api-0.2.9/docs/_static/
+-rwxrwxrwx   0 luke      (1000) luke      (1000)     3549 2023-04-16 23:50:10.000000 firemon-api-0.2.9/docs/_static/logo_firemon.png
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 03:18:42.918214 firemon-api-0.2.9/docs/_templates/
+-rw-r--r--   0 luke      (1000) luke      (1000)      812 2023-04-17 02:40:33.000000 firemon-api-0.2.9/docs/_templates/sidebarintro.html
+-rw-r--r--   0 luke      (1000) luke      (1000)      642 2023-04-17 02:40:15.000000 firemon-api-0.2.9/docs/_templates/sidebarlogo.html
+-rw-r--r--   0 luke      (1000) luke      (1000)     1649 2023-04-17 02:43:48.000000 firemon-api-0.2.9/docs/conf.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1023 2023-04-17 02:49:26.000000 firemon-api-0.2.9/docs/index.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      800 2023-04-16 22:05:23.000000 firemon-api-0.2.9/docs/make.bat
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 03:18:42.918214 firemon-api-0.2.9/docs/securitymanager/
+-rw-r--r--   0 luke      (1000) luke      (1000)       22 2023-04-16 23:04:16.000000 firemon-api-0.2.9/docs/securitymanager/devices.rst
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 03:18:42.918214 firemon-api-0.2.9/docs/user/
+-rw-r--r--   0 luke      (1000) luke      (1000)       28 2023-04-16 22:59:59.000000 firemon-api-0.2.9/docs/user/quickstart.rst
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 03:18:42.918214 firemon-api-0.2.9/firemon_api/
+-rw-r--r--   0 luke      (1000) luke      (1000)     2432 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/__init__.py
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 03:18:42.918214 firemon-api-0.2.9/firemon_api/apps/
+-rw-r--r--   0 luke      (1000) luke      (1000)    12060 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/__init__.py
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 03:18:42.918214 firemon-api-0.2.9/firemon_api/apps/controlpanel/
+-rw-r--r--   0 luke      (1000) luke      (1000)      301 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/controlpanel/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1594 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/controlpanel/certauth.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1028 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/controlpanel/cleanup.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2369 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/controlpanel/config.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1819 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/controlpanel/database.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1798 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/controlpanel/diagpkg.py
+-rw-r--r--   0 luke      (1000) luke      (1000)       68 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/controlpanel/errors.py
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 03:18:42.918214 firemon-api-0.2.9/firemon_api/apps/globalpolicycontroller/
+-rw-r--r--   0 luke      (1000) luke      (1000)      425 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/globalpolicycontroller/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1511 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/globalpolicycontroller/policycompute.py
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 03:18:42.918214 firemon-api-0.2.9/firemon_api/apps/policyoptimizer/
+-rw-r--r--   0 luke      (1000) luke      (1000)      357 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/policyoptimizer/__init__.py
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 03:18:42.918214 firemon-api-0.2.9/firemon_api/apps/policyplanner/
+-rw-r--r--   0 luke      (1000) luke      (1000)      519 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/policyplanner/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     9918 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/policyplanner/packets.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2106 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/policyplanner/siql.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5954 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/policyplanner/tasks.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     3996 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/policyplanner/workflows.py
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 03:18:42.918214 firemon-api-0.2.9/firemon_api/apps/securitymanager/
+-rw-r--r--   0 luke      (1000) luke      (1000)     1822 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2867 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/access_path.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1709 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/centralsyslogconfigs.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     3166 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/centralsyslogs.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5881 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/collectionconfigs.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5863 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/collectors.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1922 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/deviceclusters.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    10457 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/devicepacks.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    25810 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/devices.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1416 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/elasticsearch.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1943 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/license.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5764 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/logging.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     3068 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/maps.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     8005 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/revisions.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     4368 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/routes.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     4511 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/siql.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     9120 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/users.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5322 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/apps/securitymanager/zones.py
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 03:18:42.918214 firemon-api-0.2.9/firemon_api/core/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/core/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     8567 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/core/api.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     6679 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/core/endpoint.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    11340 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/core/query.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    11776 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/core/response.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     4109 2022-12-23 15:19:15.000000 firemon-api-0.2.9/firemon_api/core/utils.py
+drwxr-xr-x   0 luke      (1000) luke      (1000)        0 2023-04-17 03:18:42.918214 firemon-api-0.2.9/firemon_api.egg-info/
+-rw-r--r--   0 luke      (1000) luke      (1000)      673 2023-04-17 03:18:42.000000 firemon-api-0.2.9/firemon_api.egg-info/PKG-INFO
+-rw-r--r--   0 luke      (1000) luke      (1000)     2227 2023-04-17 03:18:42.000000 firemon-api-0.2.9/firemon_api.egg-info/SOURCES.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)        1 2023-04-17 03:18:42.000000 firemon-api-0.2.9/firemon_api.egg-info/dependency_links.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)        1 2023-04-17 02:58:14.000000 firemon-api-0.2.9/firemon_api.egg-info/not-zip-safe
+-rw-r--r--   0 luke      (1000) luke      (1000)       18 2023-04-17 03:18:42.000000 firemon-api-0.2.9/firemon_api.egg-info/requires.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)       12 2023-04-17 03:18:42.000000 firemon-api-0.2.9/firemon_api.egg-info/top_level.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)      167 2022-12-23 15:19:15.000000 firemon-api-0.2.9/pyproject.toml
+-rw-r--r--   0 luke      (1000) luke      (1000)       43 2022-12-23 15:19:15.000000 firemon-api-0.2.9/requirements.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)      783 2023-04-17 03:18:42.918214 firemon-api-0.2.9/setup.cfg
+-rw-r--r--   0 luke      (1000) luke      (1000)       91 2022-12-23 15:19:15.000000 firemon-api-0.2.9/setup.py
```

### Comparing `firemon-api-0.2.10/.gitignore` & `firemon-api-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/docs/Makefile` & `firemon-api-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/docs/_static/logo_firemon.png` & `firemon-api-0.2.9/docs/_static/logo_firemon.png`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/docs/_templates/sidebarintro.html` & `firemon-api-0.2.9/docs/_templates/sidebarintro.html`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     FireMon-API is a Python web wrapper for the FireMon SIP (Security Mangager, etc...)
     APIs. The intent is make something that is useful for quick and easy development
     against FireMon products.
 </p>
 
 <h3>Useful Links</h3>
 <ul>
-    <li><a href="https://firemon-api.readthedocs.io/en/latest/user/install/">Installation</a></li>
     <li><a href="https://firemon-api.readthedocs.io/en/latest/user/quickstart/">Quickstart</a></li>
 
     <p></p>
 
     <p></p>
 
     <li><a href="https://github.com/lukejohannsen/firemon-api">FireMon-API @ GitHub</a></li>
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
 [Firemon_logo]
 FireMon-API is a Python web wrapper for the FireMon SIP (Security Mangager,
 etc...) APIs. The intent is make something that is useful for quick and easy
 development against FireMon products.
 **** Useful Links ****
-    * Installation
     * Quickstart
     * FireMon-API_@_GitHub
     * FireMon-API_@_PyPI
     * Issue_Tracker
```

### Comparing `firemon-api-0.2.10/docs/conf.py` & `firemon-api-0.2.9/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,15 @@
 project = "firemon-api"
 copyright = "2023, Luke Johannsen"
 author = "Luke Johannsen"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
-extensions = [
-    "sphinx.ext.todo",
-]
-
-# Display todos by setting to True
-todo_include_todos = True
+extensions = []
 
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
```

### Comparing `firemon-api-0.2.10/docs/make.bat` & `firemon-api-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/__init__.py` & `firemon-api-0.2.9/firemon_api/__init__.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/__init__.py` & `firemon-api-0.2.9/firemon_api/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/controlpanel/certauth.py` & `firemon-api-0.2.9/firemon_api/apps/controlpanel/certauth.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/controlpanel/cleanup.py` & `firemon-api-0.2.9/firemon_api/apps/controlpanel/cleanup.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/controlpanel/config.py` & `firemon-api-0.2.9/firemon_api/apps/controlpanel/config.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/controlpanel/database.py` & `firemon-api-0.2.9/firemon_api/apps/controlpanel/database.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/controlpanel/diagpkg.py` & `firemon-api-0.2.9/firemon_api/apps/controlpanel/diagpkg.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/globalpolicycontroller/policycompute.py` & `firemon-api-0.2.9/firemon_api/apps/globalpolicycontroller/policycompute.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/policyplanner/__init__.py` & `firemon-api-0.2.9/firemon_api/apps/policyplanner/__init__.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/policyplanner/packets.py` & `firemon-api-0.2.9/firemon_api/apps/policyplanner/packets.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/policyplanner/siql.py` & `firemon-api-0.2.9/firemon_api/apps/policyplanner/siql.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/policyplanner/tasks.py` & `firemon-api-0.2.9/firemon_api/apps/policyplanner/tasks.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/policyplanner/workflows.py` & `firemon-api-0.2.9/firemon_api/apps/policyplanner/workflows.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/__init__.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/__init__.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/access_path.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/access_path.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/centralsyslogconfigs.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/centralsyslogconfigs.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/centralsyslogs.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/centralsyslogs.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/collectionconfigs.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/collectionconfigs.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/collectors.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/collectors.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/deviceclusters.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/deviceclusters.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/devicepacks.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/devicepacks.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/devices.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/devices.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/elasticsearch.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/license.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/license.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/logging.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/logging.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/maps.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/maps.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/revisions.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/revisions.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/routes.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/routes.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/siql.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/siql.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/users.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/users.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/apps/securitymanager/zones.py` & `firemon-api-0.2.9/firemon_api/apps/securitymanager/zones.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/core/api.py` & `firemon-api-0.2.9/firemon_api/core/api.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/core/endpoint.py` & `firemon-api-0.2.9/firemon_api/core/endpoint.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/core/query.py` & `firemon-api-0.2.9/firemon_api/core/query.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/core/response.py` & `firemon-api-0.2.9/firemon_api/core/response.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api/core/utils.py` & `firemon-api-0.2.9/firemon_api/core/utils.py`

 * *Files identical despite different names*

### Comparing `firemon-api-0.2.10/firemon_api.egg-info/SOURCES.txt` & `firemon-api-0.2.9/firemon_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 .gitignore
 .pre-commit-config.yaml
 Makefile
 README.md
-README.rst
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/_static/logo_firemon.png
 docs/_templates/sidebarintro.html
 docs/_templates/sidebarlogo.html
-docs/securitymanager/devicepacks.rst
 docs/securitymanager/devices.rst
-docs/securitymanager/siql.rst
-docs/user/advanced.rst
-docs/user/install.rst
 docs/user/quickstart.rst
 firemon_api/__init__.py
 firemon_api.egg-info/PKG-INFO
 firemon_api.egg-info/SOURCES.txt
 firemon_api.egg-info/dependency_links.txt
 firemon_api.egg-info/not-zip-safe
 firemon_api.egg-info/requires.txt
```

