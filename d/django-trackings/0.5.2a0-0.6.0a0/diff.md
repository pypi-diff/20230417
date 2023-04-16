# Comparing `tmp/django_trackings-0.5.2a0.tar.gz` & `tmp/django_trackings-0.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_trackings-0.5.2a0.tar", last modified: Wed Mar  8 18:13:30 2023, max compression
+gzip compressed data, was "django_trackings-0.6.0a0.tar", last modified: Sun Apr 16 16:04:06 2023, max compression
```

## Comparing `django_trackings-0.5.2a0.tar` & `django_trackings-0.6.0a0.tar`

### file list

```diff
@@ -1,60 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:13:30.962373 django_trackings-0.5.2a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-03-08 18:13:30.962373 django_trackings-0.5.2a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-08 18:13:30.966374 django_trackings-0.5.2a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:13:30.954373 django_trackings-0.5.2a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:13:30.958373 django_trackings-0.5.2a0/src/dj_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)   429342 2023-03-08 18:13:30.000000 django_trackings-0.5.2a0/src/dj_tracker/cache_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/cache_utils.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/cache_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/db_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/field_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)   313345 2023-03-08 18:13:30.000000 django_trackings-0.5.2a0/src/dj_tracker/hash_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/hash_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:13:30.962373 django_trackings-0.5.2a0/src/dj_tracker/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:13:30.962373 django_trackings-0.5.2a0/src/dj_tracker/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    16063 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/pythoncapi_compat.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:13:30.950373 django_trackings-0.5.2a0/src/dj_tracker/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:13:30.950373 django_trackings-0.5.2a0/src/dj_tracker/static/dj_tracker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:13:30.962373 django_trackings-0.5.2a0/src/dj_tracker/static/dj_tracker/css/
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-03-08 18:13:12.000000 django_trackings-0.5.2a0/src/dj_tracker/static/dj_tracker/css/main.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:13:30.962373 django_trackings-0.5.2a0/src/dj_tracker/static/dj_tracker/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/static/dj_tracker/js/query_group.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:13:30.950373 django_trackings-0.5.2a0/src/dj_tracker/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:13:30.962373 django_trackings-0.5.2a0/src/dj_tracker/templates/dj_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/templates/dj_tracker/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/templates/dj_tracker/home.html
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/templates/dj_tracker/pagination.html
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/templates/dj_tracker/qs_tracking.html
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/templates/dj_tracker/query_group.html
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/templates/dj_tracker/queryset_tracking.html
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/templates/dj_tracker/requests.html
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/templates/dj_tracker/url_trackings.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:13:30.962373 django_trackings-0.5.2a0/src/dj_tracker/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/templatetags/dj_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:13:30.962373 django_trackings-0.5.2a0/src/dj_tracker/test/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   578632 2023-03-08 18:13:30.000000 django_trackings-0.5.2a0/src/dj_tracker/traceback.c
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/traceback.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-03-08 18:13:11.000000 django_trackings-0.5.2a0/src/dj_tracker/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 18:13:30.962373 django_trackings-0.5.2a0/src/django_trackings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-03-08 18:13:30.000000 django_trackings-0.5.2a0/src/django_trackings.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:04:06.194437 django_trackings-0.6.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-16 16:04:06.194437 django_trackings-0.6.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-16 16:04:06.194437 django_trackings-0.6.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:04:06.174435 django_trackings-0.6.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:04:06.186436 django_trackings-0.6.0a0/src/dj_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)   429184 2023-04-16 16:04:05.000000 django_trackings-0.6.0a0/src/dj_tracker/cache_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/cache_utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/cache_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15429 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/db_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/field_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   312989 2023-04-16 16:03:55.000000 django_trackings-0.6.0a0/src/dj_tracker/hash_utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/hash_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:04:06.186436 django_trackings-0.6.0a0/src/dj_tracker/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:04:06.186436 django_trackings-0.6.0a0/src/dj_tracker/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19667 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16063 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/pythoncapi_compat.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:04:06.174435 django_trackings-0.6.0a0/src/dj_tracker/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:04:06.174435 django_trackings-0.6.0a0/src/dj_tracker/static/dj_tracker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:04:06.186436 django_trackings-0.6.0a0/src/dj_tracker/static/dj_tracker/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-16 16:03:50.000000 django_trackings-0.6.0a0/src/dj_tracker/static/dj_tracker/css/main.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:04:06.186436 django_trackings-0.6.0a0/src/dj_tracker/static/dj_tracker/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/static/dj_tracker/js/query_group.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:04:06.174435 django_trackings-0.6.0a0/src/dj_tracker/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:04:06.194437 django_trackings-0.6.0a0/src/dj_tracker/templates/dj_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/templates/dj_tracker/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/templates/dj_tracker/home.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:04:06.194437 django_trackings-0.6.0a0/src/dj_tracker/templates/dj_tracker/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/templates/dj_tracker/includes/listing.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/templates/dj_tracker/includes/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/templates/dj_tracker/includes/query.html
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/templates/dj_tracker/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/templates/dj_tracker/queries.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/templates/dj_tracker/query.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/templates/dj_tracker/query_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/templates/dj_tracker/query_groups.html
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/templates/dj_tracker/requests.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:04:06.194437 django_trackings-0.6.0a0/src/dj_tracker/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/templatetags/dj_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:04:06.194437 django_trackings-0.6.0a0/src/dj_tracker/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   594765 2023-04-16 16:04:05.000000 django_trackings-0.6.0a0/src/dj_tracker/traceback.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/traceback.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-04-16 16:03:49.000000 django_trackings-0.6.0a0/src/dj_tracker/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:04:06.194437 django_trackings-0.6.0a0/src/django_trackings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-16 16:04:06.000000 django_trackings-0.6.0a0/src/django_trackings.egg-info/SOURCES.txt
```

### Comparing `django_trackings-0.5.2a0/LICENSE` & `django_trackings-0.6.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_trackings-0.5.2a0/PKG-INFO` & `django_trackings-0.6.0a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_trackings
-Version: 0.5.2a0
+Version: 0.6.0a0
 Summary: A Django app that tracks your queries to help optimize them.
 Home-page: https://github.com/tijani-dia/dj-tracker/
 Author: Tidiane Dia
 Author-email: atdia97@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://tijani-dia.github.io/dj-tracker/
 Project-URL: Source, https://github.com/tijani-dia/dj-tracker/
@@ -54,14 +54,15 @@
 - Detect when a deferred field is loaded
 - and many more insights into your queries with minimized overhead....
 
 ## Requirements
 
 - Python: `>=3.8`
 - Django: `>=3.2`
+- [django-filter](https://github.com/carltongibson/django-filter)
 
 ## Getting started
 
 Check out the [installation steps](https://tijani-dia.github.io/dj-tracker/installation/) if you want to get started quickly or the [tutorial](https://tijani-dia.github.io/dj-tracker/tutorial/setup/) to see a concrete example of `dj-tracker` usage.
 
 ## Documentation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django_trackings Version: 0.5.2a0 Summary: A Django
+Metadata-Version: 2.1 Name: django_trackings Version: 0.6.0a0 Summary: A Django
 app that tracks your queries to help optimize them. Home-page: https://
 github.com/tijani-dia/dj-tracker/ Author: Tidiane Dia Author-email:
 atdia97@gmail.com License: BSD-3-Clause Project-URL: Documentation, https://
 tijani-dia.github.io/dj-tracker/ Project-URL: Source, https://github.com/
 tijani-dia/dj-tracker/ Project-URL: Issue tracker, https://github.com/tijani-
 dia/dj-tracker/issues/ Classifier: Development Status :: 3 - Alpha Classifier:
 Environment :: Web Environment Classifier: Framework :: Django Classifier:
@@ -21,15 +21,16 @@
 field usage of model instances - Report unused fields in a model instance and
 provides hints on when to use `.defer` and `.only` - Report model instance
 attributes access and provides hints on when to use `.values` or `.values_list`
 - Report cache hits and provides hints on when to use `iterator` - Provides
 hints on when to use `.count`, `.contains`, `.exists` - Detect N+1 queries -
 Detect when a deferred field is loaded - and many more insights into your
 queries with minimized overhead.... ## Requirements - Python: `>=3.8` - Django:
-`>=3.2` ## Getting started Check out the [installation steps](https://tijani-
+`>=3.2` - [django-filter](https://github.com/carltongibson/django-filter) ##
+Getting started Check out the [installation steps](https://tijani-
 dia.github.io/dj-tracker/installation/) if you want to get started quickly or
 the [tutorial](https://tijani-dia.github.io/dj-tracker/tutorial/setup/) to see
 a concrete example of `dj-tracker` usage. ## Documentation All documentation is
 in the "docs" directory and online at https://tijani-dia.github.io/dj-tracker/
 ## Development phase - Contributing `dj-tracker` is in [alpha phase](https://
 en.wikipedia.org/wiki/Software_release_life_cycle#Alpha). You can help a lot by
 [reporting bugs](https://github.com/Tijani-Dia/dj-tracker/issues/new) you'll
```

### Comparing `django_trackings-0.5.2a0/README.md` & `django_trackings-0.6.0a0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 - Detect when a deferred field is loaded
 - and many more insights into your queries with minimized overhead....
 
 ## Requirements
 
 - Python: `>=3.8`
 - Django: `>=3.2`
+- [django-filter](https://github.com/carltongibson/django-filter)
 
 ## Getting started
 
 Check out the [installation steps](https://tijani-dia.github.io/dj-tracker/installation/) if you want to get started quickly or the [tutorial](https://tijani-dia.github.io/dj-tracker/tutorial/setup/) to see a concrete example of `dj-tracker` usage.
 
 ## Documentation
```

#### html2text {}

```diff
@@ -8,15 +8,16 @@
 field usage of model instances - Report unused fields in a model instance and
 provides hints on when to use `.defer` and `.only` - Report model instance
 attributes access and provides hints on when to use `.values` or `.values_list`
 - Report cache hits and provides hints on when to use `iterator` - Provides
 hints on when to use `.count`, `.contains`, `.exists` - Detect N+1 queries -
 Detect when a deferred field is loaded - and many more insights into your
 queries with minimized overhead.... ## Requirements - Python: `>=3.8` - Django:
-`>=3.2` ## Getting started Check out the [installation steps](https://tijani-
+`>=3.2` - [django-filter](https://github.com/carltongibson/django-filter) ##
+Getting started Check out the [installation steps](https://tijani-
 dia.github.io/dj-tracker/installation/) if you want to get started quickly or
 the [tutorial](https://tijani-dia.github.io/dj-tracker/tutorial/setup/) to see
 a concrete example of `dj-tracker` usage. ## Documentation All documentation is
 in the "docs" directory and online at https://tijani-dia.github.io/dj-tracker/
 ## Development phase - Contributing `dj-tracker` is in [alpha phase](https://
 en.wikipedia.org/wiki/Software_release_life_cycle#Alpha). You can help a lot by
 [reporting bugs](https://github.com/Tijani-Dia/dj-tracker/issues/new) you'll
```

### Comparing `django_trackings-0.5.2a0/setup.cfg` & `django_trackings-0.6.0a0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_trackings
-version = 0.5.2a0
+version = 0.6.0a0
 description = A Django app that tracks your queries to help optimize them.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tijani-dia/dj-tracker/
 author = Tidiane Dia
 author_email = atdia97@gmail.com
 license = BSD-3-Clause
@@ -22,24 +22,26 @@
 	Source=https://github.com/tijani-dia/dj-tracker/
 	Issue tracker=https://github.com/tijani-dia/dj-tracker/issues/
 
 [options]
 packages = find_namespace:
 install_requires = 
 	django>=3.2
+	django-filter
 python_requires = >=3.8
 include_package_data = True
 package_dir = =src
 zip_safe = False
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 dev = 
+	Cython>=3.0.0b2
 	autoflake
 	black>=23.1
 	factory-boy
 	flake8
 	isort
 	pytailwindcss
 docs = 
@@ -52,15 +54,15 @@
 python-tag = py3
 
 [tool:isort]
 profile = black
 known_first_party = "dj_tracker"
 
 [flake8]
-extend-ignore = E501
+extend-ignore = E501, E203
 exclude = **/migrations/*.py
 filename = *.py, *.pyx
 per-file-ignores = src/dj_tracker/*.pyx:E999
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django_trackings-0.5.2a0/setup.py` & `django_trackings-0.6.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/cache_utils.c` & `django_trackings-0.6.0a0/src/dj_tracker/cache_utils.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.0b1 */
+/* Generated by Cython 3.0.0b2 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "CYTHON_TRACE",
@@ -39,18 +39,18 @@
     #endif
     
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0b1"
+#define CYTHON_ABI "3_0_0b2"
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000B1
+#define CYTHON_HEX_VERSION 0x030000B2
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -2142,25 +2142,25 @@
 static const char __pyx_k_LRUCache_get[] = "LRUCache.get";
 static const char __pyx_k_LRUCache_set[] = "LRUCache.set";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_stringsource[] = "<stringsource>";
 static const char __pyx_k_init_subclass[] = "__init_subclass__";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_AttributeError[] = "AttributeError";
+static const char __pyx_k_lazy_attribute[] = "lazy_attribute";
 static const char __pyx_k_LazySlots___new[] = "LazySlots.__new__";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
-static const char __pyx_k_cached_attribute[] = "cached_attribute";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static const char __pyx_k_cached_attribute___get[] = "cached_attribute.__get__";
+static const char __pyx_k_lazy_attribute___get[] = "lazy_attribute.__get__";
+static const char __pyx_k_lazy_attribute___init[] = "lazy_attribute.__init__";
 static const char __pyx_k_dj_tracker_cache_utils[] = "dj_tracker.cache_utils";
-static const char __pyx_k_cached_attribute___init[] = "cached_attribute.__init__";
 static const char __pyx_k_LRUCache___reduce_cython[] = "LRUCache.__reduce_cython__";
+static const char __pyx_k_lazy_attribute___set_name[] = "lazy_attribute.__set_name__";
 static const char __pyx_k_LRUCache___setstate_cython[] = "LRUCache.__setstate_cython__";
-static const char __pyx_k_cached_attribute___set_name[] = "cached_attribute.__set_name__";
 static const char __pyx_k_src_dj_tracker_cache_utils_pyx[] = "src/dj_tracker/cache_utils.pyx";
 static const char __pyx_k_This_is_similar_to_cached_prope[] = "\n    This is similar to `cached_property` but for classes rather than class instances.\n    ";
 static const char __pyx_k_LazySlots___new___locals___getat[] = "LazySlots.__new__.<locals>.__getattr__";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 /* #### Code section: decls ### */
 static int __pyx_pf_10dj_tracker_11cache_utils_8LRUCache___cinit__(struct __pyx_obj_10dj_tracker_11cache_utils_LRUCache *__pyx_v_self, int __pyx_v_maxsize); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_11cache_utils_8LRUCache_2get(struct __pyx_obj_10dj_tracker_11cache_utils_LRUCache *__pyx_v_self, PyObject *__pyx_v_key); /* proto */
@@ -2169,17 +2169,17 @@
 static PyObject *__pyx_pf_10dj_tracker_11cache_utils_8LRUCache_8__repr__(struct __pyx_obj_10dj_tracker_11cache_utils_LRUCache *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_11cache_utils_8LRUCache_7maxsize___get__(struct __pyx_obj_10dj_tracker_11cache_utils_LRUCache *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_11cache_utils_8LRUCache_10__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10dj_tracker_11cache_utils_LRUCache *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_11cache_utils_8LRUCache_12__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10dj_tracker_11cache_utils_LRUCache *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_11cache_utils___defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_11cache_utils_9LazySlots_7__new_____getattr__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_attr, PyObject *__pyx_v_lazy_slots); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_11cache_utils_9LazySlots___new__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_cls, PyObject *__pyx_v_name, PyObject *__pyx_v_bases, PyObject *__pyx_v_namespace, PyObject *__pyx_v_kwargs); /* proto */
-static PyObject *__pyx_pf_10dj_tracker_11cache_utils_16cached_attribute___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_func); /* proto */
-static PyObject *__pyx_pf_10dj_tracker_11cache_utils_16cached_attribute_2__set_name__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_owner, PyObject *__pyx_v_name); /* proto */
-static PyObject *__pyx_pf_10dj_tracker_11cache_utils_16cached_attribute_4__get__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_instance, PyObject *__pyx_v_cls); /* proto */
+static PyObject *__pyx_pf_10dj_tracker_11cache_utils_14lazy_attribute___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_func); /* proto */
+static PyObject *__pyx_pf_10dj_tracker_11cache_utils_14lazy_attribute_2__set_name__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_owner, PyObject *__pyx_v_name); /* proto */
+static PyObject *__pyx_pf_10dj_tracker_11cache_utils_14lazy_attribute_4__get__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_instance, PyObject *__pyx_v_cls); /* proto */
 static PyObject *__pyx_tp_new_10dj_tracker_11cache_utils_LRUCache(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_get = {0, 0, 0, 0, 0};
 static __Pyx_CachedCFunction __pyx_umethod_PyDict_Type_pop = {0, 0, 0, 0, 0};
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
   PyObject *__pyx_d;
@@ -2240,18 +2240,14 @@
   PyObject *__pyx_n_s_LazySlots___new___locals___getat;
   PyObject *__pyx_kp_s_This_is_similar_to_cached_prope;
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_n_s__21;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_attr;
   PyObject *__pyx_n_s_bases;
-  PyObject *__pyx_n_s_cached_attribute;
-  PyObject *__pyx_n_s_cached_attribute___get;
-  PyObject *__pyx_n_s_cached_attribute___init;
-  PyObject *__pyx_n_s_cached_attribute___set_name;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_cls;
   PyObject *__pyx_n_s_dict;
   PyObject *__pyx_kp_u_disable;
   PyObject *__pyx_n_s_dj_tracker_cache_utils;
   PyObject *__pyx_n_s_doc;
   PyObject *__pyx_kp_u_enable;
@@ -2265,14 +2261,18 @@
   PyObject *__pyx_n_s_init_subclass;
   PyObject *__pyx_n_s_instance;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_n_s_items;
   PyObject *__pyx_n_s_key;
   PyObject *__pyx_n_s_kwargs;
+  PyObject *__pyx_n_s_lazy_attribute;
+  PyObject *__pyx_n_s_lazy_attribute___get;
+  PyObject *__pyx_n_s_lazy_attribute___init;
+  PyObject *__pyx_n_s_lazy_attribute___set_name;
   PyObject *__pyx_n_s_lazy_slots;
   PyObject *__pyx_n_u_lazy_slots;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_maxsize;
   PyObject *__pyx_n_s_metaclass;
   PyObject *__pyx_n_s_meth;
   PyObject *__pyx_n_s_method;
@@ -2383,18 +2383,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_LazySlots___new___locals___getat);
   Py_CLEAR(clear_module_state->__pyx_kp_s_This_is_similar_to_cached_prope);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_n_s__21);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_attr);
   Py_CLEAR(clear_module_state->__pyx_n_s_bases);
-  Py_CLEAR(clear_module_state->__pyx_n_s_cached_attribute);
-  Py_CLEAR(clear_module_state->__pyx_n_s_cached_attribute___get);
-  Py_CLEAR(clear_module_state->__pyx_n_s_cached_attribute___init);
-  Py_CLEAR(clear_module_state->__pyx_n_s_cached_attribute___set_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_cls);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
   Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
   Py_CLEAR(clear_module_state->__pyx_n_s_dj_tracker_cache_utils);
   Py_CLEAR(clear_module_state->__pyx_n_s_doc);
   Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
@@ -2408,14 +2404,18 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_init_subclass);
   Py_CLEAR(clear_module_state->__pyx_n_s_instance);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_n_s_items);
   Py_CLEAR(clear_module_state->__pyx_n_s_key);
   Py_CLEAR(clear_module_state->__pyx_n_s_kwargs);
+  Py_CLEAR(clear_module_state->__pyx_n_s_lazy_attribute);
+  Py_CLEAR(clear_module_state->__pyx_n_s_lazy_attribute___get);
+  Py_CLEAR(clear_module_state->__pyx_n_s_lazy_attribute___init);
+  Py_CLEAR(clear_module_state->__pyx_n_s_lazy_attribute___set_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_lazy_slots);
   Py_CLEAR(clear_module_state->__pyx_n_u_lazy_slots);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_maxsize);
   Py_CLEAR(clear_module_state->__pyx_n_s_metaclass);
   Py_CLEAR(clear_module_state->__pyx_n_s_meth);
   Py_CLEAR(clear_module_state->__pyx_n_s_method);
@@ -2504,18 +2504,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_LazySlots___new___locals___getat);
   Py_VISIT(traverse_module_state->__pyx_kp_s_This_is_similar_to_cached_prope);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_n_s__21);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_attr);
   Py_VISIT(traverse_module_state->__pyx_n_s_bases);
-  Py_VISIT(traverse_module_state->__pyx_n_s_cached_attribute);
-  Py_VISIT(traverse_module_state->__pyx_n_s_cached_attribute___get);
-  Py_VISIT(traverse_module_state->__pyx_n_s_cached_attribute___init);
-  Py_VISIT(traverse_module_state->__pyx_n_s_cached_attribute___set_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_cls);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
   Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
   Py_VISIT(traverse_module_state->__pyx_n_s_dj_tracker_cache_utils);
   Py_VISIT(traverse_module_state->__pyx_n_s_doc);
   Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
@@ -2529,14 +2525,18 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_init_subclass);
   Py_VISIT(traverse_module_state->__pyx_n_s_instance);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_n_s_items);
   Py_VISIT(traverse_module_state->__pyx_n_s_key);
   Py_VISIT(traverse_module_state->__pyx_n_s_kwargs);
+  Py_VISIT(traverse_module_state->__pyx_n_s_lazy_attribute);
+  Py_VISIT(traverse_module_state->__pyx_n_s_lazy_attribute___get);
+  Py_VISIT(traverse_module_state->__pyx_n_s_lazy_attribute___init);
+  Py_VISIT(traverse_module_state->__pyx_n_s_lazy_attribute___set_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_lazy_slots);
   Py_VISIT(traverse_module_state->__pyx_n_u_lazy_slots);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_maxsize);
   Py_VISIT(traverse_module_state->__pyx_n_s_metaclass);
   Py_VISIT(traverse_module_state->__pyx_n_s_meth);
   Py_VISIT(traverse_module_state->__pyx_n_s_method);
@@ -2651,18 +2651,14 @@
 #define __pyx_n_s_LazySlots___new___locals___getat __pyx_mstate_global->__pyx_n_s_LazySlots___new___locals___getat
 #define __pyx_kp_s_This_is_similar_to_cached_prope __pyx_mstate_global->__pyx_kp_s_This_is_similar_to_cached_prope
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_n_s__21 __pyx_mstate_global->__pyx_n_s__21
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_attr __pyx_mstate_global->__pyx_n_s_attr
 #define __pyx_n_s_bases __pyx_mstate_global->__pyx_n_s_bases
-#define __pyx_n_s_cached_attribute __pyx_mstate_global->__pyx_n_s_cached_attribute
-#define __pyx_n_s_cached_attribute___get __pyx_mstate_global->__pyx_n_s_cached_attribute___get
-#define __pyx_n_s_cached_attribute___init __pyx_mstate_global->__pyx_n_s_cached_attribute___init
-#define __pyx_n_s_cached_attribute___set_name __pyx_mstate_global->__pyx_n_s_cached_attribute___set_name
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_cls __pyx_mstate_global->__pyx_n_s_cls
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
 #define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
 #define __pyx_n_s_dj_tracker_cache_utils __pyx_mstate_global->__pyx_n_s_dj_tracker_cache_utils
 #define __pyx_n_s_doc __pyx_mstate_global->__pyx_n_s_doc
 #define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
@@ -2676,14 +2672,18 @@
 #define __pyx_n_s_init_subclass __pyx_mstate_global->__pyx_n_s_init_subclass
 #define __pyx_n_s_instance __pyx_mstate_global->__pyx_n_s_instance
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_n_s_items __pyx_mstate_global->__pyx_n_s_items
 #define __pyx_n_s_key __pyx_mstate_global->__pyx_n_s_key
 #define __pyx_n_s_kwargs __pyx_mstate_global->__pyx_n_s_kwargs
+#define __pyx_n_s_lazy_attribute __pyx_mstate_global->__pyx_n_s_lazy_attribute
+#define __pyx_n_s_lazy_attribute___get __pyx_mstate_global->__pyx_n_s_lazy_attribute___get
+#define __pyx_n_s_lazy_attribute___init __pyx_mstate_global->__pyx_n_s_lazy_attribute___init
+#define __pyx_n_s_lazy_attribute___set_name __pyx_mstate_global->__pyx_n_s_lazy_attribute___set_name
 #define __pyx_n_s_lazy_slots __pyx_mstate_global->__pyx_n_s_lazy_slots
 #define __pyx_n_u_lazy_slots __pyx_mstate_global->__pyx_n_u_lazy_slots
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_maxsize __pyx_mstate_global->__pyx_n_s_maxsize
 #define __pyx_n_s_metaclass __pyx_mstate_global->__pyx_n_s_metaclass
 #define __pyx_n_s_meth __pyx_mstate_global->__pyx_n_s_meth
 #define __pyx_n_s_method __pyx_mstate_global->__pyx_n_s_method
@@ -4621,23 +4621,23 @@
  * 
  *     def __init__(self, func):             # <<<<<<<<<<<<<<
  *         self.func = func
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10dj_tracker_11cache_utils_16cached_attribute_1__init__(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_10dj_tracker_11cache_utils_14lazy_attribute_1__init__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_10dj_tracker_11cache_utils_16cached_attribute_1__init__ = {"__init__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10dj_tracker_11cache_utils_16cached_attribute_1__init__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_10dj_tracker_11cache_utils_16cached_attribute_1__init__(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_10dj_tracker_11cache_utils_14lazy_attribute_1__init__ = {"__init__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10dj_tracker_11cache_utils_14lazy_attribute_1__init__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_10dj_tracker_11cache_utils_14lazy_attribute_1__init__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -4692,26 +4692,26 @@
     __pyx_v_self = values[0];
     __pyx_v_func = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, __pyx_nargs); __PYX_ERR(1, 64, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("dj_tracker.cache_utils.cached_attribute.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dj_tracker.cache_utils.lazy_attribute.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10dj_tracker_11cache_utils_16cached_attribute___init__(__pyx_self, __pyx_v_self, __pyx_v_func);
+  __pyx_r = __pyx_pf_10dj_tracker_11cache_utils_14lazy_attribute___init__(__pyx_self, __pyx_v_self, __pyx_v_func);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10dj_tracker_11cache_utils_16cached_attribute___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_func) {
+static PyObject *__pyx_pf_10dj_tracker_11cache_utils_14lazy_attribute___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_func) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
@@ -4732,15 +4732,15 @@
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("dj_tracker.cache_utils.cached_attribute.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dj_tracker.cache_utils.lazy_attribute.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -4749,23 +4749,23 @@
  * 
  *     def __set_name__(self, owner, name):             # <<<<<<<<<<<<<<
  *         self.name = name
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10dj_tracker_11cache_utils_16cached_attribute_3__set_name__(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_10dj_tracker_11cache_utils_14lazy_attribute_3__set_name__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_10dj_tracker_11cache_utils_16cached_attribute_3__set_name__ = {"__set_name__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10dj_tracker_11cache_utils_16cached_attribute_3__set_name__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_10dj_tracker_11cache_utils_16cached_attribute_3__set_name__(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_10dj_tracker_11cache_utils_14lazy_attribute_3__set_name__ = {"__set_name__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10dj_tracker_11cache_utils_14lazy_attribute_3__set_name__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_10dj_tracker_11cache_utils_14lazy_attribute_3__set_name__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -4832,26 +4832,26 @@
     __pyx_v_owner = values[1];
     __pyx_v_name = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__set_name__", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 67, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("dj_tracker.cache_utils.cached_attribute.__set_name__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dj_tracker.cache_utils.lazy_attribute.__set_name__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10dj_tracker_11cache_utils_16cached_attribute_2__set_name__(__pyx_self, __pyx_v_self, __pyx_v_owner, __pyx_v_name);
+  __pyx_r = __pyx_pf_10dj_tracker_11cache_utils_14lazy_attribute_2__set_name__(__pyx_self, __pyx_v_self, __pyx_v_owner, __pyx_v_name);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10dj_tracker_11cache_utils_16cached_attribute_2__set_name__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_owner, PyObject *__pyx_v_name) {
+static PyObject *__pyx_pf_10dj_tracker_11cache_utils_14lazy_attribute_2__set_name__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_owner, PyObject *__pyx_v_name) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set_name__", 0);
 
@@ -4872,15 +4872,15 @@
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("dj_tracker.cache_utils.cached_attribute.__set_name__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dj_tracker.cache_utils.lazy_attribute.__set_name__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -4889,23 +4889,23 @@
  * 
  *     def __get__(self, instance, cls):             # <<<<<<<<<<<<<<
  *         if not cls:
  *             cls = type(instance)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10dj_tracker_11cache_utils_16cached_attribute_5__get__(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_10dj_tracker_11cache_utils_14lazy_attribute_5__get__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_10dj_tracker_11cache_utils_16cached_attribute_5__get__ = {"__get__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10dj_tracker_11cache_utils_16cached_attribute_5__get__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_10dj_tracker_11cache_utils_16cached_attribute_5__get__(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_10dj_tracker_11cache_utils_14lazy_attribute_5__get__ = {"__get__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10dj_tracker_11cache_utils_14lazy_attribute_5__get__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_10dj_tracker_11cache_utils_14lazy_attribute_5__get__(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
@@ -4972,26 +4972,26 @@
     __pyx_v_instance = values[1];
     __pyx_v_cls = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__get__", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 70, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("dj_tracker.cache_utils.cached_attribute.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dj_tracker.cache_utils.lazy_attribute.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10dj_tracker_11cache_utils_16cached_attribute_4__get__(__pyx_self, __pyx_v_self, __pyx_v_instance, __pyx_v_cls);
+  __pyx_r = __pyx_pf_10dj_tracker_11cache_utils_14lazy_attribute_4__get__(__pyx_self, __pyx_v_self, __pyx_v_instance, __pyx_v_cls);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10dj_tracker_11cache_utils_16cached_attribute_4__get__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_instance, PyObject *__pyx_v_cls) {
+static PyObject *__pyx_pf_10dj_tracker_11cache_utils_14lazy_attribute_4__get__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_instance, PyObject *__pyx_v_cls) {
   PyObject *__pyx_v_result = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -5096,15 +5096,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("dj_tracker.cache_utils.cached_attribute.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("dj_tracker.cache_utils.lazy_attribute.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XDECREF(__pyx_v_cls);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -5338,18 +5338,14 @@
     {&__pyx_n_s_LazySlots___new___locals___getat, __pyx_k_LazySlots___new___locals___getat, sizeof(__pyx_k_LazySlots___new___locals___getat), 0, 0, 1, 1},
     {&__pyx_kp_s_This_is_similar_to_cached_prope, __pyx_k_This_is_similar_to_cached_prope, sizeof(__pyx_k_This_is_similar_to_cached_prope), 0, 0, 1, 0},
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_n_s__21, __pyx_k__21, sizeof(__pyx_k__21), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_attr, __pyx_k_attr, sizeof(__pyx_k_attr), 0, 0, 1, 1},
     {&__pyx_n_s_bases, __pyx_k_bases, sizeof(__pyx_k_bases), 0, 0, 1, 1},
-    {&__pyx_n_s_cached_attribute, __pyx_k_cached_attribute, sizeof(__pyx_k_cached_attribute), 0, 0, 1, 1},
-    {&__pyx_n_s_cached_attribute___get, __pyx_k_cached_attribute___get, sizeof(__pyx_k_cached_attribute___get), 0, 0, 1, 1},
-    {&__pyx_n_s_cached_attribute___init, __pyx_k_cached_attribute___init, sizeof(__pyx_k_cached_attribute___init), 0, 0, 1, 1},
-    {&__pyx_n_s_cached_attribute___set_name, __pyx_k_cached_attribute___set_name, sizeof(__pyx_k_cached_attribute___set_name), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
     {&__pyx_n_s_cls, __pyx_k_cls, sizeof(__pyx_k_cls), 0, 0, 1, 1},
     {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
     {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
     {&__pyx_n_s_dj_tracker_cache_utils, __pyx_k_dj_tracker_cache_utils, sizeof(__pyx_k_dj_tracker_cache_utils), 0, 0, 1, 1},
     {&__pyx_n_s_doc, __pyx_k_doc, sizeof(__pyx_k_doc), 0, 0, 1, 1},
     {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
@@ -5363,14 +5359,18 @@
     {&__pyx_n_s_init_subclass, __pyx_k_init_subclass, sizeof(__pyx_k_init_subclass), 0, 0, 1, 1},
     {&__pyx_n_s_instance, __pyx_k_instance, sizeof(__pyx_k_instance), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
     {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
     {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
     {&__pyx_n_s_kwargs, __pyx_k_kwargs, sizeof(__pyx_k_kwargs), 0, 0, 1, 1},
+    {&__pyx_n_s_lazy_attribute, __pyx_k_lazy_attribute, sizeof(__pyx_k_lazy_attribute), 0, 0, 1, 1},
+    {&__pyx_n_s_lazy_attribute___get, __pyx_k_lazy_attribute___get, sizeof(__pyx_k_lazy_attribute___get), 0, 0, 1, 1},
+    {&__pyx_n_s_lazy_attribute___init, __pyx_k_lazy_attribute___init, sizeof(__pyx_k_lazy_attribute___init), 0, 0, 1, 1},
+    {&__pyx_n_s_lazy_attribute___set_name, __pyx_k_lazy_attribute___set_name, sizeof(__pyx_k_lazy_attribute___set_name), 0, 0, 1, 1},
     {&__pyx_n_s_lazy_slots, __pyx_k_lazy_slots, sizeof(__pyx_k_lazy_slots), 0, 0, 1, 1},
     {&__pyx_n_u_lazy_slots, __pyx_k_lazy_slots, sizeof(__pyx_k_lazy_slots), 0, 1, 0, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_s_maxsize, __pyx_k_maxsize, sizeof(__pyx_k_maxsize), 0, 0, 1, 1},
     {&__pyx_n_s_metaclass, __pyx_k_metaclass, sizeof(__pyx_k_metaclass), 0, 0, 1, 1},
     {&__pyx_n_s_meth, __pyx_k_meth, sizeof(__pyx_k_meth), 0, 0, 1, 1},
     {&__pyx_n_s_method, __pyx_k_method, sizeof(__pyx_k_method), 0, 0, 1, 1},
@@ -6071,67 +6071,67 @@
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "dj_tracker/cache_utils.pyx":59
  * 
  * 
- * class cached_attribute:             # <<<<<<<<<<<<<<
+ * class lazy_attribute:             # <<<<<<<<<<<<<<
  *     """
  *     This is similar to `cached_property` but for classes rather than class instances.
  */
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_cached_attribute, __pyx_n_s_cached_attribute, (PyObject *) NULL, __pyx_n_s_dj_tracker_cache_utils, __pyx_kp_s_This_is_similar_to_cached_prope); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 59, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_lazy_attribute, __pyx_n_s_lazy_attribute, (PyObject *) NULL, __pyx_n_s_dj_tracker_cache_utils, __pyx_kp_s_This_is_similar_to_cached_prope); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
   /* "dj_tracker/cache_utils.pyx":64
  *     """
  * 
  *     def __init__(self, func):             # <<<<<<<<<<<<<<
  *         self.func = func
  * 
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_10dj_tracker_11cache_utils_16cached_attribute_1__init__, 0, __pyx_n_s_cached_attribute___init, NULL, __pyx_n_s_dj_tracker_cache_utils, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 64, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_10dj_tracker_11cache_utils_14lazy_attribute_1__init__, 0, __pyx_n_s_lazy_attribute___init, NULL, __pyx_n_s_dj_tracker_cache_utils, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(1, 64, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "dj_tracker/cache_utils.pyx":67
  *         self.func = func
  * 
  *     def __set_name__(self, owner, name):             # <<<<<<<<<<<<<<
  *         self.name = name
  * 
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_10dj_tracker_11cache_utils_16cached_attribute_3__set_name__, 0, __pyx_n_s_cached_attribute___set_name, NULL, __pyx_n_s_dj_tracker_cache_utils, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 67, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_10dj_tracker_11cache_utils_14lazy_attribute_3__set_name__, 0, __pyx_n_s_lazy_attribute___set_name, NULL, __pyx_n_s_dj_tracker_cache_utils, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_set_name, __pyx_t_4) < 0) __PYX_ERR(1, 67, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "dj_tracker/cache_utils.pyx":70
  *         self.name = name
  * 
  *     def __get__(self, instance, cls):             # <<<<<<<<<<<<<<
  *         if not cls:
  *             cls = type(instance)
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_10dj_tracker_11cache_utils_16cached_attribute_5__get__, 0, __pyx_n_s_cached_attribute___get, NULL, __pyx_n_s_dj_tracker_cache_utils, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_10dj_tracker_11cache_utils_14lazy_attribute_5__get__, 0, __pyx_n_s_lazy_attribute___get, NULL, __pyx_n_s_dj_tracker_cache_utils, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_get_2, __pyx_t_4) < 0) __PYX_ERR(1, 70, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "dj_tracker/cache_utils.pyx":59
  * 
  * 
- * class cached_attribute:             # <<<<<<<<<<<<<<
+ * class lazy_attribute:             # <<<<<<<<<<<<<<
  *     """
  *     This is similar to `cached_property` but for classes rather than class instances.
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_cached_attribute, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 59, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_lazy_attribute, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cached_attribute, __pyx_t_4) < 0) __PYX_ERR(1, 59, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lazy_attribute, __pyx_t_4) < 0) __PYX_ERR(1, 59, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "dj_tracker/cache_utils.pyx":1
  * from cpython.dict cimport PyDict_Next             # <<<<<<<<<<<<<<
  * from cpython.object cimport PyObject
  *
```

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/cache_utils.pyx` & `django_trackings-0.6.0a0/src/dj_tracker/cache_utils.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 __getattr__=__getattr__,
                 __slots__=(*namespace.get("__slots__", ()), *lazy_slots),
             )
 
         return super().__new__(cls, name, bases, namespace, **kwargs)
 
 
-class cached_attribute:
+class lazy_attribute:
     """
     This is similar to `cached_property` but for classes rather than class instances.
     """
 
     def __init__(self, func):
         self.func = func
```

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/collector.py` & `django_trackings-0.6.0a0/src/dj_tracker/collector.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/constants.py` & `django_trackings-0.6.0a0/src/dj_tracker/constants.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/datastructures.py` & `django_trackings-0.6.0a0/src/dj_tracker/datastructures.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import weakref
 from collections import Counter, defaultdict, deque
 from itertools import chain
 
 from django.db import transaction
 from django.utils.timezone import now
 
-from dj_tracker.cache_utils import LazySlots, cached_attribute
+from dj_tracker.cache_utils import LazySlots, lazy_attribute
 from dj_tracker.collector import Collector
 from dj_tracker.constants import DUMMY_REQUEST, TRACKINGS_DB
 from dj_tracker.context import get_request
 from dj_tracker.hash_utils import HashableCounter, HashableMixin
 from dj_tracker.models import QueryGroup, QuerySetTracking, Tracking
 from dj_tracker.promise import QueryGroupPromise, QueryPromise, RequestPromise
 from dj_tracker.traceback import get_traceback
@@ -133,14 +133,17 @@
     def __lt__(self, other):
         if type(other) is FieldTracker:
             return (self.get, self.set) < (other.get, other.set)
         elif not other:
             return False
         return NotImplemented
 
+    def __repr__(self):
+        return f"get: {self.get}, set: {self.set}"
+
 
 class InstanceTracker(dict):
     __slots__ = ()
 
     def __missing__(self, field):
         return
 
@@ -247,15 +250,15 @@
 class DummyRequestTracker:
     queries = Counter()
 
     @classmethod
     def add_query(cls, query_id):
         cls.queries[query_id] += 1
 
-    @cached_attribute
+    @lazy_attribute
     def query_group_id(cls):
         started_at = now()
         pk = hash(uuid.uuid1().int)
 
         with transaction.atomic(using=TRACKINGS_DB):
             request_id = RequestPromise.get_or_create(
                 path="",
@@ -494,7 +497,10 @@
     def save_trackers(trackers):
         deque((tracker.save() for tracker in trackers), maxlen=0)
         QueryPromise.resolve()
         return len(trackers)
 
     def __hash__(self):
         return id(self)
+
+    def __repr__(self):
+        return f"<QueryTracker {self['sql']}>"
```

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/db_router.py` & `django_trackings-0.6.0a0/src/dj_tracker/db_router.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from django.apps import apps
 
-from dj_tracker.cache_utils import cached_attribute
+from dj_tracker.cache_utils import lazy_attribute
 
 
 class DjTrackerRouter:
     app_label = "dj_tracker"
     db_alias = "trackings"
 
-    @cached_attribute
+    @lazy_attribute
     def models(cls):
         return frozenset(
             apps.get_app_config(cls.app_label).get_models(include_auto_created=True)
         )
 
     def db_for_read(self, model, **hints):
         if model in self.models:
```

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/field_descriptors.py` & `django_trackings-0.6.0a0/src/dj_tracker/field_descriptors.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/hash_utils.c` & `django_trackings-0.6.0a0/src/dj_tracker/hash_utils.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,8 @@
-/* Generated by Cython 3.0.0b1 */
-
-/* BEGIN: Cython Metadata
-{
-    "distutils": {
-        "define_macros": [
-            [
-                "CYTHON_TRACE",
-                0
-            ]
-        ],
-        "name": "dj_tracker.hash_utils",
-        "sources": [
-            "src/dj_tracker/hash_utils.pyx"
-        ]
-    },
-    "module_name": "dj_tracker.hash_utils"
-}
-END: Cython Metadata */
+/* Generated by Cython 3.0.0b2 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #if defined(CYTHON_LIMITED_API) && 0
   #ifndef Py_LIMITED_API
     #if CYTHON_LIMITED_API+0 > 0x03030000
@@ -33,18 +15,18 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0b1"
+#define CYTHON_ABI "3_0_0b2"
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000B1
+#define CYTHON_HEX_VERSION 0x030000B2
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
```

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/hash_utils.pyx` & `django_trackings-0.6.0a0/src/dj_tracker/hash_utils.pyx`

 * *Files identical despite different names*

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/logging.py` & `django_trackings-0.6.0a0/src/dj_tracker/logging.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/migrations/0001_initial.py` & `django_trackings-0.6.0a0/src/dj_tracker/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/models.py` & `django_trackings-0.6.0a0/src/dj_tracker/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -45,31 +45,14 @@
 class URLPath(Promisable):
     path = models.CharField(max_length=1024)
 
     def __str__(self):
         return self.path
 
 
-class Request(Promisable):
-    path = models.ForeignKey(URLPath, on_delete=models.CASCADE, related_name="requests")
-    method = models.CharField(max_length=8)
-    content_type = models.CharField(max_length=256)
-    query_string = models.CharField(max_length=1024)
-
-    def get_absolute_url(self):
-        return reverse("url-trackings", kwargs={"pk": self.pk})
-
-    def __str__(self):
-        if not self.method:
-            return "DummyRequest"
-
-        base = f"[{self.method}] {self.path}"
-        return base if not self.query_string else f"{base}?{self.query_string}"
-
-
 class SourceFile(Promisable):
     name = models.CharField(max_length=255)
 
     def __str__(self):
         return self.name
 
 
@@ -151,16 +134,20 @@
     related_queryset = models.ForeignKey(
         "self",
         null=True,
         on_delete=models.CASCADE,
         related_name="related_querysets",
     )
 
+    @property
+    def average_duration_in_ms(self):
+        return round(self.average_duration * 1e-6, 2)
+
     def get_absolute_url(self):
-        return reverse("queryset-tracking", kwargs={"pk": self.pk})
+        return reverse("query", kwargs={"pk": self.pk})
 
     def get_hints(self):
         if self.query_type != QueryType.SELECT:
             return
 
         cache_hits = self.cache_hits
         if self.len_calls and cache_hits == 2 * self.len_calls - 1:
@@ -178,59 +165,114 @@
         if (
             (attrs_accessed := self.attributes_accessed) is not None
             and len(attrs_accessed) <= 3
             and set(attrs_accessed).issubset({"__dict__", "__class__", "_state"})
         ):
             yield "Use .values() or .values_list()"
 
-    @property
-    def average_duration_in_ms(self):
-        return round(self.average_duration * 1e-6, 2)
 
+class QueryGroupQuerySet(models.QuerySet):
+    def annotate_latest_occurrence(self):
+        return self.annotate(latest_occurrence=models.Max("trackings__started_at"))
+
+    def order_by_latest_occurrence(self):
+        return self.annotate_latest_occurrence().order_by("-latest_occurrence")
+
+    def annotate_n_plus_one(self):
+        return self.annotate(
+            n_plus_one=models.Exists(
+                QuerySetTracking.objects.filter(
+                    num_occurrences__gt=1,
+                    query_group_id=models.OuterRef("pk"),
+                    query__related_queryset__isnull=False,
+                )
+            )
+        )
+
+    def n_plus_one(self):
+        return self.annotate_n_plus_one().filter(n_plus_one=True)
+
+    def annotate_num_trackings(self):
+        return self.annotate(num_trackings=models.Count("trackings"))
 
-class QueryGroupManager(models.Manager):
     def annotate_num_queries(self):
         # https://stackoverflow.com/questions/52027676/using-subquery-to-annotate-a-count
         num_queries = (
             QuerySetTracking.objects.filter(query_group_id=models.OuterRef("pk"))
             .order_by()
             .annotate(total=models.Func(models.F("num_occurrences"), function="Sum"))
             .values("total")
         )
         return self.annotate(num_queries=models.Subquery(num_queries))
 
 
 class QueryGroup(Promisable):
     queries = models.ManyToManyField(Query, through="QuerySetTracking")
-    objects = QueryGroupManager()
+    objects = QueryGroupQuerySet.as_manager()
 
     def get_absolute_url(self):
         return reverse("query-group", kwargs={"pk": self.pk})
 
 
 class QuerySetTracking(models.Model):
     query = models.ForeignKey(Query, on_delete=models.CASCADE, related_name="trackings")
-    query_group = models.ForeignKey(QueryGroup, on_delete=models.CASCADE)
+    query_group = models.ForeignKey(
+        QueryGroup, on_delete=models.CASCADE, related_name="qs_trackings"
+    )
     # Number of occurrences of query in query_group.
     num_occurrences = models.PositiveSmallIntegerField()
 
-    def get_absolute_url(self):
-        return self.query.get_absolute_url()
-
+    @property
     def duplicate(self):
         return self.num_occurrences > 1
 
 
+class RequestQuerySet(models.QuerySet):
+    def annotate_latest_occurrence(self):
+        return self.annotate(latest_occurrence=models.Max("trackings__started_at"))
+
+    def annotate_num_trackings(self):
+        return self.annotate(num_trackings=models.Count("trackings"))
+
+    def annotate_n_plus_one(self):
+        return self.annotate(
+            n_plus_one=models.Exists(
+                QueryGroup.objects.n_plus_one().filter(
+                    trackings__request=models.OuterRef("pk")
+                )
+            )
+        )
+
+    def n_plus_one(self):
+        return self.annotate_n_plus_one().filter(n_plus_one=True)
+
+
+class Request(Promisable):
+    path = models.ForeignKey(URLPath, on_delete=models.CASCADE, related_name="requests")
+    method = models.CharField(max_length=8)
+    content_type = models.CharField(max_length=256)
+    query_string = models.CharField(max_length=1024)
+
+    objects = RequestQuerySet.as_manager()
+
+    def get_absolute_url(self):
+        return reverse("request", kwargs={"request_id": self.pk})
+
+    def __str__(self):
+        if not self.method:
+            return "DummyRequest"
+
+        base = f"[{self.method}] {self.path}"
+        return base if not self.query_string else f"{base}?{self.query_string}"
+
+
 class Tracking(models.Model):
     started_at = models.DateTimeField()
-    request = models.ForeignKey(
-        Request, on_delete=models.CASCADE, related_name="trackings"
-    )
     query_group = models.ForeignKey(
         QueryGroup, on_delete=models.CASCADE, related_name="trackings"
     )
+    request = models.ForeignKey(
+        Request, on_delete=models.CASCADE, related_name="trackings"
+    )
 
     class Meta:
         ordering = ("-started_at",)
-
-    def get_absolute_url(self):
-        return reverse("tracking", kwargs={"pk": self.pk})
```

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/promise.py` & `django_trackings-0.6.0a0/src/dj_tracker/promise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, FrozenSet, Hashable, Optional, Tuple
 
 from django.apps import apps
 from django.db.models.base import ModelBase
 from django.db.models.query import BaseIterable
 
-from dj_tracker.cache_utils import LRUCache, cached_attribute
+from dj_tracker.cache_utils import LRUCache, lazy_attribute
 from dj_tracker.hash_utils import HashableCounter, HashableList, hash_string
 from dj_tracker.models import (
     InstanceFieldTracking,
     QuerySetTracking,
     QueryType,
     StackEntry,
 )
@@ -77,15 +77,15 @@
     def obj_created(cls, cache_key: int):
         """
         Hook run when an object with the given `cache_key` is created
         """
         # Remove and return the corresponding promise from `to_resolve`.
         return cls.resolve_promise(cache_key)
 
-    @cached_attribute
+    @lazy_attribute
     def queryset(cls):
         return cls.model.objects.only("cache_key").values_list("cache_key", flat=True)
 
     @classmethod
     def resolve_existing(cls, to_resolve):
         """
         Finds all existing objects with primary keys matching the ones in `to_resolve`
```

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/pythoncapi_compat.h` & `django_trackings-0.6.0a0/src/dj_tracker/pythoncapi_compat.h`

 * *Files identical despite different names*

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/static/dj_tracker/css/main.css` & `django_trackings-0.6.0a0/src/dj_tracker/static/dj_tracker/css/main.css`

 * *Files 26% similar despite different names*

```diff
@@ -1 +1 @@
-/*! tailwindcss v3.2.7 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}html{-webkit-text-size-adjust:100%;font-feature-settings:normal;font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:initial}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:initial;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:initial}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}a{--tw-text-opacity:1;color:rgb(49 46 129/var(--tw-text-opacity));font-weight:500}a:hover{text-decoration:underline}li{list-style-type:none}li:hover{--tw-bg-opacity:1;background-color:rgb(241 245 249/var(--tw-bg-opacity))}table{border-collapse:collapse;border-color:rgb(148 163 184/var(--tw-border-opacity))}table,td,th{--tw-border-opacity:1;border-width:1px}td,th{border-color:rgb(203 213 225/var(--tw-border-opacity));padding:.625rem}th{text-align:start}*,::backdrop,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:#3b82f680;--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }section{margin-bottom:2rem;margin-top:2rem}.section__title{--tw-border-opacity:1;--tw-text-opacity:1;border-bottom-color:rgb(30 41 59/var(--tw-border-opacity));border-bottom-width:4px;color:rgb(30 41 59/var(--tw-text-opacity));font-size:1.5rem;font-weight:500;line-height:2rem;width:-moz-min-content;width:min-content}.section__subtitle{--tw-text-opacity:1;color:rgb(100 116 139/var(--tw-text-opacity));font-size:1.25rem;line-height:1.75rem;padding-bottom:1rem;padding-top:1rem}.section__body{margin-top:.5rem}.rounded-pill{--tw-bg-opacity:1;--tw-text-opacity:1;background-color:rgb(226 232 240/var(--tw-bg-opacity));border-radius:9999px;color:rgb(71 85 105/var(--tw-text-opacity));font-size:.875rem;height:-moz-fit-content;height:fit-content;line-height:1.25rem;padding:.25rem .5rem}.text-muted{font-size:.875rem;line-height:1.25rem;opacity:.8}.static{position:static}.float-right{float:right}.m-2{margin:.5rem}.m-\[12px\]{margin:12px}.m-auto{margin:auto}.mx-10{margin-left:2.5rem;margin-right:2.5rem}.mx-2{margin-left:.5rem;margin-right:.5rem}.my-1{margin-bottom:.25rem;margin-top:.25rem}.my-2{margin-bottom:.5rem;margin-top:.5rem}.my-3{margin-bottom:.75rem;margin-top:.75rem}.my-4{margin-bottom:1rem;margin-top:1rem}.mb-12{margin-bottom:3rem}.mb-2{margin-bottom:.5rem}.mb-3{margin-bottom:.75rem}.mb-4{margin-bottom:1rem}.mb-8{margin-bottom:2rem}.ml-1{margin-left:.25rem}.ml-1\.5{margin-left:.375rem}.ml-2{margin-left:.5rem}.mr-1{margin-right:.25rem}.mr-1\.5{margin-right:.375rem}.mr-4{margin-right:1rem}.mr-5{margin-right:1.25rem}.mr-8{margin-right:2rem}.mt-10{margin-top:2.5rem}.mt-16{margin-top:4rem}.mt-2{margin-top:.5rem}.mt-4{margin-top:1rem}.block{display:block}.flex{display:flex}.table{display:table}.min-h-screen{min-height:100vh}.w-1\/3{width:33.333333%}.w-1\/5{width:20%}.w-1\/6{width:16.666667%}.w-11\/12{width:91.666667%}.w-12{width:3rem}.w-2\/3{width:66.666667%}.w-3\/4{width:75%}.w-3\/5{width:60%}.w-5\/12{width:41.666667%}.w-full{width:100%}.w-max{width:-moz-max-content;width:max-content}.max-w-sm{max-width:24rem}.shrink-0{flex-shrink:0}.flex-grow,.grow{flex-grow:1}.flex-col{flex-direction:column}.flex-wrap{flex-wrap:wrap}.items-center{align-items:center}.items-baseline{align-items:baseline}.justify-between{justify-content:space-between}.divide-y>:not([hidden])~:not([hidden]){--tw-divide-y-reverse:0;border-bottom-width:calc(1px*var(--tw-divide-y-reverse));border-top-width:calc(1px*(1 - var(--tw-divide-y-reverse)))}.divide-slate-300>:not([hidden])~:not([hidden]){--tw-divide-opacity:1;border-color:rgb(203 213 225/var(--tw-divide-opacity))}.break-words{overflow-wrap:break-word}.break-all{word-break:break-all}.border{border-width:1px}.border-l-8{border-left-width:8px}.border-l-\[12px\]{border-left-width:12px}.border-slate-300{--tw-border-opacity:1;border-color:rgb(203 213 225/var(--tw-border-opacity))}.border-l-violet-100{--tw-border-opacity:1;border-left-color:rgb(237 233 254/var(--tw-border-opacity))}.bg-indigo-900{--tw-bg-opacity:1;background-color:rgb(49 46 129/var(--tw-bg-opacity))}.bg-slate-100{--tw-bg-opacity:1;background-color:rgb(241 245 249/var(--tw-bg-opacity))}.fill-indigo-50{fill:#eef2ff}.p-2{padding:.5rem}.p-2\.5{padding:.625rem}.p-3{padding:.75rem}.p-6{padding:1.5rem}.p-8{padding:2rem}.px-1{padding-left:.25rem;padding-right:.25rem}.px-1\.5{padding-left:.375rem;padding-right:.375rem}.py-2{padding-bottom:.5rem;padding-top:.5rem}.py-2\.5{padding-bottom:.625rem;padding-top:.625rem}.py-3{padding-bottom:.75rem;padding-top:.75rem}.pb-4{padding-bottom:1rem}.pl-8{padding-left:2rem}.pr-20{padding-right:5rem}.font-mono{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace}.font-sans{font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji}.text-3xl{font-size:1.875rem;line-height:2.25rem}.text-base{font-size:1rem;line-height:1.5rem}.text-lg{font-size:1.125rem}.text-lg,.text-xl{line-height:1.75rem}.text-xl{font-size:1.25rem}.font-bold{font-weight:700}.font-medium{font-weight:500}.leading-none{line-height:1}.tracking-tight{letter-spacing:-.025em}.text-indigo-50{--tw-text-opacity:1;color:rgb(238 242 255/var(--tw-text-opacity))}.text-indigo-800{--tw-text-opacity:1;color:rgb(55 48 163/var(--tw-text-opacity))}.text-indigo-900{--tw-text-opacity:1;color:rgb(49 46 129/var(--tw-text-opacity))}.text-inherit{color:inherit}.text-slate-50{--tw-text-opacity:1;color:rgb(248 250 252/var(--tw-text-opacity))}.text-slate-600{--tw-text-opacity:1;color:rgb(71 85 105/var(--tw-text-opacity))}.text-slate-800{--tw-text-opacity:1;color:rgb(30 41 59/var(--tw-text-opacity))}.text-slate-900{--tw-text-opacity:1;color:rgb(15 23 42/var(--tw-text-opacity))}.underline{text-decoration-line:underline}.underline-offset-2{text-underline-offset:2px}.opacity-75{opacity:.75}.first\:pt-0:first-child{padding-top:0}.hover\:bg-indigo-800:hover{--tw-bg-opacity:1;background-color:rgb(55 48 163/var(--tw-bg-opacity))}.hover\:no-underline:hover{text-decoration-line:none}
+/*! tailwindcss v3.3.1 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}html{-webkit-text-size-adjust:100%;font-feature-settings:normal;font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-variation-settings:normal;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:initial}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:initial;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:initial}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}a{--tw-text-opacity:1;color:rgb(49 46 129/var(--tw-text-opacity));display:block;font-weight:500;width:100%}li{list-style-type:none}li:hover{--tw-bg-opacity:1;background-color:rgb(241 245 249/var(--tw-bg-opacity))}table{--tw-text-opacity:1;text-align:left;width:100%}table,thead{color:rgb(51 65 85/var(--tw-text-opacity))}thead{--tw-bg-opacity:1;--tw-text-opacity:1;background-color:rgb(248 250 252/var(--tw-bg-opacity));font-size:.875rem;line-height:1.25rem;text-transform:uppercase}th[scope=col]{padding:.75rem 1.5rem}th[scope=row]{--tw-text-opacity:1;color:rgb(15 23 42/var(--tw-text-opacity));font-weight:500;padding:1rem 1.5rem;white-space:nowrap}tr{--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));border-bottom-width:1px}td{padding-bottom:1rem;padding-top:1rem}section{margin-bottom:2rem;margin-top:2rem}*,::backdrop,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:#3b82f680;--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.rounded-pill{--tw-bg-opacity:1;--tw-text-opacity:1;background-color:rgb(226 232 240/var(--tw-bg-opacity));border-radius:9999px;color:rgb(71 85 105/var(--tw-text-opacity));font-size:.875rem;height:-moz-fit-content;height:fit-content;line-height:1.25rem;padding:.25rem .5rem}.text-muted{font-size:.875rem;line-height:1.25rem;opacity:.75}.listing-objects .text-muted{color:initial}.listing-form label{--tw-text-opacity:1;color:rgb(17 24 39/var(--tw-text-opacity));font-weight:500;margin-bottom:.25rem;margin-top:.25rem}.listing-form>div{display:flex;flex-direction:column;margin-bottom:.5rem;margin-top:.5rem}.listing-form select{--tw-border-opacity:1;--tw-bg-opacity:1;--tw-text-opacity:1;background-color:rgb(249 250 251/var(--tw-bg-opacity));border-color:rgb(209 213 219/var(--tw-border-opacity));border-radius:.5rem;border-width:1px;color:rgb(17 24 39/var(--tw-text-opacity));display:block;padding:.625rem;width:100%}.listing-form select:focus{--tw-border-opacity:1;--tw-ring-opacity:1;--tw-ring-color:rgb(99 102 241/var(--tw-ring-opacity));border-color:rgb(99 102 241/var(--tw-border-opacity))}[type=submit]{--tw-gradient-from:#4f46e5 var(--tw-gradient-from-position);--tw-gradient-from-position: ;--tw-gradient-to:#4f46e500 var(--tw-gradient-from-position);--tw-gradient-stops:var(--tw-gradient-from),var(--tw-gradient-to);--tw-gradient-via-position: ;--tw-gradient-to:#4338ca00 var(--tw-gradient-to-position);--tw-gradient-stops:var(--tw-gradient-from),#4338ca var(--tw-gradient-via-position),var(--tw-gradient-to);--tw-gradient-to:#3730a3 var(--tw-gradient-to-position);--tw-gradient-to-position: ;--tw-text-opacity:1;background-image:linear-gradient(to right,var(--tw-gradient-stops));border-radius:.5rem;color:rgb(255 255 255/var(--tw-text-opacity));font-size:.875rem;font-weight:500;line-height:1.25rem;margin-bottom:.5rem;margin-right:.5rem;padding:.625rem 1.25rem;text-align:center}.section__title{--tw-text-opacity:1;color:rgb(51 65 85/var(--tw-text-opacity));font-size:1.875rem;font-weight:700;line-height:2.25rem}.section__subtitle{--tw-text-opacity:1;color:rgb(71 85 105/var(--tw-text-opacity));font-size:1.25rem;font-weight:500;line-height:1.75rem;padding-bottom:.5rem;padding-top:.5rem}.section__body{margin-top:.5rem}.static{position:static}.m-2{margin:.5rem}.m-\[12px\]{margin:12px}.m-auto{margin:auto}.mx-10{margin-left:2.5rem;margin-right:2.5rem}.my-1{margin-bottom:.25rem;margin-top:.25rem}.my-2{margin-bottom:.5rem;margin-top:.5rem}.my-3{margin-bottom:.75rem;margin-top:.75rem}.my-4{margin-bottom:1rem;margin-top:1rem}.my-8{margin-bottom:2rem;margin-top:2rem}.-mr-1{margin-right:-.25rem}.mb-12{margin-bottom:3rem}.mb-2{margin-bottom:.5rem}.mb-3{margin-bottom:.75rem}.mb-4{margin-bottom:1rem}.mb-8{margin-bottom:2rem}.ml-1{margin-left:.25rem}.ml-1\.5{margin-left:.375rem}.ml-2{margin-left:.5rem}.mr-1{margin-right:.25rem}.mr-1\.5{margin-right:.375rem}.mr-5{margin-right:1.25rem}.mr-8{margin-right:2rem}.mt-10{margin-top:2.5rem}.mt-16{margin-top:4rem}.mt-2{margin-top:.5rem}.mt-4{margin-top:1rem}.mt-8{margin-top:2rem}.block{display:block}.flex{display:flex}.inline-flex{display:inline-flex}.table{display:table}.h-5{height:1.25rem}.h-px{height:1px}.min-h-screen{min-height:100vh}.w-1\/2{width:50%}.w-1\/3{width:33.333333%}.w-1\/5{width:20%}.w-11\/12{width:91.666667%}.w-2\/3{width:66.666667%}.w-3\/5{width:60%}.w-4\/5{width:80%}.w-5{width:1.25rem}.w-auto{width:auto}.w-full{width:100%}.w-max{width:-moz-max-content;width:max-content}.max-w-sm{max-width:24rem}.shrink-0{flex-shrink:0}.flex-grow,.grow{flex-grow:1}.cursor-pointer{cursor:pointer}.flex-col{flex-direction:column}.flex-wrap{flex-wrap:wrap}.items-center{align-items:center}.items-baseline{align-items:baseline}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.divide-y>:not([hidden])~:not([hidden]){--tw-divide-y-reverse:0;border-bottom-width:calc(1px*var(--tw-divide-y-reverse));border-top-width:calc(1px*(1 - var(--tw-divide-y-reverse)))}.divide-slate-300>:not([hidden])~:not([hidden]){--tw-divide-opacity:1;border-color:rgb(203 213 225/var(--tw-divide-opacity))}.break-words{overflow-wrap:break-word}.break-all{word-break:break-all}.rounded-lg{border-radius:.5rem}.rounded-t-lg{border-top-left-radius:.5rem;border-top-right-radius:.5rem}.border{border-width:1px}.border-0{border-width:0}.border-b{border-bottom-width:1px}.border-l-8{border-left-width:8px}.border-gray-200{--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity))}.border-slate-300{--tw-border-opacity:1;border-color:rgb(203 213 225/var(--tw-border-opacity))}.border-l-violet-100{--tw-border-opacity:1;border-left-color:rgb(237 233 254/var(--tw-border-opacity))}.bg-gray-200{--tw-bg-opacity:1;background-color:rgb(229 231 235/var(--tw-bg-opacity))}.bg-indigo-700{--tw-bg-opacity:1;background-color:rgb(67 56 202/var(--tw-bg-opacity))}.bg-indigo-900{--tw-bg-opacity:1;background-color:rgb(49 46 129/var(--tw-bg-opacity))}.bg-slate-100{--tw-bg-opacity:1;background-color:rgb(241 245 249/var(--tw-bg-opacity))}.bg-white{--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity))}.bg-gradient-to-l{background-image:linear-gradient(to left,var(--tw-gradient-stops))}.bg-gradient-to-r{background-image:linear-gradient(to right,var(--tw-gradient-stops))}.from-indigo-800{--tw-gradient-from:#3730a3 var(--tw-gradient-from-position);--tw-gradient-from-position: ;--tw-gradient-to:#3730a300 var(--tw-gradient-from-position);--tw-gradient-to-position: ;--tw-gradient-stops:var(--tw-gradient-from),var(--tw-gradient-to)}.to-indigo-900{--tw-gradient-to:#312e81 var(--tw-gradient-to-position);--tw-gradient-to-position: }.p-2{padding:.5rem}.p-2\.5{padding:.625rem}.p-3{padding:.75rem}.p-6{padding:1.5rem}.p-8{padding:2rem}.px-1{padding-left:.25rem;padding-right:.25rem}.px-1\.5{padding-left:.375rem;padding-right:.375rem}.px-4{padding-left:1rem;padding-right:1rem}.px-5{padding-left:1.25rem;padding-right:1.25rem}.py-2{padding-bottom:.5rem;padding-top:.5rem}.py-2\.5{padding-bottom:.625rem;padding-top:.625rem}.py-3{padding-bottom:.75rem;padding-top:.75rem}.py-4{padding-top:1rem}.pb-4,.py-4{padding-bottom:1rem}.pl-8{padding-left:2rem}.pr-20{padding-right:5rem}.text-center{text-align:center}.font-mono{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace}.font-sans{font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji}.text-3xl{font-size:1.875rem;line-height:2.25rem}.text-base{font-size:1rem;line-height:1.5rem}.text-lg{font-size:1.125rem}.text-lg,.text-xl{line-height:1.75rem}.text-xl{font-size:1.25rem}.font-bold{font-weight:700}.font-medium{font-weight:500}.leading-none{line-height:1}.tracking-tight{letter-spacing:-.025em}.text-gray-900{--tw-text-opacity:1;color:rgb(17 24 39/var(--tw-text-opacity))}.text-indigo-800{--tw-text-opacity:1;color:rgb(55 48 163/var(--tw-text-opacity))}.text-indigo-900{--tw-text-opacity:1;color:rgb(49 46 129/var(--tw-text-opacity))}.text-inherit{color:inherit}.text-slate-50{--tw-text-opacity:1;color:rgb(248 250 252/var(--tw-text-opacity))}.text-slate-600{--tw-text-opacity:1;color:rgb(71 85 105/var(--tw-text-opacity))}.text-slate-800{--tw-text-opacity:1;color:rgb(30 41 59/var(--tw-text-opacity))}.text-slate-900{--tw-text-opacity:1;color:rgb(15 23 42/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.underline{text-decoration-line:underline}.underline-offset-2{text-underline-offset:2px}.opacity-75{opacity:.75}.filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.first\:pt-0:first-child{padding-top:0}@media (prefers-color-scheme:dark){.dark\:bg-gray-700{--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}}
```

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/static/dj_tracker/js/query_group.js` & `django_trackings-0.6.0a0/src/dj_tracker/static/dj_tracker/js/query_group.js`

 * *Files identical despite different names*

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/templates/dj_tracker/base.html` & `django_trackings-0.6.0a0/src/dj_tracker/templates/dj_tracker/base.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 {% load static %}
 
 <html>
     <head>
         <meta charset="UTF-8">
         <meta http-equiv="X-UA-Compatible" content="IE=edge">
         <meta name="viewport" content="width=device-width, initial-scale=1.0">
-        <title>
-            {% block title %}
-            {% endblock title %}
-        </title>
+
+        <title>{% block title %}{% endblock title %}</title>
+
         <link rel="stylesheet" href="{% static 'dj_tracker/css/main.css' %}">
         <script defer src="https://cdn.jsdelivr.net/npm/alpinejs@3.x.x/dist/cdn.min.js"></script>
+
         {% block extra_js %}{% endblock extra_js %}
     </head>
 
     <body class="font-sans text-slate-900 flex flex-col min-h-screen">
-        <div class="bg-indigo-900 text-indigo-50 text-3xl p-6 pl-8 flex">
-            <a href="{% url 'trackings' %}"
-               class="text-inherit font-bold hover:no-underline">dj-tracker</a>
-            <span class="mx-2">-</span>
+        <div class="bg-gradient-to-r from-indigo-800 to-indigo-900 text-slate-50 text-3xl p-6 pl-8 flex justify-between">
             <h1 class="font-medium">
-                {% block h1 %}
-                {% endblock h1 %}
+                {% block h1 %}{% endblock h1 %}
             </h1>
+            <a href="{% url 'trackings' %}" class="text-inherit font-bold w-auto">dj-tracker</a>
         </div>
+
         <div class="mx-10 my-4 flex-grow">
-            {% block body %}
-            {% endblock body %}
+            {% block body %}{% endblock body %}
         </div>
-        <footer class="bg-indigo-900 p-8 pb-4 mt-16">
-            <a href="https://tijani-dia.github.io/dj-tracker/"
-               class="text-indigo-50 underline underline-offset-2">Docs</a>
+
+        <footer class="bg-gradient-to-r from-indigo-800 to-indigo-900 p-8 pb-4 mt-16">
+            <a href="https://tijani-dia.github.io/dj-tracker/" class="text-slate-50 underline underline-offset-2">Docs</a>
         </footer>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
 {% load static %}
 
 
  {% block extra_js %}{% endblock extra_js %}
-dj-tracker -
-****** {% block h1 %} {% endblock h1 %} ******
-{% block body %} {% endblock body %}
+****** {% block h1 %}{% endblock h1 %} ******
+dj-tracker
+{% block body %}{% endblock body %}
  Docs
```

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/templates/dj_tracker/qs_tracking.html` & `django_trackings-0.6.0a0/src/dj_tracker/templates/dj_tracker/includes/query.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 {% load dj_tracker %}
-
 <div class="mb-12"
-     id="{{ query_pk }}"
+     id="{{ query.pk }}"
      data-sql-id="{{ query.sql_id }}"
      data-traceback-id="{{ query.traceback_id }}"
      data-depth="{{ query.depth }}"
-     data-duplicate="{{ qs_tracking.duplicate }}"
-     data-related="{{ qs_tracking.related|length }}">
-    <h5 class="text-xl my-2 bg-indigo-900 p-2 border-l-[12px] border-l-violet-100">
-        <a href="{{ query.get_absolute_url }}" class="text-slate-50">{{ query_pk }}</a>
+     data-duplicate="{{ query.duplicate }}"
+     data-related="{{ query.related|length }}">
+    <h5 class="text-xl my-2 bg-gradient-to-l from-indigo-800 to-indigo-900 text-slate-50 p-2 flex justify-between">
+        <a href="{{ query.get_absolute_url }}" class="text-slate-50">{{ query.pk }}</a>
+        {% if query.from_other_query_group %}
+            <span class="rounded-pill"
+                  title="Indicates that this query (and not the related ones) comes from another request/query group.">
+                External
+            </span>
+        {% endif %}
     </h5>
     <dl class="flex flex-wrap text-lg m-[12px]">
         <dt class="w-1/3 font-medium text-slate-600 mb-2">
             Model
         </dt>
         <dd class="w-2/3">
             {{ query.model }}
@@ -31,20 +36,20 @@
         </dd>
         <dt class="w-1/3 font-medium text-slate-600 mb-2">
             Average duration
         </dt>
         <dd class="w-2/3">
             {{ query.average_duration_in_ms }} ms
         </dd>
-        {% if qs_tracking.duplicate %}
+        {% if query.duplicate %}
             <dt class="w-1/3 font-medium text-slate-600 mb-2">
                 Repeated
             </dt>
             <dd class="w-2/3">
-                {{ qs_tracking.num_occurrences }} time(s)
+                {{ query.num_occurrences }} time(s)
             </dd>
         {% endif %}
         {% if query.field %}
             <dt class="w-1/3 font-medium text-slate-600 mb-2">
                 Field
             </dt>
             <dd class="w-2/3">
@@ -111,33 +116,31 @@
                 </dt>
                 <dd class="w-2/3">
                     {{ query.iterable_class }}
                 </dd>
             {% endif %}
         {% endif %}
     </dl>
-
-    {% if qs_tracking.related %}
+    {% if query.related %}
         <h5 class="m-2 text-lg font-medium text-slate-600">Related</h5>
         <div id="query-{{ query_pk }}"
              x-data="{ current: null }"
              class="divide-y divide-slate-300 w-full ml-2">
-            {% for field, related_trackings in qs_tracking.related.items %}
+            {% for field, related_queries in query.related.items %}
                 <div x-data>
-                    <div class="flex justify-between items-baseline py-3 px-1.5 bg-indigo-900 text-slate-50 border-l-8 border-l-violet-100 w-full">
-                        <h2 class="leading-none">
-                            <button @click="current = current === $root ? null : $root">{{ field }}</button>
-                        </h2>
-                        {% with num_queries=related_trackings|total_queries %}
+                    <div class="flex justify-between items-baseline px-1.5 bg-indigo-900 text-slate-50 border-l-8 border-l-violet-100 w-full">
+                        <h2 class="leading-none flex-grow py-4"
+                            @click="current = current === $root ? null : $root">{{ field }}</h2>
+                        {% with num_queries=related_queries|total_queries %}
                             <small class="text-muted">{{ num_queries }} quer{{ num_queries|pluralize:"y,ies" }}</small>
                         {% endwith %}
                     </div>
                     <div x-show="current === $root" class="my-4 mx-10">
-                        {% for related_qs in related_trackings %}
-                            {% include "dj_tracker/qs_tracking.html" with qs_tracking=related_qs query=related_qs.query query_pk=related_qs.query.pk %}
+                        {% for related_query in related_queries %}
+                            {% include "dj_tracker/includes/query.html" with query=related_query %}
                         {% endfor %}
                     </div>
                 </div>
             {% endfor %}
         </div>
     {% endif %}
 </div>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% load dj_tracker %}
-** {{_query_pk_}} **
+** {{_query.pk_}} {% if query.from_other_query_group %}  External  {% endif %}
+**
   .__len__
       {{ query.len_calls }}
   .__bool__
       {{ query.exists_calls }}
   .__contains__
       {{ query.contains_calls }}
 {% endif %} {% if query.iterable_class %} {% if query.iterable_class ==
@@ -11,18 +12,17 @@
 Model attributes accessed
 click="open = !open">Show
 {% for attr, count in query.attributes_accessed.items %}
 {% endif %} {% else %}
 Iterable class
 {{ query.iterable_class }}
 {% endif %} {% endif %}
-{% if qs_tracking.related %}
+{% if query.related %}
 ** Related **
-{% for field, related_trackings in qs_tracking.related.items %}
-***** click="current = current === $root ? null : $root">{{ field }} *****
-{% with num_queries=related_trackings|total_queries %} {{ num_queries }} quer{
+{% for field, related_queries in query.related.items %}
+click="current = current === $root ? null : $root">{{ field }}
+{% with num_queries=related_queries|total_queries %} {{ num_queries }} quer{
 { num_queries|pluralize:"y,ies" }} {% endwith %}
-{% for related_qs in related_trackings %} {% include "dj_tracker/
-qs_tracking.html" with qs_tracking=related_qs query=related_qs.query
-query_pk=related_qs.query.pk %} {% endfor %}
+{% for related_query in related_queries %} {% include "dj_tracker/includes/
+query.html" with query=related_query %} {% endfor %}
 {% endfor %}
 {% endif %}
```

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/templates/dj_tracker/query_group.html` & `django_trackings-0.6.0a0/src/dj_tracker/templates/dj_tracker/query_group.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,77 @@
 {% extends "dj_tracker/base.html" %}
 
 {% load static %}
 
 {% block title %}Query Group #{{ object.pk }}{% endblock %}
-
 {% block h1 %}
     Query Group {{ object.pk }}
     <small class="text-muted">{{ object.num_queries }} quer{{ object.num_queries|pluralize:"y,ies" }}</small>
 {% endblock %}
 
 {% block body %}
     <section class="flex">
         <div class="shrink-0 pr-20 max-w-sm">
             <form>
                 <fieldset>
-                    <legend class="section__subtitle">Filter</legend>
+                    <legend class="section__subtitle">
+                        Filter
+                    </legend>
                     <div class="mb-3">
-                        <input type="radio" id="show-related" name="select" data-select-type="related" value="related">
+                        <input type="radio"
+                               id="show-related"
+                               name="select"
+                               data-select-type="related"
+                               value="related">
                         <label class="ml-1.5" for="show-related">Related</label>
                     </div>
                     <div>
-                        <input type="radio" id="show-duplicates" name="select" data-select-type="duplicates" value="duplicates">
+                        <input type="radio"
+                               id="show-duplicates"
+                               name="select"
+                               data-select-type="duplicates"
+                               value="duplicates">
                         <label class="ml-1.5" for="show-duplicates">Duplicates</label>
                     </div>
                 </fieldset>
 
                 {% if similar_sqls %}
                     <fieldset>
                         <legend class="section__subtitle">Similar SQLs</legend>
                         {% for sql_id, objs in similar_sqls %}
                             <div class="mb-3 flex justify-between">
                                 <label for="show-sql-{{ sql_id }}" class="shrink-0 flex items-center mr-5">
                                     <span class="rounded-pill mr-1.5">{{ objs }}</span>
                                     <span>{{ sql_id }}</span>
                                 </label>
-                                <input type="radio" id="show-sql-{{ sql_id }}" name="select" data-select-type="sql" value="{{ sql_id }}">
+                                <input type="radio"
+                                       id="show-sql-{{ sql_id }}"
+                                       name="select"
+                                       data-select-type="sql"
+                                       value="{{ sql_id }}">
                             </div>
                         {% endfor %}
                     </fieldset>
                 {% endif %}
 
                 {% if similar_tracebacks %}
                     <fieldset>
                         <legend class="section__subtitle">Similar Tracebacks</legend>
                         {% for traceback_id, objs in similar_tracebacks %}
                             <div class="mb-3 flex justify-between">
-                                <label for="show-traceback-{{ traceback_id }}" class="shrink-0 flex items-center mr-5">
+                                <label for="show-traceback-{{ traceback_id }}"
+                                       class="shrink-0 flex items-center mr-5">
                                     <span class="rounded-pill mr-1.5">{{ objs }}</span>
                                     <span>{{ traceback_id }}</span>
                                 </label>
-                                <input type="radio" id="show-traceback-{{ traceback_id }}" name="select" data-select-type="traceback" value="{{ traceback_id }}">
+                                <input type="radio"
+                                       id="show-traceback-{{ traceback_id }}"
+                                       name="select"
+                                       data-select-type="traceback"
+                                       value="{{ traceback_id }}">
                             </div>
                         {% endfor %}
                     </fieldset>
                 {% endif %}
             </form>
 
             <h5 class="section__subtitle mt-4">Requests</h5>
@@ -61,19 +79,20 @@
                 {% for request in requests %}
                     <li class="py-2.5 first:pt-0">
                         <a href="{{ request.get_absolute_url }}" class="break-words">{{ request }}</a>
                     </li>
                 {% endfor %}
             </ol>
         </div>
+
         <div class="grow">
             <h5 class="section__subtitle">Queries</h5>
             <div>
-                {% for qs_tracking in qs_trackings %}
-                    {% include "dj_tracker/qs_tracking.html" with qs_tracking=qs_tracking query=qs_tracking.query query_pk=qs_tracking.query.pk %}
+                {% for query in queries %}
+                    {% include "dj_tracker/includes/query.html" with query=query %}
                 {% endfor %}
             </div>
         </div>
     </section>
 {% endblock %}
 
 {% block extra_js %}
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
 {% extends "dj_tracker/base.html" %} {% load static %} {% block title %}Query
 Group #{{ object.pk }}{% endblock %} {% block h1 %} Query Group {{ object.pk }}
 {{ object.num_queries }} quer{{ object.num_queries|pluralize:"y,ies" }} {%
 endblock %} {% block body %}
- Filter
+  Filter
 o Related
 o Duplicates
  {% if similar_sqls %}  Similar SQLs {% for sql_id, objs in similar_sqls %}
  {{ objs }} {{ sql_id }}  o
 {% endfor %}  {% endif %} {% if similar_tracebacks %}  Similar Tracebacks {%
 for traceback_id, objs in similar_tracebacks %}
  {{ objs }} {{ traceback_id }}  o
 {% endfor %}  {% endif %}
 ** Requests **
    1. {% for request in requests %}
    2. {{_request_}}
    3. {% endfor %}
 ** Queries **
-{% for qs_tracking in qs_trackings %} {% include "dj_tracker/qs_tracking.html"
-with qs_tracking=qs_tracking query=qs_tracking.query
-query_pk=qs_tracking.query.pk %} {% endfor %}
+{% for query in queries %} {% include "dj_tracker/includes/query.html" with
+query=query %} {% endfor %}
  {% endblock %} {% block extra_js %}
  {% endblock %}
```

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/templates/dj_tracker/queryset_tracking.html` & `django_trackings-0.6.0a0/src/dj_tracker/templates/dj_tracker/query.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 {% extends "dj_tracker/base.html" %}
 
 {% block title %}Queryset {{ object.pk }}{% endblock %}
-
 {% block h1 %}
     Queryset {{ object.pk }}
     <small class="text-muted">{{ object.num_instances }} instance{{ object.num_instances|pluralize }} tracked.</small>
 {% endblock %}
 
 {% block body %}
     <section class="flex w-full"
@@ -28,14 +27,15 @@
         <div class="flex-grow mr-8 w-3/5">
             <div x-show="showSQL">
                 <h5 class="section__subtitle">SQL</h5>
                 <code class="font-mono font-medium text-slate-800 tracking-tight">
                     {{ object.sql }}
                 </code>
             </div>
+
             <div x-show="showTraceback">
                 {% if object.traceback.template_info %}
                     <h5 class="section__subtitle">Template Info</h5>
                     <p class="bg-slate-100 font-medium text-slate-800 p-2.5">
                         {{ object.traceback.template_info.filename }}:{{ object.traceback.template_info.lineno }}
                     </p>
                     <div class="p-2 mb-4">
@@ -52,14 +52,15 @@
                                     <code>{{ entry.code }}</code>
                                 </div>
                             {% endfor %}
                         </div>
                     {% endif %}
                 {% endwith %}
             </div>
+
             <div x-show="showFieldStats">
                 <h5 class="section__subtitle">Fields stats</h5>
                 {% for instance_tracking in object.instance_trackings.all %}
                     <h4 class="font-medium text-lg text-indigo-800 my-2">{{ instance_tracking.select_related_field }}</h4>
                     <table class="mb-8 w-full">
                         <thead>
                             <tr>
@@ -81,14 +82,15 @@
                         </tbody>
                     </table>
                 {% empty %}
                     <p>No field stats available.</p>
                 {% endfor %}
             </div>
         </div>
+
         <div class="w-1/5">
             <h4 class="section__subtitle">Hints</h4>
             <ul>
                 {% for hint in object.get_hints %}
                     <li>{{ hint }}</li>
                 {% empty %}
                     <p>No hints available</p>
```

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/test/__init__.py` & `django_trackings-0.6.0a0/src/dj_tracker/test/__init__.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/traceback.c` & `django_trackings-0.6.0a0/src/dj_tracker/traceback.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.0b1 */
+/* Generated by Cython 3.0.0b2 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "CYTHON_TRACE",
@@ -39,18 +39,18 @@
 
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0b1"
+#define CYTHON_ABI "3_0_0b2"
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000B1
+#define CYTHON_HEX_VERSION 0x030000B2
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -1321,55 +1321,55 @@
 struct __pyx_obj_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr;
 struct __pyx_obj_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info;
 struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry;
 struct __pyx_obj_10dj_tracker_11cache_utils_LRUCache;
 struct __pyx_opt_args_10dj_tracker_9traceback_get_file_info;
 struct __pyx_opt_args_10dj_tracker_9traceback_get_entry;
 
-/* "dj_tracker/traceback.pyx":85
+/* "dj_tracker/traceback.pyx":88
  * 
  * 
  * cdef tuple get_file_info(str filename, PyFrameObject *frame, dict cache = {}):             # <<<<<<<<<<<<<<
  *     """Retrieves the relative path for a filename and indicates if it should be ignored."""
  *     cdef:
  */
 struct __pyx_opt_args_10dj_tracker_9traceback_get_file_info {
   int __pyx_n;
   PyObject *cache;
 };
 
-/* "dj_tracker/traceback.pyx":118
+/* "dj_tracker/traceback.pyx":121
  * 
  * 
  * cdef inline TracebackEntry get_entry(             # <<<<<<<<<<<<<<
  *     str filename,
  *     object lineno,
  */
 struct __pyx_opt_args_10dj_tracker_9traceback_get_entry {
   int __pyx_n;
   PyCodeObject *code;
   struct __pyx_obj_10dj_tracker_11cache_utils_LRUCache *cache;
 };
 
-/* "dj_tracker/traceback.pyx":113
+/* "dj_tracker/traceback.pyx":116
  * 
  *         rel_path = os.path.relpath(filename, module_dir)
  *         ignore = any(module in filename for module in IGNORED_MODULES)             # <<<<<<<<<<<<<<
  *         cache[filename] = file_info = rel_path, ignore
  *         return file_info
  */
 struct __pyx_obj_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr {
   PyObject_HEAD
   struct __pyx_obj_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info *__pyx_outer_scope;
   PyObject *__pyx_genexpr_arg_0;
   PyObject *__pyx_v_module;
 };
 
 
-/* "dj_tracker/traceback.pyx":95
+/* "dj_tracker/traceback.pyx":98
  *     except KeyError:
  *         try:
  *             module_dir = next(path for path in sys.path if filename.startswith(path))             # <<<<<<<<<<<<<<
  *         except StopIteration:
  *             # The following logic is inspired from:
  */
 struct __pyx_obj_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr {
@@ -1379,15 +1379,15 @@
   PyObject *__pyx_v_path;
   PyObject *__pyx_t_0;
   Py_ssize_t __pyx_t_1;
   PyObject *(*__pyx_t_2)(PyObject *);
 };
 
 
-/* "dj_tracker/traceback.pyx":85
+/* "dj_tracker/traceback.pyx":88
  * 
  * 
  * cdef tuple get_file_info(str filename, PyFrameObject *frame, dict cache = {}):             # <<<<<<<<<<<<<<
  *     """Retrieves the relative path for a filename and indicates if it should be ignored."""
  *     cdef:
  */
 struct __pyx_obj_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info {
@@ -1728,14 +1728,55 @@
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
 /* PyObjectFastCall.proto */
 #define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
 
+/* PyUnicode_Unicode.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyUnicode_Unicode(PyObject *obj);
+
+/* GCCDiagnostics.proto */
+#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
+
+/* BuildPyUnicode.proto */
+static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
+                                                int prepend_sign, char padding_char);
+
+/* CIntToPyUnicode.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_int(int value, Py_ssize_t width, char padding_char, char format_char);
+
+/* PyObjectFormatSimple.proto */
+#if CYTHON_COMPILING_IN_PYPY
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        PyObject_Format(s, f))
+#elif PY_MAJOR_VERSION < 3
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        likely(PyString_CheckExact(s)) ? PyUnicode_FromEncodedObject(s, NULL, "strict") :\
+        PyObject_Format(s, f))
+#elif CYTHON_USE_TYPE_SLOTS
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        likely(PyLong_CheckExact(s)) ? PyLong_Type.tp_repr(s) :\
+        likely(PyFloat_CheckExact(s)) ? PyFloat_Type.tp_repr(s) :\
+        PyObject_Format(s, f))
+#else
+    #define __Pyx_PyObject_FormatSimple(s, f) (\
+        likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
+        PyObject_Format(s, f))
+#endif
+
+/* JoinPyUnicode.proto */
+static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
+                                      Py_UCS4 max_char);
+
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* KeywordStringCheck.proto */
@@ -1965,14 +2006,17 @@
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyTypeObject *type);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
+#endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
@@ -2112,19 +2156,14 @@
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
 #endif
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
-/* GCCDiagnostics.proto */
-#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
-#define __Pyx_HAS_GCC_DIAGNOSTIC
-#endif
-
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntFromPy.proto */
@@ -2293,25 +2332,28 @@
 /* Implementation of "dj_tracker.traceback" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_AttributeError;
 static PyObject *__pyx_builtin_KeyError;
 static PyObject *__pyx_builtin_StopIteration;
 static PyObject *__pyx_builtin_NameError;
 /* #### Code section: string_decls ### */
-static const char __pyx_k__2[] = "";
-static const char __pyx_k__3[] = ".";
-static const char __pyx_k__8[] = "*";
+static const char __pyx_k_[] = ":";
+static const char __pyx_k__2[] = " - ";
+static const char __pyx_k__4[] = "";
+static const char __pyx_k__5[] = ".";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_os[] = "os";
-static const char __pyx_k__16[] = "?";
+static const char __pyx_k__10[] = "*";
+static const char __pyx_k__18[] = "?";
 static const char __pyx_k_get[] = "get";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_sep[] = "sep";
 static const char __pyx_k_sys[] = "sys";
 static const char __pyx_k_Node[] = "Node";
+static const char __pyx_k_None[] = "None";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_code[] = "code";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_file[] = "__file__";
 static const char __pyx_k_func[] = "func";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "name";
@@ -2393,21 +2435,22 @@
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x6d8739c, 0xdb324b9, 0x268af81) = (filename, func, hash_value, ignore, is_render, lineno, rel_path))";
 static const char __pyx_k_TracebackEntry___setstate_cython[] = "TracebackEntry.__setstate_cython__";
 /* #### Code section: decls ### */
 static int __pyx_pf_10dj_tracker_9traceback_14TracebackEntry___init__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self, PyObject *__pyx_v_filename, PyObject *__pyx_v_rel_path, int __pyx_v_ignore, int __pyx_v_lineno, PyObject *__pyx_v_func); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_11filename_id___get__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_4code___get__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_9cache_key___get__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_2__getattr__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self, PyObject *__pyx_v_name); /* proto */
+static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_2__repr__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_4__getattr__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self, PyObject *__pyx_v_name); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_8filename___get__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_8rel_path___get__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_6lineno___get__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_4func___get__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_4__reduce_cython__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_6__setstate_cython__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_6__reduce_cython__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_8__setstate_cython__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_9traceback_13get_file_info_genexpr(PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_9traceback_13get_file_info_3genexpr(PyObject *__pyx_self, PyObject *__pyx_genexpr_arg_0); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_9traceback_get_traceback(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_10dj_tracker_9traceback_2__pyx_unpickle_TracebackEntry(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
@@ -2466,31 +2509,34 @@
   PyObject *__pyx_type_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info;
   PyObject *__pyx_type_10dj_tracker_9traceback_TracebackEntry;
   #endif
   PyTypeObject *__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr;
   PyTypeObject *__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr;
   PyTypeObject *__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info;
   PyTypeObject *__pyx_ptype_10dj_tracker_9traceback_TracebackEntry;
+  PyObject *__pyx_kp_u_;
   PyObject *__pyx_n_s_AttributeError;
   PyObject *__pyx_n_s_HashableList;
   PyObject *__pyx_n_s_IGNORED_MODULES;
   PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
   PyObject *__pyx_n_s_KeyError;
   PyObject *__pyx_n_s_NameError;
   PyObject *__pyx_n_s_Node;
+  PyObject *__pyx_kp_u_None;
   PyObject *__pyx_n_s_PickleError;
   PyObject *__pyx_n_s_SourceFilePromise;
   PyObject *__pyx_n_s_StopIteration;
   PyObject *__pyx_n_s_TracebackEntry;
   PyObject *__pyx_n_s_TracebackEntry___reduce_cython;
   PyObject *__pyx_n_s_TracebackEntry___setstate_cython;
-  PyObject *__pyx_n_s__16;
+  PyObject *__pyx_n_s__10;
+  PyObject *__pyx_n_s__18;
   PyObject *__pyx_kp_u__2;
-  PyObject *__pyx_kp_u__3;
-  PyObject *__pyx_n_s__8;
+  PyObject *__pyx_kp_u__4;
+  PyObject *__pyx_kp_u__5;
   PyObject *__pyx_n_s_args;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_close;
   PyObject *__pyx_n_s_code;
   PyObject *__pyx_n_s_dict;
   PyObject *__pyx_n_s_dict_2;
@@ -2569,26 +2615,26 @@
   PyObject *__pyx_n_s_use_setstate;
   PyObject *__pyx_int_1;
   PyObject *__pyx_int_2;
   PyObject *__pyx_int_512;
   PyObject *__pyx_int_40415105;
   PyObject *__pyx_int_114848668;
   PyObject *__pyx_int_229844153;
-  PyObject *__pyx_k_;
-  struct __pyx_obj_10dj_tracker_11cache_utils_LRUCache *__pyx_k__5;
-  PyObject *__pyx_tuple__4;
+  PyObject *__pyx_k__3;
+  struct __pyx_obj_10dj_tracker_11cache_utils_LRUCache *__pyx_k__7;
   PyObject *__pyx_tuple__6;
-  PyObject *__pyx_tuple__7;
+  PyObject *__pyx_tuple__8;
   PyObject *__pyx_tuple__9;
   PyObject *__pyx_tuple__11;
-  PyObject *__pyx_tuple__14;
-  PyObject *__pyx_codeobj__10;
+  PyObject *__pyx_tuple__13;
+  PyObject *__pyx_tuple__16;
   PyObject *__pyx_codeobj__12;
-  PyObject *__pyx_codeobj__13;
+  PyObject *__pyx_codeobj__14;
   PyObject *__pyx_codeobj__15;
+  PyObject *__pyx_codeobj__17;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -2633,31 +2679,34 @@
   Py_CLEAR(clear_module_state->__pyx_type_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr);
   Py_CLEAR(clear_module_state->__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr);
   Py_CLEAR(clear_module_state->__pyx_type_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr);
   Py_CLEAR(clear_module_state->__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info);
   Py_CLEAR(clear_module_state->__pyx_type_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info);
   Py_CLEAR(clear_module_state->__pyx_ptype_10dj_tracker_9traceback_TracebackEntry);
   Py_CLEAR(clear_module_state->__pyx_type_10dj_tracker_9traceback_TracebackEntry);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_);
   Py_CLEAR(clear_module_state->__pyx_n_s_AttributeError);
   Py_CLEAR(clear_module_state->__pyx_n_s_HashableList);
   Py_CLEAR(clear_module_state->__pyx_n_s_IGNORED_MODULES);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_CLEAR(clear_module_state->__pyx_n_s_KeyError);
   Py_CLEAR(clear_module_state->__pyx_n_s_NameError);
   Py_CLEAR(clear_module_state->__pyx_n_s_Node);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_None);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_SourceFilePromise);
   Py_CLEAR(clear_module_state->__pyx_n_s_StopIteration);
   Py_CLEAR(clear_module_state->__pyx_n_s_TracebackEntry);
   Py_CLEAR(clear_module_state->__pyx_n_s_TracebackEntry___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_TracebackEntry___setstate_cython);
-  Py_CLEAR(clear_module_state->__pyx_n_s__16);
+  Py_CLEAR(clear_module_state->__pyx_n_s__10);
+  Py_CLEAR(clear_module_state->__pyx_n_s__18);
   Py_CLEAR(clear_module_state->__pyx_kp_u__2);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__3);
-  Py_CLEAR(clear_module_state->__pyx_n_s__8);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__4);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__5);
   Py_CLEAR(clear_module_state->__pyx_n_s_args);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_close);
   Py_CLEAR(clear_module_state->__pyx_n_s_code);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict_2);
@@ -2736,26 +2785,26 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_use_setstate);
   Py_CLEAR(clear_module_state->__pyx_int_1);
   Py_CLEAR(clear_module_state->__pyx_int_2);
   Py_CLEAR(clear_module_state->__pyx_int_512);
   Py_CLEAR(clear_module_state->__pyx_int_40415105);
   Py_CLEAR(clear_module_state->__pyx_int_114848668);
   Py_CLEAR(clear_module_state->__pyx_int_229844153);
-  Py_CLEAR(clear_module_state->__pyx_k_);
-  Py_CLEAR(clear_module_state->__pyx_k__5);
-  Py_CLEAR(clear_module_state->__pyx_tuple__4);
+  Py_CLEAR(clear_module_state->__pyx_k__3);
+  Py_CLEAR(clear_module_state->__pyx_k__7);
   Py_CLEAR(clear_module_state->__pyx_tuple__6);
-  Py_CLEAR(clear_module_state->__pyx_tuple__7);
+  Py_CLEAR(clear_module_state->__pyx_tuple__8);
   Py_CLEAR(clear_module_state->__pyx_tuple__9);
   Py_CLEAR(clear_module_state->__pyx_tuple__11);
-  Py_CLEAR(clear_module_state->__pyx_tuple__14);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__10);
+  Py_CLEAR(clear_module_state->__pyx_tuple__13);
+  Py_CLEAR(clear_module_state->__pyx_tuple__16);
   Py_CLEAR(clear_module_state->__pyx_codeobj__12);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__13);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__14);
   Py_CLEAR(clear_module_state->__pyx_codeobj__15);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__17);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -2778,31 +2827,34 @@
   Py_VISIT(traverse_module_state->__pyx_type_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr);
   Py_VISIT(traverse_module_state->__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr);
   Py_VISIT(traverse_module_state->__pyx_type_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr);
   Py_VISIT(traverse_module_state->__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info);
   Py_VISIT(traverse_module_state->__pyx_type_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info);
   Py_VISIT(traverse_module_state->__pyx_ptype_10dj_tracker_9traceback_TracebackEntry);
   Py_VISIT(traverse_module_state->__pyx_type_10dj_tracker_9traceback_TracebackEntry);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_);
   Py_VISIT(traverse_module_state->__pyx_n_s_AttributeError);
   Py_VISIT(traverse_module_state->__pyx_n_s_HashableList);
   Py_VISIT(traverse_module_state->__pyx_n_s_IGNORED_MODULES);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_VISIT(traverse_module_state->__pyx_n_s_KeyError);
   Py_VISIT(traverse_module_state->__pyx_n_s_NameError);
   Py_VISIT(traverse_module_state->__pyx_n_s_Node);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_None);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_SourceFilePromise);
   Py_VISIT(traverse_module_state->__pyx_n_s_StopIteration);
   Py_VISIT(traverse_module_state->__pyx_n_s_TracebackEntry);
   Py_VISIT(traverse_module_state->__pyx_n_s_TracebackEntry___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_TracebackEntry___setstate_cython);
-  Py_VISIT(traverse_module_state->__pyx_n_s__16);
+  Py_VISIT(traverse_module_state->__pyx_n_s__10);
+  Py_VISIT(traverse_module_state->__pyx_n_s__18);
   Py_VISIT(traverse_module_state->__pyx_kp_u__2);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__3);
-  Py_VISIT(traverse_module_state->__pyx_n_s__8);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__4);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__5);
   Py_VISIT(traverse_module_state->__pyx_n_s_args);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_close);
   Py_VISIT(traverse_module_state->__pyx_n_s_code);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict_2);
@@ -2881,26 +2933,26 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_use_setstate);
   Py_VISIT(traverse_module_state->__pyx_int_1);
   Py_VISIT(traverse_module_state->__pyx_int_2);
   Py_VISIT(traverse_module_state->__pyx_int_512);
   Py_VISIT(traverse_module_state->__pyx_int_40415105);
   Py_VISIT(traverse_module_state->__pyx_int_114848668);
   Py_VISIT(traverse_module_state->__pyx_int_229844153);
-  Py_VISIT(traverse_module_state->__pyx_k_);
-  Py_VISIT(traverse_module_state->__pyx_k__5);
-  Py_VISIT(traverse_module_state->__pyx_tuple__4);
+  Py_VISIT(traverse_module_state->__pyx_k__3);
+  Py_VISIT(traverse_module_state->__pyx_k__7);
   Py_VISIT(traverse_module_state->__pyx_tuple__6);
-  Py_VISIT(traverse_module_state->__pyx_tuple__7);
+  Py_VISIT(traverse_module_state->__pyx_tuple__8);
   Py_VISIT(traverse_module_state->__pyx_tuple__9);
   Py_VISIT(traverse_module_state->__pyx_tuple__11);
-  Py_VISIT(traverse_module_state->__pyx_tuple__14);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__10);
+  Py_VISIT(traverse_module_state->__pyx_tuple__13);
+  Py_VISIT(traverse_module_state->__pyx_tuple__16);
   Py_VISIT(traverse_module_state->__pyx_codeobj__12);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__13);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__14);
   Py_VISIT(traverse_module_state->__pyx_codeobj__15);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__17);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -2951,31 +3003,34 @@
 #define __pyx_type_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info __pyx_mstate_global->__pyx_type_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info
 #define __pyx_type_10dj_tracker_9traceback_TracebackEntry __pyx_mstate_global->__pyx_type_10dj_tracker_9traceback_TracebackEntry
 #endif
 #define __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr __pyx_mstate_global->__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr
 #define __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr __pyx_mstate_global->__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr
 #define __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info __pyx_mstate_global->__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info
 #define __pyx_ptype_10dj_tracker_9traceback_TracebackEntry __pyx_mstate_global->__pyx_ptype_10dj_tracker_9traceback_TracebackEntry
+#define __pyx_kp_u_ __pyx_mstate_global->__pyx_kp_u_
 #define __pyx_n_s_AttributeError __pyx_mstate_global->__pyx_n_s_AttributeError
 #define __pyx_n_s_HashableList __pyx_mstate_global->__pyx_n_s_HashableList
 #define __pyx_n_s_IGNORED_MODULES __pyx_mstate_global->__pyx_n_s_IGNORED_MODULES
 #define __pyx_kp_s_Incompatible_checksums_0x_x_vs_0 __pyx_mstate_global->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0
 #define __pyx_n_s_KeyError __pyx_mstate_global->__pyx_n_s_KeyError
 #define __pyx_n_s_NameError __pyx_mstate_global->__pyx_n_s_NameError
 #define __pyx_n_s_Node __pyx_mstate_global->__pyx_n_s_Node
+#define __pyx_kp_u_None __pyx_mstate_global->__pyx_kp_u_None
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
 #define __pyx_n_s_SourceFilePromise __pyx_mstate_global->__pyx_n_s_SourceFilePromise
 #define __pyx_n_s_StopIteration __pyx_mstate_global->__pyx_n_s_StopIteration
 #define __pyx_n_s_TracebackEntry __pyx_mstate_global->__pyx_n_s_TracebackEntry
 #define __pyx_n_s_TracebackEntry___reduce_cython __pyx_mstate_global->__pyx_n_s_TracebackEntry___reduce_cython
 #define __pyx_n_s_TracebackEntry___setstate_cython __pyx_mstate_global->__pyx_n_s_TracebackEntry___setstate_cython
-#define __pyx_n_s__16 __pyx_mstate_global->__pyx_n_s__16
+#define __pyx_n_s__10 __pyx_mstate_global->__pyx_n_s__10
+#define __pyx_n_s__18 __pyx_mstate_global->__pyx_n_s__18
 #define __pyx_kp_u__2 __pyx_mstate_global->__pyx_kp_u__2
-#define __pyx_kp_u__3 __pyx_mstate_global->__pyx_kp_u__3
-#define __pyx_n_s__8 __pyx_mstate_global->__pyx_n_s__8
+#define __pyx_kp_u__4 __pyx_mstate_global->__pyx_kp_u__4
+#define __pyx_kp_u__5 __pyx_mstate_global->__pyx_kp_u__5
 #define __pyx_n_s_args __pyx_mstate_global->__pyx_n_s_args
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_close __pyx_mstate_global->__pyx_n_s_close
 #define __pyx_n_s_code __pyx_mstate_global->__pyx_n_s_code
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
 #define __pyx_n_s_dict_2 __pyx_mstate_global->__pyx_n_s_dict_2
@@ -3054,26 +3109,26 @@
 #define __pyx_n_s_use_setstate __pyx_mstate_global->__pyx_n_s_use_setstate
 #define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
 #define __pyx_int_2 __pyx_mstate_global->__pyx_int_2
 #define __pyx_int_512 __pyx_mstate_global->__pyx_int_512
 #define __pyx_int_40415105 __pyx_mstate_global->__pyx_int_40415105
 #define __pyx_int_114848668 __pyx_mstate_global->__pyx_int_114848668
 #define __pyx_int_229844153 __pyx_mstate_global->__pyx_int_229844153
-#define __pyx_k_ __pyx_mstate_global->__pyx_k_
-#define __pyx_k__5 __pyx_mstate_global->__pyx_k__5
-#define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
+#define __pyx_k__3 __pyx_mstate_global->__pyx_k__3
+#define __pyx_k__7 __pyx_mstate_global->__pyx_k__7
 #define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
-#define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
+#define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
 #define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
 #define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
-#define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
-#define __pyx_codeobj__10 __pyx_mstate_global->__pyx_codeobj__10
+#define __pyx_tuple__13 __pyx_mstate_global->__pyx_tuple__13
+#define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
 #define __pyx_codeobj__12 __pyx_mstate_global->__pyx_codeobj__12
-#define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
+#define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
 #define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
+#define __pyx_codeobj__17 __pyx_mstate_global->__pyx_codeobj__17
 /* #### Code section: module_code ### */
 
 /* "dj_tracker/traceback.pyx":50
  *         int hash_value
  * 
  *     def __init__(self, str filename, str rel_path, bint ignore, int lineno, str func):             # <<<<<<<<<<<<<<
  *         self.filename = filename
@@ -3673,114 +3728,220 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "dj_tracker/traceback.pyx":77
  *         )
  * 
+ *     def __repr__(self):             # <<<<<<<<<<<<<<
+ *         return f"{self.rel_path}:{self.lineno} - {self.code}"
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_3__repr__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_3__repr__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__repr__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_10dj_tracker_9traceback_14TracebackEntry_2__repr__(((struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_2__repr__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  Py_UCS4 __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__repr__", 0);
+
+  /* "dj_tracker/traceback.pyx":78
+ * 
+ *     def __repr__(self):
+ *         return f"{self.rel_path}:{self.lineno} - {self.code}"             # <<<<<<<<<<<<<<
+ * 
+ *     def __getattr__(self, name):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyTuple_New(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = 0;
+  __pyx_t_3 = 127;
+  __pyx_t_4 = __Pyx_PyUnicode_Unicode(__pyx_v_self->rel_path); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_3;
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
+  __pyx_t_4 = 0;
+  __Pyx_INCREF(__pyx_kp_u_);
+  __pyx_t_2 += 1;
+  __Pyx_GIVEREF(__pyx_kp_u_);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_kp_u_);
+  __pyx_t_4 = __Pyx_PyUnicode_From_int(__pyx_v_self->lineno, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_4);
+  __pyx_t_4 = 0;
+  __Pyx_INCREF(__pyx_kp_u__2);
+  __pyx_t_2 += 3;
+  __Pyx_GIVEREF(__pyx_kp_u__2);
+  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_kp_u__2);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_code); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
+  __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_t_5);
+  __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 5, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_r = __pyx_t_5;
+  __pyx_t_5 = 0;
+  goto __pyx_L0;
+
+  /* "dj_tracker/traceback.pyx":77
+ *         )
+ * 
+ *     def __repr__(self):             # <<<<<<<<<<<<<<
+ *         return f"{self.rel_path}:{self.lineno} - {self.code}"
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("dj_tracker.traceback.TracebackEntry.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "dj_tracker/traceback.pyx":80
+ *         return f"{self.rel_path}:{self.lineno} - {self.code}"
+ * 
  *     def __getattr__(self, name):             # <<<<<<<<<<<<<<
  *         if name == "hash_value":
  *             self.hash_value = hash((self.rel_path, self.lineno))
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_3__getattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_name); /*proto*/
-static PyObject *__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_3__getattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_name) {
+static PyObject *__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_5__getattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_name); /*proto*/
+static PyObject *__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_5__getattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_name) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__getattr__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_10dj_tracker_9traceback_14TracebackEntry_2__getattr__(((struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *)__pyx_v_self), ((PyObject *)__pyx_v_name));
+  __pyx_r = __pyx_pf_10dj_tracker_9traceback_14TracebackEntry_4__getattr__(((struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *)__pyx_v_self), ((PyObject *)__pyx_v_name));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_2__getattr__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self, PyObject *__pyx_v_name) {
+static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_4__getattr__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self, PyObject *__pyx_v_name) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_hash_t __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getattr__", 0);
 
-  /* "dj_tracker/traceback.pyx":78
+  /* "dj_tracker/traceback.pyx":81
  * 
  *     def __getattr__(self, name):
  *         if name == "hash_value":             # <<<<<<<<<<<<<<
  *             self.hash_value = hash((self.rel_path, self.lineno))
  *             return self.hash_value
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_name, __pyx_n_u_hash_value, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_name, __pyx_n_u_hash_value, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 81, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "dj_tracker/traceback.pyx":79
+    /* "dj_tracker/traceback.pyx":82
  *     def __getattr__(self, name):
  *         if name == "hash_value":
  *             self.hash_value = hash((self.rel_path, self.lineno))             # <<<<<<<<<<<<<<
  *             return self.hash_value
  * 
  */
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->lineno); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->lineno); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 79, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_self->rel_path);
     __Pyx_GIVEREF(__pyx_v_self->rel_path);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_self->rel_path);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
     __pyx_t_2 = 0;
-    __pyx_t_4 = PyObject_Hash(__pyx_t_3); if (unlikely(__pyx_t_4 == ((Py_hash_t)-1))) __PYX_ERR(0, 79, __pyx_L1_error)
+    __pyx_t_4 = PyObject_Hash(__pyx_t_3); if (unlikely(__pyx_t_4 == ((Py_hash_t)-1))) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_self->hash_value = __pyx_t_4;
 
-    /* "dj_tracker/traceback.pyx":80
+    /* "dj_tracker/traceback.pyx":83
  *         if name == "hash_value":
  *             self.hash_value = hash((self.rel_path, self.lineno))
  *             return self.hash_value             # <<<<<<<<<<<<<<
  * 
  *         raise AttributeError(name)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->hash_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 80, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_self->hash_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 83, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "dj_tracker/traceback.pyx":78
+    /* "dj_tracker/traceback.pyx":81
  * 
  *     def __getattr__(self, name):
  *         if name == "hash_value":             # <<<<<<<<<<<<<<
  *             self.hash_value = hash((self.rel_path, self.lineno))
  *             return self.hash_value
  */
   }
 
-  /* "dj_tracker/traceback.pyx":82
+  /* "dj_tracker/traceback.pyx":85
  *             return self.hash_value
  * 
  *         raise AttributeError(name)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_AttributeError, __pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_AttributeError, __pyx_v_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_3, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 82, __pyx_L1_error)
+  __PYX_ERR(0, 85, __pyx_L1_error)
 
-  /* "dj_tracker/traceback.pyx":77
- *         )
+  /* "dj_tracker/traceback.pyx":80
+ *         return f"{self.rel_path}:{self.lineno} - {self.code}"
  * 
  *     def __getattr__(self, name):             # <<<<<<<<<<<<<<
  *         if name == "hash_value":
  *             self.hash_value = hash((self.rel_path, self.lineno))
  */
 
   /* function exit code */
@@ -3960,23 +4121,23 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_5__reduce_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_7__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_10dj_tracker_9traceback_14TracebackEntry_5__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_5__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_5__reduce_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_10dj_tracker_9traceback_14TracebackEntry_7__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_7__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_7__reduce_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
@@ -3985,22 +4146,22 @@
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  __pyx_r = __pyx_pf_10dj_tracker_9traceback_14TracebackEntry_4__reduce_cython__(((struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *)__pyx_v_self));
+  __pyx_r = __pyx_pf_10dj_tracker_9traceback_14TracebackEntry_6__reduce_cython__(((struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_4__reduce_cython__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self) {
+static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_6__reduce_cython__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -4257,23 +4418,23 @@
  *     else:
  *         return __pyx_unpickle_TracebackEntry, (type(self), 0x6d8739c, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_TracebackEntry__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_7__setstate_cython__(PyObject *__pyx_v_self, 
+static PyObject *__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_9__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_10dj_tracker_9traceback_14TracebackEntry_7__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_7__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_7__setstate_cython__(PyObject *__pyx_v_self, 
+static PyMethodDef __pyx_mdef_10dj_tracker_9traceback_14TracebackEntry_9__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_9__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_9__setstate_cython__(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v___pyx_state = 0;
@@ -4320,22 +4481,22 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 16, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("dj_tracker.traceback.TracebackEntry.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_10dj_tracker_9traceback_14TracebackEntry_6__setstate_cython__(((struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *)__pyx_v_self), __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_10dj_tracker_9traceback_14TracebackEntry_8__setstate_cython__(((struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_6__setstate_cython__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_10dj_tracker_9traceback_14TracebackEntry_8__setstate_cython__(struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -4367,15 +4528,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_10dj_tracker_9traceback_13get_file_info_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "dj_tracker/traceback.pyx":95
+/* "dj_tracker/traceback.pyx":98
  *     except KeyError:
  *         try:
  *             module_dir = next(path for path in sys.path if filename.startswith(path))             # <<<<<<<<<<<<<<
  *         except StopIteration:
  *             # The following logic is inspired from:
  */
 
@@ -4387,26 +4548,26 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr *)__pyx_tp_new_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr(__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 95, __pyx_L1_error)
+    __PYX_ERR(0, 98, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info *) __pyx_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_outer_scope);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_outer_scope);
   __pyx_cur_scope->__pyx_genexpr_arg_0 = __pyx_genexpr_arg_0;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10dj_tracker_9traceback_13get_file_info_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_get_file_info_locals_genexpr, __pyx_n_s_dj_tracker_traceback); if (unlikely(!gen)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10dj_tracker_9traceback_13get_file_info_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_get_file_info_locals_genexpr, __pyx_n_s_dj_tracker_traceback); if (unlikely(!gen)) __PYX_ERR(0, 98, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4436,65 +4597,65 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L7_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 95, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 95, __pyx_L1_error) }
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 98, __pyx_L1_error) }
   if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) {
     __pyx_t_1 = __pyx_cur_scope->__pyx_genexpr_arg_0; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_genexpr_arg_0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_genexpr_arg_0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 95, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 98, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 98, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 95, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 98, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 98, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 95, __pyx_L1_error)
+          else __PYX_ERR(0, 98, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_path);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_path, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     __pyx_t_4 = 0;
-    if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_filename)) { __Pyx_RaiseClosureNameError("filename"); __PYX_ERR(0, 95, __pyx_L1_error) }
+    if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_filename)) { __Pyx_RaiseClosureNameError("filename"); __PYX_ERR(0, 98, __pyx_L1_error) }
     if (unlikely(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_filename == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "startswith");
-      __PYX_ERR(0, 95, __pyx_L1_error)
+      __PYX_ERR(0, 98, __pyx_L1_error)
     }
-    __pyx_t_5 = __Pyx_PyUnicode_Tailmatch(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_filename, __pyx_cur_scope->__pyx_v_path, 0, PY_SSIZE_T_MAX, -1); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 95, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyUnicode_Tailmatch(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_filename, __pyx_cur_scope->__pyx_v_path, 0, PY_SSIZE_T_MAX, -1); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 98, __pyx_L1_error)
     if (__pyx_t_5) {
       __Pyx_INCREF(__pyx_cur_scope->__pyx_v_path);
       __pyx_r = __pyx_cur_scope->__pyx_v_path;
       __Pyx_XGIVEREF(__pyx_t_1);
       __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
       __pyx_cur_scope->__pyx_t_1 = __pyx_t_2;
       __pyx_cur_scope->__pyx_t_2 = __pyx_t_3;
@@ -4506,15 +4667,15 @@
       return __pyx_r;
       __pyx_L7_resume_from_yield:;
       __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
       __pyx_cur_scope->__pyx_t_0 = 0;
       __Pyx_XGOTREF(__pyx_t_1);
       __pyx_t_2 = __pyx_cur_scope->__pyx_t_1;
       __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
-      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 95, __pyx_L1_error)
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 98, __pyx_L1_error)
     }
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
@@ -4532,15 +4693,15 @@
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_10dj_tracker_9traceback_13get_file_info_5generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "dj_tracker/traceback.pyx":113
+/* "dj_tracker/traceback.pyx":116
  * 
  *         rel_path = os.path.relpath(filename, module_dir)
  *         ignore = any(module in filename for module in IGNORED_MODULES)             # <<<<<<<<<<<<<<
  *         cache[filename] = file_info = rel_path, ignore
  *         return file_info
  */
 
@@ -4552,26 +4713,26 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr *)__pyx_tp_new_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr(__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 113, __pyx_L1_error)
+    __PYX_ERR(0, 116, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info *) __pyx_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_outer_scope);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_outer_scope);
   __pyx_cur_scope->__pyx_genexpr_arg_0 = __pyx_genexpr_arg_0;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10dj_tracker_9traceback_13get_file_info_5generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_get_file_info_locals_genexpr, __pyx_n_s_dj_tracker_traceback); if (unlikely(!gen)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10dj_tracker_9traceback_13get_file_info_5generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_get_file_info_locals_genexpr, __pyx_n_s_dj_tracker_traceback); if (unlikely(!gen)) __PYX_ERR(0, 116, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4600,65 +4761,65 @@
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 113, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 113, __pyx_L1_error) }
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 116, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 116, __pyx_L1_error) }
   if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) {
     __pyx_t_1 = __pyx_cur_scope->__pyx_genexpr_arg_0; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_genexpr_arg_0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_genexpr_arg_0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 113, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 116, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 113, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 116, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 113, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 116, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 113, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 116, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 113, __pyx_L1_error)
+          else __PYX_ERR(0, 116, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_module);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_module, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     __pyx_t_4 = 0;
-    if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_filename)) { __Pyx_RaiseClosureNameError("filename"); __PYX_ERR(0, 113, __pyx_L1_error) }
+    if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_filename)) { __Pyx_RaiseClosureNameError("filename"); __PYX_ERR(0, 116, __pyx_L1_error) }
     if (unlikely(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_filename == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-      __PYX_ERR(0, 113, __pyx_L1_error)
+      __PYX_ERR(0, 116, __pyx_L1_error)
     }
-    __pyx_t_5 = (__Pyx_PyUnicode_ContainsTF(__pyx_cur_scope->__pyx_v_module, __pyx_cur_scope->__pyx_outer_scope->__pyx_v_filename, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 113, __pyx_L1_error)
+    __pyx_t_5 = (__Pyx_PyUnicode_ContainsTF(__pyx_cur_scope->__pyx_v_module, __pyx_cur_scope->__pyx_outer_scope->__pyx_v_filename, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 116, __pyx_L1_error)
     if (__pyx_t_5) {
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(Py_True);
       __pyx_r = Py_True;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       goto __pyx_L0;
     }
@@ -4687,25 +4848,25 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dj_tracker/traceback.pyx":85
+/* "dj_tracker/traceback.pyx":88
  * 
  * 
  * cdef tuple get_file_info(str filename, PyFrameObject *frame, dict cache = {}):             # <<<<<<<<<<<<<<
  *     """Retrieves the relative path for a filename and indicates if it should be ignored."""
  *     cdef:
  */
 
 static PyObject *__pyx_f_10dj_tracker_9traceback_get_file_info(PyObject *__pyx_v_filename, PyFrameObject *__pyx_v_frame, struct __pyx_opt_args_10dj_tracker_9traceback_get_file_info *__pyx_optional_args) {
   struct __pyx_obj_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info *__pyx_cur_scope;
-  PyObject *__pyx_v_cache = __pyx_k_;
+  PyObject *__pyx_v_cache = __pyx_k__3;
   PyObject *__pyx_v_rel_path = 0;
   int __pyx_v_ignore;
   PyObject *__pyx_v_module_dir = NULL;
   PyObject *__pyx_v_f_globals;
   PyObject *__pyx_v_module = NULL;
   PyObject *__pyx_v_file_info = NULL;
   PyObject *__pyx_gb_10dj_tracker_9traceback_13get_file_info_2generator = 0;
@@ -4738,28 +4899,28 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_file_info", 0);
   __pyx_cur_scope = (struct __pyx_obj_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info *)__pyx_tp_new_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info(__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 85, __pyx_L1_error)
+    __PYX_ERR(0, 88, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_cache = __pyx_optional_args->cache;
     }
   }
   __pyx_cur_scope->__pyx_v_filename = __pyx_v_filename;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_filename);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_filename);
 
-  /* "dj_tracker/traceback.pyx":91
+  /* "dj_tracker/traceback.pyx":94
  *         bint ignore
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         return cache[filename]
  *     except KeyError:
  */
   {
@@ -4767,60 +4928,60 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "dj_tracker/traceback.pyx":92
+      /* "dj_tracker/traceback.pyx":95
  * 
  *     try:
  *         return cache[filename]             # <<<<<<<<<<<<<<
  *     except KeyError:
  *         try:
  */
       __Pyx_XDECREF(__pyx_r);
       if (unlikely(__pyx_v_cache == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 92, __pyx_L3_error)
+        __PYX_ERR(0, 95, __pyx_L3_error)
       }
-      __pyx_t_4 = __Pyx_PyDict_GetItem(__pyx_v_cache, __pyx_cur_scope->__pyx_v_filename); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L3_error)
+      __pyx_t_4 = __Pyx_PyDict_GetItem(__pyx_v_cache, __pyx_cur_scope->__pyx_v_filename); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (!(likely(PyTuple_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_t_4))) __PYX_ERR(0, 92, __pyx_L3_error)
+      if (!(likely(PyTuple_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_t_4))) __PYX_ERR(0, 95, __pyx_L3_error)
       __pyx_r = ((PyObject*)__pyx_t_4);
       __pyx_t_4 = 0;
       goto __pyx_L7_try_return;
 
-      /* "dj_tracker/traceback.pyx":91
+      /* "dj_tracker/traceback.pyx":94
  *         bint ignore
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         return cache[filename]
  *     except KeyError:
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "dj_tracker/traceback.pyx":93
+    /* "dj_tracker/traceback.pyx":96
  *     try:
  *         return cache[filename]
  *     except KeyError:             # <<<<<<<<<<<<<<
  *         try:
  *             module_dir = next(path for path in sys.path if filename.startswith(path))
  */
     __pyx_t_5 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
     if (__pyx_t_5) {
       __Pyx_AddTraceback("dj_tracker.traceback.get_file_info", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 93, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 96, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "dj_tracker/traceback.pyx":94
+      /* "dj_tracker/traceback.pyx":97
  *         return cache[filename]
  *     except KeyError:
  *         try:             # <<<<<<<<<<<<<<
  *             module_dir = next(path for path in sys.path if filename.startswith(path))
  *         except StopIteration:
  */
       {
@@ -4828,36 +4989,36 @@
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_8, &__pyx_t_9, &__pyx_t_10);
         __Pyx_XGOTREF(__pyx_t_8);
         __Pyx_XGOTREF(__pyx_t_9);
         __Pyx_XGOTREF(__pyx_t_10);
         /*try:*/ {
 
-          /* "dj_tracker/traceback.pyx":95
+          /* "dj_tracker/traceback.pyx":98
  *     except KeyError:
  *         try:
  *             module_dir = next(path for path in sys.path if filename.startswith(path))             # <<<<<<<<<<<<<<
  *         except StopIteration:
  *             # The following logic is inspired from:
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_sys); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 95, __pyx_L11_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_sys); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 98, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_11);
-          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_path); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 95, __pyx_L11_error)
+          __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_path); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 98, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-          __pyx_t_11 = __pyx_pf_10dj_tracker_9traceback_13get_file_info_genexpr(((PyObject*)__pyx_cur_scope), __pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 95, __pyx_L11_error)
+          __pyx_t_11 = __pyx_pf_10dj_tracker_9traceback_13get_file_info_genexpr(((PyObject*)__pyx_cur_scope), __pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 98, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-          __pyx_t_12 = __Pyx_PyIter_Next(__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 95, __pyx_L11_error)
+          __pyx_t_12 = __Pyx_PyIter_Next(__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 98, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
           __pyx_v_module_dir = __pyx_t_12;
           __pyx_t_12 = 0;
 
-          /* "dj_tracker/traceback.pyx":94
+          /* "dj_tracker/traceback.pyx":97
  *         return cache[filename]
  *     except KeyError:
  *         try:             # <<<<<<<<<<<<<<
  *             module_dir = next(path for path in sys.path if filename.startswith(path))
  *         except StopIteration:
  */
         }
@@ -4865,84 +5026,84 @@
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         goto __pyx_L18_try_end;
         __pyx_L11_error:;
         __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
 
-        /* "dj_tracker/traceback.pyx":96
+        /* "dj_tracker/traceback.pyx":99
  *         try:
  *             module_dir = next(path for path in sys.path if filename.startswith(path))
  *         except StopIteration:             # <<<<<<<<<<<<<<
  *             # The following logic is inspired from:
  *             # https://github.com/scoutapp/scout_apm_python/blob/master/src/scout_apm/core/backtrace.py#L29
  */
         __pyx_t_5 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_StopIteration);
         if (__pyx_t_5) {
           __Pyx_AddTraceback("dj_tracker.traceback.get_file_info", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_12, &__pyx_t_11, &__pyx_t_13) < 0) __PYX_ERR(0, 96, __pyx_L13_except_error)
+          if (__Pyx_GetException(&__pyx_t_12, &__pyx_t_11, &__pyx_t_13) < 0) __PYX_ERR(0, 99, __pyx_L13_except_error)
           __Pyx_GOTREF(__pyx_t_12);
           __Pyx_GOTREF(__pyx_t_11);
           __Pyx_GOTREF(__pyx_t_13);
 
-          /* "dj_tracker/traceback.pyx":99
+          /* "dj_tracker/traceback.pyx":102
  *             # The following logic is inspired from:
  *             # https://github.com/scoutapp/scout_apm_python/blob/master/src/scout_apm/core/backtrace.py#L29
  *             f_globals = PyFrame_GetGlobals(frame)             # <<<<<<<<<<<<<<
  *             module = (<dict>f_globals).get("__name__", "")
  *             Py_DECREF(f_globals)
  */
           __pyx_v_f_globals = PyFrame_GetGlobals(__pyx_v_frame);
 
-          /* "dj_tracker/traceback.pyx":100
+          /* "dj_tracker/traceback.pyx":103
  *             # https://github.com/scoutapp/scout_apm_python/blob/master/src/scout_apm/core/backtrace.py#L29
  *             f_globals = PyFrame_GetGlobals(frame)
  *             module = (<dict>f_globals).get("__name__", "")             # <<<<<<<<<<<<<<
  *             Py_DECREF(f_globals)
  * 
  */
           if (unlikely(((PyObject *)__pyx_v_f_globals) == Py_None)) {
             PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "get");
-            __PYX_ERR(0, 100, __pyx_L13_except_error)
+            __PYX_ERR(0, 103, __pyx_L13_except_error)
           }
-          __pyx_t_14 = __Pyx_PyDict_GetItemDefault(((PyObject*)__pyx_v_f_globals), __pyx_n_u_name_2, __pyx_kp_u__2); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 100, __pyx_L13_except_error)
+          __pyx_t_14 = __Pyx_PyDict_GetItemDefault(((PyObject*)__pyx_v_f_globals), __pyx_n_u_name_2, __pyx_kp_u__4); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 103, __pyx_L13_except_error)
           __Pyx_GOTREF(__pyx_t_14);
           __pyx_v_module = __pyx_t_14;
           __pyx_t_14 = 0;
 
-          /* "dj_tracker/traceback.pyx":101
+          /* "dj_tracker/traceback.pyx":104
  *             f_globals = PyFrame_GetGlobals(frame)
  *             module = (<dict>f_globals).get("__name__", "")
  *             Py_DECREF(f_globals)             # <<<<<<<<<<<<<<
  * 
  *             if (root_module := sys.modules.get(module.split(".", 1)[0])) is not None:
  */
           Py_DECREF(__pyx_v_f_globals);
 
-          /* "dj_tracker/traceback.pyx":103
+          /* "dj_tracker/traceback.pyx":106
  *             Py_DECREF(f_globals)
  * 
  *             if (root_module := sys.modules.get(module.split(".", 1)[0])) is not None:             # <<<<<<<<<<<<<<
  *                 if module_path := root_module.__file__:
  *                     module_dir = module_path.rsplit(os.sep, 2)[0]
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_sys); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 103, __pyx_L13_except_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_sys); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 106, __pyx_L13_except_error)
           __Pyx_GOTREF(__pyx_t_15);
-          __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_modules); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 103, __pyx_L13_except_error)
+          __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_modules); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 106, __pyx_L13_except_error)
           __Pyx_GOTREF(__pyx_t_16);
           __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-          __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_get); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 103, __pyx_L13_except_error)
+          __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_get); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 106, __pyx_L13_except_error)
           __Pyx_GOTREF(__pyx_t_15);
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-          __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_v_module, __pyx_n_s_split); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 103, __pyx_L13_except_error)
+          __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_v_module, __pyx_n_s_split); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 106, __pyx_L13_except_error)
           __Pyx_GOTREF(__pyx_t_16);
-          __pyx_t_17 = __Pyx_PyObject_Call(__pyx_t_16, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 103, __pyx_L13_except_error)
+          __pyx_t_17 = __Pyx_PyObject_Call(__pyx_t_16, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 106, __pyx_L13_except_error)
           __Pyx_GOTREF(__pyx_t_17);
           __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-          __pyx_t_16 = __Pyx_GetItemInt(__pyx_t_17, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 103, __pyx_L13_except_error)
+          __pyx_t_16 = __Pyx_GetItemInt(__pyx_t_17, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 106, __pyx_L13_except_error)
           __Pyx_GOTREF(__pyx_t_16);
           __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
           __pyx_t_17 = NULL;
           __pyx_t_5 = 0;
           if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_15))) {
             __pyx_t_17 = PyMethod_GET_SELF(__pyx_t_15);
             if (likely(__pyx_t_17)) {
@@ -4954,51 +5115,51 @@
             }
           }
           {
             PyObject *__pyx_callargs[2] = {__pyx_t_17, __pyx_t_16};
             __pyx_t_14 = __Pyx_PyObject_FastCall(__pyx_t_15, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
             __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
             __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-            if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 103, __pyx_L13_except_error)
+            if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 106, __pyx_L13_except_error)
             __Pyx_GOTREF(__pyx_t_14);
             __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
           }
           __pyx_v_root_module = __pyx_t_14;
           __Pyx_INCREF(__pyx_t_14);
           __pyx_t_18 = (__pyx_t_14 != Py_None);
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
           if (__pyx_t_18) {
 
-            /* "dj_tracker/traceback.pyx":104
+            /* "dj_tracker/traceback.pyx":107
  * 
  *             if (root_module := sys.modules.get(module.split(".", 1)[0])) is not None:
  *                 if module_path := root_module.__file__:             # <<<<<<<<<<<<<<
  *                     module_dir = module_path.rsplit(os.sep, 2)[0]
  *                 elif (module_path := root_module.__path__) and isinstance(module_path, (list, tuple)):
  */
-            __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_v_root_module, __pyx_n_s_file); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 104, __pyx_L13_except_error)
+            __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_v_root_module, __pyx_n_s_file); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 107, __pyx_L13_except_error)
             __Pyx_GOTREF(__pyx_t_14);
             __pyx_v_module_path = __pyx_t_14;
             __Pyx_INCREF(__pyx_t_14);
-            __pyx_t_18 = __Pyx_PyObject_IsTrue(__pyx_t_14); if (unlikely((__pyx_t_18 < 0))) __PYX_ERR(0, 104, __pyx_L13_except_error)
+            __pyx_t_18 = __Pyx_PyObject_IsTrue(__pyx_t_14); if (unlikely((__pyx_t_18 < 0))) __PYX_ERR(0, 107, __pyx_L13_except_error)
             __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
             if (__pyx_t_18) {
 
-              /* "dj_tracker/traceback.pyx":105
+              /* "dj_tracker/traceback.pyx":108
  *             if (root_module := sys.modules.get(module.split(".", 1)[0])) is not None:
  *                 if module_path := root_module.__file__:
  *                     module_dir = module_path.rsplit(os.sep, 2)[0]             # <<<<<<<<<<<<<<
  *                 elif (module_path := root_module.__path__) and isinstance(module_path, (list, tuple)):
  *                     module_dir = module_path[0].rsplit(os.sep, 1)[0]
  */
-              __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_v_module_path, __pyx_n_s_rsplit); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 105, __pyx_L13_except_error)
+              __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_v_module_path, __pyx_n_s_rsplit); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 108, __pyx_L13_except_error)
               __Pyx_GOTREF(__pyx_t_15);
-              __Pyx_GetModuleGlobalName(__pyx_t_16, __pyx_n_s_os); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 105, __pyx_L13_except_error)
+              __Pyx_GetModuleGlobalName(__pyx_t_16, __pyx_n_s_os); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 108, __pyx_L13_except_error)
               __Pyx_GOTREF(__pyx_t_16);
-              __pyx_t_17 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_sep); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 105, __pyx_L13_except_error)
+              __pyx_t_17 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_sep); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 108, __pyx_L13_except_error)
               __Pyx_GOTREF(__pyx_t_17);
               __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
               __pyx_t_16 = NULL;
               __pyx_t_5 = 0;
               if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_15))) {
                 __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_15);
                 if (likely(__pyx_t_16)) {
@@ -5010,46 +5171,46 @@
                 }
               }
               {
                 PyObject *__pyx_callargs[3] = {__pyx_t_16, __pyx_t_17, __pyx_int_2};
                 __pyx_t_14 = __Pyx_PyObject_FastCall(__pyx_t_15, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
                 __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
                 __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-                if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 105, __pyx_L13_except_error)
+                if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 108, __pyx_L13_except_error)
                 __Pyx_GOTREF(__pyx_t_14);
                 __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
               }
-              __pyx_t_15 = __Pyx_GetItemInt(__pyx_t_14, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 105, __pyx_L13_except_error)
+              __pyx_t_15 = __Pyx_GetItemInt(__pyx_t_14, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 108, __pyx_L13_except_error)
               __Pyx_GOTREF(__pyx_t_15);
               __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
               __Pyx_XDECREF_SET(__pyx_v_module_dir, __pyx_t_15);
               __pyx_t_15 = 0;
 
-              /* "dj_tracker/traceback.pyx":104
+              /* "dj_tracker/traceback.pyx":107
  * 
  *             if (root_module := sys.modules.get(module.split(".", 1)[0])) is not None:
  *                 if module_path := root_module.__file__:             # <<<<<<<<<<<<<<
  *                     module_dir = module_path.rsplit(os.sep, 2)[0]
  *                 elif (module_path := root_module.__path__) and isinstance(module_path, (list, tuple)):
  */
               goto __pyx_L22;
             }
 
-            /* "dj_tracker/traceback.pyx":106
+            /* "dj_tracker/traceback.pyx":109
  *                 if module_path := root_module.__file__:
  *                     module_dir = module_path.rsplit(os.sep, 2)[0]
  *                 elif (module_path := root_module.__path__) and isinstance(module_path, (list, tuple)):             # <<<<<<<<<<<<<<
  *                     module_dir = module_path[0].rsplit(os.sep, 1)[0]
  *             else:
  */
-            __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_v_root_module, __pyx_n_s_path_2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 106, __pyx_L13_except_error)
+            __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_v_root_module, __pyx_n_s_path_2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 109, __pyx_L13_except_error)
             __Pyx_GOTREF(__pyx_t_15);
             __Pyx_DECREF_SET(__pyx_v_module_path, __pyx_t_15);
             __Pyx_INCREF(__pyx_t_15);
-            __pyx_t_19 = __Pyx_PyObject_IsTrue(__pyx_t_15); if (unlikely((__pyx_t_19 < 0))) __PYX_ERR(0, 106, __pyx_L13_except_error)
+            __pyx_t_19 = __Pyx_PyObject_IsTrue(__pyx_t_15); if (unlikely((__pyx_t_19 < 0))) __PYX_ERR(0, 109, __pyx_L13_except_error)
             __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
             if (__pyx_t_19) {
             } else {
               __pyx_t_18 = __pyx_t_19;
               goto __pyx_L23_bool_binop_done;
             }
             __pyx_t_20 = PyList_Check(__pyx_v_module_path); 
@@ -5061,29 +5222,29 @@
             __pyx_t_20 = PyTuple_Check(__pyx_v_module_path); 
             __pyx_t_19 = __pyx_t_20;
             __pyx_L25_bool_binop_done:;
             __pyx_t_18 = __pyx_t_19;
             __pyx_L23_bool_binop_done:;
             if (__pyx_t_18) {
 
-              /* "dj_tracker/traceback.pyx":107
+              /* "dj_tracker/traceback.pyx":110
  *                     module_dir = module_path.rsplit(os.sep, 2)[0]
  *                 elif (module_path := root_module.__path__) and isinstance(module_path, (list, tuple)):
  *                     module_dir = module_path[0].rsplit(os.sep, 1)[0]             # <<<<<<<<<<<<<<
  *             else:
  *                 # Fall back to current working directory.
  */
-              __pyx_t_14 = __Pyx_GetItemInt(__pyx_v_module_path, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 107, __pyx_L13_except_error)
+              __pyx_t_14 = __Pyx_GetItemInt(__pyx_v_module_path, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 110, __pyx_L13_except_error)
               __Pyx_GOTREF(__pyx_t_14);
-              __pyx_t_17 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_rsplit); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 107, __pyx_L13_except_error)
+              __pyx_t_17 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_rsplit); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 110, __pyx_L13_except_error)
               __Pyx_GOTREF(__pyx_t_17);
               __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
-              __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_os); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 107, __pyx_L13_except_error)
+              __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_os); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 110, __pyx_L13_except_error)
               __Pyx_GOTREF(__pyx_t_14);
-              __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_sep); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 107, __pyx_L13_except_error)
+              __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_sep); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 110, __pyx_L13_except_error)
               __Pyx_GOTREF(__pyx_t_16);
               __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
               __pyx_t_14 = NULL;
               __pyx_t_5 = 0;
               if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_17))) {
                 __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_17);
                 if (likely(__pyx_t_14)) {
@@ -5095,55 +5256,55 @@
                 }
               }
               {
                 PyObject *__pyx_callargs[3] = {__pyx_t_14, __pyx_t_16, __pyx_int_1};
                 __pyx_t_15 = __Pyx_PyObject_FastCall(__pyx_t_17, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
                 __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
                 __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
-                if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 107, __pyx_L13_except_error)
+                if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 110, __pyx_L13_except_error)
                 __Pyx_GOTREF(__pyx_t_15);
                 __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
               }
-              __pyx_t_17 = __Pyx_GetItemInt(__pyx_t_15, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 107, __pyx_L13_except_error)
+              __pyx_t_17 = __Pyx_GetItemInt(__pyx_t_15, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 110, __pyx_L13_except_error)
               __Pyx_GOTREF(__pyx_t_17);
               __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
               __Pyx_XDECREF_SET(__pyx_v_module_dir, __pyx_t_17);
               __pyx_t_17 = 0;
 
-              /* "dj_tracker/traceback.pyx":106
+              /* "dj_tracker/traceback.pyx":109
  *                 if module_path := root_module.__file__:
  *                     module_dir = module_path.rsplit(os.sep, 2)[0]
  *                 elif (module_path := root_module.__path__) and isinstance(module_path, (list, tuple)):             # <<<<<<<<<<<<<<
  *                     module_dir = module_path[0].rsplit(os.sep, 1)[0]
  *             else:
  */
             }
             __pyx_L22:;
 
-            /* "dj_tracker/traceback.pyx":103
+            /* "dj_tracker/traceback.pyx":106
  *             Py_DECREF(f_globals)
  * 
  *             if (root_module := sys.modules.get(module.split(".", 1)[0])) is not None:             # <<<<<<<<<<<<<<
  *                 if module_path := root_module.__file__:
  *                     module_dir = module_path.rsplit(os.sep, 2)[0]
  */
             goto __pyx_L21;
           }
 
-          /* "dj_tracker/traceback.pyx":110
+          /* "dj_tracker/traceback.pyx":113
  *             else:
  *                 # Fall back to current working directory.
  *                 module_dir = os.getcwd()             # <<<<<<<<<<<<<<
  * 
  *         rel_path = os.path.relpath(filename, module_dir)
  */
           /*else*/ {
-            __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_os); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 110, __pyx_L13_except_error)
+            __Pyx_GetModuleGlobalName(__pyx_t_15, __pyx_n_s_os); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 113, __pyx_L13_except_error)
             __Pyx_GOTREF(__pyx_t_15);
-            __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_getcwd); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 110, __pyx_L13_except_error)
+            __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_getcwd); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 113, __pyx_L13_except_error)
             __Pyx_GOTREF(__pyx_t_16);
             __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
             __pyx_t_15 = NULL;
             __pyx_t_5 = 0;
             if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_16))) {
               __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_16);
               if (likely(__pyx_t_15)) {
@@ -5154,15 +5315,15 @@
                 __pyx_t_5 = 1;
               }
             }
             {
               PyObject *__pyx_callargs[1] = {__pyx_t_15, };
               __pyx_t_17 = __Pyx_PyObject_FastCall(__pyx_t_16, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
               __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-              if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 110, __pyx_L13_except_error)
+              if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 113, __pyx_L13_except_error)
               __Pyx_GOTREF(__pyx_t_17);
               __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
             }
             __Pyx_XDECREF_SET(__pyx_v_module_dir, __pyx_t_17);
             __pyx_t_17 = 0;
           }
           __pyx_L21:;
@@ -5170,15 +5331,15 @@
           __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
           __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
           goto __pyx_L12_exception_handled;
         }
         goto __pyx_L13_except_error;
         __pyx_L13_except_error:;
 
-        /* "dj_tracker/traceback.pyx":94
+        /* "dj_tracker/traceback.pyx":97
  *         return cache[filename]
  *     except KeyError:
  *         try:             # <<<<<<<<<<<<<<
  *             module_dir = next(path for path in sys.path if filename.startswith(path))
  *         except StopIteration:
  */
         __Pyx_XGIVEREF(__pyx_t_8);
@@ -5190,30 +5351,30 @@
         __Pyx_XGIVEREF(__pyx_t_8);
         __Pyx_XGIVEREF(__pyx_t_9);
         __Pyx_XGIVEREF(__pyx_t_10);
         __Pyx_ExceptionReset(__pyx_t_8, __pyx_t_9, __pyx_t_10);
         __pyx_L18_try_end:;
       }
 
-      /* "dj_tracker/traceback.pyx":112
+      /* "dj_tracker/traceback.pyx":115
  *                 module_dir = os.getcwd()
  * 
  *         rel_path = os.path.relpath(filename, module_dir)             # <<<<<<<<<<<<<<
  *         ignore = any(module in filename for module in IGNORED_MODULES)
  *         cache[filename] = file_info = rel_path, ignore
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_os); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 112, __pyx_L5_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_os); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 115, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_11);
-      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_path); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 112, __pyx_L5_except_error)
+      __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_path); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 115, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_relpath); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 112, __pyx_L5_except_error)
+      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_relpath); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 115, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-      if (unlikely(!__pyx_v_module_dir)) { __Pyx_RaiseUnboundLocalError("module_dir"); __PYX_ERR(0, 112, __pyx_L5_except_error) }
+      if (unlikely(!__pyx_v_module_dir)) { __Pyx_RaiseUnboundLocalError("module_dir"); __PYX_ERR(0, 115, __pyx_L5_except_error) }
       __pyx_t_12 = NULL;
       __pyx_t_5 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
         __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
         if (likely(__pyx_t_12)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
           __Pyx_INCREF(__pyx_t_12);
@@ -5222,68 +5383,68 @@
           __pyx_t_5 = 1;
         }
       }
       {
         PyObject *__pyx_callargs[3] = {__pyx_t_12, __pyx_cur_scope->__pyx_v_filename, __pyx_v_module_dir};
         __pyx_t_13 = __Pyx_PyObject_FastCall(__pyx_t_11, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-        if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 112, __pyx_L5_except_error)
+        if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 115, __pyx_L5_except_error)
         __Pyx_GOTREF(__pyx_t_13);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       }
-      if (!(likely(PyUnicode_CheckExact(__pyx_t_13))||((__pyx_t_13) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_13))) __PYX_ERR(0, 112, __pyx_L5_except_error)
+      if (!(likely(PyUnicode_CheckExact(__pyx_t_13))||((__pyx_t_13) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_13))) __PYX_ERR(0, 115, __pyx_L5_except_error)
       __pyx_v_rel_path = ((PyObject*)__pyx_t_13);
       __pyx_t_13 = 0;
 
-      /* "dj_tracker/traceback.pyx":113
+      /* "dj_tracker/traceback.pyx":116
  * 
  *         rel_path = os.path.relpath(filename, module_dir)
  *         ignore = any(module in filename for module in IGNORED_MODULES)             # <<<<<<<<<<<<<<
  *         cache[filename] = file_info = rel_path, ignore
  *         return file_info
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_IGNORED_MODULES); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 113, __pyx_L5_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_13, __pyx_n_s_IGNORED_MODULES); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 116, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_13);
-      __pyx_t_11 = __pyx_pf_10dj_tracker_9traceback_13get_file_info_3genexpr(((PyObject*)__pyx_cur_scope), __pyx_t_13); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 113, __pyx_L5_except_error)
+      __pyx_t_11 = __pyx_pf_10dj_tracker_9traceback_13get_file_info_3genexpr(((PyObject*)__pyx_cur_scope), __pyx_t_13); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 116, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-      __pyx_t_13 = __Pyx_Generator_Next(__pyx_t_11); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 113, __pyx_L5_except_error)
+      __pyx_t_13 = __Pyx_Generator_Next(__pyx_t_11); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 116, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_13);
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      __pyx_t_18 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely((__pyx_t_18 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 113, __pyx_L5_except_error)
+      __pyx_t_18 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely((__pyx_t_18 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L5_except_error)
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
       __pyx_v_ignore = __pyx_t_18;
 
-      /* "dj_tracker/traceback.pyx":114
+      /* "dj_tracker/traceback.pyx":117
  *         rel_path = os.path.relpath(filename, module_dir)
  *         ignore = any(module in filename for module in IGNORED_MODULES)
  *         cache[filename] = file_info = rel_path, ignore             # <<<<<<<<<<<<<<
  *         return file_info
  * 
  */
-      __pyx_t_13 = __Pyx_PyBool_FromLong(__pyx_v_ignore); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 114, __pyx_L5_except_error)
+      __pyx_t_13 = __Pyx_PyBool_FromLong(__pyx_v_ignore); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 117, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_13);
-      __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 114, __pyx_L5_except_error)
+      __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 117, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_INCREF(__pyx_v_rel_path);
       __Pyx_GIVEREF(__pyx_v_rel_path);
       PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_v_rel_path);
       __Pyx_GIVEREF(__pyx_t_13);
       PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_13);
       __pyx_t_13 = 0;
       if (unlikely(__pyx_v_cache == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 114, __pyx_L5_except_error)
+        __PYX_ERR(0, 117, __pyx_L5_except_error)
       }
-      if (unlikely((PyDict_SetItem(__pyx_v_cache, __pyx_cur_scope->__pyx_v_filename, __pyx_t_11) < 0))) __PYX_ERR(0, 114, __pyx_L5_except_error)
+      if (unlikely((PyDict_SetItem(__pyx_v_cache, __pyx_cur_scope->__pyx_v_filename, __pyx_t_11) < 0))) __PYX_ERR(0, 117, __pyx_L5_except_error)
       __Pyx_INCREF(__pyx_t_11);
       __pyx_v_file_info = __pyx_t_11;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-      /* "dj_tracker/traceback.pyx":115
+      /* "dj_tracker/traceback.pyx":118
  *         ignore = any(module in filename for module in IGNORED_MODULES)
  *         cache[filename] = file_info = rel_path, ignore
  *         return file_info             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __Pyx_XDECREF(__pyx_r);
@@ -5293,15 +5454,15 @@
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       goto __pyx_L6_except_return;
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "dj_tracker/traceback.pyx":91
+    /* "dj_tracker/traceback.pyx":94
  *         bint ignore
  * 
  *     try:             # <<<<<<<<<<<<<<
  *         return cache[filename]
  *     except KeyError:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
@@ -5319,15 +5480,15 @@
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L0;
   }
 
-  /* "dj_tracker/traceback.pyx":85
+  /* "dj_tracker/traceback.pyx":88
  * 
  * 
  * cdef tuple get_file_info(str filename, PyFrameObject *frame, dict cache = {}):             # <<<<<<<<<<<<<<
  *     """Retrieves the relative path for a filename and indicates if it should be ignored."""
  *     cdef:
  */
 
@@ -5356,33 +5517,33 @@
   __Pyx_XDECREF(__pyx_gb_10dj_tracker_9traceback_13get_file_info_5generator1);
   __Pyx_DECREF((PyObject *)__pyx_cur_scope);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dj_tracker/traceback.pyx":118
+/* "dj_tracker/traceback.pyx":121
  * 
  * 
  * cdef inline TracebackEntry get_entry(             # <<<<<<<<<<<<<<
  *     str filename,
  *     object lineno,
  */
 
 static CYTHON_INLINE struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_f_10dj_tracker_9traceback_get_entry(PyObject *__pyx_v_filename, PyObject *__pyx_v_lineno, PyFrameObject *__pyx_v_frame, struct __pyx_opt_args_10dj_tracker_9traceback_get_entry *__pyx_optional_args) {
 
-  /* "dj_tracker/traceback.pyx":122
+  /* "dj_tracker/traceback.pyx":125
  *     object lineno,
  *     PyFrameObject *frame,
  *     PyCodeObject *code = NULL,             # <<<<<<<<<<<<<<
  *     LRUCache cache = LRUCache(maxsize=512)
  * ):
  */
   PyCodeObject *__pyx_v_code = ((PyCodeObject *)NULL);
-  struct __pyx_obj_10dj_tracker_11cache_utils_LRUCache *__pyx_v_cache = __pyx_k__5;
+  struct __pyx_obj_10dj_tracker_11cache_utils_LRUCache *__pyx_v_cache = __pyx_k__7;
   struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_v_entry = 0;
   PyObject *__pyx_v_cache_key = NULL;
   struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
@@ -5396,158 +5557,158 @@
       __pyx_v_code = __pyx_optional_args->code;
       if (__pyx_optional_args->__pyx_n > 1) {
         __pyx_v_cache = __pyx_optional_args->cache;
       }
     }
   }
 
-  /* "dj_tracker/traceback.pyx":126
+  /* "dj_tracker/traceback.pyx":129
  * ):
  *     cdef TracebackEntry entry
  *     cache_key = filename, lineno             # <<<<<<<<<<<<<<
  * 
  *     if (entry := cache.get(cache_key)) is None:
  */
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_filename);
   __Pyx_GIVEREF(__pyx_v_filename);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_filename);
   __Pyx_INCREF(__pyx_v_lineno);
   __Pyx_GIVEREF(__pyx_v_lineno);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_lineno);
   __pyx_v_cache_key = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "dj_tracker/traceback.pyx":128
+  /* "dj_tracker/traceback.pyx":131
  *     cache_key = filename, lineno
  * 
  *     if (entry := cache.get(cache_key)) is None:             # <<<<<<<<<<<<<<
  *         entry = TracebackEntry(
  *             filename,
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10dj_tracker_11cache_utils_LRUCache *)__pyx_v_cache->__pyx_vtab)->get(__pyx_v_cache, __pyx_v_cache_key, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10dj_tracker_11cache_utils_LRUCache *)__pyx_v_cache->__pyx_vtab)->get(__pyx_v_cache, __pyx_v_cache_key, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_10dj_tracker_9traceback_TracebackEntry))))) __PYX_ERR(0, 128, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_10dj_tracker_9traceback_TracebackEntry))))) __PYX_ERR(0, 131, __pyx_L1_error)
   __pyx_v_entry = ((struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *)__pyx_t_1);
   __Pyx_INCREF(__pyx_t_1);
   __pyx_t_2 = (__pyx_t_1 == Py_None);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "dj_tracker/traceback.pyx":129
+    /* "dj_tracker/traceback.pyx":132
  * 
  *     if (entry := cache.get(cache_key)) is None:
  *         entry = TracebackEntry(             # <<<<<<<<<<<<<<
  *             filename,
  *             *get_file_info(filename, frame),
  */
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_filename);
     __Pyx_GIVEREF(__pyx_v_filename);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_filename);
 
-    /* "dj_tracker/traceback.pyx":131
+    /* "dj_tracker/traceback.pyx":134
  *         entry = TracebackEntry(
  *             filename,
  *             *get_file_info(filename, frame),             # <<<<<<<<<<<<<<
  *             lineno,
  *             <object>code.co_name if code else "",
  */
-    __pyx_t_3 = __pyx_f_10dj_tracker_9traceback_get_file_info(__pyx_v_filename, __pyx_v_frame, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_3 = __pyx_f_10dj_tracker_9traceback_get_file_info(__pyx_v_filename, __pyx_v_frame, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (unlikely(__pyx_t_3 == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-      __PYX_ERR(0, 131, __pyx_L1_error)
+      __PYX_ERR(0, 134, __pyx_L1_error)
     }
 
-    /* "dj_tracker/traceback.pyx":129
+    /* "dj_tracker/traceback.pyx":132
  * 
  *     if (entry := cache.get(cache_key)) is None:
  *         entry = TracebackEntry(             # <<<<<<<<<<<<<<
  *             filename,
  *             *get_file_info(filename, frame),
  */
-    __pyx_t_4 = PyNumber_Add(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_4 = PyNumber_Add(__pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "dj_tracker/traceback.pyx":133
+    /* "dj_tracker/traceback.pyx":136
  *             *get_file_info(filename, frame),
  *             lineno,
  *             <object>code.co_name if code else "",             # <<<<<<<<<<<<<<
  *         )
  *         cache.set(cache_key, entry)
  */
     if ((__pyx_v_code != 0)) {
       __Pyx_INCREF(((PyObject *)__pyx_v_code->co_name));
       __pyx_t_3 = ((PyObject *)__pyx_v_code->co_name);
     } else {
-      __Pyx_INCREF(__pyx_kp_u__2);
-      __pyx_t_3 = __pyx_kp_u__2;
+      __Pyx_INCREF(__pyx_kp_u__4);
+      __pyx_t_3 = __pyx_kp_u__4;
     }
 
-    /* "dj_tracker/traceback.pyx":129
+    /* "dj_tracker/traceback.pyx":132
  * 
  *     if (entry := cache.get(cache_key)) is None:
  *         entry = TracebackEntry(             # <<<<<<<<<<<<<<
  *             filename,
  *             *get_file_info(filename, frame),
  */
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_lineno);
     __Pyx_GIVEREF(__pyx_v_lineno);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_lineno);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10dj_tracker_9traceback_TracebackEntry), __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10dj_tracker_9traceback_TracebackEntry), __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF_SET(__pyx_v_entry, ((struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "dj_tracker/traceback.pyx":135
+    /* "dj_tracker/traceback.pyx":138
  *             <object>code.co_name if code else "",
  *         )
  *         cache.set(cache_key, entry)             # <<<<<<<<<<<<<<
  * 
  *     return entry
  */
-    ((struct __pyx_vtabstruct_10dj_tracker_11cache_utils_LRUCache *)__pyx_v_cache->__pyx_vtab)->set(__pyx_v_cache, __pyx_v_cache_key, ((PyObject *)__pyx_v_entry), 0); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 135, __pyx_L1_error)
+    ((struct __pyx_vtabstruct_10dj_tracker_11cache_utils_LRUCache *)__pyx_v_cache->__pyx_vtab)->set(__pyx_v_cache, __pyx_v_cache_key, ((PyObject *)__pyx_v_entry), 0); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 138, __pyx_L1_error)
 
-    /* "dj_tracker/traceback.pyx":128
+    /* "dj_tracker/traceback.pyx":131
  *     cache_key = filename, lineno
  * 
  *     if (entry := cache.get(cache_key)) is None:             # <<<<<<<<<<<<<<
  *         entry = TracebackEntry(
  *             filename,
  */
   }
 
-  /* "dj_tracker/traceback.pyx":137
+  /* "dj_tracker/traceback.pyx":140
  *         cache.set(cache_key, entry)
  * 
  *     return entry             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_entry);
   __pyx_r = __pyx_v_entry;
   goto __pyx_L0;
 
-  /* "dj_tracker/traceback.pyx":118
+  /* "dj_tracker/traceback.pyx":121
  * 
  * 
  * cdef inline TracebackEntry get_entry(             # <<<<<<<<<<<<<<
  *     str filename,
  *     object lineno,
  */
 
@@ -5562,15 +5723,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_entry);
   __Pyx_XDECREF(__pyx_v_cache_key);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "dj_tracker/traceback.pyx":140
+/* "dj_tracker/traceback.pyx":143
  * 
  * 
  * cpdef tuple get_traceback():             # <<<<<<<<<<<<<<
  *     cdef:
  *         PyFrameObject *frame
  */
 
@@ -5603,50 +5764,50 @@
   PyObject *__pyx_t_12;
   int __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_traceback", 0);
 
-  /* "dj_tracker/traceback.pyx":147
+  /* "dj_tracker/traceback.pyx":150
  *         PyObject *node
  *         TracebackEntry entry
  *         str self_var = "self"             # <<<<<<<<<<<<<<
  *         bint top_entries_found = False
  *         int num_bottom_entries = 0
  */
   __Pyx_INCREF(__pyx_n_u_self);
   __pyx_v_self_var = __pyx_n_u_self;
 
-  /* "dj_tracker/traceback.pyx":148
+  /* "dj_tracker/traceback.pyx":151
  *         TracebackEntry entry
  *         str self_var = "self"
  *         bint top_entries_found = False             # <<<<<<<<<<<<<<
  *         int num_bottom_entries = 0
  *         list stack = <list>HashableList()
  */
   __pyx_v_top_entries_found = 0;
 
-  /* "dj_tracker/traceback.pyx":149
+  /* "dj_tracker/traceback.pyx":152
  *         str self_var = "self"
  *         bint top_entries_found = False
  *         int num_bottom_entries = 0             # <<<<<<<<<<<<<<
  *         list stack = <list>HashableList()
  *         object template_info = None
  */
   __pyx_v_num_bottom_entries = 0;
 
-  /* "dj_tracker/traceback.pyx":150
+  /* "dj_tracker/traceback.pyx":153
  *         bint top_entries_found = False
  *         int num_bottom_entries = 0
  *         list stack = <list>HashableList()             # <<<<<<<<<<<<<<
  *         object template_info = None
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_HashableList); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_HashableList); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -5656,147 +5817,147 @@
       __pyx_t_4 = 1;
     }
   }
   {
     PyObject *__pyx_callargs[1] = {__pyx_t_3, };
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_t_2 = __pyx_t_1;
   __Pyx_INCREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_stack = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "dj_tracker/traceback.pyx":151
+  /* "dj_tracker/traceback.pyx":154
  *         int num_bottom_entries = 0
  *         list stack = <list>HashableList()
  *         object template_info = None             # <<<<<<<<<<<<<<
  * 
  *     if not (last_frame := PyEval_GetFrame()):
  */
   __Pyx_INCREF(Py_None);
   __pyx_v_template_info = Py_None;
 
-  /* "dj_tracker/traceback.pyx":153
+  /* "dj_tracker/traceback.pyx":156
  *         object template_info = None
  * 
  *     if not (last_frame := PyEval_GetFrame()):             # <<<<<<<<<<<<<<
  *         return (), None
  * 
  */
   __pyx_t_5 = PyEval_GetFrame();
   __pyx_v_last_frame = __pyx_t_5;
   __pyx_t_6 = (!(__pyx_t_5 != 0));
   if (__pyx_t_6) {
 
-    /* "dj_tracker/traceback.pyx":154
+    /* "dj_tracker/traceback.pyx":157
  * 
  *     if not (last_frame := PyEval_GetFrame()):
  *         return (), None             # <<<<<<<<<<<<<<
  * 
  *     Py_INCREF(<PyObject*>last_frame)
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(__pyx_tuple__6);
-    __pyx_r = __pyx_tuple__6;
+    __Pyx_INCREF(__pyx_tuple__8);
+    __pyx_r = __pyx_tuple__8;
     goto __pyx_L0;
 
-    /* "dj_tracker/traceback.pyx":153
+    /* "dj_tracker/traceback.pyx":156
  *         object template_info = None
  * 
  *     if not (last_frame := PyEval_GetFrame()):             # <<<<<<<<<<<<<<
  *         return (), None
  * 
  */
   }
 
-  /* "dj_tracker/traceback.pyx":156
+  /* "dj_tracker/traceback.pyx":159
  *         return (), None
  * 
  *     Py_INCREF(<PyObject*>last_frame)             # <<<<<<<<<<<<<<
  * 
  *     while frame := PyFrame_GetBack(last_frame):
  */
   Py_INCREF(((PyObject *)__pyx_v_last_frame));
 
-  /* "dj_tracker/traceback.pyx":158
+  /* "dj_tracker/traceback.pyx":161
  *     Py_INCREF(<PyObject*>last_frame)
  * 
  *     while frame := PyFrame_GetBack(last_frame):             # <<<<<<<<<<<<<<
  *         Py_DECREF(<PyObject*>last_frame)
  *         last_frame = frame
  */
   while (1) {
     __pyx_t_5 = PyFrame_GetBack(__pyx_v_last_frame);
     __pyx_v_frame = __pyx_t_5;
     __pyx_t_6 = (__pyx_t_5 != 0);
     if (!__pyx_t_6) break;
 
-    /* "dj_tracker/traceback.pyx":159
+    /* "dj_tracker/traceback.pyx":162
  * 
  *     while frame := PyFrame_GetBack(last_frame):
  *         Py_DECREF(<PyObject*>last_frame)             # <<<<<<<<<<<<<<
  *         last_frame = frame
  * 
  */
     Py_DECREF(((PyObject *)__pyx_v_last_frame));
 
-    /* "dj_tracker/traceback.pyx":160
+    /* "dj_tracker/traceback.pyx":163
  *     while frame := PyFrame_GetBack(last_frame):
  *         Py_DECREF(<PyObject*>last_frame)
  *         last_frame = frame             # <<<<<<<<<<<<<<
  * 
  *         code = PyFrame_GetCode(frame)
  */
     __pyx_v_last_frame = __pyx_v_frame;
 
-    /* "dj_tracker/traceback.pyx":162
+    /* "dj_tracker/traceback.pyx":165
  *         last_frame = frame
  * 
  *         code = PyFrame_GetCode(frame)             # <<<<<<<<<<<<<<
  *         entry = get_entry(<object>code.co_filename, PyFrame_GetLineNumber(frame), frame, code)
  *         Py_DECREF(<PyObject*>code)
  */
     __pyx_v_code = PyFrame_GetCode(__pyx_v_frame);
 
-    /* "dj_tracker/traceback.pyx":163
+    /* "dj_tracker/traceback.pyx":166
  * 
  *         code = PyFrame_GetCode(frame)
  *         entry = get_entry(<object>code.co_filename, PyFrame_GetLineNumber(frame), frame, code)             # <<<<<<<<<<<<<<
  *         Py_DECREF(<PyObject*>code)
  * 
  */
-    if (!(likely(PyUnicode_CheckExact(((PyObject *)__pyx_v_code->co_filename)))||((((PyObject *)__pyx_v_code->co_filename)) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", ((PyObject *)__pyx_v_code->co_filename)))) __PYX_ERR(0, 163, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(((PyObject *)__pyx_v_code->co_filename)))||((((PyObject *)__pyx_v_code->co_filename)) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", ((PyObject *)__pyx_v_code->co_filename)))) __PYX_ERR(0, 166, __pyx_L1_error)
     __pyx_t_2 = ((PyObject *)__pyx_v_code->co_filename);
     __Pyx_INCREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyInt_From_int(PyFrame_GetLineNumber(__pyx_v_frame)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(PyFrame_GetLineNumber(__pyx_v_frame)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_7.__pyx_n = 1;
     __pyx_t_7.code = __pyx_v_code;
-    __pyx_t_3 = ((PyObject *)__pyx_f_10dj_tracker_9traceback_get_entry(((PyObject*)__pyx_t_2), __pyx_t_1, __pyx_v_frame, &__pyx_t_7)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __pyx_t_3 = ((PyObject *)__pyx_f_10dj_tracker_9traceback_get_entry(((PyObject*)__pyx_t_2), __pyx_t_1, __pyx_v_frame, &__pyx_t_7)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF_SET(__pyx_v_entry, ((struct __pyx_obj_10dj_tracker_9traceback_TracebackEntry *)__pyx_t_3));
     __pyx_t_3 = 0;
 
-    /* "dj_tracker/traceback.pyx":164
+    /* "dj_tracker/traceback.pyx":167
  *         code = PyFrame_GetCode(frame)
  *         entry = get_entry(<object>code.co_filename, PyFrame_GetLineNumber(frame), frame, code)
  *         Py_DECREF(<PyObject*>code)             # <<<<<<<<<<<<<<
  * 
  *         if template_info is None and entry.is_render:
  */
     Py_DECREF(((PyObject *)__pyx_v_code));
 
-    /* "dj_tracker/traceback.pyx":166
+    /* "dj_tracker/traceback.pyx":169
  *         Py_DECREF(<PyObject*>code)
  * 
  *         if template_info is None and entry.is_render:             # <<<<<<<<<<<<<<
  *             # This logic is inspired from:
  *             # https://github.com/jazzband/django-debug-toolbar/blob/main/debug_toolbar/utils.py#L123-L127
  */
     __pyx_t_8 = (__pyx_v_template_info == Py_None);
@@ -5805,15 +5966,15 @@
       __pyx_t_6 = __pyx_t_8;
       goto __pyx_L7_bool_binop_done;
     }
     __pyx_t_6 = __pyx_v_entry->is_render;
     __pyx_L7_bool_binop_done:;
     if (__pyx_t_6) {
 
-      /* "dj_tracker/traceback.pyx":169
+      /* "dj_tracker/traceback.pyx":172
  *             # This logic is inspired from:
  *             # https://github.com/jazzband/django-debug-toolbar/blob/main/debug_toolbar/utils.py#L123-L127
  *             try:             # <<<<<<<<<<<<<<
  *                 node = PyFrame_GetVar(frame, <PyObject*>self_var)
  *             except NameError:
  */
       {
@@ -5821,94 +5982,94 @@
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_9, &__pyx_t_10, &__pyx_t_11);
         __Pyx_XGOTREF(__pyx_t_9);
         __Pyx_XGOTREF(__pyx_t_10);
         __Pyx_XGOTREF(__pyx_t_11);
         /*try:*/ {
 
-          /* "dj_tracker/traceback.pyx":170
+          /* "dj_tracker/traceback.pyx":173
  *             # https://github.com/jazzband/django-debug-toolbar/blob/main/debug_toolbar/utils.py#L123-L127
  *             try:
  *                 node = PyFrame_GetVar(frame, <PyObject*>self_var)             # <<<<<<<<<<<<<<
  *             except NameError:
  *                 pass
  */
-          __pyx_t_12 = PyFrame_GetVar(__pyx_v_frame, ((PyObject *)__pyx_v_self_var)); if (unlikely(__pyx_t_12 == ((PyObject *)NULL))) __PYX_ERR(0, 170, __pyx_L9_error)
+          __pyx_t_12 = PyFrame_GetVar(__pyx_v_frame, ((PyObject *)__pyx_v_self_var)); if (unlikely(__pyx_t_12 == ((PyObject *)NULL))) __PYX_ERR(0, 173, __pyx_L9_error)
           __pyx_v_node = __pyx_t_12;
 
-          /* "dj_tracker/traceback.pyx":169
+          /* "dj_tracker/traceback.pyx":172
  *             # This logic is inspired from:
  *             # https://github.com/jazzband/django-debug-toolbar/blob/main/debug_toolbar/utils.py#L123-L127
  *             try:             # <<<<<<<<<<<<<<
  *                 node = PyFrame_GetVar(frame, <PyObject*>self_var)
  *             except NameError:
  */
         }
 
-        /* "dj_tracker/traceback.pyx":174
+        /* "dj_tracker/traceback.pyx":177
  *                 pass
  *             else:
  *                 node_obj = <object>node             # <<<<<<<<<<<<<<
  *                 if isinstance(node_obj, Node):
  *                     template_info = get_entry(node_obj.origin.name, node_obj.token.lineno, frame)
  */
         /*else:*/ {
           __pyx_t_3 = ((PyObject *)__pyx_v_node);
           __Pyx_INCREF(__pyx_t_3);
           __Pyx_XDECREF_SET(__pyx_v_node_obj, __pyx_t_3);
           __pyx_t_3 = 0;
 
-          /* "dj_tracker/traceback.pyx":175
+          /* "dj_tracker/traceback.pyx":178
  *             else:
  *                 node_obj = <object>node
  *                 if isinstance(node_obj, Node):             # <<<<<<<<<<<<<<
  *                     template_info = get_entry(node_obj.origin.name, node_obj.token.lineno, frame)
  *                 Py_DECREF(node)
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Node); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L11_except_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Node); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 178, __pyx_L11_except_error)
           __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_6 = PyObject_IsInstance(__pyx_v_node_obj, __pyx_t_3); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 175, __pyx_L11_except_error)
+          __pyx_t_6 = PyObject_IsInstance(__pyx_v_node_obj, __pyx_t_3); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(0, 178, __pyx_L11_except_error)
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           if (__pyx_t_6) {
 
-            /* "dj_tracker/traceback.pyx":176
+            /* "dj_tracker/traceback.pyx":179
  *                 node_obj = <object>node
  *                 if isinstance(node_obj, Node):
  *                     template_info = get_entry(node_obj.origin.name, node_obj.token.lineno, frame)             # <<<<<<<<<<<<<<
  *                 Py_DECREF(node)
  * 
  */
-            __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node_obj, __pyx_n_s_origin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 176, __pyx_L11_except_error)
+            __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node_obj, __pyx_n_s_origin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L11_except_error)
             __Pyx_GOTREF(__pyx_t_3);
-            __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L11_except_error)
+            __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L11_except_error)
             __Pyx_GOTREF(__pyx_t_1);
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-            if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 176, __pyx_L11_except_error)
-            __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node_obj, __pyx_n_s_token); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 176, __pyx_L11_except_error)
+            if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 179, __pyx_L11_except_error)
+            __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_node_obj, __pyx_n_s_token); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L11_except_error)
             __Pyx_GOTREF(__pyx_t_3);
-            __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_lineno); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 176, __pyx_L11_except_error)
+            __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_lineno); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L11_except_error)
             __Pyx_GOTREF(__pyx_t_2);
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-            __pyx_t_3 = ((PyObject *)__pyx_f_10dj_tracker_9traceback_get_entry(((PyObject*)__pyx_t_1), __pyx_t_2, __pyx_v_frame, NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 176, __pyx_L11_except_error)
+            __pyx_t_3 = ((PyObject *)__pyx_f_10dj_tracker_9traceback_get_entry(((PyObject*)__pyx_t_1), __pyx_t_2, __pyx_v_frame, NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L11_except_error)
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
             __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
             __Pyx_DECREF_SET(__pyx_v_template_info, __pyx_t_3);
             __pyx_t_3 = 0;
 
-            /* "dj_tracker/traceback.pyx":175
+            /* "dj_tracker/traceback.pyx":178
  *             else:
  *                 node_obj = <object>node
  *                 if isinstance(node_obj, Node):             # <<<<<<<<<<<<<<
  *                     template_info = get_entry(node_obj.origin.name, node_obj.token.lineno, frame)
  *                 Py_DECREF(node)
  */
           }
 
-          /* "dj_tracker/traceback.pyx":177
+          /* "dj_tracker/traceback.pyx":180
  *                 if isinstance(node_obj, Node):
  *                     template_info = get_entry(node_obj.origin.name, node_obj.token.lineno, frame)
  *                 Py_DECREF(node)             # <<<<<<<<<<<<<<
  * 
  *         if entry.ignore:
  */
           Py_DECREF(__pyx_v_node);
@@ -5918,30 +6079,30 @@
         __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
         goto __pyx_L16_try_end;
         __pyx_L9_error:;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-        /* "dj_tracker/traceback.pyx":171
+        /* "dj_tracker/traceback.pyx":174
  *             try:
  *                 node = PyFrame_GetVar(frame, <PyObject*>self_var)
  *             except NameError:             # <<<<<<<<<<<<<<
  *                 pass
  *             else:
  */
         __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_NameError);
         if (__pyx_t_4) {
           __Pyx_ErrRestore(0,0,0);
           goto __pyx_L10_exception_handled;
         }
         goto __pyx_L11_except_error;
         __pyx_L11_except_error:;
 
-        /* "dj_tracker/traceback.pyx":169
+        /* "dj_tracker/traceback.pyx":172
  *             # This logic is inspired from:
  *             # https://github.com/jazzband/django-debug-toolbar/blob/main/debug_toolbar/utils.py#L123-L127
  *             try:             # <<<<<<<<<<<<<<
  *                 node = PyFrame_GetVar(frame, <PyObject*>self_var)
  *             except NameError:
  */
         __Pyx_XGIVEREF(__pyx_t_9);
@@ -5953,220 +6114,220 @@
         __Pyx_XGIVEREF(__pyx_t_9);
         __Pyx_XGIVEREF(__pyx_t_10);
         __Pyx_XGIVEREF(__pyx_t_11);
         __Pyx_ExceptionReset(__pyx_t_9, __pyx_t_10, __pyx_t_11);
         __pyx_L16_try_end:;
       }
 
-      /* "dj_tracker/traceback.pyx":166
+      /* "dj_tracker/traceback.pyx":169
  *         Py_DECREF(<PyObject*>code)
  * 
  *         if template_info is None and entry.is_render:             # <<<<<<<<<<<<<<
  *             # This logic is inspired from:
  *             # https://github.com/jazzband/django-debug-toolbar/blob/main/debug_toolbar/utils.py#L123-L127
  */
     }
 
-    /* "dj_tracker/traceback.pyx":179
+    /* "dj_tracker/traceback.pyx":182
  *                 Py_DECREF(node)
  * 
  *         if entry.ignore:             # <<<<<<<<<<<<<<
  *             if top_entries_found:
  *                 stack.append(entry)
  */
     if (__pyx_v_entry->ignore) {
 
-      /* "dj_tracker/traceback.pyx":180
+      /* "dj_tracker/traceback.pyx":183
  * 
  *         if entry.ignore:
  *             if top_entries_found:             # <<<<<<<<<<<<<<
  *                 stack.append(entry)
  *                 num_bottom_entries += 1
  */
       if (__pyx_v_top_entries_found) {
 
-        /* "dj_tracker/traceback.pyx":181
+        /* "dj_tracker/traceback.pyx":184
  *         if entry.ignore:
  *             if top_entries_found:
  *                 stack.append(entry)             # <<<<<<<<<<<<<<
  *                 num_bottom_entries += 1
  *         else:
  */
         if (unlikely(__pyx_v_stack == Py_None)) {
           PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
-          __PYX_ERR(0, 181, __pyx_L1_error)
+          __PYX_ERR(0, 184, __pyx_L1_error)
         }
-        __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_stack, ((PyObject *)__pyx_v_entry)); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 181, __pyx_L1_error)
+        __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_stack, ((PyObject *)__pyx_v_entry)); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 184, __pyx_L1_error)
 
-        /* "dj_tracker/traceback.pyx":182
+        /* "dj_tracker/traceback.pyx":185
  *             if top_entries_found:
  *                 stack.append(entry)
  *                 num_bottom_entries += 1             # <<<<<<<<<<<<<<
  *         else:
  *             if num_bottom_entries:
  */
         __pyx_v_num_bottom_entries = (__pyx_v_num_bottom_entries + 1);
 
-        /* "dj_tracker/traceback.pyx":180
+        /* "dj_tracker/traceback.pyx":183
  * 
  *         if entry.ignore:
  *             if top_entries_found:             # <<<<<<<<<<<<<<
  *                 stack.append(entry)
  *                 num_bottom_entries += 1
  */
       }
 
-      /* "dj_tracker/traceback.pyx":179
+      /* "dj_tracker/traceback.pyx":182
  *                 Py_DECREF(node)
  * 
  *         if entry.ignore:             # <<<<<<<<<<<<<<
  *             if top_entries_found:
  *                 stack.append(entry)
  */
       goto __pyx_L18;
     }
 
-    /* "dj_tracker/traceback.pyx":184
+    /* "dj_tracker/traceback.pyx":187
  *                 num_bottom_entries += 1
  *         else:
  *             if num_bottom_entries:             # <<<<<<<<<<<<<<
  *                 num_bottom_entries = 0
  *             elif not top_entries_found:
  */
     /*else*/ {
       __pyx_t_6 = (__pyx_v_num_bottom_entries != 0);
       if (__pyx_t_6) {
 
-        /* "dj_tracker/traceback.pyx":185
+        /* "dj_tracker/traceback.pyx":188
  *         else:
  *             if num_bottom_entries:
  *                 num_bottom_entries = 0             # <<<<<<<<<<<<<<
  *             elif not top_entries_found:
  *                 top_entries_found = True
  */
         __pyx_v_num_bottom_entries = 0;
 
-        /* "dj_tracker/traceback.pyx":184
+        /* "dj_tracker/traceback.pyx":187
  *                 num_bottom_entries += 1
  *         else:
  *             if num_bottom_entries:             # <<<<<<<<<<<<<<
  *                 num_bottom_entries = 0
  *             elif not top_entries_found:
  */
         goto __pyx_L20;
       }
 
-      /* "dj_tracker/traceback.pyx":186
+      /* "dj_tracker/traceback.pyx":189
  *             if num_bottom_entries:
  *                 num_bottom_entries = 0
  *             elif not top_entries_found:             # <<<<<<<<<<<<<<
  *                 top_entries_found = True
  * 
  */
       __pyx_t_6 = (!__pyx_v_top_entries_found);
       if (__pyx_t_6) {
 
-        /* "dj_tracker/traceback.pyx":187
+        /* "dj_tracker/traceback.pyx":190
  *                 num_bottom_entries = 0
  *             elif not top_entries_found:
  *                 top_entries_found = True             # <<<<<<<<<<<<<<
  * 
  *             stack.append(entry)
  */
         __pyx_v_top_entries_found = 1;
 
-        /* "dj_tracker/traceback.pyx":186
+        /* "dj_tracker/traceback.pyx":189
  *             if num_bottom_entries:
  *                 num_bottom_entries = 0
  *             elif not top_entries_found:             # <<<<<<<<<<<<<<
  *                 top_entries_found = True
  * 
  */
       }
       __pyx_L20:;
 
-      /* "dj_tracker/traceback.pyx":189
+      /* "dj_tracker/traceback.pyx":192
  *                 top_entries_found = True
  * 
  *             stack.append(entry)             # <<<<<<<<<<<<<<
  * 
  *     Py_DECREF(<PyObject*>last_frame)
  */
       if (unlikely(__pyx_v_stack == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
-        __PYX_ERR(0, 189, __pyx_L1_error)
+        __PYX_ERR(0, 192, __pyx_L1_error)
       }
-      __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_stack, ((PyObject *)__pyx_v_entry)); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 189, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_stack, ((PyObject *)__pyx_v_entry)); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 192, __pyx_L1_error)
     }
     __pyx_L18:;
   }
 
-  /* "dj_tracker/traceback.pyx":191
+  /* "dj_tracker/traceback.pyx":194
  *             stack.append(entry)
  * 
  *     Py_DECREF(<PyObject*>last_frame)             # <<<<<<<<<<<<<<
  * 
  *     if num_bottom_entries:
  */
   Py_DECREF(((PyObject *)__pyx_v_last_frame));
 
-  /* "dj_tracker/traceback.pyx":193
+  /* "dj_tracker/traceback.pyx":196
  *     Py_DECREF(<PyObject*>last_frame)
  * 
  *     if num_bottom_entries:             # <<<<<<<<<<<<<<
  *         stack[-num_bottom_entries:] = []
  * 
  */
   __pyx_t_6 = (__pyx_v_num_bottom_entries != 0);
   if (__pyx_t_6) {
 
-    /* "dj_tracker/traceback.pyx":194
+    /* "dj_tracker/traceback.pyx":197
  * 
  *     if num_bottom_entries:
  *         stack[-num_bottom_entries:] = []             # <<<<<<<<<<<<<<
  * 
  *     return stack, template_info
  */
-    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 194, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (unlikely(__pyx_v_stack == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 194, __pyx_L1_error)
+      __PYX_ERR(0, 197, __pyx_L1_error)
     }
-    if (__Pyx_PyObject_SetSlice(__pyx_v_stack, __pyx_t_3, (-__pyx_v_num_bottom_entries), 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 194, __pyx_L1_error)
+    if (__Pyx_PyObject_SetSlice(__pyx_v_stack, __pyx_t_3, (-__pyx_v_num_bottom_entries), 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "dj_tracker/traceback.pyx":193
+    /* "dj_tracker/traceback.pyx":196
  *     Py_DECREF(<PyObject*>last_frame)
  * 
  *     if num_bottom_entries:             # <<<<<<<<<<<<<<
  *         stack[-num_bottom_entries:] = []
  * 
  */
   }
 
-  /* "dj_tracker/traceback.pyx":196
+  /* "dj_tracker/traceback.pyx":199
  *         stack[-num_bottom_entries:] = []
  * 
  *     return stack, template_info             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_stack);
   __Pyx_GIVEREF(__pyx_v_stack);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_stack);
   __Pyx_INCREF(__pyx_v_template_info);
   __Pyx_GIVEREF(__pyx_v_template_info);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_template_info);
   __pyx_r = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "dj_tracker/traceback.pyx":140
+  /* "dj_tracker/traceback.pyx":143
  * 
  * 
  * cpdef tuple get_traceback():             # <<<<<<<<<<<<<<
  *     cdef:
  *         PyFrameObject *frame
  */
 
@@ -6208,15 +6369,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_traceback", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_10dj_tracker_9traceback_get_traceback(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_10dj_tracker_9traceback_get_traceback(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6350,15 +6511,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x6d8739c, 0xdb324b9, 0x268af81):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x6d8739c, 0xdb324b9, 0x268af81) = (filename, func, hash_value, ignore, is_render, lineno, rel_path))" % __pyx_checksum
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__7, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__9, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x6d8739c, 0xdb324b9, 0x268af81):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
@@ -7193,15 +7354,15 @@
   }
 }
 
 static PyObject *__pyx_tp_getattro_10dj_tracker_9traceback_TracebackEntry(PyObject *o, PyObject *n) {
   PyObject *v = __Pyx_PyObject_GenericGetAttr(o, n);
   if (!v && PyErr_ExceptionMatches(PyExc_AttributeError)) {
     PyErr_Clear();
-    v = __pyx_pw_10dj_tracker_9traceback_14TracebackEntry_3__getattr__(o, n);
+    v = __pyx_pw_10dj_tracker_9traceback_14TracebackEntry_5__getattr__(o, n);
   }
   return v;
 }
 
 static PyObject *__pyx_getprop_10dj_tracker_9traceback_14TracebackEntry_filename_id(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_10dj_tracker_9traceback_14TracebackEntry_11filename_id_1__get__(o);
 }
@@ -7226,18 +7387,23 @@
   return __pyx_pw_10dj_tracker_9traceback_14TracebackEntry_6lineno_1__get__(o);
 }
 
 static PyObject *__pyx_getprop_10dj_tracker_9traceback_14TracebackEntry_func(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_10dj_tracker_9traceback_14TracebackEntry_4func_1__get__(o);
 }
 
+static PyObject *__pyx_specialmethod___pyx_pw_10dj_tracker_9traceback_14TracebackEntry_3__repr__(PyObject *self, CYTHON_UNUSED PyObject *arg) {
+  return __pyx_pw_10dj_tracker_9traceback_14TracebackEntry_3__repr__(self);
+}
+
 static PyMethodDef __pyx_methods_10dj_tracker_9traceback_TracebackEntry[] = {
-  {"__getattr__", (PyCFunction)__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_3__getattr__, METH_O|METH_COEXIST, 0},
-  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_5__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_7__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__repr__", (PyCFunction)__pyx_specialmethod___pyx_pw_10dj_tracker_9traceback_14TracebackEntry_3__repr__, METH_NOARGS|METH_COEXIST, 0},
+  {"__getattr__", (PyCFunction)__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_5__getattr__, METH_O|METH_COEXIST, 0},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_7__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_9__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
 
 static struct PyGetSetDef __pyx_getsets_10dj_tracker_9traceback_TracebackEntry[] = {
   {(char *)"filename_id", __pyx_getprop_10dj_tracker_9traceback_14TracebackEntry_filename_id, 0, (char *)0, 0},
   {(char *)"code", __pyx_getprop_10dj_tracker_9traceback_14TracebackEntry_code, 0, (char *)0, 0},
   {(char *)"cache_key", __pyx_getprop_10dj_tracker_9traceback_14TracebackEntry_cache_key, 0, (char *)0, 0},
@@ -7246,14 +7412,15 @@
   {(char *)"lineno", __pyx_getprop_10dj_tracker_9traceback_14TracebackEntry_lineno, 0, (char *)0, 0},
   {(char *)"func", __pyx_getprop_10dj_tracker_9traceback_14TracebackEntry_func, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 #if CYTHON_USE_TYPE_SPECS
 static PyType_Slot __pyx_type_10dj_tracker_9traceback_TracebackEntry_slots[] = {
   {Py_tp_dealloc, (void *)__pyx_tp_dealloc_10dj_tracker_9traceback_TracebackEntry},
+  {Py_tp_repr, (void *)__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_3__repr__},
   {Py_tp_getattro, (void *)__pyx_tp_getattro_10dj_tracker_9traceback_TracebackEntry},
   {Py_tp_methods, (void *)__pyx_methods_10dj_tracker_9traceback_TracebackEntry},
   {Py_tp_getset, (void *)__pyx_getsets_10dj_tracker_9traceback_TracebackEntry},
   {Py_tp_init, (void *)__pyx_pw_10dj_tracker_9traceback_14TracebackEntry_1__init__},
   {Py_tp_new, (void *)__pyx_tp_new_10dj_tracker_9traceback_TracebackEntry},
   {0, 0},
 };
@@ -7282,15 +7449,15 @@
   0, /*tp_setattr*/
   #if PY_MAJOR_VERSION < 3
   0, /*tp_compare*/
   #endif
   #if PY_MAJOR_VERSION >= 3
   0, /*tp_as_async*/
   #endif
-  0, /*tp_repr*/
+  __pyx_pw_10dj_tracker_9traceback_14TracebackEntry_3__repr__, /*tp_repr*/
   0, /*tp_as_number*/
   0, /*tp_as_sequence*/
   0, /*tp_as_mapping*/
   0, /*tp_hash*/
   0, /*tp_call*/
   0, /*tp_str*/
   __pyx_tp_getattro_10dj_tracker_9traceback_TracebackEntry, /*tp_getattro*/
@@ -7360,31 +7527,34 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 /* #### Code section: pystring_table ### */
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
+    {&__pyx_kp_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 0},
     {&__pyx_n_s_AttributeError, __pyx_k_AttributeError, sizeof(__pyx_k_AttributeError), 0, 0, 1, 1},
     {&__pyx_n_s_HashableList, __pyx_k_HashableList, sizeof(__pyx_k_HashableList), 0, 0, 1, 1},
     {&__pyx_n_s_IGNORED_MODULES, __pyx_k_IGNORED_MODULES, sizeof(__pyx_k_IGNORED_MODULES), 0, 0, 1, 1},
     {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
     {&__pyx_n_s_KeyError, __pyx_k_KeyError, sizeof(__pyx_k_KeyError), 0, 0, 1, 1},
     {&__pyx_n_s_NameError, __pyx_k_NameError, sizeof(__pyx_k_NameError), 0, 0, 1, 1},
     {&__pyx_n_s_Node, __pyx_k_Node, sizeof(__pyx_k_Node), 0, 0, 1, 1},
+    {&__pyx_kp_u_None, __pyx_k_None, sizeof(__pyx_k_None), 0, 1, 0, 0},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_SourceFilePromise, __pyx_k_SourceFilePromise, sizeof(__pyx_k_SourceFilePromise), 0, 0, 1, 1},
     {&__pyx_n_s_StopIteration, __pyx_k_StopIteration, sizeof(__pyx_k_StopIteration), 0, 0, 1, 1},
     {&__pyx_n_s_TracebackEntry, __pyx_k_TracebackEntry, sizeof(__pyx_k_TracebackEntry), 0, 0, 1, 1},
     {&__pyx_n_s_TracebackEntry___reduce_cython, __pyx_k_TracebackEntry___reduce_cython, sizeof(__pyx_k_TracebackEntry___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_TracebackEntry___setstate_cython, __pyx_k_TracebackEntry___setstate_cython, sizeof(__pyx_k_TracebackEntry___setstate_cython), 0, 0, 1, 1},
-    {&__pyx_n_s__16, __pyx_k__16, sizeof(__pyx_k__16), 0, 0, 1, 1},
+    {&__pyx_n_s__10, __pyx_k__10, sizeof(__pyx_k__10), 0, 0, 1, 1},
+    {&__pyx_n_s__18, __pyx_k__18, sizeof(__pyx_k__18), 0, 0, 1, 1},
     {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
-    {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
-    {&__pyx_n_s__8, __pyx_k__8, sizeof(__pyx_k__8), 0, 0, 1, 1},
+    {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
+    {&__pyx_kp_u__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 1, 0, 0},
     {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
     {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
     {&__pyx_n_s_code, __pyx_k_code, sizeof(__pyx_k_code), 0, 0, 1, 1},
     {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
     {&__pyx_n_s_dict_2, __pyx_k_dict_2, sizeof(__pyx_k_dict_2), 0, 0, 1, 1},
@@ -7463,100 +7633,100 @@
     {&__pyx_n_s_use_setstate, __pyx_k_use_setstate, sizeof(__pyx_k_use_setstate), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_AttributeError = __Pyx_GetBuiltinName(__pyx_n_s_AttributeError); if (!__pyx_builtin_AttributeError) __PYX_ERR(0, 82, __pyx_L1_error)
-  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 93, __pyx_L1_error)
-  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 96, __pyx_L1_error)
-  __pyx_builtin_NameError = __Pyx_GetBuiltinName(__pyx_n_s_NameError); if (!__pyx_builtin_NameError) __PYX_ERR(0, 171, __pyx_L1_error)
+  __pyx_builtin_AttributeError = __Pyx_GetBuiltinName(__pyx_n_s_AttributeError); if (!__pyx_builtin_AttributeError) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_builtin_NameError = __Pyx_GetBuiltinName(__pyx_n_s_NameError); if (!__pyx_builtin_NameError) __PYX_ERR(0, 174, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "dj_tracker/traceback.pyx":103
+  /* "dj_tracker/traceback.pyx":106
  *             Py_DECREF(f_globals)
  * 
  *             if (root_module := sys.modules.get(module.split(".", 1)[0])) is not None:             # <<<<<<<<<<<<<<
  *                 if module_path := root_module.__file__:
  *                     module_dir = module_path.rsplit(os.sep, 2)[0]
  */
-  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_kp_u__3, __pyx_int_1); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 103, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_tuple__6 = PyTuple_Pack(2, __pyx_kp_u__5, __pyx_int_1); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "dj_tracker/traceback.pyx":154
+  /* "dj_tracker/traceback.pyx":157
  * 
  *     if not (last_frame := PyEval_GetFrame()):
  *         return (), None             # <<<<<<<<<<<<<<
  * 
  *     Py_INCREF(<PyObject*>last_frame)
  */
-  __pyx_tuple__6 = PyTuple_Pack(2, __pyx_empty_tuple, Py_None); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 154, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_empty_tuple, Py_None); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 157, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x6d8739c, 0xdb324b9, 0x268af81):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x6d8739c, 0xdb324b9, 0x268af81) = (filename, func, hash_value, ignore, is_render, lineno, rel_path))" % __pyx_checksum
  */
-  __pyx_tuple__7 = PyTuple_Pack(3, __pyx_int_114848668, __pyx_int_229844153, __pyx_int_40415105); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_tuple__9 = PyTuple_Pack(3, __pyx_int_114848668, __pyx_int_229844153, __pyx_int_40415105); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_tuple__9 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(1, 1, __pyx_L1_error)
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_TracebackEntry, (type(self), 0x6d8739c, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_TracebackEntry__set_state(self, __pyx_state)
  */
-  __pyx_tuple__11 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(1, 16, __pyx_L1_error)
 
-  /* "dj_tracker/traceback.pyx":140
+  /* "dj_tracker/traceback.pyx":143
  * 
  * 
  * cpdef tuple get_traceback():             # <<<<<<<<<<<<<<
  *     cdef:
  *         PyFrameObject *frame
  */
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_dj_tracker_traceback_pyx, __pyx_n_s_get_traceback, 140, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_dj_tracker_traceback_pyx, __pyx_n_s_get_traceback, 143, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 143, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_TracebackEntry(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__14 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_TracebackEntry, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__16 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_TracebackEntry, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -7618,61 +7788,61 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr)) __PYX_ERR(0, 113, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr_spec, __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
+  __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr)) __PYX_ERR(0, 116, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr_spec, __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
   #else
   __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr = &__pyx_type_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 113, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 116, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr->tp_dictoffset && __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_2_genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr)) __PYX_ERR(0, 95, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr_spec, __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr)) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr_spec, __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
   #else
   __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr = &__pyx_type_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr->tp_dictoffset && __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct_1_genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info_spec, NULL); if (unlikely(!__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info)) __PYX_ERR(0, 85, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info_spec, __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info_spec, NULL); if (unlikely(!__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info)) __PYX_ERR(0, 88, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info_spec, __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
   #else
   __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info = &__pyx_type_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info) < 0) __PYX_ERR(0, 85, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info->tp_dictoffset && __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_10dj_tracker_9traceback___pyx_scope_struct____pyx_f_10dj_tracker_9traceback_get_file_info->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
@@ -8173,80 +8343,80 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10dj_tracker_9traceback_14TracebackEntry_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_TracebackEntry___reduce_cython, NULL, __pyx_n_s_dj_tracker_traceback, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10dj_tracker_9traceback_14TracebackEntry_7__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_TracebackEntry___reduce_cython, NULL, __pyx_n_s_dj_tracker_traceback, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_10dj_tracker_9traceback_TracebackEntry->tp_dict, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_10dj_tracker_9traceback_TracebackEntry);
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_TracebackEntry, (type(self), 0x6d8739c, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_TracebackEntry__set_state(self, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10dj_tracker_9traceback_14TracebackEntry_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_TracebackEntry___setstate_cython, NULL, __pyx_n_s_dj_tracker_traceback, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 16, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_10dj_tracker_9traceback_14TracebackEntry_9__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_TracebackEntry___setstate_cython, NULL, __pyx_n_s_dj_tracker_traceback, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem((PyObject *)__pyx_ptype_10dj_tracker_9traceback_TracebackEntry->tp_dict, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_10dj_tracker_9traceback_TracebackEntry);
 
-  /* "dj_tracker/traceback.pyx":85
+  /* "dj_tracker/traceback.pyx":88
  * 
  * 
  * cdef tuple get_file_info(str filename, PyFrameObject *frame, dict cache = {}):             # <<<<<<<<<<<<<<
  *     """Retrieves the relative path for a filename and indicates if it should be ignored."""
  *     cdef:
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 85, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_k_ = ((PyObject*)__pyx_t_3);
+  __pyx_k__3 = ((PyObject*)__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "dj_tracker/traceback.pyx":123
+  /* "dj_tracker/traceback.pyx":126
  *     PyFrameObject *frame,
  *     PyCodeObject *code = NULL,
  *     LRUCache cache = LRUCache(maxsize=512)             # <<<<<<<<<<<<<<
  * ):
  *     cdef TracebackEntry entry
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_maxsize, __pyx_int_512) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10dj_tracker_11cache_utils_LRUCache), __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_maxsize, __pyx_int_512) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_10dj_tracker_11cache_utils_LRUCache), __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_k__5 = ((struct __pyx_obj_10dj_tracker_11cache_utils_LRUCache *)__pyx_t_2);
+  __pyx_k__7 = ((struct __pyx_obj_10dj_tracker_11cache_utils_LRUCache *)__pyx_t_2);
   __Pyx_GIVEREF((PyObject *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "dj_tracker/traceback.pyx":140
+  /* "dj_tracker/traceback.pyx":143
  * 
  * 
  * cpdef tuple get_traceback():             # <<<<<<<<<<<<<<
  *     cdef:
  *         PyFrameObject *frame
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10dj_tracker_9traceback_1get_traceback, 0, __pyx_n_s_get_traceback, NULL, __pyx_n_s_dj_tracker_traceback, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 140, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10dj_tracker_9traceback_1get_traceback, 0, __pyx_n_s_get_traceback, NULL, __pyx_n_s_dj_tracker_traceback, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_traceback, __pyx_t_2) < 0) __PYX_ERR(0, 140, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_traceback, __pyx_t_2) < 0) __PYX_ERR(0, 143, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_TracebackEntry(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10dj_tracker_9traceback_3__pyx_unpickle_TracebackEntry, 0, __pyx_n_s_pyx_unpickle_TracebackEntry, NULL, __pyx_n_s_dj_tracker_traceback, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_10dj_tracker_9traceback_3__pyx_unpickle_TracebackEntry, 0, __pyx_n_s_pyx_unpickle_TracebackEntry, NULL, __pyx_n_s_dj_tracker_traceback, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_TracebackEntry, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "dj_tracker/traceback.pyx":1
  * cimport cython             # <<<<<<<<<<<<<<
  * from cpython.object cimport PyObject
@@ -9114,14 +9284,263 @@
     #endif
     if (nargs == 0) {
         return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
     }
     return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
 }
 
+/* PyUnicode_Unicode */
+static CYTHON_INLINE PyObject* __Pyx_PyUnicode_Unicode(PyObject *obj) {
+    if (unlikely(obj == Py_None))
+        obj = __pyx_kp_u_None;
+    return __Pyx_NewRef(obj);
+}
+
+/* CIntToDigits */
+static const char DIGIT_PAIRS_10[2*10*10+1] = {
+    "00010203040506070809"
+    "10111213141516171819"
+    "20212223242526272829"
+    "30313233343536373839"
+    "40414243444546474849"
+    "50515253545556575859"
+    "60616263646566676869"
+    "70717273747576777879"
+    "80818283848586878889"
+    "90919293949596979899"
+};
+static const char DIGIT_PAIRS_8[2*8*8+1] = {
+    "0001020304050607"
+    "1011121314151617"
+    "2021222324252627"
+    "3031323334353637"
+    "4041424344454647"
+    "5051525354555657"
+    "6061626364656667"
+    "7071727374757677"
+};
+static const char DIGITS_HEX[2*16+1] = {
+    "0123456789abcdef"
+    "0123456789ABCDEF"
+};
+
+/* BuildPyUnicode */
+static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
+                                                int prepend_sign, char padding_char) {
+    PyObject *uval;
+    Py_ssize_t uoffset = ulength - clength;
+#if CYTHON_USE_UNICODE_INTERNALS
+    Py_ssize_t i;
+#if CYTHON_PEP393_ENABLED
+    void *udata;
+    uval = PyUnicode_New(ulength, 127);
+    if (unlikely(!uval)) return NULL;
+    udata = PyUnicode_DATA(uval);
+#else
+    Py_UNICODE *udata;
+    uval = PyUnicode_FromUnicode(NULL, ulength);
+    if (unlikely(!uval)) return NULL;
+    udata = PyUnicode_AS_UNICODE(uval);
+#endif
+    if (uoffset > 0) {
+        i = 0;
+        if (prepend_sign) {
+            __Pyx_PyUnicode_WRITE(PyUnicode_1BYTE_KIND, udata, 0, '-');
+            i++;
+        }
+        for (; i < uoffset; i++) {
+            __Pyx_PyUnicode_WRITE(PyUnicode_1BYTE_KIND, udata, i, padding_char);
+        }
+    }
+    for (i=0; i < clength; i++) {
+        __Pyx_PyUnicode_WRITE(PyUnicode_1BYTE_KIND, udata, uoffset+i, chars[i]);
+    }
+#else
+    {
+        PyObject *sign = NULL, *padding = NULL;
+        uval = NULL;
+        if (uoffset > 0) {
+            prepend_sign = !!prepend_sign;
+            if (uoffset > prepend_sign) {
+                padding = PyUnicode_FromOrdinal(padding_char);
+                if (likely(padding) && uoffset > prepend_sign + 1) {
+                    PyObject *tmp;
+                    PyObject *repeat = PyInt_FromSsize_t(uoffset - prepend_sign);
+                    if (unlikely(!repeat)) goto done_or_error;
+                    tmp = PyNumber_Multiply(padding, repeat);
+                    Py_DECREF(repeat);
+                    Py_DECREF(padding);
+                    padding = tmp;
+                }
+                if (unlikely(!padding)) goto done_or_error;
+            }
+            if (prepend_sign) {
+                sign = PyUnicode_FromOrdinal('-');
+                if (unlikely(!sign)) goto done_or_error;
+            }
+        }
+        uval = PyUnicode_DecodeASCII(chars, clength, NULL);
+        if (likely(uval) && padding) {
+            PyObject *tmp = PyNumber_Add(padding, uval);
+            Py_DECREF(uval);
+            uval = tmp;
+        }
+        if (likely(uval) && sign) {
+            PyObject *tmp = PyNumber_Add(sign, uval);
+            Py_DECREF(uval);
+            uval = tmp;
+        }
+done_or_error:
+        Py_XDECREF(padding);
+        Py_XDECREF(sign);
+    }
+#endif
+    return uval;
+}
+
+/* CIntToPyUnicode */
+static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_int(int value, Py_ssize_t width, char padding_char, char format_char) {
+    char digits[sizeof(int)*3+2];
+    char *dpos, *end = digits + sizeof(int)*3+2;
+    const char *hex_digits = DIGITS_HEX;
+    Py_ssize_t length, ulength;
+    int prepend_sign, last_one_off;
+    int remaining;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (format_char == 'X') {
+        hex_digits += 16;
+        format_char = 'x';
+    }
+    remaining = value;
+    last_one_off = 0;
+    dpos = end;
+    do {
+        int digit_pos;
+        switch (format_char) {
+        case 'o':
+            digit_pos = abs((int)(remaining % (8*8)));
+            remaining = (int) (remaining / (8*8));
+            dpos -= 2;
+            memcpy(dpos, DIGIT_PAIRS_8 + digit_pos * 2, 2);
+            last_one_off = (digit_pos < 8);
+            break;
+        case 'd':
+            digit_pos = abs((int)(remaining % (10*10)));
+            remaining = (int) (remaining / (10*10));
+            dpos -= 2;
+            memcpy(dpos, DIGIT_PAIRS_10 + digit_pos * 2, 2);
+            last_one_off = (digit_pos < 10);
+            break;
+        case 'x':
+            *(--dpos) = hex_digits[abs((int)(remaining % 16))];
+            remaining = (int) (remaining / 16);
+            break;
+        default:
+            assert(0);
+            break;
+        }
+    } while (unlikely(remaining != 0));
+    assert(!last_one_off || *dpos == '0');
+    dpos += last_one_off;
+    length = end - dpos;
+    ulength = length;
+    prepend_sign = 0;
+    if (!is_unsigned && value <= neg_one) {
+        if (padding_char == ' ' || width <= length + 1) {
+            *(--dpos) = '-';
+            ++length;
+        } else {
+            prepend_sign = 1;
+        }
+        ++ulength;
+    }
+    if (width > ulength) {
+        ulength = width;
+    }
+    if (ulength == 1) {
+        return PyUnicode_FromOrdinal(*dpos);
+    }
+    return __Pyx_PyUnicode_BuildFromAscii(ulength, dpos, (int) length, prepend_sign, padding_char);
+}
+
+/* JoinPyUnicode */
+static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
+                                      Py_UCS4 max_char) {
+#if CYTHON_USE_UNICODE_INTERNALS && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    PyObject *result_uval;
+    int result_ukind, kind_shift;
+    Py_ssize_t i, char_pos;
+    void *result_udata;
+    CYTHON_MAYBE_UNUSED_VAR(max_char);
+#if CYTHON_PEP393_ENABLED
+    result_uval = PyUnicode_New(result_ulength, max_char);
+    if (unlikely(!result_uval)) return NULL;
+    result_ukind = (max_char <= 255) ? PyUnicode_1BYTE_KIND : (max_char <= 65535) ? PyUnicode_2BYTE_KIND : PyUnicode_4BYTE_KIND;
+    kind_shift = (result_ukind == PyUnicode_4BYTE_KIND) ? 2 : result_ukind - 1;
+    result_udata = PyUnicode_DATA(result_uval);
+#else
+    result_uval = PyUnicode_FromUnicode(NULL, result_ulength);
+    if (unlikely(!result_uval)) return NULL;
+    result_ukind = sizeof(Py_UNICODE);
+    kind_shift = (result_ukind == 4) ? 2 : result_ukind - 1;
+    result_udata = PyUnicode_AS_UNICODE(result_uval);
+#endif
+    assert(kind_shift == 2 || kind_shift == 1 || kind_shift == 0);
+    char_pos = 0;
+    for (i=0; i < value_count; i++) {
+        int ukind;
+        Py_ssize_t ulength;
+        void *udata;
+        PyObject *uval = PyTuple_GET_ITEM(value_tuple, i);
+        if (unlikely(__Pyx_PyUnicode_READY(uval)))
+            goto bad;
+        ulength = __Pyx_PyUnicode_GET_LENGTH(uval);
+        if (unlikely(!ulength))
+            continue;
+        if (unlikely((PY_SSIZE_T_MAX >> kind_shift) - ulength < char_pos))
+            goto overflow;
+        ukind = __Pyx_PyUnicode_KIND(uval);
+        udata = __Pyx_PyUnicode_DATA(uval);
+        if (!CYTHON_PEP393_ENABLED || ukind == result_ukind) {
+            memcpy((char *)result_udata + (char_pos << kind_shift), udata, (size_t) (ulength << kind_shift));
+        } else {
+            #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
+            _PyUnicode_FastCopyCharacters(result_uval, char_pos, uval, 0, ulength);
+            #else
+            Py_ssize_t j;
+            for (j=0; j < ulength; j++) {
+                Py_UCS4 uchar = __Pyx_PyUnicode_READ(ukind, udata, j);
+                __Pyx_PyUnicode_WRITE(result_ukind, result_udata, char_pos+j, uchar);
+            }
+            #endif
+        }
+        char_pos += ulength;
+    }
+    return result_uval;
+overflow:
+    PyErr_SetString(PyExc_OverflowError, "join() result is too long for a Python string");
+bad:
+    Py_DECREF(result_uval);
+    return NULL;
+#else
+    CYTHON_UNUSED_VAR(max_char);
+    CYTHON_UNUSED_VAR(result_ulength);
+    CYTHON_UNUSED_VAR(value_count);
+    return PyUnicode_Join(__pyx_empty_unicode, value_tuple);
+#endif
+}
+
 /* PyObjectCallOneArg */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
     PyObject *args[2] = {NULL, arg};
     return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
 /* RaiseException */
@@ -10187,15 +10606,15 @@
         PyObject* module_dot = 0;
         PyObject* full_name = 0;
         PyErr_Clear();
         module_name_str = PyModule_GetName(module);
         if (unlikely(!module_name_str)) { goto modbad; }
         module_name = PyUnicode_FromString(module_name_str);
         if (unlikely(!module_name)) { goto modbad; }
-        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__3);
+        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__5);
         if (unlikely(!module_dot)) { goto modbad; }
         full_name = PyUnicode_Concat(module_dot, name);
         if (unlikely(!full_name)) { goto modbad; }
         #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
         {
             PyObject *modules = PyImport_GetModuleDict();
             if (unlikely(!modules))
@@ -10883,56 +11302,62 @@
     Py_XINCREF(imported_module);
 #else
     imported_module = PyImport_GetModule(name);
 #endif
     return imported_module;
 }
 #endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple) {
+    Py_ssize_t i, nparts;
+    nparts = PyTuple_GET_SIZE(parts_tuple);
+    for (i=1; i < nparts && module; i++) {
+        PyObject *part, *submodule;
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        part = PyTuple_GET_ITEM(parts_tuple, i);
+#else
+        part = PySequence_ITEM(parts_tuple, i);
+#endif
+        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
+#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+        Py_DECREF(part);
+#endif
+        Py_DECREF(module);
+        module = submodule;
+    }
+    if (unlikely(!module)) {
+        return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
+    }
+    return module;
+}
+#endif
 static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
 #if PY_MAJOR_VERSION < 3
-    PyObject *module, *from_list, *star = __pyx_n_s__8;
+    PyObject *module, *from_list, *star = __pyx_n_s__10;
     CYTHON_UNUSED_VAR(parts_tuple);
     from_list = PyList_New(1);
     if (unlikely(!from_list))
         return NULL;
     Py_INCREF(star);
     PyList_SET_ITEM(from_list, 0, star);
     module = __Pyx_Import(name, from_list, 0);
     Py_DECREF(from_list);
     return module;
 #else
-    Py_ssize_t i, nparts;
     PyObject *imported_module;
     PyObject *module = __Pyx_Import(name, NULL, 0);
     if (!parts_tuple || unlikely(!module))
         return module;
     imported_module = __Pyx__ImportDottedModule_Lookup(name);
     if (likely(imported_module)) {
         Py_DECREF(module);
         return imported_module;
     }
     PyErr_Clear();
-    nparts = PyTuple_GET_SIZE(parts_tuple);
-    for (i=1; i < nparts && module; i++) {
-        PyObject *part, *submodule;
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        part = PyTuple_GET_ITEM(parts_tuple, i);
-#else
-        part = PySequence_ITEM(parts_tuple, i);
-#endif
-        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
-#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
-        Py_DECREF(part);
-#endif
-        Py_DECREF(module);
-        module = submodule;
-    }
-    if (likely(module))
-        return module;
-    return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
+    return __Pyx_ImportDottedModule_WalkParts(module, name, parts_tuple);
 #endif
 }
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
     PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
     if (likely(module)) {
         PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
@@ -12745,15 +13170,15 @@
 static __Pyx_TypeName
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name_2);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
-        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__16));
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__18));
     }
     return name;
 }
 #endif
 
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
```

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/traceback.pyx` & `django_trackings-0.6.0a0/src/dj_tracker/traceback.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,17 @@
                 self.filename_id,
                 self.lineno,
                 hash_string(self.code),
                 hash_string(self.func),
             )
         )
     
+    def __repr__(self):
+        return f"{self.rel_path}:{self.lineno} - {self.code}"
+    
     def __getattr__(self, name):
         if name == "hash_value":
             self.hash_value = hash((self.rel_path, self.lineno))
             return self.hash_value
 
         raise AttributeError(name)
```

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/tracker.py` & `django_trackings-0.6.0a0/src/dj_tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.5.2a0/src/dj_tracker/utils.py` & `django_trackings-0.6.0a0/src/dj_tracker/utils.py`

 * *Files identical despite different names*

### Comparing `django_trackings-0.5.2a0/src/django_trackings.egg-info/SOURCES.txt` & `django_trackings-0.6.0a0/src/django_trackings.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -29,16 +29,19 @@
 src/dj_tracker/middleware/__init__.py
 src/dj_tracker/migrations/0001_initial.py
 src/dj_tracker/migrations/__init__.py
 src/dj_tracker/static/dj_tracker/css/main.css
 src/dj_tracker/static/dj_tracker/js/query_group.js
 src/dj_tracker/templates/dj_tracker/base.html
 src/dj_tracker/templates/dj_tracker/home.html
-src/dj_tracker/templates/dj_tracker/pagination.html
-src/dj_tracker/templates/dj_tracker/qs_tracking.html
+src/dj_tracker/templates/dj_tracker/list.html
+src/dj_tracker/templates/dj_tracker/queries.html
+src/dj_tracker/templates/dj_tracker/query.html
 src/dj_tracker/templates/dj_tracker/query_group.html
-src/dj_tracker/templates/dj_tracker/queryset_tracking.html
+src/dj_tracker/templates/dj_tracker/query_groups.html
 src/dj_tracker/templates/dj_tracker/requests.html
-src/dj_tracker/templates/dj_tracker/url_trackings.html
+src/dj_tracker/templates/dj_tracker/includes/listing.html
+src/dj_tracker/templates/dj_tracker/includes/pagination.html
+src/dj_tracker/templates/dj_tracker/includes/query.html
 src/dj_tracker/templatetags/__init__.py
 src/dj_tracker/templatetags/dj_tracker.py
 src/dj_tracker/test/__init__.py
```

