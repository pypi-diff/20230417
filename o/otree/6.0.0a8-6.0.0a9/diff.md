# Comparing `tmp/otree-6.0.0a8.tar.gz` & `tmp/otree-6.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otree-6.0.0a8.tar", last modified: Sat Apr 15 18:48:35 2023, max compression
+gzip compressed data, was "otree-6.0.0a9.tar", last modified: Mon Apr 17 16:33:52 2023, max compression
```

## Comparing `otree-6.0.0a8.tar` & `otree-6.0.0a9.tar`

### file list

```diff
@@ -1,325 +1,325 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.311947 otree-6.0.0a8/
--rw-rw-rw-   0        0        0     1573 2018-11-23 17:31:44.000000 otree-6.0.0a8/LICENSE
--rw-rw-rw-   0        0        0      390 2021-06-06 11:37:30.000000 otree-6.0.0a8/MANIFEST.in
--rw-rw-rw-   0        0        0     1886 2023-04-15 18:48:35.311947 otree-6.0.0a8/PKG-INFO
--rw-rw-rw-   0        0        0     1581 2022-03-03 11:49:02.000000 otree-6.0.0a8/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.075647 otree-6.0.0a8/otree/
--rw-rw-rw-   0        0        0       91 2023-04-15 18:47:37.000000 otree-6.0.0a8/otree/__init__.py
--rw-rw-rw-   0        0        0      634 2023-04-15 17:56:00.000000 otree-6.0.0a8/otree/api.py
--rw-rw-rw-   0        0        0    10444 2023-04-15 18:05:39.000000 otree-6.0.0a8/otree/api.pyi
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.095983 otree-6.0.0a8/otree/app_template/
--rw-rw-rw-   0        0        0        0 2018-11-23 17:31:44.000000 otree-6.0.0a8/otree/app_template/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.104268 otree-6.0.0a8/otree/app_template/__pycache__/
--rw-rw-rw-   0        0        0      127 2017-10-09 12:58:16.000000 otree-6.0.0a8/otree/app_template/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      131 2019-07-18 16:08:18.000000 otree-6.0.0a8/otree/app_template/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0     1013 2017-10-09 12:58:16.000000 otree-6.0.0a8/otree/app_template/__pycache__/models.cpython-36.pyc
--rw-rw-rw-   0        0        0     1017 2019-07-18 16:08:18.000000 otree-6.0.0a8/otree/app_template/__pycache__/models.cpython-37.pyc
--rw-rw-rw-   0        0        0      615 2017-10-09 12:58:16.000000 otree-6.0.0a8/otree/app_template/__pycache__/tests.cpython-36.pyc
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.105322 otree-6.0.0a8/otree/app_template/_builtin/
--rw-rw-rw-   0        0        0      446 2020-10-07 12:35:10.000000 otree-6.0.0a8/otree/app_template/_builtin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.107717 otree-6.0.0a8/otree/app_template/_builtin/__pycache__/
--rw-rw-rw-   0        0        0     1170 2017-10-09 12:58:16.000000 otree-6.0.0a8/otree/app_template/_builtin/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0      871 2019-07-18 16:08:18.000000 otree-6.0.0a8/otree/app_template/_builtin/__pycache__/__init__.cpython-37.pyc
--rw-rw-rw-   0        0        0      464 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/app_template/models.py
--rw-rw-rw-   0        0        0      297 2020-10-07 12:35:10.000000 otree-6.0.0a8/otree/app_template/pages.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.025650 otree-6.0.0a8/otree/app_template/templates/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.109616 otree-6.0.0a8/otree/app_template/templates/app_name/
--rw-rw-rw-   0        0        0      200 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/app_template/templates/app_name/MyPage.html
--rw-rw-rw-   0        0        0      180 2020-12-11 18:14:00.000000 otree-6.0.0a8/otree/app_template/templates/app_name/Results.html
--rw-rw-rw-   0        0        0      200 2020-03-20 01:44:18.000000 otree-6.0.0a8/otree/app_template/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.112511 otree-6.0.0a8/otree/app_template_lite/
--rw-rw-rw-   0        0        0      137 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/app_template_lite/MyPage.html
--rw-rw-rw-   0        0        0      119 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/app_template_lite/Results.html
--rw-rw-rw-   0        0        0      495 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/app_template_lite/__init__.py
--rw-rw-rw-   0        0        0     2888 2022-03-04 18:20:48.000000 otree-6.0.0a8/otree/asgi.py
--rw-rw-rw-   0        0        0        0 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/auth.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.117003 otree-6.0.0a8/otree/bots/
--rw-rw-rw-   0        0        0       75 2020-03-20 01:44:18.000000 otree-6.0.0a8/otree/bots/__init__.py
--rw-rw-rw-   0        0        0    18278 2023-04-15 00:24:13.000000 otree-6.0.0a8/otree/bots/bot.py
--rw-rw-rw-   0        0        0     4815 2022-12-23 08:54:23.000000 otree-6.0.0a8/otree/bots/browser.py
--rw-rw-rw-   0        0        0    11868 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/bots/browser_launcher.py
--rw-rw-rw-   0        0        0     6713 2022-02-01 22:47:42.000000 otree-6.0.0a8/otree/bots/runner.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.122230 otree-6.0.0a8/otree/channels/
--rw-rw-rw-   0        0        0        0 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/channels/__init__.py
--rw-rw-rw-   0        0        0    27401 2023-03-24 17:39:59.000000 otree-6.0.0a8/otree/channels/consumers.py
--rw-rw-rw-   0        0        0      930 2023-03-24 17:39:59.000000 otree-6.0.0a8/otree/channels/routing.py
--rw-rw-rw-   0        0        0     4489 2023-03-24 17:39:59.000000 otree-6.0.0a8/otree/channels/utils.py
--rw-rw-rw-   0        0        0     2407 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/chat.py
--rw-rw-rw-   0        0        0    11062 2023-04-15 16:38:25.000000 otree-6.0.0a8/otree/checks.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.140693 otree-6.0.0a8/otree/cli/
--rw-rw-rw-   0        0        0        0 2021-09-07 01:38:00.000000 otree-6.0.0a8/otree/cli/__init__.py
--rw-rw-rw-   0        0        0      841 2021-06-29 10:07:36.000000 otree-6.0.0a8/otree/cli/base.py
--rw-rw-rw-   0        0        0     1846 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/cli/bots.py
--rw-rw-rw-   0        0        0     1072 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/cli/browser_bots.py
--rw-rw-rw-   0        0        0     1337 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/cli/create_session.py
--rw-rw-rw-   0        0        0     3402 2021-09-28 08:02:58.000000 otree-6.0.0a8/otree/cli/devserver.py
--rw-rw-rw-   0        0        0     2051 2021-09-28 08:03:24.000000 otree-6.0.0a8/otree/cli/devserver_inner.py
--rw-rw-rw-   0        0        0       35 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/cli/prodserver.py
--rw-rw-rw-   0        0        0     1766 2021-06-30 10:11:04.000000 otree-6.0.0a8/otree/cli/prodserver1of2.py
--rw-rw-rw-   0        0        0      258 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/cli/prodserver2of2.py
--rw-rw-rw-   0        0        0    14172 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/cli/remove_self.py
--rw-rw-rw-   0        0        0     1981 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/cli/resetdb.py
--rw-rw-rw-   0        0        0     1957 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/cli/startapp.py
--rw-rw-rw-   0        0        0     2796 2022-12-23 08:54:35.000000 otree-6.0.0a8/otree/cli/startproject.py
--rw-rw-rw-   0        0        0      345 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/cli/timeoutsubprocess.py
--rw-rw-rw-   0        0        0     1224 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/cli/unzip.py
--rw-rw-rw-   0        0        0     2290 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/cli/upcase_constants.py
--rw-rw-rw-   0        0        0     7229 2021-06-30 09:55:02.000000 otree-6.0.0a8/otree/cli/update_my_code.py
--rw-rw-rw-   0        0        0     7301 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/cli/zip.py
--rw-rw-rw-   0        0        0     6434 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/cli/zipserver.py
--rw-rw-rw-   0        0        0     7803 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/common.py
--rw-rw-rw-   0        0        0     5217 2023-04-15 09:44:16.000000 otree-6.0.0a8/otree/common2.py
--rw-rw-rw-   0        0        0     2511 2022-11-23 14:41:17.000000 otree-6.0.0a8/otree/constants.py
--rw-rw-rw-   0        0        0     8663 2022-09-17 23:55:17.000000 otree-6.0.0a8/otree/currency.py
--rw-rw-rw-   0        0        0    33059 2023-04-15 18:40:54.000000 otree-6.0.0a8/otree/database.py
--rw-rw-rw-   0        0        0     8278 2022-03-04 18:20:48.000000 otree-6.0.0a8/otree/errorpage.py
--rw-rw-rw-   0        0        0    16209 2022-11-23 14:41:17.000000 otree-6.0.0a8/otree/export.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.144818 otree-6.0.0a8/otree/forms/
--rw-rw-rw-   0        0        0        0 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/forms/__init__.py
--rw-rw-rw-   0        0        0     3620 2022-09-19 10:51:45.000000 otree-6.0.0a8/otree/forms/fields.py
--rw-rw-rw-   0        0        0    10547 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/forms/forms.py
--rw-rw-rw-   0        0        0     7446 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/forms/widgets.py
--rw-rw-rw-   0        0        0     6841 2022-09-19 10:51:45.000000 otree-6.0.0a8/otree/i18n.py
--rw-rw-rw-   0        0        0     3662 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/live.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.145865 otree-6.0.0a8/otree/locale/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.030486 otree-6.0.0a8/otree/locale/ar/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.147971 otree-6.0.0a8/otree/locale/ar/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1532 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/ar/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3986 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/ar/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0      120 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/babel.ini
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.030486 otree-6.0.0a8/otree/locale/cs/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.150098 otree-6.0.0a8/otree/locale/cs/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1409 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/cs/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3712 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/cs/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.031755 otree-6.0.0a8/otree/locale/de/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.153630 otree-6.0.0a8/otree/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1762 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3875 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/de/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0     3188 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/django.pot
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.032501 otree-6.0.0a8/otree/locale/es/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.154757 otree-6.0.0a8/otree/locale/es/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1567 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/es/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.033278 otree-6.0.0a8/otree/locale/fi/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.156462 otree-6.0.0a8/otree/locale/fi/LC_MESSAGES/
--rw-rw-rw-   0        0        0      497 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/fi/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3114 2021-11-29 03:59:50.000000 otree-6.0.0a8/otree/locale/fi/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.033278 otree-6.0.0a8/otree/locale/fr/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.158309 otree-6.0.0a8/otree/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1634 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3747 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/fr/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.034294 otree-6.0.0a8/otree/locale/he/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.160303 otree-6.0.0a8/otree/locale/he/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1652 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/he/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3703 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/he/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.035291 otree-6.0.0a8/otree/locale/hi/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.162082 otree-6.0.0a8/otree/locale/hi/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2206 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/hi/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     4254 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/hi/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.036289 otree-6.0.0a8/otree/locale/hu/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.163946 otree-6.0.0a8/otree/locale/hu/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1722 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/hu/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3900 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/hu/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.037289 otree-6.0.0a8/otree/locale/id/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.166149 otree-6.0.0a8/otree/locale/id/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1520 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/locale/id/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3605 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/locale/id/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.038289 otree-6.0.0a8/otree/locale/it/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.169209 otree-6.0.0a8/otree/locale/it/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1620 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/it/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3733 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/it/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.038289 otree-6.0.0a8/otree/locale/ja/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.170373 otree-6.0.0a8/otree/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1747 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/ja/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3826 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/ja/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.039291 otree-6.0.0a8/otree/locale/ko/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.172393 otree-6.0.0a8/otree/locale/ko/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1783 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/ko/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3917 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/ko/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.040289 otree-6.0.0a8/otree/locale/nb/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.174069 otree-6.0.0a8/otree/locale/nb/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1023 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/nb/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3421 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/nb/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.040289 otree-6.0.0a8/otree/locale/nl/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.176060 otree-6.0.0a8/otree/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1579 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3669 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.041355 otree-6.0.0a8/otree/locale/pl/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.178069 otree-6.0.0a8/otree/locale/pl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1616 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/pl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/pl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.041355 otree-6.0.0a8/otree/locale/pt/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.179864 otree-6.0.0a8/otree/locale/pt/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1616 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/pt/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/pt/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.042405 otree-6.0.0a8/otree/locale/ru/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.181652 otree-6.0.0a8/otree/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2047 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/ru/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     4156 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/ru/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.042405 otree-6.0.0a8/otree/locale/tr/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.185052 otree-6.0.0a8/otree/locale/tr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1537 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/tr/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3731 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/tr/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.043402 otree-6.0.0a8/otree/locale/zh_Hans/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.186842 otree-6.0.0a8/otree/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1452 2022-04-27 15:07:46.000000 otree-6.0.0a8/otree/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0     3521 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/locale/zh_Hans/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0     2323 2021-08-31 15:42:14.000000 otree-6.0.0a8/otree/lookup.py
--rw-rw-rw-   0        0        0     6971 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/main.py
--rw-rw-rw-   0        0        0     1819 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.192719 otree-6.0.0a8/otree/models/
--rw-rw-rw-   0        0        0      230 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/models/__init__.py
--rw-rw-rw-   0        0        0     4133 2021-11-18 17:14:02.000000 otree-6.0.0a8/otree/models/group.py
--rw-rw-rw-   0        0        0     8714 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/models/participant.py
--rw-rw-rw-   0        0        0     3346 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/models/player.py
--rw-rw-rw-   0        0        0     9750 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/models/session.py
--rw-rw-rw-   0        0        0     9025 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/models/subsession.py
--rw-rw-rw-   0        0        0     1929 2021-08-18 09:23:18.000000 otree-6.0.0a8/otree/models_concrete.py
--rw-rw-rw-   0        0        0     7383 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/mturk_client.py
--rw-rw-rw-   0        0        0     1897 2022-03-04 18:20:48.000000 otree-6.0.0a8/otree/patch.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.197107 otree-6.0.0a8/otree/project_template/
--rw-rw-rw-   0        0        0      133 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/project_template/.gitignore
--rw-rw-rw-   0        0        0       57 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/project_template/Procfile
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.044414 otree-6.0.0a8/otree/project_template/_static/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.198029 otree-6.0.0a8/otree/project_template/_static/global/
--rw-rw-rw-   0        0        0        0 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/project_template/_static/global/empty.css
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.045402 otree-6.0.0a8/otree/project_template/_templates/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.199071 otree-6.0.0a8/otree/project_template/_templates/global/
--rw-rw-rw-   0        0        0      149 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/project_template/_templates/global/Page.html
--rw-rw-rw-   0        0        0      169 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/project_template/requirements.txt
--rw-rw-rw-   0        0        0     1018 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/project_template/settings.py
--rw-rw-rw-   0        0        0     2567 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/read_csv.py
--rw-rw-rw-   0        0        0     4291 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/room.py
--rw-rw-rw-   0        0        0    15047 2022-12-23 08:54:23.000000 otree-6.0.0a8/otree/session.py
--rw-rw-rw-   0        0        0     2380 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.201847 otree-6.0.0a8/otree/static/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.046402 otree-6.0.0a8/otree/static/bootstrap5/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.203816 otree-6.0.0a8/otree/static/bootstrap5/css/
--rw-rw-rw-   0        0        0   155637 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/bootstrap5/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   429472 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/bootstrap5/css/bootstrap.min.css.map
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.205822 otree-6.0.0a8/otree/static/bootstrap5/js/
--rw-rw-rw-   0        0        0    78754 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/bootstrap5/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   326390 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/bootstrap5/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0        0        0      198 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/favicon.ico
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.221932 otree-6.0.0a8/otree/static/glyphicons/
--rw-rw-rw-   0        0        0     1412 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/clock.png
--rw-rw-rw-   0        0        0     1307 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/cloud.png
--rw-rw-rw-   0        0        0     1443 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/cogwheel.png
--rw-rw-rw-   0        0        0     1310 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/delete.png
--rw-rw-rw-   0        0        0     1314 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/download-alt.png
--rw-rw-rw-   0        0        0     1475 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/eye-open.png
--rw-rw-rw-   0        0        0     1243 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/folder-closed.png
--rw-rw-rw-   0        0        0     1436 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/link.png
--rw-rw-rw-   0        0        0     1231 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/list-alt.png
--rw-rw-rw-   0        0        0     1342 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/pencil.png
--rw-rw-rw-   0        0        0     1218 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/plus.png
--rw-rw-rw-   0        0        0     1378 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/pushpin.png
--rw-rw-rw-   0        0        0     1471 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/refresh.png
--rw-rw-rw-   0        0        0     1499 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/stats.png
--rw-rw-rw-   0        0        0     1432 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/glyphicons/usd.png
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.046402 otree-6.0.0a8/otree/static/otree/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.223786 otree-6.0.0a8/otree/static/otree/css/
--rw-rw-rw-   0        0        0      868 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/otree/css/table.css
--rw-rw-rw-   0        0        0     2015 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/otree/css/theme.css
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.241020 otree-6.0.0a8/otree/static/otree/js/
--rw-rw-rw-   0        0        0     1909 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/static/otree/js/common.js
--rw-rw-rw-   0        0        0     1624 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/static/otree/js/formInputs.js
--rw-rw-rw-   0        0        0      504 2020-10-07 12:35:10.000000 otree-6.0.0a8/otree/static/otree/js/internet-explorer.js
--rw-rw-rw-   0        0        0    86663 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/otree/js/jquery-3.2.1.min.js
--rw-rw-rw-   0        0        0     6605 2020-11-23 22:42:18.000000 otree-6.0.0a8/otree/static/otree/js/jquery.color-2.1.2.min.js
--rw-rw-rw-   0        0        0     5360 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/otree/js/jquery.countdown.min.js
--rw-rw-rw-   0        0        0      702 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/otree/js/jquery.timeago.en-short.js
--rw-rw-rw-   0        0        0     7200 2018-12-27 12:55:56.000000 otree-6.0.0a8/otree/static/otree/js/jquery.timeago.js
--rw-rw-rw-   0        0        0      663 2023-03-24 17:39:59.000000 otree-6.0.0a8/otree/static/otree/js/live.js
--rw-rw-rw-   0        0        0     4271 2022-11-23 14:41:17.000000 otree-6.0.0a8/otree/static/otree/js/monitor2.js
--rw-rw-rw-   0        0        0    49322 2023-04-15 17:21:55.000000 otree-6.0.0a8/otree/static/otree/js/otree-front.js
--rw-rw-rw-   0        0        0      967 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/otree/js/page-websocket-redirect.js
--rw-rw-rw-   0        0        0     8729 2020-03-20 01:44:18.000000 otree-6.0.0a8/otree/static/otree/js/reconnecting-websocket-iife.min.js
--rw-rw-rw-   0        0        0     4837 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/static/otree/js/table-utils.js
--rw-rw-rw-   0        0        0      861 2023-04-15 16:01:01.000000 otree-6.0.0a8/otree/static/otree/js/trial-default.js
--rw-rw-rw-   0        0        0      221 2023-04-15 08:05:11.000000 otree-6.0.0a8/otree/static/otree/js/trial-setup.js
--rw-rw-rw-   0        0        0       26 2018-11-23 17:31:48.000000 otree-6.0.0a8/otree/static/robots.txt
--rw-rw-rw-   0        0        0     5360 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/tasks.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.047402 otree-6.0.0a8/otree/templates/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.243353 otree-6.0.0a8/otree/templates/global/
--rw-rw-rw-   0        0        0       33 2020-12-01 22:34:50.000000 otree-6.0.0a8/otree/templates/global/Base.html
--rw-rw-rw-   0        0        0      293 2021-10-18 21:34:16.000000 otree-6.0.0a8/otree/templates/global/Page.html
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.274743 otree-6.0.0a8/otree/templates/otree/
--rw-rw-rw-   0        0        0      881 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/AdminReport.html
--rw-rw-rw-   0        0        0     1768 2023-04-15 08:08:38.000000 otree-6.0.0a8/otree/templates/otree/Base.html
--rw-rw-rw-   0        0        0     3065 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/BaseAdmin.html
--rw-rw-rw-   0        0        0     2881 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/CreateDemoSession.html
--rw-rw-rw-   0        0        0      199 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/CreateSession.html
--rw-rw-rw-   0        0        0      955 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/DemoIndex.html
--rw-rw-rw-   0        0        0     5961 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/templates/otree/Export.html
--rw-rw-rw-   0        0        0       31 2020-12-01 22:34:50.000000 otree-6.0.0a8/otree/templates/otree/FormPage.html
--rw-rw-rw-   0        0        0     1240 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/Login.html
--rw-rw-rw-   0        0        0     2796 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/templates/otree/MTurkCreateHIT.html
--rw-rw-rw-   0        0        0     1214 2020-12-01 22:34:50.000000 otree-6.0.0a8/otree/templates/otree/MTurkHTMLQuestion.html
--rw-rw-rw-   0        0        0     6732 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/templates/otree/MTurkSessionPayments.html
--rw-rw-rw-   0        0        0       18 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/OutOfRangeNotification.html
--rw-rw-rw-   0        0        0     3116 2023-04-15 17:20:30.000000 otree-6.0.0a8/otree/templates/otree/Page.html
--rw-rw-rw-   0        0        0      911 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/templates/otree/RoomInputLabel.html
--rw-rw-rw-   0        0        0      754 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/RoomWithSession.html
--rw-rw-rw-   0        0        0     4282 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/RoomWithoutSession.html
--rw-rw-rw-   0        0        0      353 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/Rooms.html
--rw-rw-rw-   0        0        0     1784 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/templates/otree/ServerCheck.html
--rw-rw-rw-   0        0        0     2532 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/Session.html
--rw-rw-rw-   0        0        0     7856 2021-08-19 09:01:20.000000 otree-6.0.0a8/otree/templates/otree/SessionData.html
--rw-rw-rw-   0        0        0      139 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/SessionDescription.html
--rw-rw-rw-   0        0        0      323 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/SessionEditProperties.html
--rw-rw-rw-   0        0        0     2391 2022-11-23 14:41:17.000000 otree-6.0.0a8/otree/templates/otree/SessionMonitor.html
--rw-rw-rw-   0        0        0     1582 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/SessionPayments.html
--rw-rw-rw-   0        0        0     3329 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/SessionSplitScreen.html
--rw-rw-rw-   0        0        0     4087 2021-09-02 00:40:54.000000 otree-6.0.0a8/otree/templates/otree/SessionStartLinks.html
--rw-rw-rw-   0        0        0     5469 2022-05-14 06:42:33.000000 otree-6.0.0a8/otree/templates/otree/Sessions.html
--rw-rw-rw-   0        0        0     5121 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/templates/otree/WaitPage.html
--rw-rw-rw-   0        0        0       37 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/WaitPageRoom.html
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.286472 otree-6.0.0a8/otree/templates/otree/includes/
--rw-rw-rw-   0        0        0     5461 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/includes/CreateSessionForm.html
--rw-rw-rw-   0        0        0     1528 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/includes/RoomParticipantLinks.html
--rw-rw-rw-   0        0        0      402 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/includes/SessionInfo.html
--rw-rw-rw-   0        0        0      213 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/includes/TimeLimit.html
--rw-rw-rw-   0        0        0      997 2022-07-06 11:50:24.000000 otree-6.0.0a8/otree/templates/otree/includes/TimeLimit.js.html
--rw-rw-rw-   0        0        0      969 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/includes/debug_info.html
--rw-rw-rw-   0        0        0     2679 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/templates/otree/includes/hidden_form_errors.html
--rw-rw-rw-   0        0        0      244 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/includes/messages.html
--rw-rw-rw-   0        0        0     1368 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templates/otree/includes/mturk_payment_table.html
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.287651 otree-6.0.0a8/otree/templates/otree/tags/
--rw-rw-rw-   0        0        0     3572 2021-09-09 20:27:16.000000 otree-6.0.0a8/otree/templates/otree/tags/chat.html
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.297592 otree-6.0.0a8/otree/templating/
--rw-rw-rw-   0        0        0       70 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templating/__init__.py
--rw-rw-rw-   0        0        0     6993 2021-09-10 18:14:58.000000 otree-6.0.0a8/otree/templating/compiler.py
--rw-rw-rw-   0        0        0     2948 2021-09-23 22:55:28.000000 otree-6.0.0a8/otree/templating/context.py
--rw-rw-rw-   0        0        0     1342 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templating/errors.py
--rw-rw-rw-   0        0        0     2081 2021-08-11 02:49:06.000000 otree-6.0.0a8/otree/templating/filters.py
--rw-rw-rw-   0        0        0     3392 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/templating/loader.py
--rw-rw-rw-   0        0        0    33516 2023-04-15 08:53:48.000000 otree-6.0.0a8/otree/templating/nodes.py
--rw-rw-rw-   0        0        0     1495 2021-09-10 17:48:20.000000 otree-6.0.0a8/otree/templating/template.py
--rw-rw-rw-   0        0        0     1836 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/templating/utils.py
--rw-rw-rw-   0        0        0      173 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/test.py
--rw-rw-rw-   0        0        0     4850 2023-04-15 18:39:16.000000 otree-6.0.0a8/otree/trial.py
--rw-rw-rw-   0        0        0     1919 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/update.py
--rw-rw-rw-   0        0        0     4635 2023-03-24 17:39:59.000000 otree-6.0.0a8/otree/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.310293 otree-6.0.0a8/otree/views/
--rw-rw-rw-   0        0        0       49 2020-06-23 01:10:42.000000 otree-6.0.0a8/otree/views/__init__.py
--rw-rw-rw-   0        0        0    49935 2023-04-15 09:49:30.000000 otree-6.0.0a8/otree/views/abstract.py
--rw-rw-rw-   0        0        0    19290 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/views/admin.py
--rw-rw-rw-   0        0        0     8261 2022-03-03 11:49:02.000000 otree-6.0.0a8/otree/views/cbv.py
--rw-rw-rw-   0        0        0     1537 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/views/demo.py
--rw-rw-rw-   0        0        0     3722 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/views/export.py
--rw-rw-rw-   0        0        0    14856 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/views/mturk.py
--rw-rw-rw-   0        0        0    12981 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/views/participant.py
--rw-rw-rw-   0        0        0    10004 2023-03-08 18:09:53.000000 otree-6.0.0a8/otree/views/rest.py
--rw-rw-rw-   0        0        0     2523 2021-06-06 11:37:30.000000 otree-6.0.0a8/otree/views/room.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:48:35.092073 otree-6.0.0a8/otree.egg-info/
--rw-rw-rw-   0        0        0     1886 2023-04-15 18:48:34.000000 otree-6.0.0a8/otree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8038 2023-04-15 18:48:34.000000 otree-6.0.0a8/otree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 18:48:34.000000 otree-6.0.0a8/otree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-04-15 18:48:34.000000 otree-6.0.0a8/otree.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2020-11-22 05:26:26.000000 otree-6.0.0a8/otree.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      196 2023-04-15 18:48:34.000000 otree-6.0.0a8/otree.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-15 18:48:34.000000 otree-6.0.0a8/otree.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      311 2023-03-08 18:09:53.000000 otree-6.0.0a8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 18:48:35.311947 otree-6.0.0a8/setup.cfg
--rw-rw-rw-   0        0        0     2548 2023-03-08 18:09:53.000000 otree-6.0.0a8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:52.109933 otree-6.0.0a9/
+-rw-rw-rw-   0        0        0     1573 2018-11-23 17:31:44.000000 otree-6.0.0a9/LICENSE
+-rw-rw-rw-   0        0        0      390 2021-06-06 11:37:30.000000 otree-6.0.0a9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1886 2023-04-17 16:33:52.108884 otree-6.0.0a9/PKG-INFO
+-rw-rw-rw-   0        0        0     1581 2022-03-03 11:49:02.000000 otree-6.0.0a9/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.879711 otree-6.0.0a9/otree/
+-rw-rw-rw-   0        0        0       91 2023-04-17 16:33:27.000000 otree-6.0.0a9/otree/__init__.py
+-rw-rw-rw-   0        0        0      634 2023-04-15 17:56:00.000000 otree-6.0.0a9/otree/api.py
+-rw-rw-rw-   0        0        0    10442 2023-04-17 02:46:42.000000 otree-6.0.0a9/otree/api.pyi
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.901075 otree-6.0.0a9/otree/app_template/
+-rw-rw-rw-   0        0        0        0 2018-11-23 17:31:44.000000 otree-6.0.0a9/otree/app_template/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.908223 otree-6.0.0a9/otree/app_template/__pycache__/
+-rw-rw-rw-   0        0        0      127 2017-10-09 12:58:16.000000 otree-6.0.0a9/otree/app_template/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      131 2019-07-18 16:08:18.000000 otree-6.0.0a9/otree/app_template/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0     1013 2017-10-09 12:58:16.000000 otree-6.0.0a9/otree/app_template/__pycache__/models.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1017 2019-07-18 16:08:18.000000 otree-6.0.0a9/otree/app_template/__pycache__/models.cpython-37.pyc
+-rw-rw-rw-   0        0        0      615 2017-10-09 12:58:16.000000 otree-6.0.0a9/otree/app_template/__pycache__/tests.cpython-36.pyc
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.909226 otree-6.0.0a9/otree/app_template/_builtin/
+-rw-rw-rw-   0        0        0      446 2020-10-07 12:35:10.000000 otree-6.0.0a9/otree/app_template/_builtin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.911268 otree-6.0.0a9/otree/app_template/_builtin/__pycache__/
+-rw-rw-rw-   0        0        0     1170 2017-10-09 12:58:16.000000 otree-6.0.0a9/otree/app_template/_builtin/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0      871 2019-07-18 16:08:18.000000 otree-6.0.0a9/otree/app_template/_builtin/__pycache__/__init__.cpython-37.pyc
+-rw-rw-rw-   0        0        0      464 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/app_template/models.py
+-rw-rw-rw-   0        0        0      297 2020-10-07 12:35:10.000000 otree-6.0.0a9/otree/app_template/pages.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.825076 otree-6.0.0a9/otree/app_template/templates/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.913492 otree-6.0.0a9/otree/app_template/templates/app_name/
+-rw-rw-rw-   0        0        0      200 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/app_template/templates/app_name/MyPage.html
+-rw-rw-rw-   0        0        0      180 2020-12-11 18:14:00.000000 otree-6.0.0a9/otree/app_template/templates/app_name/Results.html
+-rw-rw-rw-   0        0        0      200 2020-03-20 01:44:18.000000 otree-6.0.0a9/otree/app_template/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.916189 otree-6.0.0a9/otree/app_template_lite/
+-rw-rw-rw-   0        0        0      137 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/app_template_lite/MyPage.html
+-rw-rw-rw-   0        0        0      119 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/app_template_lite/Results.html
+-rw-rw-rw-   0        0        0      495 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/app_template_lite/__init__.py
+-rw-rw-rw-   0        0        0     2888 2022-03-04 18:20:48.000000 otree-6.0.0a9/otree/asgi.py
+-rw-rw-rw-   0        0        0        0 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/auth.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.922618 otree-6.0.0a9/otree/bots/
+-rw-rw-rw-   0        0        0       75 2020-03-20 01:44:18.000000 otree-6.0.0a9/otree/bots/__init__.py
+-rw-rw-rw-   0        0        0    18278 2023-04-15 00:24:13.000000 otree-6.0.0a9/otree/bots/bot.py
+-rw-rw-rw-   0        0        0     4815 2022-12-23 08:54:23.000000 otree-6.0.0a9/otree/bots/browser.py
+-rw-rw-rw-   0        0        0    11868 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/bots/browser_launcher.py
+-rw-rw-rw-   0        0        0     6713 2022-02-01 22:47:42.000000 otree-6.0.0a9/otree/bots/runner.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.927614 otree-6.0.0a9/otree/channels/
+-rw-rw-rw-   0        0        0        0 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/channels/__init__.py
+-rw-rw-rw-   0        0        0    27401 2023-03-24 17:39:59.000000 otree-6.0.0a9/otree/channels/consumers.py
+-rw-rw-rw-   0        0        0      930 2023-03-24 17:39:59.000000 otree-6.0.0a9/otree/channels/routing.py
+-rw-rw-rw-   0        0        0     4489 2023-03-24 17:39:59.000000 otree-6.0.0a9/otree/channels/utils.py
+-rw-rw-rw-   0        0        0     2407 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/chat.py
+-rw-rw-rw-   0        0        0    11714 2023-04-17 16:24:50.000000 otree-6.0.0a9/otree/checks.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.946950 otree-6.0.0a9/otree/cli/
+-rw-rw-rw-   0        0        0        0 2021-09-07 01:38:00.000000 otree-6.0.0a9/otree/cli/__init__.py
+-rw-rw-rw-   0        0        0      841 2021-06-29 10:07:36.000000 otree-6.0.0a9/otree/cli/base.py
+-rw-rw-rw-   0        0        0     1846 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/cli/bots.py
+-rw-rw-rw-   0        0        0     1072 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/cli/browser_bots.py
+-rw-rw-rw-   0        0        0     1337 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/cli/create_session.py
+-rw-rw-rw-   0        0        0     3402 2021-09-28 08:02:58.000000 otree-6.0.0a9/otree/cli/devserver.py
+-rw-rw-rw-   0        0        0     2051 2021-09-28 08:03:24.000000 otree-6.0.0a9/otree/cli/devserver_inner.py
+-rw-rw-rw-   0        0        0       35 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/cli/prodserver.py
+-rw-rw-rw-   0        0        0     1766 2021-06-30 10:11:04.000000 otree-6.0.0a9/otree/cli/prodserver1of2.py
+-rw-rw-rw-   0        0        0      258 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/cli/prodserver2of2.py
+-rw-rw-rw-   0        0        0    14172 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/cli/remove_self.py
+-rw-rw-rw-   0        0        0     1981 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/cli/resetdb.py
+-rw-rw-rw-   0        0        0     1957 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/cli/startapp.py
+-rw-rw-rw-   0        0        0     2796 2022-12-23 08:54:35.000000 otree-6.0.0a9/otree/cli/startproject.py
+-rw-rw-rw-   0        0        0      345 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/cli/timeoutsubprocess.py
+-rw-rw-rw-   0        0        0     1224 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/cli/unzip.py
+-rw-rw-rw-   0        0        0     2290 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/cli/upcase_constants.py
+-rw-rw-rw-   0        0        0     7229 2021-06-30 09:55:02.000000 otree-6.0.0a9/otree/cli/update_my_code.py
+-rw-rw-rw-   0        0        0     7301 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/cli/zip.py
+-rw-rw-rw-   0        0        0     6434 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/cli/zipserver.py
+-rw-rw-rw-   0        0        0     7803 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/common.py
+-rw-rw-rw-   0        0        0     5462 2023-04-15 18:59:50.000000 otree-6.0.0a9/otree/common2.py
+-rw-rw-rw-   0        0        0     2511 2022-11-23 14:41:17.000000 otree-6.0.0a9/otree/constants.py
+-rw-rw-rw-   0        0        0     8663 2022-09-17 23:55:17.000000 otree-6.0.0a9/otree/currency.py
+-rw-rw-rw-   0        0        0    33059 2023-04-15 18:40:54.000000 otree-6.0.0a9/otree/database.py
+-rw-rw-rw-   0        0        0     8278 2022-03-04 18:20:48.000000 otree-6.0.0a9/otree/errorpage.py
+-rw-rw-rw-   0        0        0    16209 2022-11-23 14:41:17.000000 otree-6.0.0a9/otree/export.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.950144 otree-6.0.0a9/otree/forms/
+-rw-rw-rw-   0        0        0        0 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/forms/__init__.py
+-rw-rw-rw-   0        0        0     3620 2022-09-19 10:51:45.000000 otree-6.0.0a9/otree/forms/fields.py
+-rw-rw-rw-   0        0        0    10547 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/forms/forms.py
+-rw-rw-rw-   0        0        0     7446 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/forms/widgets.py
+-rw-rw-rw-   0        0        0     6841 2022-09-19 10:51:45.000000 otree-6.0.0a9/otree/i18n.py
+-rw-rw-rw-   0        0        0     3662 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/live.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.952105 otree-6.0.0a9/otree/locale/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.829326 otree-6.0.0a9/otree/locale/ar/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.954086 otree-6.0.0a9/otree/locale/ar/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1532 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/ar/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3986 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/ar/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0      120 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/babel.ini
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.829971 otree-6.0.0a9/otree/locale/cs/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.955665 otree-6.0.0a9/otree/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1409 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/cs/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3712 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/cs/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.830797 otree-6.0.0a9/otree/locale/de/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.958001 otree-6.0.0a9/otree/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1762 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3875 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/de/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     3188 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/django.pot
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.831206 otree-6.0.0a9/otree/locale/es/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.959954 otree-6.0.0a9/otree/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1567 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/es/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/es/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.831537 otree-6.0.0a9/otree/locale/fi/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.961897 otree-6.0.0a9/otree/locale/fi/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      497 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/fi/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3114 2021-11-29 03:59:50.000000 otree-6.0.0a9/otree/locale/fi/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.832315 otree-6.0.0a9/otree/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.963695 otree-6.0.0a9/otree/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1634 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3747 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/fr/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.832508 otree-6.0.0a9/otree/locale/he/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.965389 otree-6.0.0a9/otree/locale/he/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1652 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/he/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3703 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/he/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.833622 otree-6.0.0a9/otree/locale/hi/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.967064 otree-6.0.0a9/otree/locale/hi/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2206 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/hi/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     4254 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/hi/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.834203 otree-6.0.0a9/otree/locale/hu/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.969092 otree-6.0.0a9/otree/locale/hu/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1722 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/hu/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3900 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/hu/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.834903 otree-6.0.0a9/otree/locale/id/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.971093 otree-6.0.0a9/otree/locale/id/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1520 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/locale/id/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3605 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/locale/id/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.835494 otree-6.0.0a9/otree/locale/it/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.973249 otree-6.0.0a9/otree/locale/it/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1620 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/it/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3733 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/it/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.836088 otree-6.0.0a9/otree/locale/ja/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.975523 otree-6.0.0a9/otree/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1747 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/ja/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3826 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/ja/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.836587 otree-6.0.0a9/otree/locale/ko/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.976523 otree-6.0.0a9/otree/locale/ko/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1783 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/ko/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3917 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/ko/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.836959 otree-6.0.0a9/otree/locale/nb/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.978495 otree-6.0.0a9/otree/locale/nb/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1023 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/nb/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3421 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/nb/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.837691 otree-6.0.0a9/otree/locale/nl/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.980261 otree-6.0.0a9/otree/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1579 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3669 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.838158 otree-6.0.0a9/otree/locale/pl/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.982032 otree-6.0.0a9/otree/locale/pl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1616 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/pl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.838996 otree-6.0.0a9/otree/locale/pt/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.983828 otree-6.0.0a9/otree/locale/pt/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1616 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3683 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/pt/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.839533 otree-6.0.0a9/otree/locale/ru/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.985826 otree-6.0.0a9/otree/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2047 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     4156 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/ru/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.840336 otree-6.0.0a9/otree/locale/tr/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.986963 otree-6.0.0a9/otree/locale/tr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1537 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/tr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3731 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/tr/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.840957 otree-6.0.0a9/otree/locale/zh_Hans/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.988986 otree-6.0.0a9/otree/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1452 2022-04-27 15:07:46.000000 otree-6.0.0a9/otree/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0     3521 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     2323 2021-08-31 15:42:14.000000 otree-6.0.0a9/otree/lookup.py
+-rw-rw-rw-   0        0        0     6971 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/main.py
+-rw-rw-rw-   0        0        0     1819 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.994549 otree-6.0.0a9/otree/models/
+-rw-rw-rw-   0        0        0      230 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/models/__init__.py
+-rw-rw-rw-   0        0        0     4133 2021-11-18 17:14:02.000000 otree-6.0.0a9/otree/models/group.py
+-rw-rw-rw-   0        0        0     8714 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/models/participant.py
+-rw-rw-rw-   0        0        0     3346 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/models/player.py
+-rw-rw-rw-   0        0        0     9750 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/models/session.py
+-rw-rw-rw-   0        0        0     9025 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/models/subsession.py
+-rw-rw-rw-   0        0        0     1929 2021-08-18 09:23:18.000000 otree-6.0.0a9/otree/models_concrete.py
+-rw-rw-rw-   0        0        0     7383 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/mturk_client.py
+-rw-rw-rw-   0        0        0     1897 2022-03-04 18:20:48.000000 otree-6.0.0a9/otree/patch.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.999040 otree-6.0.0a9/otree/project_template/
+-rw-rw-rw-   0        0        0      133 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/project_template/.gitignore
+-rw-rw-rw-   0        0        0       57 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/project_template/Procfile
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.842182 otree-6.0.0a9/otree/project_template/_static/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:52.000038 otree-6.0.0a9/otree/project_template/_static/global/
+-rw-rw-rw-   0        0        0        0 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/project_template/_static/global/empty.css
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.842762 otree-6.0.0a9/otree/project_template/_templates/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:52.000038 otree-6.0.0a9/otree/project_template/_templates/global/
+-rw-rw-rw-   0        0        0      149 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/project_template/_templates/global/Page.html
+-rw-rw-rw-   0        0        0      169 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/project_template/requirements.txt
+-rw-rw-rw-   0        0        0     1018 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/project_template/settings.py
+-rw-rw-rw-   0        0        0     2567 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/read_csv.py
+-rw-rw-rw-   0        0        0     4291 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/room.py
+-rw-rw-rw-   0        0        0    15047 2022-12-23 08:54:23.000000 otree-6.0.0a9/otree/session.py
+-rw-rw-rw-   0        0        0     2380 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:52.001994 otree-6.0.0a9/otree/static/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.843931 otree-6.0.0a9/otree/static/bootstrap5/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:52.004405 otree-6.0.0a9/otree/static/bootstrap5/css/
+-rw-rw-rw-   0        0        0   155637 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/static/bootstrap5/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   429472 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/static/bootstrap5/css/bootstrap.min.css.map
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:52.007444 otree-6.0.0a9/otree/static/bootstrap5/js/
+-rw-rw-rw-   0        0        0    78754 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/static/bootstrap5/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   326390 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/static/bootstrap5/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0        0        0      198 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/static/favicon.ico
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:52.022619 otree-6.0.0a9/otree/static/glyphicons/
+-rw-rw-rw-   0        0        0     1412 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/glyphicons/clock.png
+-rw-rw-rw-   0        0        0     1307 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/glyphicons/cloud.png
+-rw-rw-rw-   0        0        0     1443 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/glyphicons/cogwheel.png
+-rw-rw-rw-   0        0        0     1310 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/glyphicons/delete.png
+-rw-rw-rw-   0        0        0     1314 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/glyphicons/download-alt.png
+-rw-rw-rw-   0        0        0     1475 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/glyphicons/eye-open.png
+-rw-rw-rw-   0        0        0     1243 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/glyphicons/folder-closed.png
+-rw-rw-rw-   0        0        0     1436 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/glyphicons/link.png
+-rw-rw-rw-   0        0        0     1231 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/glyphicons/list-alt.png
+-rw-rw-rw-   0        0        0     1342 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/glyphicons/pencil.png
+-rw-rw-rw-   0        0        0     1218 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/glyphicons/plus.png
+-rw-rw-rw-   0        0        0     1378 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/glyphicons/pushpin.png
+-rw-rw-rw-   0        0        0     1471 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/glyphicons/refresh.png
+-rw-rw-rw-   0        0        0     1499 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/glyphicons/stats.png
+-rw-rw-rw-   0        0        0     1432 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/glyphicons/usd.png
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.845445 otree-6.0.0a9/otree/static/otree/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:52.025095 otree-6.0.0a9/otree/static/otree/css/
+-rw-rw-rw-   0        0        0      868 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/otree/css/table.css
+-rw-rw-rw-   0        0        0     2015 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/static/otree/css/theme.css
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:52.042961 otree-6.0.0a9/otree/static/otree/js/
+-rw-rw-rw-   0        0        0     1909 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/static/otree/js/common.js
+-rw-rw-rw-   0        0        0     1624 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/static/otree/js/formInputs.js
+-rw-rw-rw-   0        0        0      504 2020-10-07 12:35:10.000000 otree-6.0.0a9/otree/static/otree/js/internet-explorer.js
+-rw-rw-rw-   0        0        0    86663 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/otree/js/jquery-3.2.1.min.js
+-rw-rw-rw-   0        0        0     6605 2020-11-23 22:42:18.000000 otree-6.0.0a9/otree/static/otree/js/jquery.color-2.1.2.min.js
+-rw-rw-rw-   0        0        0     5360 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/otree/js/jquery.countdown.min.js
+-rw-rw-rw-   0        0        0      702 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/static/otree/js/jquery.timeago.en-short.js
+-rw-rw-rw-   0        0        0     7200 2018-12-27 12:55:56.000000 otree-6.0.0a9/otree/static/otree/js/jquery.timeago.js
+-rw-rw-rw-   0        0        0      663 2023-03-24 17:39:59.000000 otree-6.0.0a9/otree/static/otree/js/live.js
+-rw-rw-rw-   0        0        0     4271 2022-11-23 14:41:17.000000 otree-6.0.0a9/otree/static/otree/js/monitor2.js
+-rw-rw-rw-   0        0        0    49536 2023-04-17 04:40:44.000000 otree-6.0.0a9/otree/static/otree/js/otree-front.js
+-rw-rw-rw-   0        0        0      967 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/static/otree/js/page-websocket-redirect.js
+-rw-rw-rw-   0        0        0     8729 2020-03-20 01:44:18.000000 otree-6.0.0a9/otree/static/otree/js/reconnecting-websocket-iife.min.js
+-rw-rw-rw-   0        0        0     4837 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/static/otree/js/table-utils.js
+-rw-rw-rw-   0        0        0      902 2023-04-17 13:15:34.000000 otree-6.0.0a9/otree/static/otree/js/trial-default.js
+-rw-rw-rw-   0        0        0      221 2023-04-15 08:05:11.000000 otree-6.0.0a9/otree/static/otree/js/trial-setup.js
+-rw-rw-rw-   0        0        0       26 2018-11-23 17:31:48.000000 otree-6.0.0a9/otree/static/robots.txt
+-rw-rw-rw-   0        0        0     5360 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/tasks.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.846080 otree-6.0.0a9/otree/templates/
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:52.045076 otree-6.0.0a9/otree/templates/global/
+-rw-rw-rw-   0        0        0       33 2020-12-01 22:34:50.000000 otree-6.0.0a9/otree/templates/global/Base.html
+-rw-rw-rw-   0        0        0      293 2021-10-18 21:34:16.000000 otree-6.0.0a9/otree/templates/global/Page.html
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:52.078511 otree-6.0.0a9/otree/templates/otree/
+-rw-rw-rw-   0        0        0      881 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/AdminReport.html
+-rw-rw-rw-   0        0        0     1768 2023-04-15 08:08:38.000000 otree-6.0.0a9/otree/templates/otree/Base.html
+-rw-rw-rw-   0        0        0     3065 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/BaseAdmin.html
+-rw-rw-rw-   0        0        0     2881 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/CreateDemoSession.html
+-rw-rw-rw-   0        0        0      199 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/CreateSession.html
+-rw-rw-rw-   0        0        0      955 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/DemoIndex.html
+-rw-rw-rw-   0        0        0     5961 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/templates/otree/Export.html
+-rw-rw-rw-   0        0        0       31 2020-12-01 22:34:50.000000 otree-6.0.0a9/otree/templates/otree/FormPage.html
+-rw-rw-rw-   0        0        0     1240 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/Login.html
+-rw-rw-rw-   0        0        0     2796 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/templates/otree/MTurkCreateHIT.html
+-rw-rw-rw-   0        0        0     1214 2020-12-01 22:34:50.000000 otree-6.0.0a9/otree/templates/otree/MTurkHTMLQuestion.html
+-rw-rw-rw-   0        0        0     6732 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/templates/otree/MTurkSessionPayments.html
+-rw-rw-rw-   0        0        0       18 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/OutOfRangeNotification.html
+-rw-rw-rw-   0        0        0     3116 2023-04-15 17:20:30.000000 otree-6.0.0a9/otree/templates/otree/Page.html
+-rw-rw-rw-   0        0        0      911 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/templates/otree/RoomInputLabel.html
+-rw-rw-rw-   0        0        0      754 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/RoomWithSession.html
+-rw-rw-rw-   0        0        0     4282 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/RoomWithoutSession.html
+-rw-rw-rw-   0        0        0      353 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/Rooms.html
+-rw-rw-rw-   0        0        0     1784 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/templates/otree/ServerCheck.html
+-rw-rw-rw-   0        0        0     2532 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/Session.html
+-rw-rw-rw-   0        0        0     7856 2021-08-19 09:01:20.000000 otree-6.0.0a9/otree/templates/otree/SessionData.html
+-rw-rw-rw-   0        0        0      139 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/SessionDescription.html
+-rw-rw-rw-   0        0        0      323 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/SessionEditProperties.html
+-rw-rw-rw-   0        0        0     2391 2022-11-23 14:41:17.000000 otree-6.0.0a9/otree/templates/otree/SessionMonitor.html
+-rw-rw-rw-   0        0        0     1582 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/SessionPayments.html
+-rw-rw-rw-   0        0        0     3329 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/SessionSplitScreen.html
+-rw-rw-rw-   0        0        0     4087 2021-09-02 00:40:54.000000 otree-6.0.0a9/otree/templates/otree/SessionStartLinks.html
+-rw-rw-rw-   0        0        0     5469 2022-05-14 06:42:33.000000 otree-6.0.0a9/otree/templates/otree/Sessions.html
+-rw-rw-rw-   0        0        0     5121 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/templates/otree/WaitPage.html
+-rw-rw-rw-   0        0        0       37 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/WaitPageRoom.html
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:52.086946 otree-6.0.0a9/otree/templates/otree/includes/
+-rw-rw-rw-   0        0        0     5461 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/includes/CreateSessionForm.html
+-rw-rw-rw-   0        0        0     1528 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/includes/RoomParticipantLinks.html
+-rw-rw-rw-   0        0        0      402 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/includes/SessionInfo.html
+-rw-rw-rw-   0        0        0      213 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/includes/TimeLimit.html
+-rw-rw-rw-   0        0        0      997 2022-07-06 11:50:24.000000 otree-6.0.0a9/otree/templates/otree/includes/TimeLimit.js.html
+-rw-rw-rw-   0        0        0      969 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/includes/debug_info.html
+-rw-rw-rw-   0        0        0     2679 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/templates/otree/includes/hidden_form_errors.html
+-rw-rw-rw-   0        0        0      244 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/includes/messages.html
+-rw-rw-rw-   0        0        0     1368 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templates/otree/includes/mturk_payment_table.html
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:52.087732 otree-6.0.0a9/otree/templates/otree/tags/
+-rw-rw-rw-   0        0        0     3572 2021-09-09 20:27:16.000000 otree-6.0.0a9/otree/templates/otree/tags/chat.html
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:52.097453 otree-6.0.0a9/otree/templating/
+-rw-rw-rw-   0        0        0       70 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templating/__init__.py
+-rw-rw-rw-   0        0        0     6993 2021-09-10 18:14:58.000000 otree-6.0.0a9/otree/templating/compiler.py
+-rw-rw-rw-   0        0        0     2948 2021-09-23 22:55:28.000000 otree-6.0.0a9/otree/templating/context.py
+-rw-rw-rw-   0        0        0     1342 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templating/errors.py
+-rw-rw-rw-   0        0        0     2081 2021-08-11 02:49:06.000000 otree-6.0.0a9/otree/templating/filters.py
+-rw-rw-rw-   0        0        0     3392 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/templating/loader.py
+-rw-rw-rw-   0        0        0    33516 2023-04-15 08:53:48.000000 otree-6.0.0a9/otree/templating/nodes.py
+-rw-rw-rw-   0        0        0     1495 2021-09-10 17:48:20.000000 otree-6.0.0a9/otree/templating/template.py
+-rw-rw-rw-   0        0        0     1836 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/templating/utils.py
+-rw-rw-rw-   0        0        0      173 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/test.py
+-rw-rw-rw-   0        0        0     4939 2023-04-16 03:54:00.000000 otree-6.0.0a9/otree/trial.py
+-rw-rw-rw-   0        0        0     1919 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/update.py
+-rw-rw-rw-   0        0        0     4635 2023-03-24 17:39:59.000000 otree-6.0.0a9/otree/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:52.107843 otree-6.0.0a9/otree/views/
+-rw-rw-rw-   0        0        0       49 2020-06-23 01:10:42.000000 otree-6.0.0a9/otree/views/__init__.py
+-rw-rw-rw-   0        0        0    48667 2023-04-17 04:43:00.000000 otree-6.0.0a9/otree/views/abstract.py
+-rw-rw-rw-   0        0        0    19290 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/views/admin.py
+-rw-rw-rw-   0        0        0     8261 2022-03-03 11:49:02.000000 otree-6.0.0a9/otree/views/cbv.py
+-rw-rw-rw-   0        0        0     1537 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/views/demo.py
+-rw-rw-rw-   0        0        0     3722 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/views/export.py
+-rw-rw-rw-   0        0        0    14856 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/views/mturk.py
+-rw-rw-rw-   0        0        0    12981 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/views/participant.py
+-rw-rw-rw-   0        0        0    10004 2023-03-08 18:09:53.000000 otree-6.0.0a9/otree/views/rest.py
+-rw-rw-rw-   0        0        0     2523 2021-06-06 11:37:30.000000 otree-6.0.0a9/otree/views/room.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:33:51.897328 otree-6.0.0a9/otree.egg-info/
+-rw-rw-rw-   0        0        0     1886 2023-04-17 16:33:51.000000 otree-6.0.0a9/otree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8038 2023-04-17 16:33:51.000000 otree-6.0.0a9/otree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 16:33:51.000000 otree-6.0.0a9/otree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-17 16:33:51.000000 otree-6.0.0a9/otree.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2020-11-22 05:26:26.000000 otree-6.0.0a9/otree.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      196 2023-04-17 16:33:51.000000 otree-6.0.0a9/otree.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-17 16:33:51.000000 otree-6.0.0a9/otree.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      311 2023-03-08 18:09:53.000000 otree-6.0.0a9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 16:33:52.109933 otree-6.0.0a9/setup.cfg
+-rw-rw-rw-   0        0        0     2548 2023-03-08 18:09:53.000000 otree-6.0.0a9/setup.py
```

### Comparing `otree-6.0.0a8/LICENSE` & `otree-6.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/PKG-INFO` & `otree-6.0.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otree
-Version: 6.0.0a8
+Version: 6.0.0a9
 Summary: Framework for multiplayer strategy games and complex surveys.
 Home-page: http://otree.org/
 Author: chris@otree.org
 Author-email: chris@otree.org
 License: MIT License
 Platform: UNKNOWN
 Provides-Extra: mturk
```

### Comparing `otree-6.0.0a8/README.rst` & `otree-6.0.0a9/README.rst`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/api.py` & `otree-6.0.0a9/otree/api.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/api.pyi` & `otree-6.0.0a9/otree/api.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -386,9 +386,9 @@
     "WaitPage",
     "Page",
     "Bot",
     "Submission",
     "SubmissionMustFail",
     "expect",
     "read_csv",
-    # "url_of_static_file",
+    "url_of_static_file",
 ]
```

### Comparing `otree-6.0.0a8/otree/app_template/__pycache__/models.cpython-36.pyc` & `otree-6.0.0a9/otree/app_template/__pycache__/models.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/app_template/__pycache__/models.cpython-37.pyc` & `otree-6.0.0a9/otree/app_template/__pycache__/models.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/app_template/__pycache__/tests.cpython-36.pyc` & `otree-6.0.0a9/otree/app_template/__pycache__/tests.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/app_template/_builtin/__pycache__/__init__.cpython-36.pyc` & `otree-6.0.0a9/otree/app_template/_builtin/__pycache__/__init__.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/app_template/_builtin/__pycache__/__init__.cpython-37.pyc` & `otree-6.0.0a9/otree/app_template/_builtin/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/asgi.py` & `otree-6.0.0a9/otree/asgi.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/bots/bot.py` & `otree-6.0.0a9/otree/bots/bot.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/bots/browser.py` & `otree-6.0.0a9/otree/bots/browser.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/bots/browser_launcher.py` & `otree-6.0.0a9/otree/bots/browser_launcher.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/bots/runner.py` & `otree-6.0.0a9/otree/bots/runner.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/channels/consumers.py` & `otree-6.0.0a9/otree/channels/consumers.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/channels/routing.py` & `otree-6.0.0a9/otree/channels/routing.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/channels/utils.py` & `otree-6.0.0a9/otree/channels/utils.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/chat.py` & `otree-6.0.0a9/otree/chat.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/checks.py` & `otree-6.0.0a9/otree/checks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,60 @@
 import inspect
 import os
 from importlib import import_module
 from pathlib import Path
 import sys
 from otree import common
-from otree.api import BasePlayer, BaseGroup, BaseSubsession, Currency, WaitPage, ExtraModel
+from otree.api import (
+    BasePlayer,
+    BaseGroup,
+    BaseSubsession,
+    Currency,
+    WaitPage,
+    ExtraModel,
+)
 from otree.views.abstract import Page
 from otree import settings
 from otree.common import get_pages_module, get_models_module, get_builtin_constant
 from collections import namedtuple
 
 Error = namedtuple(
     'Error',
     [
+        'app_name',
         'title',
         'id',
+    ],
+)
+Warning = namedtuple(
+    'Warning',
+    [
         'app_name',
+        'title',
+        'id',
     ],
 )
-Warning = namedtuple('Warning', ['title', 'id', 'app_name'])
 
 print_function = print
 
 
 class AppCheckHelper:
     def __init__(self, app_name):
         self.app_name = app_name
         self.path = Path(app_name)
         self.errors = []
         self.warnings = []
 
     def add_error(self, title, numeric_id: int):
-        self.errors.append(Error(title, id=numeric_id, app_name=self.app_name))
+        self.errors.append(Error(title=title, id=numeric_id, app_name=self.app_name))
 
     def add_warning(self, title, numeric_id: int):
-        self.warnings.append(Warning(title, id=numeric_id, app_name=self.app_name))
+        self.warnings.append(
+            Warning(title=title, id=numeric_id, app_name=self.app_name)
+        )
 
     def get_template_names(self):
         templates_dir = self.path / 'templates'
         for root, dirs, files in os.walk(templates_dir):
             for name in files:
                 if name.endswith('.html'):
                     yield templates_dir.joinpath(root, name)
@@ -244,15 +260,24 @@
                             'You should instead define a top-level function called group_by_arrival_time_method. '
                             ''.format(ViewCls.__name__),
                             numeric_id=25,
                         )
             elif issubclass(ViewCls, Page):
                 if ViewCls.has_trial():
                     Trial = ViewCls.trial_model
-                    #if not isinstance(Trial, ExtraModel):
+                    for fn in ViewCls.trial_stimulus_fields + getattr(
+                        ViewCls, 'trial_response_fields', []
+                    ):
+                        if not hasattr(Trial, fn):
+                            helper.add_error(
+                                f"Page '{ViewCls.__name__}' includes '{fn}' in its trial fields, "
+                                f"but this is not a field on the '{Trial.__name__}' model.",
+                                numeric_id=27,
+                            )
+                    # if not isinstance(Trial, ExtraModel):
                     #    helper.add_error()
             else:
                 msg = '"{}" is not a valid page'.format(ViewCls)
                 helper.add_error(msg, numeric_id=26)
 
 
 def get_checks_output(app_names=None):
```

### Comparing `otree-6.0.0a8/otree/cli/base.py` & `otree-6.0.0a9/otree/cli/base.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/cli/bots.py` & `otree-6.0.0a9/otree/cli/bots.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/cli/browser_bots.py` & `otree-6.0.0a9/otree/cli/browser_bots.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/cli/create_session.py` & `otree-6.0.0a9/otree/cli/create_session.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/cli/devserver.py` & `otree-6.0.0a9/otree/cli/devserver.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/cli/devserver_inner.py` & `otree-6.0.0a9/otree/cli/devserver_inner.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/cli/prodserver1of2.py` & `otree-6.0.0a9/otree/cli/prodserver1of2.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/cli/remove_self.py` & `otree-6.0.0a9/otree/cli/remove_self.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/cli/resetdb.py` & `otree-6.0.0a9/otree/cli/resetdb.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/cli/startapp.py` & `otree-6.0.0a9/otree/cli/startapp.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/cli/startproject.py` & `otree-6.0.0a9/otree/cli/startproject.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/cli/unzip.py` & `otree-6.0.0a9/otree/cli/unzip.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/cli/upcase_constants.py` & `otree-6.0.0a9/otree/cli/upcase_constants.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/cli/update_my_code.py` & `otree-6.0.0a9/otree/cli/update_my_code.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/cli/zip.py` & `otree-6.0.0a9/otree/cli/zip.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/cli/zipserver.py` & `otree-6.0.0a9/otree/cli/zipserver.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/common.py` & `otree-6.0.0a9/otree/common.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/common2.py` & `otree-6.0.0a9/otree/common2.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,26 +121,31 @@
 
 
 existing_filenames_cache = set()
 
 
 def url_of_static_file(path):
     """
+    - better than hardcoding '/static/', which will fail silently if the file
+    doesn't exist.
+    - there is the {{ static }} tag in templates.
+      good to have this in python code for consistency,
+      rather than making people construct it manually.
+    - useful for:
+        - Trials, which are generated on the server side.
+          this would be useful for 2 situations:
+        - live pages, where {% static %} can't be used because the template was already rendered
+        - js_vars (don't want {% static %} mixed in with JS code)
+
     naming:
     - it shouldn't start with
     'static' because that would distract from @staticmethod in autocomplete,
     which is much more important.
     - url_of_static is more specific than url_for_static (which looks like vars_for_template but works differently)
 
-    better than hardcoding '/static/', which will fail silently if the file
-    doesn't exist.
-
-    this would be useful for 2 situations:
-    - live pages, where {% static %} can't be used because the template was already rendered
-    - for use with js_vars (don't want {% static %} mixed in with JS code)
     """
     from otree.asgi import app
 
     static_files_app.assert_file_exists(path)
     return app.router.url_path_for('static', path=path)
```

### Comparing `otree-6.0.0a8/otree/constants.py` & `otree-6.0.0a9/otree/constants.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/currency.py` & `otree-6.0.0a9/otree/currency.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/database.py` & `otree-6.0.0a9/otree/database.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/errorpage.py` & `otree-6.0.0a9/otree/errorpage.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/export.py` & `otree-6.0.0a9/otree/export.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/forms/fields.py` & `otree-6.0.0a9/otree/forms/fields.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/forms/forms.py` & `otree-6.0.0a9/otree/forms/forms.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/forms/widgets.py` & `otree-6.0.0a9/otree/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/i18n.py` & `otree-6.0.0a9/otree/i18n.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/live.py` & `otree-6.0.0a9/otree/live.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/ar/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/ar/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/cs/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/cs/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/de/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/de/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/django.pot` & `otree-6.0.0a9/otree/locale/django.pot`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/es/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/es/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/fi/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/fr/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/fr/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/he/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/he/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/hi/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/hi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/hi/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/hi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/hu/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/hu/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/id/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/id/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/it/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/it/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/ja/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/ja/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/ko/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/ko/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/nb/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/nb/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/nl/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/nl/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/pl/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/pl/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/pt/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/pt/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/ru/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/ru/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/tr/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/tr/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/zh_Hans/LC_MESSAGES/django.mo` & `otree-6.0.0a9/otree/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/locale/zh_Hans/LC_MESSAGES/django.po` & `otree-6.0.0a9/otree/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/lookup.py` & `otree-6.0.0a9/otree/lookup.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/main.py` & `otree-6.0.0a9/otree/main.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/middleware.py` & `otree-6.0.0a9/otree/middleware.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/models/group.py` & `otree-6.0.0a9/otree/models/group.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/models/participant.py` & `otree-6.0.0a9/otree/models/participant.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/models/player.py` & `otree-6.0.0a9/otree/models/player.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/models/session.py` & `otree-6.0.0a9/otree/models/session.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/models/subsession.py` & `otree-6.0.0a9/otree/models/subsession.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/models_concrete.py` & `otree-6.0.0a9/otree/models_concrete.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/mturk_client.py` & `otree-6.0.0a9/otree/mturk_client.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/patch.py` & `otree-6.0.0a9/otree/patch.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/project_template/settings.py` & `otree-6.0.0a9/otree/project_template/settings.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/read_csv.py` & `otree-6.0.0a9/otree/read_csv.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/room.py` & `otree-6.0.0a9/otree/room.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/session.py` & `otree-6.0.0a9/otree/session.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/settings.py` & `otree-6.0.0a9/otree/settings.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/bootstrap5/css/bootstrap.min.css` & `otree-6.0.0a9/otree/static/bootstrap5/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/bootstrap5/css/bootstrap.min.css.map` & `otree-6.0.0a9/otree/static/bootstrap5/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/bootstrap5/js/bootstrap.bundle.min.js` & `otree-6.0.0a9/otree/static/bootstrap5/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/bootstrap5/js/bootstrap.bundle.min.js.map` & `otree-6.0.0a9/otree/static/bootstrap5/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/glyphicons/clock.png` & `otree-6.0.0a9/otree/static/glyphicons/clock.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/glyphicons/cloud.png` & `otree-6.0.0a9/otree/static/glyphicons/cloud.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/glyphicons/cogwheel.png` & `otree-6.0.0a9/otree/static/glyphicons/cogwheel.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/glyphicons/delete.png` & `otree-6.0.0a9/otree/static/glyphicons/delete.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/glyphicons/download-alt.png` & `otree-6.0.0a9/otree/static/glyphicons/download-alt.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/glyphicons/eye-open.png` & `otree-6.0.0a9/otree/static/glyphicons/eye-open.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/glyphicons/folder-closed.png` & `otree-6.0.0a9/otree/static/glyphicons/folder-closed.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/glyphicons/link.png` & `otree-6.0.0a9/otree/static/glyphicons/link.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/glyphicons/list-alt.png` & `otree-6.0.0a9/otree/static/glyphicons/list-alt.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/glyphicons/pencil.png` & `otree-6.0.0a9/otree/static/glyphicons/pencil.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/glyphicons/plus.png` & `otree-6.0.0a9/otree/static/glyphicons/plus.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/glyphicons/pushpin.png` & `otree-6.0.0a9/otree/static/glyphicons/pushpin.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/glyphicons/refresh.png` & `otree-6.0.0a9/otree/static/glyphicons/refresh.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/glyphicons/stats.png` & `otree-6.0.0a9/otree/static/glyphicons/stats.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/glyphicons/usd.png` & `otree-6.0.0a9/otree/static/glyphicons/usd.png`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/otree/css/table.css` & `otree-6.0.0a9/otree/static/otree/css/table.css`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/otree/css/theme.css` & `otree-6.0.0a9/otree/static/otree/css/theme.css`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/otree/js/common.js` & `otree-6.0.0a9/otree/static/otree/js/common.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/otree/js/formInputs.js` & `otree-6.0.0a9/otree/static/otree/js/formInputs.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/otree/js/jquery-3.2.1.min.js` & `otree-6.0.0a9/otree/static/otree/js/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/otree/js/jquery.color-2.1.2.min.js` & `otree-6.0.0a9/otree/static/otree/js/jquery.color-2.1.2.min.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/otree/js/jquery.countdown.min.js` & `otree-6.0.0a9/otree/static/otree/js/jquery.countdown.min.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/otree/js/jquery.timeago.en-short.js` & `otree-6.0.0a9/otree/static/otree/js/jquery.timeago.en-short.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/otree/js/jquery.timeago.js` & `otree-6.0.0a9/otree/static/otree/js/jquery.timeago.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/otree/js/live.js` & `otree-6.0.0a9/otree/static/otree/js/live.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/otree/js/monitor2.js` & `otree-6.0.0a9/otree/static/otree/js/monitor2.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/otree/js/otree-front.js` & `otree-6.0.0a9/otree/static/otree/js/otree-front.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -925,14 +925,18 @@
     function getMeasurement() {
         let name = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : "response";
         return get(name);
     }
 
     function init$1() {
         window._trialSocket.onmessage = function(message) {
+            console.log('trialSocket received', message.data);
+            console.log({
+                _TRIALS_SSE
+            });
             let data = JSON.parse(message.data);
             if (data.type === 'error') {
                 console.error("An error occurred processing a trial on the server.");
             } else if (_TRIALS_SSE) {
                 _onServerRecvSSE(data);
             } else if (data.type === 'load') {
                 _onServerRecvCSE(data);
@@ -954,16 +958,19 @@
     function _onServerRecvSSE(_ref2) {
         let {
             is_page_load,
             feedback,
             trial,
             progress
         } = _ref2;
-        page.nextTrial = trial;
+        // users might use .nextTrial with some slightly different semantics,
+        // don't want to clash with that.
+        page._nextTrial = trial;
         page.progress = progress;
+        console.log('server recv', _ref2);
         if (is_page_load) {
             emitEvent('load');
         } else {
             page.feedback = feedback;
             completeTrial();
         }
     }
@@ -985,15 +992,15 @@
 
     function getPlayableTrial() {
         // in roundtrip mode, we determine whether we're finished by whether
         // the trial received from the server is non-null.
         // in non-roundrip mode, we look at the progress.completed attribute.
 
         if (_TRIALS_SSE) {
-            return page.nextTrial;
+            return page._nextTrial;
         } else {
             if (page.progress.completed < TRIALS.length) {
                 return TRIALS[page.progress.completed];
             }
         }
     }
```

### Comparing `otree-6.0.0a8/otree/static/otree/js/page-websocket-redirect.js` & `otree-6.0.0a9/otree/static/otree/js/page-websocket-redirect.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/otree/js/reconnecting-websocket-iife.min.js` & `otree-6.0.0a9/otree/static/otree/js/reconnecting-websocket-iife.min.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/otree/js/table-utils.js` & `otree-6.0.0a9/otree/static/otree/js/table-utils.js`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/static/otree/js/trial-default.js` & `otree-6.0.0a9/otree/static/otree/js/trial-default.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -2,16 +2,19 @@
 ot.onLoad(function() {
     ot.freezeInputs();
     ot.startIteration();
 });
 
 ot.onIteration(function() {
     delete ot.page.trial;
-    delete ot.page.response;
     delete ot.page.feedback;
+    // should we automatically delete response? doesn't seem good
+    // to special-case this variable name.
+    delete ot.page.response;
+
 
     let nextTrial = ot.getPlayableTrial();
     if (nextTrial) {
         ot.startTrial(nextTrial);
     } else {
         ot.completePage();
     }
@@ -24,10 +27,9 @@
 
 // don't pass feedback to onCompleteTrial.
 // the user should set ot.page.feedback in onInput or somewhere else.
 // this makes it easier to handle both half-live and full-live mode.
 ot.onComplete(function() {
     ot.delay(window.TRIAL_DELAY || 0, function() {
         ot.startIteration();
-        console.log('did startIteration', ot.page.progress.completed);
     });
 });
```

### Comparing `otree-6.0.0a8/otree/tasks.py` & `otree-6.0.0a9/otree/tasks.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/AdminReport.html` & `otree-6.0.0a9/otree/templates/otree/AdminReport.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/Base.html` & `otree-6.0.0a9/otree/templates/otree/Base.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/BaseAdmin.html` & `otree-6.0.0a9/otree/templates/otree/BaseAdmin.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/CreateDemoSession.html` & `otree-6.0.0a9/otree/templates/otree/CreateDemoSession.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/DemoIndex.html` & `otree-6.0.0a9/otree/templates/otree/DemoIndex.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/Export.html` & `otree-6.0.0a9/otree/templates/otree/Export.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/Login.html` & `otree-6.0.0a9/otree/templates/otree/Login.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/MTurkCreateHIT.html` & `otree-6.0.0a9/otree/templates/otree/MTurkCreateHIT.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/MTurkHTMLQuestion.html` & `otree-6.0.0a9/otree/templates/otree/MTurkHTMLQuestion.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/MTurkSessionPayments.html` & `otree-6.0.0a9/otree/templates/otree/MTurkSessionPayments.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/Page.html` & `otree-6.0.0a9/otree/templates/otree/Page.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/RoomInputLabel.html` & `otree-6.0.0a9/otree/templates/otree/RoomInputLabel.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/RoomWithSession.html` & `otree-6.0.0a9/otree/templates/otree/RoomWithSession.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/RoomWithoutSession.html` & `otree-6.0.0a9/otree/templates/otree/RoomWithoutSession.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/ServerCheck.html` & `otree-6.0.0a9/otree/templates/otree/ServerCheck.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/Session.html` & `otree-6.0.0a9/otree/templates/otree/Session.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/SessionData.html` & `otree-6.0.0a9/otree/templates/otree/SessionData.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/SessionMonitor.html` & `otree-6.0.0a9/otree/templates/otree/SessionMonitor.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/SessionPayments.html` & `otree-6.0.0a9/otree/templates/otree/SessionPayments.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/SessionSplitScreen.html` & `otree-6.0.0a9/otree/templates/otree/SessionSplitScreen.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/SessionStartLinks.html` & `otree-6.0.0a9/otree/templates/otree/SessionStartLinks.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/Sessions.html` & `otree-6.0.0a9/otree/templates/otree/Sessions.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/WaitPage.html` & `otree-6.0.0a9/otree/templates/otree/WaitPage.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/includes/CreateSessionForm.html` & `otree-6.0.0a9/otree/templates/otree/includes/CreateSessionForm.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/includes/RoomParticipantLinks.html` & `otree-6.0.0a9/otree/templates/otree/includes/RoomParticipantLinks.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/includes/TimeLimit.js.html` & `otree-6.0.0a9/otree/templates/otree/includes/TimeLimit.js.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/includes/debug_info.html` & `otree-6.0.0a9/otree/templates/otree/includes/debug_info.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/includes/hidden_form_errors.html` & `otree-6.0.0a9/otree/templates/otree/includes/hidden_form_errors.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/includes/mturk_payment_table.html` & `otree-6.0.0a9/otree/templates/otree/includes/mturk_payment_table.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templates/otree/tags/chat.html` & `otree-6.0.0a9/otree/templates/otree/tags/chat.html`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templating/compiler.py` & `otree-6.0.0a9/otree/templating/compiler.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templating/context.py` & `otree-6.0.0a9/otree/templating/context.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templating/errors.py` & `otree-6.0.0a9/otree/templating/errors.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templating/filters.py` & `otree-6.0.0a9/otree/templating/filters.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templating/loader.py` & `otree-6.0.0a9/otree/templating/loader.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templating/nodes.py` & `otree-6.0.0a9/otree/templating/nodes.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templating/template.py` & `otree-6.0.0a9/otree/templating/template.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/templating/utils.py` & `otree-6.0.0a9/otree/templating/utils.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/trial.py` & `otree-6.0.0a9/otree/trial.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from otree.database import NoResultFound
 
 logger = logging.getLogger(__name__)
 
 
 async def trial_payload_function(participant_code, page_name, msg):
 
-    # print('in trial_payload_function', msg)
+    print('in trial_payload_function', msg)
     try:
         participant = Participant.objects_get(code=participant_code)
     except NoResultFound:
         logger.warning(f'Participant not found: {participant_code}')
         return
 
     def send_error():
@@ -64,15 +64,16 @@
             server_fields = set(PageClass.trial_response_fields)
             client_fields = response.keys()
             server_only = server_fields - client_fields
             if server_only:
                 await send_error()
                 msg = (
                     "The following fields are in trial_response_fields, "
-                    f"but were not sent from sendTrialResponse: {server_only}"
+                    f"but were not received from sendTrialResponse: {server_only}. "
+                    "If this key was indeed sent, make sure its value is non-null."
                 )
                 raise Exception(msg)
             client_only = client_fields - server_fields
             if client_only:
                 await send_error()
                 msg = (
                     "The following fields were sent from the sendTrialResponse, "
```

### Comparing `otree-6.0.0a8/otree/update.py` & `otree-6.0.0a9/otree/update.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/urls.py` & `otree-6.0.0a9/otree/urls.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/views/abstract.py` & `otree-6.0.0a9/otree/views/abstract.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,1268 +1,1268 @@
-import inspect
-import logging
-import time
-import typing
-from html import escape
-from pathlib import Path
-from typing import List
-from typing import Optional
-
-import starlette.exceptions
-from starlette.concurrency import run_in_threadpool
-from starlette.datastructures import FormData as StarletteFormData
-from starlette.requests import Request
-from starlette.responses import RedirectResponse, HTMLResponse
-from starlette.types import Receive, Scope, Send
-
-# this is an expensive import
-import otree.bots.browser as browser_bots
-import otree.channels.utils as channel_utils
-import otree.common
-import otree.common2
-import otree.constants
-from otree.currency import json_dumps
-import otree.forms
-import otree.models
-import otree.tasks
-import otree.views.cbv
-from otree import settings
-from otree.bots.bot import bot_prettify_post_data
-from otree.common import (
-    get_app_label_from_import_path,
-    get_dotted_name,
-    get_admin_secret_code,
-    DebugTable,
-    BotError,
-    NON_FIELD_ERROR_KEY,
-    get_constants,
-)
-from otree.database import db, dbq
-from otree.forms.forms import get_form
-from otree.i18n import core_gettext
-from otree.lookup import get_min_idx_for_app, get_page_lookup
-from otree.models import Participant, Session, BaseGroup, BaseSubsession
-from otree.models_concrete import (
-    CompletedSubsessionWaitPage,
-    CompletedGroupWaitPage,
-    CompletedGBATWaitPage,
-)
-import otree.trial
-from otree.templating import render
-
-logger = logging.getLogger(__name__)
-
-
-ADMIN_SECRET_CODE = get_admin_secret_code()
-
-
-BOT_COMPLETE_HTML_MESSAGE = '''
-<html>
-    <head>
-        <title>Bot completed</title>
-    </head>
-    <body>Bot completed</body>
-</html>
-'''
-
-
-class FormPageOrInGameWaitPage:
-    request: Request
-
-    @classmethod
-    def instantiate_without_request(cls):
-        return cls({'type': 'http'}, None, None)
-
-    def __init__(self, scope: Scope, receive: Receive, send: Send) -> None:
-        assert scope["type"] == "http"
-        self.scope = scope
-        self.receive = receive
-        self.send = send
-
-    def __await__(self) -> typing.Generator:
-        return self.dispatch().__await__()
-
-    def call_user_defined(self, method_name, *args, **kwargs):
-        """
-        the default user-defined methods should not reference self, so they can work
-        both as Player methods and Page methods.
-        """
-        if self.is_noself:
-            return getattr(type(self), method_name)(self.player, *args, **kwargs)
-        return getattr(self, method_name)(*args, **kwargs)
-
-    async def dispatch(self) -> None:
-        self.request = request = Request(self.scope, receive=self.receive)
-        participant_code = request.path_params['participant_code']
-        msg = (
-            "This user does not exist in the database. " "Maybe the database was reset."
-        )
-        participant = db.get_or_404(Participant, code=participant_code, msg=msg)
-
-        # if the player tried to skip past a part of the subsession
-        # (e.g. by typing in a future URL)
-        # or if they hit the back button to a previous subsession
-        # in the sequence.
-        url_should_be_on = participant._url_i_should_be_on()
-        if not request.url.path == url_should_be_on:
-            response = RedirectResponse(url_should_be_on, status_code=302)
-        else:
-            self.set_attributes(participant)
-            # need to await the form from async function, otherwise run into complicated RuntimeError
-            try:
-                if request.method == 'POST':
-                    self._form_data = await self.request.form()
-            except starlette.requests.ClientDisconnect:
-                # just make an empty response, to avoid
-                # "RuntimeError: No response returned"
-                response = starlette.responses.Response()
-            else:
-                response = await run_in_threadpool(self.inner_dispatch, request)
-        await response(self.scope, self.receive, self.send)
-
-    template_name = None
-
-    is_debug = settings.DEBUG
-
-    def inner_dispatch(self, request):
-        '''inner dispatch function'''
-        raise NotImplementedError()
-
-    def get_template_name(self):
-        raise NotImplementedError()
-
-    @classmethod
-    def url_pattern(cls, name_in_url):
-        p = '/p/{participant_code}/%s/%s/{page_index}' % (name_in_url, cls.__name__)
-        return p
-
-    @classmethod
-    def get_url(cls, participant_code, name_in_url, page_index):
-        '''need this because reverse() is too slow in create_session'''
-        # if i change this URL pattern, i should also change assert_correct_page()
-        # in bot.py
-        return f'/p/{participant_code}/{name_in_url}/{cls.__name__}/{page_index}'
-
-    @classmethod
-    def url_name(cls):
-        '''using dots seems not to work'''
-        return get_dotted_name(cls).replace('.', '-')
-
-    def _redirect_to_page_the_user_should_be_on(self):
-        return RedirectResponse(self.participant._url_i_should_be_on(), status_code=302)
-
-    @classmethod
-    def has_trial(cls):
-        return bool(getattr(cls, 'trial_model', None))
-
-    def get_context_data(self, **context):
-
-        context.update(
-            view=self,
-            object=getattr(self, 'object', None),
-            player=self.player,
-            group=self.group,
-            subsession=self.subsession,
-            session=self.session,
-            participant=self.participant,
-            timer_text=getattr(self, 'timer_text', None),
-            current_page_name=self.__class__.__name__,
-            has_live_method=bool(getattr(self, 'live_method', None)),
-            has_trial=self.has_trial(),
-        )
-
-        Constants = self._Constants
-        # it could be called C or Constants
-        context[Constants.__name__] = Constants
-
-        vars_for_template = {}
-
-        user_vars = self.call_user_defined('vars_for_template')
-        user_vars = user_vars or {}
-        if not isinstance(user_vars, dict):
-            raise Exception('vars_for_template did not return a dict')
-
-        js_vars = self.call_user_defined('js_vars')
-
-        try:
-            # better to convert to json here so we can catch any errors,
-            # rather than applying the filter in the template.
-            context['js_vars'] = json_dumps(js_vars)
-        except TypeError as exc:
-            raise TypeError(f'js_vars contains an invalid value; {exc}') from None
-
-        has_trial = self.has_trial()
-        if has_trial:
-            Trial = self.trial_model
-            use_roundtrip_mode = hasattr(self, 'evaluate_trial')
-            if use_roundtrip_mode:
-                trials = []
-            else:
-                trials = [
-                    otree.trial.encode_trial(t, self.trial_stimulus_fields)
-                    for t in Trial.filter(player=self.player)
-                ]
-            context['trials_json'] = json_dumps(trials)
-            context['_trials_use_roundtrip_mode'] = json_dumps(use_roundtrip_mode)
-
-        vars_for_template.update(user_vars)
-
-        context.update(vars_for_template)
-
-        if settings.DEBUG:
-            self.debug_tables = self._get_debug_tables(vars_for_template)
-        return context
-
-    def render_to_response(self, context):
-        return render(
-            self.get_template_name(), context, template_type=self._template_type
-        )
-
-    _template_type = None
-
-    def vars_for_template(self):
-        return {}
-
-    def js_vars(self):
-        return {}
-
-    def _get_debug_tables(self, vars_for_template):
-
-        tables = []
-        if vars_for_template:
-            # use repr() so that we can distinguish strings from numbers
-            # and can see currency types, etc.
-            items = [(k, escape(repr(v))) for (k, v) in vars_for_template.items()]
-            rows = sorted(items)
-            tables.append(DebugTable(title='vars_for_template', rows=rows))
-
-        player = self.player
-        participant = self.participant
-        basic_info_table = DebugTable(
-            title='Basic info',
-            rows=[
-                ('ID in group', player.id_in_group),
-                ('Group', player.group_id),
-                ('Round number', player.round_number),
-                ('Participant', participant._numeric_label()),
-                ('Participant label', participant.label or ''),
-                ('Session code', participant._session_code),
-            ],
-        )
-
-        tables.append(basic_info_table)
-
-        return tables
-
-    def _is_displayed(self):
-        return self.call_user_defined('is_displayed')
-
-    @property
-    def group(self) -> BaseGroup:
-        '''can't cache self._group_pk because group can change'''
-        return self.player.group
-
-    @property
-    def subsession(self) -> BaseSubsession:
-        '''so that it doesn't rely on player'''
-        # this goes through idmap cache, so no perf hit
-        return self.SubsessionClass.objects_get(id=self._subsession_pk)
-
-    @property
-    def session(self) -> Session:
-        return Session.objects_get(id=self._session_pk)
-
-    def set_attributes(self, participant):
-
-        lookup = get_page_lookup(participant._session_code, participant._index_in_pages)
-        self._lookup = lookup
-
-        app_name = lookup.app_name
-
-        models_module = otree.common.get_models_module(app_name)
-
-        self._Constants = get_constants(app_name)
-        self.PlayerClass = getattr(models_module, 'Player')
-        self.GroupClass = getattr(models_module, 'Group')
-        self.SubsessionClass = getattr(models_module, 'Subsession')
-        self.player = self.PlayerClass.objects_get(
-            participant=participant, round_number=lookup.round_number
-        )
-        self._subsession_pk = lookup.subsession_id
-        self.round_number = lookup.round_number
-        self._session_pk = lookup.session_pk
-        # simpler if we set it directly so that we can do tests without idmap cache
-        self._participant_pk = participant.id
-        # setting it directly makes testing easier (tests dont need to use cache)
-        self.participant: Participant = participant
-
-        # it's already validated that participant is on right page
-        self._index_in_pages = participant._index_in_pages
-
-        # for the participant changelist
-        participant._current_app_name = app_name
-        participant._current_page_name = self.__class__.__name__
-        participant._last_request_timestamp = int(time.time())
-        participant._round_number = lookup.round_number
-
-    def set_attributes_waitpage_clone(self, *, original_view: 'WaitPage'):
-        '''put it here so it can be compared with set_attributes...
-        but this is really just a method on wait pages'''
-        # make a clean copy for AAPA
-        # self.player and self.participant etc are undefined
-        # and no objects are cached inside it
-        # and it doesn't affect the current instance
-
-        self._Constants = original_view._Constants
-        self.GroupClass = original_view.GroupClass
-        self.SubsessionClass = original_view.SubsessionClass
-        self._subsession_pk = original_view._subsession_pk
-        self._session_pk = original_view._session_pk
-        self.round_number = original_view.round_number
-
-    def _increment_index_in_pages(self):
-        # when is this not the case?
-        participant = self.participant
-        assert self._index_in_pages == participant._index_in_pages
-
-        # we should allow a user to move beyond the last page if it's mturk
-        # also in general maybe we should show the 'out of sequence' page
-
-        # we skip any page that is a sequence page where is_displayed
-        # evaluates to False to eliminate unnecessary redirection
-
-        page_index_to_skip_to = self._get_next_page_index_if_skipping_apps()
-        is_skipping_apps = bool(page_index_to_skip_to)
-
-        for page_index in range(
-            # go to max_page_index+2 because range() skips the last index
-            # and it's possible to go to max_page_index + 1 (OutOfRange)
-            self._index_in_pages + 1,
-            participant._max_page_index + 2,
-        ):
-            participant._index_in_pages = page_index
-            if page_index == participant._max_page_index + 1:
-                # break and go to OutOfRangeNotification
-                break
-            if is_skipping_apps and page_index == page_index_to_skip_to:
-                break
-
-            # scope, receive, send
-            page = get_page_lookup(
-                participant._session_code, page_index
-            ).page_class.instantiate_without_request()
-
-            page.set_attributes(self.participant)
-            if not is_skipping_apps and page._is_displayed():
-                break
-
-            # if it's a wait page, record that they visited
-            if isinstance(page, WaitPage):
-
-                if page.group_by_arrival_time:
-                    # keep looping
-                    # if 1 participant can skip the page,
-                    # then all other participants should skip it also,
-                    # as described in the docs
-                    # so there is no need to mark as complete.
-                    continue
-
-                # save the participant, because tally_unvisited
-                # queries index_in_pages directly from the DB
-                db.commit()
-
-                is_last, someone_waiting = page._tally_unvisited()
-                if is_last and someone_waiting:
-                    page._run_aapa_and_notify(page._group_or_subsession)
-
-    def is_displayed(self):
-        return True
-
-    def _update_monitor_table(self):
-        self.participant._update_monitor_table()
-
-    def _get_next_page_index_if_skipping_apps(self):
-        # don't run it if the page is not displayed, because:
-        # (1) it's consistent with other functions like before_next_page, vars_for_template
-        # (2) then when we do
-        # a lookahead skipping pages, we would need to check each page if it
-        # has app_after_this_page defined, then set attributes and run it.
-        # what if we are already skipping to a future app, then another page
-        # has app_after_this_page? does it override the first one?
-        if not self._is_displayed():
-            return
-        if not hasattr(self, 'app_after_this_page'):
-            return
-
-        current_app = self.participant._current_app_name
-        app_sequence = self.session.config['app_sequence']
-        current_app_index = app_sequence.index(current_app)
-        upcoming_apps = app_sequence[current_app_index + 1 :]
-
-        app_to_skip_to = self.call_user_defined('app_after_this_page', upcoming_apps)
-        if app_to_skip_to:
-            if app_to_skip_to not in upcoming_apps:
-                msg = f'"{app_to_skip_to}" is not in the upcoming_apps list'
-                raise InvalidAppError(msg)
-            return get_min_idx_for_app(self.participant._session_code, app_to_skip_to)
-
-    def _record_page_completion_time(self):
-        now = int(time.time())
-        participant = self.participant
-
-        session_code = participant._session_code
-
-        otree.common2.make_page_completion_row(
-            view=self,
-            app_name=self.player.get_folder_name(),
-            participant__id_in_session=participant.id_in_session,
-            participant__code=participant.code,
-            session_code=session_code,
-            is_wait_page=0,
-        )
-
-        participant._last_page_timestamp = now
-
-    def live_url(self):
-        return channel_utils.live_path(
-            participant_code=self.participant.code,
-            page_name=type(self).__name__,
-            page_index=self._index_in_pages,
-            session_code=self.participant._session_code,
-        )
-
-    def trial_url(self):
-        return channel_utils.trial_path(
-            participant_code=self.participant.code,
-            page_name=type(self).__name__,
-            page_index=self._index_in_pages,
-        )
-
-    live_method = ''
-
-
-class Page(FormPageOrInGameWaitPage):
-    form_model = None
-    form_fields = []
-
-    _template_type = 'Page'
-
-    def inner_dispatch(self, request):
-        if request.method == 'POST':
-            return self.post()
-        return self.get()
-
-    def browser_bot_stuff(self, response: HTMLResponse):
-        """we use this hack of appending to the HTML, rather than sending a context var,
-        because we don't know if we need to submit the page until we try enqueueing the next post data.
-        i guess that can't be done until we have the HTML of the page.
-        """
-        if self.participant.is_browser_bot:
-            browser_bots.set_attributes(
-                participant_code=self.participant.code,
-                request_path=self.request.url.path,
-                html=response.body.decode('utf-8'),
-            )
-            has_next_submission = browser_bots.enqueue_next_post_data(
-                participant_code=self.participant.code
-            )
-            if has_next_submission:
-                # this doesn't work because we also would need to do this on OutOfRange page.
-                # sometimes the player submits the last page, especially during development.
-                # if self._index_in_pages == self.participant._max_page_index:
-                auto_submit_js = '''
-                <script>
-                    var form = document.querySelector('#form');
-                    form.submit();
-                    // browser-bot-auto-submit
-                    form.on('submit', function (e) {
-                        e.preventDefault();
-                    });
-                </script>
-                '''
-                extra_content = auto_submit_js.encode('utf8')
-                response.body += extra_content
-                response.headers['Content-Length'] = str(
-                    int(response.headers['Content-Length']) + len(extra_content)
-                )
-            else:
-                browser_bots.send_completion_message(
-                    session_code=self.participant._session_code,
-                    participant_code=self.participant.code,
-                )
-
-    def get(self):
-
-        if not self._is_displayed():
-            self._increment_index_in_pages()
-            return self._redirect_to_page_the_user_should_be_on()
-
-        # this needs to be set AFTER scheduling submit_expired_url,
-        # to prevent race conditions.
-        # see that function for an explanation.
-        # self.participant._current_form_page_url = self.request.url.path
-
-        self._update_monitor_table()
-
-        # 2020-07-10: maybe we should call vars_for_template before instantiating the form
-        # so that you can set initial value for a field in vars_for_template?
-        # No, i don't want to commit to that.
-        form = self.get_form_or_mockform()
-
-        context = self.get_context_data(form=form)
-        response = self.render_to_response(context)
-        self.browser_bot_stuff(response)
-        return response
-
-    def get_form_or_mockform(self):
-        if self.has_form():
-            obj = self.get_object()
-            return self.get_form(instance=obj)
-        else:
-            return MockForm()
-
-    def get_template_name(self):
-        if self.template_name is not None:
-            return self.template_name
-        return '{}/{}.html'.format(
-            get_app_label_from_import_path(self.__module__), self.__class__.__name__
-        )
-
-    def has_form(self):
-        return bool(self._get_form_fields())
-
-    def _get_form_fields(self):
-        if hasattr(self, 'get_form_fields'):
-            return self.call_user_defined('get_form_fields')
-        return self.form_fields
-
-    def get_object(self):
-        if not self.form_model:
-            msg = 'Page has form_fields but not form_model'
-            raise Exception(msg)
-        return {
-            'player': self.player,
-            'group': self.group,
-            self.PlayerClass: self.player,
-            self.GroupClass: self.group,
-        }[self.form_model]
-
-    def get_form(self, instance, formdata=None) -> otree.forms.forms.ModelForm:
-        fields = self._get_form_fields()
-        form = get_form(instance, field_names=fields, view=self, formdata=formdata)
-        return form
-
-    def form_invalid(self, form):
-        context = self.get_context_data(form=form)
-
-        fields_with_errors = [
-            fname for fname in form.errors if fname != NON_FIELD_ERROR_KEY
-        ]
-
-        # i think this should be before we call render_to_response
-        # because the view (self) is passed to the template and rendered
-        if fields_with_errors:
-            self.first_field_with_errors = fields_with_errors[0]
-            self.other_fields_with_errors = fields_with_errors[1:]
-
-        response = self.render_to_response(context)
-        response.headers[
-            otree.constants.redisplay_with_errors_http_header
-        ] = otree.constants.get_param_truth_value
-
-        return response
-
-    def must_complete_trials(self):
-        if self.timeout_happened:
-            return False
-        if self.has_trial():
-            Trial = self.trial_model
-            return bool(otree.trial.get_current_trial(Trial, self.player))
-        return False
-
-    def trials_incomplete_handler(self, form):
-        context = self.get_context_data(form=form, _trials_incomplete=True)
-        response = self.render_to_response(context)
-        response.headers[
-            otree.constants.redisplay_with_errors_http_header
-        ] = otree.constants.get_param_truth_value
-
-        return response
-
-    def _check_submission_must_fail(self, is_bot, post_data):
-        if is_bot and post_data.get('must_fail'):
-            msg = (
-                'Page "{}": Bot tried to submit intentionally invalid '
-                'data with '
-                'SubmissionMustFail, but it passed validation anyway:'
-                ' {}.'.format(
-                    self.__class__.__name__, bot_prettify_post_data(post_data)
-                )
-            )
-            raise BotError(msg)
-
-    def post_handle_form(self, post_data):
-        obj = self.get_object()
-        form = self.get_form(formdata=post_data, instance=obj)
-        self.form = form
-
-        if self.must_complete_trials():
-            return self.trials_incomplete_handler(form)
-
-        if self.timeout_happened:
-            self._process_auto_submitted_form(form, obj)
-        else:
-            is_bot = self.participant._is_bot
-            if form.validate():
-                self._check_submission_must_fail(is_bot, post_data)
-                form.populate_obj(obj)
-            else:
-                if is_bot:
-                    PageName = self.__class__.__name__
-                    if not post_data.get('must_fail'):
-                        errors = [
-                            "{}: {}".format(k, repr(v)) for k, v in form.errors.items()
-                        ]
-                        msg = (
-                            'Page "{}": Bot submission failed form validation: {} '
-                            'Check your bot code, '
-                            'then create a new session. '
-                            'Data submitted was: {}'.format(
-                                PageName, errors, bot_prettify_post_data(post_data)
-                            )
-                        )
-                        raise BotError(msg)
-                    if post_data.get('error_fields'):
-                        expected_error_fields = set(post_data.getlist('error_fields'))
-                        actual_error_fields = set(form.errors.keys())
-                        if not expected_error_fields == actual_error_fields:
-                            msg = (
-                                'Page {}, SubmissionMustFail: '
-                                'Expected error_fields were {}, but actual '
-                                'error_fields are {}'.format(
-                                    PageName, expected_error_fields, actual_error_fields
-                                )
-                            )
-                            raise BotError(msg)
-                response = self.form_invalid(form)
-                self.browser_bot_stuff(response)
-                return response
-
-    _form_data = None
-
-    def post(self):
-        post_data = self._form_data
-        auto_submitted = post_data.get(otree.constants.timeout_happened)
-        # if the page doesn't have a timeout_seconds, only the timeoutworker
-        # should be able to auto-submit it.
-        # otherwise users could append timeout_happened to the URL to skip pages
-        has_secret_code = (
-            post_data.get(otree.constants.admin_secret_code) == ADMIN_SECRET_CODE
-        )
-        # convert it to a bool so that you can do e.g.
-        # player.timeout_happened = timeout_happened
-        self.timeout_happened = bool(
-            auto_submitted and (has_secret_code or self._is_past_timeout())
-        )
-        if self.participant.is_browser_bot:
-            submission = browser_bots.pop_enqueued_post_data(
-                participant_code=self.participant.code
-            )
-
-            d = dict(post_data)
-            # normalize to string because wtforms gets confused when it receives
-            # string input, for example the int 0 does not pass InputRequired
-            # (but how about CLI bots?)
-            d.update({k: str(v) for k, v in submission.items()})
-            post_data = StarletteFormData(d)
-
-        if self.has_form():
-            resp = self.post_handle_form(post_data)
-            if resp:
-                return resp
-        elif self.must_complete_trials():
-            return self.trials_incomplete_handler(form=MockForm())
-        elif hasattr(self, 'error_message') and not self.timeout_happened:
-            # if the page has no form, we should still run error_message.
-            # this is useful for live pages.
-            # the code here is a stripped-down version of what happens with forms.
-            is_bot = self.participant._is_bot
-            error_message = self.call_user_defined('error_message', {})
-            if error_message:
-                if is_bot and not post_data.get('must_fail'):
-                    msg = (
-                        'Page "{}": Bot submission failed form validation: {} '
-                        'Check your bot code, '
-                        'then create a new session. '
-                    ).format(self.__class__.__name__, error_message)
-                    raise BotError(msg)
-                context = self.get_context_data(
-                    form=MockForm(error_message=error_message)
-                )
-                response = self.render_to_response(context)
-                response.headers[
-                    otree.constants.redisplay_with_errors_http_header
-                ] = otree.constants.get_param_truth_value
-                self.browser_bot_stuff(response)
-                return response
-            elif is_bot and post_data.get('must_fail'):
-                self._check_submission_must_fail(is_bot, post_data)
-
-        extra_args = (
-            dict(timeout_happened=self.timeout_happened) if self.is_noself else {}
-        )
-        self.call_user_defined('before_next_page', **extra_args)
-        self._record_page_completion_time()
-        self._increment_index_in_pages()
-        return self._redirect_to_page_the_user_should_be_on()
-
-    def before_next_page(self, timeout_happened=False):
-        pass
-
-    def socket_url(self):
-        '''called from template. can't start with underscore because used
-        in template
-        '''
-        return channel_utils.auto_advance_path(
-            participant_code=self.participant.code, page_index=self._index_in_pages
-        )
-
-    def _get_timeout_submission(self):
-        '''timeout_submission is deprecated'''
-        timeout_submission = self.timeout_submission or {}
-        for field_name in self._get_form_fields():
-            if field_name not in timeout_submission:
-                # get default value for datatype if the user didn't specify
-                ModelClass = type(self.get_object())
-                value = getattr(ModelClass, field_name).auto_submit_default
-                timeout_submission[field_name] = value
-        return timeout_submission
-
-    def _process_auto_submitted_form(self, form, obj):
-        '''
-        # an empty submitted form looks like this:
-        # {'f_currency': None, 'f_bool': None, 'f_int': None, 'f_char': ''}
-        '''
-        timeout_submission = self._get_timeout_submission()
-
-        # force the form to be cleaned
-        form.validate()
-
-        has_non_field_error = form.non_field_error
-
-        # If there is a timeout, we accept whatever fields don't have errors,
-        # so if there are errors, we have to call error_message manually,
-        # since error_message is only run if there are no
-        # field errors (because the error_message function assumes all fields exist)
-        if form.errors and not has_non_field_error:
-            if hasattr(self, 'error_message'):
-                try:
-                    has_non_field_error = bool(
-                        self.call_user_defined('error_message', form.data)
-                    )
-                except:
-                    has_non_field_error = True
-
-        if has_non_field_error:
-            # non-field errors exist.
-            # ignore form, use timeout_submission entirely
-            auto_submit_values_to_use = timeout_submission
-        elif form.errors:
-            auto_submit_values_to_use = {}
-            for field_name in form.errors:
-                auto_submit_values_to_use[field_name] = timeout_submission[field_name]
-            # save the fields without errors. we will overwrite the other fields with timeout_submission.
-            form.errors.clear()
-            form.populate_obj(obj)
-        else:
-            auto_submit_values_to_use = {}
-            form.populate_obj(obj)
-        for field_name in auto_submit_values_to_use:
-            setattr(obj, field_name, auto_submit_values_to_use[field_name])
-
-    def _is_past_timeout(self):
-        """
-        Need to check that we are actually past the expiration time.
-        Otherwise, a participant could skip past a page before it's ready,
-        by bypassing the execution of error_message(),
-        which is skipped when there is a timeout.
-        """
-        pp = self.participant
-        # the 2 seconds should not be necessary but there may be some unexpected case.
-        return (
-            pp._timeout_page_index == pp._index_in_pages
-            and pp._timeout_expiration_time is not None
-            and (pp._timeout_expiration_time - time.time() < 2)
-        )
-
-    # don't use lru_cache. it is a global cache
-    # @cached_property only in python 3.8
-    _remaining_timeout_seconds = 'unset'
-
-    def remaining_timeout_seconds(self):
-        if self._remaining_timeout_seconds == 'unset':
-            self._remaining_timeout_seconds = self.remaining_timeout_seconds_inner()
-        return self._remaining_timeout_seconds
-
-    def remaining_timeout_seconds_inner(self):
-        current_time = time.time()
-        participant = self.participant
-        if participant._timeout_page_index == participant._index_in_pages:
-            if participant._timeout_expiration_time is None:
-                return None
-            return participant._timeout_expiration_time - current_time
-        if hasattr(self, 'get_timeout_seconds'):
-            timeout_seconds = self.call_user_defined('get_timeout_seconds')
-        else:
-            timeout_seconds = self.timeout_seconds
-        participant._timeout_page_index = participant._index_in_pages
-        if timeout_seconds is None:
-            participant._timeout_expiration_time = None
-            return None
-        participant._timeout_expiration_time = current_time + timeout_seconds
-
-        if otree.common.USE_TIMEOUT_WORKER:
-            # if using browser bots, don't schedule the timeout,
-            # because if it's a short timeout, it could happen before
-            # the browser bot submits the page. Because the timeout
-            # doesn't query the botworker (it is distinguished from bot
-            # submits by the timeout_happened flag), it will "skip ahead"
-            # and therefore confuse the bot system.
-            if not self.participant.is_browser_bot:
-                otree.tasks.submit_expired_url(
-                    participant_code=self.participant.code,
-                    page_index=self.participant._index_in_pages,
-                    # add some seconds to account for latency of request + response
-                    # this will (almost) ensure
-                    # (1) that the page will be submitted by JS before the
-                    # timeoutworker, which ensures that self.request.POST
-                    # actually contains a value.
-                    # (2) that the timeoutworker doesn't accumulate a lead
-                    # ahead of the real page, which could result in being >1
-                    # page ahead. that means that entire pages could be skipped
-                    delay=timeout_seconds + 6,
-                )
-        return timeout_seconds
-
-    timeout_seconds = None
-    timeout_submission = None
-    timer_text = core_gettext("Time left to complete this page:")
-
-
-class GenericWaitPageMixin:
-    """used for in-game wait pages, as well as other wait-type pages oTree has
-    (like waiting for session to be created, or waiting for players to be
-    assigned to matches
-
-    """
-
-    request: Request = None
-
-    def get_template_name(self):
-        '''built-in wait pages should not be overridable'''
-        return 'otree/WaitPage.html'
-
-    def _get_wait_page(self):
-        self.participant.is_on_wait_page = True
-        self._update_monitor_table()
-        response = render(self.get_template_name(), self.get_context_data())
-        response.headers[
-            otree.constants.wait_page_http_header
-        ] = otree.constants.get_param_truth_value
-        return response
-
-    # Translators: the default title of a wait page
-    title_text = core_gettext('Please wait')
-    body_text = None
-
-    def _get_default_body_text(self):
-        '''
-        needs to be a method because it could say
-        "waiting for the other player", "waiting for the other players"...
-        '''
-        return ''
-
-    def get_context_data(self):
-        title_text = self.title_text
-        body_text = self.body_text
-
-        # could evaluate to false like 0
-        if body_text is None:
-            body_text = self._get_default_body_text()
-
-        # default title/body text can be overridden
-        # if user specifies it in vars_for_template
-        return dict(view=self, title_text=title_text, body_text=body_text)
-
-
-class WaitPage(FormPageOrInGameWaitPage, GenericWaitPageMixin):
-    """
-    Wait pages during game play (i.e. checkpoints),
-    where users wait for others to complete
-    """
-
-    wait_for_all_groups = False
-    group_by_arrival_time = False
-
-    _template_type = 'WaitPage'
-
-    def get_context_data(self):
-        context = GenericWaitPageMixin.get_context_data(self)
-        return FormPageOrInGameWaitPage.get_context_data(self, **context)
-
-    def get_template_name(self):
-        """fallback to otree/WaitPage.html, which is guaranteed to exist.
-        the reason for the 'if' statement, rather than returning a list,
-        is that if the user explicitly defined template_name, and that template
-        does not exist, then we should not fail silently.
-        (for example, the user forgot to add it to git)
-        """
-        if self.template_name:
-            return self.template_name
-
-        if Path('_templates/global/WaitPage.html').exists():
-            return 'global/WaitPage.html'
-        return 'otree/WaitPage.html'
-
-    def inner_dispatch(self, request):
-        # we need inner_dispatch() for common interface w/ parent class
-        # and .get() so it can be called explicitly.
-        return self.get()
-
-    def get(self):
-        # necessary because queries are made directly from DB
-
-        if self.wait_for_all_groups == True:
-            resp = self.inner_dispatch_subsession()
-        elif self.group_by_arrival_time:
-            resp = self.inner_dispatch_gbat()
-        else:
-            resp = self.inner_dispatch_group()
-        return resp
-
-    def _run_aapa_and_notify(self, group_or_subsession):
-        '''
-        group_or_subsession is passed explicitly, because in the case of GBAT it might
-        not include the current player, so we can't just use self.player.group.
-
-        new design is that if anybody is waiting on the wait page, we run AAPA.
-        If nobody is shown the wait page, we don't need to notify or even create a
-        CompletedGroupWaitPage record.
-        '''
-        if self.wait_for_all_groups:
-            group = None
-            noself_kwargs = dict(subsession=group_or_subsession)
-        else:
-            group = group_or_subsession
-            noself_kwargs = dict(group=group_or_subsession)
-
-        aapa = type(self).after_all_players_arrive
-        if isinstance(aapa, str):
-            group_or_subsession.call_user_defined(aapa)
-        # old format; it's a regular method
-        elif str(inspect.signature(aapa)) == '(self)':
-            wp: WaitPage = type(self)({'type': 'http'}, None, None)
-            wp.set_attributes_waitpage_clone(original_view=self)
-            wp._group_for_wp_clone = group
-            wp.after_all_players_arrive()
-        else:
-            # noself
-            # pass kwargs so that we can ensure the user did not use a group method
-            # where a subsession method should have been used
-            aapa(**noself_kwargs)
-        self._mark_completed_and_notify(group=group)
-
-    def inner_dispatch_group(self):
-        ## EARLY EXITS
-        if CompletedGroupWaitPage.objects_exists(
-            page_index=self._index_in_pages,
-            group_id=self.player.group_id,
-            session_id=self._session_pk,
-        ):
-            return self._response_when_ready()
-        is_displayed = self._is_displayed()
-        is_last, someone_waiting = self._tally_unvisited()
-        if is_displayed and not is_last:
-            return self._get_wait_page()
-        elif is_last and (someone_waiting or is_displayed):
-            self._run_aapa_and_notify(self.group)
-        return self._response_when_ready()
-
-    def inner_dispatch_subsession(self):
-
-        if CompletedSubsessionWaitPage.objects_exists(
-            page_index=self._index_in_pages, session=self.session
-        ):
-            return self._response_when_ready()
-
-        is_displayed = self._is_displayed()
-        is_last, someone_waiting = self._tally_unvisited()
-        if is_displayed and not is_last:
-            return self._get_wait_page()
-        elif is_last and (someone_waiting or is_displayed):
-            self._run_aapa_and_notify(self.subsession)
-        return self._response_when_ready()
-
-    def inner_dispatch_gbat(self):
-        if CompletedGBATWaitPage.objects_exists(
-            page_index=self._index_in_pages,
-            id_in_subsession=self.group.id_in_subsession,
-            session=self.session,
-        ):
-            return self._response_when_ready()
-
-        if not self._is_displayed():
-            # in GBAT, either all players should skip a page, or none should.
-            # we don't support some players skipping and others not.
-            return self._response_when_ready()
-
-        participant = self.participant
-
-        participant._gbat_is_connected = True
-        participant._gbat_page_index = self._index_in_pages
-        participant._gbat_grouped = False
-        # _last_request_timestamp is already set in set_attributes,
-        # but set it here just so we can guarantee
-        participant._last_request_timestamp = int(time.time())
-        # need to save it inside the lock (check-then-act)
-        # also because it needs to be up to date for get_players_for_group
-        # which gets this info from the DB
-        # make a clean copy for GBAT and AAPA
-        # self.player and self.participant etc are undefined
-        # and no objects are cached inside it
-        # and it doesn't affect the current instance
-
-        gbat_new_group = self.subsession._gbat_try_to_make_new_group(
-            self._index_in_pages
-        )
-
-        if gbat_new_group:
-            self._run_aapa_and_notify(gbat_new_group)
-            # gbat_new_group may not include the current player!
-            # maybe this will not work if i change the implementation
-            # so that the player is cached,
-            # but that's OK because it will be obvious it doesn't work.
-
-            if participant._gbat_grouped:
-                return self._response_when_ready()
-
-        return self._get_wait_page()
-
-    @property
-    def _group_or_subsession(self):
-        return self.subsession if self.wait_for_all_groups else self.group
-
-    def _get_participants_for_this_waitpage(self, group_or_subsession):
-        """
-        group_or_subsession needs to be passed because it could be a newly created group with GBAT,
-        and may not equal self.group because the current player may not be part of the group.
-        (for example, when creating single-player groups with waiting_too_long).
-        """
-        Player = self.PlayerClass
-        fk_field = Player.subsession_id if self.wait_for_all_groups else Player.group_id
-        # tried select_from but my filter clause didn't work
-        return (
-            dbq(Player)
-            .join(Participant)
-            .filter(fk_field == group_or_subsession.id)
-            .with_entities(Participant)
-        )
-
-    # this is needed because on wait pages, self.player doesn't exist.
-    # usually oTree finds the group by doing self.player.group.
-    _group_for_wp_clone = None
-
-    @property
-    def group(self):
-        return self._group_for_wp_clone or super().group
-
-    def _mark_page_completions(self, participants: List[Participant]):
-        '''
-        this is more accurate than page load,
-        because the player may delay doing that,
-        to make it look like they waited longer.
-        '''
-        app_name = self.player.get_folder_name()
-        session_code = self.participant._session_code
-
-        for pp in participants:
-            otree.common2.make_page_completion_row(
-                view=self,
-                app_name=app_name,
-                participant__id_in_session=pp.id_in_session,
-                participant__code=pp.code,
-                session_code=session_code,
-                is_wait_page=1,
-            )
-
-    def _mark_completed_and_notify(self, group: Optional[BaseGroup]):
-        # if group is not passed, then it's the whole subsession
-        # could be 2 people creating the record at the same time
-        # in _increment_index_in_pages, so could end up creating 2 records
-        # but it's not a problem.
-
-        base_kwargs = dict(page_index=self._index_in_pages, session_id=self._session_pk)
-        Player = self.PlayerClass
-
-        if self.wait_for_all_groups:
-            CompletedSubsessionWaitPage.objects_create(**base_kwargs)
-        elif self.group_by_arrival_time:
-            db.add(
-                CompletedGBATWaitPage(
-                    **base_kwargs, id_in_subsession=group.id_in_subsession
-                )
-            )
-        else:
-            db.add(CompletedGroupWaitPage(**base_kwargs, group_id=group.id))
-
-        participants = self._get_participants_for_this_waitpage(
-            group or self.subsession
-        )
-        self._mark_page_completions(list(participants))
-        for pp in participants:
-            pp._last_page_timestamp = int(time.time())
-
-        # this can cause messages to get wrongly enqueued in the botworker
-        if otree.common.USE_TIMEOUT_WORKER and not self.participant.is_browser_bot:
-            # 2016-11-15: we used to only ensure the next page is visited
-            # if the next page has a timeout, or if it's a wait page
-            # but this is not reliable because next page might be skipped anyway,
-            # and we don't know what page will actually be shown next to the user.
-            otree.tasks.ensure_pages_visited(
-                participant_pks=[pp.id for pp in participants],
-                delay=10,
-                page_index=self._index_in_pages,
-            )
-
-        if self.group_by_arrival_time:
-            channel_utils.sync_group_send(
-                group=channel_utils.gbat_group_name(**base_kwargs),
-                data={'status': 'ready'},
-            )
-        else:
-            if self.wait_for_all_groups:
-                channels_group_name = channel_utils.subsession_wait_page_name(
-                    **base_kwargs
-                )
-            else:
-                channels_group_name = channel_utils.group_wait_page_name(
-                    **base_kwargs, group_id=group.id
-                )
-
-            channel_utils.sync_group_send(
-                group=channels_group_name, data={'status': 'ready'}
-            )
-
-    def socket_url(self):
-        session_pk = self._session_pk
-        page_index = self._index_in_pages
-        participant_id = self.participant.id
-        if self.group_by_arrival_time:
-            return channel_utils.gbat_path(
-                session_pk=session_pk,
-                page_index=page_index,
-                app_name=self.player.get_folder_name(),
-                participant_id=participant_id,
-                player_id=self.player.id,
-            )
-        elif self.wait_for_all_groups:
-            return channel_utils.subsession_wait_page_path(
-                session_pk=session_pk,
-                page_index=page_index,
-                participant_id=participant_id,
-            )
-        else:
-            return channel_utils.group_wait_page_path(
-                session_pk=session_pk,
-                page_index=page_index,
-                participant_id=participant_id,
-                group_id=self.player.group_id,
-            )
-
-    def _tally_unvisited(self):
-
-        participants = self._get_participants_for_this_waitpage(
-            self._group_or_subsession
-        )
-        session_code = self.participant._session_code
-
-        visited = []
-        unvisited = []
-        for p in participants:
-            [unvisited, visited][p._index_in_pages >= self._index_in_pages].append(p)
-
-        # this is not essential to functionality.
-        # just for the display in the Monitor tab.
-        if len(unvisited) <= 3:
-            if len(unvisited) == 0:
-                note = ''
-            else:
-                note = ', '.join(p._numeric_label() for p in unvisited)
-
-                for p in visited:
-                    p._monitor_note = note
-
-            channel_utils.sync_group_send(
-                group=channel_utils.session_monitor_group_name(session_code),
-                data=dict(
-                    ids=[p.id_in_session for p in visited],
-                    note=note,
-                    type='update_notes',
-                ),
-            )
-
-        # is_last is not technically true. maybe someone else also is waiting for this page
-        # just behind you. but it doesn't matter; you can still advance the waitpage.
-        is_last = not bool(unvisited)
-        someone_waiting = any(
-            [
-                p._index_in_pages == self._index_in_pages and p.is_on_wait_page
-                for p in participants
-            ]
-        )
-        return (is_last, someone_waiting)
-
-    def is_displayed(self):
-        return True
-
-    def _response_when_ready(self):
-        '''
-        Before calling this function, the following must be satisfied:
-        - The completion object exists
-        OR
-        - The player skips this page
-        '''
-        participant = self.participant
-        participant.is_on_wait_page = False
-        participant._monitor_note = None
-        self._increment_index_in_pages()
-        return self._redirect_to_page_the_user_should_be_on()
-
-    def after_all_players_arrive(self):
-        pass
-
-    def _get_default_body_text(self):
-        num_other_players = self._group_or_subsession.player_set.count() - 1
-        if num_other_players > 1:
-            return core_gettext('Waiting for the other participants.')
-        if num_other_players == 1:
-            return core_gettext('Waiting for the other participant.')
-        return ''
-
-
-class InvalidAppError(Exception):
-    pass
-
-
-class MockForm:
-    def __iter__(self):
-        if False:
-            yield
-
-    def __init__(self, error_message=None):
-        self.non_field_error = error_message
-
-    field_names = []
-
-    @property
-    def errors(self):
-        return bool(self.non_field_error)
+import inspect
+import logging
+import time
+import typing
+from html import escape
+from pathlib import Path
+from typing import List
+from typing import Optional
+
+import starlette.exceptions
+from starlette.concurrency import run_in_threadpool
+from starlette.datastructures import FormData as StarletteFormData
+from starlette.requests import Request
+from starlette.responses import RedirectResponse, HTMLResponse
+from starlette.types import Receive, Scope, Send
+
+# this is an expensive import
+import otree.bots.browser as browser_bots
+import otree.channels.utils as channel_utils
+import otree.common
+import otree.common2
+import otree.constants
+from otree.currency import json_dumps
+import otree.forms
+import otree.models
+import otree.tasks
+import otree.views.cbv
+from otree import settings
+from otree.bots.bot import bot_prettify_post_data
+from otree.common import (
+    get_app_label_from_import_path,
+    get_dotted_name,
+    get_admin_secret_code,
+    DebugTable,
+    BotError,
+    NON_FIELD_ERROR_KEY,
+    get_constants,
+)
+from otree.database import db, dbq
+from otree.forms.forms import get_form
+from otree.i18n import core_gettext
+from otree.lookup import get_min_idx_for_app, get_page_lookup
+from otree.models import Participant, Session, BaseGroup, BaseSubsession
+from otree.models_concrete import (
+    CompletedSubsessionWaitPage,
+    CompletedGroupWaitPage,
+    CompletedGBATWaitPage,
+)
+import otree.trial
+from otree.templating import render
+
+logger = logging.getLogger(__name__)
+
+
+ADMIN_SECRET_CODE = get_admin_secret_code()
+
+
+BOT_COMPLETE_HTML_MESSAGE = '''
+<html>
+    <head>
+        <title>Bot completed</title>
+    </head>
+    <body>Bot completed</body>
+</html>
+'''
+
+
+class FormPageOrInGameWaitPage:
+    request: Request
+
+    @classmethod
+    def instantiate_without_request(cls):
+        return cls({'type': 'http'}, None, None)
+
+    def __init__(self, scope: Scope, receive: Receive, send: Send) -> None:
+        assert scope["type"] == "http"
+        self.scope = scope
+        self.receive = receive
+        self.send = send
+
+    def __await__(self) -> typing.Generator:
+        return self.dispatch().__await__()
+
+    def call_user_defined(self, method_name, *args, **kwargs):
+        """
+        the default user-defined methods should not reference self, so they can work
+        both as Player methods and Page methods.
+        """
+        if self.is_noself:
+            return getattr(type(self), method_name)(self.player, *args, **kwargs)
+        return getattr(self, method_name)(*args, **kwargs)
+
+    async def dispatch(self) -> None:
+        self.request = request = Request(self.scope, receive=self.receive)
+        participant_code = request.path_params['participant_code']
+        msg = (
+            "This user does not exist in the database. " "Maybe the database was reset."
+        )
+        participant = db.get_or_404(Participant, code=participant_code, msg=msg)
+
+        # if the player tried to skip past a part of the subsession
+        # (e.g. by typing in a future URL)
+        # or if they hit the back button to a previous subsession
+        # in the sequence.
+        url_should_be_on = participant._url_i_should_be_on()
+        if not request.url.path == url_should_be_on:
+            response = RedirectResponse(url_should_be_on, status_code=302)
+        else:
+            self.set_attributes(participant)
+            # need to await the form from async function, otherwise run into complicated RuntimeError
+            try:
+                if request.method == 'POST':
+                    self._form_data = await self.request.form()
+            except starlette.requests.ClientDisconnect:
+                # just make an empty response, to avoid
+                # "RuntimeError: No response returned"
+                response = starlette.responses.Response()
+            else:
+                response = await run_in_threadpool(self.inner_dispatch, request)
+        await response(self.scope, self.receive, self.send)
+
+    template_name = None
+
+    is_debug = settings.DEBUG
+
+    def inner_dispatch(self, request):
+        '''inner dispatch function'''
+        raise NotImplementedError()
+
+    def get_template_name(self):
+        raise NotImplementedError()
+
+    @classmethod
+    def url_pattern(cls, name_in_url):
+        p = '/p/{participant_code}/%s/%s/{page_index}' % (name_in_url, cls.__name__)
+        return p
+
+    @classmethod
+    def get_url(cls, participant_code, name_in_url, page_index):
+        '''need this because reverse() is too slow in create_session'''
+        # if i change this URL pattern, i should also change assert_correct_page()
+        # in bot.py
+        return f'/p/{participant_code}/{name_in_url}/{cls.__name__}/{page_index}'
+
+    @classmethod
+    def url_name(cls):
+        '''using dots seems not to work'''
+        return get_dotted_name(cls).replace('.', '-')
+
+    def _redirect_to_page_the_user_should_be_on(self):
+        return RedirectResponse(self.participant._url_i_should_be_on(), status_code=302)
+
+    @classmethod
+    def has_trial(cls):
+        return bool(getattr(cls, 'trial_model', None))
+
+    def get_context_data(self, **context):
+
+        context.update(
+            view=self,
+            object=getattr(self, 'object', None),
+            player=self.player,
+            group=self.group,
+            subsession=self.subsession,
+            session=self.session,
+            participant=self.participant,
+            timer_text=getattr(self, 'timer_text', None),
+            current_page_name=self.__class__.__name__,
+            has_live_method=bool(getattr(self, 'live_method', None)),
+            has_trial=self.has_trial(),
+        )
+
+        Constants = self._Constants
+        # it could be called C or Constants
+        context[Constants.__name__] = Constants
+
+        vars_for_template = {}
+
+        user_vars = self.call_user_defined('vars_for_template')
+        user_vars = user_vars or {}
+        if not isinstance(user_vars, dict):
+            raise Exception('vars_for_template did not return a dict')
+
+        js_vars = self.call_user_defined('js_vars')
+
+        try:
+            # better to convert to json here so we can catch any errors,
+            # rather than applying the filter in the template.
+            context['js_vars'] = json_dumps(js_vars)
+        except TypeError as exc:
+            raise TypeError(f'js_vars contains an invalid value; {exc}') from None
+
+        has_trial = self.has_trial()
+        if has_trial:
+            Trial = self.trial_model
+            use_roundtrip_mode = hasattr(self, 'evaluate_trial')
+            if use_roundtrip_mode:
+                trials = []
+            else:
+                trials = [
+                    otree.trial.encode_trial(t, self.trial_stimulus_fields)
+                    for t in Trial.filter(player=self.player)
+                ]
+            context['trials_json'] = json_dumps(trials)
+            context['_trials_use_roundtrip_mode'] = json_dumps(use_roundtrip_mode)
+
+        vars_for_template.update(user_vars)
+
+        context.update(vars_for_template)
+
+        if settings.DEBUG:
+            self.debug_tables = self._get_debug_tables(vars_for_template)
+        return context
+
+    def render_to_response(self, context):
+        return render(
+            self.get_template_name(), context, template_type=self._template_type
+        )
+
+    _template_type = None
+
+    def vars_for_template(self):
+        return {}
+
+    def js_vars(self):
+        return {}
+
+    def _get_debug_tables(self, vars_for_template):
+
+        tables = []
+        if vars_for_template:
+            # use repr() so that we can distinguish strings from numbers
+            # and can see currency types, etc.
+            items = [(k, escape(repr(v))) for (k, v) in vars_for_template.items()]
+            rows = sorted(items)
+            tables.append(DebugTable(title='vars_for_template', rows=rows))
+
+        player = self.player
+        participant = self.participant
+        basic_info_table = DebugTable(
+            title='Basic info',
+            rows=[
+                ('ID in group', player.id_in_group),
+                ('Group', player.group_id),
+                ('Round number', player.round_number),
+                ('Participant', participant._numeric_label()),
+                ('Participant label', participant.label or ''),
+                ('Session code', participant._session_code),
+            ],
+        )
+
+        tables.append(basic_info_table)
+
+        return tables
+
+    def _is_displayed(self):
+        return self.call_user_defined('is_displayed')
+
+    @property
+    def group(self) -> BaseGroup:
+        '''can't cache self._group_pk because group can change'''
+        return self.player.group
+
+    @property
+    def subsession(self) -> BaseSubsession:
+        '''so that it doesn't rely on player'''
+        # this goes through idmap cache, so no perf hit
+        return self.SubsessionClass.objects_get(id=self._subsession_pk)
+
+    @property
+    def session(self) -> Session:
+        return Session.objects_get(id=self._session_pk)
+
+    def set_attributes(self, participant):
+
+        lookup = get_page_lookup(participant._session_code, participant._index_in_pages)
+        self._lookup = lookup
+
+        app_name = lookup.app_name
+
+        models_module = otree.common.get_models_module(app_name)
+
+        self._Constants = get_constants(app_name)
+        self.PlayerClass = getattr(models_module, 'Player')
+        self.GroupClass = getattr(models_module, 'Group')
+        self.SubsessionClass = getattr(models_module, 'Subsession')
+        self.player = self.PlayerClass.objects_get(
+            participant=participant, round_number=lookup.round_number
+        )
+        self._subsession_pk = lookup.subsession_id
+        self.round_number = lookup.round_number
+        self._session_pk = lookup.session_pk
+        # simpler if we set it directly so that we can do tests without idmap cache
+        self._participant_pk = participant.id
+        # setting it directly makes testing easier (tests dont need to use cache)
+        self.participant: Participant = participant
+
+        # it's already validated that participant is on right page
+        self._index_in_pages = participant._index_in_pages
+
+        # for the participant changelist
+        participant._current_app_name = app_name
+        participant._current_page_name = self.__class__.__name__
+        participant._last_request_timestamp = int(time.time())
+        participant._round_number = lookup.round_number
+
+    def set_attributes_waitpage_clone(self, *, original_view: 'WaitPage'):
+        '''put it here so it can be compared with set_attributes...
+        but this is really just a method on wait pages'''
+        # make a clean copy for AAPA
+        # self.player and self.participant etc are undefined
+        # and no objects are cached inside it
+        # and it doesn't affect the current instance
+
+        self._Constants = original_view._Constants
+        self.GroupClass = original_view.GroupClass
+        self.SubsessionClass = original_view.SubsessionClass
+        self._subsession_pk = original_view._subsession_pk
+        self._session_pk = original_view._session_pk
+        self.round_number = original_view.round_number
+
+    def _increment_index_in_pages(self):
+        # when is this not the case?
+        participant = self.participant
+        assert self._index_in_pages == participant._index_in_pages
+
+        # we should allow a user to move beyond the last page if it's mturk
+        # also in general maybe we should show the 'out of sequence' page
+
+        # we skip any page that is a sequence page where is_displayed
+        # evaluates to False to eliminate unnecessary redirection
+
+        page_index_to_skip_to = self._get_next_page_index_if_skipping_apps()
+        is_skipping_apps = bool(page_index_to_skip_to)
+
+        for page_index in range(
+            # go to max_page_index+2 because range() skips the last index
+            # and it's possible to go to max_page_index + 1 (OutOfRange)
+            self._index_in_pages + 1,
+            participant._max_page_index + 2,
+        ):
+            participant._index_in_pages = page_index
+            if page_index == participant._max_page_index + 1:
+                # break and go to OutOfRangeNotification
+                break
+            if is_skipping_apps and page_index == page_index_to_skip_to:
+                break
+
+            # scope, receive, send
+            page = get_page_lookup(
+                participant._session_code, page_index
+            ).page_class.instantiate_without_request()
+
+            page.set_attributes(self.participant)
+            if not is_skipping_apps and page._is_displayed():
+                break
+
+            # if it's a wait page, record that they visited
+            if isinstance(page, WaitPage):
+
+                if page.group_by_arrival_time:
+                    # keep looping
+                    # if 1 participant can skip the page,
+                    # then all other participants should skip it also,
+                    # as described in the docs
+                    # so there is no need to mark as complete.
+                    continue
+
+                # save the participant, because tally_unvisited
+                # queries index_in_pages directly from the DB
+                db.commit()
+
+                is_last, someone_waiting = page._tally_unvisited()
+                if is_last and someone_waiting:
+                    page._run_aapa_and_notify(page._group_or_subsession)
+
+    def is_displayed(self):
+        return True
+
+    def _update_monitor_table(self):
+        self.participant._update_monitor_table()
+
+    def _get_next_page_index_if_skipping_apps(self):
+        # don't run it if the page is not displayed, because:
+        # (1) it's consistent with other functions like before_next_page, vars_for_template
+        # (2) then when we do
+        # a lookahead skipping pages, we would need to check each page if it
+        # has app_after_this_page defined, then set attributes and run it.
+        # what if we are already skipping to a future app, then another page
+        # has app_after_this_page? does it override the first one?
+        if not self._is_displayed():
+            return
+        if not hasattr(self, 'app_after_this_page'):
+            return
+
+        current_app = self.participant._current_app_name
+        app_sequence = self.session.config['app_sequence']
+        current_app_index = app_sequence.index(current_app)
+        upcoming_apps = app_sequence[current_app_index + 1 :]
+
+        app_to_skip_to = self.call_user_defined('app_after_this_page', upcoming_apps)
+        if app_to_skip_to:
+            if app_to_skip_to not in upcoming_apps:
+                msg = f'"{app_to_skip_to}" is not in the upcoming_apps list'
+                raise InvalidAppError(msg)
+            return get_min_idx_for_app(self.participant._session_code, app_to_skip_to)
+
+    def _record_page_completion_time(self):
+        now = int(time.time())
+        participant = self.participant
+
+        session_code = participant._session_code
+
+        otree.common2.make_page_completion_row(
+            view=self,
+            app_name=self.player.get_folder_name(),
+            participant__id_in_session=participant.id_in_session,
+            participant__code=participant.code,
+            session_code=session_code,
+            is_wait_page=0,
+        )
+
+        participant._last_page_timestamp = now
+
+    def live_url(self):
+        return channel_utils.live_path(
+            participant_code=self.participant.code,
+            page_name=type(self).__name__,
+            page_index=self._index_in_pages,
+            session_code=self.participant._session_code,
+        )
+
+    def trial_url(self):
+        return channel_utils.trial_path(
+            participant_code=self.participant.code,
+            page_name=type(self).__name__,
+            page_index=self._index_in_pages,
+        )
+
+    live_method = ''
+
+
+class Page(FormPageOrInGameWaitPage):
+    form_model = None
+    form_fields = []
+
+    _template_type = 'Page'
+
+    def inner_dispatch(self, request):
+        if request.method == 'POST':
+            return self.post()
+        return self.get()
+
+    def browser_bot_stuff(self, response: HTMLResponse):
+        """we use this hack of appending to the HTML, rather than sending a context var,
+        because we don't know if we need to submit the page until we try enqueueing the next post data.
+        i guess that can't be done until we have the HTML of the page.
+        """
+        if self.participant.is_browser_bot:
+            browser_bots.set_attributes(
+                participant_code=self.participant.code,
+                request_path=self.request.url.path,
+                html=response.body.decode('utf-8'),
+            )
+            has_next_submission = browser_bots.enqueue_next_post_data(
+                participant_code=self.participant.code
+            )
+            if has_next_submission:
+                # this doesn't work because we also would need to do this on OutOfRange page.
+                # sometimes the player submits the last page, especially during development.
+                # if self._index_in_pages == self.participant._max_page_index:
+                auto_submit_js = '''
+                <script>
+                    var form = document.querySelector('#form');
+                    form.submit();
+                    // browser-bot-auto-submit
+                    form.on('submit', function (e) {
+                        e.preventDefault();
+                    });
+                </script>
+                '''
+                extra_content = auto_submit_js.encode('utf8')
+                response.body += extra_content
+                response.headers['Content-Length'] = str(
+                    int(response.headers['Content-Length']) + len(extra_content)
+                )
+            else:
+                browser_bots.send_completion_message(
+                    session_code=self.participant._session_code,
+                    participant_code=self.participant.code,
+                )
+
+    def get(self):
+
+        if not self._is_displayed():
+            self._increment_index_in_pages()
+            return self._redirect_to_page_the_user_should_be_on()
+
+        # this needs to be set AFTER scheduling submit_expired_url,
+        # to prevent race conditions.
+        # see that function for an explanation.
+        # self.participant._current_form_page_url = self.request.url.path
+
+        self._update_monitor_table()
+
+        # 2020-07-10: maybe we should call vars_for_template before instantiating the form
+        # so that you can set initial value for a field in vars_for_template?
+        # No, i don't want to commit to that.
+        form = self.get_form_or_mockform()
+
+        context = self.get_context_data(form=form)
+        response = self.render_to_response(context)
+        self.browser_bot_stuff(response)
+        return response
+
+    def get_form_or_mockform(self):
+        if self.has_form():
+            obj = self.get_object()
+            return self.get_form(instance=obj)
+        else:
+            return MockForm()
+
+    def get_template_name(self):
+        if self.template_name is not None:
+            return self.template_name
+        return '{}/{}.html'.format(
+            get_app_label_from_import_path(self.__module__), self.__class__.__name__
+        )
+
+    def has_form(self):
+        return bool(self._get_form_fields())
+
+    def _get_form_fields(self):
+        if hasattr(self, 'get_form_fields'):
+            return self.call_user_defined('get_form_fields')
+        return self.form_fields
+
+    def get_object(self):
+        if not self.form_model:
+            msg = 'Page has form_fields but not form_model'
+            raise Exception(msg)
+        return {
+            'player': self.player,
+            'group': self.group,
+            self.PlayerClass: self.player,
+            self.GroupClass: self.group,
+        }[self.form_model]
+
+    def get_form(self, instance, formdata=None) -> otree.forms.forms.ModelForm:
+        fields = self._get_form_fields()
+        form = get_form(instance, field_names=fields, view=self, formdata=formdata)
+        return form
+
+    def form_invalid(self, form):
+        context = self.get_context_data(form=form)
+
+        fields_with_errors = [
+            fname for fname in form.errors if fname != NON_FIELD_ERROR_KEY
+        ]
+
+        # i think this should be before we call render_to_response
+        # because the view (self) is passed to the template and rendered
+        if fields_with_errors:
+            self.first_field_with_errors = fields_with_errors[0]
+            self.other_fields_with_errors = fields_with_errors[1:]
+
+        response = self.render_to_response(context)
+        response.headers[
+            otree.constants.redisplay_with_errors_http_header
+        ] = otree.constants.get_param_truth_value
+
+        return response
+
+    def must_complete_trials(self):
+        if self.timeout_happened:
+            return False
+        if self.has_trial():
+            Trial = self.trial_model
+            return bool(otree.trial.get_current_trial(Trial, self.player))
+        return False
+
+    def trials_incomplete_handler(self, form):
+        context = self.get_context_data(form=form, _trials_incomplete=True)
+        response = self.render_to_response(context)
+        response.headers[
+            otree.constants.redisplay_with_errors_http_header
+        ] = otree.constants.get_param_truth_value
+
+        return response
+
+    def _check_submission_must_fail(self, is_bot, post_data):
+        if is_bot and post_data.get('must_fail'):
+            msg = (
+                'Page "{}": Bot tried to submit intentionally invalid '
+                'data with '
+                'SubmissionMustFail, but it passed validation anyway:'
+                ' {}.'.format(
+                    self.__class__.__name__, bot_prettify_post_data(post_data)
+                )
+            )
+            raise BotError(msg)
+
+    def post_handle_form(self, post_data):
+        obj = self.get_object()
+        form = self.get_form(formdata=post_data, instance=obj)
+        self.form = form
+
+        if self.must_complete_trials():
+            return self.trials_incomplete_handler(form)
+
+        if self.timeout_happened:
+            self._process_auto_submitted_form(form, obj)
+        else:
+            is_bot = self.participant._is_bot
+            if form.validate():
+                self._check_submission_must_fail(is_bot, post_data)
+                form.populate_obj(obj)
+            else:
+                if is_bot:
+                    PageName = self.__class__.__name__
+                    if not post_data.get('must_fail'):
+                        errors = [
+                            "{}: {}".format(k, repr(v)) for k, v in form.errors.items()
+                        ]
+                        msg = (
+                            'Page "{}": Bot submission failed form validation: {} '
+                            'Check your bot code, '
+                            'then create a new session. '
+                            'Data submitted was: {}'.format(
+                                PageName, errors, bot_prettify_post_data(post_data)
+                            )
+                        )
+                        raise BotError(msg)
+                    if post_data.get('error_fields'):
+                        expected_error_fields = set(post_data.getlist('error_fields'))
+                        actual_error_fields = set(form.errors.keys())
+                        if not expected_error_fields == actual_error_fields:
+                            msg = (
+                                'Page {}, SubmissionMustFail: '
+                                'Expected error_fields were {}, but actual '
+                                'error_fields are {}'.format(
+                                    PageName, expected_error_fields, actual_error_fields
+                                )
+                            )
+                            raise BotError(msg)
+                response = self.form_invalid(form)
+                self.browser_bot_stuff(response)
+                return response
+
+    _form_data = None
+
+    def post(self):
+        post_data = self._form_data
+        auto_submitted = post_data.get(otree.constants.timeout_happened)
+        # if the page doesn't have a timeout_seconds, only the timeoutworker
+        # should be able to auto-submit it.
+        # otherwise users could append timeout_happened to the URL to skip pages
+        has_secret_code = (
+            post_data.get(otree.constants.admin_secret_code) == ADMIN_SECRET_CODE
+        )
+        # convert it to a bool so that you can do e.g.
+        # player.timeout_happened = timeout_happened
+        self.timeout_happened = bool(
+            auto_submitted and (has_secret_code or self._is_past_timeout())
+        )
+        if self.participant.is_browser_bot:
+            submission = browser_bots.pop_enqueued_post_data(
+                participant_code=self.participant.code
+            )
+
+            d = dict(post_data)
+            # normalize to string because wtforms gets confused when it receives
+            # string input, for example the int 0 does not pass InputRequired
+            # (but how about CLI bots?)
+            d.update({k: str(v) for k, v in submission.items()})
+            post_data = StarletteFormData(d)
+
+        if self.has_form():
+            resp = self.post_handle_form(post_data)
+            if resp:
+                return resp
+        elif self.must_complete_trials():
+            return self.trials_incomplete_handler(form=MockForm())
+        elif hasattr(self, 'error_message') and not self.timeout_happened:
+            # if the page has no form, we should still run error_message.
+            # this is useful for live pages.
+            # the code here is a stripped-down version of what happens with forms.
+            is_bot = self.participant._is_bot
+            error_message = self.call_user_defined('error_message', {})
+            if error_message:
+                if is_bot and not post_data.get('must_fail'):
+                    msg = (
+                        'Page "{}": Bot submission failed form validation: {} '
+                        'Check your bot code, '
+                        'then create a new session. '
+                    ).format(self.__class__.__name__, error_message)
+                    raise BotError(msg)
+                context = self.get_context_data(
+                    form=MockForm(error_message=error_message)
+                )
+                response = self.render_to_response(context)
+                response.headers[
+                    otree.constants.redisplay_with_errors_http_header
+                ] = otree.constants.get_param_truth_value
+                self.browser_bot_stuff(response)
+                return response
+            elif is_bot and post_data.get('must_fail'):
+                self._check_submission_must_fail(is_bot, post_data)
+
+        extra_args = (
+            dict(timeout_happened=self.timeout_happened) if self.is_noself else {}
+        )
+        self.call_user_defined('before_next_page', **extra_args)
+        self._record_page_completion_time()
+        self._increment_index_in_pages()
+        return self._redirect_to_page_the_user_should_be_on()
+
+    def before_next_page(self, timeout_happened=False):
+        pass
+
+    def socket_url(self):
+        '''called from template. can't start with underscore because used
+        in template
+        '''
+        return channel_utils.auto_advance_path(
+            participant_code=self.participant.code, page_index=self._index_in_pages
+        )
+
+    def _get_timeout_submission(self):
+        '''timeout_submission is deprecated'''
+        timeout_submission = self.timeout_submission or {}
+        for field_name in self._get_form_fields():
+            if field_name not in timeout_submission:
+                # get default value for datatype if the user didn't specify
+                ModelClass = type(self.get_object())
+                value = getattr(ModelClass, field_name).auto_submit_default
+                timeout_submission[field_name] = value
+        return timeout_submission
+
+    def _process_auto_submitted_form(self, form, obj):
+        '''
+        # an empty submitted form looks like this:
+        # {'f_currency': None, 'f_bool': None, 'f_int': None, 'f_char': ''}
+        '''
+        timeout_submission = self._get_timeout_submission()
+
+        # force the form to be cleaned
+        form.validate()
+
+        has_non_field_error = form.non_field_error
+
+        # If there is a timeout, we accept whatever fields don't have errors,
+        # so if there are errors, we have to call error_message manually,
+        # since error_message is only run if there are no
+        # field errors (because the error_message function assumes all fields exist)
+        if form.errors and not has_non_field_error:
+            if hasattr(self, 'error_message'):
+                try:
+                    has_non_field_error = bool(
+                        self.call_user_defined('error_message', form.data)
+                    )
+                except:
+                    has_non_field_error = True
+
+        if has_non_field_error:
+            # non-field errors exist.
+            # ignore form, use timeout_submission entirely
+            auto_submit_values_to_use = timeout_submission
+        elif form.errors:
+            auto_submit_values_to_use = {}
+            for field_name in form.errors:
+                auto_submit_values_to_use[field_name] = timeout_submission[field_name]
+            # save the fields without errors. we will overwrite the other fields with timeout_submission.
+            form.errors.clear()
+            form.populate_obj(obj)
+        else:
+            auto_submit_values_to_use = {}
+            form.populate_obj(obj)
+        for field_name in auto_submit_values_to_use:
+            setattr(obj, field_name, auto_submit_values_to_use[field_name])
+
+    def _is_past_timeout(self):
+        """
+        Need to check that we are actually past the expiration time.
+        Otherwise, a participant could skip past a page before it's ready,
+        by bypassing the execution of error_message(),
+        which is skipped when there is a timeout.
+        """
+        pp = self.participant
+        # the 2 seconds should not be necessary but there may be some unexpected case.
+        return (
+            pp._timeout_page_index == pp._index_in_pages
+            and pp._timeout_expiration_time is not None
+            and (pp._timeout_expiration_time - time.time() < 2)
+        )
+
+    # don't use lru_cache. it is a global cache
+    # @cached_property only in python 3.8
+    _remaining_timeout_seconds = 'unset'
+
+    def remaining_timeout_seconds(self):
+        if self._remaining_timeout_seconds == 'unset':
+            self._remaining_timeout_seconds = self.remaining_timeout_seconds_inner()
+        return self._remaining_timeout_seconds
+
+    def remaining_timeout_seconds_inner(self):
+        current_time = time.time()
+        participant = self.participant
+        if participant._timeout_page_index == participant._index_in_pages:
+            if participant._timeout_expiration_time is None:
+                return None
+            return participant._timeout_expiration_time - current_time
+        if hasattr(self, 'get_timeout_seconds'):
+            timeout_seconds = self.call_user_defined('get_timeout_seconds')
+        else:
+            timeout_seconds = self.timeout_seconds
+        participant._timeout_page_index = participant._index_in_pages
+        if timeout_seconds is None:
+            participant._timeout_expiration_time = None
+            return None
+        participant._timeout_expiration_time = current_time + timeout_seconds
+
+        if otree.common.USE_TIMEOUT_WORKER:
+            # if using browser bots, don't schedule the timeout,
+            # because if it's a short timeout, it could happen before
+            # the browser bot submits the page. Because the timeout
+            # doesn't query the botworker (it is distinguished from bot
+            # submits by the timeout_happened flag), it will "skip ahead"
+            # and therefore confuse the bot system.
+            if not self.participant.is_browser_bot:
+                otree.tasks.submit_expired_url(
+                    participant_code=self.participant.code,
+                    page_index=self.participant._index_in_pages,
+                    # add some seconds to account for latency of request + response
+                    # this will (almost) ensure
+                    # (1) that the page will be submitted by JS before the
+                    # timeoutworker, which ensures that self.request.POST
+                    # actually contains a value.
+                    # (2) that the timeoutworker doesn't accumulate a lead
+                    # ahead of the real page, which could result in being >1
+                    # page ahead. that means that entire pages could be skipped
+                    delay=timeout_seconds + 6,
+                )
+        return timeout_seconds
+
+    timeout_seconds = None
+    timeout_submission = None
+    timer_text = core_gettext("Time left to complete this page:")
+
+
+class GenericWaitPageMixin:
+    """used for in-game wait pages, as well as other wait-type pages oTree has
+    (like waiting for session to be created, or waiting for players to be
+    assigned to matches
+
+    """
+
+    request: Request = None
+
+    def get_template_name(self):
+        '''built-in wait pages should not be overridable'''
+        return 'otree/WaitPage.html'
+
+    def _get_wait_page(self):
+        self.participant.is_on_wait_page = True
+        self._update_monitor_table()
+        response = render(self.get_template_name(), self.get_context_data())
+        response.headers[
+            otree.constants.wait_page_http_header
+        ] = otree.constants.get_param_truth_value
+        return response
+
+    # Translators: the default title of a wait page
+    title_text = core_gettext('Please wait')
+    body_text = None
+
+    def _get_default_body_text(self):
+        '''
+        needs to be a method because it could say
+        "waiting for the other player", "waiting for the other players"...
+        '''
+        return ''
+
+    def get_context_data(self):
+        title_text = self.title_text
+        body_text = self.body_text
+
+        # could evaluate to false like 0
+        if body_text is None:
+            body_text = self._get_default_body_text()
+
+        # default title/body text can be overridden
+        # if user specifies it in vars_for_template
+        return dict(view=self, title_text=title_text, body_text=body_text)
+
+
+class WaitPage(FormPageOrInGameWaitPage, GenericWaitPageMixin):
+    """
+    Wait pages during game play (i.e. checkpoints),
+    where users wait for others to complete
+    """
+
+    wait_for_all_groups = False
+    group_by_arrival_time = False
+
+    _template_type = 'WaitPage'
+
+    def get_context_data(self):
+        context = GenericWaitPageMixin.get_context_data(self)
+        return FormPageOrInGameWaitPage.get_context_data(self, **context)
+
+    def get_template_name(self):
+        """fallback to otree/WaitPage.html, which is guaranteed to exist.
+        the reason for the 'if' statement, rather than returning a list,
+        is that if the user explicitly defined template_name, and that template
+        does not exist, then we should not fail silently.
+        (for example, the user forgot to add it to git)
+        """
+        if self.template_name:
+            return self.template_name
+
+        if Path('_templates/global/WaitPage.html').exists():
+            return 'global/WaitPage.html'
+        return 'otree/WaitPage.html'
+
+    def inner_dispatch(self, request):
+        # we need inner_dispatch() for common interface w/ parent class
+        # and .get() so it can be called explicitly.
+        return self.get()
+
+    def get(self):
+        # necessary because queries are made directly from DB
+
+        if self.wait_for_all_groups == True:
+            resp = self.inner_dispatch_subsession()
+        elif self.group_by_arrival_time:
+            resp = self.inner_dispatch_gbat()
+        else:
+            resp = self.inner_dispatch_group()
+        return resp
+
+    def _run_aapa_and_notify(self, group_or_subsession):
+        '''
+        group_or_subsession is passed explicitly, because in the case of GBAT it might
+        not include the current player, so we can't just use self.player.group.
+
+        new design is that if anybody is waiting on the wait page, we run AAPA.
+        If nobody is shown the wait page, we don't need to notify or even create a
+        CompletedGroupWaitPage record.
+        '''
+        if self.wait_for_all_groups:
+            group = None
+            noself_kwargs = dict(subsession=group_or_subsession)
+        else:
+            group = group_or_subsession
+            noself_kwargs = dict(group=group_or_subsession)
+
+        aapa = type(self).after_all_players_arrive
+        if isinstance(aapa, str):
+            group_or_subsession.call_user_defined(aapa)
+        # old format; it's a regular method
+        elif str(inspect.signature(aapa)) == '(self)':
+            wp: WaitPage = type(self)({'type': 'http'}, None, None)
+            wp.set_attributes_waitpage_clone(original_view=self)
+            wp._group_for_wp_clone = group
+            wp.after_all_players_arrive()
+        else:
+            # noself
+            # pass kwargs so that we can ensure the user did not use a group method
+            # where a subsession method should have been used
+            aapa(**noself_kwargs)
+        self._mark_completed_and_notify(group=group)
+
+    def inner_dispatch_group(self):
+        ## EARLY EXITS
+        if CompletedGroupWaitPage.objects_exists(
+            page_index=self._index_in_pages,
+            group_id=self.player.group_id,
+            session_id=self._session_pk,
+        ):
+            return self._response_when_ready()
+        is_displayed = self._is_displayed()
+        is_last, someone_waiting = self._tally_unvisited()
+        if is_displayed and not is_last:
+            return self._get_wait_page()
+        elif is_last and (someone_waiting or is_displayed):
+            self._run_aapa_and_notify(self.group)
+        return self._response_when_ready()
+
+    def inner_dispatch_subsession(self):
+
+        if CompletedSubsessionWaitPage.objects_exists(
+            page_index=self._index_in_pages, session=self.session
+        ):
+            return self._response_when_ready()
+
+        is_displayed = self._is_displayed()
+        is_last, someone_waiting = self._tally_unvisited()
+        if is_displayed and not is_last:
+            return self._get_wait_page()
+        elif is_last and (someone_waiting or is_displayed):
+            self._run_aapa_and_notify(self.subsession)
+        return self._response_when_ready()
+
+    def inner_dispatch_gbat(self):
+        if CompletedGBATWaitPage.objects_exists(
+            page_index=self._index_in_pages,
+            id_in_subsession=self.group.id_in_subsession,
+            session=self.session,
+        ):
+            return self._response_when_ready()
+
+        if not self._is_displayed():
+            # in GBAT, either all players should skip a page, or none should.
+            # we don't support some players skipping and others not.
+            return self._response_when_ready()
+
+        participant = self.participant
+
+        participant._gbat_is_connected = True
+        participant._gbat_page_index = self._index_in_pages
+        participant._gbat_grouped = False
+        # _last_request_timestamp is already set in set_attributes,
+        # but set it here just so we can guarantee
+        participant._last_request_timestamp = int(time.time())
+        # need to save it inside the lock (check-then-act)
+        # also because it needs to be up to date for get_players_for_group
+        # which gets this info from the DB
+        # make a clean copy for GBAT and AAPA
+        # self.player and self.participant etc are undefined
+        # and no objects are cached inside it
+        # and it doesn't affect the current instance
+
+        gbat_new_group = self.subsession._gbat_try_to_make_new_group(
+            self._index_in_pages
+        )
+
+        if gbat_new_group:
+            self._run_aapa_and_notify(gbat_new_group)
+            # gbat_new_group may not include the current player!
+            # maybe this will not work if i change the implementation
+            # so that the player is cached,
+            # but that's OK because it will be obvious it doesn't work.
+
+            if participant._gbat_grouped:
+                return self._response_when_ready()
+
+        return self._get_wait_page()
+
+    @property
+    def _group_or_subsession(self):
+        return self.subsession if self.wait_for_all_groups else self.group
+
+    def _get_participants_for_this_waitpage(self, group_or_subsession):
+        """
+        group_or_subsession needs to be passed because it could be a newly created group with GBAT,
+        and may not equal self.group because the current player may not be part of the group.
+        (for example, when creating single-player groups with waiting_too_long).
+        """
+        Player = self.PlayerClass
+        fk_field = Player.subsession_id if self.wait_for_all_groups else Player.group_id
+        # tried select_from but my filter clause didn't work
+        return (
+            dbq(Player)
+            .join(Participant)
+            .filter(fk_field == group_or_subsession.id)
+            .with_entities(Participant)
+        )
+
+    # this is needed because on wait pages, self.player doesn't exist.
+    # usually oTree finds the group by doing self.player.group.
+    _group_for_wp_clone = None
+
+    @property
+    def group(self):
+        return self._group_for_wp_clone or super().group
+
+    def _mark_page_completions(self, participants: List[Participant]):
+        '''
+        this is more accurate than page load,
+        because the player may delay doing that,
+        to make it look like they waited longer.
+        '''
+        app_name = self.player.get_folder_name()
+        session_code = self.participant._session_code
+
+        for pp in participants:
+            otree.common2.make_page_completion_row(
+                view=self,
+                app_name=app_name,
+                participant__id_in_session=pp.id_in_session,
+                participant__code=pp.code,
+                session_code=session_code,
+                is_wait_page=1,
+            )
+
+    def _mark_completed_and_notify(self, group: Optional[BaseGroup]):
+        # if group is not passed, then it's the whole subsession
+        # could be 2 people creating the record at the same time
+        # in _increment_index_in_pages, so could end up creating 2 records
+        # but it's not a problem.
+
+        base_kwargs = dict(page_index=self._index_in_pages, session_id=self._session_pk)
+        Player = self.PlayerClass
+
+        if self.wait_for_all_groups:
+            CompletedSubsessionWaitPage.objects_create(**base_kwargs)
+        elif self.group_by_arrival_time:
+            db.add(
+                CompletedGBATWaitPage(
+                    **base_kwargs, id_in_subsession=group.id_in_subsession
+                )
+            )
+        else:
+            db.add(CompletedGroupWaitPage(**base_kwargs, group_id=group.id))
+
+        participants = self._get_participants_for_this_waitpage(
+            group or self.subsession
+        )
+        self._mark_page_completions(list(participants))
+        for pp in participants:
+            pp._last_page_timestamp = int(time.time())
+
+        # this can cause messages to get wrongly enqueued in the botworker
+        if otree.common.USE_TIMEOUT_WORKER and not self.participant.is_browser_bot:
+            # 2016-11-15: we used to only ensure the next page is visited
+            # if the next page has a timeout, or if it's a wait page
+            # but this is not reliable because next page might be skipped anyway,
+            # and we don't know what page will actually be shown next to the user.
+            otree.tasks.ensure_pages_visited(
+                participant_pks=[pp.id for pp in participants],
+                delay=10,
+                page_index=self._index_in_pages,
+            )
+
+        if self.group_by_arrival_time:
+            channel_utils.sync_group_send(
+                group=channel_utils.gbat_group_name(**base_kwargs),
+                data={'status': 'ready'},
+            )
+        else:
+            if self.wait_for_all_groups:
+                channels_group_name = channel_utils.subsession_wait_page_name(
+                    **base_kwargs
+                )
+            else:
+                channels_group_name = channel_utils.group_wait_page_name(
+                    **base_kwargs, group_id=group.id
+                )
+
+            channel_utils.sync_group_send(
+                group=channels_group_name, data={'status': 'ready'}
+            )
+
+    def socket_url(self):
+        session_pk = self._session_pk
+        page_index = self._index_in_pages
+        participant_id = self.participant.id
+        if self.group_by_arrival_time:
+            return channel_utils.gbat_path(
+                session_pk=session_pk,
+                page_index=page_index,
+                app_name=self.player.get_folder_name(),
+                participant_id=participant_id,
+                player_id=self.player.id,
+            )
+        elif self.wait_for_all_groups:
+            return channel_utils.subsession_wait_page_path(
+                session_pk=session_pk,
+                page_index=page_index,
+                participant_id=participant_id,
+            )
+        else:
+            return channel_utils.group_wait_page_path(
+                session_pk=session_pk,
+                page_index=page_index,
+                participant_id=participant_id,
+                group_id=self.player.group_id,
+            )
+
+    def _tally_unvisited(self):
+
+        participants = self._get_participants_for_this_waitpage(
+            self._group_or_subsession
+        )
+        session_code = self.participant._session_code
+
+        visited = []
+        unvisited = []
+        for p in participants:
+            [unvisited, visited][p._index_in_pages >= self._index_in_pages].append(p)
+
+        # this is not essential to functionality.
+        # just for the display in the Monitor tab.
+        if len(unvisited) <= 3:
+            if len(unvisited) == 0:
+                note = ''
+            else:
+                note = ', '.join(p._numeric_label() for p in unvisited)
+
+                for p in visited:
+                    p._monitor_note = note
+
+            channel_utils.sync_group_send(
+                group=channel_utils.session_monitor_group_name(session_code),
+                data=dict(
+                    ids=[p.id_in_session for p in visited],
+                    note=note,
+                    type='update_notes',
+                ),
+            )
+
+        # is_last is not technically true. maybe someone else also is waiting for this page
+        # just behind you. but it doesn't matter; you can still advance the waitpage.
+        is_last = not bool(unvisited)
+        someone_waiting = any(
+            [
+                p._index_in_pages == self._index_in_pages and p.is_on_wait_page
+                for p in participants
+            ]
+        )
+        return (is_last, someone_waiting)
+
+    def is_displayed(self):
+        return True
+
+    def _response_when_ready(self):
+        '''
+        Before calling this function, the following must be satisfied:
+        - The completion object exists
+        OR
+        - The player skips this page
+        '''
+        participant = self.participant
+        participant.is_on_wait_page = False
+        participant._monitor_note = None
+        self._increment_index_in_pages()
+        return self._redirect_to_page_the_user_should_be_on()
+
+    def after_all_players_arrive(self):
+        pass
+
+    def _get_default_body_text(self):
+        num_other_players = self._group_or_subsession.player_set.count() - 1
+        if num_other_players > 1:
+            return core_gettext('Waiting for the other participants.')
+        if num_other_players == 1:
+            return core_gettext('Waiting for the other participant.')
+        return ''
+
+
+class InvalidAppError(Exception):
+    pass
+
+
+class MockForm:
+    def __iter__(self):
+        if False:
+            yield
+
+    def __init__(self, error_message=None):
+        self.non_field_error = error_message
+
+    field_names = []
+
+    @property
+    def errors(self):
+        return bool(self.non_field_error)
```

### Comparing `otree-6.0.0a8/otree/views/admin.py` & `otree-6.0.0a9/otree/views/admin.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/views/cbv.py` & `otree-6.0.0a9/otree/views/cbv.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/views/demo.py` & `otree-6.0.0a9/otree/views/demo.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/views/export.py` & `otree-6.0.0a9/otree/views/export.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/views/mturk.py` & `otree-6.0.0a9/otree/views/mturk.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/views/participant.py` & `otree-6.0.0a9/otree/views/participant.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/views/rest.py` & `otree-6.0.0a9/otree/views/rest.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree/views/room.py` & `otree-6.0.0a9/otree/views/room.py`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/otree.egg-info/PKG-INFO` & `otree-6.0.0a9/otree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otree
-Version: 6.0.0a8
+Version: 6.0.0a9
 Summary: Framework for multiplayer strategy games and complex surveys.
 Home-page: http://otree.org/
 Author: chris@otree.org
 Author-email: chris@otree.org
 License: MIT License
 Platform: UNKNOWN
 Provides-Extra: mturk
```

### Comparing `otree-6.0.0a8/otree.egg-info/SOURCES.txt` & `otree-6.0.0a9/otree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otree-6.0.0a8/setup.py` & `otree-6.0.0a9/setup.py`

 * *Files identical despite different names*

