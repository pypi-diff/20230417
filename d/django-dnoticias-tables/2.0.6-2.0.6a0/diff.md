# Comparing `tmp/django_dnoticias_tables-2.0.6.tar.gz` & `tmp/django_dnoticias_tables-2.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/nelson/Development/dnoticias_tables/dist/.tmp-0qc2t0gq/django_dnoticias_tables-2.0.6.tar", last modified: Mon Apr 17 09:43:36 2023, max compression
+gzip compressed data, was "django_dnoticias_tables-2.0.6a0.tar", last modified: Wed Dec 21 14:48:46 2022, max compression
```

## Comparing `django_dnoticias_tables-2.0.6.tar` & `django_dnoticias_tables-2.0.6a0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     1082 2021-04-23 08:15:26.000000 django_dnoticias_tables-2.0.6/LICENSE
--rw-rw-r--   0 nelson    (1000) nelson    (1000)       80 2021-04-23 08:15:26.000000 django_dnoticias_tables-2.0.6/MANIFEST.in
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     8068 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/PKG-INFO
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     7050 2022-11-03 17:44:30.000000 django_dnoticias_tables-2.0.6/README.md
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     6997 2022-11-03 17:44:30.000000 django_dnoticias_tables-2.0.6/README.rst
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/django_dnoticias_tables.egg-info/
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     8068 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/django_dnoticias_tables.egg-info/PKG-INFO
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     2212 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/django_dnoticias_tables.egg-info/SOURCES.txt
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     1660 2022-11-04 11:26:33.000000 django_dnoticias_tables-2.0.6/django_dnoticias_tables.egg-info/SOURCES__.txt
--rw-rw-r--   0 nelson    (1000) nelson    (1000)        1 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/django_dnoticias_tables.egg-info/dependency_links.txt
--rw-rw-r--   0 nelson    (1000) nelson    (1000)        7 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/django_dnoticias_tables.egg-info/requires.txt
--rw-rw-r--   0 nelson    (1000) nelson    (1000)       17 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/django_dnoticias_tables.egg-info/top_level.txt
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/
--rw-rw-r--   0 nelson    (1000) nelson    (1000)        0 2022-04-21 15:14:30.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/__init__.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/__pycache__/
--rw-r--r--   0 nelson    (1000) nelson    (1000)     6237 2022-10-27 11:31:59.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/__pycache__/abstract_process.cpython-310.pyc
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     6248 2022-05-16 10:04:10.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/__pycache__/abstract_process.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      968 2022-09-20 15:00:18.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/__pycache__/order_object.cpython-310.pyc
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      982 2022-02-22 15:10:22.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/__pycache__/order_object.cpython-39.pyc
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     6292 2022-10-27 11:31:56.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/abstract_process.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      604 2021-04-23 08:15:26.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/order_object.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/__pycache__/
--rw-r--r--   0 nelson    (1000) nelson    (1000)     4131 2022-09-20 15:00:18.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/__pycache__/metronic_process.cpython-310.pyc
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     4147 2022-05-16 10:04:10.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/__pycache__/metronic_process.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)     3240 2022-09-20 15:00:18.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/__pycache__/process.cpython-310.pyc
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     3256 2022-05-16 10:04:10.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/__pycache__/process.cpython-39.pyc
--rw-r--r--   0 nelson    (1000) nelson    (1000)      534 2022-09-20 15:00:18.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/__pycache__/utils.cpython-310.pyc
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      548 2022-02-22 15:10:22.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/__pycache__/utils.cpython-39.pyc
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     3661 2022-04-21 15:14:14.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/metronic_process.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     2711 2022-04-21 14:49:48.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/process.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      326 2021-04-23 08:15:26.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/utils.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      106 2021-04-23 08:15:26.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/apps.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      675 2022-11-03 15:24:41.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/choices.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     5199 2023-04-17 09:41:10.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/columns.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     1122 2022-12-14 16:34:24.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/conf.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)    27472 2023-04-17 09:41:55.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/datatable.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     3973 2022-11-03 17:58:21.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/forms.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      794 2022-12-14 16:23:08.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/meta.py
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/templates/
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/includes/
--rw-rw-r--   0 nelson    (1000) nelson    (1000)        0 2022-10-28 10:56:56.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/includes/action.html
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     1857 2023-02-06 16:56:26.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/includes/column.html
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     7071 2023-02-08 12:23:30.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/includes/datatable.js
--rw-rw-r--   0 nelson    (1000) nelson    (1000)       94 2022-11-03 11:40:05.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/includes/datepicker.js
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     1129 2022-11-03 11:44:38.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/includes/daterange.js
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     3205 2022-10-28 14:20:47.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/includes/delete_popover.js
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      356 2022-10-27 11:45:38.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/includes/get_attributes.js
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      782 2022-10-27 11:44:38.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/includes/post.js
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      194 2022-10-27 11:45:18.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/includes/set_post_link.js
--rw-rw-r--   0 nelson    (1000) nelson    (1000)     4856 2023-02-08 12:23:03.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/list.html
-drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/templatetags/
--rw-rw-r--   0 nelson    (1000) nelson    (1000)        0 2022-10-28 10:22:22.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/templatetags/__init__.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      140 2022-10-31 12:23:17.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/templatetags/tables.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      729 2022-11-03 17:12:29.000000 django_dnoticias_tables-2.0.6/dnoticias_tables/utils.py
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      829 2023-04-17 09:43:36.000000 django_dnoticias_tables-2.0.6/setup.cfg
--rw-rw-r--   0 nelson    (1000) nelson    (1000)      843 2023-04-17 09:41:33.000000 django_dnoticias_tables-2.0.6/setup.py
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-12-21 14:48:46.205552 django_dnoticias_tables-2.0.6a0/
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     1082 2021-04-23 08:15:26.000000 django_dnoticias_tables-2.0.6a0/LICENSE
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)       80 2021-04-23 08:15:26.000000 django_dnoticias_tables-2.0.6a0/MANIFEST.in
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     8070 2022-12-21 14:48:46.205552 django_dnoticias_tables-2.0.6a0/PKG-INFO
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     7050 2022-11-03 17:44:30.000000 django_dnoticias_tables-2.0.6a0/README.md
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     6997 2022-11-03 17:44:30.000000 django_dnoticias_tables-2.0.6a0/README.rst
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-12-21 14:48:46.149552 django_dnoticias_tables-2.0.6a0/django_dnoticias_tables.egg-info/
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     8070 2022-12-21 14:48:46.000000 django_dnoticias_tables-2.0.6a0/django_dnoticias_tables.egg-info/PKG-INFO
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     2212 2022-12-21 14:48:46.000000 django_dnoticias_tables-2.0.6a0/django_dnoticias_tables.egg-info/SOURCES.txt
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     1660 2022-11-04 11:26:33.000000 django_dnoticias_tables-2.0.6a0/django_dnoticias_tables.egg-info/SOURCES__.txt
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)        1 2022-12-21 14:48:46.000000 django_dnoticias_tables-2.0.6a0/django_dnoticias_tables.egg-info/dependency_links.txt
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)        7 2022-12-21 14:48:46.000000 django_dnoticias_tables-2.0.6a0/django_dnoticias_tables.egg-info/requires.txt
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)       17 2022-12-21 14:48:46.000000 django_dnoticias_tables-2.0.6a0/django_dnoticias_tables.egg-info/top_level.txt
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-12-21 14:48:46.177552 django_dnoticias_tables-2.0.6a0/dnoticias_tables/
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)        0 2022-04-21 15:14:30.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/__init__.py
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-12-21 14:48:46.181552 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-12-21 14:48:46.185552 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/__pycache__/
+-rw-r--r--   0 nelson    (1000) nelson    (1000)     6237 2022-10-27 11:31:59.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/__pycache__/abstract_process.cpython-310.pyc
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     6248 2022-05-16 10:04:10.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/__pycache__/abstract_process.cpython-39.pyc
+-rw-r--r--   0 nelson    (1000) nelson    (1000)      968 2022-09-20 15:00:18.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/__pycache__/order_object.cpython-310.pyc
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      982 2022-02-22 15:10:22.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/__pycache__/order_object.cpython-39.pyc
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     6292 2022-10-27 11:31:56.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/abstract_process.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      604 2021-04-23 08:15:26.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/order_object.py
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-12-21 14:48:46.185552 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-12-21 14:48:46.189552 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/__pycache__/
+-rw-r--r--   0 nelson    (1000) nelson    (1000)     4131 2022-09-20 15:00:18.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/__pycache__/metronic_process.cpython-310.pyc
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     4147 2022-05-16 10:04:10.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/__pycache__/metronic_process.cpython-39.pyc
+-rw-r--r--   0 nelson    (1000) nelson    (1000)     3240 2022-09-20 15:00:18.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/__pycache__/process.cpython-310.pyc
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     3256 2022-05-16 10:04:10.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/__pycache__/process.cpython-39.pyc
+-rw-r--r--   0 nelson    (1000) nelson    (1000)      534 2022-09-20 15:00:18.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/__pycache__/utils.cpython-310.pyc
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      548 2022-02-22 15:10:22.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/__pycache__/utils.cpython-39.pyc
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     3661 2022-04-21 15:14:14.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/metronic_process.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     2711 2022-04-21 14:49:48.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/process.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      326 2021-04-23 08:15:26.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/utils.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      106 2021-04-23 08:15:26.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/apps.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      675 2022-11-03 15:24:41.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/choices.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     5032 2022-11-03 17:48:47.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/columns.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     1122 2022-12-14 16:34:24.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/conf.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)    27472 2022-12-19 15:04:03.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/datatable.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     3973 2022-11-03 17:58:21.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/forms.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      794 2022-12-14 16:23:08.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/meta.py
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-12-21 14:48:46.121552 django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-12-21 14:48:46.189552 django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-12-21 14:48:46.197552 django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/includes/
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)        0 2022-10-28 10:56:56.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/includes/action.html
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     1830 2022-12-14 16:25:54.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/includes/column.html
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     6876 2022-12-14 16:42:52.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/includes/datatable.js
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)       94 2022-11-03 11:40:05.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/includes/datepicker.js
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     1129 2022-11-03 11:44:38.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/includes/daterange.js
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     3205 2022-10-28 14:20:47.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/includes/delete_popover.js
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      356 2022-10-27 11:45:38.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/includes/get_attributes.js
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      782 2022-10-27 11:44:38.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/includes/post.js
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      194 2022-10-27 11:45:18.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/includes/set_post_link.js
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)     4855 2022-12-20 12:24:56.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/list.html
+drwxrwxr-x   0 nelson    (1000) nelson    (1000)        0 2022-12-21 14:48:46.205552 django_dnoticias_tables-2.0.6a0/dnoticias_tables/templatetags/
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)        0 2022-10-28 10:22:22.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/templatetags/__init__.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      140 2022-10-31 12:23:17.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/templatetags/tables.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      729 2022-11-03 17:12:29.000000 django_dnoticias_tables-2.0.6a0/dnoticias_tables/utils.py
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      829 2022-12-21 14:48:46.205552 django_dnoticias_tables-2.0.6a0/setup.cfg
+-rw-rw-r--   0 nelson    (1000) nelson    (1000)      844 2022-12-21 14:47:06.000000 django_dnoticias_tables-2.0.6a0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django_dnoticias_tables-2.0.6/LICENSE` & `django_dnoticias_tables-2.0.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/PKG-INFO` & `django_dnoticias_tables-2.0.6a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_dnoticias_tables
-Version: 2.0.6
+Version: 2.0.6a0
 Home-page: https://www.dnoticias.pt/
 Author: Pedro Mendes
 Author-email: pedro.trabalho.uma@gmail.com
 Maintainer: Nélson Gomes
 Maintainer-email: ngoncalves@dnoticias.pt
 License: MIT
 Classifier: Environment :: Web Environment
```

### Comparing `django_dnoticias_tables-2.0.6/README.md` & `django_dnoticias_tables-2.0.6a0/README.md`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/README.rst` & `django_dnoticias_tables-2.0.6a0/README.rst`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/django_dnoticias_tables.egg-info/PKG-INFO` & `django_dnoticias_tables-2.0.6a0/django_dnoticias_tables.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dnoticias-tables
-Version: 2.0.6
+Version: 2.0.6a0
 Home-page: https://www.dnoticias.pt/
 Author: Pedro Mendes
 Author-email: pedro.trabalho.uma@gmail.com
 Maintainer: Nélson Gomes
 Maintainer-email: ngoncalves@dnoticias.pt
 License: MIT
 Classifier: Environment :: Web Environment
```

### Comparing `django_dnoticias_tables-2.0.6/django_dnoticias_tables.egg-info/SOURCES.txt` & `django_dnoticias_tables-2.0.6a0/django_dnoticias_tables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/django_dnoticias_tables.egg-info/SOURCES__.txt` & `django_dnoticias_tables-2.0.6a0/django_dnoticias_tables.egg-info/SOURCES__.txt`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/__pycache__/abstract_process.cpython-310.pyc` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/__pycache__/abstract_process.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/__pycache__/abstract_process.cpython-39.pyc` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/__pycache__/abstract_process.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/__pycache__/order_object.cpython-310.pyc` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/__pycache__/order_object.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/__pycache__/order_object.cpython-39.pyc` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/__pycache__/order_object.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/abstract_process.py` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/abstract_process.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/order_object.py` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/order_object.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/__pycache__/metronic_process.cpython-310.pyc` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/__pycache__/metronic_process.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/__pycache__/metronic_process.cpython-39.pyc` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/__pycache__/metronic_process.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/__pycache__/process.cpython-310.pyc` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/__pycache__/process.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/__pycache__/process.cpython-39.pyc` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/__pycache__/process.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/__pycache__/utils.cpython-310.pyc` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/__pycache__/utils.cpython-39.pyc` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/metronic_process.py` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/metronic_process.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/abstract/relational/process.py` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/abstract/relational/process.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/choices.py` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/choices.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/columns.py` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/columns.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Any, Iterable, Optional, Type
 from dataclasses import dataclass
 from datetime import datetime
 
 from django.db.models.fields.files import FieldFile
 from django.views.generic import View
 from django.db.models import Model
-from django.utils import timezone
 
 from .choices import FilterType
 
 
 @dataclass
 class BaseColumn:
     name: Optional[str] = None
@@ -49,18 +48,15 @@
         :param view: The view that is rendering the table
         :return: The value for the field
         :rtype: Any
         """
         value = getattr(obj, field)
 
         if type(value) == datetime:
-            try:
-                value = timezone.localtime(value).strftime(self.datetime_format)
-            except ValueError:
-                value = value.strftime(self.datetime_format)
+            value = value.strftime(self.datetime_format)
         elif isinstance(value, FieldFile):
             value = value.url if value else None
 
         return value
 
 
 class ColumnMethod(BaseColumn):
```

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/conf.py` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/conf.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/datatable.py` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/datatable.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/forms.py` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/forms.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/meta.py` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/meta.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/includes/column.html` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/includes/column.html`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
     template: function (data, i) {
         console.log(data)
         {% if not column.is_action %}
         try{
             return get_{{column.field}}_html(data);
         } catch(e) {
-            console.log(e)
             return data.{{ column.field }};
         }
         {% else %}
         let action = "";
 
         {% for action in column.actions %}
         if(data.{{ action.identifier }}_show === true && data.{{ action.identifier }}_perm === true) {
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
 {% load tables %} {% if column.visible %} { field: "{{ column.field }}", title:
 "{{ column.name }}", width: {{ column.width }}, autoHide: "{{ column.auto_hide
 }}" == "True", sortable: "{{ column.sortable }}" == "True", textAlign: "{
 { column.align|default:'left' }}", template: function (data, i) { console.log
 (data) {% if not column.is_action %} try{ return get_{{column.field}}_html
-(data); } catch(e) { console.log(e) return data.{{ column.field }}; } {% else
-%} let action = ""; {% for action in column.actions %} if(data.{
-{ action.identifier }}_show === true && data.{{ action.identifier }}_perm ===
-true) { {% if not action.is_delete %} action += get_action_item({ url: data.{
-{ action.identifier }}_url, name: "{{ action.name }}", icon: "{{ action.icon
-}}", method: "{{ action.method }}", target: "{{ action.target }}", id:
-data.DT_RowId }); {% else %} action += get_delete_item({ name: "{{ action.name
-}}", url: data.{{ action.identifier }}_url, icon: "{{ action.icon }}", id:
-data.DT_RowId }) {% endif %} } {% endfor %} action = `
+(data); } catch(e) { return data.{{ column.field }}; } {% else %} let action =
+""; {% for action in column.actions %} if(data.{{ action.identifier }}_show ===
+true && data.{{ action.identifier }}_perm === true) { {% if not
+action.is_delete %} action += get_action_item({ url: data.{{ action.identifier
+}}_url, name: "{{ action.name }}", icon: "{{ action.icon }}", method: "{
+{ action.method }}", target: "{{ action.target }}", id: data.DT_RowId }); {%
+else %} action += get_delete_item({ name: "{{ action.name }}", url: data.{
+{ action.identifier }}_url, icon: "{{ action.icon }}", id: data.DT_RowId }) {%
+endif %} } {% endfor %} action = `
     * ${action}
 `; return `
 \
 ${action}
 `; {% endif %} } }, {% endif %}
```

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/includes/datatable.js` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/includes/datatable.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -172,19 +172,14 @@
             } {
                 % endfor %
             }]
         });
 
         datatable.on("kt-datatable--on-layout-updated", function(event, data) {
             setDeleteActionHandlers();
-
-            $('[data-toggle="kt-tooltip"]').each(function() {
-                KTApp.initTooltips();
-            });
-            document.dispatchEvent(new Event('kt-layout-updated'));
         });
     }
 
     return {
         init: function() {
             datatableEmailsList();
             var loading = new KTDialog({
```

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/includes/daterange.js` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/includes/daterange.js`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/includes/delete_popover.js` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/includes/delete_popover.js`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/includes/post.js` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/includes/post.js`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/templates/datatable/list.html` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/templates/datatable/list.html`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,14 @@
 <script>
     "use strict";
 
     jQuery(document).ready(function () {
         {% include "./includes/post.js" %}
         {% include "./includes/set_post_link.js" %}
         {% include "./includes/delete_popover.js" %}
-
         {% if extend_js %}
             {% include extended_filepath %}
         {% endif %}
 
         {% include "./includes/datatable.js" %}
 
         {% include "./includes/daterange.js" %}
```

### Comparing `django_dnoticias_tables-2.0.6/dnoticias_tables/utils.py` & `django_dnoticias_tables-2.0.6a0/dnoticias_tables/utils.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/setup.cfg` & `django_dnoticias_tables-2.0.6a0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_dnoticias_tables-2.0.6/setup.py` & `django_dnoticias_tables-2.0.6a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="django_dnoticias_tables",
-    version='2.0.6',
+    version='2.0.6a',
     url="https://www.dnoticias.pt/",
     author="Pedro Mendes",
     author_email="pedro.trabalho.uma@gmail.com",
     maintainer="Nélson Gomes",
     maintainer_email="ngoncalves@dnoticias.pt",
     license="MIT",
     long_description=long_description,
```

