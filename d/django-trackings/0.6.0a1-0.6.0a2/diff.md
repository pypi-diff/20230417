# Comparing `tmp/django_trackings-0.6.0a1.tar.gz` & `tmp/django_trackings-0.6.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_trackings-0.6.0a1.tar", last modified: Sun Apr 16 22:50:53 2023, max compression
+gzip compressed data, was "django_trackings-0.6.0a2.tar", last modified: Sun Apr 16 23:10:20 2023, max compression
```

## Comparing `django_trackings-0.6.0a1.tar` & `django_trackings-0.6.0a2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:53.307664 django_trackings-0.6.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-16 22:50:53.307664 django_trackings-0.6.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-16 22:50:53.307664 django_trackings-0.6.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:53.299664 django_trackings-0.6.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:53.303664 django_trackings-0.6.0a1/src/dj_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)   429184 2023-04-16 22:50:52.000000 django_trackings-0.6.0a1/src/dj_tracker/cache_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/cache_utils.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/cache_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    15429 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/db_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/field_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)   312989 2023-04-16 22:50:42.000000 django_trackings-0.6.0a1/src/dj_tracker/hash_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/hash_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:53.303664 django_trackings-0.6.0a1/src/dj_tracker/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:53.303664 django_trackings-0.6.0a1/src/dj_tracker/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    19667 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    16063 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/pythoncapi_compat.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:53.299664 django_trackings-0.6.0a1/src/dj_tracker/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:53.299664 django_trackings-0.6.0a1/src/dj_tracker/static/dj_tracker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:53.303664 django_trackings-0.6.0a1/src/dj_tracker/static/dj_tracker/css/
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/static/dj_tracker/css/main.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:53.303664 django_trackings-0.6.0a1/src/dj_tracker/static/dj_tracker/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/static/dj_tracker/js/query_group.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:53.299664 django_trackings-0.6.0a1/src/dj_tracker/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:53.307664 django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/home.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:53.307664 django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/includes/listing.html
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/includes/pagination.html
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/includes/query.html
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/list.html
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/queries.html
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/query.html
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/query_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/query_groups.html
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/requests.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:53.307664 django_trackings-0.6.0a1/src/dj_tracker/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/templatetags/dj_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:53.307664 django_trackings-0.6.0a1/src/dj_tracker/test/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   594765 2023-04-16 22:50:52.000000 django_trackings-0.6.0a1/src/dj_tracker/traceback.c
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/traceback.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-04-16 22:50:38.000000 django_trackings-0.6.0a1/src/dj_tracker/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:50:53.307664 django_trackings-0.6.0a1/src/django_trackings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-16 22:50:53.000000 django_trackings-0.6.0a1/src/django_trackings.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.880776 django_trackings-0.6.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-16 23:10:20.880776 django_trackings-0.6.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-16 23:10:20.880776 django_trackings-0.6.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.872775 django_trackings-0.6.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.876775 django_trackings-0.6.0a2/src/dj_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)   429184 2023-04-16 23:10:20.000000 django_trackings-0.6.0a2/src/dj_tracker/cache_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/cache_utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/cache_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15429 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/db_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/field_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   312989 2023-04-16 23:10:09.000000 django_trackings-0.6.0a2/src/dj_tracker/hash_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/hash_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.876775 django_trackings-0.6.0a2/src/dj_tracker/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.876775 django_trackings-0.6.0a2/src/dj_tracker/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19667 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16063 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/pythoncapi_compat.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.872775 django_trackings-0.6.0a2/src/dj_tracker/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.872775 django_trackings-0.6.0a2/src/dj_tracker/static/dj_tracker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.876775 django_trackings-0.6.0a2/src/dj_tracker/static/dj_tracker/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/static/dj_tracker/css/main.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.876775 django_trackings-0.6.0a2/src/dj_tracker/static/dj_tracker/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/static/dj_tracker/js/query_group.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.872775 django_trackings-0.6.0a2/src/dj_tracker/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.880776 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/home.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.880776 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/includes/listing.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/includes/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/includes/query.html
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/queries.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/query.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/query_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/query_groups.html
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/requests.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.880776 django_trackings-0.6.0a2/src/dj_tracker/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/templatetags/dj_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.880776 django_trackings-0.6.0a2/src/dj_tracker/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   594765 2023-04-16 23:10:20.000000 django_trackings-0.6.0a2/src/dj_tracker/traceback.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/traceback.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-04-16 23:10:03.000000 django_trackings-0.6.0a2/src/dj_tracker/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:10:20.880776 django_trackings-0.6.0a2/src/django_trackings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-16 23:10:20.000000 django_trackings-0.6.0a2/src/django_trackings.egg-info/SOURCES.txt
```

### Comparing `django_trackings-0.6.0a1/LICENSE` & `django_trackings-0.6.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/PKG-INFO` & `django_trackings-0.6.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_trackings
-Version: 0.6.0a1
+Version: 0.6.0a2
 Summary: A Django app that tracks your queries to help optimize them.
 Home-page: https://github.com/tijani-dia/dj-tracker/
 Author: Tidiane Dia
 Author-email: atdia97@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://tijani-dia.github.io/dj-tracker/
 Project-URL: Source, https://github.com/tijani-dia/dj-tracker/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django_trackings Version: 0.6.0a1 Summary: A Django
+Metadata-Version: 2.1 Name: django_trackings Version: 0.6.0a2 Summary: A Django
 app that tracks your queries to help optimize them. Home-page: https://
 github.com/tijani-dia/dj-tracker/ Author: Tidiane Dia Author-email:
 atdia97@gmail.com License: BSD-3-Clause Project-URL: Documentation, https://
 tijani-dia.github.io/dj-tracker/ Project-URL: Source, https://github.com/
 tijani-dia/dj-tracker/ Project-URL: Issue tracker, https://github.com/tijani-
 dia/dj-tracker/issues/ Classifier: Development Status :: 3 - Alpha Classifier:
 Environment :: Web Environment Classifier: Framework :: Django Classifier:
```

### Comparing `django_trackings-0.6.0a1/README.md` & `django_trackings-0.6.0a2/README.md`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/setup.cfg` & `django_trackings-0.6.0a2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_trackings
-version = 0.6.0a1
+version = 0.6.0a2
 description = A Django app that tracks your queries to help optimize them.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tijani-dia/dj-tracker/
 author = Tidiane Dia
 author_email = atdia97@gmail.com
 license = BSD-3-Clause
```

### Comparing `django_trackings-0.6.0a1/setup.py` & `django_trackings-0.6.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/cache_utils.c` & `django_trackings-0.6.0a2/src/dj_tracker/cache_utils.c`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/cache_utils.pyx` & `django_trackings-0.6.0a2/src/dj_tracker/cache_utils.pyx`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/collector.py` & `django_trackings-0.6.0a2/src/dj_tracker/collector.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/constants.py` & `django_trackings-0.6.0a2/src/dj_tracker/constants.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/datastructures.py` & `django_trackings-0.6.0a2/src/dj_tracker/datastructures.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/db_router.py` & `django_trackings-0.6.0a2/src/dj_tracker/db_router.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/field_descriptors.py` & `django_trackings-0.6.0a2/src/dj_tracker/field_descriptors.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/hash_utils.c` & `django_trackings-0.6.0a2/src/dj_tracker/hash_utils.c`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/hash_utils.pyx` & `django_trackings-0.6.0a2/src/dj_tracker/hash_utils.pyx`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/logging.py` & `django_trackings-0.6.0a2/src/dj_tracker/logging.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/migrations/0001_initial.py` & `django_trackings-0.6.0a2/src/dj_tracker/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/models.py` & `django_trackings-0.6.0a2/src/dj_tracker/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
             )
         )
 
     def n_plus_one(self):
         return self.annotate_n_plus_one().filter(n_plus_one=True)
 
     def annotate_num_trackings(self):
-        return self.annotate(num_trackings=models.Count("trackings"))
+        return self.annotate(num_trackings=models.Count("trackings", distinct=True))
 
     def annotate_num_queries(self):
         # https://stackoverflow.com/questions/52027676/using-subquery-to-annotate-a-count
         num_queries = (
             QuerySetTracking.objects.filter(query_group_id=models.OuterRef("pk"))
             .order_by()
             .annotate(total=models.Func(models.F("num_occurrences"), function="Sum"))
@@ -225,15 +225,15 @@
 
 
 class RequestQuerySet(models.QuerySet):
     def annotate_latest_occurrence(self):
         return self.annotate(latest_occurrence=models.Max("trackings__started_at"))
 
     def annotate_num_trackings(self):
-        return self.annotate(num_trackings=models.Count("trackings"))
+        return self.annotate(num_trackings=models.Count("trackings", distinct=True))
 
     def annotate_n_plus_one(self):
         return self.annotate(
             n_plus_one=models.Exists(
                 QueryGroup.objects.n_plus_one().filter(
                     trackings__request=models.OuterRef("pk")
                 )
```

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/profile.py` & `django_trackings-0.6.0a2/src/dj_tracker/profile.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/promise.py` & `django_trackings-0.6.0a2/src/dj_tracker/promise.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/pythoncapi_compat.h` & `django_trackings-0.6.0a2/src/dj_tracker/pythoncapi_compat.h`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/static/dj_tracker/css/main.css` & `django_trackings-0.6.0a2/src/dj_tracker/static/dj_tracker/css/main.css`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/static/dj_tracker/js/query_group.js` & `django_trackings-0.6.0a2/src/dj_tracker/static/dj_tracker/js/query_group.js`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/base.html` & `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/base.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/home.html` & `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/home.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/includes/listing.html` & `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/includes/listing.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/includes/pagination.html` & `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/includes/query.html` & `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/includes/query.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/queries.html` & `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/queries.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/query.html` & `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/query.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/query_group.html` & `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/query_group.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/query_groups.html` & `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/query_groups.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/templates/dj_tracker/requests.html` & `django_trackings-0.6.0a2/src/dj_tracker/templates/dj_tracker/requests.html`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/templatetags/dj_tracker.py` & `django_trackings-0.6.0a2/src/dj_tracker/templatetags/dj_tracker.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/test/__init__.py` & `django_trackings-0.6.0a2/src/dj_tracker/test/__init__.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/traceback.c` & `django_trackings-0.6.0a2/src/dj_tracker/traceback.c`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/traceback.pyx` & `django_trackings-0.6.0a2/src/dj_tracker/traceback.pyx`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/tracker.py` & `django_trackings-0.6.0a2/src/dj_tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/urls.py` & `django_trackings-0.6.0a2/src/dj_tracker/urls.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.6.0a1/src/dj_tracker/views.py` & `django_trackings-0.6.0a2/src/dj_tracker/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
 
         # Requests
         context["most_tracked"] = (
             Request.objects.select_related("path")
-            .annotate(num_trackings=Count("trackings"))
+            .annotate_num_trackings()
             .order_by("-num_trackings")[:5]
         )
         context["latest"] = (
             Request.objects.alias(latest_tracking=Max("trackings__started_at"))
             .order_by("-latest_tracking")
             .select_related("path")
             .distinct()[:5]
@@ -112,15 +112,15 @@
         context["slowest"] = Query.objects.only("average_duration").order_by(
             "-average_duration"
         )[:5]
         context["largest"] = Query.objects.only("num_instances").order_by(
             "-num_instances"
         )[:5]
         context["most_repeated_queries"] = (
-            Query.objects.annotate(num_trackings=Count("trackings"))
+            Query.objects.annotate(num_trackings=Count("trackings", distinct=True))
             .only("cache_key")
             .order_by("-num_trackings")[:5]
         )
         return context
 
 
 class RequestsView(ListView):
@@ -285,15 +285,15 @@
 
     model = Query
     filterset_fields = ["model", "query_type"]
 
     @lazy_attribute
     def base_queryset(cls):
         return (
-            Query.objects.annotate(num_trackings=Count("trackings"))
+            Query.objects.annotate(num_trackings=Count("trackings", distinct=True))
             .select_related("sql", "model")
             .only(
                 "query_type",
                 "num_instances",
                 "average_duration",
                 "sql__sql",
                 "model__label",
```

### Comparing `django_trackings-0.6.0a1/src/django_trackings.egg-info/SOURCES.txt` & `django_trackings-0.6.0a2/src/django_trackings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

