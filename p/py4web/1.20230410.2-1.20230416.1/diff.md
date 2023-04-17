# Comparing `tmp/py4web-1.20230410.2.tar.gz` & `tmp/py4web-1.20230416.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-1.20230410.2.tar", last modified: Tue Apr 11 05:54:14 2023, max compression
+gzip compressed data, was "py4web-1.20230416.1.tar", last modified: Mon Apr 17 00:40:00 2023, max compression
```

## Comparing `py4web-1.20230410.2.tar` & `py4web-1.20230416.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-11 05:54:14.893966 py4web-1.20230410.2/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      826 2023-04-11 05:54:14.893966 py4web-1.20230410.2/PKG-INFO
--rw-r--r--   0 massimo   (1000) massimo   (1000)     7120 2022-01-11 05:54:38.000000 py4web-1.20230410.2/README.rst
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-11 05:54:14.873966 py4web-1.20230410.2/py4web/
--rw-r--r--   0 massimo   (1000) massimo   (1000)      721 2023-04-11 05:53:42.000000 py4web-1.20230410.2/py4web/__init__.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-11 05:54:14.885966 py4web-1.20230410.2/py4web/assets/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  2990826 2023-04-11 05:51:49.000000 py4web-1.20230410.2/py4web/assets/py4web.app._dashboard.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)   182307 2023-04-11 05:51:49.000000 py4web-1.20230410.2/py4web/assets/py4web.app._default.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  4278028 2023-04-11 05:51:50.000000 py4web-1.20230410.2/py4web/assets/py4web.app._documentation.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      409 2023-04-11 05:51:49.000000 py4web-1.20230410.2/py4web/assets/py4web.app._minimal.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    16674 2023-04-11 05:51:49.000000 py4web-1.20230410.2/py4web/assets/py4web.app._scaffold.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  1386102 2023-04-11 05:51:50.000000 py4web-1.20230410.2/py4web/assets/py4web.app.showcase.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    67000 2023-04-11 05:51:13.000000 py4web-1.20230410.2/py4web/core.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7510 2022-06-30 06:41:15.000000 py4web-1.20230410.2/py4web/server_adapters.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-11 05:54:14.889966 py4web-1.20230410.2/py4web/utils/
--rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2019-07-23 06:20:41.000000 py4web-1.20230410.2/py4web/utils/__init__.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)    69664 2023-04-10 05:23:42.000000 py4web-1.20230410.2/py4web/utils/auth.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-11 05:54:14.893966 py4web-1.20230410.2/py4web/utils/auth_plugins/
--rw-r--r--   0 massimo   (1000) massimo   (1000)     6207 2023-04-10 03:57:23.000000 py4web-1.20230410.2/py4web/utils/auth_plugins/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      798 2023-04-10 01:56:10.000000 py4web-1.20230410.2/py4web/utils/auth_plugins/basic_auth_plugin.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)     8154 2022-03-15 04:37:19.000000 py4web-1.20230410.2/py4web/utils/auth_plugins/cas_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1441 2023-04-10 01:56:10.000000 py4web-1.20230410.2/py4web/utils/auth_plugins/email_auth_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    35513 2023-04-10 03:57:06.000000 py4web-1.20230410.2/py4web/utils/auth_plugins/ldap_plugin.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)     3563 2022-03-14 19:17:56.000000 py4web-1.20230410.2/py4web/utils/auth_plugins/newsamlplugin.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)     1759 2022-02-21 23:58:14.000000 py4web-1.20230410.2/py4web/utils/auth_plugins/oauth2discord.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      654 2020-10-10 04:20:35.000000 py4web-1.20230410.2/py4web/utils/auth_plugins/oauth2facebook.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      514 2023-04-10 03:57:06.000000 py4web-1.20230410.2/py4web/utils/auth_plugins/oauth2github.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      524 2020-10-10 04:20:35.000000 py4web-1.20230410.2/py4web/utils/auth_plugins/oauth2google.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      489 2020-10-10 04:20:35.000000 py4web-1.20230410.2/py4web/utils/auth_plugins/oauth2okta.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2084 2022-03-20 01:46:38.000000 py4web-1.20230410.2/py4web/utils/auth_plugins/oauth2server.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6090 2022-03-20 01:46:38.000000 py4web-1.20230410.2/py4web/utils/auth_plugins/oauth2wpminiorange.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5051 2022-03-20 01:46:38.000000 py4web-1.20230410.2/py4web/utils/auth_plugins/pam.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      187 2023-04-10 01:56:10.000000 py4web-1.20230410.2/py4web/utils/auth_plugins/pam_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6672 2022-03-20 01:46:38.000000 py4web-1.20230410.2/py4web/utils/auth_plugins/saml2_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2848 2022-03-20 01:46:38.000000 py4web-1.20230410.2/py4web/utils/auth_plugins/x509_auth_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      857 2022-03-20 01:46:38.000000 py4web-1.20230410.2/py4web/utils/cors.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1628 2023-01-11 05:50:14.000000 py4web-1.20230410.2/py4web/utils/dbstore.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2075 2022-03-20 01:46:38.000000 py4web-1.20230410.2/py4web/utils/downloader.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3142 2022-03-20 01:46:38.000000 py4web-1.20230410.2/py4web/utils/factories.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    35864 2023-03-17 04:41:37.000000 py4web-1.20230410.2/py4web/utils/form.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    68937 2023-04-10 02:55:45.000000 py4web-1.20230410.2/py4web/utils/grid.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1651 2022-06-08 06:27:50.000000 py4web-1.20230410.2/py4web/utils/jsonrpc.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    34865 2022-11-11 06:40:11.000000 py4web-1.20230410.2/py4web/utils/mailer.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     9196 2022-06-03 04:17:49.000000 py4web-1.20230410.2/py4web/utils/misc.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      502 2020-09-13 06:17:02.000000 py4web-1.20230410.2/py4web/utils/param.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    18269 2022-03-20 01:46:38.000000 py4web-1.20230410.2/py4web/utils/populate.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1694 2022-05-31 06:26:42.000000 py4web-1.20230410.2/py4web/utils/publisher.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2225 2023-03-19 21:28:12.000000 py4web-1.20230410.2/py4web/utils/recaptcha.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)    70958 2022-03-14 20:46:56.000000 py4web-1.20230410.2/py4web/utils/scheduler.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)    70958 2022-03-14 20:46:56.000000 py4web-1.20230410.2/py4web/utils/scheduler_old.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3728 2022-03-20 01:46:38.000000 py4web-1.20230410.2/py4web/utils/security.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      158 2022-03-20 01:46:38.000000 py4web-1.20230410.2/py4web/utils/tags.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6425 2022-09-24 20:59:44.000000 py4web-1.20230410.2/py4web/utils/url_signer.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-11 05:54:14.877966 py4web-1.20230410.2/py4web.egg-info/
--rw-r--r--   0 massimo   (1000) massimo   (1000)      826 2023-04-11 05:54:14.000000 py4web-1.20230410.2/py4web.egg-info/PKG-INFO
--rw-r--r--   0 massimo   (1000) massimo   (1000)     1727 2023-04-11 05:54:14.000000 py4web-1.20230410.2/py4web.egg-info/SOURCES.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2023-04-11 05:54:14.000000 py4web-1.20230410.2/py4web.egg-info/dependency_links.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)       44 2023-04-11 05:54:14.000000 py4web-1.20230410.2/py4web.egg-info/entry_points.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2020-09-07 23:01:39.000000 py4web-1.20230410.2/py4web.egg-info/not-zip-safe
--rw-r--r--   0 massimo   (1000) massimo   (1000)      215 2023-04-11 05:54:14.000000 py4web-1.20230410.2/py4web.egg-info/requires.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)        7 2023-04-11 05:54:14.000000 py4web-1.20230410.2/py4web.egg-info/top_level.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-04-11 05:54:14.893966 py4web-1.20230410.2/setup.cfg
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1758 2023-03-12 23:37:12.000000 py4web-1.20230410.2/setup.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 00:40:00.326947 py4web-1.20230416.1/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      826 2023-04-17 00:40:00.326947 py4web-1.20230416.1/PKG-INFO
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     7120 2022-01-11 05:54:38.000000 py4web-1.20230416.1/README.rst
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 00:40:00.310947 py4web-1.20230416.1/py4web/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      721 2023-04-17 00:39:40.000000 py4web-1.20230416.1/py4web/__init__.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 00:40:00.318947 py4web-1.20230416.1/py4web/assets/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)  2990826 2023-04-11 05:51:49.000000 py4web-1.20230416.1/py4web/assets/py4web.app._dashboard.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)   182307 2023-04-11 05:51:49.000000 py4web-1.20230416.1/py4web/assets/py4web.app._default.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)  4278028 2023-04-11 05:51:50.000000 py4web-1.20230416.1/py4web/assets/py4web.app._documentation.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      409 2023-04-11 05:51:49.000000 py4web-1.20230416.1/py4web/assets/py4web.app._minimal.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    16674 2023-04-11 05:51:49.000000 py4web-1.20230416.1/py4web/assets/py4web.app._scaffold.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)  1386102 2023-04-11 05:51:50.000000 py4web-1.20230416.1/py4web/assets/py4web.app.showcase.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    67378 2023-04-16 18:21:53.000000 py4web-1.20230416.1/py4web/core.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     7510 2022-06-30 06:41:15.000000 py4web-1.20230416.1/py4web/server_adapters.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 00:40:00.322947 py4web-1.20230416.1/py4web/utils/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2019-07-23 06:20:41.000000 py4web-1.20230416.1/py4web/utils/__init__.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)    69664 2023-04-10 05:23:42.000000 py4web-1.20230416.1/py4web/utils/auth.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 00:40:00.326947 py4web-1.20230416.1/py4web/utils/auth_plugins/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     6207 2023-04-10 03:57:23.000000 py4web-1.20230416.1/py4web/utils/auth_plugins/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      798 2023-04-10 01:56:10.000000 py4web-1.20230416.1/py4web/utils/auth_plugins/basic_auth_plugin.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     8154 2022-03-15 04:37:19.000000 py4web-1.20230416.1/py4web/utils/auth_plugins/cas_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1441 2023-04-10 01:56:10.000000 py4web-1.20230416.1/py4web/utils/auth_plugins/email_auth_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    35513 2023-04-10 03:57:06.000000 py4web-1.20230416.1/py4web/utils/auth_plugins/ldap_plugin.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     3563 2022-03-14 19:17:56.000000 py4web-1.20230416.1/py4web/utils/auth_plugins/newsamlplugin.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     1759 2022-02-21 23:58:14.000000 py4web-1.20230416.1/py4web/utils/auth_plugins/oauth2discord.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      654 2020-10-10 04:20:35.000000 py4web-1.20230416.1/py4web/utils/auth_plugins/oauth2facebook.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      514 2023-04-10 03:57:06.000000 py4web-1.20230416.1/py4web/utils/auth_plugins/oauth2github.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      524 2020-10-10 04:20:35.000000 py4web-1.20230416.1/py4web/utils/auth_plugins/oauth2google.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      489 2020-10-10 04:20:35.000000 py4web-1.20230416.1/py4web/utils/auth_plugins/oauth2okta.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2084 2022-03-20 01:46:38.000000 py4web-1.20230416.1/py4web/utils/auth_plugins/oauth2server.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6090 2022-03-20 01:46:38.000000 py4web-1.20230416.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5051 2022-03-20 01:46:38.000000 py4web-1.20230416.1/py4web/utils/auth_plugins/pam.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      187 2023-04-10 01:56:10.000000 py4web-1.20230416.1/py4web/utils/auth_plugins/pam_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6672 2022-03-20 01:46:38.000000 py4web-1.20230416.1/py4web/utils/auth_plugins/saml2_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2848 2022-03-20 01:46:38.000000 py4web-1.20230416.1/py4web/utils/auth_plugins/x509_auth_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      857 2022-03-20 01:46:38.000000 py4web-1.20230416.1/py4web/utils/cors.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1628 2023-01-11 05:50:14.000000 py4web-1.20230416.1/py4web/utils/dbstore.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2075 2022-03-20 01:46:38.000000 py4web-1.20230416.1/py4web/utils/downloader.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3142 2022-03-20 01:46:38.000000 py4web-1.20230416.1/py4web/utils/factories.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    35844 2023-04-15 18:09:37.000000 py4web-1.20230416.1/py4web/utils/form.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    68937 2023-04-10 02:55:45.000000 py4web-1.20230416.1/py4web/utils/grid.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1651 2022-06-08 06:27:50.000000 py4web-1.20230416.1/py4web/utils/jsonrpc.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    34865 2022-11-11 06:40:11.000000 py4web-1.20230416.1/py4web/utils/mailer.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     9196 2022-06-03 04:17:49.000000 py4web-1.20230416.1/py4web/utils/misc.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      502 2020-09-13 06:17:02.000000 py4web-1.20230416.1/py4web/utils/param.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    18269 2022-03-20 01:46:38.000000 py4web-1.20230416.1/py4web/utils/populate.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1694 2022-05-31 06:26:42.000000 py4web-1.20230416.1/py4web/utils/publisher.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2225 2023-03-19 21:28:12.000000 py4web-1.20230416.1/py4web/utils/recaptcha.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)    70958 2022-03-14 20:46:56.000000 py4web-1.20230416.1/py4web/utils/scheduler.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)    70958 2022-03-14 20:46:56.000000 py4web-1.20230416.1/py4web/utils/scheduler_old.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3728 2022-03-20 01:46:38.000000 py4web-1.20230416.1/py4web/utils/security.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      158 2022-03-20 01:46:38.000000 py4web-1.20230416.1/py4web/utils/tags.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6554 2023-04-15 18:18:02.000000 py4web-1.20230416.1/py4web/utils/url_signer.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 00:40:00.310947 py4web-1.20230416.1/py4web.egg-info/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      826 2023-04-17 00:40:00.000000 py4web-1.20230416.1/py4web.egg-info/PKG-INFO
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     1727 2023-04-17 00:40:00.000000 py4web-1.20230416.1/py4web.egg-info/SOURCES.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2023-04-17 00:40:00.000000 py4web-1.20230416.1/py4web.egg-info/dependency_links.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)       44 2023-04-17 00:40:00.000000 py4web-1.20230416.1/py4web.egg-info/entry_points.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2020-09-07 23:01:39.000000 py4web-1.20230416.1/py4web.egg-info/not-zip-safe
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      215 2023-04-17 00:40:00.000000 py4web-1.20230416.1/py4web.egg-info/requires.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)        7 2023-04-17 00:40:00.000000 py4web-1.20230416.1/py4web.egg-info/top_level.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-04-17 00:40:00.326947 py4web-1.20230416.1/setup.cfg
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1758 2023-03-12 23:37:12.000000 py4web-1.20230416.1/setup.py
```

### Comparing `py4web-1.20230410.2/PKG-INFO` & `py4web-1.20230416.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: py4web
-Version: 1.20230410.2
+Version: 1.20230416.1
 Summary: Experimental py4web (a better web2py)
 Home-page: https://github.com/web2py/py4web
 Author: Massimo Di Pierro
 Author-email: massimo.dipierro@gmail.com
 Maintainer: Massimo Di Pierro
 Maintainer-email: massimo.dipierro@gmail.com
 License: BSD
```

### Comparing `py4web-1.20230410.2/README.rst` & `py4web-1.20230416.1/README.rst`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/__init__.py` & `py4web-1.20230416.1/py4web/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 __author__ = "Massimo Di Pierro <massimo.dipierro@gmail.com>"
 __license__ = "BSDv3"
-__version__ = "1.20230410.2"
+__version__ = "1.20230416.1"
 
 
 def _maybe_gevent():
     for arg in sys.argv[1:]:
         if "gevent" in arg.lower():
             from gevent import monkey
```

### Comparing `py4web-1.20230410.2/py4web/assets/py4web.app._dashboard.zip` & `py4web-1.20230416.1/py4web/assets/py4web.app._dashboard.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/assets/py4web.app._default.zip` & `py4web-1.20230416.1/py4web/assets/py4web.app._default.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/assets/py4web.app._documentation.zip` & `py4web-1.20230416.1/py4web/assets/py4web.app._documentation.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/assets/py4web.app._scaffold.zip` & `py4web-1.20230416.1/py4web/assets/py4web.app._scaffold.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/assets/py4web.app.showcase.zip` & `py4web-1.20230416.1/py4web/assets/py4web.app.showcase.zip`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/core.py` & `py4web-1.20230416.1/py4web/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -960,15 +960,14 @@
 
     def __call__(self, func):
         """Building the decorator"""
         app_name = action.app_name
         if self.path[0] == "/":
             path = self.path.rstrip("/") or "/"
         else:
-
             base_path = "" if app_name == "_default" else f"/{app_name}"
             path = (f"{base_path}/{self.path}").rstrip("/")
         Reloader.register_route(app_name, path, self.kwargs, func)
         if path.endswith("/index"):  # /index is always optional
             short_path = path[:-6] or "/"
             Reloader.register_route(app_name, short_path, self.kwargs, func)
         return func
@@ -1272,15 +1271,19 @@
         folder = os.environ["PY4WEB_APPS_FOLDER"]
         # if first time reload dummy top module
         if not Reloader.MODULES:
             path = os.path.join(folder, "__init__.py")
             loader = importlib.machinery.SourceFileLoader("apps", path)
             loader.load_module()
         # Then load all the apps as submodules
-        for app_name in os.listdir(folder):
+        if os.environ.get("PY4WEB_APP_NAMES"):
+            app_names = os.environ.get("PY4WEB_APP_NAMES").split(",")
+        else:
+            app_names = os.listdir(folder)
+        for app_name in app_names:
             Reloader.import_app(app_name, clear_before_import=False)
 
     @staticmethod
     def import_app(app_name, clear_before_import=True):
         if clear_before_import:
             Reloader.clear_routes([app_name])
         Reloader.ROUTES[app_name] = []
@@ -1360,14 +1363,16 @@
             Reloader.register_route(app_name, path, {"method": "GET"}, server_static)
 
         ICECUBE.update(threadsafevariable.ThreadSafeVariable.freeze())
 
     @staticmethod
     def register_route(app_name, rule, kwargs, func):
         url_prefix = os.environ.get("PY4WEB_URL_PREFIX", "")
+        if url_prefix and rule == "/":
+            rule = ""
         dec_func = action.catch_errors(app_name, func)
         bottle.route(url_prefix + rule, **kwargs)(dec_func)
         filename = module2filename(func.__module__)
         methods = kwargs.get("method", ["GET"])
         if isinstance(methods, str):
             methods = [methods]
         for method in methods:
@@ -1895,14 +1900,20 @@
     show_default=True,
 )
 @click.option("-H", "--host", default="127.0.0.1", help="Host name", show_default=True)
 @click.option(
     "-P", "--port", default=8000, type=int, help="Port number", show_default=True
 )
 @click.option(
+    "-A",
+    "--app_names",
+    default="",
+    help="List of apps to run (all if omitted or empty)",
+)
+@click.option(
     "-p",
     "--password_file",
     default="password.txt",
     help="File for the encrypted password",
     show_default=True,
 )
 @click.option(
@@ -1983,28 +1994,29 @@
     install_args(kwargs)
 
     from py4web import __version__
 
     click.secho(ART, fg="blue")
     click.echo("Py4web: %s on Python %s\n\n" % (__version__, sys.version))
 
+    # Start
+    Reloader.import_apps()
+
     # If we know where the password is stored, read it, otherwise ask for one
     if os.path.exists(os.path.join(os.environ["PY4WEB_APPS_FOLDER"], "_dashboard")):
         if kwargs["dashboard_mode"] not in ("demo", "none") and not os.path.exists(
             kwargs["password_file"]
         ):
             click.echo(
                 'You have not set a dashboard password. Run "%s set_password" to do so.'
                 % PY4WEB_CMD
             )
-        else:
+        elif "_dashboard" in Reloader.ROUTES:
             click.echo(
                 f"Dashboard is at: http{'s' if kwargs.get('ssl_cert', None) else ''}://{kwargs['host']}:{kwargs['port']}/_dashboard"
             )
 
-    # Start
-    Reloader.import_apps()
     start_server(kwargs)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `py4web-1.20230410.2/py4web/server_adapters.py` & `py4web-1.20230416.1/py4web/server_adapters.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/auth.py` & `py4web-1.20230416.1/py4web/utils/auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/auth_plugins/__init__.py` & `py4web-1.20230416.1/py4web/utils/auth_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/auth_plugins/basic_auth_plugin.py` & `py4web-1.20230416.1/py4web/utils/auth_plugins/basic_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/auth_plugins/cas_plugin.py` & `py4web-1.20230416.1/py4web/utils/auth_plugins/cas_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/auth_plugins/email_auth_plugin.py` & `py4web-1.20230416.1/py4web/utils/auth_plugins/email_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/auth_plugins/ldap_plugin.py` & `py4web-1.20230416.1/py4web/utils/auth_plugins/ldap_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/auth_plugins/newsamlplugin.py` & `py4web-1.20230416.1/py4web/utils/auth_plugins/newsamlplugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/auth_plugins/oauth2discord.py` & `py4web-1.20230416.1/py4web/utils/auth_plugins/oauth2discord.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/auth_plugins/oauth2facebook.py` & `py4web-1.20230416.1/py4web/utils/auth_plugins/oauth2facebook.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/auth_plugins/oauth2github.py` & `py4web-1.20230416.1/py4web/utils/auth_plugins/oauth2github.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/auth_plugins/oauth2google.py` & `py4web-1.20230416.1/py4web/utils/auth_plugins/oauth2google.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/auth_plugins/oauth2server.py` & `py4web-1.20230416.1/py4web/utils/auth_plugins/oauth2server.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/auth_plugins/oauth2wpminiorange.py` & `py4web-1.20230416.1/py4web/utils/auth_plugins/oauth2wpminiorange.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/auth_plugins/pam.py` & `py4web-1.20230416.1/py4web/utils/auth_plugins/pam.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/auth_plugins/saml2_plugin.py` & `py4web-1.20230416.1/py4web/utils/auth_plugins/saml2_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/auth_plugins/x509_auth_plugin.py` & `py4web-1.20230416.1/py4web/utils/auth_plugins/x509_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/cors.py` & `py4web-1.20230416.1/py4web/utils/cors.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/dbstore.py` & `py4web-1.20230416.1/py4web/utils/dbstore.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/downloader.py` & `py4web-1.20230416.1/py4web/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/factories.py` & `py4web-1.20230416.1/py4web/utils/factories.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/form.py` & `py4web-1.20230416.1/py4web/utils/form.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,48 +345,29 @@
         class_info = self.classes["info"]
 
         all_fields = [x for x in table]
         if "_virtual_fields" in dir(table):
             all_fields += table._virtual_fields
         for field in all_fields:
 
-            # Reset the json control fields.
-            field_attributes = dict()
-            field_value = None
-
-            field_name = field.name
-            field_type = field.type
-            field_comment = field.comment if field.comment else ""
-            field_label = field.label
-            input_id = to_id(field)
-            if isinstance(field, FieldVirtual):
-                value = None
-            else:
-                value = vars.get(
-                    field.name,
-                    field.default() if callable(field.default) else field.default,
-                )
-            error = errors.get(field.name)
-            field_class = "type-" + field.type.split()[0].replace(":", "-")
-            placeholder = (
-                field._placeholder if "_placeholder" in field.__dict__ else None
-            )
-
-            title = field._title if "_title" in field.__dict__ else None
-            field_disabled = False
+            is_virtual = isinstance(field, FieldVirtual)
 
             # only display field if readable or writable
             if not field.readable and not field.writable:
                 continue
 
             # if this is a readonly field only show readable fields
             if readonly:
                 if not field.readable:
                     continue
 
+            # do not display virtual fields in edit forms
+            if not readonly and is_virtual:
+                continue
+
             # do not show the id if not desired
             if field.type == "id" and not show_id:
                 continue
 
             #  if this is an create form (unkown id) then only show writable fields.
             #  Some if an edit form was made from a list of fields and noncreate=True
             elif not vars.get("id") and noncreate:
@@ -394,34 +375,50 @@
                     continue
 
             # ignore blob fields
             if field.type == "blob":  # never display blobs (mistake?)
                 continue
 
             # ignore fields of type id its value is equal to None
-            if field.type == "id" and value is None:
+            if field.type == "id" and vars.get(field.name) is None:
                 field.writable = False
                 continue
 
+            # Reset the json control fields.
+            field_attributes = dict()
+            field_value = None
+
+            field_name = field.name
+            field_type = field.type
+            field_comment = field.comment if field.comment else ""
+            field_label = field.label
+            input_id = to_id(field)
+            default = field.default() if callable(field.default) else field.default
+            value = vars.get(field.name, default) if not is_virtual else None
+
+            error = errors.get(field.name)
+            field_class = "type-" + field.type.split()[0].replace(":", "-")
+            placeholder = (
+                field._placeholder if "_placeholder" in field.__dict__ else None
+            )
+
+            title = field._title if "_title" in field.__dict__ else None
+            field_disabled = False
+
             # if the form is readonly or this is an id type field, display it as readonly
-            if (
-                readonly
-                or not field.writable
-                or field.type == "id"
-                or isinstance(field, FieldVirtual)
-            ):
+            if readonly or not field.writable or field.type == "id" or is_virtual:
                 # for boolean readonly we use a readonly checbox
                 if field.type == "boolean":
 
                     control = CheckboxWidget().make(
                         field, value, error, title, readonly=True
                     )
                 # for all othe readonly fields we use represent or a string
                 else:
-                    if isinstance(field, FieldVirtual):
+                    if is_virtual:
                         field_value = field.f(vars)
                     else:
                         field_value = compat_represent(field, value, vars)
                     field_type = "represent"
                     control = DIV(field_value)
 
                 field_disabled = True
```

### Comparing `py4web-1.20230410.2/py4web/utils/grid.py` & `py4web-1.20230416.1/py4web/utils/grid.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/jsonrpc.py` & `py4web-1.20230416.1/py4web/utils/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/mailer.py` & `py4web-1.20230416.1/py4web/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/misc.py` & `py4web-1.20230416.1/py4web/utils/misc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/populate.py` & `py4web-1.20230416.1/py4web/utils/populate.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/publisher.py` & `py4web-1.20230416.1/py4web/utils/publisher.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/recaptcha.py` & `py4web-1.20230416.1/py4web/utils/recaptcha.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/scheduler.py` & `py4web-1.20230416.1/py4web/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/scheduler_old.py` & `py4web-1.20230416.1/py4web/utils/scheduler_old.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/security.py` & `py4web-1.20230416.1/py4web/utils/security.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/py4web/utils/url_signer.py` & `py4web-1.20230416.1/py4web/utils/url_signer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import base64
 import hashlib
 import json
+import os
 import time
 import uuid
 
 from py4web import HTTP, request
 from py4web.core import Fixture, Session
 
 
@@ -154,14 +155,17 @@
     def sign(self, url, variables):
         """Signs the URL"""
         for v in self.RESERVED_VARIABLES:
             assert v not in variables
         h = self.algo(self.get_key())
         ts = "%.3f" % time.time()
         salt = str(uuid.uuid1())
+        url_prefix = os.environ.get("PY4WEB_URL_PREFIX", "")
+        if url_prefix:
+            url = url_prefix + url
         h.update(self.get_info_to_sign(url, variables, ts, salt))
         sig = base64.b16encode(h.digest()).decode("utf-8")
         sig_content = json.dumps(dict(ts=ts, salt=salt, sig=sig))
         signature = base64.b16encode(sig_content.encode("utf-8")).decode("utf-8")
         variables["_signature"] = signature
 
     def verify(self):
```

### Comparing `py4web-1.20230410.2/py4web.egg-info/PKG-INFO` & `py4web-1.20230416.1/py4web.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: py4web
-Version: 1.20230410.2
+Version: 1.20230416.1
 Summary: Experimental py4web (a better web2py)
 Home-page: https://github.com/web2py/py4web
 Author: Massimo Di Pierro
 Author-email: massimo.dipierro@gmail.com
 Maintainer: Massimo Di Pierro
 Maintainer-email: massimo.dipierro@gmail.com
 License: BSD
```

### Comparing `py4web-1.20230410.2/py4web.egg-info/SOURCES.txt` & `py4web-1.20230416.1/py4web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4web-1.20230410.2/setup.py` & `py4web-1.20230416.1/setup.py`

 * *Files identical despite different names*

