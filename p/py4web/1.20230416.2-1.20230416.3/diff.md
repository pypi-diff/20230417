# Comparing `tmp/py4web-1.20230416.2.tar.gz` & `tmp/py4web-1.20230416.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-1.20230416.2.tar", last modified: Mon Apr 17 01:41:47 2023, max compression
+gzip compressed data, was "py4web-1.20230416.3.tar", last modified: Mon Apr 17 05:04:36 2023, max compression
```

## Comparing `py4web-1.20230416.2.tar` & `py4web-1.20230416.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 01:41:47.969790 py4web-1.20230416.2/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      826 2023-04-17 01:41:47.969790 py4web-1.20230416.2/PKG-INFO
--rw-r--r--   0 massimo   (1000) massimo   (1000)     7120 2022-01-11 05:54:38.000000 py4web-1.20230416.2/README.rst
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 01:41:47.949790 py4web-1.20230416.2/py4web/
--rw-r--r--   0 massimo   (1000) massimo   (1000)      721 2023-04-17 01:41:01.000000 py4web-1.20230416.2/py4web/__init__.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 01:41:47.961790 py4web-1.20230416.2/py4web/assets/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  2990826 2023-04-11 05:51:49.000000 py4web-1.20230416.2/py4web/assets/py4web.app._dashboard.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)   182307 2023-04-11 05:51:49.000000 py4web-1.20230416.2/py4web/assets/py4web.app._default.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  4278028 2023-04-11 05:51:50.000000 py4web-1.20230416.2/py4web/assets/py4web.app._documentation.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      409 2023-04-11 05:51:49.000000 py4web-1.20230416.2/py4web/assets/py4web.app._minimal.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    16674 2023-04-11 05:51:49.000000 py4web-1.20230416.2/py4web/assets/py4web.app._scaffold.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  1386102 2023-04-11 05:51:50.000000 py4web-1.20230416.2/py4web/assets/py4web.app.showcase.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    67378 2023-04-16 18:21:53.000000 py4web-1.20230416.2/py4web/core.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7510 2022-06-30 06:41:15.000000 py4web-1.20230416.2/py4web/server_adapters.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 01:41:47.965790 py4web-1.20230416.2/py4web/utils/
--rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2019-07-23 06:20:41.000000 py4web-1.20230416.2/py4web/utils/__init__.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)    69664 2023-04-10 05:23:42.000000 py4web-1.20230416.2/py4web/utils/auth.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 01:41:47.969790 py4web-1.20230416.2/py4web/utils/auth_plugins/
--rw-r--r--   0 massimo   (1000) massimo   (1000)     6207 2023-04-10 03:57:23.000000 py4web-1.20230416.2/py4web/utils/auth_plugins/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      798 2023-04-10 01:56:10.000000 py4web-1.20230416.2/py4web/utils/auth_plugins/basic_auth_plugin.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)     8154 2022-03-15 04:37:19.000000 py4web-1.20230416.2/py4web/utils/auth_plugins/cas_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1441 2023-04-10 01:56:10.000000 py4web-1.20230416.2/py4web/utils/auth_plugins/email_auth_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    35513 2023-04-10 03:57:06.000000 py4web-1.20230416.2/py4web/utils/auth_plugins/ldap_plugin.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)     3563 2022-03-14 19:17:56.000000 py4web-1.20230416.2/py4web/utils/auth_plugins/newsamlplugin.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)     1759 2022-02-21 23:58:14.000000 py4web-1.20230416.2/py4web/utils/auth_plugins/oauth2discord.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      654 2020-10-10 04:20:35.000000 py4web-1.20230416.2/py4web/utils/auth_plugins/oauth2facebook.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      514 2023-04-10 03:57:06.000000 py4web-1.20230416.2/py4web/utils/auth_plugins/oauth2github.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      524 2020-10-10 04:20:35.000000 py4web-1.20230416.2/py4web/utils/auth_plugins/oauth2google.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      489 2020-10-10 04:20:35.000000 py4web-1.20230416.2/py4web/utils/auth_plugins/oauth2okta.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2084 2022-03-20 01:46:38.000000 py4web-1.20230416.2/py4web/utils/auth_plugins/oauth2server.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6090 2022-03-20 01:46:38.000000 py4web-1.20230416.2/py4web/utils/auth_plugins/oauth2wpminiorange.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5051 2022-03-20 01:46:38.000000 py4web-1.20230416.2/py4web/utils/auth_plugins/pam.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      187 2023-04-10 01:56:10.000000 py4web-1.20230416.2/py4web/utils/auth_plugins/pam_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6672 2022-03-20 01:46:38.000000 py4web-1.20230416.2/py4web/utils/auth_plugins/saml2_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2848 2022-03-20 01:46:38.000000 py4web-1.20230416.2/py4web/utils/auth_plugins/x509_auth_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      857 2022-03-20 01:46:38.000000 py4web-1.20230416.2/py4web/utils/cors.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1628 2023-01-11 05:50:14.000000 py4web-1.20230416.2/py4web/utils/dbstore.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2075 2022-03-20 01:46:38.000000 py4web-1.20230416.2/py4web/utils/downloader.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3142 2022-03-20 01:46:38.000000 py4web-1.20230416.2/py4web/utils/factories.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    35844 2023-04-15 18:09:37.000000 py4web-1.20230416.2/py4web/utils/form.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    68937 2023-04-10 02:55:45.000000 py4web-1.20230416.2/py4web/utils/grid.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1651 2022-06-08 06:27:50.000000 py4web-1.20230416.2/py4web/utils/jsonrpc.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    34865 2022-11-11 06:40:11.000000 py4web-1.20230416.2/py4web/utils/mailer.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     9196 2022-06-03 04:17:49.000000 py4web-1.20230416.2/py4web/utils/misc.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      502 2020-09-13 06:17:02.000000 py4web-1.20230416.2/py4web/utils/param.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    18269 2022-03-20 01:46:38.000000 py4web-1.20230416.2/py4web/utils/populate.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1694 2022-05-31 06:26:42.000000 py4web-1.20230416.2/py4web/utils/publisher.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2225 2023-03-19 21:28:12.000000 py4web-1.20230416.2/py4web/utils/recaptcha.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)    70958 2022-03-14 20:46:56.000000 py4web-1.20230416.2/py4web/utils/scheduler.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)    70958 2022-03-14 20:46:56.000000 py4web-1.20230416.2/py4web/utils/scheduler_old.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3728 2022-03-20 01:46:38.000000 py4web-1.20230416.2/py4web/utils/security.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      158 2022-03-20 01:46:38.000000 py4web-1.20230416.2/py4web/utils/tags.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6554 2023-04-15 18:18:02.000000 py4web-1.20230416.2/py4web/utils/url_signer.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 01:41:47.949790 py4web-1.20230416.2/py4web.egg-info/
--rw-r--r--   0 massimo   (1000) massimo   (1000)      826 2023-04-17 01:41:47.000000 py4web-1.20230416.2/py4web.egg-info/PKG-INFO
--rw-r--r--   0 massimo   (1000) massimo   (1000)     1727 2023-04-17 01:41:47.000000 py4web-1.20230416.2/py4web.egg-info/SOURCES.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2023-04-17 01:41:47.000000 py4web-1.20230416.2/py4web.egg-info/dependency_links.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)       44 2023-04-17 01:41:47.000000 py4web-1.20230416.2/py4web.egg-info/entry_points.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2020-09-07 23:01:39.000000 py4web-1.20230416.2/py4web.egg-info/not-zip-safe
--rw-r--r--   0 massimo   (1000) massimo   (1000)      215 2023-04-17 01:41:47.000000 py4web-1.20230416.2/py4web.egg-info/requires.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)        7 2023-04-17 01:41:47.000000 py4web-1.20230416.2/py4web.egg-info/top_level.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-04-17 01:41:47.969790 py4web-1.20230416.2/setup.cfg
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1758 2023-03-12 23:37:12.000000 py4web-1.20230416.2/setup.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 05:04:36.818078 py4web-1.20230416.3/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      826 2023-04-17 05:04:36.818078 py4web-1.20230416.3/PKG-INFO
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     7120 2022-01-11 05:54:38.000000 py4web-1.20230416.3/README.rst
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 05:04:36.798077 py4web-1.20230416.3/py4web/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      721 2023-04-17 05:02:51.000000 py4web-1.20230416.3/py4web/__init__.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 05:04:36.810078 py4web-1.20230416.3/py4web/assets/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)  2995768 2023-04-17 05:03:22.000000 py4web-1.20230416.3/py4web/assets/py4web.app._dashboard.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)   187155 2023-04-17 05:03:22.000000 py4web-1.20230416.3/py4web/assets/py4web.app._default.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)  4287226 2023-04-17 05:03:23.000000 py4web-1.20230416.3/py4web/assets/py4web.app._documentation.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5245 2023-04-17 05:03:22.000000 py4web-1.20230416.3/py4web/assets/py4web.app._minimal.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    21524 2023-04-17 05:03:22.000000 py4web-1.20230416.3/py4web/assets/py4web.app._scaffold.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)  1392585 2023-04-17 05:03:23.000000 py4web-1.20230416.3/py4web/assets/py4web.app.showcase.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    67378 2023-04-16 18:21:53.000000 py4web-1.20230416.3/py4web/core.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     7510 2022-06-30 06:41:15.000000 py4web-1.20230416.3/py4web/server_adapters.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 05:04:36.814077 py4web-1.20230416.3/py4web/utils/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2019-07-23 06:20:41.000000 py4web-1.20230416.3/py4web/utils/__init__.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)    69664 2023-04-10 05:23:42.000000 py4web-1.20230416.3/py4web/utils/auth.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 05:04:36.818078 py4web-1.20230416.3/py4web/utils/auth_plugins/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     6207 2023-04-10 03:57:23.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      798 2023-04-10 01:56:10.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/basic_auth_plugin.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     8154 2022-03-15 04:37:19.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/cas_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1441 2023-04-10 01:56:10.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/email_auth_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    35513 2023-04-10 03:57:06.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/ldap_plugin.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     3563 2022-03-14 19:17:56.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/newsamlplugin.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     1759 2022-02-21 23:58:14.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2discord.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      654 2020-10-10 04:20:35.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2facebook.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      514 2023-04-10 03:57:06.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2github.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      524 2020-10-10 04:20:35.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2google.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      489 2020-10-10 04:20:35.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2okta.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2084 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2server.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6090 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2wpminiorange.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5051 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/pam.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      187 2023-04-10 01:56:10.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/pam_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6672 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/saml2_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2848 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/auth_plugins/x509_auth_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      857 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/cors.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1628 2023-01-11 05:50:14.000000 py4web-1.20230416.3/py4web/utils/dbstore.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2075 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/downloader.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3142 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/factories.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    35844 2023-04-15 18:09:37.000000 py4web-1.20230416.3/py4web/utils/form.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    68937 2023-04-10 02:55:45.000000 py4web-1.20230416.3/py4web/utils/grid.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1651 2022-06-08 06:27:50.000000 py4web-1.20230416.3/py4web/utils/jsonrpc.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    34865 2022-11-11 06:40:11.000000 py4web-1.20230416.3/py4web/utils/mailer.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     9196 2022-06-03 04:17:49.000000 py4web-1.20230416.3/py4web/utils/misc.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      502 2020-09-13 06:17:02.000000 py4web-1.20230416.3/py4web/utils/param.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    18269 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/populate.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1694 2022-05-31 06:26:42.000000 py4web-1.20230416.3/py4web/utils/publisher.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2225 2023-03-19 21:28:12.000000 py4web-1.20230416.3/py4web/utils/recaptcha.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)    70958 2022-03-14 20:46:56.000000 py4web-1.20230416.3/py4web/utils/scheduler.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)    70958 2022-03-14 20:46:56.000000 py4web-1.20230416.3/py4web/utils/scheduler_old.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3728 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/security.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      158 2022-03-20 01:46:38.000000 py4web-1.20230416.3/py4web/utils/tags.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6554 2023-04-15 18:18:02.000000 py4web-1.20230416.3/py4web/utils/url_signer.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-17 05:04:36.798077 py4web-1.20230416.3/py4web.egg-info/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      826 2023-04-17 05:04:36.000000 py4web-1.20230416.3/py4web.egg-info/PKG-INFO
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     1727 2023-04-17 05:04:36.000000 py4web-1.20230416.3/py4web.egg-info/SOURCES.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2023-04-17 05:04:36.000000 py4web-1.20230416.3/py4web.egg-info/dependency_links.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)       44 2023-04-17 05:04:36.000000 py4web-1.20230416.3/py4web.egg-info/entry_points.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2020-09-07 23:01:39.000000 py4web-1.20230416.3/py4web.egg-info/not-zip-safe
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      215 2023-04-17 05:04:36.000000 py4web-1.20230416.3/py4web.egg-info/requires.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)        7 2023-04-17 05:04:36.000000 py4web-1.20230416.3/py4web.egg-info/top_level.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-04-17 05:04:36.818078 py4web-1.20230416.3/setup.cfg
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1758 2023-03-12 23:37:12.000000 py4web-1.20230416.3/setup.py
```

### Comparing `py4web-1.20230416.2/PKG-INFO` & `py4web-1.20230416.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: py4web
-Version: 1.20230416.2
+Version: 1.20230416.3
 Summary: Experimental py4web (a better web2py)
 Home-page: https://github.com/web2py/py4web
 Author: Massimo Di Pierro
 Author-email: massimo.dipierro@gmail.com
 Maintainer: Massimo Di Pierro
 Maintainer-email: massimo.dipierro@gmail.com
 License: BSD
```

### Comparing `py4web-1.20230416.2/README.rst` & `py4web-1.20230416.3/README.rst`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/__init__.py` & `py4web-1.20230416.3/py4web/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 __author__ = "Massimo Di Pierro <massimo.dipierro@gmail.com>"
 __license__ = "BSDv3"
-__version__ = "1.20230416.2"
+__version__ = "1.20230416.3"
 
 
 def _maybe_gevent():
     for arg in sys.argv[1:]:
         if "gevent" in arg.lower():
             from gevent import monkey
```

### Comparing `py4web-1.20230416.2/py4web/assets/py4web.app._dashboard.zip` & `py4web-1.20230416.3/py4web/assets/py4web.app._dashboard.zip`

 * *Files 6% similar despite different names*

#### zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                   2990826 (00000000002DA2EAh)
-  Actual end-cent-dir record offset:       2990804 (00000000002DA2D4h)
-  Expected end-cent-dir record offset:     2990804 (00000000002DA2D4h)
+  Zip archive file size:                   2995768 (00000000002DB638h)
+  Actual end-cent-dir record offset:       2995746 (00000000002DB622h)
+  Expected end-cent-dir record offset:     2995746 (00000000002DB622h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 378 entries.
-  The central directory is 37654 (0000000000009316h) bytes long,
+  central directory contains 379 entries.
+  The central directory is 37742 (000000000000936Eh) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 2953150 (00000000002D0FBEh).
+  is 2958004 (00000000002D22B4h).
 
 
 Central directory entry #1:
 ---------------------------
 
   utils.py
 
@@ -63,20 +63,20 @@
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Apr 12 23:23:02
-  file last modified on (UT extra field modtime): 2022 Apr 13 06:23:02 local
-  file last modified on (UT extra field modtime): 2022 Apr 13 06:23:02 UTC
-  32-bit CRC value (hex):                         125ea65e
-  compressed size:                                2263 bytes
-  uncompressed size:                              8304 bytes
+  file last modified on (DOS date/time):          2023 Apr 16 17:32:04
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:32:03 local
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:32:03 UTC
+  32-bit CRC value (hex):                         8155e653
+  compressed size:                                2245 bytes
+  uncompressed size:                              8097 bytes
   length of filename:                             27 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
@@ -90,36 +90,36 @@
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
   static/components/mtable.html
 
-  offset of local header from start of archive:   3897
-                                                  (0000000000000F39h) bytes
+  offset of local header from start of archive:   3879
+                                                  (0000000000000F27h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2021 Sep 26 23:28:08
-  file last modified on (UT extra field modtime): 2021 Sep 27 06:28:08 local
-  file last modified on (UT extra field modtime): 2021 Sep 27 06:28:08 UTC
-  32-bit CRC value (hex):                         8146daa4
-  compressed size:                                1579 bytes
-  uncompressed size:                              7597 bytes
+  file last modified on (DOS date/time):          2023 Apr 16 17:08:16
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:08:15 local
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:08:15 UTC
+  32-bit CRC value (hex):                         9bb8ce4d
+  compressed size:                                1582 bytes
+  uncompressed size:                              7447 bytes
   length of filename:                             29 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
   The central-directory extra field contains:
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
@@ -127,16 +127,16 @@
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
   static/images/alert-red.gif
 
-  offset of local header from start of archive:   5563
-                                                  (00000000000015BBh) bytes
+  offset of local header from start of archive:   5548
+                                                  (00000000000015ACh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -164,16 +164,16 @@
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
   static/images/alert-blue.gif
 
-  offset of local header from start of archive:   17026
-                                                  (0000000000004282h) bytes
+  offset of local header from start of archive:   17011
+                                                  (0000000000004273h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -201,16 +201,16 @@
   There is no file comment.
 
 Central directory entry #6:
 ---------------------------
 
   static/images/alert-orange.gif
 
-  offset of local header from start of archive:   28722
-                                                  (0000000000007032h) bytes
+  offset of local header from start of archive:   28707
+                                                  (0000000000007023h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -238,16 +238,16 @@
   There is no file comment.
 
 Central directory entry #7:
 ---------------------------
 
   static/images/widget.gif
 
-  offset of local header from start of archive:   41280
-                                                  (000000000000A140h) bytes
+  offset of local header from start of archive:   41265
+                                                  (000000000000A131h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -275,16 +275,16 @@
   There is no file comment.
 
 Central directory entry #8:
 ---------------------------
 
   static/images/forkme.png
 
-  offset of local header from start of archive:   1042954
-                                                  (00000000000FEA0Ah) bytes
+  offset of local header from start of archive:   1042939
+                                                  (00000000000FE9FBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -312,16 +312,16 @@
   There is no file comment.
 
 Central directory entry #9:
 ---------------------------
 
   static/images/alert-yellow.gif
 
-  offset of local header from start of archive:   1050959
-                                                  (000000000010094Fh) bytes
+  offset of local header from start of archive:   1050944
+                                                  (0000000000100940h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -349,16 +349,16 @@
   There is no file comment.
 
 Central directory entry #10:
 ---------------------------
 
   static/images/alert-green.gif
 
-  offset of local header from start of archive:   1063688
-                                                  (0000000000103B08h) bytes
+  offset of local header from start of archive:   1063673
+                                                  (0000000000103AF9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -386,30 +386,30 @@
   There is no file comment.
 
 Central directory entry #11:
 ---------------------------
 
   static/css/future.css
 
-  offset of local header from start of archive:   1074401
-                                                  (00000000001064E1h) bytes
+  offset of local header from start of archive:   1074386
+                                                  (00000000001064D2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Jul 19 06:20:36
-  file last modified on (UT extra field modtime): 2022 Jul 19 13:20:36 local
-  file last modified on (UT extra field modtime): 2022 Jul 19 13:20:36 UTC
-  32-bit CRC value (hex):                         7fdd6812
-  compressed size:                                1670 bytes
-  uncompressed size:                              5744 bytes
+  file last modified on (DOS date/time):          2023 Apr 16 17:28:22
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:28:22 local
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:28:22 UTC
+  32-bit CRC value (hex):                         3eb4c4c1
+  compressed size:                                1721 bytes
+  uncompressed size:                              5926 bytes
   length of filename:                             21 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -423,16 +423,16 @@
   There is no file comment.
 
 Central directory entry #12:
 ---------------------------
 
   static/css/gitlog.min.css
 
-  offset of local header from start of archive:   1076150
-                                                  (0000000000106BB6h) bytes
+  offset of local header from start of archive:   1076186
+                                                  (0000000000106BDAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -460,16 +460,16 @@
   There is no file comment.
 
 Central directory entry #13:
 ---------------------------
 
   static/js/index.js
 
-  offset of local header from start of archive:   1076548
-                                                  (0000000000106D44h) bytes
+  offset of local header from start of archive:   1076584
+                                                  (0000000000106D68h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -497,16 +497,16 @@
   There is no file comment.
 
 Central directory entry #14:
 ---------------------------
 
   static/js/translations.js
 
-  offset of local header from start of archive:   1079351
-                                                  (0000000000107837h) bytes
+  offset of local header from start of archive:   1079387
+                                                  (000000000010785Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -534,16 +534,16 @@
   There is no file comment.
 
 Central directory entry #15:
 ---------------------------
 
   static/js/sugar.min.js
 
-  offset of local header from start of archive:   1080317
-                                                  (0000000000107BFDh) bytes
+  offset of local header from start of archive:   1080353
+                                                  (0000000000107C21h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -571,16 +571,16 @@
   There is no file comment.
 
 Central directory entry #16:
 ---------------------------
 
   static/js/ace/mode-d.js
 
-  offset of local header from start of archive:   1105501
-                                                  (000000000010DE5Dh) bytes
+  offset of local header from start of archive:   1105537
+                                                  (000000000010DE81h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -608,16 +608,16 @@
   There is no file comment.
 
 Central directory entry #17:
 ---------------------------
 
   static/js/ace/mode-php.js
 
-  offset of local header from start of archive:   1108770
-                                                  (000000000010EB22h) bytes
+  offset of local header from start of archive:   1108806
+                                                  (000000000010EB46h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -645,16 +645,16 @@
   There is no file comment.
 
 Central directory entry #18:
 ---------------------------
 
   static/js/ace/mode-rust.js
 
-  offset of local header from start of archive:   1226216
-                                                  (000000000012B5E8h) bytes
+  offset of local header from start of archive:   1226252
+                                                  (000000000012B60Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -682,16 +682,16 @@
   There is no file comment.
 
 Central directory entry #19:
 ---------------------------
 
   static/js/ace/mode-elm.js
 
-  offset of local header from start of archive:   1228828
-                                                  (000000000012C01Ch) bytes
+  offset of local header from start of archive:   1228864
+                                                  (000000000012C040h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -719,16 +719,16 @@
   There is no file comment.
 
 Central directory entry #20:
 ---------------------------
 
   static/js/ace/ext-elastic_tabstops_lite.js
 
-  offset of local header from start of archive:   1230765
-                                                  (000000000012C7ADh) bytes
+  offset of local header from start of archive:   1230801
+                                                  (000000000012C7D1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -756,16 +756,16 @@
   There is no file comment.
 
 Central directory entry #21:
 ---------------------------
 
   static/js/ace/mode-curly.js
 
-  offset of local header from start of archive:   1232320
-                                                  (000000000012CDC0h) bytes
+  offset of local header from start of archive:   1232356
+                                                  (000000000012CDE4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -793,16 +793,16 @@
   There is no file comment.
 
 Central directory entry #22:
 ---------------------------
 
   static/js/ace/theme-mono_industrial.js
 
-  offset of local header from start of archive:   1249567
-                                                  (000000000013111Fh) bytes
+  offset of local header from start of archive:   1249603
+                                                  (0000000000131143h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -830,16 +830,16 @@
   There is no file comment.
 
 Central directory entry #23:
 ---------------------------
 
   static/js/ace/theme-textmate.js
 
-  offset of local header from start of archive:   1250533
-                                                  (00000000001314E5h) bytes
+  offset of local header from start of archive:   1250569
+                                                  (0000000000131509h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -867,16 +867,16 @@
   There is no file comment.
 
 Central directory entry #24:
 ---------------------------
 
   static/js/ace/theme-chrome.js
 
-  offset of local header from start of archive:   1251562
-                                                  (00000000001318EAh) bytes
+  offset of local header from start of archive:   1251598
+                                                  (000000000013190Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -904,16 +904,16 @@
   There is no file comment.
 
 Central directory entry #25:
 ---------------------------
 
   static/js/ace/mode-rhtml.js
 
-  offset of local header from start of archive:   1252596
-                                                  (0000000000131CF4h) bytes
+  offset of local header from start of archive:   1252632
+                                                  (0000000000131D18h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -941,16 +941,16 @@
   There is no file comment.
 
 Central directory entry #26:
 ---------------------------
 
   static/js/ace/mode-r.js
 
-  offset of local header from start of archive:   1270901
-                                                  (0000000000136475h) bytes
+  offset of local header from start of archive:   1270937
+                                                  (0000000000136499h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -978,16 +978,16 @@
   There is no file comment.
 
 Central directory entry #27:
 ---------------------------
 
   static/js/ace/mode-ada.js
 
-  offset of local header from start of archive:   1272539
-                                                  (0000000000136ADBh) bytes
+  offset of local header from start of archive:   1272575
+                                                  (0000000000136AFFh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1015,16 +1015,16 @@
   There is no file comment.
 
 Central directory entry #28:
 ---------------------------
 
   static/js/ace/mode-pascal.js
 
-  offset of local header from start of archive:   1273476
-                                                  (0000000000136E84h) bytes
+  offset of local header from start of archive:   1273512
+                                                  (0000000000136EA8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1052,16 +1052,16 @@
   There is no file comment.
 
 Central directory entry #29:
 ---------------------------
 
   static/js/ace/mode-ftl.js
 
-  offset of local header from start of archive:   1275095
-                                                  (00000000001374D7h) bytes
+  offset of local header from start of archive:   1275131
+                                                  (00000000001374FBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1089,16 +1089,16 @@
   There is no file comment.
 
 Central directory entry #30:
 ---------------------------
 
   static/js/ace/ext-beautify.js
 
-  offset of local header from start of archive:   1284771
-                                                  (0000000000139AA3h) bytes
+  offset of local header from start of archive:   1284807
+                                                  (0000000000139AC7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1126,16 +1126,16 @@
   There is no file comment.
 
 Central directory entry #31:
 ---------------------------
 
   static/js/ace/mode-gcode.js
 
-  offset of local header from start of archive:   1286076
-                                                  (0000000000139FBCh) bytes
+  offset of local header from start of archive:   1286112
+                                                  (0000000000139FE0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1163,16 +1163,16 @@
   There is no file comment.
 
 Central directory entry #32:
 ---------------------------
 
   static/js/ace/worker-xquery.js
 
-  offset of local header from start of archive:   1286810
-                                                  (000000000013A29Ah) bytes
+  offset of local header from start of archive:   1286846
+                                                  (000000000013A2BEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1200,16 +1200,16 @@
   There is no file comment.
 
 Central directory entry #33:
 ---------------------------
 
   static/js/ace/mode-jade.js
 
-  offset of local header from start of archive:   1477019
-                                                  (000000000016899Bh) bytes
+  offset of local header from start of archive:   1477055
+                                                  (00000000001689BFh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1237,16 +1237,16 @@
   There is no file comment.
 
 Central directory entry #34:
 ---------------------------
 
   static/js/ace/mode-less.js
 
-  offset of local header from start of archive:   1490865
-                                                  (000000000016BFB1h) bytes
+  offset of local header from start of archive:   1490901
+                                                  (000000000016BFD5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1274,16 +1274,16 @@
   There is no file comment.
 
 Central directory entry #35:
 ---------------------------
 
   static/js/ace/mode-autohotkey.js
 
-  offset of local header from start of archive:   1497376
-                                                  (000000000016D920h) bytes
+  offset of local header from start of archive:   1497412
+                                                  (000000000016D944h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1311,16 +1311,16 @@
   There is no file comment.
 
 Central directory entry #36:
 ---------------------------
 
   static/js/ace/mode-mipsassembler.js
 
-  offset of local header from start of archive:   1514116
-                                                  (0000000000171A84h) bytes
+  offset of local header from start of archive:   1514152
+                                                  (0000000000171AA8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1348,16 +1348,16 @@
   There is no file comment.
 
 Central directory entry #37:
 ---------------------------
 
   static/js/ace/ext-static_highlight.js
 
-  offset of local header from start of archive:   1515333
-                                                  (0000000000171F45h) bytes
+  offset of local header from start of archive:   1515369
+                                                  (0000000000171F69h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1385,16 +1385,16 @@
   There is no file comment.
 
 Central directory entry #38:
 ---------------------------
 
   static/js/ace/mode-text.js
 
-  offset of local header from start of archive:   1516770
-                                                  (00000000001724E2h) bytes
+  offset of local header from start of archive:   1516806
+                                                  (0000000000172506h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -1421,16 +1421,16 @@
   There is no file comment.
 
 Central directory entry #39:
 ---------------------------
 
   static/js/ace/mode-diff.js
 
-  offset of local header from start of archive:   1516854
-                                                  (0000000000172536h) bytes
+  offset of local header from start of archive:   1516890
+                                                  (000000000017255Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1458,16 +1458,16 @@
   There is no file comment.
 
 Central directory entry #40:
 ---------------------------
 
   static/js/ace/mode-space.js
 
-  offset of local header from start of archive:   1517820
-                                                  (00000000001728FCh) bytes
+  offset of local header from start of archive:   1517856
+                                                  (0000000000172920h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1495,16 +1495,16 @@
   There is no file comment.
 
 Central directory entry #41:
 ---------------------------
 
   static/js/ace/mode-cobol.js
 
-  offset of local header from start of archive:   1518671
-                                                  (0000000000172C4Fh) bytes
+  offset of local header from start of archive:   1518707
+                                                  (0000000000172C73h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1532,16 +1532,16 @@
   There is no file comment.
 
 Central directory entry #42:
 ---------------------------
 
   static/js/ace/ext-split.js
 
-  offset of local header from start of archive:   1519967
-                                                  (000000000017315Fh) bytes
+  offset of local header from start of archive:   1520003
+                                                  (0000000000173183h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1569,16 +1569,16 @@
   There is no file comment.
 
 Central directory entry #43:
 ---------------------------
 
   static/js/ace/mode-rst.js
 
-  offset of local header from start of archive:   1521392
-                                                  (00000000001736F0h) bytes
+  offset of local header from start of archive:   1521428
+                                                  (0000000000173714h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1606,16 +1606,16 @@
   There is no file comment.
 
 Central directory entry #44:
 ---------------------------
 
   static/js/ace/theme-tomorrow_night_blue.js
 
-  offset of local header from start of archive:   1522446
-                                                  (0000000000173B0Eh) bytes
+  offset of local header from start of archive:   1522482
+                                                  (0000000000173B32h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1643,16 +1643,16 @@
   There is no file comment.
 
 Central directory entry #45:
 ---------------------------
 
   static/js/ace/mode-mask.js
 
-  offset of local header from start of archive:   1523406
-                                                  (0000000000173ECEh) bytes
+  offset of local header from start of archive:   1523442
+                                                  (0000000000173EF2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1680,16 +1680,16 @@
   There is no file comment.
 
 Central directory entry #46:
 ---------------------------
 
   static/js/ace/mode-sqlserver.js
 
-  offset of local header from start of archive:   1535895
-                                                  (0000000000176F97h) bytes
+  offset of local header from start of archive:   1535931
+                                                  (0000000000176FBBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1717,16 +1717,16 @@
   There is no file comment.
 
 Central directory entry #47:
 ---------------------------
 
   static/js/ace/mode-yaml.js
 
-  offset of local header from start of archive:   1542458
-                                                  (000000000017893Ah) bytes
+  offset of local header from start of archive:   1542494
+                                                  (000000000017895Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1754,16 +1754,16 @@
   There is no file comment.
 
 Central directory entry #48:
 ---------------------------
 
   static/js/ace/theme-tomorrow.js
 
-  offset of local header from start of archive:   1543963
-                                                  (0000000000178F1Bh) bytes
+  offset of local header from start of archive:   1543999
+                                                  (0000000000178F3Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1791,16 +1791,16 @@
   There is no file comment.
 
 Central directory entry #49:
 ---------------------------
 
   static/js/ace/mode-actionscript.js
 
-  offset of local header from start of archive:   1544889
-                                                  (00000000001792B9h) bytes
+  offset of local header from start of archive:   1544925
+                                                  (00000000001792DDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1828,16 +1828,16 @@
   There is no file comment.
 
 Central directory entry #50:
 ---------------------------
 
   static/js/ace/mode-twig.js
 
-  offset of local header from start of archive:   1552978
-                                                  (000000000017B252h) bytes
+  offset of local header from start of archive:   1553014
+                                                  (000000000017B276h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1865,16 +1865,16 @@
   There is no file comment.
 
 Central directory entry #51:
 ---------------------------
 
   static/js/ace/mode-golang.js
 
-  offset of local header from start of archive:   1571065
-                                                  (000000000017F8F9h) bytes
+  offset of local header from start of archive:   1571101
+                                                  (000000000017F91Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1902,16 +1902,16 @@
   There is no file comment.
 
 Central directory entry #52:
 ---------------------------
 
   static/js/ace/worker-json.js
 
-  offset of local header from start of archive:   1573637
-                                                  (0000000000180305h) bytes
+  offset of local header from start of archive:   1573673
+                                                  (0000000000180329h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1939,16 +1939,16 @@
   There is no file comment.
 
 Central directory entry #53:
 ---------------------------
 
   static/js/ace/ext-modelist.js
 
-  offset of local header from start of archive:   1583373
-                                                  (000000000018290Dh) bytes
+  offset of local header from start of archive:   1583409
+                                                  (0000000000182931h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1976,16 +1976,16 @@
   There is no file comment.
 
 Central directory entry #54:
 ---------------------------
 
   static/js/ace/mode-textile.js
 
-  offset of local header from start of archive:   1585413
-                                                  (0000000000183105h) bytes
+  offset of local header from start of archive:   1585449
+                                                  (0000000000183129h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2013,16 +2013,16 @@
   There is no file comment.
 
 Central directory entry #55:
 ---------------------------
 
   static/js/ace/mode-tcl.js
 
-  offset of local header from start of archive:   1586273
-                                                  (0000000000183461h) bytes
+  offset of local header from start of archive:   1586309
+                                                  (0000000000183485h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2050,16 +2050,16 @@
   There is no file comment.
 
 Central directory entry #56:
 ---------------------------
 
   static/js/ace/mode-smarty.js
 
-  offset of local header from start of archive:   1588246
-                                                  (0000000000183C16h) bytes
+  offset of local header from start of archive:   1588282
+                                                  (0000000000183C3Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2087,16 +2087,16 @@
   There is no file comment.
 
 Central directory entry #57:
 ---------------------------
 
   static/js/ace/theme-dreamweaver.js
 
-  offset of local header from start of archive:   1606250
-                                                  (000000000018826Ah) bytes
+  offset of local header from start of archive:   1606286
+                                                  (000000000018828Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2124,16 +2124,16 @@
   There is no file comment.
 
 Central directory entry #58:
 ---------------------------
 
   static/js/ace/mode-c9search.js
 
-  offset of local header from start of archive:   1607292
-                                                  (000000000018867Ch) bytes
+  offset of local header from start of archive:   1607328
+                                                  (00000000001886A0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2161,16 +2161,16 @@
   There is no file comment.
 
 Central directory entry #59:
 ---------------------------
 
   static/js/ace/mode-kotlin.js
 
-  offset of local header from start of archive:   1608918
-                                                  (0000000000188CD6h) bytes
+  offset of local header from start of archive:   1608954
+                                                  (0000000000188CFAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2198,16 +2198,16 @@
   There is no file comment.
 
 Central directory entry #60:
 ---------------------------
 
   static/js/ace/theme-solarized_dark.js
 
-  offset of local header from start of archive:   1611761
-                                                  (00000000001897F1h) bytes
+  offset of local header from start of archive:   1611797
+                                                  (0000000000189815h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2235,16 +2235,16 @@
   There is no file comment.
 
 Central directory entry #61:
 ---------------------------
 
   static/js/ace/worker-xml.js
 
-  offset of local header from start of archive:   1612658
-                                                  (0000000000189B72h) bytes
+  offset of local header from start of archive:   1612694
+                                                  (0000000000189B96h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2272,16 +2272,16 @@
   There is no file comment.
 
 Central directory entry #62:
 ---------------------------
 
   static/js/ace/mode-eiffel.js
 
-  offset of local header from start of archive:   1629501
-                                                  (000000000018DD3Dh) bytes
+  offset of local header from start of archive:   1629537
+                                                  (000000000018DD61h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2309,16 +2309,16 @@
   There is no file comment.
 
 Central directory entry #63:
 ---------------------------
 
   static/js/ace/worker-css.js
 
-  offset of local header from start of archive:   1630690
-                                                  (000000000018E1E2h) bytes
+  offset of local header from start of archive:   1630726
+                                                  (000000000018E206h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2346,16 +2346,16 @@
   There is no file comment.
 
 Central directory entry #64:
 ---------------------------
 
   static/js/ace/theme-clouds.js
 
-  offset of local header from start of archive:   1667458
-                                                  (0000000000197182h) bytes
+  offset of local header from start of archive:   1667494
+                                                  (00000000001971A6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2383,16 +2383,16 @@
   There is no file comment.
 
 Central directory entry #65:
 ---------------------------
 
   static/js/ace/mode-sjs.js
 
-  offset of local header from start of archive:   1668313
-                                                  (00000000001974D9h) bytes
+  offset of local header from start of archive:   1668349
+                                                  (00000000001974FDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2420,16 +2420,16 @@
   There is no file comment.
 
 Central directory entry #66:
 ---------------------------
 
   static/js/ace/mode-dockerfile.js
 
-  offset of local header from start of archive:   1675279
-                                                  (000000000019900Fh) bytes
+  offset of local header from start of archive:   1675315
+                                                  (0000000000199033h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2457,16 +2457,16 @@
   There is no file comment.
 
 Central directory entry #67:
 ---------------------------
 
   static/js/ace/mode-scheme.js
 
-  offset of local header from start of archive:   1678304
-                                                  (0000000000199BE0h) bytes
+  offset of local header from start of archive:   1678340
+                                                  (0000000000199C04h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2494,16 +2494,16 @@
   There is no file comment.
 
 Central directory entry #68:
 ---------------------------
 
   static/js/ace/mode-live_script.js
 
-  offset of local header from start of archive:   1679842
-                                                  (000000000019A1E2h) bytes
+  offset of local header from start of archive:   1679878
+                                                  (000000000019A206h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2531,16 +2531,16 @@
   There is no file comment.
 
 Central directory entry #69:
 ---------------------------
 
   static/js/ace/mode-jsoniq.js
 
-  offset of local header from start of archive:   1685099
-                                                  (000000000019B66Bh) bytes
+  offset of local header from start of archive:   1685135
+                                                  (000000000019B68Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2568,16 +2568,16 @@
   There is no file comment.
 
 Central directory entry #70:
 ---------------------------
 
   static/js/ace/mode-haxe.js
 
-  offset of local header from start of archive:   1721424
-                                                  (00000000001A4450h) bytes
+  offset of local header from start of archive:   1721460
+                                                  (00000000001A4474h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2605,16 +2605,16 @@
   There is no file comment.
 
 Central directory entry #71:
 ---------------------------
 
   static/js/ace/mode-wollok.js
 
-  offset of local header from start of archive:   1723837
-                                                  (00000000001A4DBDh) bytes
+  offset of local header from start of archive:   1723873
+                                                  (00000000001A4DE1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2642,16 +2642,16 @@
   There is no file comment.
 
 Central directory entry #72:
 ---------------------------
 
   static/js/ace/theme-katzenmilch.js
 
-  offset of local header from start of archive:   1730732
-                                                  (00000000001A68ACh) bytes
+  offset of local header from start of archive:   1730768
+                                                  (00000000001A68D0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2679,16 +2679,16 @@
   There is no file comment.
 
 Central directory entry #73:
 ---------------------------
 
   static/js/ace/theme-iplastic.js
 
-  offset of local header from start of archive:   1731764
-                                                  (00000000001A6CB4h) bytes
+  offset of local header from start of archive:   1731800
+                                                  (00000000001A6CD8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2716,16 +2716,16 @@
   There is no file comment.
 
 Central directory entry #74:
 ---------------------------
 
   static/js/ace/mode-perl.js
 
-  offset of local header from start of archive:   1735667
-                                                  (00000000001A7BF3h) bytes
+  offset of local header from start of archive:   1735703
+                                                  (00000000001A7C17h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2753,16 +2753,16 @@
   There is no file comment.
 
 Central directory entry #75:
 ---------------------------
 
   static/js/ace/keybinding-emacs.js
 
-  offset of local header from start of archive:   1738615
-                                                  (00000000001A8777h) bytes
+  offset of local header from start of archive:   1738651
+                                                  (00000000001A879Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2790,16 +2790,16 @@
   There is no file comment.
 
 Central directory entry #76:
 ---------------------------
 
   static/js/ace/mode-elixir.js
 
-  offset of local header from start of archive:   1745675
-                                                  (00000000001AA30Bh) bytes
+  offset of local header from start of archive:   1745711
+                                                  (00000000001AA32Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2827,16 +2827,16 @@
   There is no file comment.
 
 Central directory entry #77:
 ---------------------------
 
   static/js/ace/mode-gherkin.js
 
-  offset of local header from start of archive:   1748997
-                                                  (00000000001AB005h) bytes
+  offset of local header from start of archive:   1749033
+                                                  (00000000001AB029h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2864,16 +2864,16 @@
   There is no file comment.
 
 Central directory entry #78:
 ---------------------------
 
   static/js/ace/mode-java.js
 
-  offset of local header from start of archive:   1749991
-                                                  (00000000001AB3E7h) bytes
+  offset of local header from start of archive:   1750027
+                                                  (00000000001AB40Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2901,16 +2901,16 @@
   There is no file comment.
 
 Central directory entry #79:
 ---------------------------
 
   static/js/ace/mode-jsp.js
 
-  offset of local header from start of archive:   1757456
-                                                  (00000000001AD110h) bytes
+  offset of local header from start of archive:   1757492
+                                                  (00000000001AD134h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2938,16 +2938,16 @@
   There is no file comment.
 
 Central directory entry #80:
 ---------------------------
 
   static/js/ace/theme-sqlserver.js
 
-  offset of local header from start of archive:   1768259
-                                                  (00000000001AFB43h) bytes
+  offset of local header from start of archive:   1768295
+                                                  (00000000001AFB67h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2975,16 +2975,16 @@
   There is no file comment.
 
 Central directory entry #81:
 ---------------------------
 
   static/js/ace/mode-csharp.js
 
-  offset of local header from start of archive:   1769319
-                                                  (00000000001AFF67h) bytes
+  offset of local header from start of archive:   1769355
+                                                  (00000000001AFF8Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3012,16 +3012,16 @@
   There is no file comment.
 
 Central directory entry #82:
 ---------------------------
 
   static/js/ace/mode-gobstones.js
 
-  offset of local header from start of archive:   1772141
-                                                  (00000000001B0A6Dh) bytes
+  offset of local header from start of archive:   1772177
+                                                  (00000000001B0A91h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3049,16 +3049,16 @@
   There is no file comment.
 
 Central directory entry #83:
 ---------------------------
 
   static/js/ace/mode-prolog.js
 
-  offset of local header from start of archive:   1779081
-                                                  (00000000001B2589h) bytes
+  offset of local header from start of archive:   1779117
+                                                  (00000000001B25ADh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3086,16 +3086,16 @@
   There is no file comment.
 
 Central directory entry #84:
 ---------------------------
 
   static/js/ace/theme-twilight.js
 
-  offset of local header from start of archive:   1781622
-                                                  (00000000001B2F76h) bytes
+  offset of local header from start of archive:   1781658
+                                                  (00000000001B2F9Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3123,16 +3123,16 @@
   There is no file comment.
 
 Central directory entry #85:
 ---------------------------
 
   static/js/ace/mode-properties.js
 
-  offset of local header from start of archive:   1782584
-                                                  (00000000001B3338h) bytes
+  offset of local header from start of archive:   1782620
+                                                  (00000000001B335Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3160,16 +3160,16 @@
   There is no file comment.
 
 Central directory entry #86:
 ---------------------------
 
   static/js/ace/mode-velocity.js
 
-  offset of local header from start of archive:   1783098
-                                                  (00000000001B353Ah) bytes
+  offset of local header from start of archive:   1783134
+                                                  (00000000001B355Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3197,16 +3197,16 @@
   There is no file comment.
 
 Central directory entry #87:
 ---------------------------
 
   static/js/ace/mode-stylus.js
 
-  offset of local header from start of archive:   1801249
-                                                  (00000000001B7C21h) bytes
+  offset of local header from start of archive:   1801285
+                                                  (00000000001B7C45h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3234,16 +3234,16 @@
   There is no file comment.
 
 Central directory entry #88:
 ---------------------------
 
   static/js/ace/mode-html.js
 
-  offset of local header from start of archive:   1805529
-                                                  (00000000001B8CD9h) bytes
+  offset of local header from start of archive:   1805565
+                                                  (00000000001B8CFDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3271,16 +3271,16 @@
   There is no file comment.
 
 Central directory entry #89:
 ---------------------------
 
   static/js/ace/worker-javascript.js
 
-  offset of local header from start of archive:   1822624
-                                                  (00000000001BCFA0h) bytes
+  offset of local header from start of archive:   1822660
+                                                  (00000000001BCFC4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3308,16 +3308,16 @@
   There is no file comment.
 
 Central directory entry #90:
 ---------------------------
 
   static/js/ace/mode-powershell.js
 
-  offset of local header from start of archive:   1872154
-                                                  (00000000001C911Ah) bytes
+  offset of local header from start of archive:   1872190
+                                                  (00000000001C913Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3345,16 +3345,16 @@
   There is no file comment.
 
 Central directory entry #91:
 ---------------------------
 
   static/js/ace/mode-hjson.js
 
-  offset of local header from start of archive:   1880948
-                                                  (00000000001CB374h) bytes
+  offset of local header from start of archive:   1880984
+                                                  (00000000001CB398h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3382,16 +3382,16 @@
   There is no file comment.
 
 Central directory entry #92:
 ---------------------------
 
   static/js/ace/mode-latex.js
 
-  offset of local header from start of archive:   1882952
-                                                  (00000000001CBB48h) bytes
+  offset of local header from start of archive:   1882988
+                                                  (00000000001CBB6Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3419,16 +3419,16 @@
   There is no file comment.
 
 Central directory entry #93:
 ---------------------------
 
   static/js/ace/theme-xcode.js
 
-  offset of local header from start of archive:   1884328
-                                                  (00000000001CC0A8h) bytes
+  offset of local header from start of archive:   1884364
+                                                  (00000000001CC0CCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3456,16 +3456,16 @@
   There is no file comment.
 
 Central directory entry #94:
 ---------------------------
 
   static/js/ace/mode-ocaml.js
 
-  offset of local header from start of archive:   1885144
-                                                  (00000000001CC3D8h) bytes
+  offset of local header from start of archive:   1885180
+                                                  (00000000001CC3FCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3493,16 +3493,16 @@
   There is no file comment.
 
 Central directory entry #95:
 ---------------------------
 
   static/js/ace/mode-clojure.js
 
-  offset of local header from start of archive:   1890808
-                                                  (00000000001CD9F8h) bytes
+  offset of local header from start of archive:   1890844
+                                                  (00000000001CDA1Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3530,16 +3530,16 @@
   There is no file comment.
 
 Central directory entry #96:
 ---------------------------
 
   static/js/ace/mode-makefile.js
 
-  offset of local header from start of archive:   1894195
-                                                  (00000000001CE733h) bytes
+  offset of local header from start of archive:   1894231
+                                                  (00000000001CE757h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3567,16 +3567,16 @@
   There is no file comment.
 
 Central directory entry #97:
 ---------------------------
 
   static/js/ace/worker-coffee.js
 
-  offset of local header from start of archive:   1896515
-                                                  (00000000001CF043h) bytes
+  offset of local header from start of archive:   1896551
+                                                  (00000000001CF067h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3604,16 +3604,16 @@
   There is no file comment.
 
 Central directory entry #98:
 ---------------------------
 
   static/js/ace/mode-applescript.js
 
-  offset of local header from start of archive:   1945151
-                                                  (00000000001DAE3Fh) bytes
+  offset of local header from start of archive:   1945187
+                                                  (00000000001DAE63h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3641,16 +3641,16 @@
   There is no file comment.
 
 Central directory entry #99:
 ---------------------------
 
   static/js/ace/mode-dot.js
 
-  offset of local header from start of archive:   1947481
-                                                  (00000000001DB759h) bytes
+  offset of local header from start of archive:   1947517
+                                                  (00000000001DB77Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3678,16 +3678,16 @@
   There is no file comment.
 
 Central directory entry #100:
 ---------------------------
 
   static/js/ace/snippets/objectivec.js
 
-  offset of local header from start of archive:   1950278
-                                                  (00000000001DC246h) bytes
+  offset of local header from start of archive:   1950314
+                                                  (00000000001DC26Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3715,16 +3715,16 @@
   There is no file comment.
 
 Central directory entry #101:
 ---------------------------
 
   static/js/ace/snippets/gobstones.js
 
-  offset of local header from start of archive:   1950487
-                                                  (00000000001DC317h) bytes
+  offset of local header from start of archive:   1950523
+                                                  (00000000001DC33Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3752,16 +3752,16 @@
   There is no file comment.
 
 Central directory entry #102:
 ---------------------------
 
   static/js/ace/snippets/kotlin.js
 
-  offset of local header from start of archive:   1950876
-                                                  (00000000001DC49Ch) bytes
+  offset of local header from start of archive:   1950912
+                                                  (00000000001DC4C0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3789,16 +3789,16 @@
   There is no file comment.
 
 Central directory entry #103:
 ---------------------------
 
   static/js/ace/snippets/hjson.js
 
-  offset of local header from start of archive:   1951075
-                                                  (00000000001DC563h) bytes
+  offset of local header from start of archive:   1951111
+                                                  (00000000001DC587h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3826,16 +3826,16 @@
   There is no file comment.
 
 Central directory entry #104:
 ---------------------------
 
   static/js/ace/snippets/assembly_x86.js
 
-  offset of local header from start of archive:   1951273
-                                                  (00000000001DC629h) bytes
+  offset of local header from start of archive:   1951309
+                                                  (00000000001DC64Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3863,16 +3863,16 @@
   There is no file comment.
 
 Central directory entry #105:
 ---------------------------
 
   static/js/ace/snippets/ruby.js
 
-  offset of local header from start of archive:   1951487
-                                                  (00000000001DC6FFh) bytes
+  offset of local header from start of archive:   1951523
+                                                  (00000000001DC723h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3900,16 +3900,16 @@
   There is no file comment.
 
 Central directory entry #106:
 ---------------------------
 
   static/js/ace/snippets/logiql.js
 
-  offset of local header from start of archive:   1957447
-                                                  (00000000001DDE47h) bytes
+  offset of local header from start of archive:   1957483
+                                                  (00000000001DDE6Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3937,16 +3937,16 @@
   There is no file comment.
 
 Central directory entry #107:
 ---------------------------
 
   static/js/ace/snippets/text.js
 
-  offset of local header from start of archive:   1957648
-                                                  (00000000001DDF10h) bytes
+  offset of local header from start of archive:   1957684
+                                                  (00000000001DDF34h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3974,16 +3974,16 @@
   There is no file comment.
 
 Central directory entry #108:
 ---------------------------
 
   static/js/ace/snippets/html_ruby.js
 
-  offset of local header from start of archive:   1957845
-                                                  (00000000001DDFD5h) bytes
+  offset of local header from start of archive:   1957881
+                                                  (00000000001DDFF9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4011,16 +4011,16 @@
   There is no file comment.
 
 Central directory entry #109:
 ---------------------------
 
   static/js/ace/snippets/php.js
 
-  offset of local header from start of archive:   1958053
-                                                  (00000000001DE0A5h) bytes
+  offset of local header from start of archive:   1958089
+                                                  (00000000001DE0C9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4048,16 +4048,16 @@
   There is no file comment.
 
 Central directory entry #110:
 ---------------------------
 
   static/js/ace/snippets/makefile.js
 
-  offset of local header from start of archive:   1960122
-                                                  (00000000001DE8BAh) bytes
+  offset of local header from start of archive:   1960158
+                                                  (00000000001DE8DEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4085,16 +4085,16 @@
   There is no file comment.
 
 Central directory entry #111:
 ---------------------------
 
   static/js/ace/snippets/vbscript.js
 
-  offset of local header from start of archive:   1960366
-                                                  (00000000001DE9AEh) bytes
+  offset of local header from start of archive:   1960402
+                                                  (00000000001DE9D2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4122,16 +4122,16 @@
   There is no file comment.
 
 Central directory entry #112:
 ---------------------------
 
   static/js/ace/snippets/snippets.js
 
-  offset of local header from start of archive:   1960570
-                                                  (00000000001DEA7Ah) bytes
+  offset of local header from start of archive:   1960606
+                                                  (00000000001DEA9Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4159,16 +4159,16 @@
   There is no file comment.
 
 Central directory entry #113:
 ---------------------------
 
   static/js/ace/snippets/haml.js
 
-  offset of local header from start of archive:   1960846
-                                                  (00000000001DEB8Eh) bytes
+  offset of local header from start of archive:   1960882
+                                                  (00000000001DEBB2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4196,16 +4196,16 @@
   There is no file comment.
 
 Central directory entry #114:
 ---------------------------
 
   static/js/ace/snippets/json.js
 
-  offset of local header from start of archive:   1961162
-                                                  (00000000001DECCAh) bytes
+  offset of local header from start of archive:   1961198
+                                                  (00000000001DECEEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4233,16 +4233,16 @@
   There is no file comment.
 
 Central directory entry #115:
 ---------------------------
 
   static/js/ace/snippets/svg.js
 
-  offset of local header from start of archive:   1961359
-                                                  (00000000001DED8Fh) bytes
+  offset of local header from start of archive:   1961395
+                                                  (00000000001DEDB3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4270,16 +4270,16 @@
   There is no file comment.
 
 Central directory entry #116:
 ---------------------------
 
   static/js/ace/snippets/drools.js
 
-  offset of local header from start of archive:   1961555
-                                                  (00000000001DEE53h) bytes
+  offset of local header from start of archive:   1961591
+                                                  (00000000001DEE77h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4307,16 +4307,16 @@
   There is no file comment.
 
 Central directory entry #117:
 ---------------------------
 
   static/js/ace/snippets/haskell.js
 
-  offset of local header from start of archive:   1961866
-                                                  (00000000001DEF8Ah) bytes
+  offset of local header from start of archive:   1961902
+                                                  (00000000001DEFAEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4344,16 +4344,16 @@
   There is no file comment.
 
 Central directory entry #118:
 ---------------------------
 
   static/js/ace/snippets/vhdl.js
 
-  offset of local header from start of archive:   1962782
-                                                  (00000000001DF31Eh) bytes
+  offset of local header from start of archive:   1962818
+                                                  (00000000001DF342h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4381,16 +4381,16 @@
   There is no file comment.
 
 Central directory entry #119:
 ---------------------------
 
   static/js/ace/snippets/gcode.js
 
-  offset of local header from start of archive:   1962980
-                                                  (00000000001DF3E4h) bytes
+  offset of local header from start of archive:   1963016
+                                                  (00000000001DF408h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4418,16 +4418,16 @@
   There is no file comment.
 
 Central directory entry #120:
 ---------------------------
 
   static/js/ace/snippets/erlang.js
 
-  offset of local header from start of archive:   1963178
-                                                  (00000000001DF4AAh) bytes
+  offset of local header from start of archive:   1963214
+                                                  (00000000001DF4CEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4455,16 +4455,16 @@
   There is no file comment.
 
 Central directory entry #121:
 ---------------------------
 
   static/js/ace/snippets/matlab.js
 
-  offset of local header from start of archive:   1964485
-                                                  (00000000001DF9C5h) bytes
+  offset of local header from start of archive:   1964521
+                                                  (00000000001DF9E9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4492,16 +4492,16 @@
   There is no file comment.
 
 Central directory entry #122:
 ---------------------------
 
   static/js/ace/snippets/properties.js
 
-  offset of local header from start of archive:   1964686
-                                                  (00000000001DFA8Eh) bytes
+  offset of local header from start of archive:   1964722
+                                                  (00000000001DFAB2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4529,16 +4529,16 @@
   There is no file comment.
 
 Central directory entry #123:
 ---------------------------
 
   static/js/ace/snippets/io.js
 
-  offset of local header from start of archive:   1964893
-                                                  (00000000001DFB5Dh) bytes
+  offset of local header from start of archive:   1964929
+                                                  (00000000001DFB81h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4566,16 +4566,16 @@
   There is no file comment.
 
 Central directory entry #124:
 ---------------------------
 
   static/js/ace/snippets/xquery.js
 
-  offset of local header from start of archive:   1965480
-                                                  (00000000001DFDA8h) bytes
+  offset of local header from start of archive:   1965516
+                                                  (00000000001DFDCCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4603,16 +4603,16 @@
   There is no file comment.
 
 Central directory entry #125:
 ---------------------------
 
   static/js/ace/snippets/razor.js
 
-  offset of local header from start of archive:   1966144
-                                                  (00000000001E0040h) bytes
+  offset of local header from start of archive:   1966180
+                                                  (00000000001E0064h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4640,16 +4640,16 @@
   There is no file comment.
 
 Central directory entry #126:
 ---------------------------
 
   static/js/ace/snippets/typescript.js
 
-  offset of local header from start of archive:   1966368
-                                                  (00000000001E0120h) bytes
+  offset of local header from start of archive:   1966404
+                                                  (00000000001E0144h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4677,16 +4677,16 @@
   There is no file comment.
 
 Central directory entry #127:
 ---------------------------
 
   static/js/ace/snippets/mips_assembler.js
 
-  offset of local header from start of archive:   1966575
-                                                  (00000000001E01EFh) bytes
+  offset of local header from start of archive:   1966611
+                                                  (00000000001E0213h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4714,16 +4714,16 @@
   There is no file comment.
 
 Central directory entry #128:
 ---------------------------
 
   static/js/ace/snippets/textile.js
 
-  offset of local header from start of archive:   1966790
-                                                  (00000000001E02C6h) bytes
+  offset of local header from start of archive:   1966826
+                                                  (00000000001E02EAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4751,16 +4751,16 @@
   There is no file comment.
 
 Central directory entry #129:
 ---------------------------
 
   static/js/ace/snippets/perl.js
 
-  offset of local header from start of archive:   1967206
-                                                  (00000000001E0466h) bytes
+  offset of local header from start of archive:   1967242
+                                                  (00000000001E048Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4788,16 +4788,16 @@
   There is no file comment.
 
 Central directory entry #130:
 ---------------------------
 
   static/js/ace/snippets/mel.js
 
-  offset of local header from start of archive:   1969358
-                                                  (00000000001E0CCEh) bytes
+  offset of local header from start of archive:   1969394
+                                                  (00000000001E0CF2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4825,16 +4825,16 @@
   There is no file comment.
 
 Central directory entry #131:
 ---------------------------
 
   static/js/ace/snippets/applescript.js
 
-  offset of local header from start of archive:   1969553
-                                                  (00000000001E0D91h) bytes
+  offset of local header from start of archive:   1969589
+                                                  (00000000001E0DB5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4862,16 +4862,16 @@
   There is no file comment.
 
 Central directory entry #132:
 ---------------------------
 
   static/js/ace/snippets/less.js
 
-  offset of local header from start of archive:   1969762
-                                                  (00000000001E0E62h) bytes
+  offset of local header from start of archive:   1969798
+                                                  (00000000001E0E86h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4899,16 +4899,16 @@
   There is no file comment.
 
 Central directory entry #133:
 ---------------------------
 
   static/js/ace/snippets/live_script.js
 
-  offset of local header from start of archive:   1969959
-                                                  (00000000001E0F27h) bytes
+  offset of local header from start of archive:   1969995
+                                                  (00000000001E0F4Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4936,16 +4936,16 @@
   There is no file comment.
 
 Central directory entry #134:
 ---------------------------
 
   static/js/ace/snippets/coffee.js
 
-  offset of local header from start of archive:   1970166
-                                                  (00000000001E0FF6h) bytes
+  offset of local header from start of archive:   1970202
+                                                  (00000000001E101Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4973,16 +4973,16 @@
   There is no file comment.
 
 Central directory entry #135:
 ---------------------------
 
   static/js/ace/snippets/bro.js
 
-  offset of local header from start of archive:   1970965
-                                                  (00000000001E1315h) bytes
+  offset of local header from start of archive:   1971001
+                                                  (00000000001E1339h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5010,16 +5010,16 @@
   There is no file comment.
 
 Central directory entry #136:
 ---------------------------
 
   static/js/ace/snippets/prolog.js
 
-  offset of local header from start of archive:   1971159
-                                                  (00000000001E13D7h) bytes
+  offset of local header from start of archive:   1971195
+                                                  (00000000001E13FBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5047,16 +5047,16 @@
   There is no file comment.
 
 Central directory entry #137:
 ---------------------------
 
   static/js/ace/snippets/velocity.js
 
-  offset of local header from start of archive:   1971359
-                                                  (00000000001E149Fh) bytes
+  offset of local header from start of archive:   1971395
+                                                  (00000000001E14C3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5084,16 +5084,16 @@
   There is no file comment.
 
 Central directory entry #138:
 ---------------------------
 
   static/js/ace/snippets/ini.js
 
-  offset of local header from start of archive:   1971778
-                                                  (00000000001E1642h) bytes
+  offset of local header from start of archive:   1971814
+                                                  (00000000001E1666h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5121,16 +5121,16 @@
   There is no file comment.
 
 Central directory entry #139:
 ---------------------------
 
   static/js/ace/snippets/rdoc.js
 
-  offset of local header from start of archive:   1971973
-                                                  (00000000001E1705h) bytes
+  offset of local header from start of archive:   1972009
+                                                  (00000000001E1729h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5158,16 +5158,16 @@
   There is no file comment.
 
 Central directory entry #140:
 ---------------------------
 
   static/js/ace/snippets/actionscript.js
 
-  offset of local header from start of archive:   1972169
-                                                  (00000000001E17C9h) bytes
+  offset of local header from start of archive:   1972205
+                                                  (00000000001E17EDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5195,16 +5195,16 @@
   There is no file comment.
 
 Central directory entry #141:
 ---------------------------
 
   static/js/ace/snippets/cirru.js
 
-  offset of local header from start of archive:   1973454
-                                                  (00000000001E1CCEh) bytes
+  offset of local header from start of archive:   1973490
+                                                  (00000000001E1CF2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5232,16 +5232,16 @@
   There is no file comment.
 
 Central directory entry #142:
 ---------------------------
 
   static/js/ace/snippets/html.js
 
-  offset of local header from start of archive:   1973652
-                                                  (00000000001E1D94h) bytes
+  offset of local header from start of archive:   1973688
+                                                  (00000000001E1DB8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5269,16 +5269,16 @@
   There is no file comment.
 
 Central directory entry #143:
 ---------------------------
 
   static/js/ace/snippets/groovy.js
 
-  offset of local header from start of archive:   1977892
-                                                  (00000000001E2E24h) bytes
+  offset of local header from start of archive:   1977928
+                                                  (00000000001E2E48h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5306,16 +5306,16 @@
   There is no file comment.
 
 Central directory entry #144:
 ---------------------------
 
   static/js/ace/snippets/lsl.js
 
-  offset of local header from start of archive:   1978093
-                                                  (00000000001E2EEDh) bytes
+  offset of local header from start of archive:   1978129
+                                                  (00000000001E2F11h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5343,16 +5343,16 @@
   There is no file comment.
 
 Central directory entry #145:
 ---------------------------
 
   static/js/ace/snippets/r.js
 
-  offset of local header from start of archive:   1985192
-                                                  (00000000001E4AA8h) bytes
+  offset of local header from start of archive:   1985228
+                                                  (00000000001E4ACCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5380,16 +5380,16 @@
   There is no file comment.
 
 Central directory entry #146:
 ---------------------------
 
   static/js/ace/snippets/plain_text.js
 
-  offset of local header from start of archive:   1986038
-                                                  (00000000001E4DF6h) bytes
+  offset of local header from start of archive:   1986074
+                                                  (00000000001E4E1Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5417,16 +5417,16 @@
   There is no file comment.
 
 Central directory entry #147:
 ---------------------------
 
   static/js/ace/snippets/mysql.js
 
-  offset of local header from start of archive:   1986246
-                                                  (00000000001E4EC6h) bytes
+  offset of local header from start of archive:   1986282
+                                                  (00000000001E4EEAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5454,16 +5454,16 @@
   There is no file comment.
 
 Central directory entry #148:
 ---------------------------
 
   static/js/ace/snippets/css.js
 
-  offset of local header from start of archive:   1986445
-                                                  (00000000001E4F8Dh) bytes
+  offset of local header from start of archive:   1986481
+                                                  (00000000001E4FB1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5491,16 +5491,16 @@
   There is no file comment.
 
 Central directory entry #149:
 ---------------------------
 
   static/js/ace/snippets/pgsql.js
 
-  offset of local header from start of archive:   1990516
-                                                  (00000000001E5F74h) bytes
+  offset of local header from start of archive:   1990552
+                                                  (00000000001E5F98h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5528,16 +5528,16 @@
   There is no file comment.
 
 Central directory entry #150:
 ---------------------------
 
   static/js/ace/snippets/lucene.js
 
-  offset of local header from start of archive:   1990715
-                                                  (00000000001E603Bh) bytes
+  offset of local header from start of archive:   1990751
+                                                  (00000000001E605Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5565,16 +5565,16 @@
   There is no file comment.
 
 Central directory entry #151:
 ---------------------------
 
   static/js/ace/snippets/ocaml.js
 
-  offset of local header from start of archive:   1990914
-                                                  (00000000001E6102h) bytes
+  offset of local header from start of archive:   1990950
+                                                  (00000000001E6126h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5602,16 +5602,16 @@
   There is no file comment.
 
 Central directory entry #152:
 ---------------------------
 
   static/js/ace/snippets/java.js
 
-  offset of local header from start of archive:   1991113
-                                                  (00000000001E61C9h) bytes
+  offset of local header from start of archive:   1991149
+                                                  (00000000001E61EDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5639,16 +5639,16 @@
   There is no file comment.
 
 Central directory entry #153:
 ---------------------------
 
   static/js/ace/snippets/mushcode.js
 
-  offset of local header from start of archive:   1992722
-                                                  (00000000001E6812h) bytes
+  offset of local header from start of archive:   1992758
+                                                  (00000000001E6836h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5676,16 +5676,16 @@
   There is no file comment.
 
 Central directory entry #154:
 ---------------------------
 
   static/js/ace/snippets/dot.js
 
-  offset of local header from start of archive:   1992926
-                                                  (00000000001E68DEh) bytes
+  offset of local header from start of archive:   1992962
+                                                  (00000000001E6902h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5713,16 +5713,16 @@
   There is no file comment.
 
 Central directory entry #155:
 ---------------------------
 
   static/js/ace/snippets/verilog.js
 
-  offset of local header from start of archive:   1993121
-                                                  (00000000001E69A1h) bytes
+  offset of local header from start of archive:   1993157
+                                                  (00000000001E69C5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5750,16 +5750,16 @@
   There is no file comment.
 
 Central directory entry #156:
 ---------------------------
 
   static/js/ace/snippets/twig.js
 
-  offset of local header from start of archive:   1993324
-                                                  (00000000001E6A6Ch) bytes
+  offset of local header from start of archive:   1993360
+                                                  (00000000001E6A90h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5787,16 +5787,16 @@
   There is no file comment.
 
 Central directory entry #157:
 ---------------------------
 
   static/js/ace/snippets/eiffel.js
 
-  offset of local header from start of archive:   1993522
-                                                  (00000000001E6B32h) bytes
+  offset of local header from start of archive:   1993558
+                                                  (00000000001E6B56h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5824,16 +5824,16 @@
   There is no file comment.
 
 Central directory entry #158:
 ---------------------------
 
   static/js/ace/snippets/dockerfile.js
 
-  offset of local header from start of archive:   1993722
-                                                  (00000000001E6BFAh) bytes
+  offset of local header from start of archive:   1993758
+                                                  (00000000001E6C1Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5861,16 +5861,16 @@
   There is no file comment.
 
 Central directory entry #159:
 ---------------------------
 
   static/js/ace/snippets/sql.js
 
-  offset of local header from start of archive:   1993930
-                                                  (00000000001E6CCAh) bytes
+  offset of local header from start of archive:   1993966
+                                                  (00000000001E6CEEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5898,16 +5898,16 @@
   There is no file comment.
 
 Central directory entry #160:
 ---------------------------
 
   static/js/ace/snippets/fortran.js
 
-  offset of local header from start of archive:   1994408
-                                                  (00000000001E6EA8h) bytes
+  offset of local header from start of archive:   1994444
+                                                  (00000000001E6ECCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5935,16 +5935,16 @@
   There is no file comment.
 
 Central directory entry #161:
 ---------------------------
 
   static/js/ace/snippets/tcl.js
 
-  offset of local header from start of archive:   1994610
-                                                  (00000000001E6F72h) bytes
+  offset of local header from start of archive:   1994646
+                                                  (00000000001E6F96h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5972,16 +5972,16 @@
   There is no file comment.
 
 Central directory entry #162:
 ---------------------------
 
   static/js/ace/snippets/golang.js
 
-  offset of local header from start of archive:   1995344
-                                                  (00000000001E7250h) bytes
+  offset of local header from start of archive:   1995380
+                                                  (00000000001E7274h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6009,16 +6009,16 @@
   There is no file comment.
 
 Central directory entry #163:
 ---------------------------
 
   static/js/ace/snippets/curly.js
 
-  offset of local header from start of archive:   1995545
-                                                  (00000000001E7319h) bytes
+  offset of local header from start of archive:   1995581
+                                                  (00000000001E733Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6046,16 +6046,16 @@
   There is no file comment.
 
 Central directory entry #164:
 ---------------------------
 
   static/js/ace/snippets/lean.js
 
-  offset of local header from start of archive:   1995744
-                                                  (00000000001E73E0h) bytes
+  offset of local header from start of archive:   1995780
+                                                  (00000000001E7404h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6083,16 +6083,16 @@
   There is no file comment.
 
 Central directory entry #165:
 ---------------------------
 
   static/js/ace/snippets/jsp.js
 
-  offset of local header from start of archive:   1995941
-                                                  (00000000001E74A5h) bytes
+  offset of local header from start of archive:   1995977
+                                                  (00000000001E74C9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6120,16 +6120,16 @@
   There is no file comment.
 
 Central directory entry #166:
 ---------------------------
 
   static/js/ace/snippets/ejs.js
 
-  offset of local header from start of archive:   1996877
-                                                  (00000000001E784Dh) bytes
+  offset of local header from start of archive:   1996913
+                                                  (00000000001E7871h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6157,16 +6157,16 @@
   There is no file comment.
 
 Central directory entry #167:
 ---------------------------
 
   static/js/ace/snippets/swig.js
 
-  offset of local header from start of archive:   1997073
-                                                  (00000000001E7911h) bytes
+  offset of local header from start of archive:   1997109
+                                                  (00000000001E7935h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6194,16 +6194,16 @@
   There is no file comment.
 
 Central directory entry #168:
 ---------------------------
 
   static/js/ace/snippets/soy_template.js
 
-  offset of local header from start of archive:   1997271
-                                                  (00000000001E79D7h) bytes
+  offset of local header from start of archive:   1997307
+                                                  (00000000001E79FBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6231,16 +6231,16 @@
   There is no file comment.
 
 Central directory entry #169:
 ---------------------------
 
   static/js/ace/snippets/gitignore.js
 
-  offset of local header from start of archive:   1997482
-                                                  (00000000001E7AAAh) bytes
+  offset of local header from start of archive:   1997518
+                                                  (00000000001E7ACEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6268,16 +6268,16 @@
   There is no file comment.
 
 Central directory entry #170:
 ---------------------------
 
   static/js/ace/snippets/pascal.js
 
-  offset of local header from start of archive:   1997687
-                                                  (00000000001E7B77h) bytes
+  offset of local header from start of archive:   1997723
+                                                  (00000000001E7B9Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6305,16 +6305,16 @@
   There is no file comment.
 
 Central directory entry #171:
 ---------------------------
 
   static/js/ace/snippets/wollok.js
 
-  offset of local header from start of archive:   1997887
-                                                  (00000000001E7C3Fh) bytes
+  offset of local header from start of archive:   1997923
+                                                  (00000000001E7C63h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6342,16 +6342,16 @@
   There is no file comment.
 
 Central directory entry #172:
 ---------------------------
 
   static/js/ace/snippets/c_cpp.js
 
-  offset of local header from start of archive:   1998535
-                                                  (00000000001E7EC7h) bytes
+  offset of local header from start of archive:   1998571
+                                                  (00000000001E7EEBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6379,16 +6379,16 @@
   There is no file comment.
 
 Central directory entry #173:
 ---------------------------
 
   static/js/ace/snippets/haxe.js
 
-  offset of local header from start of archive:   1999535
-                                                  (00000000001E82AFh) bytes
+  offset of local header from start of archive:   1999571
+                                                  (00000000001E82D3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6416,16 +6416,16 @@
   There is no file comment.
 
 Central directory entry #174:
 ---------------------------
 
   static/js/ace/snippets/gherkin.js
 
-  offset of local header from start of archive:   1999732
-                                                  (00000000001E8374h) bytes
+  offset of local header from start of archive:   1999768
+                                                  (00000000001E8398h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6453,16 +6453,16 @@
   There is no file comment.
 
 Central directory entry #175:
 ---------------------------
 
   static/js/ace/snippets/python.js
 
-  offset of local header from start of archive:   1999935
-                                                  (00000000001E843Fh) bytes
+  offset of local header from start of archive:   1999971
+                                                  (00000000001E8463h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6490,16 +6490,16 @@
   There is no file comment.
 
 Central directory entry #176:
 ---------------------------
 
   static/js/ace/snippets/maze.js
 
-  offset of local header from start of archive:   2001303
-                                                  (00000000001E8997h) bytes
+  offset of local header from start of archive:   2001339
+                                                  (00000000001E89BBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6527,16 +6527,16 @@
   There is no file comment.
 
 Central directory entry #177:
 ---------------------------
 
   static/js/ace/snippets/autohotkey.js
 
-  offset of local header from start of archive:   2001586
-                                                  (00000000001E8AB2h) bytes
+  offset of local header from start of archive:   2001622
+                                                  (00000000001E8AD6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6564,16 +6564,16 @@
   There is no file comment.
 
 Central directory entry #178:
 ---------------------------
 
   static/js/ace/snippets/scheme.js
 
-  offset of local header from start of archive:   2001795
-                                                  (00000000001E8B83h) bytes
+  offset of local header from start of archive:   2001831
+                                                  (00000000001E8BA7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6601,16 +6601,16 @@
   There is no file comment.
 
 Central directory entry #179:
 ---------------------------
 
   static/js/ace/snippets/abc.js
 
-  offset of local header from start of archive:   2001995
-                                                  (00000000001E8C4Bh) bytes
+  offset of local header from start of archive:   2002031
+                                                  (00000000001E8C6Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6638,16 +6638,16 @@
   There is no file comment.
 
 Central directory entry #180:
 ---------------------------
 
   static/js/ace/snippets/scss.js
 
-  offset of local header from start of archive:   2002487
-                                                  (00000000001E8E37h) bytes
+  offset of local header from start of archive:   2002523
+                                                  (00000000001E8E5Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6675,16 +6675,16 @@
   There is no file comment.
 
 Central directory entry #181:
 ---------------------------
 
   static/js/ace/snippets/html_elixir.js
 
-  offset of local header from start of archive:   2002683
-                                                  (00000000001E8EFBh) bytes
+  offset of local header from start of archive:   2002719
+                                                  (00000000001E8F1Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6712,16 +6712,16 @@
   There is no file comment.
 
 Central directory entry #182:
 ---------------------------
 
   static/js/ace/snippets/latex.js
 
-  offset of local header from start of archive:   2002893
-                                                  (00000000001E8FCDh) bytes
+  offset of local header from start of archive:   2002929
+                                                  (00000000001E8FF1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6749,16 +6749,16 @@
   There is no file comment.
 
 Central directory entry #183:
 ---------------------------
 
   static/js/ace/snippets/nsis.js
 
-  offset of local header from start of archive:   2003091
-                                                  (00000000001E9093h) bytes
+  offset of local header from start of archive:   2003127
+                                                  (00000000001E90B7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6786,16 +6786,16 @@
   There is no file comment.
 
 Central directory entry #184:
 ---------------------------
 
   static/js/ace/snippets/sjs.js
 
-  offset of local header from start of archive:   2003286
-                                                  (00000000001E9156h) bytes
+  offset of local header from start of archive:   2003322
+                                                  (00000000001E917Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6823,16 +6823,16 @@
   There is no file comment.
 
 Central directory entry #185:
 ---------------------------
 
   static/js/ace/snippets/jsx.js
 
-  offset of local header from start of archive:   2003482
-                                                  (00000000001E921Ah) bytes
+  offset of local header from start of archive:   2003518
+                                                  (00000000001E923Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6860,16 +6860,16 @@
   There is no file comment.
 
 Central directory entry #186:
 ---------------------------
 
   static/js/ace/snippets/tex.js
 
-  offset of local header from start of archive:   2003678
-                                                  (00000000001E92DEh) bytes
+  offset of local header from start of archive:   2003714
+                                                  (00000000001E9302h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6897,16 +6897,16 @@
   There is no file comment.
 
 Central directory entry #187:
 ---------------------------
 
   static/js/ace/snippets/vala.js
 
-  offset of local header from start of archive:   2004990
-                                                  (00000000001E97FEh) bytes
+  offset of local header from start of archive:   2005026
+                                                  (00000000001E9822h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6934,16 +6934,16 @@
   There is no file comment.
 
 Central directory entry #188:
 ---------------------------
 
   static/js/ace/snippets/tsx.js
 
-  offset of local header from start of archive:   2006037
-                                                  (00000000001E9C15h) bytes
+  offset of local header from start of archive:   2006073
+                                                  (00000000001E9C39h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -6971,16 +6971,16 @@
   There is no file comment.
 
 Central directory entry #189:
 ---------------------------
 
   static/js/ace/snippets/rst.js
 
-  offset of local header from start of archive:   2006232
-                                                  (00000000001E9CD8h) bytes
+  offset of local header from start of archive:   2006268
+                                                  (00000000001E9CFCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7008,16 +7008,16 @@
   There is no file comment.
 
 Central directory entry #190:
 ---------------------------
 
   static/js/ace/snippets/scala.js
 
-  offset of local header from start of archive:   2006575
-                                                  (00000000001E9E2Fh) bytes
+  offset of local header from start of archive:   2006611
+                                                  (00000000001E9E53h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7045,16 +7045,16 @@
   There is no file comment.
 
 Central directory entry #191:
 ---------------------------
 
   static/js/ace/snippets/yaml.js
 
-  offset of local header from start of archive:   2006774
-                                                  (00000000001E9EF6h) bytes
+  offset of local header from start of archive:   2006810
+                                                  (00000000001E9F1Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7082,16 +7082,16 @@
   There is no file comment.
 
 Central directory entry #192:
 ---------------------------
 
   static/js/ace/snippets/ada.js
 
-  offset of local header from start of archive:   2006972
-                                                  (00000000001E9FBCh) bytes
+  offset of local header from start of archive:   2007008
+                                                  (00000000001E9FE0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7119,16 +7119,16 @@
   There is no file comment.
 
 Central directory entry #193:
 ---------------------------
 
   static/js/ace/snippets/batchfile.js
 
-  offset of local header from start of archive:   2007168
-                                                  (00000000001EA080h) bytes
+  offset of local header from start of archive:   2007204
+                                                  (00000000001EA0A4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7156,16 +7156,16 @@
   There is no file comment.
 
 Central directory entry #194:
 ---------------------------
 
   static/js/ace/snippets/smarty.js
 
-  offset of local header from start of archive:   2007374
-                                                  (00000000001EA14Eh) bytes
+  offset of local header from start of archive:   2007410
+                                                  (00000000001EA172h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7193,16 +7193,16 @@
   There is no file comment.
 
 Central directory entry #195:
 ---------------------------
 
   static/js/ace/snippets/praat.js
 
-  offset of local header from start of archive:   2007575
-                                                  (00000000001EA217h) bytes
+  offset of local header from start of archive:   2007611
+                                                  (00000000001EA23Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7230,16 +7230,16 @@
   There is no file comment.
 
 Central directory entry #196:
 ---------------------------
 
   static/js/ace/snippets/asciidoc.js
 
-  offset of local header from start of archive:   2007774
-                                                  (00000000001EA2DEh) bytes
+  offset of local header from start of archive:   2007810
+                                                  (00000000001EA302h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7267,16 +7267,16 @@
   There is no file comment.
 
 Central directory entry #197:
 ---------------------------
 
   static/js/ace/snippets/swift.js
 
-  offset of local header from start of archive:   2007978
-                                                  (00000000001EA3AAh) bytes
+  offset of local header from start of archive:   2008014
+                                                  (00000000001EA3CEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7304,16 +7304,16 @@
   There is no file comment.
 
 Central directory entry #198:
 ---------------------------
 
   static/js/ace/snippets/scad.js
 
-  offset of local header from start of archive:   2008177
-                                                  (00000000001EA471h) bytes
+  offset of local header from start of archive:   2008213
+                                                  (00000000001EA495h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7341,16 +7341,16 @@
   There is no file comment.
 
 Central directory entry #199:
 ---------------------------
 
   static/js/ace/snippets/elm.js
 
-  offset of local header from start of archive:   2008374
-                                                  (00000000001EA536h) bytes
+  offset of local header from start of archive:   2008410
+                                                  (00000000001EA55Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7378,16 +7378,16 @@
   There is no file comment.
 
 Central directory entry #200:
 ---------------------------
 
   static/js/ace/snippets/glsl.js
 
-  offset of local header from start of archive:   2008569
-                                                  (00000000001EA5F9h) bytes
+  offset of local header from start of archive:   2008605
+                                                  (00000000001EA61Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7415,16 +7415,16 @@
   There is no file comment.
 
 Central directory entry #201:
 ---------------------------
 
   static/js/ace/snippets/mask.js
 
-  offset of local header from start of archive:   2008767
-                                                  (00000000001EA6BFh) bytes
+  offset of local header from start of archive:   2008803
+                                                  (00000000001EA6E3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7452,16 +7452,16 @@
   There is no file comment.
 
 Central directory entry #202:
 ---------------------------
 
   static/js/ace/snippets/lua.js
 
-  offset of local header from start of archive:   2008965
-                                                  (00000000001EA785h) bytes
+  offset of local header from start of archive:   2009001
+                                                  (00000000001EA7A9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7489,16 +7489,16 @@
   There is no file comment.
 
 Central directory entry #203:
 ---------------------------
 
   static/js/ace/snippets/c9search.js
 
-  offset of local header from start of archive:   2009316
-                                                  (00000000001EA8E4h) bytes
+  offset of local header from start of archive:   2009352
+                                                  (00000000001EA908h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7526,16 +7526,16 @@
   There is no file comment.
 
 Central directory entry #204:
 ---------------------------
 
   static/js/ace/snippets/diff.js
 
-  offset of local header from start of archive:   2009520
-                                                  (00000000001EA9B0h) bytes
+  offset of local header from start of archive:   2009556
+                                                  (00000000001EA9D4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7563,16 +7563,16 @@
   There is no file comment.
 
 Central directory entry #205:
 ---------------------------
 
   static/js/ace/snippets/clojure.js
 
-  offset of local header from start of archive:   2009978
-                                                  (00000000001EAB7Ah) bytes
+  offset of local header from start of archive:   2010014
+                                                  (00000000001EAB9Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7600,16 +7600,16 @@
   There is no file comment.
 
 Central directory entry #206:
 ---------------------------
 
   static/js/ace/snippets/livescript.js
 
-  offset of local header from start of archive:   2010788
-                                                  (00000000001EAEA4h) bytes
+  offset of local header from start of archive:   2010824
+                                                  (00000000001EAEC8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7637,16 +7637,16 @@
   There is no file comment.
 
 Central directory entry #207:
 ---------------------------
 
   static/js/ace/snippets/rust.js
 
-  offset of local header from start of archive:   2010996
-                                                  (00000000001EAF74h) bytes
+  offset of local header from start of archive:   2011032
+                                                  (00000000001EAF98h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7674,16 +7674,16 @@
   There is no file comment.
 
 Central directory entry #208:
 ---------------------------
 
   static/js/ace/snippets/powershell.js
 
-  offset of local header from start of archive:   2011192
-                                                  (00000000001EB038h) bytes
+  offset of local header from start of archive:   2011228
+                                                  (00000000001EB05Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7711,16 +7711,16 @@
   There is no file comment.
 
 Central directory entry #209:
 ---------------------------
 
   static/js/ace/snippets/jsoniq.js
 
-  offset of local header from start of archive:   2011401
-                                                  (00000000001EB109h) bytes
+  offset of local header from start of archive:   2011437
+                                                  (00000000001EB12Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7748,16 +7748,16 @@
   There is no file comment.
 
 Central directory entry #210:
 ---------------------------
 
   static/js/ace/snippets/d.js
 
-  offset of local header from start of archive:   2012065
-                                                  (00000000001EB3A1h) bytes
+  offset of local header from start of archive:   2012101
+                                                  (00000000001EB3C5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7785,16 +7785,16 @@
   There is no file comment.
 
 Central directory entry #211:
 ---------------------------
 
   static/js/ace/snippets/toml.js
 
-  offset of local header from start of archive:   2012256
-                                                  (00000000001EB460h) bytes
+  offset of local header from start of archive:   2012292
+                                                  (00000000001EB484h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7822,16 +7822,16 @@
   There is no file comment.
 
 Central directory entry #212:
 ---------------------------
 
   static/js/ace/snippets/csharp.js
 
-  offset of local header from start of archive:   2012453
-                                                  (00000000001EB525h) bytes
+  offset of local header from start of archive:   2012489
+                                                  (00000000001EB549h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7859,16 +7859,16 @@
   There is no file comment.
 
 Central directory entry #213:
 ---------------------------
 
   static/js/ace/snippets/lisp.js
 
-  offset of local header from start of archive:   2012653
-                                                  (00000000001EB5EDh) bytes
+  offset of local header from start of archive:   2012689
+                                                  (00000000001EB611h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7896,16 +7896,16 @@
   There is no file comment.
 
 Central directory entry #214:
 ---------------------------
 
   static/js/ace/snippets/sqlserver.js
 
-  offset of local header from start of archive:   2012850
-                                                  (00000000001EB6B2h) bytes
+  offset of local header from start of archive:   2012886
+                                                  (00000000001EB6D6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7933,16 +7933,16 @@
   There is no file comment.
 
 Central directory entry #215:
 ---------------------------
 
   static/js/ace/snippets/nix.js
 
-  offset of local header from start of archive:   2013833
-                                                  (00000000001EBA89h) bytes
+  offset of local header from start of archive:   2013869
+                                                  (00000000001EBAADh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -7970,16 +7970,16 @@
   There is no file comment.
 
 Central directory entry #216:
 ---------------------------
 
   static/js/ace/snippets/dart.js
 
-  offset of local header from start of archive:   2014028
-                                                  (00000000001EBB4Ch) bytes
+  offset of local header from start of archive:   2014064
+                                                  (00000000001EBB70h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8007,16 +8007,16 @@
   There is no file comment.
 
 Central directory entry #217:
 ---------------------------
 
   static/js/ace/snippets/cobol.js
 
-  offset of local header from start of archive:   2014635
-                                                  (00000000001EBDABh) bytes
+  offset of local header from start of archive:   2014671
+                                                  (00000000001EBDCFh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8044,16 +8044,16 @@
   There is no file comment.
 
 Central directory entry #218:
 ---------------------------
 
   static/js/ace/snippets/jade.js
 
-  offset of local header from start of archive:   2014834
-                                                  (00000000001EBE72h) bytes
+  offset of local header from start of archive:   2014870
+                                                  (00000000001EBE96h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8081,16 +8081,16 @@
   There is no file comment.
 
 Central directory entry #219:
 ---------------------------
 
   static/js/ace/snippets/protobuf.js
 
-  offset of local header from start of archive:   2015031
-                                                  (00000000001EBF37h) bytes
+  offset of local header from start of archive:   2015067
+                                                  (00000000001EBF5Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8118,16 +8118,16 @@
   There is no file comment.
 
 Central directory entry #220:
 ---------------------------
 
   static/js/ace/snippets/mipsassembler.js
 
-  offset of local header from start of archive:   2015233
-                                                  (00000000001EC001h) bytes
+  offset of local header from start of archive:   2015269
+                                                  (00000000001EC025h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8155,16 +8155,16 @@
   There is no file comment.
 
 Central directory entry #221:
 ---------------------------
 
   static/js/ace/snippets/liquid.js
 
-  offset of local header from start of archive:   2015443
-                                                  (00000000001EC0D3h) bytes
+  offset of local header from start of archive:   2015479
+                                                  (00000000001EC0F7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8192,16 +8192,16 @@
   There is no file comment.
 
 Central directory entry #222:
 ---------------------------
 
   static/js/ace/snippets/jack.js
 
-  offset of local header from start of archive:   2015643
-                                                  (00000000001EC19Bh) bytes
+  offset of local header from start of archive:   2015679
+                                                  (00000000001EC1BFh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8229,16 +8229,16 @@
   There is no file comment.
 
 Central directory entry #223:
 ---------------------------
 
   static/js/ace/snippets/rhtml.js
 
-  offset of local header from start of archive:   2015841
-                                                  (00000000001EC261h) bytes
+  offset of local header from start of archive:   2015877
+                                                  (00000000001EC285h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8266,16 +8266,16 @@
   There is no file comment.
 
 Central directory entry #224:
 ---------------------------
 
   static/js/ace/snippets/handlebars.js
 
-  offset of local header from start of archive:   2016040
-                                                  (00000000001EC328h) bytes
+  offset of local header from start of archive:   2016076
+                                                  (00000000001EC34Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8303,16 +8303,16 @@
   There is no file comment.
 
 Central directory entry #225:
 ---------------------------
 
   static/js/ace/snippets/xml.js
 
-  offset of local header from start of archive:   2016249
-                                                  (00000000001EC3F9h) bytes
+  offset of local header from start of archive:   2016285
+                                                  (00000000001EC41Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8340,16 +8340,16 @@
   There is no file comment.
 
 Central directory entry #226:
 ---------------------------
 
   static/js/ace/snippets/abap.js
 
-  offset of local header from start of archive:   2016445
-                                                  (00000000001EC4BDh) bytes
+  offset of local header from start of archive:   2016481
+                                                  (00000000001EC4E1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8377,16 +8377,16 @@
   There is no file comment.
 
 Central directory entry #227:
 ---------------------------
 
   static/js/ace/snippets/elixir.js
 
-  offset of local header from start of archive:   2016643
-                                                  (00000000001EC583h) bytes
+  offset of local header from start of archive:   2016679
+                                                  (00000000001EC5A7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8414,16 +8414,16 @@
   There is no file comment.
 
 Central directory entry #228:
 ---------------------------
 
   static/js/ace/snippets/forth.js
 
-  offset of local header from start of archive:   2016842
-                                                  (00000000001EC64Ah) bytes
+  offset of local header from start of archive:   2016878
+                                                  (00000000001EC66Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8451,16 +8451,16 @@
   There is no file comment.
 
 Central directory entry #229:
 ---------------------------
 
   static/js/ace/snippets/apache_conf.js
 
-  offset of local header from start of archive:   2017041
-                                                  (00000000001EC711h) bytes
+  offset of local header from start of archive:   2017077
+                                                  (00000000001EC735h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8488,16 +8488,16 @@
   There is no file comment.
 
 Central directory entry #230:
 ---------------------------
 
   static/js/ace/snippets/julia.js
 
-  offset of local header from start of archive:   2017251
-                                                  (00000000001EC7E3h) bytes
+  offset of local header from start of archive:   2017287
+                                                  (00000000001EC807h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8525,16 +8525,16 @@
   There is no file comment.
 
 Central directory entry #231:
 ---------------------------
 
   static/js/ace/snippets/haskell_cabal.js
 
-  offset of local header from start of archive:   2017450
-                                                  (00000000001EC8AAh) bytes
+  offset of local header from start of archive:   2017486
+                                                  (00000000001EC8CEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8562,16 +8562,16 @@
   There is no file comment.
 
 Central directory entry #232:
 ---------------------------
 
   static/js/ace/snippets/stylus.js
 
-  offset of local header from start of archive:   2017664
-                                                  (00000000001EC980h) bytes
+  offset of local header from start of archive:   2017700
+                                                  (00000000001EC9A4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8599,16 +8599,16 @@
   There is no file comment.
 
 Central directory entry #233:
 ---------------------------
 
   static/js/ace/snippets/sass.js
 
-  offset of local header from start of archive:   2017864
-                                                  (00000000001ECA48h) bytes
+  offset of local header from start of archive:   2017900
+                                                  (00000000001ECA6Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8636,16 +8636,16 @@
   There is no file comment.
 
 Central directory entry #234:
 ---------------------------
 
   static/js/ace/snippets/django.js
 
-  offset of local header from start of archive:   2018061
-                                                  (00000000001ECB0Dh) bytes
+  offset of local header from start of archive:   2018097
+                                                  (00000000001ECB31h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8673,16 +8673,16 @@
   There is no file comment.
 
 Central directory entry #235:
 ---------------------------
 
   static/js/ace/snippets/coldfusion.js
 
-  offset of local header from start of archive:   2019450
-                                                  (00000000001ED07Ah) bytes
+  offset of local header from start of archive:   2019486
+                                                  (00000000001ED09Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8710,16 +8710,16 @@
   There is no file comment.
 
 Central directory entry #236:
 ---------------------------
 
   static/js/ace/snippets/javascript.js
 
-  offset of local header from start of archive:   2019658
-                                                  (00000000001ED14Ah) bytes
+  offset of local header from start of archive:   2019694
+                                                  (00000000001ED16Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8747,16 +8747,16 @@
   There is no file comment.
 
 Central directory entry #237:
 ---------------------------
 
   static/js/ace/snippets/sh.js
 
-  offset of local header from start of archive:   2021212
-                                                  (00000000001ED75Ch) bytes
+  offset of local header from start of archive:   2021248
+                                                  (00000000001ED780h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8784,16 +8784,16 @@
   There is no file comment.
 
 Central directory entry #238:
 ---------------------------
 
   static/js/ace/snippets/ftl.js
 
-  offset of local header from start of archive:   2022146
-                                                  (00000000001EDB02h) bytes
+  offset of local header from start of archive:   2022182
+                                                  (00000000001EDB26h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8821,16 +8821,16 @@
   There is no file comment.
 
 Central directory entry #239:
 ---------------------------
 
   static/js/ace/snippets/space.js
 
-  offset of local header from start of archive:   2022342
-                                                  (00000000001EDBC6h) bytes
+  offset of local header from start of archive:   2022378
+                                                  (00000000001EDBEAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8858,16 +8858,16 @@
   There is no file comment.
 
 Central directory entry #240:
 ---------------------------
 
   static/js/ace/snippets/luapage.js
 
-  offset of local header from start of archive:   2022540
-                                                  (00000000001EDC8Ch) bytes
+  offset of local header from start of archive:   2022576
+                                                  (00000000001EDCB0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8895,16 +8895,16 @@
   There is no file comment.
 
 Central directory entry #241:
 ---------------------------
 
   static/js/ace/snippets/markdown.js
 
-  offset of local header from start of archive:   2022743
-                                                  (00000000001EDD57h) bytes
+  offset of local header from start of archive:   2022779
+                                                  (00000000001EDD7Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8932,16 +8932,16 @@
   There is no file comment.
 
 Central directory entry #242:
 ---------------------------
 
   static/js/ace/keybinding-vim.js
 
-  offset of local header from start of archive:   2023545
-                                                  (00000000001EE079h) bytes
+  offset of local header from start of archive:   2023581
+                                                  (00000000001EE09Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -8969,16 +8969,16 @@
   There is no file comment.
 
 Central directory entry #243:
 ---------------------------
 
   static/js/ace/mode-forth.js
 
-  offset of local header from start of archive:   2052997
-                                                  (00000000001F5385h) bytes
+  offset of local header from start of archive:   2053033
+                                                  (00000000001F53A9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9006,16 +9006,16 @@
   There is no file comment.
 
 Central directory entry #244:
 ---------------------------
 
   static/js/ace/mode-sh.js
 
-  offset of local header from start of archive:   2055488
-                                                  (00000000001F5D40h) bytes
+  offset of local header from start of archive:   2055524
+                                                  (00000000001F5D64h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9043,16 +9043,16 @@
   There is no file comment.
 
 Central directory entry #245:
 ---------------------------
 
   static/js/ace/ext-whitespace.js
 
-  offset of local header from start of archive:   2058236
-                                                  (00000000001F67FCh) bytes
+  offset of local header from start of archive:   2058272
+                                                  (00000000001F6820h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9080,16 +9080,16 @@
   There is no file comment.
 
 Central directory entry #246:
 ---------------------------
 
   static/js/ace/mode-apache_conf.js
 
-  offset of local header from start of archive:   2059491
-                                                  (00000000001F6CE3h) bytes
+  offset of local header from start of archive:   2059527
+                                                  (00000000001F6D07h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9117,16 +9117,16 @@
   There is no file comment.
 
 Central directory entry #247:
 ---------------------------
 
   static/js/ace/mode-mushcode.js
 
-  offset of local header from start of archive:   2063978
-                                                  (00000000001F7E6Ah) bytes
+  offset of local header from start of archive:   2064014
+                                                  (00000000001F7E8Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9154,16 +9154,16 @@
   There is no file comment.
 
 Central directory entry #248:
 ---------------------------
 
   static/js/ace/mode-toml.js
 
-  offset of local header from start of archive:   2067067
-                                                  (00000000001F8A7Bh) bytes
+  offset of local header from start of archive:   2067103
+                                                  (00000000001F8A9Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9191,16 +9191,16 @@
   There is no file comment.
 
 Central directory entry #249:
 ---------------------------
 
   static/js/ace/mode-sql.js
 
-  offset of local header from start of archive:   2068031
-                                                  (00000000001F8E3Fh) bytes
+  offset of local header from start of archive:   2068067
+                                                  (00000000001F8E63h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9228,16 +9228,16 @@
   There is no file comment.
 
 Central directory entry #250:
 ---------------------------
 
   static/js/ace/mode-vhdl.js
 
-  offset of local header from start of archive:   2068990
-                                                  (00000000001F91FEh) bytes
+  offset of local header from start of archive:   2069026
+                                                  (00000000001F9222h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9265,16 +9265,16 @@
   There is no file comment.
 
 Central directory entry #251:
 ---------------------------
 
   static/js/ace/mode-lua.js
 
-  offset of local header from start of archive:   2070064
-                                                  (00000000001F9630h) bytes
+  offset of local header from start of archive:   2070100
+                                                  (00000000001F9654h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9302,16 +9302,16 @@
   There is no file comment.
 
 Central directory entry #252:
 ---------------------------
 
   static/js/ace/mode-assembly_x86.js
 
-  offset of local header from start of archive:   2072951
-                                                  (00000000001FA177h) bytes
+  offset of local header from start of archive:   2072987
+                                                  (00000000001FA19Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9339,16 +9339,16 @@
   There is no file comment.
 
 Central directory entry #253:
 ---------------------------
 
   static/js/ace/mode-glsl.js
 
-  offset of local header from start of archive:   2076406
-                                                  (00000000001FAEF6h) bytes
+  offset of local header from start of archive:   2076442
+                                                  (00000000001FAF1Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9376,16 +9376,16 @@
   There is no file comment.
 
 Central directory entry #254:
 ---------------------------
 
   static/js/ace/theme-terminal.js
 
-  offset of local header from start of archive:   2080926
-                                                  (00000000001FC09Eh) bytes
+  offset of local header from start of archive:   2080962
+                                                  (00000000001FC0C2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9413,16 +9413,16 @@
   There is no file comment.
 
 Central directory entry #255:
 ---------------------------
 
   static/js/ace/mode-cirru.js
 
-  offset of local header from start of archive:   2081901
-                                                  (00000000001FC46Dh) bytes
+  offset of local header from start of archive:   2081937
+                                                  (00000000001FC491h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9450,16 +9450,16 @@
   There is no file comment.
 
 Central directory entry #256:
 ---------------------------
 
   static/js/ace/mode-scala.js
 
-  offset of local header from start of archive:   2082920
-                                                  (00000000001FC868h) bytes
+  offset of local header from start of archive:   2082956
+                                                  (00000000001FC88Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9487,16 +9487,16 @@
   There is no file comment.
 
 Central directory entry #257:
 ---------------------------
 
   static/js/ace/mode-jsx.js
 
-  offset of local header from start of archive:   2090711
-                                                  (00000000001FE6D7h) bytes
+  offset of local header from start of archive:   2090747
+                                                  (00000000001FE6FBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9524,16 +9524,16 @@
   There is no file comment.
 
 Central directory entry #258:
 ---------------------------
 
   static/js/ace/mode-coldfusion.js
 
-  offset of local header from start of archive:   2093300
-                                                  (00000000001FF0F4h) bytes
+  offset of local header from start of archive:   2093336
+                                                  (00000000001FF118h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9561,16 +9561,16 @@
   There is no file comment.
 
 Central directory entry #259:
 ---------------------------
 
   static/js/ace/mode-sass.js
 
-  offset of local header from start of archive:   2111001
-                                                  (0000000000203619h) bytes
+  offset of local header from start of archive:   2111037
+                                                  (000000000020363Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9598,16 +9598,16 @@
   There is no file comment.
 
 Central directory entry #260:
 ---------------------------
 
   static/js/ace/theme-github.js
 
-  offset of local header from start of archive:   2114859
-                                                  (000000000020452Bh) bytes
+  offset of local header from start of archive:   2114895
+                                                  (000000000020454Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9635,16 +9635,16 @@
   There is no file comment.
 
 Central directory entry #261:
 ---------------------------
 
   static/js/ace/mode-svg.js
 
-  offset of local header from start of archive:   2115748
-                                                  (00000000002048A4h) bytes
+  offset of local header from start of archive:   2115784
+                                                  (00000000002048C8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9672,16 +9672,16 @@
   There is no file comment.
 
 Central directory entry #262:
 ---------------------------
 
   static/js/ace/mode-scss.js
 
-  offset of local header from start of archive:   2125010
-                                                  (0000000000206CD2h) bytes
+  offset of local header from start of archive:   2125046
+                                                  (0000000000206CF6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9709,16 +9709,16 @@
   There is no file comment.
 
 Central directory entry #263:
 ---------------------------
 
   static/js/ace/ace.js
 
-  offset of local header from start of archive:   2129766
-                                                  (0000000000207F66h) bytes
+  offset of local header from start of archive:   2129802
+                                                  (0000000000207F8Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9746,16 +9746,16 @@
   There is no file comment.
 
 Central directory entry #264:
 ---------------------------
 
   static/js/ace/mode-tex.js
 
-  offset of local header from start of archive:   2228773
-                                                  (0000000000220225h) bytes
+  offset of local header from start of archive:   2228809
+                                                  (0000000000220249h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9783,16 +9783,16 @@
   There is no file comment.
 
 Central directory entry #265:
 ---------------------------
 
   static/js/ace/mode-io.js
 
-  offset of local header from start of archive:   2229742
-                                                  (00000000002205EEh) bytes
+  offset of local header from start of archive:   2229778
+                                                  (0000000000220612h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9820,16 +9820,16 @@
   There is no file comment.
 
 Central directory entry #266:
 ---------------------------
 
   static/js/ace/mode-drools.js
 
-  offset of local header from start of archive:   2231879
-                                                  (0000000000220E47h) bytes
+  offset of local header from start of archive:   2231915
+                                                  (0000000000220E6Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9857,16 +9857,16 @@
   There is no file comment.
 
 Central directory entry #267:
 ---------------------------
 
   static/js/ace/theme-monokai.js
 
-  offset of local header from start of archive:   2234935
-                                                  (0000000000221A37h) bytes
+  offset of local header from start of archive:   2234971
+                                                  (0000000000221A5Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9894,16 +9894,16 @@
   There is no file comment.
 
 Central directory entry #268:
 ---------------------------
 
   static/js/ace/theme-eclipse.js
 
-  offset of local header from start of archive:   2235854
-                                                  (0000000000221DCEh) bytes
+  offset of local header from start of archive:   2235890
+                                                  (0000000000221DF2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9931,16 +9931,16 @@
   There is no file comment.
 
 Central directory entry #269:
 ---------------------------
 
   static/js/ace/mode-protobuf.js
 
-  offset of local header from start of archive:   2236723
-                                                  (0000000000222133h) bytes
+  offset of local header from start of archive:   2236759
+                                                  (0000000000222157h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -9968,16 +9968,16 @@
   There is no file comment.
 
 Central directory entry #270:
 ---------------------------
 
   static/js/ace/mode-ruby.js
 
-  offset of local header from start of archive:   2240940
-                                                  (00000000002231ACh) bytes
+  offset of local header from start of archive:   2240976
+                                                  (00000000002231D0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10005,16 +10005,16 @@
   There is no file comment.
 
 Central directory entry #271:
 ---------------------------
 
   static/js/ace/theme-chaos.js
 
-  offset of local header from start of archive:   2244801
-                                                  (00000000002240C1h) bytes
+  offset of local header from start of archive:   2244837
+                                                  (00000000002240E5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10042,16 +10042,16 @@
   There is no file comment.
 
 Central directory entry #272:
 ---------------------------
 
   static/js/ace/ext-linking.js
 
-  offset of local header from start of archive:   2245803
-                                                  (00000000002244ABh) bytes
+  offset of local header from start of archive:   2245839
+                                                  (00000000002244CFh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10079,16 +10079,16 @@
   There is no file comment.
 
 Central directory entry #273:
 ---------------------------
 
   static/js/ace/ext-statusbar.js
 
-  offset of local header from start of archive:   2246273
-                                                  (0000000000224681h) bytes
+  offset of local header from start of archive:   2246309
+                                                  (00000000002246A5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10116,16 +10116,16 @@
   There is no file comment.
 
 Central directory entry #274:
 ---------------------------
 
   static/js/ace/worker-html.js
 
-  offset of local header from start of archive:   2246907
-                                                  (00000000002248FBh) bytes
+  offset of local header from start of archive:   2246943
+                                                  (000000000022491Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10153,16 +10153,16 @@
   There is no file comment.
 
 Central directory entry #275:
 ---------------------------
 
   static/js/ace/mode-nsis.js
 
-  offset of local header from start of archive:   2296990
-                                                  (0000000000230C9Eh) bytes
+  offset of local header from start of archive:   2297026
+                                                  (0000000000230CC2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10190,16 +10190,16 @@
   There is no file comment.
 
 Central directory entry #276:
 ---------------------------
 
   static/js/ace/worker-php.js
 
-  offset of local header from start of archive:   2300890
-                                                  (0000000000231BDAh) bytes
+  offset of local header from start of archive:   2300926
+                                                  (0000000000231BFEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10227,16 +10227,16 @@
   There is no file comment.
 
 Central directory entry #277:
 ---------------------------
 
   static/js/ace/mode-objectivec.js
 
-  offset of local header from start of archive:   2322541
-                                                  (000000000023706Dh) bytes
+  offset of local header from start of archive:   2322577
+                                                  (0000000000237091h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10264,16 +10264,16 @@
   There is no file comment.
 
 Central directory entry #278:
 ---------------------------
 
   static/js/ace/ext-spellcheck.js
 
-  offset of local header from start of archive:   2340761
-                                                  (000000000023B799h) bytes
+  offset of local header from start of archive:   2340797
+                                                  (000000000023B7BDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10301,16 +10301,16 @@
   There is no file comment.
 
 Central directory entry #279:
 ---------------------------
 
   static/js/ace/mode-javascript.js
 
-  offset of local header from start of archive:   2341485
-                                                  (000000000023BA6Dh) bytes
+  offset of local header from start of archive:   2341521
+                                                  (000000000023BA91h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10338,16 +10338,16 @@
   There is no file comment.
 
 Central directory entry #280:
 ---------------------------
 
   static/js/ace/mode-praat.js
 
-  offset of local header from start of archive:   2347853
-                                                  (000000000023D34Dh) bytes
+  offset of local header from start of archive:   2347889
+                                                  (000000000023D371h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10375,16 +10375,16 @@
   There is no file comment.
 
 Central directory entry #281:
 ---------------------------
 
   static/js/ace/mode-matlab.js
 
-  offset of local header from start of archive:   2351722
-                                                  (000000000023E26Ah) bytes
+  offset of local header from start of archive:   2351758
+                                                  (000000000023E28Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10412,16 +10412,16 @@
   There is no file comment.
 
 Central directory entry #282:
 ---------------------------
 
   static/js/ace/mode-plain_text.js
 
-  offset of local header from start of archive:   2360717
-                                                  (000000000024058Dh) bytes
+  offset of local header from start of archive:   2360753
+                                                  (00000000002405B1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10449,16 +10449,16 @@
   There is no file comment.
 
 Central directory entry #283:
 ---------------------------
 
   static/js/ace/mode-mel.js
 
-  offset of local header from start of archive:   2361073
-                                                  (00000000002406F1h) bytes
+  offset of local header from start of archive:   2361109
+                                                  (0000000000240715h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10486,16 +10486,16 @@
   There is no file comment.
 
 Central directory entry #284:
 ---------------------------
 
   static/js/ace/mode-rdoc.js
 
-  offset of local header from start of archive:   2371724
-                                                  (000000000024308Ch) bytes
+  offset of local header from start of archive:   2371760
+                                                  (00000000002430B0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10523,16 +10523,16 @@
   There is no file comment.
 
 Central directory entry #285:
 ---------------------------
 
   static/js/ace/theme-tomorrow_night.js
 
-  offset of local header from start of archive:   2372975
-                                                  (000000000024356Fh) bytes
+  offset of local header from start of archive:   2373011
+                                                  (0000000000243593h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10560,16 +10560,16 @@
   There is no file comment.
 
 Central directory entry #286:
 ---------------------------
 
   static/js/ace/mode-groovy.js
 
-  offset of local header from start of archive:   2373937
-                                                  (0000000000243931h) bytes
+  offset of local header from start of archive:   2373973
+                                                  (0000000000243955h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10597,16 +10597,16 @@
   There is no file comment.
 
 Central directory entry #287:
 ---------------------------
 
   static/js/ace/mode-markdown.js
 
-  offset of local header from start of archive:   2381570
-                                                  (0000000000245702h) bytes
+  offset of local header from start of archive:   2381606
+                                                  (0000000000245726h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10634,16 +10634,16 @@
   There is no file comment.
 
 Central directory entry #288:
 ---------------------------
 
   static/js/ace/mode-mysql.js
 
-  offset of local header from start of archive:   2400224
-                                                  (0000000000249FE0h) bytes
+  offset of local header from start of archive:   2400260
+                                                  (000000000024A004h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10671,16 +10671,16 @@
   There is no file comment.
 
 Central directory entry #289:
 ---------------------------
 
   static/js/ace/mode-batchfile.js
 
-  offset of local header from start of archive:   2403100
-                                                  (000000000024AB1Ch) bytes
+  offset of local header from start of archive:   2403136
+                                                  (000000000024AB40h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10708,16 +10708,16 @@
   There is no file comment.
 
 Central directory entry #290:
 ---------------------------
 
   static/js/ace/mode-gitignore.js
 
-  offset of local header from start of archive:   2405010
-                                                  (000000000024B292h) bytes
+  offset of local header from start of archive:   2405046
+                                                  (000000000024B2B6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10745,16 +10745,16 @@
   There is no file comment.
 
 Central directory entry #291:
 ---------------------------
 
   static/js/ace/mode-julia.js
 
-  offset of local header from start of archive:   2405471
-                                                  (000000000024B45Fh) bytes
+  offset of local header from start of archive:   2405507
+                                                  (000000000024B483h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10782,16 +10782,16 @@
   There is no file comment.
 
 Central directory entry #292:
 ---------------------------
 
   static/js/ace/theme-kr_theme.js
 
-  offset of local header from start of archive:   2407954
-                                                  (000000000024BE12h) bytes
+  offset of local header from start of archive:   2407990
+                                                  (000000000024BE36h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10819,16 +10819,16 @@
   There is no file comment.
 
 Central directory entry #293:
 ---------------------------
 
   static/js/ace/ext-error_marker.js
 
-  offset of local header from start of archive:   2408886
-                                                  (000000000024C1B6h) bytes
+  offset of local header from start of archive:   2408922
+                                                  (000000000024C1DAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10856,16 +10856,16 @@
   There is no file comment.
 
 Central directory entry #294:
 ---------------------------
 
   static/js/ace/mode-json.js
 
-  offset of local header from start of archive:   2409049
-                                                  (000000000024C259h) bytes
+  offset of local header from start of archive:   2409085
+                                                  (000000000024C27Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10893,16 +10893,16 @@
   There is no file comment.
 
 Central directory entry #295:
 ---------------------------
 
   static/js/ace/mode-soy_template.js
 
-  offset of local header from start of archive:   2410896
-                                                  (000000000024C990h) bytes
+  offset of local header from start of archive:   2410932
+                                                  (000000000024C9B4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10930,16 +10930,16 @@
   There is no file comment.
 
 Central directory entry #296:
 ---------------------------
 
   static/js/ace/ext-settings_menu.js
 
-  offset of local header from start of archive:   2429522
-                                                  (0000000000251252h) bytes
+  offset of local header from start of archive:   2429558
+                                                  (0000000000251276h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -10967,16 +10967,16 @@
   There is no file comment.
 
 Central directory entry #297:
 ---------------------------
 
   static/js/ace/mode-vala.js
 
-  offset of local header from start of archive:   2434357
-                                                  (0000000000252535h) bytes
+  offset of local header from start of archive:   2434393
+                                                  (0000000000252559h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11004,16 +11004,16 @@
   There is no file comment.
 
 Central directory entry #298:
 ---------------------------
 
   static/js/ace/mode-logiql.js
 
-  offset of local header from start of archive:   2438793
-                                                  (0000000000253689h) bytes
+  offset of local header from start of archive:   2438829
+                                                  (00000000002536ADh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11041,16 +11041,16 @@
   There is no file comment.
 
 Central directory entry #299:
 ---------------------------
 
   static/js/ace/mode-abap.js
 
-  offset of local header from start of archive:   2440879
-                                                  (0000000000253EAFh) bytes
+  offset of local header from start of archive:   2440915
+                                                  (0000000000253ED3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11078,16 +11078,16 @@
   There is no file comment.
 
 Central directory entry #300:
 ---------------------------
 
   static/js/ace/mode-lisp.js
 
-  offset of local header from start of archive:   2443523
-                                                  (0000000000254903h) bytes
+  offset of local header from start of archive:   2443559
+                                                  (0000000000254927h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11115,16 +11115,16 @@
   There is no file comment.
 
 Central directory entry #301:
 ---------------------------
 
   static/js/ace/mode-dart.js
 
-  offset of local header from start of archive:   2444434
-                                                  (0000000000254C92h) bytes
+  offset of local header from start of archive:   2444470
+                                                  (0000000000254CB6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11152,16 +11152,16 @@
   There is no file comment.
 
 Central directory entry #302:
 ---------------------------
 
   static/js/ace/ext-themelist.js
 
-  offset of local header from start of archive:   2449082
-                                                  (0000000000255EBAh) bytes
+  offset of local header from start of archive:   2449118
+                                                  (0000000000255EDEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11189,16 +11189,16 @@
   There is no file comment.
 
 Central directory entry #303:
 ---------------------------
 
   static/js/ace/theme-idle_fingers.js
 
-  offset of local header from start of archive:   2449803
-                                                  (000000000025618Bh) bytes
+  offset of local header from start of archive:   2449839
+                                                  (00000000002561AFh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11226,16 +11226,16 @@
   There is no file comment.
 
 Central directory entry #304:
 ---------------------------
 
   static/js/ace/ext-searchbox.js
 
-  offset of local header from start of archive:   2450696
-                                                  (0000000000256508h) bytes
+  offset of local header from start of archive:   2450732
+                                                  (000000000025652Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11263,16 +11263,16 @@
   There is no file comment.
 
 Central directory entry #305:
 ---------------------------
 
   static/js/ace/mode-ini.js
 
-  offset of local header from start of archive:   2453876
-                                                  (0000000000257174h) bytes
+  offset of local header from start of archive:   2453912
+                                                  (0000000000257198h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11300,16 +11300,16 @@
   There is no file comment.
 
 Central directory entry #306:
 ---------------------------
 
   static/js/ace/mode-c_cpp.js
 
-  offset of local header from start of archive:   2454955
-                                                  (00000000002575ABh) bytes
+  offset of local header from start of archive:   2454991
+                                                  (00000000002575CFh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11337,16 +11337,16 @@
   There is no file comment.
 
 Central directory entry #307:
 ---------------------------
 
   static/js/ace/worker-lua.js
 
-  offset of local header from start of archive:   2458881
-                                                  (0000000000258501h) bytes
+  offset of local header from start of archive:   2458917
+                                                  (0000000000258525h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11374,16 +11374,16 @@
   There is no file comment.
 
 Central directory entry #308:
 ---------------------------
 
   static/js/ace/theme-crimson_editor.js
 
-  offset of local header from start of archive:   2472943
-                                                  (000000000025BBEFh) bytes
+  offset of local header from start of archive:   2472979
+                                                  (000000000025BC13h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11411,16 +11411,16 @@
   There is no file comment.
 
 Central directory entry #309:
 ---------------------------
 
   static/js/ace/mode-tsx.js
 
-  offset of local header from start of archive:   2473936
-                                                  (000000000025BFD0h) bytes
+  offset of local header from start of archive:   2473972
+                                                  (000000000025BFF4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11448,16 +11448,16 @@
   There is no file comment.
 
 Central directory entry #310:
 ---------------------------
 
   static/js/ace/mode-handlebars.js
 
-  offset of local header from start of archive:   2480726
-                                                  (000000000025DA56h) bytes
+  offset of local header from start of archive:   2480762
+                                                  (000000000025DA7Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11485,16 +11485,16 @@
   There is no file comment.
 
 Central directory entry #311:
 ---------------------------
 
   static/js/ace/ext-language_tools.js
 
-  offset of local header from start of archive:   2498159
-                                                  (0000000000261E6Fh) bytes
+  offset of local header from start of archive:   2498195
+                                                  (0000000000261E93h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11522,16 +11522,16 @@
   There is no file comment.
 
 Central directory entry #312:
 ---------------------------
 
   static/js/ace/mode-typescript.js
 
-  offset of local header from start of archive:   2509158
-                                                  (0000000000264966h) bytes
+  offset of local header from start of archive:   2509194
+                                                  (000000000026498Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11559,16 +11559,16 @@
   There is no file comment.
 
 Central directory entry #313:
 ---------------------------
 
   static/js/ace/mode-lean.js
 
-  offset of local header from start of archive:   2515899
-                                                  (00000000002663BBh) bytes
+  offset of local header from start of archive:   2515935
+                                                  (00000000002663DFh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11596,16 +11596,16 @@
   There is no file comment.
 
 Central directory entry #314:
 ---------------------------
 
   static/js/ace/mode-verilog.js
 
-  offset of local header from start of archive:   2518079
-                                                  (0000000000266C3Fh) bytes
+  offset of local header from start of archive:   2518115
+                                                  (0000000000266C63h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11633,16 +11633,16 @@
   There is no file comment.
 
 Central directory entry #315:
 ---------------------------
 
   static/js/ace/theme-vibrant_ink.js
 
-  offset of local header from start of archive:   2519319
-                                                  (0000000000267117h) bytes
+  offset of local header from start of archive:   2519355
+                                                  (000000000026713Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11670,16 +11670,16 @@
   There is no file comment.
 
 Central directory entry #316:
 ---------------------------
 
   static/js/ace/mode-jack.js
 
-  offset of local header from start of archive:   2520179
-                                                  (0000000000267473h) bytes
+  offset of local header from start of archive:   2520215
+                                                  (0000000000267497h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11707,16 +11707,16 @@
   There is no file comment.
 
 Central directory entry #317:
 ---------------------------
 
   static/js/ace/mode-liquid.js
 
-  offset of local header from start of archive:   2522269
-                                                  (0000000000267C9Dh) bytes
+  offset of local header from start of archive:   2522305
+                                                  (0000000000267CC1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11744,16 +11744,16 @@
   There is no file comment.
 
 Central directory entry #318:
 ---------------------------
 
   static/js/ace/mode-razor.js
 
-  offset of local header from start of archive:   2531713
-                                                  (000000000026A181h) bytes
+  offset of local header from start of archive:   2531749
+                                                  (000000000026A1A5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11781,16 +11781,16 @@
   There is no file comment.
 
 Central directory entry #319:
 ---------------------------
 
   static/js/ace/mode-snippets.js
 
-  offset of local header from start of archive:   2550765
-                                                  (000000000026EBEDh) bytes
+  offset of local header from start of archive:   2550801
+                                                  (000000000026EC11h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11818,16 +11818,16 @@
   There is no file comment.
 
 Central directory entry #320:
 ---------------------------
 
   static/js/ace/mode-maze.js
 
-  offset of local header from start of archive:   2552189
-                                                  (000000000026F17Dh) bytes
+  offset of local header from start of archive:   2552225
+                                                  (000000000026F1A1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11855,16 +11855,16 @@
   There is no file comment.
 
 Central directory entry #321:
 ---------------------------
 
   static/js/ace/ext-textarea.js
 
-  offset of local header from start of archive:   2553879
-                                                  (000000000026F817h) bytes
+  offset of local header from start of archive:   2553915
+                                                  (000000000026F83Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11892,16 +11892,16 @@
   There is no file comment.
 
 Central directory entry #322:
 ---------------------------
 
   static/js/ace/mode-haskell.js
 
-  offset of local header from start of archive:   2557576
-                                                  (0000000000270688h) bytes
+  offset of local header from start of archive:   2557612
+                                                  (00000000002706ACh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11929,16 +11929,16 @@
   There is no file comment.
 
 Central directory entry #323:
 ---------------------------
 
   static/js/ace/mode-bro.js
 
-  offset of local header from start of archive:   2561381
-                                                  (0000000000271565h) bytes
+  offset of local header from start of archive:   2561417
+                                                  (0000000000271589h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -11966,16 +11966,16 @@
   There is no file comment.
 
 Central directory entry #324:
 ---------------------------
 
   static/js/ace/mode-lsl.js
 
-  offset of local header from start of archive:   2563674
-                                                  (0000000000271E5Ah) bytes
+  offset of local header from start of archive:   2563710
+                                                  (0000000000271E7Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12003,16 +12003,16 @@
   There is no file comment.
 
 Central directory entry #325:
 ---------------------------
 
   static/js/ace/mode-ejs.js
 
-  offset of local header from start of archive:   2572583
-                                                  (0000000000274127h) bytes
+  offset of local header from start of archive:   2572619
+                                                  (000000000027414Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12040,16 +12040,16 @@
   There is no file comment.
 
 Central directory entry #326:
 ---------------------------
 
   static/js/ace/theme-ambiance.js
 
-  offset of local header from start of archive:   2592977
-                                                  (00000000002790D1h) bytes
+  offset of local header from start of archive:   2593013
+                                                  (00000000002790F5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12077,16 +12077,16 @@
   There is no file comment.
 
 Central directory entry #327:
 ---------------------------
 
   static/js/ace/ext-old_ie.js
 
-  offset of local header from start of archive:   2612377
-                                                  (000000000027DC99h) bytes
+  offset of local header from start of archive:   2612413
+                                                  (000000000027DCBDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12114,16 +12114,16 @@
   There is no file comment.
 
 Central directory entry #328:
 ---------------------------
 
   static/js/ace/mode-lucene.js
 
-  offset of local header from start of archive:   2616304
-                                                  (000000000027EBF0h) bytes
+  offset of local header from start of archive:   2616340
+                                                  (000000000027EC14h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12151,16 +12151,16 @@
   There is no file comment.
 
 Central directory entry #329:
 ---------------------------
 
   static/js/ace/mode-coffee.js
 
-  offset of local header from start of archive:   2616835
-                                                  (000000000027EE03h) bytes
+  offset of local header from start of archive:   2616871
+                                                  (000000000027EE27h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12188,16 +12188,16 @@
   There is no file comment.
 
 Central directory entry #330:
 ---------------------------
 
   static/js/ace/mode-haml.js
 
-  offset of local header from start of archive:   2619637
-                                                  (000000000027F8F5h) bytes
+  offset of local header from start of archive:   2619673
+                                                  (000000000027F919h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12225,16 +12225,16 @@
   There is no file comment.
 
 Central directory entry #331:
 ---------------------------
 
   static/js/ace/mode-haskell_cabal.js
 
-  offset of local header from start of archive:   2631160
-                                                  (00000000002825F8h) bytes
+  offset of local header from start of archive:   2631196
+                                                  (000000000028261Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12262,16 +12262,16 @@
   There is no file comment.
 
 Central directory entry #332:
 ---------------------------
 
   static/js/ace/mode-css.js
 
-  offset of local header from start of archive:   2632097
-                                                  (00000000002829A1h) bytes
+  offset of local header from start of archive:   2632133
+                                                  (00000000002829C5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12299,16 +12299,16 @@
   There is no file comment.
 
 Central directory entry #333:
 ---------------------------
 
   static/js/ace/theme-merbivore_soft.js
 
-  offset of local header from start of archive:   2638255
-                                                  (00000000002841AFh) bytes
+  offset of local header from start of archive:   2638291
+                                                  (00000000002841D3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12336,16 +12336,16 @@
   There is no file comment.
 
 Central directory entry #334:
 ---------------------------
 
   static/js/ace/mode-vbscript.js
 
-  offset of local header from start of archive:   2639156
-                                                  (0000000000284534h) bytes
+  offset of local header from start of archive:   2639192
+                                                  (0000000000284558h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12373,16 +12373,16 @@
   There is no file comment.
 
 Central directory entry #335:
 ---------------------------
 
   static/js/ace/mode-html_ruby.js
 
-  offset of local header from start of archive:   2641405
-                                                  (0000000000284DFDh) bytes
+  offset of local header from start of archive:   2641441
+                                                  (0000000000284E21h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12410,16 +12410,16 @@
   There is no file comment.
 
 Central directory entry #336:
 ---------------------------
 
   static/js/ace/mode-pgsql.js
 
-  offset of local header from start of archive:   2661507
-                                                  (0000000000289C83h) bytes
+  offset of local header from start of archive:   2661543
+                                                  (0000000000289CA7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12447,16 +12447,16 @@
   There is no file comment.
 
 Central directory entry #337:
 ---------------------------
 
   static/js/ace/mode-abc.js
 
-  offset of local header from start of archive:   2678962
-                                                  (000000000028E0B2h) bytes
+  offset of local header from start of archive:   2678998
+                                                  (000000000028E0D6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12484,16 +12484,16 @@
   There is no file comment.
 
 Central directory entry #338:
 ---------------------------
 
   static/js/ace/theme-tomorrow_night_eighties.js
 
-  offset of local header from start of archive:   2680644
-                                                  (000000000028E744h) bytes
+  offset of local header from start of archive:   2680680
+                                                  (000000000028E768h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12521,16 +12521,16 @@
   There is no file comment.
 
 Central directory entry #339:
 ---------------------------
 
   static/js/ace/ext-emmet.js
 
-  offset of local header from start of archive:   2681602
-                                                  (000000000028EB02h) bytes
+  offset of local header from start of archive:   2681638
+                                                  (000000000028EB26h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12558,16 +12558,16 @@
   There is no file comment.
 
 Central directory entry #340:
 ---------------------------
 
   static/js/ace/mode-html_elixir.js
 
-  offset of local header from start of archive:   2688954
-                                                  (00000000002907BAh) bytes
+  offset of local header from start of archive:   2688990
+                                                  (00000000002907DEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12595,16 +12595,16 @@
   There is no file comment.
 
 Central directory entry #341:
 ---------------------------
 
   static/js/ace/mode-erlang.js
 
-  offset of local header from start of archive:   2709197
-                                                  (00000000002956CDh) bytes
+  offset of local header from start of archive:   2709233
+                                                  (00000000002956F1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12632,16 +12632,16 @@
   There is no file comment.
 
 Central directory entry #342:
 ---------------------------
 
   static/js/ace/ext-keybinding_menu.js
 
-  offset of local header from start of archive:   2713991
-                                                  (0000000000296987h) bytes
+  offset of local header from start of archive:   2714027
+                                                  (00000000002969ABh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12669,16 +12669,16 @@
   There is no file comment.
 
 Central directory entry #343:
 ---------------------------
 
   static/js/ace/theme-dawn.js
 
-  offset of local header from start of archive:   2715546
-                                                  (0000000000296F9Ah) bytes
+  offset of local header from start of archive:   2715582
+                                                  (0000000000296FBEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12706,16 +12706,16 @@
   There is no file comment.
 
 Central directory entry #344:
 ---------------------------
 
   static/js/ace/mode-asciidoc.js
 
-  offset of local header from start of archive:   2716468
-                                                  (0000000000297334h) bytes
+  offset of local header from start of archive:   2716504
+                                                  (0000000000297358h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12743,16 +12743,16 @@
   There is no file comment.
 
 Central directory entry #345:
 ---------------------------
 
   static/js/ace/theme-pastel_on_dark.js
 
-  offset of local header from start of archive:   2719081
-                                                  (0000000000297D69h) bytes
+  offset of local header from start of archive:   2719117
+                                                  (0000000000297D8Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12780,16 +12780,16 @@
   There is no file comment.
 
 Central directory entry #346:
 ---------------------------
 
   static/js/ace/mode-swig.js
 
-  offset of local header from start of archive:   2720058
-                                                  (000000000029813Ah) bytes
+  offset of local header from start of archive:   2720094
+                                                  (000000000029815Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12817,16 +12817,16 @@
   There is no file comment.
 
 Central directory entry #347:
 ---------------------------
 
   static/js/ace/mode-swift.js
 
-  offset of local header from start of archive:   2729690
-                                                  (000000000029A6DAh) bytes
+  offset of local header from start of archive:   2729726
+                                                  (000000000029A6FEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12854,16 +12854,16 @@
   There is no file comment.
 
 Central directory entry #348:
 ---------------------------
 
   static/js/ace/mode-python.js
 
-  offset of local header from start of archive:   2732361
-                                                  (000000000029B149h) bytes
+  offset of local header from start of archive:   2732397
+                                                  (000000000029B16Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12891,16 +12891,16 @@
   There is no file comment.
 
 Central directory entry #349:
 ---------------------------
 
   static/js/ace/mode-livescript.js
 
-  offset of local header from start of archive:   2734326
-                                                  (000000000029B8F6h) bytes
+  offset of local header from start of archive:   2734362
+                                                  (000000000029B91Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12928,16 +12928,16 @@
   There is no file comment.
 
 Central directory entry #350:
 ---------------------------
 
   static/js/ace/theme-cobalt.js
 
-  offset of local header from start of archive:   2736382
-                                                  (000000000029C0FEh) bytes
+  offset of local header from start of archive:   2736418
+                                                  (000000000029C122h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -12965,16 +12965,16 @@
   There is no file comment.
 
 Central directory entry #351:
 ---------------------------
 
   static/js/ace/mode-django.js
 
-  offset of local header from start of archive:   2737320
-                                                  (000000000029C4A8h) bytes
+  offset of local header from start of archive:   2737356
+                                                  (000000000029C4CCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13002,16 +13002,16 @@
   There is no file comment.
 
 Central directory entry #352:
 ---------------------------
 
   static/js/ace/mode-xquery.js
 
-  offset of local header from start of archive:   2754698
-                                                  (00000000002A088Ah) bytes
+  offset of local header from start of archive:   2754734
+                                                  (00000000002A08AEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13039,16 +13039,16 @@
   There is no file comment.
 
 Central directory entry #353:
 ---------------------------
 
   static/js/ace/mode-scad.js
 
-  offset of local header from start of archive:   2790678
-                                                  (00000000002A9516h) bytes
+  offset of local header from start of archive:   2790714
+                                                  (00000000002A953Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13076,16 +13076,16 @@
   There is no file comment.
 
 Central directory entry #354:
 ---------------------------
 
   static/js/ace/theme-clouds_midnight.js
 
-  offset of local header from start of archive:   2792939
-                                                  (00000000002A9DEBh) bytes
+  offset of local header from start of archive:   2792975
+                                                  (00000000002A9E0Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13113,16 +13113,16 @@
   There is no file comment.
 
 Central directory entry #355:
 ---------------------------
 
   static/js/ace/ext-chromevox.js
 
-  offset of local header from start of archive:   2793834
-                                                  (00000000002AA16Ah) bytes
+  offset of local header from start of archive:   2793870
+                                                  (00000000002AA18Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13150,16 +13150,16 @@
   There is no file comment.
 
 Central directory entry #356:
 ---------------------------
 
   static/js/ace/theme-solarized_light.js
 
-  offset of local header from start of archive:   2796513
-                                                  (00000000002AABE1h) bytes
+  offset of local header from start of archive:   2796549
+                                                  (00000000002AAC05h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13187,16 +13187,16 @@
   There is no file comment.
 
 Central directory entry #357:
 ---------------------------
 
   static/js/ace/mode-nix.js
 
-  offset of local header from start of archive:   2797405
-                                                  (00000000002AAF5Dh) bytes
+  offset of local header from start of archive:   2797441
+                                                  (00000000002AAF81h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13224,16 +13224,16 @@
   There is no file comment.
 
 Central directory entry #358:
 ---------------------------
 
   static/js/ace/mode-luapage.js
 
-  offset of local header from start of archive:   2801725
-                                                  (00000000002AC03Dh) bytes
+  offset of local header from start of archive:   2801761
+                                                  (00000000002AC061h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13261,16 +13261,16 @@
   There is no file comment.
 
 Central directory entry #359:
 ---------------------------
 
   static/js/ace/theme-kuroir.js
 
-  offset of local header from start of archive:   2821241
-                                                  (00000000002B0C79h) bytes
+  offset of local header from start of archive:   2821277
+                                                  (00000000002B0C9Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13298,16 +13298,16 @@
   There is no file comment.
 
 Central directory entry #360:
 ---------------------------
 
   static/js/ace/mode-fortran.js
 
-  offset of local header from start of archive:   2822064
-                                                  (00000000002B0FB0h) bytes
+  offset of local header from start of archive:   2822100
+                                                  (00000000002B0FD4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13335,16 +13335,16 @@
   There is no file comment.
 
 Central directory entry #361:
 ---------------------------
 
   static/js/ace/theme-merbivore.js
 
-  offset of local header from start of archive:   2825710
-                                                  (00000000002B1DEEh) bytes
+  offset of local header from start of archive:   2825746
+                                                  (00000000002B1E12h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13372,16 +13372,16 @@
   There is no file comment.
 
 Central directory entry #362:
 ---------------------------
 
   static/js/ace/theme-tomorrow_night_bright.js
 
-  offset of local header from start of archive:   2826582
-                                                  (00000000002B2156h) bytes
+  offset of local header from start of archive:   2826618
+                                                  (00000000002B217Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13409,16 +13409,16 @@
   There is no file comment.
 
 Central directory entry #363:
 ---------------------------
 
   static/js/ace/mode-xml.js
 
-  offset of local header from start of archive:   2827643
-                                                  (00000000002B257Bh) bytes
+  offset of local header from start of archive:   2827679
+                                                  (00000000002B259Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13446,16 +13446,16 @@
   There is no file comment.
 
 Central directory entry #364:
 ---------------------------
 
   static/js/ace/mode-mips_assembler.js
 
-  offset of local header from start of archive:   2830970
-                                                  (00000000002B327Ah) bytes
+  offset of local header from start of archive:   2831006
+                                                  (00000000002B329Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13483,30 +13483,30 @@
   There is no file comment.
 
 Central directory entry #365:
 ---------------------------
 
   static/js/utils.js
 
-  offset of local header from start of archive:   2833253
-                                                  (00000000002B3B65h) bytes
+  offset of local header from start of archive:   2833289
+                                                  (00000000002B3B89h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 19 15:19:00
-  file last modified on (UT extra field modtime): 2023 Mar 19 22:18:59 local
-  file last modified on (UT extra field modtime): 2023 Mar 19 22:18:59 UTC
-  32-bit CRC value (hex):                         bc2e37ac
-  compressed size:                                4133 bytes
-  uncompressed size:                              11826 bytes
+  file last modified on (DOS date/time):          2023 Apr 16 17:36:22
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:36:22 local
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:36:22 UTC
+  32-bit CRC value (hex):                         84d306f5
+  compressed size:                                4147 bytes
+  uncompressed size:                              11888 bytes
   length of filename:                             18 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
@@ -13520,16 +13520,16 @@
   There is no file comment.
 
 Central directory entry #366:
 ---------------------------
 
   static/js/axios.min.js
 
-  offset of local header from start of archive:   2837462
-                                                  (00000000002B4BD6h) bytes
+  offset of local header from start of archive:   2837512
+                                                  (00000000002B4C08h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13557,16 +13557,16 @@
   There is no file comment.
 
 Central directory entry #367:
 ---------------------------
 
   static/js/dbadmin.js
 
-  offset of local header from start of archive:   2842456
-                                                  (00000000002B5F58h) bytes
+  offset of local header from start of archive:   2842506
+                                                  (00000000002B5F8Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13594,16 +13594,16 @@
   There is no file comment.
 
 Central directory entry #368:
 ---------------------------
 
   static/js/vue.min.js
 
-  offset of local header from start of archive:   2842763
-                                                  (00000000002B608Bh) bytes
+  offset of local header from start of archive:   2842813
+                                                  (00000000002B60BDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13631,16 +13631,16 @@
   There is no file comment.
 
 Central directory entry #369:
 ---------------------------
 
   static/js/jquery.min.js
 
-  offset of local header from start of archive:   2876816
-                                                  (00000000002BE590h) bytes
+  offset of local header from start of archive:   2876866
+                                                  (00000000002BE5C2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13668,16 +13668,16 @@
   There is no file comment.
 
 Central directory entry #370:
 ---------------------------
 
   static/js/highlight.min.js
 
-  offset of local header from start of archive:   2907469
-                                                  (00000000002C5D4Dh) bytes
+  offset of local header from start of archive:   2907519
+                                                  (00000000002C5D7Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13703,32 +13703,69 @@
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
 Central directory entry #371:
 ---------------------------
 
+  static/favicon.ico
+
+  offset of local header from start of archive:   2938891
+                                                  (00000000002CD80Bh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2019 Sep 6 22:18:24
+  file last modified on (UT extra field modtime): 2019 Sep 7 05:18:24 local
+  file last modified on (UT extra field modtime): 2019 Sep 7 05:18:24 UTC
+  32-bit CRC value (hex):                         21d942a1
+  compressed size:                                4672 bytes
+  uncompressed size:                              32038 bytes
+  length of filename:                             18 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #372:
+---------------------------
+
   __init__.py
 
-  offset of local header from start of archive:   2938841
-                                                  (00000000002CD7D9h) bytes
+  offset of local header from start of archive:   2943639
+                                                  (00000000002CEA97h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 May 1 13:04:18
-  file last modified on (UT extra field modtime): 2022 May 1 20:04:17 local
-  file last modified on (UT extra field modtime): 2022 May 1 20:04:17 UTC
-  32-bit CRC value (hex):                         b46de5b2
-  compressed size:                                5390 bytes
-  uncompressed size:                              20255 bytes
+  file last modified on (DOS date/time):          2023 Apr 16 18:40:24
+  file last modified on (UT extra field modtime): 2023 Apr 17 01:40:23 local
+  file last modified on (UT extra field modtime): 2023 Apr 17 01:40:23 UTC
+  32-bit CRC value (hex):                         26add6e6
+  compressed size:                                5446 bytes
+  uncompressed size:                              20446 bytes
   length of filename:                             11 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -13737,21 +13774,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #372:
+Central directory entry #373:
 ---------------------------
 
   templates/translations.html
 
-  offset of local header from start of archive:   2944300
-                                                  (00000000002CED2Ch) bytes
+  offset of local header from start of archive:   2949154
+                                                  (00000000002D0022h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13774,32 +13811,32 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #373:
+Central directory entry #374:
 ---------------------------
 
   templates/index.html
 
-  offset of local header from start of archive:   2945394
-                                                  (00000000002CF172h) bytes
+  offset of local header from start of archive:   2950248
+                                                  (00000000002D0468h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Mar 19 18:11:28
-  file last modified on (UT extra field modtime): 2022 Mar 20 01:11:27 local
-  file last modified on (UT extra field modtime): 2022 Mar 20 01:11:27 UTC
+  file last modified on (DOS date/time):          2023 Apr 16 16:38:50
+  file last modified on (UT extra field modtime): 2023 Apr 16 23:38:49 local
+  file last modified on (UT extra field modtime): 2023 Apr 16 23:38:49 UTC
   32-bit CRC value (hex):                         69ad39ae
   compressed size:                                2913 bytes
   uncompressed size:                              13886 bytes
   length of filename:                             20 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -13811,21 +13848,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #374:
+Central directory entry #375:
 ---------------------------
 
   templates/gitlog.html
 
-  offset of local header from start of archive:   2948385
-                                                  (00000000002CFD21h) bytes
+  offset of local header from start of archive:   2953239
+                                                  (00000000002D1017h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13848,21 +13885,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #375:
+Central directory entry #376:
 ---------------------------
 
   templates/dbadmin.html
 
-  offset of local header from start of archive:   2950122
-                                                  (00000000002D03EAh) bytes
+  offset of local header from start of archive:   2954976
+                                                  (00000000002D16E0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13885,21 +13922,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #376:
+Central directory entry #377:
 ---------------------------
 
   templates/ticket.html
 
-  offset of local header from start of archive:   2950630
-                                                  (00000000002D05E6h) bytes
+  offset of local header from start of archive:   2955484
+                                                  (00000000002D18DCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13922,21 +13959,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #377:
+Central directory entry #378:
 ---------------------------
 
   diff2kryten.py
 
-  offset of local header from start of archive:   2951184
-                                                  (00000000002D0810h) bytes
+  offset of local header from start of archive:   2956038
+                                                  (00000000002D1B06h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -13959,21 +13996,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #378:
+Central directory entry #379:
 ---------------------------
 
   translations/README.md
 
-  offset of local header from start of archive:   2953069
-                                                  (00000000002D0F6Dh) bytes
+  offset of local header from start of archive:   2957923
+                                                  (00000000002D2263h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
```

#### zipnote {}

```diff
@@ -1104,14 +1104,17 @@
 
 Filename: static/js/jquery.min.js
 Comment: 
 
 Filename: static/js/highlight.min.js
 Comment: 
 
+Filename: static/favicon.ico
+Comment: 
+
 Filename: __init__.py
 Comment: 
 
 Filename: templates/translations.html
 Comment: 
 
 Filename: templates/index.html
```

#### static/components/mtable.js

##### js-beautify {}

```diff
@@ -94,38 +94,19 @@
 
     mtable.methods.open_edit = function(item) {
         this.item = {};
         this.item = item;
         this.prepare_fields(this.item);
     };
 
-    mtable.methods.l2s = function(list) {
-        return (list || []).map(function(x) {
-            return '' + x
-        }).join(', ');
-    };
-
-    mtable.methods.s2l = function(string, is_list_integer) {
-        var v = string;
-        v = v && v.split(',').map(function(x) {
-            return x.trim();
-        }) || [];
-        if (is_list_integer) v = v.map(function(x) {
-            return parseInt(x)
-        })
-        return v;
-    };
-
     mtable.methods.prepare_fields = function(item) {
         let self = this;
         for (var field of this.table.model) {
-            console.log(field.name);
             if (field.type == "list:string" || field.type == "list:integer" || field.type.substr(0, 14) == "list:reference") {
-                self.string_values[field.name] = mtable.methods.l2s(item[field.name]);
-                console.log(self.string_values[field.name]);
+                self.string_values[field.name] = JSON.stringify(item[field.name]);
             } else if (field.type == "datetime") {
                 output = field.default != null ? field.default : '';
                 output = output.split('.')[0];
                 Vue.set(this.item, field.name, output);
             } else if (field.type == "reference") {
                 if (!(field.references in this.reference_options)) {
                     Vue.set(this.reference_options, field.references, []);
@@ -137,15 +118,21 @@
                         let url_components = res.config.url.split('?')[0].split('/');
                         self.reference_options[url_components[url_components.length - 1]] = res.data.items;
                     });
 
                 }
             }
         }
-    }
+        this.$nextTick(function() {
+            Q("input[type=text].type-list-string,input[type=text].type-list-integer,input[type=text].type-list-reference").forEach(
+                function(elem) {
+                    Q.tags_input(elem);
+                });
+        });
+    };
 
     mtable.methods.parse_and_validate_json = function(event) {
         try {
             event.target.style.borderColor = "";
             return JSON.parse(event.target.value);
         } catch (error) {
             event.target.style.borderColor = "#ff0000";
@@ -165,15 +152,20 @@
 
     mtable.methods.save = function(item) {
         let url = this.url;
         self.busy = true;
         for (var field of this.table.model) {
             var is_list_integer = field.type == "list:integer" || field.type.substr(0, 14) == "list:reference";
             if (field.type == "list:string" || is_list_integer) {
-                item[field.name] = mtable.methods.s2l(this.string_values[field.name], is_list_integer);
+                try {
+                    item[field.name] = JSON.parse(this.string_values[field.name]);
+                } catch (err) {
+                    alert("Invalid field value: " + field.name);
+                    break;
+                }
             }
         }
         if (item.id) {
             url += '/' + item.id;
             axios.put(url, item).then(mtable.handle_response('put', this),
                 mtable.handle_response('put', this));
         } else {
@@ -184,15 +176,14 @@
 
     mtable.handle_response = function(method, data) {
         self.busy = false;
         return function(res) {
             if (res.response) res = res.response; // deal with error weirdness
             if (method == 'post') {
                 data.table.items = [];
-                console.log(data);
                 mtable.methods.load.call(data);
             }
             if (res.data.status == 'success') {
                 data.clear();
             } else {
                 data.errors = res.data.errors;
                 data.message = res.data.message;
@@ -226,16 +217,14 @@
         vars['filter'] = fieldname + '==' + item_id;
         source = Object.keys(vars).map(function(key) {
             return key + '=' + encodeURIComponent(vars[key]);
         }).join('&');
         window.location = window.location.href.split('?')[0] + '?' + source;
     };
 
-
-
     var scripts = document.getElementsByTagName('script');
     var src = scripts[scripts.length - 1].src;
     var path = src.substr(0, src.length - 3) + '.html';
     Q.register_vue_component('mtable', path, function(template) {
         mtable.template = template.data;
         return mtable;
     });
```

#### static/components/mtable.html

```diff
@@ -1,12 +1,12 @@
 <div>
   <table>
     <tr>
       <td class="control">              
-        <input class="input" v-model="filter" type="text" placeholder="filter (example id > 1)" style="width: 100%" v-on:keyup.enter="search()"/>
+        <input v-model="filter" type="text" placeholder="filter (example id > 1)" style="width: 100%" v-on:keyup.enter="search()"/>
       </td>
       <td style="white-space: nowrap; width:10%; padding-left:5px">
         <button v-on:click="search()" class="button">Search</button>
         <button v-if="create" v-on:click="open_create()" class="button">Create</button>
       </td>
     </tr>    
     <tr>
@@ -20,32 +20,32 @@
     <i class="fa fa-3x fa-spin fa-spinner"></i>
   </div>
   <div v-else-if="item!=null">
     <table class="table">
       <tr v-for="field in table.model" v-if="field.type!='id' || item.id">
         <th>{{field.label}}</th>
         <td class="control">
-          <input class="input" v-if="field.type=='id'" type="text" readonly v-model="item[field.name]">
-          <input class="input" v-else-if="field.type=='string'" type="text" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-if="field.type=='id'" type="text" readonly v-model="item[field.name]">
+          <input v-else-if="field.type=='string'" type="text" v-model="item[field.name]" v-bind:readonly="!editable">
           <span v-else-if="field.type=='boolean'" v-on:click="toggle(item, field.name)" v-bind:readonly="!editable">
             <span v-if="item[field.name]===true"><i class="fa fa-check-square"></i> True</span>
             <span v-else-if="item[field.name]===false"><i class="fa fa-square"></i> False</span>
             <span v-else><i class="fa fa-square"></i> None</span>
           </span>
-          <input class="input" v-else-if="field.type=='integer'" type="number" step="1" v-model="item[field.name]" v-bind:readonly="!editable">
-          <input class="input" v-else-if="field.type=='float'" type="number" step="0.00000000000001" v-model="item[field.name]"  v-bind:readonly="!editable">
-          <input class="input" v-else-if="field.type=='double'" type="number" step="0.00000000000001" v-model="item[field.name]" v-bind:readonly="!editable">
-          <input class="input" v-else-if="field.type=='decimal'" type="number" step="0.1" v-model="item[field.name]" v-bind:readonly="!editable">
-          <input class="input" v-else-if="field.type=='date'" type="date" v-model="item[field.name]" v-bind:readonly="!editable">
-          <input class="input" v-else-if="field.type=='time'" type="time" v-model="item[field.name]" v-bind:readonly="!editable">
-          <input class="input" v-else-if="field.type=='datetime'" type="datetime-local" v-model="item[field.name]" v-bind:readonly="!editable">
-          <input class="input" v-else-if="field.type=='password'" type="password" v-model="item[field.name]" v-bind:readonly="!editable">
-          <input class="input type-list-integer" v-else-if="field.type=='list:integer'" type="text" v-model="string_values[field.name]" v-bind:readonly="!editable">
-          <input class="input type-list-reference" v-else-if="field.type.substr(0,14)=='list:reference'" type="text" v-model="string_values[field.name]" v-bind:readonly="!editable">
-          <input class="input type-list-string" v-else-if="field.type=='list:string'" type="text" v-model="string_values[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='integer'" type="number" step="1" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='float'" type="number" step="0.00000000000001" v-model="item[field.name]"  v-bind:readonly="!editable">
+          <input v-else-if="field.type=='double'" type="number" step="0.00000000000001" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='decimal'" type="number" step="0.1" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='date'" type="date" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='time'" type="time" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='datetime'" type="datetime-local" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='password'" type="password" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input class="type-list-integer" v-else-if="field.type=='list:integer'" type="text" v-model="string_values[field.name]" v-bind:readonly="!editable">
+          <input class="type-list-reference" v-else-if="field.type.substr(0,14)=='list:reference'" type="text" v-model="string_values[field.name]" v-bind:readonly="!editable">
+          <input class="type-list-string" v-else-if="field.type=='list:string'" type="text" v-model="string_values[field.name]" v-bind:readonly="!editable">
           <input v-else-if="field.type=='upload'" type="text" v-model="item[field.name]" v-bind:readonly="!editable">
           <textarea class="textarea" v-else-if="field.type=='text'" v-model="item[field.name]" v-bind:readonly="!editable"></textarea>
           <select v-else-if="field.type=='reference'" v-model="item[field.name]" v-bind:readonly="!editable">
             <option disabled value="">Select...</option>
             <option v-for="option in reference_options[field.references]" :key="option.value" v-bind:value="option.value">
               {{ option.text }}
             </option>
@@ -92,16 +92,16 @@
             <span v-else-if="field.type=='json'" class="field-string">(json)</span>
             <span v-else-if="field.type=='integer'" class="field-integer">{{item[field.name]}}</span>
             <span v-else-if="field.type=='double'" class="field-float">{{item[field.name]}}</span>
             <span v-else-if="field.type=='float'" class="field-float">{{item[field.name]}}</span>
             <span v-else-if="field.type=='decimal'" class="field-float">{{item[field.name]}}</span>
             <span v-else-if="field.type=='date'" class="field-date">{{item[field.name]}}</span>
             <span v-else-if="field.type=='time'" class="field-time">{{item[field.name]}}</span>
-            <span v-else-if="field.type=='list:integer'" class="field-string">{{l2s(item[field.name])}}</span>
-            <span v-else-if="field.type=='list:string'" class="field-string">{{l2s(item[field.name])}}</span>
+            <span v-else-if="field.type=='list:integer'" class="field-string">{{JSON.stringify(item[field.name])}}</span>
+            <span v-else-if="field.type=='list:string'" class="field-string">{{JSON.stringify(item[field.name])}}</span>
             <span v-else-if="field.type=='datetime'" class="field-datetime">{{(item[field.name]||'').replace('T','@').substr(0,16)}}</span>
             <span v-else-if="field.type=='password'" class="field-password">{{item[field.name]}}</span>
             <span v-else-if="field.type=='boolean'" class="field-boolean">
               <i class="fa fa-check-square" v-if="item[field.name]===true"></i>
               <i class="fa fa-square" v-if="item[field.name]===false"></i>
             </span>
             <span v-else-if="field.type=='text'" class="field-text"><i class="fa fa-expand"></i></span>
```

##### html2text {}

```diff
@@ -9,11 +9,11 @@
                 {item[field.name]}}
                 {{errors[field.name]}}
 Referenced By   {{name}}
 Save Delete Close
 {{field.label}}
 [{{item[field.name]}}] {{item[field.name]}} (json) {{item[field.name]}} {{item
 [field.name]}} {{item[field.name]}} {{item[field.name]}} {{item[field.name]}} {
-{item[field.name]}} {{l2s(item[field.name])}} {{l2s(item[field.name])}} {{(item
-[field.name]||'').replace('T','@').substr(0,16)}} {{item[field.name]}}      [{
-{item[field.name]}}]
+{item[field.name]}} {{JSON.stringify(item[field.name])}} {{JSON.stringify(item
+[field.name])}} {{(item[field.name]||'').replace('T','@').substr(0,16)}} {{item
+[field.name]}}      [{{item[field.name]}}]
 Load More
```

#### static/css/future.css

```diff
@@ -281,7 +281,10 @@
 .files li, .dirs li {
   margin: 5px;
   font-size: 1.1em;
 }
 .field-referenced {
   margin-right: 1em;
 }
+
+.tags-list li { display: inline-block; color: black; background: #d1d1d1; padding: 2px 5px; margin: 5px; border-radius: 5px; }
+.tags-list li[data-selected=false] { opacity: 0.5;  }
```

#### static/js/utils.js

##### js-beautify {}

```diff
@@ -197,45 +197,51 @@
     var keys = Q.eval(elem.value || '[]');
     keys.map(function(x) {
         if (tags.indexOf(x) < 0) tags.push(x);
     });
     var fill = function(elem, repl) {
         repl.innerHTML = '';
         tags.forEach(function(x) {
-            console.log(x);
             var item = document.createElement('li');
             item.innerHTML = options.labels[x] || x;
             item.dataset.value = x;
             item.dataset.selected = keys.indexOf(x) >= 0;
             repl.appendChild(item);
             item.onclick = function(evt) {
                 if (item.dataset.selected == 'false') keys.push(x);
                 else keys = keys.filter(function(y) {
                     return x != y;
                 });
                 item.dataset.selected = keys.indexOf(x) >= 0;
                 elem.value = JSON.stringify(keys);
+                elem.dispatchEvent(new Event('input', {
+                    bubbles: true
+                }));
             };
         });
     };
     if (options.freetext) {
         var inp = document.createElement('input');
         elem.parentNode.insertBefore(inp, elem);
+        inp.type = "text";
         inp.classList = elem.classList;
         inp.placeholder = options.placeholder;
         inp.setAttribute('list', options.autocomplete_list);
         inp.onchange = function(evt) {
             inp.value.split(',').map(function(x) {
                 x = options.transform(x.trim());
                 if (options.regex && !x.match(options.regex)) return;
                 if (x && tags.indexOf(x) < 0) tags.push(x);
                 if (x && keys.indexOf(x) < 0) keys.push(x);
             });
             inp.value = '';
             elem.value = JSON.stringify(keys);
+            elem.dispatchEvent(new Event('input', {
+                bubbles: true
+            }));
             fill(elem, repl);
         };
     }
     fill(elem, repl);
 };
 
 // Password strenght calculator
@@ -292,15 +298,14 @@
     method = (method || 'GET').toLowerCase();
     /* if target is not there, fill it with something that there isn't in the page*/
     if (target === void 0 || target === '') target = 'none';
     var onsuccess = function(res) {
         if (res.redirected) window.location = res.url;
         Q('#' + target)[0].innerHTML = res.data;
         Q.trap_form(url, target);
-        console.log(res.headers);
         var flash = res.headers.get('component-flash');
         if (flash) Q.flash(JSON.parse(flash));
     };
     var onerror = function(res) {
         alert('ajax error');
     };
     Q.ajax(method, url, form_data).then(onsuccess).catch(onerror);
@@ -334,15 +339,14 @@
     if (elem) {
         elem.addEventListener('flash', make_handler(elem), false);
         Q.flash = function(detail) {
             elem.dispatchEvent(new CustomEvent('flash', {
                 detail: detail
             }));
         };
-        console.log(elem.dataset.alert);
         if (elem.dataset.alert) Q.flash(Q.eval(elem.dataset.alert));
     }
 };
 
 Q.handle_components();
 Q.handle_flash();
 Q('input[type=text].type-list-string').forEach(function(elem) {
```

#### __init__.py

```diff
@@ -29,14 +29,15 @@
 from pydal.restapi import RestAPI, Policy
 
 from .diff2kryten import diff2kryten
 from .utils import *
 
 MODE = os.environ.get("PY4WEB_DASHBOARD_MODE", "none")
 FOLDER = os.environ["PY4WEB_APPS_FOLDER"]
+APP_NAMES = os.environ.get("PY4WEB_APP_NAMES")
 APP_FOLDER = os.path.dirname(__file__)
 T_FOLDER = os.path.join(APP_FOLDER, "translations")
 T = Translator(T_FOLDER)
 
 session = Session()
 
 
@@ -183,20 +184,23 @@
         return {"payload": sorted_routes, "status": "success"}
 
     @action("apps")
     @session_secured
     def apps():
         """Returns a list of installed apps"""
         apps = os.listdir(FOLDER)
+        print(APP_NAMES)
+        exposed_names = APP_NAMES and APP_NAMES.split(",")
         apps = [
             {"name": app, "error": Reloader.ERRORS.get(app)}
             for app in apps
             if os.path.isdir(os.path.join(FOLDER, app))
             and not app.startswith("__")
             and not app.startswith(".")
+            and (not exposed_names or app in exposed_names)
         ]
         apps.sort(key=lambda item: item["name"])
         return {"payload": apps, "status": "success"}
 
     @action("delete_app/<name:re:\w+>", method="POST")
     @session_secured
     def delete_app(name):
```

### Comparing `py4web-1.20230416.2/py4web/assets/py4web.app._default.zip` & `py4web-1.20230416.3/py4web/assets/py4web.app._default.zip`

 * *Files 7% similar despite different names*

#### zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    182307 (000000000002C823h)
-  Actual end-cent-dir record offset:        182285 (000000000002C80Dh)
-  Expected end-cent-dir record offset:      182285 (000000000002C80Dh)
+  Zip archive file size:                    187155 (000000000002DB13h)
+  Actual end-cent-dir record offset:        187133 (000000000002DAFDh)
+  Expected end-cent-dir record offset:      187133 (000000000002DAFDh)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 3 entries.
-  The central directory is 263 (0000000000000107h) bytes long,
+  central directory contains 4 entries.
+  The central directory is 351 (000000000000015Fh) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 182022 (000000000002C706h).
+  is 186782 (000000000002D99Eh).
 
 
 Central directory entry #1:
 ---------------------------
 
   static/images/logo.png
 
@@ -51,26 +51,63 @@
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  __init__.py
+  static/favicon.ico
 
   offset of local header from start of archive:   180885
                                                   (000000000002C295h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
+  file last modified on (DOS date/time):          2019 Dec 27 02:53:24
+  file last modified on (UT extra field modtime): 2019 Dec 27 10:53:23 local
+  file last modified on (UT extra field modtime): 2019 Dec 27 10:53:23 UTC
+  32-bit CRC value (hex):                         21d942a1
+  compressed size:                                4672 bytes
+  uncompressed size:                              32038 bytes
+  length of filename:                             18 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #3:
+---------------------------
+
+  __init__.py
+
+  offset of local header from start of archive:   185633
+                                                  (000000000002D521h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
   file last modified on (DOS date/time):          2019 Dec 25 10:43:12
   file last modified on (UT extra field modtime): 2019 Dec 25 18:43:11 local
   file last modified on (UT extra field modtime): 2019 Dec 25 18:43:11 UTC
   32-bit CRC value (hex):                         de02d24c
   compressed size:                                101 bytes
   uncompressed size:                              135 bytes
   length of filename:                             11 characters
@@ -85,35 +122,35 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #3:
+Central directory entry #4:
 ---------------------------
 
   templates/index.html
 
-  offset of local header from start of archive:   181055
-                                                  (000000000002C33Fh) bytes
+  offset of local header from start of archive:   185803
+                                                  (000000000002D5CBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Jun 5 18:49:36
-  file last modified on (UT extra field modtime): 2022 Jun 6 01:49:36 local
-  file last modified on (UT extra field modtime): 2022 Jun 6 01:49:36 UTC
-  32-bit CRC value (hex):                         a86f01bf
-  compressed size:                                889 bytes
-  uncompressed size:                              1799 bytes
+  file last modified on (DOS date/time):          2023 Apr 16 11:17:40
+  file last modified on (UT extra field modtime): 2023 Apr 16 18:17:40 local
+  file last modified on (UT extra field modtime): 2023 Apr 16 18:17:40 UTC
+  32-bit CRC value (hex):                         242a0dc9
+  compressed size:                                901 bytes
+  uncompressed size:                              1811 bytes
   length of filename:                             20 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
```

#### zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: static/images/logo.png
 Comment: 
 
+Filename: static/favicon.ico
+Comment: 
+
 Filename: __init__.py
 Comment: 
 
 Filename: templates/index.html
 Comment: 
 
 Zip file comment:
```

#### templates/index.html

```diff
@@ -20,15 +20,15 @@
       main h1 {margin-bottom: 2vh; margin-top: 5vh; font-size: 3em }
       main h2 {margin-bottom: 10vh; }
     </style>
   </head>
   <body>
     <a href="https://github.com/web2py/py4web" style="position:fixed;z-index:10x00;top:0;right:0;"><img width="149" height="149" src="https://github.blog/wp-content/uploads/2008/12/forkme_right_red_aa0000.png?resize=149%2C149" class="attachment-full size-full" alt="Fork me on GitHub" data-recalc-dims="1"></a>
     <main>
-      <img class="logo" src="static/images/logo.png"/>
+      <img class="logo" src="[[=URL("static/images/logo.png")]]"/>
       <h1>PY4WEB</h1>
       <h2>Different, yet cute, and a memorable evolutionary step.</h2>
       <a href="/_dashboard">Dashboard</a>
       <a href="/_documentation?version=[[=version]]">Documentation</a>
       <a href="/showcase">Examples</a>
       <a href="https://learn-py4web.github.io/">Tutorials</a>
       <a href="https://github.com/web2py/py4web">Source</a>
```

##### html2text {}

```diff
@@ -1,5 +1,6 @@
 
-[Fork_me_on_GitHub]  [static/images/logo.png]
+[Fork_me_on_GitHub]
+mages/logo.png")]]"/>
 ****** PY4WEB ******
 ***** Different, yet cute, and a memorable evolutionary step. *****
 Dashboard Documentation Examples Tutorials Source Discuss
```

### Comparing `py4web-1.20230416.2/py4web/assets/py4web.app._documentation.zip` & `py4web-1.20230416.3/py4web/assets/py4web.app._documentation.zip`

 * *Files 3% similar despite different names*

#### zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                   4278028 (000000000041470Ch)
-  Actual end-cent-dir record offset:       4278006 (00000000004146F6h)
-  Expected end-cent-dir record offset:     4278006 (00000000004146F6h)
+  Zip archive file size:                   4287226 (0000000000416AFAh)
+  Actual end-cent-dir record offset:       4287204 (0000000000416AE4h)
+  Expected end-cent-dir record offset:     4287204 (0000000000416AE4h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 149 entries.
-  The central directory is 14763 (00000000000039ABh) bytes long,
+  central directory contains 152 entries.
+  The central directory is 15055 (0000000000003ACFh) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 4263243 (0000000000410D4Bh).
+  is 4272149 (0000000000413015h).
 
 
 Central directory entry #1:
 ---------------------------
 
   static/en/chapter-10.html
 
@@ -828,21 +828,57 @@
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
 Central directory entry #23:
 ---------------------------
 
-  static/en/_static/js/html5shiv-printshiv.min.js
+  static/en/_static/logo-32x32.ico
 
   offset of local header from start of archive:   309858
                                                   (000000000004BA62h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2021 May 15 22:29:46
+  file last modified on (UT extra field modtime): 2021 May 16 05:29:45 local
+  file last modified on (UT extra field modtime): 2021 May 16 05:29:45 UTC
+  32-bit CRC value (hex):                         174acf66
+  compressed size:                                1989 bytes
+  uncompressed size:                              1989 bytes
+  length of filename:                             32 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (100664 octal):            -rw-rw-r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #24:
+---------------------------
+
+  static/en/_static/js/html5shiv-printshiv.min.js
+
+  offset of local header from start of archive:   311937
+                                                  (000000000004C281h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          2023 Jan 2 20:34:26
   file last modified on (UT extra field modtime): 2023 Jan 3 04:34:26 local
@@ -862,21 +898,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #24:
+Central directory entry #25:
 ---------------------------
 
   static/en/_static/js/badge_only.js
 
-  offset of local header from start of archive:   311982
-                                                  (000000000004C2AEh) bytes
+  offset of local header from start of archive:   314061
+                                                  (000000000004CACDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -899,21 +935,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #25:
+Central directory entry #26:
 ---------------------------
 
   static/en/_static/js/toggle.js
 
-  offset of local header from start of archive:   312510
-                                                  (000000000004C4BEh) bytes
+  offset of local header from start of archive:   314589
+                                                  (000000000004CCDDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -936,21 +972,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #26:
+Central directory entry #27:
 ---------------------------
 
   static/en/_static/js/theme.js
 
-  offset of local header from start of archive:   313132
-                                                  (000000000004C72Ch) bytes
+  offset of local header from start of archive:   315211
+                                                  (000000000004CF4Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -973,21 +1009,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #27:
+Central directory entry #28:
 ---------------------------
 
   static/en/_static/js/html5shiv.min.js
 
-  offset of local header from start of archive:   314996
-                                                  (000000000004CE74h) bytes
+  offset of local header from start of archive:   317075
+                                                  (000000000004D693h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1010,21 +1046,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #28:
+Central directory entry #29:
 ---------------------------
 
   static/en/_static/file.png
 
-  offset of local header from start of archive:   316424
-                                                  (000000000004D408h) bytes
+  offset of local header from start of archive:   318503
+                                                  (000000000004DC27h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -1046,21 +1082,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #29:
+Central directory entry #30:
 ---------------------------
 
   static/en/_static/doctools.js
 
-  offset of local header from start of archive:   316794
-                                                  (000000000004D57Ah) bytes
+  offset of local header from start of archive:   318873
+                                                  (000000000004DD99h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1083,21 +1119,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #30:
+Central directory entry #31:
 ---------------------------
 
   static/en/_static/basic.css
 
-  offset of local header from start of archive:   318514
-                                                  (000000000004DC32h) bytes
+  offset of local header from start of archive:   320593
+                                                  (000000000004E451h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1120,21 +1156,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #31:
+Central directory entry #32:
 ---------------------------
 
   static/en/chapter-15.html
 
-  offset of local header from start of archive:   322070
-                                                  (000000000004EA16h) bytes
+  offset of local header from start of archive:   324149
+                                                  (000000000004F235h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1157,21 +1193,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #32:
+Central directory entry #33:
 ---------------------------
 
   static/en/chapter-12.html
 
-  offset of local header from start of archive:   330215
-                                                  (00000000000509E7h) bytes
+  offset of local header from start of archive:   332294
+                                                  (0000000000051206h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1194,21 +1230,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #33:
+Central directory entry #34:
 ---------------------------
 
   static/en/searchindex.js
 
-  offset of local header from start of archive:   356429
-                                                  (000000000005704Dh) bytes
+  offset of local header from start of archive:   358508
+                                                  (000000000005786Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1231,21 +1267,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #34:
+Central directory entry #35:
 ---------------------------
 
   static/en/chapter-02.html
 
-  offset of local header from start of archive:   383387
-                                                  (000000000005D99Bh) bytes
+  offset of local header from start of archive:   385466
+                                                  (000000000005E1BAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1268,21 +1304,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #35:
+Central directory entry #36:
 ---------------------------
 
   static/en/chapter-11.html
 
-  offset of local header from start of archive:   389069
-                                                  (000000000005EFCDh) bytes
+  offset of local header from start of archive:   391148
+                                                  (000000000005F7ECh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1305,21 +1341,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #36:
+Central directory entry #37:
 ---------------------------
 
   static/en/chapter-01.html
 
-  offset of local header from start of archive:   392435
-                                                  (000000000005FCF3h) bytes
+  offset of local header from start of archive:   394514
+                                                  (0000000000060512h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1342,21 +1378,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #37:
+Central directory entry #38:
 ---------------------------
 
   static/en/genindex.html
 
-  offset of local header from start of archive:   397649
-                                                  (0000000000061151h) bytes
+  offset of local header from start of archive:   399728
+                                                  (0000000000061970h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1379,21 +1415,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #38:
+Central directory entry #39:
 ---------------------------
 
   static/en/toggle.css
 
-  offset of local header from start of archive:   399634
-                                                  (0000000000061912h) bytes
+  offset of local header from start of archive:   401713
+                                                  (0000000000062131h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1416,21 +1452,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #39:
+Central directory entry #40:
 ---------------------------
 
   static/en/chapter-08.html
 
-  offset of local header from start of archive:   400235
-                                                  (0000000000061B6Bh) bytes
+  offset of local header from start of archive:   402314
+                                                  (000000000006238Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1453,21 +1489,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #40:
+Central directory entry #41:
 ---------------------------
 
   static/en/_images/form1.png
 
-  offset of local header from start of archive:   408858
-                                                  (0000000000063D1Ah) bytes
+  offset of local header from start of archive:   410937
+                                                  (0000000000064539h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1490,21 +1526,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #41:
+Central directory entry #42:
 ---------------------------
 
   static/en/_images/dashboard_ticket.png
 
-  offset of local header from start of archive:   419449
-                                                  (0000000000066679h) bytes
+  offset of local header from start of archive:   421528
+                                                  (0000000000066E98h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1527,21 +1563,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #42:
+Central directory entry #43:
 ---------------------------
 
   static/en/_images/form3.png
 
-  offset of local header from start of archive:   556755
-                                                  (0000000000087ED3h) bytes
+  offset of local header from start of archive:   558834
+                                                  (00000000000886F2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1564,21 +1600,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #43:
+Central directory entry #44:
 ---------------------------
 
   static/en/_images/dashboard_edit.png
 
-  offset of local header from start of archive:   592587
-                                                  (0000000000090ACBh) bytes
+  offset of local header from start of archive:   594666
+                                                  (00000000000912EAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1601,21 +1637,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #44:
+Central directory entry #45:
 ---------------------------
 
   static/en/_images/form2.png
 
-  offset of local header from start of archive:   761930
-                                                  (00000000000BA04Ah) bytes
+  offset of local header from start of archive:   764009
+                                                  (00000000000BA869h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1638,21 +1674,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #45:
+Central directory entry #46:
 ---------------------------
 
   static/en/_images/grid.png
 
-  offset of local header from start of archive:   800213
-                                                  (00000000000C35D5h) bytes
+  offset of local header from start of archive:   802292
+                                                  (00000000000C3DF4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1675,21 +1711,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #46:
+Central directory entry #47:
 ---------------------------
 
   static/en/_images/restapi2.png
 
-  offset of local header from start of archive:   839962
-                                                  (00000000000CD11Ah) bytes
+  offset of local header from start of archive:   842041
+                                                  (00000000000CD939h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1712,21 +1748,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #47:
+Central directory entry #48:
 ---------------------------
 
   static/en/_images/simple_counter.png
 
-  offset of local header from start of archive:   867185
-                                                  (00000000000D3B71h) bytes
+  offset of local header from start of archive:   869264
+                                                  (00000000000D4390h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1749,21 +1785,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #48:
+Central directory entry #49:
 ---------------------------
 
   static/en/_images/restapi.png
 
-  offset of local header from start of archive:   881463
-                                                  (00000000000D7337h) bytes
+  offset of local header from start of archive:   883542
+                                                  (00000000000D7B56h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1786,21 +1822,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #49:
+Central directory entry #50:
 ---------------------------
 
   static/en/_images/form5.png
 
-  offset of local header from start of archive:   910699
-                                                  (00000000000DE56Bh) bytes
+  offset of local header from start of archive:   912778
+                                                  (00000000000DED8Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1823,21 +1859,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #50:
+Central directory entry #51:
 ---------------------------
 
   static/en/_images/dashboard_login.png
 
-  offset of local header from start of archive:   948758
-                                                  (00000000000E7A16h) bytes
+  offset of local header from start of archive:   950837
+                                                  (00000000000E8235h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1860,21 +1896,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #51:
+Central directory entry #52:
 ---------------------------
 
   static/en/_images/dashboard_restapi.png
 
-  offset of local header from start of archive:   1029789
-                                                  (00000000000FB69Dh) bytes
+  offset of local header from start of archive:   1031868
+                                                  (00000000000FBEBCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1897,21 +1933,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #52:
+Central directory entry #53:
 ---------------------------
 
   static/en/_images/dashboard_main.png
 
-  offset of local header from start of archive:   1172082
-                                                  (000000000011E272h) bytes
+  offset of local header from start of archive:   1174161
+                                                  (000000000011EA91h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1934,21 +1970,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #53:
+Central directory entry #54:
 ---------------------------
 
   static/en/_images/grid_columns.png
 
-  offset of local header from start of archive:   1301877
-                                                  (000000000013DD75h) bytes
+  offset of local header from start of archive:   1303956
+                                                  (000000000013E594h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1971,21 +2007,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #54:
+Central directory entry #55:
 ---------------------------
 
   static/en/_images/grid_bulmacss.png
 
-  offset of local header from start of archive:   1358378
-                                                  (000000000014BA2Ah) bytes
+  offset of local header from start of archive:   1360457
+                                                  (000000000014C249h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2008,21 +2044,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #55:
+Central directory entry #56:
 ---------------------------
 
   static/en/_images/_scaffold.png
 
-  offset of local header from start of archive:   1397167
-                                                  (00000000001551AFh) bytes
+  offset of local header from start of archive:   1399246
+                                                  (00000000001559CEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2045,21 +2081,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #56:
+Central directory entry #57:
 ---------------------------
 
   static/en/_images/logo.png
 
-  offset of local header from start of archive:   1407929
-                                                  (0000000000157BB9h) bytes
+  offset of local header from start of archive:   1410008
+                                                  (00000000001583D8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2082,21 +2118,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #57:
+Central directory entry #58:
 ---------------------------
 
   static/en/_images/dashboard.png
 
-  offset of local header from start of archive:   1588818
-                                                  (0000000000183E52h) bytes
+  offset of local header from start of archive:   1590897
+                                                  (0000000000184671h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2119,21 +2155,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #58:
+Central directory entry #59:
 ---------------------------
 
   static/en/_images/tags2.png
 
-  offset of local header from start of archive:   1632526
-                                                  (000000000018E90Eh) bytes
+  offset of local header from start of archive:   1634605
+                                                  (000000000018F12Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2156,21 +2192,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #59:
+Central directory entry #60:
 ---------------------------
 
   static/en/_images/form4.png
 
-  offset of local header from start of archive:   1662165
-                                                  (0000000000195CD5h) bytes
+  offset of local header from start of archive:   1664244
+                                                  (00000000001964F4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2193,21 +2229,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #60:
+Central directory entry #61:
 ---------------------------
 
   static/en/_images/dashboard_error.png
 
-  offset of local header from start of archive:   1705983
-                                                  (00000000001A07FFh) bytes
+  offset of local header from start of archive:   1708062
+                                                  (00000000001A101Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2230,21 +2266,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #61:
+Central directory entry #62:
 ---------------------------
 
   static/en/_images/grid_nocss.png
 
-  offset of local header from start of archive:   1754002
-                                                  (00000000001AC392h) bytes
+  offset of local header from start of archive:   1756081
+                                                  (00000000001ACBB1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2267,21 +2303,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #62:
+Central directory entry #63:
 ---------------------------
 
   static/en/_images/tags_db.png
 
-  offset of local header from start of archive:   1797081
-                                                  (00000000001B6BD9h) bytes
+  offset of local header from start of archive:   1799160
+                                                  (00000000001B73F8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2304,21 +2340,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #63:
+Central directory entry #64:
 ---------------------------
 
   static/en/_images/dashboard_new_app.png
 
-  offset of local header from start of archive:   1820701
-                                                  (00000000001BC81Dh) bytes
+  offset of local header from start of archive:   1822780
+                                                  (00000000001BD03Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2341,21 +2377,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #64:
+Central directory entry #65:
 ---------------------------
 
   static/en/_images/main_page.png
 
-  offset of local header from start of archive:   1858248
-                                                  (00000000001C5AC8h) bytes
+  offset of local header from start of archive:   1860327
+                                                  (00000000001C62E7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2378,21 +2414,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #65:
+Central directory entry #66:
 ---------------------------
 
   static/en/_images/command.png
 
-  offset of local header from start of archive:   1917348
-                                                  (00000000001D41A4h) bytes
+  offset of local header from start of archive:   1919427
+                                                  (00000000001D49C3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2415,21 +2451,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #66:
+Central directory entry #67:
 ---------------------------
 
   static/en/_images/first_run.png
 
-  offset of local header from start of archive:   1951445
-                                                  (00000000001DC6D5h) bytes
+  offset of local header from start of archive:   1953524
+                                                  (00000000001DCEF4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2452,21 +2488,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #67:
+Central directory entry #68:
 ---------------------------
 
   static/en/_images/form6.png
 
-  offset of local header from start of archive:   1996841
-                                                  (00000000001E7829h) bytes
+  offset of local header from start of archive:   1998920
+                                                  (00000000001E8048h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2489,21 +2525,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #68:
+Central directory entry #69:
 ---------------------------
 
   static/en/dark.css
 
-  offset of local header from start of archive:   2033249
-                                                  (00000000001F0661h) bytes
+  offset of local header from start of archive:   2035328
+                                                  (00000000001F0E80h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2526,21 +2562,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #69:
+Central directory entry #70:
 ---------------------------
 
   static/en/chapter-07.html
 
-  offset of local header from start of archive:   2034766
-                                                  (00000000001F0C4Eh) bytes
+  offset of local header from start of archive:   2036845
+                                                  (00000000001F146Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2563,21 +2599,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #70:
+Central directory entry #71:
 ---------------------------
 
   static/en/chapter-04.html
 
-  offset of local header from start of archive:   2101446
-                                                  (00000000002010C6h) bytes
+  offset of local header from start of archive:   2103525
+                                                  (00000000002018E5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2600,21 +2636,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #71:
+Central directory entry #72:
 ---------------------------
 
   static/en/search.html
 
-  offset of local header from start of archive:   2105121
-                                                  (0000000000201F21h) bytes
+  offset of local header from start of archive:   2107200
+                                                  (0000000000202740h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2637,21 +2673,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #72:
+Central directory entry #73:
 ---------------------------
 
   static/en/chapter-13.html
 
-  offset of local header from start of archive:   2107184
-                                                  (0000000000202730h) bytes
+  offset of local header from start of archive:   2109263
+                                                  (0000000000202F4Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2674,21 +2710,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #73:
+Central directory entry #74:
 ---------------------------
 
   static/index.html
 
-  offset of local header from start of archive:   2117130
-                                                  (0000000000204E0Ah) bytes
+  offset of local header from start of archive:   2119209
+                                                  (0000000000205629h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2711,21 +2747,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #74:
+Central directory entry #75:
 ---------------------------
 
   static/pt/chapter-10.html
 
-  offset of local header from start of archive:   2117379
-                                                  (0000000000204F03h) bytes
+  offset of local header from start of archive:   2119458
+                                                  (0000000000205722h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2748,21 +2784,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #75:
+Central directory entry #76:
 ---------------------------
 
   static/pt/chapter-14.html
 
-  offset of local header from start of archive:   2131390
-                                                  (00000000002085BEh) bytes
+  offset of local header from start of archive:   2133469
+                                                  (0000000000208DDDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2785,21 +2821,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #76:
+Central directory entry #77:
 ---------------------------
 
   static/pt/chapter-03.html
 
-  offset of local header from start of archive:   2142338
-                                                  (000000000020B082h) bytes
+  offset of local header from start of archive:   2144417
+                                                  (000000000020B8A1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2822,21 +2858,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #77:
+Central directory entry #78:
 ---------------------------
 
   static/pt/chapter-05.html
 
-  offset of local header from start of archive:   2154203
-                                                  (000000000020DEDBh) bytes
+  offset of local header from start of archive:   2156282
+                                                  (000000000020E6FAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2859,21 +2895,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #78:
+Central directory entry #79:
 ---------------------------
 
   static/pt/chapter-16.html
 
-  offset of local header from start of archive:   2164709
-                                                  (00000000002107E5h) bytes
+  offset of local header from start of archive:   2166788
+                                                  (0000000000211004h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2896,21 +2932,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #79:
+Central directory entry #80:
 ---------------------------
 
   static/pt/chapter-06.html
 
-  offset of local header from start of archive:   2177716
-                                                  (0000000000213AB4h) bytes
+  offset of local header from start of archive:   2179795
+                                                  (00000000002142D3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2933,21 +2969,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #80:
+Central directory entry #81:
 ---------------------------
 
   static/pt/index.html
 
-  offset of local header from start of archive:   2195216
-                                                  (0000000000217F10h) bytes
+  offset of local header from start of archive:   2197295
+                                                  (000000000021872Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2970,21 +3006,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #81:
+Central directory entry #82:
 ---------------------------
 
   static/pt/chapter-09.html
 
-  offset of local header from start of archive:   2199372
-                                                  (0000000000218F4Ch) bytes
+  offset of local header from start of archive:   2201451
+                                                  (000000000021976Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3007,21 +3043,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #82:
+Central directory entry #83:
 ---------------------------
 
   static/pt/_static/tabs.css
 
-  offset of local header from start of archive:   2211636
-                                                  (000000000021BF34h) bytes
+  offset of local header from start of archive:   2213715
+                                                  (000000000021C753h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3044,21 +3080,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #83:
+Central directory entry #84:
 ---------------------------
 
   static/pt/_static/documentation_options.js
 
-  offset of local header from start of archive:   2212280
-                                                  (000000000021C1B8h) bytes
+  offset of local header from start of archive:   2214359
+                                                  (000000000021C9D7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3081,21 +3117,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #84:
+Central directory entry #85:
 ---------------------------
 
   static/pt/_static/tabs.js
 
-  offset of local header from start of archive:   2212651
-                                                  (000000000021C32Bh) bytes
+  offset of local header from start of archive:   2214730
+                                                  (000000000021CB4Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3118,21 +3154,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #85:
+Central directory entry #86:
 ---------------------------
 
   static/pt/_static/sphinx_highlight.js
 
-  offset of local header from start of archive:   2214175
-                                                  (000000000021C91Fh) bytes
+  offset of local header from start of archive:   2216254
+                                                  (000000000021D13Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3155,21 +3191,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #86:
+Central directory entry #87:
 ---------------------------
 
   static/pt/_static/minus.png
 
-  offset of local header from start of archive:   2216066
-                                                  (000000000021D082h) bytes
+  offset of local header from start of archive:   2218145
+                                                  (000000000021D8A1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3192,21 +3228,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #87:
+Central directory entry #88:
 ---------------------------
 
   static/pt/_static/translations.js
 
-  offset of local header from start of archive:   2216234
-                                                  (000000000021D12Ah) bytes
+  offset of local header from start of archive:   2218313
+                                                  (000000000021D949h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3229,21 +3265,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #88:
+Central directory entry #89:
 ---------------------------
 
   static/pt/_static/plus.png
 
-  offset of local header from start of archive:   2217221
-                                                  (000000000021D505h) bytes
+  offset of local header from start of archive:   2219300
+                                                  (000000000021DD24h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3266,21 +3302,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #89:
+Central directory entry #90:
 ---------------------------
 
   static/pt/_static/language_data.js
 
-  offset of local header from start of archive:   2217389
-                                                  (000000000021D5ADh) bytes
+  offset of local header from start of archive:   2219468
+                                                  (000000000021DDCCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3303,21 +3339,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #90:
+Central directory entry #91:
 ---------------------------
 
   static/pt/_static/pygments.css
 
-  offset of local header from start of archive:   2220707
-                                                  (000000000021E2A3h) bytes
+  offset of local header from start of archive:   2222786
+                                                  (000000000021EAC2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3340,21 +3376,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #91:
+Central directory entry #92:
 ---------------------------
 
   static/pt/_static/logo.png
 
-  offset of local header from start of archive:   2221793
-                                                  (000000000021E6E1h) bytes
+  offset of local header from start of archive:   2223872
+                                                  (000000000021EF00h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3377,21 +3413,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #92:
+Central directory entry #93:
 ---------------------------
 
   static/pt/_static/base-stemmer.js
 
-  offset of local header from start of archive:   2402682
-                                                  (000000000024A97Ah) bytes
+  offset of local header from start of archive:   2404761
+                                                  (000000000024B199h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3414,21 +3450,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #93:
+Central directory entry #94:
 ---------------------------
 
   static/pt/_static/searchtools.js
 
-  offset of local header from start of archive:   2404255
-                                                  (000000000024AF9Fh) bytes
+  offset of local header from start of archive:   2406334
+                                                  (000000000024B7BEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3451,21 +3487,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #94:
+Central directory entry #95:
 ---------------------------
 
   static/pt/_static/css/theme.css
 
-  offset of local header from start of archive:   2410166
-                                                  (000000000024C6B6h) bytes
+  offset of local header from start of archive:   2412245
+                                                  (000000000024CED5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3488,21 +3524,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #95:
+Central directory entry #96:
 ---------------------------
 
   static/pt/_static/css/toggle.css
 
-  offset of local header from start of archive:   2432804
-                                                  (0000000000251F24h) bytes
+  offset of local header from start of archive:   2434883
+                                                  (0000000000252743h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3525,21 +3561,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #96:
+Central directory entry #97:
 ---------------------------
 
   static/pt/_static/css/badge_only.css
 
-  offset of local header from start of archive:   2433417
-                                                  (0000000000252189h) bytes
+  offset of local header from start of archive:   2435496
+                                                  (00000000002529A8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3562,21 +3598,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #97:
+Central directory entry #98:
 ---------------------------
 
   static/pt/_static/css/dark.css
 
-  offset of local header from start of archive:   2434581
-                                                  (0000000000252615h) bytes
+  offset of local header from start of archive:   2436660
+                                                  (0000000000252E34h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3599,21 +3635,57 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #98:
+Central directory entry #99:
+---------------------------
+
+  static/pt/_static/logo-32x32.ico
+
+  offset of local header from start of archive:   2438189
+                                                  (000000000025342Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2021 May 15 22:29:46
+  file last modified on (UT extra field modtime): 2021 May 16 05:29:45 local
+  file last modified on (UT extra field modtime): 2021 May 16 05:29:45 UTC
+  32-bit CRC value (hex):                         174acf66
+  compressed size:                                1989 bytes
+  uncompressed size:                              1989 bytes
+  length of filename:                             32 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (100664 octal):            -rw-rw-r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #100:
 ---------------------------
 
   static/pt/_static/portuguese-stemmer.js
 
-  offset of local header from start of archive:   2436110
-                                                  (0000000000252C0Eh) bytes
+  offset of local header from start of archive:   2440268
+                                                  (0000000000253C4Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3636,21 +3708,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #99:
+Central directory entry #101:
 ---------------------------
 
   static/pt/_static/js/html5shiv-printshiv.min.js
 
-  offset of local header from start of archive:   2438845
-                                                  (00000000002536BDh) bytes
+  offset of local header from start of archive:   2443003
+                                                  (00000000002546FBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3673,21 +3745,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #100:
+Central directory entry #102:
 ---------------------------
 
   static/pt/_static/js/badge_only.js
 
-  offset of local header from start of archive:   2440969
-                                                  (0000000000253F09h) bytes
+  offset of local header from start of archive:   2445127
+                                                  (0000000000254F47h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3710,21 +3782,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #101:
+Central directory entry #103:
 ---------------------------
 
   static/pt/_static/js/toggle.js
 
-  offset of local header from start of archive:   2441497
-                                                  (0000000000254119h) bytes
+  offset of local header from start of archive:   2445655
+                                                  (0000000000255157h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3747,21 +3819,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #102:
+Central directory entry #104:
 ---------------------------
 
   static/pt/_static/js/theme.js
 
-  offset of local header from start of archive:   2442119
-                                                  (0000000000254387h) bytes
+  offset of local header from start of archive:   2446277
+                                                  (00000000002553C5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3784,21 +3856,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #103:
+Central directory entry #105:
 ---------------------------
 
   static/pt/_static/js/html5shiv.min.js
 
-  offset of local header from start of archive:   2443983
-                                                  (0000000000254ACFh) bytes
+  offset of local header from start of archive:   2448141
+                                                  (0000000000255B0Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3821,21 +3893,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #104:
+Central directory entry #106:
 ---------------------------
 
   static/pt/_static/file.png
 
-  offset of local header from start of archive:   2445411
-                                                  (0000000000255063h) bytes
+  offset of local header from start of archive:   2449569
+                                                  (00000000002560A1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -3857,21 +3929,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #105:
+Central directory entry #107:
 ---------------------------
 
   static/pt/_static/doctools.js
 
-  offset of local header from start of archive:   2445781
-                                                  (00000000002551D5h) bytes
+  offset of local header from start of archive:   2449939
+                                                  (0000000000256213h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3894,21 +3966,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #106:
+Central directory entry #108:
 ---------------------------
 
   static/pt/_static/basic.css
 
-  offset of local header from start of archive:   2447501
-                                                  (000000000025588Dh) bytes
+  offset of local header from start of archive:   2451659
+                                                  (00000000002568CBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3931,21 +4003,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #107:
+Central directory entry #109:
 ---------------------------
 
   static/pt/chapter-15.html
 
-  offset of local header from start of archive:   2451057
-                                                  (0000000000256671h) bytes
+  offset of local header from start of archive:   2455215
+                                                  (00000000002576AFh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3968,21 +4040,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #108:
+Central directory entry #110:
 ---------------------------
 
   static/pt/chapter-12.html
 
-  offset of local header from start of archive:   2459333
-                                                  (00000000002586C5h) bytes
+  offset of local header from start of archive:   2463491
+                                                  (0000000000259703h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4005,21 +4077,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #109:
+Central directory entry #111:
 ---------------------------
 
   static/pt/searchindex.js
 
-  offset of local header from start of archive:   2485818
-                                                  (000000000025EE3Ah) bytes
+  offset of local header from start of archive:   2489976
+                                                  (000000000025FE78h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4042,21 +4114,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #110:
+Central directory entry #112:
 ---------------------------
 
   static/pt/chapter-02.html
 
-  offset of local header from start of archive:   2523052
-                                                  (0000000000267FACh) bytes
+  offset of local header from start of archive:   2527210
+                                                  (0000000000268FEAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4079,21 +4151,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #111:
+Central directory entry #113:
 ---------------------------
 
   static/pt/chapter-11.html
 
-  offset of local header from start of archive:   2529176
-                                                  (0000000000269798h) bytes
+  offset of local header from start of archive:   2533334
+                                                  (000000000026A7D6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4116,21 +4188,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #112:
+Central directory entry #114:
 ---------------------------
 
   static/pt/chapter-01.html
 
-  offset of local header from start of archive:   2532766
-                                                  (000000000026A59Eh) bytes
+  offset of local header from start of archive:   2536924
+                                                  (000000000026B5DCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4153,21 +4225,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #113:
+Central directory entry #115:
 ---------------------------
 
   static/pt/genindex.html
 
-  offset of local header from start of archive:   2538331
-                                                  (000000000026BB5Bh) bytes
+  offset of local header from start of archive:   2542489
+                                                  (000000000026CB99h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4190,21 +4262,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #114:
+Central directory entry #116:
 ---------------------------
 
   static/pt/toggle.css
 
-  offset of local header from start of archive:   2540406
-                                                  (000000000026C376h) bytes
+  offset of local header from start of archive:   2544564
+                                                  (000000000026D3B4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4227,21 +4299,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #115:
+Central directory entry #117:
 ---------------------------
 
   static/pt/chapter-08.html
 
-  offset of local header from start of archive:   2541007
-                                                  (000000000026C5CFh) bytes
+  offset of local header from start of archive:   2545165
+                                                  (000000000026D60Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4264,21 +4336,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #116:
+Central directory entry #118:
 ---------------------------
 
   static/pt/_images/form1.png
 
-  offset of local header from start of archive:   2549836
-                                                  (000000000026E84Ch) bytes
+  offset of local header from start of archive:   2553994
+                                                  (000000000026F88Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4301,21 +4373,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #117:
+Central directory entry #119:
 ---------------------------
 
   static/pt/_images/dashboard_ticket.png
 
-  offset of local header from start of archive:   2560427
-                                                  (00000000002711ABh) bytes
+  offset of local header from start of archive:   2564585
+                                                  (00000000002721E9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4338,21 +4410,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #118:
+Central directory entry #120:
 ---------------------------
 
   static/pt/_images/form3.png
 
-  offset of local header from start of archive:   2697733
-                                                  (0000000000292A05h) bytes
+  offset of local header from start of archive:   2701891
+                                                  (0000000000293A43h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4375,21 +4447,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #119:
+Central directory entry #121:
 ---------------------------
 
   static/pt/_images/dashboard_edit.png
 
-  offset of local header from start of archive:   2733565
-                                                  (000000000029B5FDh) bytes
+  offset of local header from start of archive:   2737723
+                                                  (000000000029C63Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4412,21 +4484,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #120:
+Central directory entry #122:
 ---------------------------
 
   static/pt/_images/form2.png
 
-  offset of local header from start of archive:   2902908
-                                                  (00000000002C4B7Ch) bytes
+  offset of local header from start of archive:   2907066
+                                                  (00000000002C5BBAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4449,21 +4521,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #121:
+Central directory entry #123:
 ---------------------------
 
   static/pt/_images/grid.png
 
-  offset of local header from start of archive:   2941191
-                                                  (00000000002CE107h) bytes
+  offset of local header from start of archive:   2945349
+                                                  (00000000002CF145h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4486,21 +4558,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #122:
+Central directory entry #124:
 ---------------------------
 
   static/pt/_images/restapi2.png
 
-  offset of local header from start of archive:   2980940
-                                                  (00000000002D7C4Ch) bytes
+  offset of local header from start of archive:   2985098
+                                                  (00000000002D8C8Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4523,21 +4595,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #123:
+Central directory entry #125:
 ---------------------------
 
   static/pt/_images/simple_counter.png
 
-  offset of local header from start of archive:   3008163
-                                                  (00000000002DE6A3h) bytes
+  offset of local header from start of archive:   3012321
+                                                  (00000000002DF6E1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4560,21 +4632,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #124:
+Central directory entry #126:
 ---------------------------
 
   static/pt/_images/restapi.png
 
-  offset of local header from start of archive:   3022441
-                                                  (00000000002E1E69h) bytes
+  offset of local header from start of archive:   3026599
+                                                  (00000000002E2EA7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4597,21 +4669,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #125:
+Central directory entry #127:
 ---------------------------
 
   static/pt/_images/form5.png
 
-  offset of local header from start of archive:   3051677
-                                                  (00000000002E909Dh) bytes
+  offset of local header from start of archive:   3055835
+                                                  (00000000002EA0DBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4634,21 +4706,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #126:
+Central directory entry #128:
 ---------------------------
 
   static/pt/_images/dashboard_login.png
 
-  offset of local header from start of archive:   3089736
-                                                  (00000000002F2548h) bytes
+  offset of local header from start of archive:   3093894
+                                                  (00000000002F3586h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4671,21 +4743,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #127:
+Central directory entry #129:
 ---------------------------
 
   static/pt/_images/dashboard_restapi.png
 
-  offset of local header from start of archive:   3170767
-                                                  (00000000003061CFh) bytes
+  offset of local header from start of archive:   3174925
+                                                  (000000000030720Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4708,21 +4780,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #128:
+Central directory entry #130:
 ---------------------------
 
   static/pt/_images/dashboard_main.png
 
-  offset of local header from start of archive:   3313060
-                                                  (0000000000328DA4h) bytes
+  offset of local header from start of archive:   3317218
+                                                  (0000000000329DE2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4745,21 +4817,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #129:
+Central directory entry #131:
 ---------------------------
 
   static/pt/_images/grid_columns.png
 
-  offset of local header from start of archive:   3442855
-                                                  (00000000003488A7h) bytes
+  offset of local header from start of archive:   3447013
+                                                  (00000000003498E5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4782,21 +4854,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #130:
+Central directory entry #132:
 ---------------------------
 
   static/pt/_images/grid_bulmacss.png
 
-  offset of local header from start of archive:   3499356
-                                                  (000000000035655Ch) bytes
+  offset of local header from start of archive:   3503514
+                                                  (000000000035759Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4819,21 +4891,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #131:
+Central directory entry #133:
 ---------------------------
 
   static/pt/_images/_scaffold.png
 
-  offset of local header from start of archive:   3538145
-                                                  (000000000035FCE1h) bytes
+  offset of local header from start of archive:   3542303
+                                                  (0000000000360D1Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4856,21 +4928,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #132:
+Central directory entry #134:
 ---------------------------
 
   static/pt/_images/logo.png
 
-  offset of local header from start of archive:   3548907
-                                                  (00000000003626EBh) bytes
+  offset of local header from start of archive:   3553065
+                                                  (0000000000363729h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4893,21 +4965,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #133:
+Central directory entry #135:
 ---------------------------
 
   static/pt/_images/dashboard.png
 
-  offset of local header from start of archive:   3729796
-                                                  (000000000038E984h) bytes
+  offset of local header from start of archive:   3733954
+                                                  (000000000038F9C2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4930,21 +5002,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #134:
+Central directory entry #136:
 ---------------------------
 
   static/pt/_images/tags2.png
 
-  offset of local header from start of archive:   3773504
-                                                  (0000000000399440h) bytes
+  offset of local header from start of archive:   3777662
+                                                  (000000000039A47Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4967,21 +5039,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #135:
+Central directory entry #137:
 ---------------------------
 
   static/pt/_images/form4.png
 
-  offset of local header from start of archive:   3803143
-                                                  (00000000003A0807h) bytes
+  offset of local header from start of archive:   3807301
+                                                  (00000000003A1845h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5004,21 +5076,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #136:
+Central directory entry #138:
 ---------------------------
 
   static/pt/_images/dashboard_error.png
 
-  offset of local header from start of archive:   3846961
-                                                  (00000000003AB331h) bytes
+  offset of local header from start of archive:   3851119
+                                                  (00000000003AC36Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5041,21 +5113,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #137:
+Central directory entry #139:
 ---------------------------
 
   static/pt/_images/grid_nocss.png
 
-  offset of local header from start of archive:   3894980
-                                                  (00000000003B6EC4h) bytes
+  offset of local header from start of archive:   3899138
+                                                  (00000000003B7F02h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5078,21 +5150,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #138:
+Central directory entry #140:
 ---------------------------
 
   static/pt/_images/tags_db.png
 
-  offset of local header from start of archive:   3938059
-                                                  (00000000003C170Bh) bytes
+  offset of local header from start of archive:   3942217
+                                                  (00000000003C2749h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5115,21 +5187,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #139:
+Central directory entry #141:
 ---------------------------
 
   static/pt/_images/dashboard_new_app.png
 
-  offset of local header from start of archive:   3961679
-                                                  (00000000003C734Fh) bytes
+  offset of local header from start of archive:   3965837
+                                                  (00000000003C838Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5152,21 +5224,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #140:
+Central directory entry #142:
 ---------------------------
 
   static/pt/_images/main_page.png
 
-  offset of local header from start of archive:   3999226
-                                                  (00000000003D05FAh) bytes
+  offset of local header from start of archive:   4003384
+                                                  (00000000003D1638h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5189,21 +5261,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #141:
+Central directory entry #143:
 ---------------------------
 
   static/pt/_images/command.png
 
-  offset of local header from start of archive:   4058326
-                                                  (00000000003DECD6h) bytes
+  offset of local header from start of archive:   4062484
+                                                  (00000000003DFD14h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5226,21 +5298,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #142:
+Central directory entry #144:
 ---------------------------
 
   static/pt/_images/first_run.png
 
-  offset of local header from start of archive:   4092423
-                                                  (00000000003E7207h) bytes
+  offset of local header from start of archive:   4096581
+                                                  (00000000003E8245h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5263,21 +5335,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #143:
+Central directory entry #145:
 ---------------------------
 
   static/pt/_images/form6.png
 
-  offset of local header from start of archive:   4137819
-                                                  (00000000003F235Bh) bytes
+  offset of local header from start of archive:   4141977
+                                                  (00000000003F3399h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5300,21 +5372,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #144:
+Central directory entry #146:
 ---------------------------
 
   static/pt/dark.css
 
-  offset of local header from start of archive:   4174227
-                                                  (00000000003FB193h) bytes
+  offset of local header from start of archive:   4178385
+                                                  (00000000003FC1D1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5337,21 +5409,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #145:
+Central directory entry #147:
 ---------------------------
 
   static/pt/chapter-07.html
 
-  offset of local header from start of archive:   4175744
-                                                  (00000000003FB780h) bytes
+  offset of local header from start of archive:   4179902
+                                                  (00000000003FC7BEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5374,21 +5446,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #146:
+Central directory entry #148:
 ---------------------------
 
   static/pt/chapter-04.html
 
-  offset of local header from start of archive:   4246543
-                                                  (000000000040CC0Fh) bytes
+  offset of local header from start of archive:   4250701
+                                                  (000000000040DC4Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5411,21 +5483,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #147:
+Central directory entry #149:
 ---------------------------
 
   static/pt/search.html
 
-  offset of local header from start of archive:   4250472
-                                                  (000000000040DB68h) bytes
+  offset of local header from start of archive:   4254630
+                                                  (000000000040EBA6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5448,21 +5520,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #148:
+Central directory entry #150:
 ---------------------------
 
   static/pt/chapter-13.html
 
-  offset of local header from start of archive:   4252631
-                                                  (000000000040E3D7h) bytes
+  offset of local header from start of archive:   4256789
+                                                  (000000000040F415h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5485,21 +5557,58 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #149:
+Central directory entry #151:
+---------------------------
+
+  static/favicon.ico
+
+  offset of local header from start of archive:   4267237
+                                                  (0000000000411CE5h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Mar 7 16:27:04
+  file last modified on (UT extra field modtime): 2023 Mar 8 00:27:03 local
+  file last modified on (UT extra field modtime): 2023 Mar 8 00:27:03 UTC
+  32-bit CRC value (hex):                         21d942a1
+  compressed size:                                4672 bytes
+  uncompressed size:                              32038 bytes
+  length of filename:                             18 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #152:
 ---------------------------
 
   __init__.py
 
-  offset of local header from start of archive:   4263079
-                                                  (0000000000410CA7h) bytes
+  offset of local header from start of archive:   4271985
+                                                  (0000000000412F71h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
```

#### zipnote {}

```diff
@@ -60,14 +60,17 @@
 
 Filename: static/en/_static/css/badge_only.css
 Comment: 
 
 Filename: static/en/_static/css/dark.css
 Comment: 
 
+Filename: static/en/_static/logo-32x32.ico
+Comment: 
+
 Filename: static/en/_static/js/html5shiv-printshiv.min.js
 Comment: 
 
 Filename: static/en/_static/js/badge_only.js
 Comment: 
 
 Filename: static/en/_static/js/toggle.js
@@ -285,14 +288,17 @@
 
 Filename: static/pt/_static/css/badge_only.css
 Comment: 
 
 Filename: static/pt/_static/css/dark.css
 Comment: 
 
+Filename: static/pt/_static/logo-32x32.ico
+Comment: 
+
 Filename: static/pt/_static/portuguese-stemmer.js
 Comment: 
 
 Filename: static/pt/_static/js/html5shiv-printshiv.min.js
 Comment: 
 
 Filename: static/pt/_static/js/badge_only.js
@@ -438,11 +444,14 @@
 
 Filename: static/pt/search.html
 Comment: 
 
 Filename: static/pt/chapter-13.html
 Comment: 
 
+Filename: static/favicon.ico
+Comment: 
+
 Filename: __init__.py
 Comment: 
 
 Zip file comment:
```

### Comparing `py4web-1.20230416.2/py4web/assets/py4web.app._scaffold.zip` & `py4web-1.20230416.3/py4web/assets/py4web.app._scaffold.zip`

 * *Files 27% similar despite different names*

#### zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                     16674 (0000000000004122h)
-  Actual end-cent-dir record offset:         16652 (000000000000410Ch)
-  Expected end-cent-dir record offset:       16652 (000000000000410Ch)
+  Zip archive file size:                     21524 (0000000000005414h)
+  Actual end-cent-dir record offset:         21502 (00000000000053FEh)
+  Expected end-cent-dir record offset:       21502 (00000000000053FEh)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 15 entries.
-  The central directory is 1284 (0000000000000504h) bytes long,
+  central directory contains 16 entries.
+  The central directory is 1372 (000000000000055Ch) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 15368 (0000000000003C08h).
+  is 20130 (0000000000004EA2h).
 
 
 Central directory entry #1:
 ---------------------------
 
   common.py
 
@@ -173,20 +173,20 @@
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 19 15:19:02
-  file last modified on (UT extra field modtime): 2023 Mar 19 22:19:01 local
-  file last modified on (UT extra field modtime): 2023 Mar 19 22:19:01 UTC
-  32-bit CRC value (hex):                         bc2e37ac
-  compressed size:                                4133 bytes
-  uncompressed size:                              11826 bytes
+  file last modified on (DOS date/time):          2023 Apr 16 17:36:34
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:36:33 local
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:36:33 UTC
+  32-bit CRC value (hex):                         84d306f5
+  compressed size:                                4147 bytes
+  uncompressed size:                              11888 bytes
   length of filename:                             18 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
@@ -198,18 +198,55 @@
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
 Central directory entry #6:
 ---------------------------
 
+  static/favicon.ico
+
+  offset of local header from start of archive:   11380
+                                                  (0000000000002C74h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2020 Aug 29 18:41:52
+  file last modified on (UT extra field modtime): 2020 Aug 30 01:41:52 local
+  file last modified on (UT extra field modtime): 2020 Aug 30 01:41:52 UTC
+  32-bit CRC value (hex):                         21d942a1
+  compressed size:                                4672 bytes
+  uncompressed size:                              32038 bytes
+  length of filename:                             18 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #7:
+---------------------------
+
   tasks.py
 
-  offset of local header from start of archive:   11366
-                                                  (0000000000002C66h) bytes
+  offset of local header from start of archive:   16128
+                                                  (0000000000003F00h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -232,21 +269,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #7:
+Central directory entry #8:
 ---------------------------
 
   __init__.py
 
-  offset of local header from start of archive:   11908
-                                                  (0000000000002E84h) bytes
+  offset of local header from start of archive:   16670
+                                                  (000000000000411Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -269,21 +306,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #8:
+Central directory entry #9:
 ---------------------------
 
   models.py
 
-  offset of local header from start of archive:   12207
-                                                  (0000000000002FAFh) bytes
+  offset of local header from start of archive:   16969
+                                                  (0000000000004249h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -306,21 +343,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #9:
+Central directory entry #10:
 ---------------------------
 
   templates/index.html
 
-  offset of local header from start of archive:   12443
-                                                  (000000000000309Bh) bytes
+  offset of local header from start of archive:   17205
+                                                  (0000000000004335h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -343,21 +380,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #10:
+Central directory entry #11:
 ---------------------------
 
   templates/README.md
 
-  offset of local header from start of archive:   12603
-                                                  (000000000000313Bh) bytes
+  offset of local header from start of archive:   17365
+                                                  (00000000000043D5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -379,21 +416,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #11:
+Central directory entry #12:
 ---------------------------
 
   templates/generic.html
 
-  offset of local header from start of archive:   12681
-                                                  (0000000000003189h) bytes
+  offset of local header from start of archive:   17443
+                                                  (0000000000004423h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -416,21 +453,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #12:
+Central directory entry #13:
 ---------------------------
 
   templates/layout.html
 
-  offset of local header from start of archive:   12944
-                                                  (0000000000003290h) bytes
+  offset of local header from start of archive:   17706
+                                                  (000000000000452Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -453,21 +490,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #13:
+Central directory entry #14:
 ---------------------------
 
   templates/auth.html
 
-  offset of local header from start of archive:   14242
-                                                  (00000000000037A2h) bytes
+  offset of local header from start of archive:   19004
+                                                  (0000000000004A3Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -490,21 +527,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #14:
+Central directory entry #15:
 ---------------------------
 
   controllers.py
 
-  offset of local header from start of archive:   14494
-                                                  (000000000000389Eh) bytes
+  offset of local header from start of archive:   19256
+                                                  (0000000000004B38h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -527,21 +564,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #15:
+Central directory entry #16:
 ---------------------------
 
   translations/it.json
 
-  offset of local header from start of archive:   15213
-                                                  (0000000000003B6Dh) bytes
+  offset of local header from start of archive:   19975
+                                                  (0000000000004E07h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
```

#### zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: static/css/no.css
 Comment: 
 
 Filename: static/js/utils.js
 Comment: 
 
+Filename: static/favicon.ico
+Comment: 
+
 Filename: tasks.py
 Comment: 
 
 Filename: __init__.py
 Comment: 
 
 Filename: models.py
```

#### static/js/utils.js

##### js-beautify {}

```diff
@@ -197,45 +197,51 @@
     var keys = Q.eval(elem.value || '[]');
     keys.map(function(x) {
         if (tags.indexOf(x) < 0) tags.push(x);
     });
     var fill = function(elem, repl) {
         repl.innerHTML = '';
         tags.forEach(function(x) {
-            console.log(x);
             var item = document.createElement('li');
             item.innerHTML = options.labels[x] || x;
             item.dataset.value = x;
             item.dataset.selected = keys.indexOf(x) >= 0;
             repl.appendChild(item);
             item.onclick = function(evt) {
                 if (item.dataset.selected == 'false') keys.push(x);
                 else keys = keys.filter(function(y) {
                     return x != y;
                 });
                 item.dataset.selected = keys.indexOf(x) >= 0;
                 elem.value = JSON.stringify(keys);
+                elem.dispatchEvent(new Event('input', {
+                    bubbles: true
+                }));
             };
         });
     };
     if (options.freetext) {
         var inp = document.createElement('input');
         elem.parentNode.insertBefore(inp, elem);
+        inp.type = "text";
         inp.classList = elem.classList;
         inp.placeholder = options.placeholder;
         inp.setAttribute('list', options.autocomplete_list);
         inp.onchange = function(evt) {
             inp.value.split(',').map(function(x) {
                 x = options.transform(x.trim());
                 if (options.regex && !x.match(options.regex)) return;
                 if (x && tags.indexOf(x) < 0) tags.push(x);
                 if (x && keys.indexOf(x) < 0) keys.push(x);
             });
             inp.value = '';
             elem.value = JSON.stringify(keys);
+            elem.dispatchEvent(new Event('input', {
+                bubbles: true
+            }));
             fill(elem, repl);
         };
     }
     fill(elem, repl);
 };
 
 // Password strenght calculator
@@ -292,15 +298,14 @@
     method = (method || 'GET').toLowerCase();
     /* if target is not there, fill it with something that there isn't in the page*/
     if (target === void 0 || target === '') target = 'none';
     var onsuccess = function(res) {
         if (res.redirected) window.location = res.url;
         Q('#' + target)[0].innerHTML = res.data;
         Q.trap_form(url, target);
-        console.log(res.headers);
         var flash = res.headers.get('component-flash');
         if (flash) Q.flash(JSON.parse(flash));
     };
     var onerror = function(res) {
         alert('ajax error');
     };
     Q.ajax(method, url, form_data).then(onsuccess).catch(onerror);
@@ -334,15 +339,14 @@
     if (elem) {
         elem.addEventListener('flash', make_handler(elem), false);
         Q.flash = function(detail) {
             elem.dispatchEvent(new CustomEvent('flash', {
                 detail: detail
             }));
         };
-        console.log(elem.dataset.alert);
         if (elem.dataset.alert) Q.flash(Q.eval(elem.dataset.alert));
     }
 };
 
 Q.handle_components();
 Q.handle_flash();
 Q('input[type=text].type-list-string').forEach(function(elem) {
```

### Comparing `py4web-1.20230416.2/py4web/assets/py4web.app.showcase.zip` & `py4web-1.20230416.3/py4web/assets/py4web.app.showcase.zip`

 * *Files 4% similar despite different names*

#### zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                   1386102 (0000000000152676h)
-  Actual end-cent-dir record offset:       1386080 (0000000000152660h)
-  Expected end-cent-dir record offset:     1386080 (0000000000152660h)
+  Zip archive file size:                   1392585 (0000000000153FC9h)
+  Actual end-cent-dir record offset:       1392563 (0000000000153FB3h)
+  Expected end-cent-dir record offset:     1392563 (0000000000153FB3h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 143 entries.
-  The central directory is 14426 (000000000000385Ah) bytes long,
+  central directory contains 144 entries.
+  The central directory is 14514 (00000000000038B2h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 1371654 (000000000014EE06h).
+  is 1378049 (0000000000150701h).
 
 
 Central directory entry #1:
 ---------------------------
 
   examples/session_counter.py
 
@@ -1909,20 +1909,20 @@
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Jun 2 22:12:20
-  file last modified on (UT extra field modtime): 2022 Jun 3 05:12:20 local
-  file last modified on (UT extra field modtime): 2022 Jun 3 05:12:20 UTC
-  32-bit CRC value (hex):                         f3d83ef6
-  compressed size:                                1693 bytes
-  uncompressed size:                              6013 bytes
+  file last modified on (DOS date/time):          2023 Apr 16 17:34:50
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:34:50 local
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:34:50 UTC
+  32-bit CRC value (hex):                         8155e653
+  compressed size:                                2245 bytes
+  uncompressed size:                              8097 bytes
   length of filename:                             27 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
@@ -1936,16 +1936,16 @@
   There is no file comment.
 
 Central directory entry #53:
 ---------------------------
 
   static/components/starrater/starrater.html
 
-  offset of local header from start of archive:   99040
-                                                  (00000000000182E0h) bytes
+  offset of local header from start of archive:   99592
+                                                  (0000000000018508h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -1973,16 +1973,16 @@
   There is no file comment.
 
 Central directory entry #54:
 ---------------------------
 
   static/components/starrater/starrater.js
 
-  offset of local header from start of archive:   99288
-                                                  (00000000000183D8h) bytes
+  offset of local header from start of archive:   99840
+                                                  (0000000000018600h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2010,16 +2010,16 @@
   There is no file comment.
 
 Central directory entry #55:
 ---------------------------
 
   static/components/starrater/starrater.css
 
-  offset of local header from start of archive:   99920
-                                                  (0000000000018650h) bytes
+  offset of local header from start of archive:   100472
+                                                  (0000000000018878h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -2046,30 +2046,30 @@
   There is no file comment.
 
 Central directory entry #56:
 ---------------------------
 
   static/components/mtable.html
 
-  offset of local header from start of archive:   100019
-                                                  (00000000000186B3h) bytes
+  offset of local header from start of archive:   100571
+                                                  (00000000000188DBh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Jun 2 22:12:20
-  file last modified on (UT extra field modtime): 2022 Jun 3 05:12:20 local
-  file last modified on (UT extra field modtime): 2022 Jun 3 05:12:20 UTC
-  32-bit CRC value (hex):                         c4131866
-  compressed size:                                1318 bytes
-  uncompressed size:                              5682 bytes
+  file last modified on (DOS date/time):          2023 Apr 16 17:12:08
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:12:08 local
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:12:08 UTC
+  32-bit CRC value (hex):                         9bb8ce4d
+  compressed size:                                1582 bytes
+  uncompressed size:                              7447 bytes
   length of filename:                             29 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
@@ -2083,16 +2083,16 @@
   There is no file comment.
 
 Central directory entry #57:
 ---------------------------
 
   static/firebase-push.html
 
-  offset of local header from start of archive:   101424
-                                                  (0000000000018C30h) bytes
+  offset of local header from start of archive:   102240
+                                                  (0000000000018F60h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2120,16 +2120,16 @@
   There is no file comment.
 
 Central directory entry #58:
 ---------------------------
 
   static/socketio/README.md
 
-  offset of local header from start of archive:   101944
-                                                  (0000000000018E38h) bytes
+  offset of local header from start of archive:   102760
+                                                  (0000000000019168h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -2156,16 +2156,16 @@
   There is no file comment.
 
 Central directory entry #59:
 ---------------------------
 
   static/error.html
 
-  offset of local header from start of archive:   102028
-                                                  (0000000000018E8Ch) bytes
+  offset of local header from start of archive:   102844
+                                                  (00000000000191BCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2193,16 +2193,16 @@
   There is no file comment.
 
 Central directory entry #60:
 ---------------------------
 
   static/css/prism.css
 
-  offset of local header from start of archive:   105114
-                                                  (0000000000019A9Ah) bytes
+  offset of local header from start of archive:   105930
+                                                  (0000000000019DCAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2230,16 +2230,16 @@
   There is no file comment.
 
 Central directory entry #61:
 ---------------------------
 
   static/css/no.css
 
-  offset of local header from start of archive:   105938
-                                                  (0000000000019DD2h) bytes
+  offset of local header from start of archive:   106754
+                                                  (000000000001A102h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2267,16 +2267,16 @@
   There is no file comment.
 
 Central directory entry #62:
 ---------------------------
 
   static/css/prism.js
 
-  offset of local header from start of archive:   109246
-                                                  (000000000001AABEh) bytes
+  offset of local header from start of archive:   110062
+                                                  (000000000001ADEEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2304,16 +2304,16 @@
   There is no file comment.
 
 Central directory entry #63:
 ---------------------------
 
   static/js/star_rater_vue.js
 
-  offset of local header from start of archive:   116277
-                                                  (000000000001C635h) bytes
+  offset of local header from start of archive:   117093
+                                                  (000000000001C965h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2341,16 +2341,16 @@
   There is no file comment.
 
 Central directory entry #64:
 ---------------------------
 
   static/js/firebase-push.js
 
-  offset of local header from start of archive:   116641
-                                                  (000000000001C7A1h) bytes
+  offset of local header from start of archive:   117457
+                                                  (000000000001CAD1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2378,16 +2378,16 @@
   There is no file comment.
 
 Central directory entry #65:
 ---------------------------
 
   static/js/sugar.min.js
 
-  offset of local header from start of archive:   117043
-                                                  (000000000001C933h) bytes
+  offset of local header from start of archive:   117859
+                                                  (000000000001CC63h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2415,16 +2415,16 @@
   There is no file comment.
 
 Central directory entry #66:
 ---------------------------
 
   static/js/utils.min.js
 
-  offset of local header from start of archive:   142227
-                                                  (0000000000022B93h) bytes
+  offset of local header from start of archive:   143043
+                                                  (0000000000022EC3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2452,30 +2452,30 @@
   There is no file comment.
 
 Central directory entry #67:
 ---------------------------
 
   static/js/utils.js
 
-  offset of local header from start of archive:   145449
-                                                  (0000000000023829h) bytes
+  offset of local header from start of archive:   146265
+                                                  (0000000000023B59h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Jun 2 22:12:20
-  file last modified on (UT extra field modtime): 2022 Jun 3 05:12:20 local
-  file last modified on (UT extra field modtime): 2022 Jun 3 05:12:20 UTC
-  32-bit CRC value (hex):                         bc2e37ac
-  compressed size:                                4133 bytes
-  uncompressed size:                              11826 bytes
+  file last modified on (DOS date/time):          2023 Apr 16 17:36:34
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:36:33 local
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:36:33 UTC
+  32-bit CRC value (hex):                         84d306f5
+  compressed size:                                4147 bytes
+  uncompressed size:                              11888 bytes
   length of filename:                             18 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
@@ -2489,16 +2489,16 @@
   There is no file comment.
 
 Central directory entry #68:
 ---------------------------
 
   static/js/axios.min.js
 
-  offset of local header from start of archive:   149658
-                                                  (000000000002489Ah) bytes
+  offset of local header from start of archive:   150488
+                                                  (0000000000024BD8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2526,16 +2526,16 @@
   There is no file comment.
 
 Central directory entry #69:
 ---------------------------
 
   static/js/vue.min.js
 
-  offset of local header from start of archive:   154652
-                                                  (0000000000025C1Ch) bytes
+  offset of local header from start of archive:   155482
+                                                  (0000000000025F5Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2563,16 +2563,16 @@
   There is no file comment.
 
 Central directory entry #70:
 ---------------------------
 
   static/js/prism.js
 
-  offset of local header from start of archive:   188705
-                                                  (000000000002E121h) bytes
+  offset of local header from start of archive:   189535
+                                                  (000000000002E45Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2600,16 +2600,16 @@
   There is no file comment.
 
 Central directory entry #71:
 ---------------------------
 
   static/js/vue.js
 
-  offset of local header from start of archive:   195728
-                                                  (000000000002FC90h) bytes
+  offset of local header from start of archive:   196558
+                                                  (000000000002FFCEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2635,18 +2635,55 @@
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
 Central directory entry #72:
 ---------------------------
 
+  static/favicon.ico
+
+  offset of local header from start of archive:   286461
+                                                  (0000000000045EFDh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2022 Jun 2 22:12:20
+  file last modified on (UT extra field modtime): 2022 Jun 3 05:12:20 local
+  file last modified on (UT extra field modtime): 2022 Jun 3 05:12:20 UTC
+  32-bit CRC value (hex):                         21d942a1
+  compressed size:                                4672 bytes
+  uncompressed size:                              32038 bytes
+  length of filename:                             18 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (100664 octal):            -rw-rw-r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #73:
+---------------------------
+
   static/components-bulma/grid/grid.js
 
-  offset of local header from start of archive:   285631
-                                                  (0000000000045BBFh) bytes
+  offset of local header from start of archive:   291209
+                                                  (0000000000047189h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2669,21 +2706,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #73:
+Central directory entry #74:
 ---------------------------
 
   static/components-bulma/grid/grid.html
 
-  offset of local header from start of archive:   287212
-                                                  (00000000000461ECh) bytes
+  offset of local header from start of archive:   292790
+                                                  (00000000000477B6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2706,21 +2743,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #74:
+Central directory entry #75:
 ---------------------------
 
   static/components-bulma/grid/luxon.js
 
-  offset of local header from start of archive:   288251
-                                                  (00000000000465FBh) bytes
+  offset of local header from start of archive:   293829
+                                                  (0000000000047BC5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2743,21 +2780,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #75:
+Central directory entry #76:
 ---------------------------
 
   static/components-bulma/grid/grid.css
 
-  offset of local header from start of archive:   342651
-                                                  (0000000000053A7Bh) bytes
+  offset of local header from start of archive:   348229
+                                                  (0000000000055045h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2780,21 +2817,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #76:
+Central directory entry #77:
 ---------------------------
 
   static/components-bulma/vueform/vueform.css
 
-  offset of local header from start of archive:   342962
-                                                  (0000000000053BB2h) bytes
+  offset of local header from start of archive:   348540
+                                                  (000000000005517Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -2816,21 +2853,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #77:
+Central directory entry #78:
 ---------------------------
 
   static/components-bulma/vueform/luxon.js
 
-  offset of local header from start of archive:   343106
-                                                  (0000000000053C42h) bytes
+  offset of local header from start of archive:   348684
+                                                  (000000000005520Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2853,21 +2890,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #78:
+Central directory entry #79:
 ---------------------------
 
   static/components-bulma/vueform/luxon.min.js
 
-  offset of local header from start of archive:   397509
-                                                  (00000000000610C5h) bytes
+  offset of local header from start of archive:   403087
+                                                  (000000000006268Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2890,21 +2927,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #79:
+Central directory entry #80:
 ---------------------------
 
   static/components-bulma/vueform/vueform.html
 
-  offset of local header from start of archive:   418412
-                                                  (000000000006626Ch) bytes
+  offset of local header from start of archive:   423990
+                                                  (0000000000067836h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2927,21 +2964,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #80:
+Central directory entry #81:
 ---------------------------
 
   static/components-bulma/vueform/vueform.js
 
-  offset of local header from start of archive:   419369
-                                                  (0000000000066629h) bytes
+  offset of local header from start of archive:   424947
+                                                  (0000000000067BF3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -2964,21 +3001,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #81:
+Central directory entry #82:
 ---------------------------
 
   static/components-bulma/fileupload/fileupload.html
 
-  offset of local header from start of archive:   421215
-                                                  (0000000000066D5Fh) bytes
+  offset of local header from start of archive:   426793
+                                                  (0000000000068329h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3001,21 +3038,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #82:
+Central directory entry #83:
 ---------------------------
 
   static/components-bulma/fileupload/fileupload.js
 
-  offset of local header from start of archive:   421391
-                                                  (0000000000066E0Fh) bytes
+  offset of local header from start of archive:   426969
+                                                  (00000000000683D9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3038,21 +3075,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #83:
+Central directory entry #84:
 ---------------------------
 
   static/components-bulma/fileupload/fileupload.css
 
-  offset of local header from start of archive:   421994
-                                                  (000000000006706Ah) bytes
+  offset of local header from start of archive:   427572
+                                                  (0000000000068634h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -3074,35 +3111,35 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #84:
+Central directory entry #85:
 ---------------------------
 
   static/components-bulma/mtable.js
 
-  offset of local header from start of archive:   422136
-                                                  (00000000000670F8h) bytes
+  offset of local header from start of archive:   427714
+                                                  (00000000000686C2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Jun 2 22:12:20
-  file last modified on (UT extra field modtime): 2022 Jun 3 05:12:20 local
-  file last modified on (UT extra field modtime): 2022 Jun 3 05:12:20 UTC
-  32-bit CRC value (hex):                         f3d83ef6
-  compressed size:                                1693 bytes
-  uncompressed size:                              6013 bytes
+  file last modified on (DOS date/time):          2023 Apr 16 17:34:50
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:34:50 local
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:34:50 UTC
+  32-bit CRC value (hex):                         8155e653
+  compressed size:                                2245 bytes
+  uncompressed size:                              8097 bytes
   length of filename:                             33 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
@@ -3111,21 +3148,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #85:
+Central directory entry #86:
 ---------------------------
 
   static/components-bulma/starrater/starrater.html
 
-  offset of local header from start of archive:   423920
-                                                  (00000000000677F0h) bytes
+  offset of local header from start of archive:   430050
+                                                  (0000000000068FE2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3148,21 +3185,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #86:
+Central directory entry #87:
 ---------------------------
 
   static/components-bulma/starrater/starrater.js
 
-  offset of local header from start of archive:   424174
-                                                  (00000000000678EEh) bytes
+  offset of local header from start of archive:   430304
+                                                  (00000000000690E0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3185,21 +3222,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #87:
+Central directory entry #88:
 ---------------------------
 
   static/components-bulma/starrater/starrater.css
 
-  offset of local header from start of archive:   424817
-                                                  (0000000000067B71h) bytes
+  offset of local header from start of archive:   430947
+                                                  (0000000000069363h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -3221,35 +3258,35 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #88:
+Central directory entry #89:
 ---------------------------
 
   static/components-bulma/mtable.html
 
-  offset of local header from start of archive:   424922
-                                                  (0000000000067BDAh) bytes
+  offset of local header from start of archive:   431052
+                                                  (00000000000693CCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Jun 2 22:12:20
-  file last modified on (UT extra field modtime): 2022 Jun 3 05:12:20 local
-  file last modified on (UT extra field modtime): 2022 Jun 3 05:12:20 UTC
-  32-bit CRC value (hex):                         c4131866
-  compressed size:                                1318 bytes
-  uncompressed size:                              5682 bytes
+  file last modified on (DOS date/time):          2023 Apr 16 17:12:08
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:12:08 local
+  file last modified on (UT extra field modtime): 2023 Apr 17 00:12:08 UTC
+  32-bit CRC value (hex):                         9bb8ce4d
+  compressed size:                                1582 bytes
+  uncompressed size:                              7447 bytes
   length of filename:                             35 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
@@ -3258,21 +3295,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #89:
+Central directory entry #90:
 ---------------------------
 
   static/data/uscities.json
 
-  offset of local header from start of archive:   426333
-                                                  (000000000006815Dh) bytes
+  offset of local header from start of archive:   432727
+                                                  (0000000000069A57h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3295,21 +3332,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #90:
+Central directory entry #91:
 ---------------------------
 
   static/data/zip_codes.json
 
-  offset of local header from start of archive:   1238909
-                                                  (000000000012E77Dh) bytes
+  offset of local header from start of archive:   1245303
+                                                  (0000000000130077h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3332,21 +3369,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #91:
+Central directory entry #92:
 ---------------------------
 
   __init__.py
 
-  offset of local header from start of archive:   1339998
-                                                  (000000000014725Eh) bytes
+  offset of local header from start of archive:   1346392
+                                                  (0000000000148B58h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3369,21 +3406,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #92:
+Central directory entry #93:
 ---------------------------
 
   uploads/README.md
 
-  offset of local header from start of archive:   1341198
-                                                  (000000000014770Eh) bytes
+  offset of local header from start of archive:   1347592
+                                                  (0000000000149008h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -3405,35 +3442,35 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #93:
+Central directory entry #94:
 ---------------------------
 
   templates/index.html
 
-  offset of local header from start of archive:   1341293
-                                                  (000000000014776Dh) bytes
+  offset of local header from start of archive:   1347687
+                                                  (0000000000149067h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Jun 8 00:32:52
-  file last modified on (UT extra field modtime): 2022 Jun 8 07:32:52 local
-  file last modified on (UT extra field modtime): 2022 Jun 8 07:32:52 UTC
-  32-bit CRC value (hex):                         68bd738b
-  compressed size:                                1062 bytes
-  uncompressed size:                              6784 bytes
+  file last modified on (DOS date/time):          2023 Apr 15 11:24:58
+  file last modified on (UT extra field modtime): 2023 Apr 15 18:24:57 local
+  file last modified on (UT extra field modtime): 2023 Apr 15 18:24:57 UTC
+  32-bit CRC value (hex):                         4f4ad5c0
+  compressed size:                                1063 bytes
+  uncompressed size:                              6788 bytes
   length of filename:                             20 characters
   length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
@@ -3442,21 +3479,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #94:
+Central directory entry #95:
 ---------------------------
 
   templates/ws/ws_index.html
 
-  offset of local header from start of archive:   1342433
-                                                  (0000000000147BE1h) bytes
+  offset of local header from start of archive:   1348828
+                                                  (00000000001494DCh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3479,21 +3516,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #95:
+Central directory entry #96:
 ---------------------------
 
   templates/examples/session_counter.html
 
-  offset of local header from start of archive:   1343384
-                                                  (0000000000147F98h) bytes
+  offset of local header from start of archive:   1349779
+                                                  (0000000000149893h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3516,21 +3553,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #96:
+Central directory entry #97:
 ---------------------------
 
   templates/examples/flash_example.html
 
-  offset of local header from start of archive:   1343636
-                                                  (0000000000148094h) bytes
+  offset of local header from start of archive:   1350031
+                                                  (000000000014998Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3553,21 +3590,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #97:
+Central directory entry #98:
 ---------------------------
 
   templates/examples/tagsinput_form.html
 
-  offset of local header from start of archive:   1343900
-                                                  (000000000014819Ch) bytes
+  offset of local header from start of archive:   1350295
+                                                  (0000000000149A97h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3590,21 +3627,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #98:
+Central directory entry #99:
 ---------------------------
 
   templates/examples/flash_example_next.html
 
-  offset of local header from start of archive:   1344779
-                                                  (000000000014850Bh) bytes
+  offset of local header from start of archive:   1351174
+                                                  (0000000000149E06h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -3626,21 +3663,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #99:
+Central directory entry #100:
 ---------------------------
 
   templates/examples/forms.html
 
-  offset of local header from start of archive:   1344905
-                                                  (0000000000148589h) bytes
+  offset of local header from start of archive:   1351300
+                                                  (0000000000149E84h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3663,21 +3700,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #100:
+Central directory entry #101:
 ---------------------------
 
   templates/examples/auth_form.html
 
-  offset of local header from start of archive:   1345143
-                                                  (0000000000148677h) bytes
+  offset of local header from start of archive:   1351538
+                                                  (0000000000149F72h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3700,21 +3737,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #101:
+Central directory entry #102:
 ---------------------------
 
   templates/examples/custom_form.html
 
-  offset of local header from start of archive:   1345395
-                                                  (0000000000148773h) bytes
+  offset of local header from start of archive:   1351790
+                                                  (000000000014A06Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3737,21 +3774,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #102:
+Central directory entry #103:
 ---------------------------
 
   templates/examples/form.html
 
-  offset of local header from start of archive:   1345844
-                                                  (0000000000148934h) bytes
+  offset of local header from start of archive:   1352239
+                                                  (000000000014A22Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3774,21 +3811,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #103:
+Central directory entry #104:
 ---------------------------
 
   templates/examples/component_loader.html
 
-  offset of local header from start of archive:   1346120
-                                                  (0000000000148A48h) bytes
+  offset of local header from start of archive:   1352515
+                                                  (000000000014A343h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3811,21 +3848,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #104:
+Central directory entry #105:
 ---------------------------
 
   templates/examples/auth_forms.html
 
-  offset of local header from start of archive:   1346330
-                                                  (0000000000148B1Ah) bytes
+  offset of local header from start of archive:   1352725
+                                                  (000000000014A415h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3848,21 +3885,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #105:
+Central directory entry #106:
 ---------------------------
 
   templates/examples/html_grid.html
 
-  offset of local header from start of archive:   1346648
-                                                  (0000000000148C58h) bytes
+  offset of local header from start of archive:   1353043
+                                                  (000000000014A553h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3885,21 +3922,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #106:
+Central directory entry #107:
 ---------------------------
 
   templates/examples/generic.html
 
-  offset of local header from start of archive:   1346860
-                                                  (0000000000148D2Ch) bytes
+  offset of local header from start of archive:   1353255
+                                                  (000000000014A627h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3922,21 +3959,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #107:
+Central directory entry #108:
 ---------------------------
 
   templates/examples/page_with_template.html
 
-  offset of local header from start of archive:   1347120
-                                                  (0000000000148E30h) bytes
+  offset of local header from start of archive:   1353515
+                                                  (000000000014A72Bh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3959,21 +3996,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #108:
+Central directory entry #109:
 ---------------------------
 
   templates/examples/auth_custom_login.html
 
-  offset of local header from start of archive:   1347299
-                                                  (0000000000148EE3h) bytes
+  offset of local header from start of archive:   1353694
+                                                  (000000000014A7DEh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -3996,21 +4033,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #109:
+Central directory entry #110:
 ---------------------------
 
   templates/examples/rest_info.html
 
-  offset of local header from start of archive:   1347673
-                                                  (0000000000149059h) bytes
+  offset of local header from start of archive:   1354068
+                                                  (000000000014A954h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4033,21 +4070,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #110:
+Central directory entry #111:
 ---------------------------
 
   templates/examples/hcaptcha_form.html
 
-  offset of local header from start of archive:   1348087
-                                                  (00000000001491F7h) bytes
+  offset of local header from start of archive:   1354482
+                                                  (000000000014AAF2h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4070,21 +4107,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #111:
+Central directory entry #112:
 ---------------------------
 
   templates/examples/ajax_grid.html
 
-  offset of local header from start of archive:   1348333
-                                                  (00000000001492EDh) bytes
+  offset of local header from start of archive:   1354728
+                                                  (000000000014ABE8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4107,21 +4144,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #112:
+Central directory entry #113:
 ---------------------------
 
   templates/socketio/socketio_index.html
 
-  offset of local header from start of archive:   1348492
-                                                  (000000000014938Ch) bytes
+  offset of local header from start of archive:   1354887
+                                                  (000000000014AC87h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4144,21 +4181,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #113:
+Central directory entry #114:
 ---------------------------
 
   templates/vue/star_rater_vue.html
 
-  offset of local header from start of archive:   1349356
-                                                  (00000000001496ECh) bytes
+  offset of local header from start of archive:   1355751
+                                                  (000000000014AFE7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4181,21 +4218,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #114:
+Central directory entry #115:
 ---------------------------
 
   templates/vue/starrating.html
 
-  offset of local header from start of archive:   1349718
-                                                  (0000000000149856h) bytes
+  offset of local header from start of archive:   1356113
+                                                  (000000000014B151h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4218,21 +4255,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #115:
+Central directory entry #116:
 ---------------------------
 
   templates/vue/edit_form.html
 
-  offset of local header from start of archive:   1350069
-                                                  (00000000001499B5h) bytes
+  offset of local header from start of archive:   1356464
+                                                  (000000000014B2B0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4255,21 +4292,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #116:
+Central directory entry #117:
 ---------------------------
 
   templates/vue/file_uploader.html
 
-  offset of local header from start of archive:   1350415
-                                                  (0000000000149B0Fh) bytes
+  offset of local header from start of archive:   1356810
+                                                  (000000000014B40Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4292,21 +4329,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #117:
+Central directory entry #118:
 ---------------------------
 
   templates/vue/star_rater_vue_bulma.html
 
-  offset of local header from start of archive:   1350724
-                                                  (0000000000149C44h) bytes
+  offset of local header from start of archive:   1357119
+                                                  (000000000014B53Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4329,21 +4366,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #118:
+Central directory entry #119:
 ---------------------------
 
   templates/vue/insert_form.html
 
-  offset of local header from start of archive:   1351117
-                                                  (0000000000149DCDh) bytes
+  offset of local header from start of archive:   1357512
+                                                  (000000000014B6C8h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4366,21 +4403,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #119:
+Central directory entry #120:
 ---------------------------
 
   templates/vue/vue_grid_and_forms.html
 
-  offset of local header from start of archive:   1351466
-                                                  (0000000000149F2Ah) bytes
+  offset of local header from start of archive:   1357861
+                                                  (000000000014B825h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4403,21 +4440,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #120:
+Central directory entry #121:
 ---------------------------
 
   templates/vue/vuegrid_bulma.html
 
-  offset of local header from start of archive:   1351899
-                                                  (000000000014A0DBh) bytes
+  offset of local header from start of archive:   1358294
+                                                  (000000000014B9D6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4440,21 +4477,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #121:
+Central directory entry #122:
 ---------------------------
 
   templates/vue/view_form.html
 
-  offset of local header from start of archive:   1352231
-                                                  (000000000014A227h) bytes
+  offset of local header from start of archive:   1358626
+                                                  (000000000014BB22h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4477,21 +4514,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #122:
+Central directory entry #123:
 ---------------------------
 
   templates/vue/vuegrid.html
 
-  offset of local header from start of archive:   1352575
-                                                  (000000000014A37Fh) bytes
+  offset of local header from start of archive:   1358970
+                                                  (000000000014BC7Ah) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4514,21 +4551,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #123:
+Central directory entry #124:
 ---------------------------
 
   templates/layout.html
 
-  offset of local header from start of archive:   1352892
-                                                  (000000000014A4BCh) bytes
+  offset of local header from start of archive:   1359287
+                                                  (000000000014BDB7h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4551,21 +4588,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #124:
+Central directory entry #125:
 ---------------------------
 
   templates/auth.html
 
-  offset of local header from start of archive:   1354146
-                                                  (000000000014A9A2h) bytes
+  offset of local header from start of archive:   1360541
+                                                  (000000000014C29Dh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4588,21 +4625,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #125:
+Central directory entry #126:
 ---------------------------
 
   templates/layout_bulma.html
 
-  offset of local header from start of archive:   1354398
-                                                  (000000000014AA9Eh) bytes
+  offset of local header from start of archive:   1360793
+                                                  (000000000014C399h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4625,21 +4662,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #126:
+Central directory entry #127:
 ---------------------------
 
   templates/show.html
 
-  offset of local header from start of archive:   1355425
-                                                  (000000000014AEA1h) bytes
+  offset of local header from start of archive:   1361820
+                                                  (000000000014C79Ch) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4662,21 +4699,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #127:
+Central directory entry #128:
 ---------------------------
 
   translations/it.json
 
-  offset of local header from start of archive:   1355768
-                                                  (000000000014AFF8h) bytes
+  offset of local header from start of archive:   1362163
+                                                  (000000000014C8F3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4699,21 +4736,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #128:
+Central directory entry #129:
 ---------------------------
 
   translations/en.json
 
-  offset of local header from start of archive:   1355982
-                                                  (000000000014B0CEh) bytes
+  offset of local header from start of archive:   1362377
+                                                  (000000000014C9C9h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4736,21 +4773,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #129:
+Central directory entry #130:
 ---------------------------
 
   vue_components_examples/vue_grid_and_forms.py
 
-  offset of local header from start of archive:   1356182
-                                                  (000000000014B196h) bytes
+  offset of local header from start of archive:   1362577
+                                                  (000000000014CA91h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4773,21 +4810,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #130:
+Central directory entry #131:
 ---------------------------
 
   vue_components_examples/components/fileupload.py
 
-  offset of local header from start of archive:   1357231
-                                                  (000000000014B5AFh) bytes
+  offset of local header from start of archive:   1363626
+                                                  (000000000014CEAAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4810,21 +4847,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #131:
+Central directory entry #132:
 ---------------------------
 
   vue_components_examples/components/vueform.py
 
-  offset of local header from start of archive:   1358026
-                                                  (000000000014B8CAh) bytes
+  offset of local header from start of archive:   1364421
+                                                  (000000000014D1C5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4847,21 +4884,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #132:
+Central directory entry #133:
 ---------------------------
 
   vue_components_examples/components/grid.py
 
-  offset of local header from start of archive:   1361334
-                                                  (000000000014C5B6h) bytes
+  offset of local header from start of archive:   1367729
+                                                  (000000000014DEB1h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4884,21 +4921,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #133:
+Central directory entry #134:
 ---------------------------
 
   vue_components_examples/components/README.md
 
-  offset of local header from start of archive:   1363991
-                                                  (000000000014D017h) bytes
+  offset of local header from start of archive:   1370386
+                                                  (000000000014E912h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4921,21 +4958,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #134:
+Central directory entry #135:
 ---------------------------
 
   vue_components_examples/components/starrater.py
 
-  offset of local header from start of archive:   1366899
-                                                  (000000000014DB73h) bytes
+  offset of local header from start of archive:   1373294
+                                                  (000000000014F46Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4958,21 +4995,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #135:
+Central directory entry #136:
 ---------------------------
 
   vue_components_examples/vue_file_uploader.py
 
-  offset of local header from start of archive:   1367844
-                                                  (000000000014DF24h) bytes
+  offset of local header from start of archive:   1374239
+                                                  (000000000014F81Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -4995,21 +5032,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #136:
+Central directory entry #137:
 ---------------------------
 
   vue_components_examples/vue_star_rater.py
 
-  offset of local header from start of archive:   1368121
-                                                  (000000000014E039h) bytes
+  offset of local header from start of archive:   1374516
+                                                  (000000000014F934h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5032,21 +5069,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #137:
+Central directory entry #138:
 ---------------------------
 
   vue_components_examples/common.py
 
-  offset of local header from start of archive:   1368751
-                                                  (000000000014E2AFh) bytes
+  offset of local header from start of archive:   1375146
+                                                  (000000000014FBAAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -5068,21 +5105,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #138:
+Central directory entry #139:
 ---------------------------
 
   vue_components_examples/vue_edit_form.py
 
-  offset of local header from start of archive:   1368874
-                                                  (000000000014E32Ah) bytes
+  offset of local header from start of archive:   1375269
+                                                  (000000000014FC25h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5105,21 +5142,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #139:
+Central directory entry #140:
 ---------------------------
 
   vue_components_examples/vue_insert_form.py
 
-  offset of local header from start of archive:   1369462
-                                                  (000000000014E576h) bytes
+  offset of local header from start of archive:   1375857
+                                                  (000000000014FE71h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5142,21 +5179,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #140:
+Central directory entry #141:
 ---------------------------
 
   vue_components_examples/vue_view_form.py
 
-  offset of local header from start of archive:   1369949
-                                                  (000000000014E75Dh) bytes
+  offset of local header from start of archive:   1376344
+                                                  (0000000000150058h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5179,21 +5216,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #141:
+Central directory entry #142:
 ---------------------------
 
   vue_components_examples/settings.py
 
-  offset of local header from start of archive:   1370570
-                                                  (000000000014E9CAh) bytes
+  offset of local header from start of archive:   1376965
+                                                  (00000000001502C5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
@@ -5215,21 +5252,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #142:
+Central directory entry #143:
 ---------------------------
 
   vue_components_examples/models.py
 
-  offset of local header from start of archive:   1370697
-                                                  (000000000014EA49h) bytes
+  offset of local header from start of archive:   1377092
+                                                  (0000000000150344h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -5252,21 +5289,21 @@
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access times.
   - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
     01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
-Central directory entry #143:
+Central directory entry #144:
 ---------------------------
 
   vue_components_examples/vue_grid.py
 
-  offset of local header from start of archive:   1371368
-                                                  (000000000014ECE8h) bytes
+  offset of local header from start of archive:   1377763
+                                                  (00000000001505E3h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
```

#### zipnote {}

```diff
@@ -207,14 +207,17 @@
 
 Filename: static/js/prism.js
 Comment: 
 
 Filename: static/js/vue.js
 Comment: 
 
+Filename: static/favicon.ico
+Comment: 
+
 Filename: static/components-bulma/grid/grid.js
 Comment: 
 
 Filename: static/components-bulma/grid/grid.html
 Comment: 
 
 Filename: static/components-bulma/grid/luxon.js
```

#### static/components/mtable.js

##### js-beautify {}

```diff
@@ -4,41 +4,43 @@
         props: ['url', 'filter', 'order', 'editable', 'create', 'deletable', 'render'],
         data: null,
         methods: {}
     };
 
     mtable.data = function() {
         var data = {
-            mtUrl: this.url,
+            url: this.url,
             busy: false,
-            mtFilter: this.filter || '',
-            mtOrder: this.order || '',
+            filter: this.filter || '',
+            order: this.order || '',
             errors: {},
             item: null,
             message: '',
+            reference_options: {},
             table: {
                 model: [],
                 items: [],
                 count: 0
-            }
+            },
+            string_values: {}
         };
         mtable.methods.load.call(data);
         return data;
     };
 
     mtable.methods.toggle = function(obj, key) {
         obj[key] = !obj[key];
     };
     mtable.methods.load = function() {
         let self = this;
         let length = this.table.items.length;
-        let url = this.mtUrl + '?@limit=20';
+        let url = this.url + '?@limit=20';
         if (length) url += '&@offset=' + length;
         else url += '&@model=true';
-        let filters = self.mtFilter.split(' and ').filter((f) => {
+        let filters = self.filter.split(' and ').filter((f) => {
             return f.trim() != ''
         });
         filters = filters.filter((f) => {
             return f.trim();
         }).map((f) => {
             let parts = (f
                 .replace(/ equals? /, '==')
@@ -58,61 +60,114 @@
                 parts[0] = parts[0].substr(4);
             }
             return ((negate ? 'not.' : '') +
                 parts[0].replace(/ /ig, '') +
                 '=' + parts[parts.length - 1].replace(/^ /, ''));
         });
         if (filters.length) url += '&' + filters.join('&');
-        if (self.mtOrder) url += '&@order=' + self.mtOrder;
+        if (self.order) url += '&@order=' + self.order;
         self.busy = true;
         axios.get(url).then(function(res) {
             self.busy = false;
             if (!length) self.table = res.data;
             else self.table.items = self.table.items.concat(res.data.items);
         });
     };
 
     mtable.methods.reorder = function(field) {
-        if (this.mtOrder == '~' + field.name) this.mtOrder = null;
-        else if (this.mtOrder == field.name) this.mtOrder = '~' + field.name;
-        else this.mtOrder = field.name;
+        if (this.order == '~' + field.name) this.order = null;
+        else if (this.order == field.name) this.order = '~' + field.name;
+        else this.order = field.name;
         this.table.items = [];
         this.load();
     };
 
     mtable.methods.clear = function() {
         this.errors = {};
         this.item = null;
         this.message = '';
     }
 
     mtable.methods.open_create = function() {
         this.item = {};
-        for (var field in this.model) this.item[field.name] = field.default || '';
+        this.prepare_fields(this.item);
     };
 
     mtable.methods.open_edit = function(item) {
         this.item = {};
         this.item = item;
+        this.prepare_fields(this.item);
     };
 
+    mtable.methods.prepare_fields = function(item) {
+        let self = this;
+        for (var field of this.table.model) {
+            if (field.type == "list:string" || field.type == "list:integer" || field.type.substr(0, 14) == "list:reference") {
+                self.string_values[field.name] = JSON.stringify(item[field.name]);
+            } else if (field.type == "datetime") {
+                output = field.default != null ? field.default : '';
+                output = output.split('.')[0];
+                Vue.set(this.item, field.name, output);
+            } else if (field.type == "reference") {
+                if (!(field.references in this.reference_options)) {
+                    Vue.set(this.reference_options, field.references, []);
+                    let reference_table_url = self.url.split('/');
+                    reference_table_url.pop()
+                    reference_table_url.push(field.references)
+                    reference_table_url = reference_table_url.join('/') + '?@options_list=true';
+                    axios.get(reference_table_url).then(function(res) {
+                        let url_components = res.config.url.split('?')[0].split('/');
+                        self.reference_options[url_components[url_components.length - 1]] = res.data.items;
+                    });
+
+                }
+            }
+        }
+        this.$nextTick(function() {
+            Q("input[type=text].type-list-string,input[type=text].type-list-integer,input[type=text].type-list-reference").forEach(
+                function(elem) {
+                    Q.tags_input(elem);
+                });
+        });
+    };
+
+    mtable.methods.parse_and_validate_json = function(event) {
+        try {
+            event.target.style.borderColor = "";
+            return JSON.parse(event.target.value);
+        } catch (error) {
+            event.target.style.borderColor = "#ff0000";
+        }
+    }
+
     mtable.methods.trash = function(item) {
         if (window.confirm("Really delete record?")) {
-            let url = this.mtUrl + '/' + item.id;
+            let url = this.url + '/' + item.id;
             this.table.items = this.table.items.filter((i) => {
                 return i.id != item.id;
             });
             axios.delete(url);
             if (item == this.item) this.item = null;
         }
     };
 
     mtable.methods.save = function(item) {
-        let url = this.mtUrl;
+        let url = this.url;
         self.busy = true;
+        for (var field of this.table.model) {
+            var is_list_integer = field.type == "list:integer" || field.type.substr(0, 14) == "list:reference";
+            if (field.type == "list:string" || is_list_integer) {
+                try {
+                    item[field.name] = JSON.parse(this.string_values[field.name]);
+                } catch (err) {
+                    alert("Invalid field value: " + field.name);
+                    break;
+                }
+            }
+        }
         if (item.id) {
             url += '/' + item.id;
             axios.put(url, item).then(mtable.handle_response('put', this),
                 mtable.handle_response('put', this));
         } else {
             axios.post(url, item).then(mtable.handle_response('post', this),
                 mtable.handle_response('post', this));
@@ -121,27 +176,22 @@
 
     mtable.handle_response = function(method, data) {
         self.busy = false;
         return function(res) {
             if (res.response) res = res.response; // deal with error weirdness
             if (method == 'post') {
                 data.table.items = [];
-                console.log(data);
                 mtable.methods.load.call(data);
             }
-            console.log('a');
-            console.log(res);
             if (res.data.status == 'success') {
                 data.clear();
             } else {
-                console.log('b')
                 data.errors = res.data.errors;
                 data.message = res.data.message;
             }
-            console.log('c');
         };
     };
 
     mtable.methods.close = function() {
         this.clear();
     };
```

#### static/components/mtable.html

```diff
@@ -1,12 +1,12 @@
 <div>
   <table>
     <tr>
       <td class="control">              
-        <input class="input" v-model="mtFilter" type="text" placeholder="filter (example id > 1)" style="width: 100%" v-on:keyup.enter="search()"/>
+        <input v-model="filter" type="text" placeholder="filter (example id > 1)" style="width: 100%" v-on:keyup.enter="search()"/>
       </td>
       <td style="white-space: nowrap; width:10%; padding-left:5px">
         <button v-on:click="search()" class="button">Search</button>
         <button v-if="create" v-on:click="open_create()" class="button">Create</button>
       </td>
     </tr>    
     <tr>
@@ -20,29 +20,41 @@
     <i class="fa fa-3x fa-spin fa-spinner"></i>
   </div>
   <div v-else-if="item!=null">
     <table class="table">
       <tr v-for="field in table.model" v-if="field.type!='id' || item.id">
         <th>{{field.label}}</th>
         <td class="control">
-          <input class="input" v-if="field.type=='id'" type="text" readonly v-model="item[field.name]">
-          <input class="input" v-else-if="field.type=='string'" type="text" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-if="field.type=='id'" type="text" readonly v-model="item[field.name]">
+          <input v-else-if="field.type=='string'" type="text" v-model="item[field.name]" v-bind:readonly="!editable">
           <span v-else-if="field.type=='boolean'" v-on:click="toggle(item, field.name)" v-bind:readonly="!editable">
             <span v-if="item[field.name]===true"><i class="fa fa-check-square"></i> True</span>
             <span v-else-if="item[field.name]===false"><i class="fa fa-square"></i> False</span>
             <span v-else><i class="fa fa-square"></i> None</span>
           </span>
-          <input class="input" v-else-if="field.type=='integer'" type="number" step="1" v-model="item[field.name]" v-bind:readonly="!editable">
-          <input class="input" v-else-if="field.type=='float'" type="number" v-model="item[field.name]" v-bind:readonly="!editable">
-          <input class="input" v-else-if="field.type=='date'" type="date" v-model="item[field.name]" v-bind:readonly="!editable">
-          <input class="input" v-else-if="field.type=='time'" type="time" v-model="item[field.name]" v-bind:readonly="!editable">
-          <input class="input" v-else-if="field.type=='datetime'" type="datetime-local" v-model="item[field.name]" v-bind:readonly="!editable">
-          <input class="input" v-else-if="field.type=='password'" type="password" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='integer'" type="number" step="1" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='float'" type="number" step="0.00000000000001" v-model="item[field.name]"  v-bind:readonly="!editable">
+          <input v-else-if="field.type=='double'" type="number" step="0.00000000000001" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='decimal'" type="number" step="0.1" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='date'" type="date" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='time'" type="time" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='datetime'" type="datetime-local" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='password'" type="password" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input class="type-list-integer" v-else-if="field.type=='list:integer'" type="text" v-model="string_values[field.name]" v-bind:readonly="!editable">
+          <input class="type-list-reference" v-else-if="field.type.substr(0,14)=='list:reference'" type="text" v-model="string_values[field.name]" v-bind:readonly="!editable">
+          <input class="type-list-string" v-else-if="field.type=='list:string'" type="text" v-model="string_values[field.name]" v-bind:readonly="!editable">
           <input v-else-if="field.type=='upload'" type="text" v-model="item[field.name]" v-bind:readonly="!editable">
           <textarea class="textarea" v-else-if="field.type=='text'" v-model="item[field.name]" v-bind:readonly="!editable"></textarea>
+          <select v-else-if="field.type=='reference'" v-model="item[field.name]" v-bind:readonly="!editable">
+            <option disabled value="">Select...</option>
+            <option v-for="option in reference_options[field.references]" :key="option.value" v-bind:value="option.value">
+              {{ option.text }}
+            </option>
+          </select>
+          <textarea class="textarea" v-else-if="field.type=='json'" @input="function(event){item[field.name] = parse_and_validate_json(event)}" v-bind:readonly="!editable">{{item[field.name]}}</textarea>
           <div class="error" v-if="editable && field.name in errors">{{errors[field.name]}}</div>
         </td>
       </tr>
       <tr v-if="item.id">
         <th>
           Referenced By
         </th>
@@ -61,40 +73,45 @@
   </div>
   <div v-else-if="table.items.length>0">
     <table class="table">
       <thead>
         <tr>
           <th v-for="field in table.model" v-on:click="reorder(field)">
             {{field.label}}
-            <i v-if="mtOrder==field.name" class="fa fa-arrow-up"></i>
-            <i v-if="mtOrder=='~'+field.name" class="fa fa-arrow-down"></i>
+            <i v-if="order==field.name" class="fa fa-arrow-up"></i>
+            <i v-if="order=='~'+field.name" class="fa fa-arrow-down"></i>
           </th>
         </tr>
       </thead>
       <tbody>
         <tr v-for="item in table.items">
           <td v-for="field in table.model">
             <a v-if="field.type=='id'" class="field-id" v-on:click="open_edit(item)"> 
               [{{item[field.name]}}]
             </a>
             <span v-else-if="field.type=='string'" class="field-string">{{item[field.name]}}</span>
+            <span v-else-if="field.type=='json'" class="field-string">(json)</span>
             <span v-else-if="field.type=='integer'" class="field-integer">{{item[field.name]}}</span>
+            <span v-else-if="field.type=='double'" class="field-float">{{item[field.name]}}</span>
             <span v-else-if="field.type=='float'" class="field-float">{{item[field.name]}}</span>
+            <span v-else-if="field.type=='decimal'" class="field-float">{{item[field.name]}}</span>
             <span v-else-if="field.type=='date'" class="field-date">{{item[field.name]}}</span>
             <span v-else-if="field.type=='time'" class="field-time">{{item[field.name]}}</span>
+            <span v-else-if="field.type=='list:integer'" class="field-string">{{JSON.stringify(item[field.name])}}</span>
+            <span v-else-if="field.type=='list:string'" class="field-string">{{JSON.stringify(item[field.name])}}</span>
             <span v-else-if="field.type=='datetime'" class="field-datetime">{{(item[field.name]||'').replace('T','@').substr(0,16)}}</span>
             <span v-else-if="field.type=='password'" class="field-password">{{item[field.name]}}</span>
             <span v-else-if="field.type=='boolean'" class="field-boolean">
               <i class="fa fa-check-square" v-if="item[field.name]===true"></i>
               <i class="fa fa-square" v-if="item[field.name]===false"></i>
             </span>
             <span v-else-if="field.type=='text'" class="field-text"><i class="fa fa-expand"></i></span>
             <a v-else-if="field.type=='reference'" class="field-reference"
                v-on:click="go_ref_by(field.references,item[field.name])">[{{item[field.name]}}]</a>
             <span v-else-if="field.type=='upload'" class="field-upload"><i class="fa fa-download"></i></span>
           </td>
         </tr>
       </tbody>
-    </table>
+    </table>          
     <button class="button" v-if="table.count > table.items.length" v-on:click="load()">Load More</button>
   </div>
 </div>
```

##### html2text {}

```diff
@@ -1,12 +1,19 @@
 enter="search()"/> Search Create
 {{message}}        (no items found) (one item found) ({{table.count}} items
                                                      found)
-{{field.label}} {{errors[field.name]}}
+                key="option.value" v-bind:value="option.value"> {{ option.text
+                }}
+
+{{field.label}} input="function(event){item[field.name] =
+                parse_and_validate_json(event)}" v-bind:readonly="!editable">{
+                {item[field.name]}}
+                {{errors[field.name]}}
 Referenced By   {{name}}
 Save Delete Close
 {{field.label}}
-[{{item[field.name]}}] {{item[field.name]}} {{item[field.name]}} {{item
-[field.name]}} {{item[field.name]}} {{item[field.name]}} {{(item
-[field.name]||'').replace('T','@').substr(0,16)}} {{item[field.name]}}      [{
-{item[field.name]}}]
+[{{item[field.name]}}] {{item[field.name]}} (json) {{item[field.name]}} {{item
+[field.name]}} {{item[field.name]}} {{item[field.name]}} {{item[field.name]}} {
+{item[field.name]}} {{JSON.stringify(item[field.name])}} {{JSON.stringify(item
+[field.name])}} {{(item[field.name]||'').replace('T','@').substr(0,16)}} {{item
+[field.name]}}      [{{item[field.name]}}]
 Load More
```

#### static/js/utils.js

##### js-beautify {}

```diff
@@ -197,45 +197,51 @@
     var keys = Q.eval(elem.value || '[]');
     keys.map(function(x) {
         if (tags.indexOf(x) < 0) tags.push(x);
     });
     var fill = function(elem, repl) {
         repl.innerHTML = '';
         tags.forEach(function(x) {
-            console.log(x);
             var item = document.createElement('li');
             item.innerHTML = options.labels[x] || x;
             item.dataset.value = x;
             item.dataset.selected = keys.indexOf(x) >= 0;
             repl.appendChild(item);
             item.onclick = function(evt) {
                 if (item.dataset.selected == 'false') keys.push(x);
                 else keys = keys.filter(function(y) {
                     return x != y;
                 });
                 item.dataset.selected = keys.indexOf(x) >= 0;
                 elem.value = JSON.stringify(keys);
+                elem.dispatchEvent(new Event('input', {
+                    bubbles: true
+                }));
             };
         });
     };
     if (options.freetext) {
         var inp = document.createElement('input');
         elem.parentNode.insertBefore(inp, elem);
+        inp.type = "text";
         inp.classList = elem.classList;
         inp.placeholder = options.placeholder;
         inp.setAttribute('list', options.autocomplete_list);
         inp.onchange = function(evt) {
             inp.value.split(',').map(function(x) {
                 x = options.transform(x.trim());
                 if (options.regex && !x.match(options.regex)) return;
                 if (x && tags.indexOf(x) < 0) tags.push(x);
                 if (x && keys.indexOf(x) < 0) keys.push(x);
             });
             inp.value = '';
             elem.value = JSON.stringify(keys);
+            elem.dispatchEvent(new Event('input', {
+                bubbles: true
+            }));
             fill(elem, repl);
         };
     }
     fill(elem, repl);
 };
 
 // Password strenght calculator
@@ -292,15 +298,14 @@
     method = (method || 'GET').toLowerCase();
     /* if target is not there, fill it with something that there isn't in the page*/
     if (target === void 0 || target === '') target = 'none';
     var onsuccess = function(res) {
         if (res.redirected) window.location = res.url;
         Q('#' + target)[0].innerHTML = res.data;
         Q.trap_form(url, target);
-        console.log(res.headers);
         var flash = res.headers.get('component-flash');
         if (flash) Q.flash(JSON.parse(flash));
     };
     var onerror = function(res) {
         alert('ajax error');
     };
     Q.ajax(method, url, form_data).then(onsuccess).catch(onerror);
@@ -334,15 +339,14 @@
     if (elem) {
         elem.addEventListener('flash', make_handler(elem), false);
         Q.flash = function(detail) {
             elem.dispatchEvent(new CustomEvent('flash', {
                 detail: detail
             }));
         };
-        console.log(elem.dataset.alert);
         if (elem.dataset.alert) Q.flash(Q.eval(elem.dataset.alert));
     }
 };
 
 Q.handle_components();
 Q.handle_flash();
 Q('input[type=text].type-list-string').forEach(function(elem) {
```

#### static/components-bulma/mtable.js

##### js-beautify {}

```diff
@@ -4,41 +4,43 @@
         props: ['url', 'filter', 'order', 'editable', 'create', 'deletable', 'render'],
         data: null,
         methods: {}
     };
 
     mtable.data = function() {
         var data = {
-            mtUrl: this.url,
+            url: this.url,
             busy: false,
-            mtFilter: this.filter || '',
-            mtOrder: this.order || '',
+            filter: this.filter || '',
+            order: this.order || '',
             errors: {},
             item: null,
             message: '',
+            reference_options: {},
             table: {
                 model: [],
                 items: [],
                 count: 0
-            }
+            },
+            string_values: {}
         };
         mtable.methods.load.call(data);
         return data;
     };
 
     mtable.methods.toggle = function(obj, key) {
         obj[key] = !obj[key];
     };
     mtable.methods.load = function() {
         let self = this;
         let length = this.table.items.length;
-        let url = this.mtUrl + '?@limit=20';
+        let url = this.url + '?@limit=20';
         if (length) url += '&@offset=' + length;
         else url += '&@model=true';
-        let filters = self.mtFilter.split(' and ').filter((f) => {
+        let filters = self.filter.split(' and ').filter((f) => {
             return f.trim() != ''
         });
         filters = filters.filter((f) => {
             return f.trim();
         }).map((f) => {
             let parts = (f
                 .replace(/ equals? /, '==')
@@ -58,61 +60,114 @@
                 parts[0] = parts[0].substr(4);
             }
             return ((negate ? 'not.' : '') +
                 parts[0].replace(/ /ig, '') +
                 '=' + parts[parts.length - 1].replace(/^ /, ''));
         });
         if (filters.length) url += '&' + filters.join('&');
-        if (self.mtOrder) url += '&@order=' + self.mtOrder;
+        if (self.order) url += '&@order=' + self.order;
         self.busy = true;
         axios.get(url).then(function(res) {
             self.busy = false;
             if (!length) self.table = res.data;
             else self.table.items = self.table.items.concat(res.data.items);
         });
     };
 
     mtable.methods.reorder = function(field) {
-        if (this.mtOrder == '~' + field.name) this.mtOrder = null;
-        else if (this.mtOrder == field.name) this.mtOrder = '~' + field.name;
-        else this.mtOrder = field.name;
+        if (this.order == '~' + field.name) this.order = null;
+        else if (this.order == field.name) this.order = '~' + field.name;
+        else this.order = field.name;
         this.table.items = [];
         this.load();
     };
 
     mtable.methods.clear = function() {
         this.errors = {};
         this.item = null;
         this.message = '';
     }
 
     mtable.methods.open_create = function() {
         this.item = {};
-        for (var field in this.model) this.item[field.name] = field.default || '';
+        this.prepare_fields(this.item);
     };
 
     mtable.methods.open_edit = function(item) {
         this.item = {};
         this.item = item;
+        this.prepare_fields(this.item);
     };
 
+    mtable.methods.prepare_fields = function(item) {
+        let self = this;
+        for (var field of this.table.model) {
+            if (field.type == "list:string" || field.type == "list:integer" || field.type.substr(0, 14) == "list:reference") {
+                self.string_values[field.name] = JSON.stringify(item[field.name]);
+            } else if (field.type == "datetime") {
+                output = field.default != null ? field.default : '';
+                output = output.split('.')[0];
+                Vue.set(this.item, field.name, output);
+            } else if (field.type == "reference") {
+                if (!(field.references in this.reference_options)) {
+                    Vue.set(this.reference_options, field.references, []);
+                    let reference_table_url = self.url.split('/');
+                    reference_table_url.pop()
+                    reference_table_url.push(field.references)
+                    reference_table_url = reference_table_url.join('/') + '?@options_list=true';
+                    axios.get(reference_table_url).then(function(res) {
+                        let url_components = res.config.url.split('?')[0].split('/');
+                        self.reference_options[url_components[url_components.length - 1]] = res.data.items;
+                    });
+
+                }
+            }
+        }
+        this.$nextTick(function() {
+            Q("input[type=text].type-list-string,input[type=text].type-list-integer,input[type=text].type-list-reference").forEach(
+                function(elem) {
+                    Q.tags_input(elem);
+                });
+        });
+    };
+
+    mtable.methods.parse_and_validate_json = function(event) {
+        try {
+            event.target.style.borderColor = "";
+            return JSON.parse(event.target.value);
+        } catch (error) {
+            event.target.style.borderColor = "#ff0000";
+        }
+    }
+
     mtable.methods.trash = function(item) {
         if (window.confirm("Really delete record?")) {
-            let url = this.mtUrl + '/' + item.id;
+            let url = this.url + '/' + item.id;
             this.table.items = this.table.items.filter((i) => {
                 return i.id != item.id;
             });
             axios.delete(url);
             if (item == this.item) this.item = null;
         }
     };
 
     mtable.methods.save = function(item) {
-        let url = this.mtUrl;
+        let url = this.url;
         self.busy = true;
+        for (var field of this.table.model) {
+            var is_list_integer = field.type == "list:integer" || field.type.substr(0, 14) == "list:reference";
+            if (field.type == "list:string" || is_list_integer) {
+                try {
+                    item[field.name] = JSON.parse(this.string_values[field.name]);
+                } catch (err) {
+                    alert("Invalid field value: " + field.name);
+                    break;
+                }
+            }
+        }
         if (item.id) {
             url += '/' + item.id;
             axios.put(url, item).then(mtable.handle_response('put', this),
                 mtable.handle_response('put', this));
         } else {
             axios.post(url, item).then(mtable.handle_response('post', this),
                 mtable.handle_response('post', this));
@@ -121,27 +176,22 @@
 
     mtable.handle_response = function(method, data) {
         self.busy = false;
         return function(res) {
             if (res.response) res = res.response; // deal with error weirdness
             if (method == 'post') {
                 data.table.items = [];
-                console.log(data);
                 mtable.methods.load.call(data);
             }
-            console.log('a');
-            console.log(res);
             if (res.data.status == 'success') {
                 data.clear();
             } else {
-                console.log('b')
                 data.errors = res.data.errors;
                 data.message = res.data.message;
             }
-            console.log('c');
         };
     };
 
     mtable.methods.close = function() {
         this.clear();
     };
```

#### static/components-bulma/mtable.html

```diff
@@ -1,12 +1,12 @@
 <div>
   <table>
     <tr>
       <td class="control">              
-        <input class="input" v-model="mtFilter" type="text" placeholder="filter (example id > 1)" style="width: 100%" v-on:keyup.enter="search()"/>
+        <input v-model="filter" type="text" placeholder="filter (example id > 1)" style="width: 100%" v-on:keyup.enter="search()"/>
       </td>
       <td style="white-space: nowrap; width:10%; padding-left:5px">
         <button v-on:click="search()" class="button">Search</button>
         <button v-if="create" v-on:click="open_create()" class="button">Create</button>
       </td>
     </tr>    
     <tr>
@@ -20,29 +20,41 @@
     <i class="fa fa-3x fa-spin fa-spinner"></i>
   </div>
   <div v-else-if="item!=null">
     <table class="table">
       <tr v-for="field in table.model" v-if="field.type!='id' || item.id">
         <th>{{field.label}}</th>
         <td class="control">
-          <input class="input" v-if="field.type=='id'" type="text" readonly v-model="item[field.name]">
-          <input class="input" v-else-if="field.type=='string'" type="text" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-if="field.type=='id'" type="text" readonly v-model="item[field.name]">
+          <input v-else-if="field.type=='string'" type="text" v-model="item[field.name]" v-bind:readonly="!editable">
           <span v-else-if="field.type=='boolean'" v-on:click="toggle(item, field.name)" v-bind:readonly="!editable">
             <span v-if="item[field.name]===true"><i class="fa fa-check-square"></i> True</span>
             <span v-else-if="item[field.name]===false"><i class="fa fa-square"></i> False</span>
             <span v-else><i class="fa fa-square"></i> None</span>
           </span>
-          <input class="input" v-else-if="field.type=='integer'" type="number" step="1" v-model="item[field.name]" v-bind:readonly="!editable">
-          <input class="input" v-else-if="field.type=='float'" type="number" v-model="item[field.name]" v-bind:readonly="!editable">
-          <input class="input" v-else-if="field.type=='date'" type="date" v-model="item[field.name]" v-bind:readonly="!editable">
-          <input class="input" v-else-if="field.type=='time'" type="time" v-model="item[field.name]" v-bind:readonly="!editable">
-          <input class="input" v-else-if="field.type=='datetime'" type="datetime-local" v-model="item[field.name]" v-bind:readonly="!editable">
-          <input class="input" v-else-if="field.type=='password'" type="password" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='integer'" type="number" step="1" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='float'" type="number" step="0.00000000000001" v-model="item[field.name]"  v-bind:readonly="!editable">
+          <input v-else-if="field.type=='double'" type="number" step="0.00000000000001" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='decimal'" type="number" step="0.1" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='date'" type="date" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='time'" type="time" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='datetime'" type="datetime-local" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input v-else-if="field.type=='password'" type="password" v-model="item[field.name]" v-bind:readonly="!editable">
+          <input class="type-list-integer" v-else-if="field.type=='list:integer'" type="text" v-model="string_values[field.name]" v-bind:readonly="!editable">
+          <input class="type-list-reference" v-else-if="field.type.substr(0,14)=='list:reference'" type="text" v-model="string_values[field.name]" v-bind:readonly="!editable">
+          <input class="type-list-string" v-else-if="field.type=='list:string'" type="text" v-model="string_values[field.name]" v-bind:readonly="!editable">
           <input v-else-if="field.type=='upload'" type="text" v-model="item[field.name]" v-bind:readonly="!editable">
           <textarea class="textarea" v-else-if="field.type=='text'" v-model="item[field.name]" v-bind:readonly="!editable"></textarea>
+          <select v-else-if="field.type=='reference'" v-model="item[field.name]" v-bind:readonly="!editable">
+            <option disabled value="">Select...</option>
+            <option v-for="option in reference_options[field.references]" :key="option.value" v-bind:value="option.value">
+              {{ option.text }}
+            </option>
+          </select>
+          <textarea class="textarea" v-else-if="field.type=='json'" @input="function(event){item[field.name] = parse_and_validate_json(event)}" v-bind:readonly="!editable">{{item[field.name]}}</textarea>
           <div class="error" v-if="editable && field.name in errors">{{errors[field.name]}}</div>
         </td>
       </tr>
       <tr v-if="item.id">
         <th>
           Referenced By
         </th>
@@ -61,40 +73,45 @@
   </div>
   <div v-else-if="table.items.length>0">
     <table class="table">
       <thead>
         <tr>
           <th v-for="field in table.model" v-on:click="reorder(field)">
             {{field.label}}
-            <i v-if="mtOrder==field.name" class="fa fa-arrow-up"></i>
-            <i v-if="mtOrder=='~'+field.name" class="fa fa-arrow-down"></i>
+            <i v-if="order==field.name" class="fa fa-arrow-up"></i>
+            <i v-if="order=='~'+field.name" class="fa fa-arrow-down"></i>
           </th>
         </tr>
       </thead>
       <tbody>
         <tr v-for="item in table.items">
           <td v-for="field in table.model">
             <a v-if="field.type=='id'" class="field-id" v-on:click="open_edit(item)"> 
               [{{item[field.name]}}]
             </a>
             <span v-else-if="field.type=='string'" class="field-string">{{item[field.name]}}</span>
+            <span v-else-if="field.type=='json'" class="field-string">(json)</span>
             <span v-else-if="field.type=='integer'" class="field-integer">{{item[field.name]}}</span>
+            <span v-else-if="field.type=='double'" class="field-float">{{item[field.name]}}</span>
             <span v-else-if="field.type=='float'" class="field-float">{{item[field.name]}}</span>
+            <span v-else-if="field.type=='decimal'" class="field-float">{{item[field.name]}}</span>
             <span v-else-if="field.type=='date'" class="field-date">{{item[field.name]}}</span>
             <span v-else-if="field.type=='time'" class="field-time">{{item[field.name]}}</span>
+            <span v-else-if="field.type=='list:integer'" class="field-string">{{JSON.stringify(item[field.name])}}</span>
+            <span v-else-if="field.type=='list:string'" class="field-string">{{JSON.stringify(item[field.name])}}</span>
             <span v-else-if="field.type=='datetime'" class="field-datetime">{{(item[field.name]||'').replace('T','@').substr(0,16)}}</span>
             <span v-else-if="field.type=='password'" class="field-password">{{item[field.name]}}</span>
             <span v-else-if="field.type=='boolean'" class="field-boolean">
               <i class="fa fa-check-square" v-if="item[field.name]===true"></i>
               <i class="fa fa-square" v-if="item[field.name]===false"></i>
             </span>
             <span v-else-if="field.type=='text'" class="field-text"><i class="fa fa-expand"></i></span>
             <a v-else-if="field.type=='reference'" class="field-reference"
                v-on:click="go_ref_by(field.references,item[field.name])">[{{item[field.name]}}]</a>
             <span v-else-if="field.type=='upload'" class="field-upload"><i class="fa fa-download"></i></span>
           </td>
         </tr>
       </tbody>
-    </table>
+    </table>          
     <button class="button" v-if="table.count > table.items.length" v-on:click="load()">Load More</button>
   </div>
 </div>
```

##### html2text {}

```diff
@@ -1,12 +1,19 @@
 enter="search()"/> Search Create
 {{message}}        (no items found) (one item found) ({{table.count}} items
                                                      found)
-{{field.label}} {{errors[field.name]}}
+                key="option.value" v-bind:value="option.value"> {{ option.text
+                }}
+
+{{field.label}} input="function(event){item[field.name] =
+                parse_and_validate_json(event)}" v-bind:readonly="!editable">{
+                {item[field.name]}}
+                {{errors[field.name]}}
 Referenced By   {{name}}
 Save Delete Close
 {{field.label}}
-[{{item[field.name]}}] {{item[field.name]}} {{item[field.name]}} {{item
-[field.name]}} {{item[field.name]}} {{item[field.name]}} {{(item
-[field.name]||'').replace('T','@').substr(0,16)}} {{item[field.name]}}      [{
-{item[field.name]}}]
+[{{item[field.name]}}] {{item[field.name]}} (json) {{item[field.name]}} {{item
+[field.name]}} {{item[field.name]}} {{item[field.name]}} {{item[field.name]}} {
+{item[field.name]}} {{JSON.stringify(item[field.name])}} {{JSON.stringify(item
+[field.name])}} {{(item[field.name]||'').replace('T','@').substr(0,16)}} {{item
+[field.name]}}      [{{item[field.name]}}]
 Load More
```

#### templates/index.html

```diff
@@ -150,19 +150,19 @@
     </tr>
     <tr>
       <td>Insertion form in Vue.</td>
       <td><a role="button" href="[[=URL('show/vue_components_examples/vue_insert_form')]]">example</a></td>
     </tr>
     <tr>
       <td>Update form in Vue.</td>
-      <td><a role="button" href="[[=URL('show/vue_components_examples/vue_edit_form')]]">example</a></td>
+      <td><a role="button" href="[[=URL('show/vue_components_examples/vue_edit_form/1')]]">example</a></td>
     </tr>
     <tr>
       <td>View form in Vue.</td>
-      <td><a role="button" href="[[=URL('show/vue_components_examples/vue_view_form')]]">example</a></td>
+      <td><a role="button" href="[[=URL('show/vue_components_examples/vue_view_form/1')]]">example</a></td>
     </tr>
     <tr>
       <td>Grid + Forms in Vue.</td>
       <td><a role="button" href="[[=URL('show/vue_components_examples/vue_grid_and_forms')]]">example</a></td>
     </tr>
     <tr>
       <td>Star rating component in Vue; example of component instantiation from Vue.</td>
```

### Comparing `py4web-1.20230416.2/py4web/core.py` & `py4web-1.20230416.3/py4web/core.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/server_adapters.py` & `py4web-1.20230416.3/py4web/server_adapters.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/auth.py` & `py4web-1.20230416.3/py4web/utils/auth.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/auth_plugins/__init__.py` & `py4web-1.20230416.3/py4web/utils/auth_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/auth_plugins/basic_auth_plugin.py` & `py4web-1.20230416.3/py4web/utils/auth_plugins/basic_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/auth_plugins/cas_plugin.py` & `py4web-1.20230416.3/py4web/utils/auth_plugins/cas_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/auth_plugins/email_auth_plugin.py` & `py4web-1.20230416.3/py4web/utils/auth_plugins/email_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/auth_plugins/ldap_plugin.py` & `py4web-1.20230416.3/py4web/utils/auth_plugins/ldap_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/auth_plugins/newsamlplugin.py` & `py4web-1.20230416.3/py4web/utils/auth_plugins/newsamlplugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/auth_plugins/oauth2discord.py` & `py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2discord.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/auth_plugins/oauth2facebook.py` & `py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2facebook.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/auth_plugins/oauth2github.py` & `py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2github.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/auth_plugins/oauth2google.py` & `py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2google.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/auth_plugins/oauth2server.py` & `py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2server.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/auth_plugins/oauth2wpminiorange.py` & `py4web-1.20230416.3/py4web/utils/auth_plugins/oauth2wpminiorange.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/auth_plugins/pam.py` & `py4web-1.20230416.3/py4web/utils/auth_plugins/pam.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/auth_plugins/saml2_plugin.py` & `py4web-1.20230416.3/py4web/utils/auth_plugins/saml2_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/auth_plugins/x509_auth_plugin.py` & `py4web-1.20230416.3/py4web/utils/auth_plugins/x509_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/cors.py` & `py4web-1.20230416.3/py4web/utils/cors.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/dbstore.py` & `py4web-1.20230416.3/py4web/utils/dbstore.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/downloader.py` & `py4web-1.20230416.3/py4web/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/factories.py` & `py4web-1.20230416.3/py4web/utils/factories.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/form.py` & `py4web-1.20230416.3/py4web/utils/form.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/grid.py` & `py4web-1.20230416.3/py4web/utils/grid.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/jsonrpc.py` & `py4web-1.20230416.3/py4web/utils/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/mailer.py` & `py4web-1.20230416.3/py4web/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/misc.py` & `py4web-1.20230416.3/py4web/utils/misc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/populate.py` & `py4web-1.20230416.3/py4web/utils/populate.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/publisher.py` & `py4web-1.20230416.3/py4web/utils/publisher.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/recaptcha.py` & `py4web-1.20230416.3/py4web/utils/recaptcha.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/scheduler.py` & `py4web-1.20230416.3/py4web/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/scheduler_old.py` & `py4web-1.20230416.3/py4web/utils/scheduler_old.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/security.py` & `py4web-1.20230416.3/py4web/utils/security.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web/utils/url_signer.py` & `py4web-1.20230416.3/py4web/utils/url_signer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/py4web.egg-info/PKG-INFO` & `py4web-1.20230416.3/py4web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: py4web
-Version: 1.20230416.2
+Version: 1.20230416.3
 Summary: Experimental py4web (a better web2py)
 Home-page: https://github.com/web2py/py4web
 Author: Massimo Di Pierro
 Author-email: massimo.dipierro@gmail.com
 Maintainer: Massimo Di Pierro
 Maintainer-email: massimo.dipierro@gmail.com
 License: BSD
```

### Comparing `py4web-1.20230416.2/py4web.egg-info/SOURCES.txt` & `py4web-1.20230416.3/py4web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4web-1.20230416.2/setup.py` & `py4web-1.20230416.3/setup.py`

 * *Files identical despite different names*

