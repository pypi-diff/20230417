# Comparing `tmp/django-torque-0.4.0.tar.gz` & `tmp/django-torque-0.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-torque-0.4.0.tar", last modified: Tue Mar 28 11:48:19 2023, max compression
+gzip compressed data, was "django-torque-0.5.0a1.tar", last modified: Mon Apr 17 15:31:00 2023, max compression
```

## Comparing `django-torque-0.4.0.tar` & `django-torque-0.5.0a1.tar`

### file list

```diff
@@ -1,69 +1,76 @@
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-03-28 11:48:19.139292 django-torque-0.4.0/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2064 2023-03-28 11:48:19.139292 django-torque-0.4.0/PKG-INFO
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1624 2023-02-19 01:57:21.000000 django-torque-0.4.0/README.md
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-03-28 11:48:19.139292 django-torque-0.4.0/django_torque.egg-info/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2064 2023-03-28 11:48:19.000000 django-torque-0.4.0/django_torque.egg-info/PKG-INFO
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2593 2023-03-28 11:48:19.000000 django-torque-0.4.0/django_torque.egg-info/SOURCES.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        1 2023-03-28 11:48:19.000000 django-torque-0.4.0/django_torque.egg-info/dependency_links.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       61 2023-03-28 11:48:19.000000 django-torque-0.4.0/django_torque.egg-info/requires.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        7 2023-03-28 11:48:19.000000 django-torque-0.4.0/django_torque.egg-info/top_level.txt
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       38 2023-03-28 11:48:19.139292 django-torque-0.4.0/setup.cfg
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1168 2023-02-19 01:57:21.000000 django-torque-0.4.0/setup.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-03-28 11:48:19.127292 django-torque-0.4.0/torque/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       87 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/apps.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-03-28 11:48:19.127292 django-torque-0.4.0/torque/cache_rebuilder/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       72 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/cache_rebuilder/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      475 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/cache_rebuilder/apps.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3592 2023-03-28 11:03:24.000000 django-torque-0.4.0/torque/cache_rebuilder/background.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-03-28 11:48:19.123292 django-torque-0.4.0/torque/management/
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-03-28 11:48:19.127292 django-torque-0.4.0/torque/management/commands/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/management/commands/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1116 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/management/commands/remove_unattached.py
-drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-03-28 11:48:19.139292 django-torque-0.4.0/torque/migrations/
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    12576 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0001_initial.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      437 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0002_auto_20210321_1604.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      451 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0003_auto_20210321_1725.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      729 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0005_auto_20210323_1303.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      573 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0006_auto_20210323_1623.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      839 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0007_auto_20210406_1738.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      373 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0008_auto_20210406_1909.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      403 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0009_sheetconfig_search_cache_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1360 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0010_tableofcontentscache.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      461 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0011_auto_20210416_1739.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      393 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0012_searchcacherow_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      398 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0013_spreadsheet_last_updated.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      404 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0014_tableofcontentscache_rendered_html.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      364 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0015_remove_tableofcontentscache_rendered_data.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2472 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0016_auto_20210721_1444.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      661 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0017_auto_20210721_1621.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      303 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0018_delete_permissiongroup.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      825 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0019_auto_20210721_1720.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      392 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0020_tableofcontents_raw.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      326 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0021_remove_column_type.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      636 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0022_auto_20210905_1430.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      837 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0023_auto_20210905_1454.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      767 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0024_auto_20210905_1535.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      791 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0025_auto_20210905_1624.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      893 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0026_auto_20210905_1638.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1333 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0027_auto_20210905_1642.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1328 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0028_auto_20210905_1659.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2538 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0029_auto_20210905_1716.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      580 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0030_auto_20210927_1304.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      707 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0031_auto_20210930_1328.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      399 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0032_searchcachedocument_filtered_data.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      877 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0033_csvspecification.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1643 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0034_auto_20220209_1209.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      391 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0035_template_in_config.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      803 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0036_remove_searchcachedocument_torque_search_data_ve_0ad953_gin_and_more.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      472 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0037_template_dirty.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      521 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0038_wiki_linked_wiki_keys.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      392 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0039_document_attached.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      456 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/0040_value_unique_value_for_field_document.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      417 2023-03-28 11:03:24.000000 django-torque-0.4.0/torque/migrations/0041_searchcachedocument_explore_rank.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.4.0/torque/migrations/__init__.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    21727 2023-03-28 11:03:24.000000 django-torque-0.4.0/torque/models.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     4809 2023-03-28 11:03:24.000000 django-torque-0.4.0/torque/urls.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3034 2023-03-28 11:03:24.000000 django-torque-0.4.0/torque/utils.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       22 2023-03-28 11:47:17.000000 django-torque-0.4.0/torque/version.py
--rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    35952 2023-03-28 11:03:24.000000 django-torque-0.4.0/torque/views.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-04-17 15:31:00.088729 django-torque-0.5.0a1/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2066 2023-04-17 15:31:00.088729 django-torque-0.5.0a1/PKG-INFO
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1624 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/README.md
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-04-17 15:31:00.088729 django-torque-0.5.0a1/django_torque.egg-info/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2066 2023-04-17 15:31:00.000000 django-torque-0.5.0a1/django_torque.egg-info/PKG-INFO
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3016 2023-04-17 15:31:00.000000 django-torque-0.5.0a1/django_torque.egg-info/SOURCES.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        1 2023-04-17 15:31:00.000000 django-torque-0.5.0a1/django_torque.egg-info/dependency_links.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       68 2023-04-17 15:31:00.000000 django-torque-0.5.0a1/django_torque.egg-info/requires.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        7 2023-04-17 15:31:00.000000 django-torque-0.5.0a1/django_torque.egg-info/top_level.txt
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       38 2023-04-17 15:31:00.088729 django-torque-0.5.0a1/setup.cfg
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1186 2023-04-07 12:16:27.000000 django-torque-0.5.0a1/setup.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-04-17 15:31:00.072728 django-torque-0.5.0a1/torque/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       87 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/apps.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-04-17 15:31:00.076728 django-torque-0.5.0a1/torque/cache_rebuilder/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       72 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/cache_rebuilder/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      475 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/cache_rebuilder/apps.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     6295 2023-04-12 18:43:02.000000 django-torque-0.5.0a1/torque/cache_rebuilder/background.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-04-17 15:31:00.072728 django-torque-0.5.0a1/torque/management/
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-04-17 15:31:00.076728 django-torque-0.5.0a1/torque/management/commands/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/management/commands/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1116 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/management/commands/remove_unattached.py
+drwxr-xr-x   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-04-17 15:31:00.088729 django-torque-0.5.0a1/torque/migrations/
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    12576 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0001_initial.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      437 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0002_auto_20210321_1604.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      451 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0003_auto_20210321_1725.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      729 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0005_auto_20210323_1303.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      573 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0006_auto_20210323_1623.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      839 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0007_auto_20210406_1738.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      373 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0008_auto_20210406_1909.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      403 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0009_sheetconfig_search_cache_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1360 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0010_tableofcontentscache.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      461 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0011_auto_20210416_1739.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      393 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0012_searchcacherow_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      398 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0013_spreadsheet_last_updated.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      404 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0014_tableofcontentscache_rendered_html.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      364 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0015_remove_tableofcontentscache_rendered_data.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2472 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0016_auto_20210721_1444.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      661 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0017_auto_20210721_1621.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      303 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0018_delete_permissiongroup.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      825 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0019_auto_20210721_1720.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      392 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0020_tableofcontents_raw.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      326 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0021_remove_column_type.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      636 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0022_auto_20210905_1430.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      837 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0023_auto_20210905_1454.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      767 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0024_auto_20210905_1535.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      791 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0025_auto_20210905_1624.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      893 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0026_auto_20210905_1638.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1333 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0027_auto_20210905_1642.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1328 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0028_auto_20210905_1659.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     2538 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0029_auto_20210905_1716.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      580 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0030_auto_20210927_1304.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      707 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0031_auto_20210930_1328.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      399 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0032_searchcachedocument_filtered_data.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      877 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0033_csvspecification.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1643 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0034_auto_20220209_1209.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      391 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0035_template_in_config.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      803 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0036_remove_searchcachedocument_torque_search_data_ve_0ad953_gin_and_more.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      472 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0037_template_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      521 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0038_wiki_linked_wiki_keys.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      392 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0039_document_attached.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      456 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/0040_value_unique_value_for_field_document.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      417 2023-03-28 11:03:24.000000 django-torque-0.5.0a1/torque/migrations/0041_searchcachedocument_explore_rank.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1245 2023-04-07 12:16:27.000000 django-torque-0.5.0a1/torque/migrations/0042_documentdictcache.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      461 2023-04-07 12:16:27.000000 django-torque-0.5.0a1/torque/migrations/0043_documentdictcache_unique_document_dict.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      414 2023-04-07 12:16:27.000000 django-torque-0.5.0a1/torque/migrations/0044_documentdictcache_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      669 2023-04-10 15:44:16.000000 django-torque-0.5.0a1/torque/migrations/0045_templatecachedocument_dirty_and_more.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      325 2023-04-10 15:44:16.000000 django-torque-0.5.0a1/torque/migrations/0046_delete_templatecachedocument.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     1585 2023-04-10 15:44:16.000000 django-torque-0.5.0a1/torque/migrations/0047_templatecachedocument_and_more.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)      393 2023-04-12 11:15:37.000000 django-torque-0.5.0a1/torque/migrations/0048_rename_search_cache_dirty_wikiconfig_cache_dirty.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)        0 2023-02-19 01:57:21.000000 django-torque-0.5.0a1/torque/migrations/__init__.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    25665 2023-04-12 18:43:02.000000 django-torque-0.5.0a1/torque/models.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     4809 2023-03-28 11:03:24.000000 django-torque-0.5.0a1/torque/urls.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)     3489 2023-04-12 18:43:02.000000 django-torque-0.5.0a1/torque/utils.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)       30 2023-04-17 15:28:54.000000 django-torque-0.5.0a1/torque/version.py
+-rw-r--r--   0 ots-macfound  (1001) ots-macfound  (1001)    36134 2023-04-12 18:43:02.000000 django-torque-0.5.0a1/torque/views.py
```

### Comparing `django-torque-0.4.0/PKG-INFO` & `django-torque-0.5.0a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-torque
-Version: 0.4.0
+Version: 0.5.0a1
 Summary: django app for torque
 Home-page: https://code.librehq.com/ots/mediawiki/torque
 Author: Open Tech Strategies, LLC
 Author-email: frankduncan@opentechstrategies.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `django-torque-0.4.0/README.md` & `django-torque-0.5.0a1/README.md`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/django_torque.egg-info/PKG-INFO` & `django-torque-0.5.0a1/django_torque.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-torque
-Version: 0.4.0
+Version: 0.5.0a1
 Summary: django app for torque
 Home-page: https://code.librehq.com/ots/mediawiki/torque
 Author: Open Tech Strategies, LLC
 Author-email: frankduncan@opentechstrategies.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `django-torque-0.4.0/django_torque.egg-info/SOURCES.txt` & `django-torque-0.5.0a1/django_torque.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -48,13 +48,20 @@
 ./torque/migrations/0035_template_in_config.py
 ./torque/migrations/0036_remove_searchcachedocument_torque_search_data_ve_0ad953_gin_and_more.py
 ./torque/migrations/0037_template_dirty.py
 ./torque/migrations/0038_wiki_linked_wiki_keys.py
 ./torque/migrations/0039_document_attached.py
 ./torque/migrations/0040_value_unique_value_for_field_document.py
 ./torque/migrations/0041_searchcachedocument_explore_rank.py
+./torque/migrations/0042_documentdictcache.py
+./torque/migrations/0043_documentdictcache_unique_document_dict.py
+./torque/migrations/0044_documentdictcache_dirty.py
+./torque/migrations/0045_templatecachedocument_dirty_and_more.py
+./torque/migrations/0046_delete_templatecachedocument.py
+./torque/migrations/0047_templatecachedocument_and_more.py
+./torque/migrations/0048_rename_search_cache_dirty_wikiconfig_cache_dirty.py
 ./torque/migrations/__init__.py
 django_torque.egg-info/PKG-INFO
 django_torque.egg-info/SOURCES.txt
 django_torque.egg-info/dependency_links.txt
 django_torque.egg-info/requires.txt
 django_torque.egg-info/top_level.txt
```

### Comparing `django-torque-0.4.0/setup.py` & `django-torque-0.5.0a1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,11 +32,12 @@
     install_requires=[
         "mwclient",
         "python-magic",
         "jinja2",
         "werkzeug",
         "django",
         "psycopg2-binary",
+        "orjson",
     ],
     package_dir={"": "."},
     python_requres=">=3.6",
 )
```

### Comparing `django-torque-0.4.0/torque/management/commands/remove_unattached.py` & `django-torque-0.5.0a1/torque/management/commands/remove_unattached.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0001_initial.py` & `django-torque-0.5.0a1/torque/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0005_auto_20210323_1303.py` & `django-torque-0.5.0a1/torque/migrations/0005_auto_20210323_1303.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0006_auto_20210323_1623.py` & `django-torque-0.5.0a1/torque/migrations/0006_auto_20210323_1623.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0007_auto_20210406_1738.py` & `django-torque-0.5.0a1/torque/migrations/0007_auto_20210406_1738.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0010_tableofcontentscache.py` & `django-torque-0.5.0a1/torque/migrations/0010_tableofcontentscache.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0016_auto_20210721_1444.py` & `django-torque-0.5.0a1/torque/migrations/0016_auto_20210721_1444.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0017_auto_20210721_1621.py` & `django-torque-0.5.0a1/torque/migrations/0017_auto_20210721_1621.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0019_auto_20210721_1720.py` & `django-torque-0.5.0a1/torque/migrations/0019_auto_20210721_1720.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0022_auto_20210905_1430.py` & `django-torque-0.5.0a1/torque/migrations/0022_auto_20210905_1430.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0023_auto_20210905_1454.py` & `django-torque-0.5.0a1/torque/migrations/0023_auto_20210905_1454.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0024_auto_20210905_1535.py` & `django-torque-0.5.0a1/torque/migrations/0024_auto_20210905_1535.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0025_auto_20210905_1624.py` & `django-torque-0.5.0a1/torque/migrations/0025_auto_20210905_1624.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0026_auto_20210905_1638.py` & `django-torque-0.5.0a1/torque/migrations/0026_auto_20210905_1638.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0027_auto_20210905_1642.py` & `django-torque-0.5.0a1/torque/migrations/0027_auto_20210905_1642.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0028_auto_20210905_1659.py` & `django-torque-0.5.0a1/torque/migrations/0028_auto_20210905_1659.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0029_auto_20210905_1716.py` & `django-torque-0.5.0a1/torque/migrations/0029_auto_20210905_1716.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0030_auto_20210927_1304.py` & `django-torque-0.5.0a1/torque/migrations/0030_auto_20210927_1304.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0031_auto_20210930_1328.py` & `django-torque-0.5.0a1/torque/migrations/0031_auto_20210930_1328.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0033_csvspecification.py` & `django-torque-0.5.0a1/torque/migrations/0033_csvspecification.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0034_auto_20220209_1209.py` & `django-torque-0.5.0a1/torque/migrations/0034_auto_20220209_1209.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0036_remove_searchcachedocument_torque_search_data_ve_0ad953_gin_and_more.py` & `django-torque-0.5.0a1/torque/migrations/0036_remove_searchcachedocument_torque_search_data_ve_0ad953_gin_and_more.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/migrations/0038_wiki_linked_wiki_keys.py` & `django-torque-0.5.0a1/torque/migrations/0038_wiki_linked_wiki_keys.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/models.py` & `django-torque-0.5.0a1/torque/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import hashlib
 import io
 import os
 import pathlib
 import json
+import orjson
+import mwclient
 from datetime import datetime
 from django.db import models
 from django.db.models import Q
 from django.conf import settings
 
 from django.contrib.postgres.search import SearchVector
 from django.contrib.postgres.search import SearchVectorField
@@ -25,46 +27,14 @@
     object_name = models.CharField(max_length=255)
     key_field = models.TextField()
     last_updated = models.DateTimeField(auto_now=True)
 
     def object_data_name(self):
         return self.object_name + "_data"
 
-    def clean_documents(self, config, document_list=None):
-        # return a reduced list of documents based on permissions defined in config
-        # (WikiConfig instance)
-        #
-        # Also reduced by the documents in document_list
-
-        document_limit = Q()
-        if document_list is not None:
-            document_limit = Q(document__in=document_list)
-
-        new_documents = {}
-        for value in (
-            Value.objects.filter(
-                document_limit,
-                document__in=config.valid_ids.all(),
-                field__in=config.valid_fields.all(),
-            )
-            .prefetch_related("field")
-            .prefetch_related("document")
-            .all()
-        ):
-            if value.document.id not in new_documents:
-                new_documents[value.document.id] = {
-                    "key": value.document.key,
-                    "db_document": value.document,
-                    "fields": {},
-                }
-            new_documents[value.document.id]["fields"][
-                value.field.name
-            ] = value.to_python()
-        return new_documents.values()
-
     @classmethod
     def from_json(cls, name, object_name, key_field, file):
         file_text = file.read().decode()
         data = json.loads(file_text)
         if Collection.objects.filter(name=name).exists():
             collection = Collection.objects.get(name=name)
         else:
@@ -89,14 +59,15 @@
                 collection_values[value.document] = {}
             if value.field not in collection_values[value.document]:
                 collection_values[value.document][value.field] = value
 
         collection.fields.update(attached=False)
         collection.documents.update(attached=False)
 
+        documents_to_dirty = set()
         for document_number, document_in in enumerate(data):
             if document_number == 0:
                 # Generate fields, but only on the first proposal
                 for field_name in document_in.keys():
                     field, created = Field.objects.update_or_create(
                         name=field_name,
                         collection=collection,
@@ -121,25 +92,28 @@
                     value = collection_values[db_document][fields[field_name]]
                     # Only update for values whose value has changed
                     if value.original != jsoned_value_value:
                         collection.last_updated = datetime.now
                         value.original = jsoned_value_value
                         value.latest = jsoned_value_value
                         value.save()
+                        documents_to_dirty.add(db_document)
                 else:
                     collection.last_updated = datetime.now
                     value = Value(
                         field=fields[field_name],
                         original=jsoned_value_value,
                         latest=jsoned_value_value,
                         document=db_document,
                     )
                     values.append(value)
+                    documents_to_dirty.add(db_document)
 
         Value.objects.bulk_create(values)
+        utils.dirty_documents(list(documents_to_dirty))
 
         # In case last_updated got set
         collection.save()
         return collection, documents
 
 
 class Wiki(models.Model):
@@ -198,75 +172,111 @@
     # This is highly NOT threadsafe, and will probably cause annoying problems
     # if two people are messing around with the configurations at the same time.
     #
     # Fortunately, that is highly unlikely, and the only real downside is that
     # the search cache has to be re-indexed, which is not a catastrophic error.
     in_config = models.BooleanField(default=False)
 
-    search_cache_dirty = models.BooleanField(default=False)
+    cache_dirty = models.BooleanField(default=False)
+
+    def rebuild_document_dict_cache(self):
+        values = (Value.objects.filter(
+                document__in=self.valid_ids.all(),
+                field__in=self.valid_fields.all(),
+            )
+            .prefetch_related("field")
+            .prefetch_related("document")
+            .values('document_id', 'document__key', 'field__name', 'latest')
+        )
+        new_documents = {}
+        for value in values:
+            try:
+                new_documents[value['document_id']]["fields"][
+                    value['field__name']
+                ] = orjson.loads(value['latest'])
+            except KeyError:
+                new_documents[value['document_id']] = {
+                    "key": value['document__key'],
+                    "fields": {
+                        value['field__name']: orjson.loads(value['latest'])
+                    },
+                }
+
+        document_dicts = []
+        for document in self.valid_ids.all():
+            document_dicts.append(
+                DocumentDictCache(
+                    document=document,
+                    wiki_config=self,
+                    dictionary=json.dumps(new_documents[document.id]),
+                )
+            )
+
+        DocumentDictCache.objects.bulk_create(document_dicts, ignore_conflicts=True)
+
 
     def rebuild_search_index(self):
         from django.conf import settings
 
         SearchCacheDocument.objects.filter(wiki_config=self).delete()
         sc_documents = []
-        for document_dict in self.collection.clean_documents(self):
-            document = document_dict["db_document"]
+        for ddc in DocumentDictCache.objects.filter(wiki_config=self, document__in=self.valid_ids.all()):
+            document_dict = orjson.loads(ddc.dictionary)["fields"]
             filtered_data = {}
             for filter in getattr(settings, "TORQUE_FILTERS", []):
-                filtered_data[filter.name()] = filter.document_value(
-                    document_dict["fields"]
-                )
+                filtered_data[filter.name()] = filter.document_value(document_dict)
 
             explore_rank = None
             if getattr(settings, "TORQUE_EXPLORE_RANK", None):
-                explore_rank = settings.TORQUE_EXPLORE_RANK.get_rank_key(
-                    document_dict["fields"]
-                )
+                explore_rank = settings.TORQUE_EXPLORE_RANK.get_rank_key(document_dict)
 
             sc_documents.append(
                 SearchCacheDocument(
-                    document=document,
+                    document=ddc.document,
                     collection=self.collection,
                     wiki=self.wiki,
                     group=self.group,
                     wiki_config=self,
                     filtered_data=filtered_data,
-                    data=" ".join(list(map(str, document_dict["fields"].values()))),
+                    data=" ".join(list(map(str, document_dict.values()))),
                     explore_rank=explore_rank,
                 )
             )
 
         SearchCacheDocument.objects.bulk_create(sc_documents)
         SearchCacheDocument.objects.filter(wiki_config=self).update(
             data_vector=SearchVector("data")
         )
 
-    def rebuild_template_cache(self, template):
-        TemplateCacheDocument.objects.filter(
-            wiki_config=self, template=template
-        ).delete()
-        template_documents = []
-
-        jinja_template = jinja_env.from_string(template.get_file_contents())
-        for document_dict in self.collection.clean_documents(self):
-            document = document_dict["db_document"]
-
-            template_documents.append(
-                TemplateCacheDocument(
-                    document=document,
-                    wiki_config=self,
-                    template=template,
-                    rendered_text=jinja_template.render(
-                        {self.collection.object_name: document_dict["fields"]}
-                    ),
+    def populate_template_cache(self, template, include_linked_wikis=False):
+        def build_cache(wiki_config):
+            template_documents = []
+            for ddc in DocumentDictCache.objects.filter(wiki_config=wiki_config):
+                template_documents.append(
+                    TemplateCacheDocument(
+                        document_dict=ddc,
+                        template=template,
+                        rendered_text="",
+                    )
                 )
-            )
+            TemplateCacheDocument.objects.bulk_create(template_documents, ignore_conflicts=True)
+
+            TemplateCacheDocument.objects.filter(template=template, document_dict__wiki_config=wiki_config).update(dirty=True)
+
+        build_cache(self)
 
-        TemplateCacheDocument.objects.bulk_create(template_documents)
+        if include_linked_wikis:
+            for wiki_key in self.wiki.linked_wiki_keys:
+                try:
+                    linked_config = WikiConfig.objects.get(group=self.group, wiki=Wiki.objects.get(wiki_key=wiki_key))
+                    build_cache(linked_config)
+                except WikiConfig.DoesNotExist:
+                    # If there's no permission set up for the group, or the wiki doesn't actually
+                    # exist, just soldier on
+                    pass
 
 
 class Document(models.Model):
     """A single document in a collection"""
 
     collection = models.ForeignKey(
         Collection, on_delete=models.CASCADE, related_name="documents"
@@ -279,20 +289,42 @@
     # When uploading a collection, if documents have been dropped off, then they are
     # no longer actively attached.  Instead of just removing them right away, and
     # losing any Value or ValueEdits associated, we just mark them as unattached,
     # and then we can later clean them up if we want.
     attached = models.BooleanField(default=True)
 
     def to_dict(self, config):
-        new_document = {"key": self.key}
-        valid_fields = config.valid_fields.all()
-        for value in self.values.filter(field__in=valid_fields).select_related("field"):
-            new_document[value.field.name] = value.to_python()
+        try:
+            return orjson.loads(DocumentDictCache.objects.get(document=self, wiki_config=config).dictionary)
+        except DocumentDictCache.DoesNotExist:
+            new_document = {"key": self.key, "fields": {}}
+            for value in self.values.filter(field__in=config.valid_fields.all()).values("field__name", "latest"):
+                new_document["fields"][value["field__name"]] = orjson.loads(value["latest"])
+
+            return new_document
+
+    def rebuild_cache(self, config):
+        try:
+            ddc = DocumentDictCache.objects.get(document=self, wiki_config=config)
+            if not ddc.dirty:
+                # No need to rebuild a cache we have that's not dirty...
+                return
+            else:
+                # We undirty now so that if it dirties while we're rebuilding, we rebuild again, just for safety
+                ddc.dirty = False
+                ddc.save()
+        except DocumentDictCache.DoesNotExist:
+            ddc = DocumentDictCache.objects.create(document=self, wiki_config=config)
+
+        new_document = {"key": self.key, "fields": {}}
+        for value in self.values.filter(field__in=config.valid_fields.all()).values("field__name", "latest"):
+            new_document["fields"][value["field__name"]] = orjson.loads(value["latest"])
 
-        return new_document
+        ddc.dictionary = json.dumps(new_document)
+        ddc.save()
 
     def __getitem__(self, key):
         try:
             return self.values.get(field__name=key).to_python()
         except Value.DoesNotExist:
             return None
 
@@ -336,15 +368,15 @@
 
     def to_python(self):
         # For legacy purposes, we return the string representation
         # if it's not valid json in the database.  Because some old
         # data may still be in the database that isn't overwritten,
         # we want to be able to soldier on.
         try:
-            return json.loads(self.latest)
+            return orjson.loads(self.latest)
         except json.JSONDecodeError:
             if self.latest:
                 return self.latest
             else:
                 return ""
 
     class Meta:
@@ -428,28 +460,35 @@
         )
         global_line_template = global_toc_templates.get(is_default=True)
         global_line_template_contents = global_line_template.get_file_contents()
 
         def add_to_data(wiki_config):
             collection = wiki_config.collection
 
-            document_limit = None
             if results_limit:
                 key_list = [rl[1] for rl in results_limit if rl[0] == collection.name]
-                document_limit = Document.objects.filter(key__in=key_list)
-            documents = collection.clean_documents(wiki_config, document_limit)
+                document_limit = Document.objects.filter(key__in=key_list, collection=collection)
+                documents = [orjson.loads(ddc.dictionary)["fields"] for ddc in DocumentDictCache.objects.filter(document__in=document_limit, wiki_config=wiki_config).all()]
+            else:
+                documents = [orjson.loads(ddc.dictionary)["fields"]
+                        for ddc
+                        in DocumentDictCache.objects.filter(
+                            document__in=wiki_config.valid_ids.all(),
+                            wiki_config=wiki_config
+                        )
+                ]
 
             data[global_collection_data_name][collection.name] = {
-                document["fields"][collection.key_field]: document["fields"]
+                document[collection.key_field]: document
                 for document in documents
             }
             data["toc_lines"][collection.name] = {
-                document["fields"][collection.key_field]: jinja_env.from_string(
+                document[collection.key_field]: jinja_env.from_string(
                     global_line_template_contents
-                ).render({collection.object_name: document["fields"]})
+                ).render({collection.object_name: document})
                 for document in documents
             }
 
         add_to_data(wiki_config)
 
         for wiki_key in wiki_config.wiki.linked_wiki_keys:
             try:
@@ -529,14 +568,15 @@
     toc = models.ForeignKey(TableOfContents, on_delete=models.CASCADE)
     dirty = models.BooleanField(default=True)
     rendered_html = models.TextField(null=True)
 
     def rebuild(self):
         import mwclient
 
+        self.dirty = False
         if self.wiki_config.wiki.server:
             if self.toc.raw:
                 self.rendered_html = self.toc.render_to_mwiki(self.wiki_config)
                 self.save()
             else:
                 (scheme, server) = self.wiki_config.wiki.server.split("://")
                 site = mwclient.Site(
@@ -566,12 +606,54 @@
 class CsvSpecification(models.Model):
     fields = models.JSONField()
     documents = models.ManyToManyField(Document)
     name = models.TextField()
     filename = models.TextField()
 
 
-class TemplateCacheDocument(models.Model):
+class DocumentDictCache(models.Model):
     document = models.ForeignKey(Document, on_delete=models.CASCADE)
     wiki_config = models.ForeignKey(WikiConfig, on_delete=models.CASCADE)
+    dirty = models.BooleanField(default=False)
+    dictionary = models.TextField(null=True)
+
+    class Meta:
+        constraints = [
+            models.UniqueConstraint(fields=["document", "wiki_config"], name="unique_document_dict"),
+        ]
+
+
+class TemplateCacheDocument(models.Model):
+    document_dict = models.ForeignKey(DocumentDictCache, on_delete=models.CASCADE)
     template = models.ForeignKey(Template, on_delete=models.CASCADE)
     rendered_text = models.TextField(null=True)
+    dirty = models.BooleanField(default=False)
+
+    class Meta:
+        constraints = [
+            models.UniqueConstraint(fields=["document_dict", "template"], name="unique_template_cache_document"),
+        ]
+
+    def rebuild(self):
+        try:
+            jinja_template = jinja_env.from_string(self.template.get_file_contents())
+
+            (scheme, server) = self.template.wiki.server.split("://")
+            site = mwclient.Site(server, self.template.wiki.script_path + "/", scheme=scheme)
+            site.login(self.template.wiki.username, self.template.wiki.password)
+
+            rendered_data = jinja_template.render(
+                {self.document_dict.document.collection.object_name: orjson.loads(self.document_dict.dictionary)["fields"]}
+            )
+            rendered_html = site.api(
+                "parse", text=rendered_data, contentmodel="wikitext", prop="text"
+            )["parse"]["text"]["*"]
+
+            self.rendered_text = rendered_html
+        except Exception:
+            # If we errored, then the cache can be set to the empty string to
+            # signal to people in the future that the cache failed, and they will have to
+            # rebuild, but we don't want to leave dirty because we tried
+            self.rendered_text = ""
+
+        self.dirty = False
+        self.save()
```

### Comparing `django-torque-0.4.0/torque/urls.py` & `django-torque-0.5.0a1/torque/urls.py`

 * *Files identical despite different names*

### Comparing `django-torque-0.4.0/torque/views.py` & `django-torque-0.5.0a1/torque/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import orjson
 import json
 import urllib.parse
 from werkzeug.utils import secure_filename
 from datetime import datetime
 from django.core.files.base import ContentFile
 from django.db.models import Q, F, Count
 from django.http import HttpResponse, JsonResponse, FileResponse
@@ -172,31 +173,36 @@
         [q], filters, wiki_configs, documents_limited_to
     )
     # While this result isn't actually mwiki text, this result is intended
     # for the mediawiki Torque extension.  Probably better to keep
     # the mwiki format than to do something like create a new "torque" format.
     # But, if we decide we need results to go to another renderer, it may
     # be worth being more clear about what we're doing here via the interface.
+    #
+    # This has gotten weird because the results are actually html from cached
+    # results
     if fmt == "mwiki":
         mwiki_text = ""
 
-        for result in returned_results[offset : (offset + 20)]:
-            template = jinja_env.from_string(
-                models.Template.objects.get(
-                    name="Search", collection=template_config.collection
-                ).get_file_contents()
-            )
-            mwiki_text += template.render(
-                {
-                    template_config.collection.object_name: result.document.to_dict(
-                        result.wiki_config
-                    )
-                }
-            )
-            mwiki_text += "\n\n"
+        template = models.Template.objects.get(name="Search", collection=template_config.collection)
+
+        cache_or = Q()
+        for r in returned_results[offset : (offset + 20)]:
+            cache_or |= Q(document_dict__wiki_config=r.wiki_config, document_dict__document=r.document)
+
+        cached_results = models.TemplateCacheDocument.objects.filter(
+            template=template,
+        ).filter(
+            cache_or
+        )
+
+        for cached_result in cached_results.filter(dirty=True):
+            cached_result.rebuild()
+
+        mwiki_text = "\n".join([c.rendered_text for c in cached_results])
 
         return JsonResponse(
             {
                 "num_results": returned_results.count(),
                 "mwiki_text": mwiki_text,
                 "filter_results": filter_results,
             },
@@ -265,16 +271,15 @@
     (returned_results, filter_results) = search_data(
         qs, filters, wiki_configs, results_limit
     )
 
     mwiki_text = ""
 
     result_set = [
-        r.document.to_dict(r.wiki_config)
-        for r in returned_results[offset : (offset + 100)]
+        orjson.loads(models.DocumentDictCache.objects.get(document=r.document, wiki_config__group=r.group).dictionary)["fields"] for r in returned_results[offset : (offset + 100)]
     ]
     explore_templates = models.Template.objects.filter(
         type="Explore",
         collection=template_config.collection,
     )
     if explore_templates:
         if template_name:
@@ -299,15 +304,15 @@
                 {template_config.collection.object_name: result}
             )
             mwiki_text += "\n\n"
 
     return JsonResponse(
         {
             "num_results": returned_results.count(),
-            "results": [(r.collection.name, r.document.key) for r in returned_results],
+            "results": [(r["collection__name"], r["document__key"]) for r in returned_results.values("collection__name", "document__key")],
             "mwiki_text": mwiki_text,
             "filter_results": filter_results,
         },
         safe=False,
     )
 
 
@@ -404,14 +409,20 @@
             wiki=wiki,
         )
         edit_record.save()
 
     models.TableOfContentsCache.objects.filter(
         toc__in=collection.tables_of_contents.all()
     ).update(dirty=True)
+    utils.dirty_documents([document])
+    # Rebuild immediately because whoever is doing the editing probably
+    # wants to see the fruits of their efforts.
+    document.rebuild_cache(wiki_config)
+    [t.rebuild() for t in models.TemplateCacheDocument.objects.filter(document_dict__wiki_config=wiki_config, document_dict__document=document).all()]
+
     wiki.invalidate_linked_wiki_toc_cache()
     models.SearchCacheDocument.objects.filter(document=document).update(dirty=True)
 
     # This is overkill, but that's ok.  There's a bit of work to make it so
     # the individaul template cache documents have a dirty method
     collection.templates.update(dirty=True)
 
@@ -490,14 +501,16 @@
         return HttpResponse(status=403)
 
     if fmt == "mwiki":
         return HttpResponse(toc.render_to_mwiki(wiki_config, results_limit))
     elif fmt == "html":
         if not results_limit:
             cached_toc = wiki_config.cached_tocs.get(toc=toc)
+            if cached_toc.dirty:
+                cached_toc.rebuild()
             return HttpResponse(cached_toc.rendered_html)
         else:
             return HttpResponse()
     else:
         raise Exception(f"Invalid format {fmt}")
 
 
@@ -512,77 +525,69 @@
         group=group,
     )
 
     if fmt == "json":
         return JsonResponse(
             [document.key for document in wiki_config.valid_ids.all()], safe=False
         )
-    elif fmt == "mwiki":
-        # Because we use mwiki as a format marker for when the mediawiki extension
-        # is contacting us, we're going to not fully follow the expected functionality,
-        # which would be to return a valid mediawiki page.  Rather, we're going to
-        # return the TOC style mediawiki text for the documents in the collection.
-        #
-        # An alternate path would be figure out how to call document.mwiki with
-        # the appropriate template.
-        caches = {
-            cache.document.key: cache.rendered_text
-            for cache in models.TemplateCacheDocument.objects.filter(
-                wiki_config=wiki_config
-            ).prefetch_related("document")
-        }
-        return JsonResponse(caches)
     else:
         raise Exception(f"Invalid format {fmt}")
 
 
 def get_document(group, wiki, key, fmt, collection_name, view=None):
     collection = models.Collection.objects.get(name=collection_name)
     wiki_config = models.WikiConfig.objects.get(
         collection=collection,
         wiki=wiki,
         group=group,
     )
     document = wiki_config.valid_ids.get(key=key, collection=collection).to_dict(
         wiki_config
-    )
+    )["fields"]
 
     if fmt == "json":
         return JsonResponse(document)
-    elif fmt == "mwiki":
-        templates = models.Template.objects.filter(
-            collection=collection,
-            wiki=wiki,
-            type="View",
-        )
+    elif fmt == "dict":
+        return document
 
-        if view is not None:
-            try:
-                view_object = json.loads(view)
 
-                view_wiki = models.Wiki.objects.get(wiki_key=view_object["wiki_key"])
-                view = view_object["view"]
-                template = models.Template.objects.get(
-                    wiki=view_wiki, type="View", name=view
-                )
-            except json.JSONDecodeError:
-                template = templates.get(name=view)
-        else:
-            template = templates.get(is_default=True)
+    templates = models.Template.objects.filter(
+        collection=collection,
+        wiki=wiki,
+        type="View",
+    )
+
+    if view is not None:
+        try:
+            view_object = json.loads(view)
+
+            view_wiki = models.Wiki.objects.get(wiki_key=view_object["wiki_key"])
+            view = view_object["view"]
+            template = models.Template.objects.get(
+                wiki=view_wiki, type="View", name=view
+            )
+        except json.JSONDecodeError:
+            template = templates.get(name=view)
+    else:
+        template = templates.get(is_default=True)
 
+    if fmt == "mwiki":
         rendered_template = jinja_env.from_string(template.get_file_contents()).render(
             {collection.object_name: document}
         )
         return HttpResponse(rendered_template)
-    elif fmt == "dict":
-        return document
     elif fmt == "html":
-        # Return the empty string because we don't have a cached version, and the
-        # TDC extension will read that and attempt to get the mwiki version.
-        return HttpResponse("")
+        try:
+            ddc = models.DocumentDictCache.objects.get(wiki_config=wiki_config, document=wiki_config.valid_ids.get(key=key, collection=collection))
+            cache = models.TemplateCacheDocument.objects.get(template=template, document_dict=ddc)
+            if cache.dirty:
+                cache.rebuild()
+            return HttpResponse(cache.rendered_text)
+        except models.TemplateCacheDocument.DoesNotExist:
+            return HttpResponse("")
     else:
         raise Exception(f"Invalid format {fmt}")
 
 
 def get_document_view(request, collection_name, key, fmt):
     group = request.GET["group"]
     wiki = get_wiki_from_request(request, collection_name)
@@ -721,16 +726,16 @@
         )
         valid_fields = models.Field.objects.filter(
             name__in=new_config.get("fields"), collection=collection
         )
         config.save()
         config.valid_ids.add(*valid_documents)
         config.valid_fields.add(*valid_fields)
-        config.search_cache_dirty = True
-        collection.templates.update(dirty=True)
+        config.cache_dirty = True
+        utils.dirty_documents(config.valid_ids.all(), config)
 
         for linked_wiki in models.Wiki.objects.filter(
             linked_wiki_keys__contains=[wiki_key]
         ):
             try:
                 linked_wiki_config = models.WikiConfig.objects.get(
                     wiki=linked_wiki, group=config.group
@@ -802,15 +807,15 @@
 
     # Regenerate search caches in case data has changed.  We assume that the
     # cache is invalid, making uploading a collection be a very expensive operation,
     # but that's probably better than attempting to analyze cache invalidation
     # and failing.
 
     for config in models.WikiConfig.objects.filter(collection=collection):
-        config.search_cache_dirty = True
+        config.cache_dirty = True
         config.save()
 
     for wiki in models.Wiki.objects.filter(configs__collection=collection):
         wiki.invalidate_linked_wiki_toc_cache()
 
     return HttpResponse(status=200)
```

