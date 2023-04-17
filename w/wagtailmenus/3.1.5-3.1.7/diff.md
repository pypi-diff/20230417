# Comparing `tmp/wagtailmenus-3.1.5.tar.gz` & `tmp/wagtailmenus-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailmenus-3.1.5.tar", last modified: Tue Feb 21 11:20:35 2023, max compression
+gzip compressed data, was "wagtailmenus-3.1.7.tar", last modified: Mon Apr 17 05:04:15 2023, max compression
```

## Comparing `wagtailmenus-3.1.5.tar` & `wagtailmenus-3.1.7.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.734230 wagtailmenus-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    34180 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-02-21 11:20:35.734230 wagtailmenus-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 11:20:35.734230 wagtailmenus-3.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.710229 wagtailmenus-3.1.5/wagtailmenus/
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.714229 wagtailmenus-3.1.5/wagtailmenus/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/conf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/conf/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.714229 wagtailmenus-3.1.5/wagtailmenus/conf/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/conf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/conf/tests/test_modeladmin_disable_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.706229 wagtailmenus-3.1.5/wagtailmenus/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.706229 wagtailmenus-3.1.5/wagtailmenus/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.714229 wagtailmenus-3.1.5/wagtailmenus/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.706229 wagtailmenus-3.1.5/wagtailmenus/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.714229 wagtailmenus-3.1.5/wagtailmenus/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.706229 wagtailmenus-3.1.5/wagtailmenus/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.714229 wagtailmenus-3.1.5/wagtailmenus/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.706229 wagtailmenus-3.1.5/wagtailmenus/locale/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.714229 wagtailmenus-3.1.5/wagtailmenus/locale/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/es_419/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/es_419/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.706229 wagtailmenus-3.1.5/wagtailmenus/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.714229 wagtailmenus-3.1.5/wagtailmenus/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.706229 wagtailmenus-3.1.5/wagtailmenus/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.714229 wagtailmenus-3.1.5/wagtailmenus/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.706229 wagtailmenus-3.1.5/wagtailmenus/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.714229 wagtailmenus-3.1.5/wagtailmenus/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.706229 wagtailmenus-3.1.5/wagtailmenus/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.714229 wagtailmenus-3.1.5/wagtailmenus/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.706229 wagtailmenus-3.1.5/wagtailmenus/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.718229 wagtailmenus-3.1.5/wagtailmenus/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.706229 wagtailmenus-3.1.5/wagtailmenus/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.718229 wagtailmenus-3.1.5/wagtailmenus/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.718229 wagtailmenus-3.1.5/wagtailmenus/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.718229 wagtailmenus-3.1.5/wagtailmenus/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/management/commands/autopopulate_main_menus.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.718229 wagtailmenus-3.1.5/wagtailmenus/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0002_auto_20160129_0901.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0003_auto_20160129_2339.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0004_auto_20160130_0024.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0005_auto_20160130_2209.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0006_auto_20160131_1347.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0007_auto_20160131_2000.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0008_auto_20160131_2327.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0009_auto_20160201_0859.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0010_auto_20160201_1558.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0011_auto_20160415_1519.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0012_auto_20160419_0039.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0013_auto_20160423_1124.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0014_auto_20160423_1339.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0015_auto_20160423_1348.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0016_auto_20160930_0645.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0017_auto_20161013_1658.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0018_auto_20161204_2043.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0019_auto_20161204_2143.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0020_auto_20161210_0004.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0021_auto_20170106_2352.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0022_auto_20170913_2125.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/0023_remove_use_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/modeladmin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.722229 wagtailmenus-3.1.5/wagtailmenus/models/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/models/menuitems.py
--rw-r--r--   0 runner    (1001) docker     (123)    51793 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/models/menus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/models/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/models/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/panels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.722229 wagtailmenus-3.1.5/wagtailmenus/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/settings/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.706229 wagtailmenus-3.1.5/wagtailmenus/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.706229 wagtailmenus-3.1.5/wagtailmenus/static/wagtailmenus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.722229 wagtailmenus-3.1.5/wagtailmenus/static/wagtailmenus/js/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/static/wagtailmenus/js/site-switcher.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.710229 wagtailmenus-3.1.5/wagtailmenus/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.722229 wagtailmenus-3.1.5/wagtailmenus/templates/menus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.722229 wagtailmenus-3.1.5/wagtailmenus/templates/menus/bootstrap3/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/templates/menus/bootstrap3/main_menu_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/templates/menus/bootstrap3/main_menu_dropdown_hover.html
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/templates/menus/bootstrap3/sub_menu_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/templates/menus/bootstrap3/sub_menu_dropdown_hover.html
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/templates/menus/children_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/templates/menus/flat_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/templates/menus/main_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/templates/menus/section_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/templates/menus/section_menu_heirarchical.html
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/templates/menus/sub_menu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.722229 wagtailmenus-3.1.5/wagtailmenus/templates/wagtailmenus/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/templates/wagtailmenus/flatmenu_copy.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.722229 wagtailmenus-3.1.5/wagtailmenus/templates/wagtailmenus/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/templates/wagtailmenus/includes/header.html
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/templates/wagtailmenus/includes/header_with_site_switcher.html
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/templates/wagtailmenus/mainmenu_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.722229 wagtailmenus-3.1.5/wagtailmenus/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/templatetags/menu_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.726230 wagtailmenus-3.1.5/wagtailmenus/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.726230 wagtailmenus-3.1.5/wagtailmenus/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/fixtures/perms.json
--rw-r--r--   0 runner    (1001) docker     (123)    30544 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/fixtures/test.json
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/fixtures/test_custom_models.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.730229 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0002_homepage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0003_auto_20160418_1204.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0004_auto_20160419_2022.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0005_auto_20160419_2025.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0006_auto_20160423_1339.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0007_auto_20160423_1348.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0008_contactpage.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0009_typicalpage.py
--rw-r--r--   0 runner    (1001) docker     (123)    13664 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0010_auto_20161211_2116.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0011_auto_20170106_2355.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0012_linkpage.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0013_auto_20170630_1002.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0014_noabsoluteurlspage.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0015_remove_use_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0016_articlelistpage_articlepage.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/modeladmin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.730229 wagtailmenus-3.1.5/wagtailmenus/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/models/menus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/models/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.730229 wagtailmenus-3.1.5/wagtailmenus/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/templates/homepage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.730229 wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.730229 wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/custom-overrides/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/custom-overrides/children.html
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/custom-overrides/section-sub.html
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/custom_section_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/custom_sub_menu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.730229 wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/flat/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.730229 wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/flat/header-secondary/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/flat/header-secondary/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/flat/header-secondary/sub_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/flat/sub_menu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.730229 wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/main/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/main/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/main/sub_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/sub_menu_level_2.html
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/sub_menu_level_3.html
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/templates/sub_menu-tag-used-directly.html
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/templates/typical-page.html
--rw-r--r--   0 runner    (1001) docker     (123)    10917 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/test_base_menu_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/test_childrenmenu_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/test_custom_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/test_flatmenu_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/test_mainmenu_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/test_menu_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/test_menu_items.py
--rw-r--r--   0 runner    (1001) docker     (123)    67291 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/test_menu_rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/test_page_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/test_sectionmenu_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/test_test_page_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.730229 wagtailmenus-3.1.5/wagtailmenus/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/utils/inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.734230 wagtailmenus-3.1.5/wagtailmenus/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/utils/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-02-21 11:20:25.000000 wagtailmenus-3.1.5/wagtailmenus/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:20:35.714229 wagtailmenus-3.1.5/wagtailmenus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-02-21 11:20:35.000000 wagtailmenus-3.1.5/wagtailmenus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-02-21 11:20:35.000000 wagtailmenus-3.1.5/wagtailmenus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 11:20:35.000000 wagtailmenus-3.1.5/wagtailmenus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 11:20:35.000000 wagtailmenus-3.1.5/wagtailmenus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-21 11:20:35.000000 wagtailmenus-3.1.5/wagtailmenus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-21 11:20:35.000000 wagtailmenus-3.1.5/wagtailmenus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.123889 wagtailmenus-3.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    34180 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-17 05:04:15.123889 wagtailmenus-3.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 05:04:15.123889 wagtailmenus-3.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.091888 wagtailmenus-3.1.7/wagtailmenus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.095888 wagtailmenus-3.1.7/wagtailmenus/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/conf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/conf/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.095888 wagtailmenus-3.1.7/wagtailmenus/conf/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/conf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/conf/tests/test_modeladmin_disable_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.083888 wagtailmenus-3.1.7/wagtailmenus/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.083888 wagtailmenus-3.1.7/wagtailmenus/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.095888 wagtailmenus-3.1.7/wagtailmenus/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.083888 wagtailmenus-3.1.7/wagtailmenus/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.095888 wagtailmenus-3.1.7/wagtailmenus/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.083888 wagtailmenus-3.1.7/wagtailmenus/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.095888 wagtailmenus-3.1.7/wagtailmenus/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.083888 wagtailmenus-3.1.7/wagtailmenus/locale/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.095888 wagtailmenus-3.1.7/wagtailmenus/locale/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/es_419/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/es_419/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.083888 wagtailmenus-3.1.7/wagtailmenus/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.095888 wagtailmenus-3.1.7/wagtailmenus/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.083888 wagtailmenus-3.1.7/wagtailmenus/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.099888 wagtailmenus-3.1.7/wagtailmenus/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.083888 wagtailmenus-3.1.7/wagtailmenus/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.099888 wagtailmenus-3.1.7/wagtailmenus/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.083888 wagtailmenus-3.1.7/wagtailmenus/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.099888 wagtailmenus-3.1.7/wagtailmenus/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.083888 wagtailmenus-3.1.7/wagtailmenus/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.099888 wagtailmenus-3.1.7/wagtailmenus/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    12354 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.083888 wagtailmenus-3.1.7/wagtailmenus/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.099888 wagtailmenus-3.1.7/wagtailmenus/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.099888 wagtailmenus-3.1.7/wagtailmenus/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.099888 wagtailmenus-3.1.7/wagtailmenus/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/management/commands/autopopulate_main_menus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.103889 wagtailmenus-3.1.7/wagtailmenus/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0002_auto_20160129_0901.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0003_auto_20160129_2339.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0004_auto_20160130_0024.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0005_auto_20160130_2209.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0006_auto_20160131_1347.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0007_auto_20160131_2000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0008_auto_20160131_2327.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0009_auto_20160201_0859.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0010_auto_20160201_1558.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0011_auto_20160415_1519.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0012_auto_20160419_0039.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0013_auto_20160423_1124.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0014_auto_20160423_1339.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0015_auto_20160423_1348.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0016_auto_20160930_0645.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0017_auto_20161013_1658.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0018_auto_20161204_2043.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0019_auto_20161204_2143.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0020_auto_20161210_0004.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0021_auto_20170106_2352.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0022_auto_20170913_2125.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/0023_remove_use_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/modeladmin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.107889 wagtailmenus-3.1.7/wagtailmenus/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/models/menuitems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51886 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/models/menus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/models/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/models/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/panels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.107889 wagtailmenus-3.1.7/wagtailmenus/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/settings/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.087888 wagtailmenus-3.1.7/wagtailmenus/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.087888 wagtailmenus-3.1.7/wagtailmenus/static/wagtailmenus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.107889 wagtailmenus-3.1.7/wagtailmenus/static/wagtailmenus/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/static/wagtailmenus/js/site-switcher.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.087888 wagtailmenus-3.1.7/wagtailmenus/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.107889 wagtailmenus-3.1.7/wagtailmenus/templates/menus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.107889 wagtailmenus-3.1.7/wagtailmenus/templates/menus/bootstrap3/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/templates/menus/bootstrap3/main_menu_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/templates/menus/bootstrap3/main_menu_dropdown_hover.html
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/templates/menus/bootstrap3/sub_menu_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/templates/menus/bootstrap3/sub_menu_dropdown_hover.html
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/templates/menus/children_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/templates/menus/flat_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/templates/menus/main_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/templates/menus/section_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/templates/menus/section_menu_heirarchical.html
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/templates/menus/sub_menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.107889 wagtailmenus-3.1.7/wagtailmenus/templates/wagtailmenus/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/templates/wagtailmenus/flatmenu_copy.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.111889 wagtailmenus-3.1.7/wagtailmenus/templates/wagtailmenus/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/templates/wagtailmenus/includes/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/templates/wagtailmenus/includes/header_with_site_switcher.html
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/templates/wagtailmenus/mainmenu_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.111889 wagtailmenus-3.1.7/wagtailmenus/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/templatetags/menu_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.115889 wagtailmenus-3.1.7/wagtailmenus/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.115889 wagtailmenus-3.1.7/wagtailmenus/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/fixtures/perms.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30544 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/fixtures/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/fixtures/test_custom_models.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.119889 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0002_homepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0003_auto_20160418_1204.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0004_auto_20160419_2022.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0005_auto_20160419_2025.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0006_auto_20160423_1339.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0007_auto_20160423_1348.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0008_contactpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0009_typicalpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13664 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0010_auto_20161211_2116.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0011_auto_20170106_2355.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0012_linkpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0013_auto_20170630_1002.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0014_noabsoluteurlspage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0015_remove_use_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0016_articlelistpage_articlepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/modeladmin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.119889 wagtailmenus-3.1.7/wagtailmenus/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/models/menus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/models/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.119889 wagtailmenus-3.1.7/wagtailmenus/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/templates/homepage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.119889 wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.119889 wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/custom-overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/custom-overrides/children.html
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/custom-overrides/section-sub.html
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/custom_section_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/custom_sub_menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.123889 wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/flat/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.123889 wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/flat/header-secondary/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/flat/header-secondary/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/flat/header-secondary/sub_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/flat/sub_menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.123889 wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/main/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/main/sub_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/sub_menu_level_2.html
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/sub_menu_level_3.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/templates/sub_menu-tag-used-directly.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/templates/typical-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10917 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/test_base_menu_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/test_childrenmenu_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/test_custom_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/test_flatmenu_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/test_mainmenu_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/test_menu_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/test_menu_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67291 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/test_menu_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/test_page_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/test_sectionmenu_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/test_test_page_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.123889 wagtailmenus-3.1.7/wagtailmenus/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/utils/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.123889 wagtailmenus-3.1.7/wagtailmenus/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/utils/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-17 05:04:00.000000 wagtailmenus-3.1.7/wagtailmenus/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 05:04:15.091888 wagtailmenus-3.1.7/wagtailmenus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-17 05:04:15.000000 wagtailmenus-3.1.7/wagtailmenus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-17 05:04:15.000000 wagtailmenus-3.1.7/wagtailmenus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 05:04:15.000000 wagtailmenus-3.1.7/wagtailmenus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 05:04:15.000000 wagtailmenus-3.1.7/wagtailmenus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-17 05:04:15.000000 wagtailmenus-3.1.7/wagtailmenus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 05:04:15.000000 wagtailmenus-3.1.7/wagtailmenus.egg-info/top_level.txt
```

### Comparing `wagtailmenus-3.1.5/CHANGELOG.md` & `wagtailmenus-3.1.7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/LICENSE.txt` & `wagtailmenus-3.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/PKG-INFO` & `wagtailmenus-3.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: wagtailmenus
-Version: 3.1.5
+Version: 3.1.7
 Summary: An app to help you manage menus in your Wagtail projects more consistently.
 Home-page: https://github.com/jazzband/wagtailmenus/tree/stable/3.1.x
-Download-URL: https://github.com/jazzband/wagtailmenus/tarball/v3.1.5
+Download-URL: https://github.com/jazzband/wagtailmenus/tarball/v3.1.7
 Author: Andy Babic
 Author-email: ababic@rkh.co.uk
 License: MIT
 Keywords: wagtail cms model utility
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Wagtail :: 2
 Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
```

### Comparing `wagtailmenus-3.1.5/README.rst` & `wagtailmenus-3.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/runtests.py` & `wagtailmenus-3.1.7/runtests.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/setup.py` & `wagtailmenus-3.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         "Operating System :: OS Independent",
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
         'Framework :: Wagtail :: 2',
         'Framework :: Wagtail :: 3',
         'Framework :: Wagtail :: 4',
```

### Comparing `wagtailmenus-3.1.5/wagtailmenus/__init__.py` & `wagtailmenus-3.1.7/wagtailmenus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from wagtailmenus.utils.version import get_stable_branch_name, get_version
 
 # major.minor.patch.release.number
 # release must be one of alpha, beta, rc, or final
-VERSION = (3, 1, 5, "final", 0)
+VERSION = (3, 1, 7, "final", 0)
 __version__ = get_version(VERSION)
 stable_branch_name = get_stable_branch_name(VERSION)
 
 default_app_config = "wagtailmenus.apps.WagtailMenusConfig"
 
 
 def get_main_menu_model_string():
```

### Comparing `wagtailmenus-3.1.5/wagtailmenus/conf/defaults.py` & `wagtailmenus-3.1.7/wagtailmenus/conf/defaults.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/conf/tests/test_modeladmin_disable_settings.py` & `wagtailmenus-3.1.7/wagtailmenus/conf/tests/test_modeladmin_disable_settings.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/context_processors.py` & `wagtailmenus-3.1.7/wagtailmenus/context_processors.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/errors.py` & `wagtailmenus-3.1.7/wagtailmenus/errors.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/forms.py` & `wagtailmenus-3.1.7/wagtailmenus/forms.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/ar/LC_MESSAGES/django.mo` & `wagtailmenus-3.1.7/wagtailmenus/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/ar/LC_MESSAGES/django.po` & `wagtailmenus-3.1.7/wagtailmenus/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/de/LC_MESSAGES/django.mo` & `wagtailmenus-3.1.7/wagtailmenus/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/de/LC_MESSAGES/django.po` & `wagtailmenus-3.1.7/wagtailmenus/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/en/LC_MESSAGES/django.po` & `wagtailmenus-3.1.7/wagtailmenus/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/es_419/LC_MESSAGES/django.mo` & `wagtailmenus-3.1.7/wagtailmenus/locale/es_419/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/es_419/LC_MESSAGES/django.po` & `wagtailmenus-3.1.7/wagtailmenus/locale/es_419/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/fr/LC_MESSAGES/django.mo` & `wagtailmenus-3.1.7/wagtailmenus/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/fr/LC_MESSAGES/django.po` & `wagtailmenus-3.1.7/wagtailmenus/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/it/LC_MESSAGES/django.mo` & `wagtailmenus-3.1.7/wagtailmenus/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/it/LC_MESSAGES/django.po` & `wagtailmenus-3.1.7/wagtailmenus/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/lt/LC_MESSAGES/django.mo` & `wagtailmenus-3.1.7/wagtailmenus/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/lt/LC_MESSAGES/django.po` & `wagtailmenus-3.1.7/wagtailmenus/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/pt_BR/LC_MESSAGES/django.mo` & `wagtailmenus-3.1.7/wagtailmenus/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/pt_BR/LC_MESSAGES/django.po` & `wagtailmenus-3.1.7/wagtailmenus/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/ru/LC_MESSAGES/django.mo` & `wagtailmenus-3.1.7/wagtailmenus/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/ru/LC_MESSAGES/django.po` & `wagtailmenus-3.1.7/wagtailmenus/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/zh_CN/LC_MESSAGES/django.mo` & `wagtailmenus-3.1.7/wagtailmenus/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/locale/zh_CN/LC_MESSAGES/django.po` & `wagtailmenus-3.1.7/wagtailmenus/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/management/commands/autopopulate_main_menus.py` & `wagtailmenus-3.1.7/wagtailmenus/management/commands/autopopulate_main_menus.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0001_initial.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0002_auto_20160129_0901.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0002_auto_20160129_0901.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0003_auto_20160129_2339.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0003_auto_20160129_2339.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0004_auto_20160130_0024.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0004_auto_20160130_0024.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0005_auto_20160130_2209.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0005_auto_20160130_2209.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0006_auto_20160131_1347.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0006_auto_20160131_1347.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0007_auto_20160131_2000.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0007_auto_20160131_2000.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0008_auto_20160131_2327.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0008_auto_20160131_2327.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0011_auto_20160415_1519.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0011_auto_20160415_1519.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0012_auto_20160419_0039.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0012_auto_20160419_0039.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0013_auto_20160423_1124.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0013_auto_20160423_1124.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0014_auto_20160423_1339.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0014_auto_20160423_1339.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0015_auto_20160423_1348.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0015_auto_20160423_1348.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0016_auto_20160930_0645.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0016_auto_20160930_0645.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0017_auto_20161013_1658.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0017_auto_20161013_1658.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0018_auto_20161204_2043.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0018_auto_20161204_2043.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0019_auto_20161204_2143.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0019_auto_20161204_2143.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0020_auto_20161210_0004.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0020_auto_20161210_0004.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0021_auto_20170106_2352.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0021_auto_20170106_2352.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/migrations/0022_auto_20170913_2125.py` & `wagtailmenus-3.1.7/wagtailmenus/migrations/0022_auto_20170913_2125.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/modeladmin.py` & `wagtailmenus-3.1.7/wagtailmenus/modeladmin.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/models/menuitems.py` & `wagtailmenus-3.1.7/wagtailmenus/models/menuitems.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/models/menus.py` & `wagtailmenus-3.1.7/wagtailmenus/models/menus.py`

 * *Files 0% similar despite different names*

```diff
@@ -493,14 +493,16 @@
         # NOTE: Attributes aren't being set yet, as the item could potentially
         # be replaced
 
         active_class = ''
 
         if option_vals.apply_active_classes:
             if page:
+                if (page.pk != page.localized.pk):
+                    page = page.localized
                 if(current_page and page.pk == current_page.pk):
                     # This is the current page, so the menu item should
                     # probably have the 'active' class
                     active_class = settings.ACTIVE_CLASS
                     if (
                         option_vals.allow_repeating_parents and
                         has_children_in_menu
```

### Comparing `wagtailmenus-3.1.5/wagtailmenus/models/mixins.py` & `wagtailmenus-3.1.7/wagtailmenus/models/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/models/pages.py` & `wagtailmenus-3.1.7/wagtailmenus/models/pages.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/panels.py` & `wagtailmenus-3.1.7/wagtailmenus/panels.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/settings/base.py` & `wagtailmenus-3.1.7/wagtailmenus/settings/base.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/templates/menus/bootstrap3/main_menu_dropdown.html` & `wagtailmenus-3.1.7/wagtailmenus/templates/menus/bootstrap3/main_menu_dropdown.html`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/templates/menus/bootstrap3/main_menu_dropdown_hover.html` & `wagtailmenus-3.1.7/wagtailmenus/templates/menus/bootstrap3/main_menu_dropdown_hover.html`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/templates/menus/bootstrap3/sub_menu_dropdown.html` & `wagtailmenus-3.1.7/wagtailmenus/templates/menus/bootstrap3/sub_menu_dropdown.html`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/templates/menus/bootstrap3/sub_menu_dropdown_hover.html` & `wagtailmenus-3.1.7/wagtailmenus/templates/menus/bootstrap3/sub_menu_dropdown_hover.html`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/templates/menus/flat_menu.html` & `wagtailmenus-3.1.7/wagtailmenus/templates/menus/flat_menu.html`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/templates/menus/section_menu.html` & `wagtailmenus-3.1.7/wagtailmenus/templates/menus/section_menu.html`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/templates/menus/section_menu_heirarchical.html` & `wagtailmenus-3.1.7/wagtailmenus/templates/menus/section_menu_heirarchical.html`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/templates/wagtailmenus/includes/header.html` & `wagtailmenus-3.1.7/wagtailmenus/templates/wagtailmenus/includes/header.html`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/templates/wagtailmenus/mainmenu_edit.html` & `wagtailmenus-3.1.7/wagtailmenus/templates/wagtailmenus/mainmenu_edit.html`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/templatetags/menu_tags.py` & `wagtailmenus-3.1.7/wagtailmenus/templatetags/menu_tags.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/base.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/fixtures/test.json` & `wagtailmenus-3.1.7/wagtailmenus/tests/fixtures/test.json`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/fixtures/test_custom_models.json` & `wagtailmenus-3.1.7/wagtailmenus/tests/fixtures/test_custom_models.json`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0001_initial.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0002_homepage.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0002_homepage.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0003_auto_20160418_1204.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0003_auto_20160418_1204.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0004_auto_20160419_2022.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0004_auto_20160419_2022.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0005_auto_20160419_2025.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0005_auto_20160419_2025.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0006_auto_20160423_1339.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0006_auto_20160423_1339.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0007_auto_20160423_1348.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0007_auto_20160423_1348.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0008_contactpage.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0008_contactpage.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0009_typicalpage.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0009_typicalpage.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0010_auto_20161211_2116.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0010_auto_20161211_2116.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0011_auto_20170106_2355.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0011_auto_20170106_2355.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0012_linkpage.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0012_linkpage.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0013_auto_20170630_1002.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0013_auto_20170630_1002.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0014_noabsoluteurlspage.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0014_noabsoluteurlspage.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/migrations/0016_articlelistpage_articlepage.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/migrations/0016_articlelistpage_articlepage.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/models/menus.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/models/menus.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/models/pages.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/models/pages.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/models/utils.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/models/utils.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/templates/base.html` & `wagtailmenus-3.1.7/wagtailmenus/tests/templates/base.html`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/templates/homepage.html` & `wagtailmenus-3.1.7/wagtailmenus/tests/templates/homepage.html`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/custom_section_menu.html` & `wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/custom_section_menu.html`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/main/menu.html` & `wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/main/menu.html`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/templates/menus/main/sub_menu.html` & `wagtailmenus-3.1.7/wagtailmenus/tests/templates/menus/main/sub_menu.html`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/templates/page.html` & `wagtailmenus-3.1.7/wagtailmenus/tests/templates/page.html`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/templates/typical-page.html` & `wagtailmenus-3.1.7/wagtailmenus/tests/templates/typical-page.html`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/test_backend.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/test_base_menu_classes.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/test_base_menu_classes.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/test_childrenmenu_class.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/test_childrenmenu_class.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/test_commands.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/test_custom_models.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/test_custom_models.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/test_flatmenu_class.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/test_flatmenu_class.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/test_hooks.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/test_mainmenu_class.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/test_mainmenu_class.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/test_menu_class.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/test_menu_class.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/test_menu_items.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/test_menu_items.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/test_menu_rendering.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/test_menu_rendering.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/test_page_models.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/test_page_models.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/test_sectionmenu_class.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/test_sectionmenu_class.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/test_test_page_models.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/test_test_page_models.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/urls.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/tests/utils.py` & `wagtailmenus-3.1.7/wagtailmenus/tests/utils.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/utils/inspection.py` & `wagtailmenus-3.1.7/wagtailmenus/utils/inspection.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/utils/misc.py` & `wagtailmenus-3.1.7/wagtailmenus/utils/misc.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/utils/tests/test_misc.py` & `wagtailmenus-3.1.7/wagtailmenus/utils/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/utils/version.py` & `wagtailmenus-3.1.7/wagtailmenus/utils/version.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/views.py` & `wagtailmenus-3.1.7/wagtailmenus/views.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus/wagtail_hooks.py` & `wagtailmenus-3.1.7/wagtailmenus/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtailmenus-3.1.5/wagtailmenus.egg-info/PKG-INFO` & `wagtailmenus-3.1.7/wagtailmenus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: wagtailmenus
-Version: 3.1.5
+Version: 3.1.7
 Summary: An app to help you manage menus in your Wagtail projects more consistently.
 Home-page: https://github.com/jazzband/wagtailmenus/tree/stable/3.1.x
-Download-URL: https://github.com/jazzband/wagtailmenus/tarball/v3.1.5
+Download-URL: https://github.com/jazzband/wagtailmenus/tarball/v3.1.7
 Author: Andy Babic
 Author-email: ababic@rkh.co.uk
 License: MIT
 Keywords: wagtail cms model utility
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Wagtail :: 2
 Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
```

### Comparing `wagtailmenus-3.1.5/wagtailmenus.egg-info/SOURCES.txt` & `wagtailmenus-3.1.7/wagtailmenus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

