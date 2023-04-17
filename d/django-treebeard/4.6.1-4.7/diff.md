# Comparing `tmp/django-treebeard-4.6.1.tar.gz` & `tmp/django-treebeard-4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-treebeard-4.6.1.tar", last modified: Sun Feb  5 04:35:10 2023, max compression
+gzip compressed data, was "django-treebeard-4.7.tar", last modified: Mon Apr 17 06:38:23 2023, max compression
```

## Comparing `django-treebeard-4.6.1.tar` & `django-treebeard-4.7.tar`

### file list

```diff
@@ -1,129 +1,118 @@
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.071439 django-treebeard-4.6.1/
--rw-rw-r--   0 samir     (1000) samir     (1000)    11359 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/LICENSE
--rw-rw-r--   0 samir     (1000) samir     (1000)      278 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/MANIFEST.in
--rw-rw-r--   0 samir     (1000) samir     (1000)        0 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/NOTICE
--rw-rw-r--   0 samir     (1000) samir     (1000)     2611 2023-02-05 04:35:10.071439 django-treebeard-4.6.1/PKG-INFO
--rw-rw-r--   0 samir     (1000) samir     (1000)     1519 2022-12-24 03:55:12.000000 django-treebeard-4.6.1/README.md
--rw-rw-r--   0 samir     (1000) samir     (1000)      482 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/UPDATING
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.063439 django-treebeard-4.6.1/django_treebeard.egg-info/
--rw-rw-r--   0 samir     (1000) samir     (1000)     2611 2023-02-05 04:35:10.000000 django-treebeard-4.6.1/django_treebeard.egg-info/PKG-INFO
--rw-rw-r--   0 samir     (1000) samir     (1000)     3150 2023-02-05 04:35:10.000000 django-treebeard-4.6.1/django_treebeard.egg-info/SOURCES.txt
--rw-rw-r--   0 samir     (1000) samir     (1000)        1 2023-02-05 04:35:10.000000 django-treebeard-4.6.1/django_treebeard.egg-info/dependency_links.txt
--rw-rw-r--   0 samir     (1000) samir     (1000)       12 2023-02-05 04:35:10.000000 django-treebeard-4.6.1/django_treebeard.egg-info/requires.txt
--rw-rw-r--   0 samir     (1000) samir     (1000)       10 2023-02-05 04:35:10.000000 django-treebeard-4.6.1/django_treebeard.egg-info/top_level.txt
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.063439 django-treebeard-4.6.1/docs/
--rw-rw-r--   0 samir     (1000) samir     (1000)     7458 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/Makefile
--rw-rw-r--   0 samir     (1000) samir     (1000)      518 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/README.md
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.063439 django-treebeard-4.6.1/docs/build/
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.063439 django-treebeard-4.6.1/docs/build/html/
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.063439 django-treebeard-4.6.1/docs/build/html/_images/
--rw-rw-r--   0 samir     (1000) samir     (1000)   116531 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/build/html/_images/treebeard-admin-advanced.png
--rw-rw-r--   0 samir     (1000) samir     (1000)    96077 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/build/html/_images/treebeard-admin-basic.png
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.067439 django-treebeard-4.6.1/docs/build/html/_static/
--rw-rw-r--   0 samir     (1000) samir     (1000)      286 2022-12-24 05:50:23.000000 django-treebeard-4.6.1/docs/build/html/_static/file.png
--rw-rw-r--   0 samir     (1000) samir     (1000)       90 2022-12-24 05:50:23.000000 django-treebeard-4.6.1/docs/build/html/_static/minus.png
--rw-rw-r--   0 samir     (1000) samir     (1000)       90 2022-12-24 05:50:23.000000 django-treebeard-4.6.1/docs/build/html/_static/plus.png
--rw-rw-r--   0 samir     (1000) samir     (1000)   116531 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/build/html/_static/treebeard-admin-advanced.png
--rw-rw-r--   0 samir     (1000) samir     (1000)    96077 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/build/html/_static/treebeard-admin-basic.png
--rw-rw-r--   0 samir     (1000) samir     (1000)     7273 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/make.bat
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.067439 django-treebeard-4.6.1/docs/source/
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.067439 django-treebeard-4.6.1/docs/source/_ext/
--rw-rw-r--   0 samir     (1000) samir     (1000)      240 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/source/_ext/djangodocs.py
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.067439 django-treebeard-4.6.1/docs/source/_static/
--rw-rw-r--   0 samir     (1000) samir     (1000)   116531 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/source/_static/treebeard-admin-advanced.png
--rw-rw-r--   0 samir     (1000) samir     (1000)    96077 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/source/_static/treebeard-admin-basic.png
--rw-rw-r--   0 samir     (1000) samir     (1000)     1521 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/source/admin.rst
--rw-rw-r--   0 samir     (1000) samir     (1000)     3485 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/source/al_tree.rst
--rw-rw-r--   0 samir     (1000) samir     (1000)     8329 2022-12-24 03:22:49.000000 django-treebeard-4.6.1/docs/source/api.rst
--rw-rw-r--   0 samir     (1000) samir     (1000)     1691 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/source/caveats.rst
--rw-rw-r--   0 samir     (1000) samir     (1000)       51 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/source/changes.rst
--rw-rw-r--   0 samir     (1000) samir     (1000)     9825 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/source/conf.py
--rw-rw-r--   0 samir     (1000) samir     (1000)      245 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/source/exceptions.rst
--rw-rw-r--   0 samir     (1000) samir     (1000)      608 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/source/forms.rst
--rw-rw-r--   0 samir     (1000) samir     (1000)     1210 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/source/index.rst
--rw-rw-r--   0 samir     (1000) samir     (1000)     2086 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/source/install.rst
--rw-rw-r--   0 samir     (1000) samir     (1000)     8391 2023-01-02 03:54:54.000000 django-treebeard-4.6.1/docs/source/mp_tree.rst
--rw-rw-r--   0 samir     (1000) samir     (1000)     1753 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/docs/source/ns_tree.rst
--rw-rw-r--   0 samir     (1000) samir     (1000)     1448 2022-12-24 03:55:12.000000 django-treebeard-4.6.1/docs/source/tests.rst
--rw-rw-r--   0 samir     (1000) samir     (1000)     3427 2022-12-24 03:55:12.000000 django-treebeard-4.6.1/docs/source/tutorial.rst
--rw-rw-r--   0 samir     (1000) samir     (1000)       73 2023-02-05 04:35:10.071439 django-treebeard-4.6.1/setup.cfg
--rw-rw-r--   0 samir     (1000) samir     (1000)     1684 2023-01-02 04:12:44.000000 django-treebeard-4.6.1/setup.py
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.067439 django-treebeard-4.6.1/treebeard/
--rw-rw-r--   0 samir     (1000) samir     (1000)      598 2023-02-05 04:33:28.000000 django-treebeard-4.6.1/treebeard/__init__.py
--rw-rw-r--   0 samir     (1000) samir     (1000)     4750 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/admin.py
--rw-rw-r--   0 samir     (1000) samir     (1000)    13940 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/al_tree.py
--rw-rw-r--   0 samir     (1000) samir     (1000)      768 2022-12-24 03:55:12.000000 django-treebeard-4.6.1/treebeard/exceptions.py
--rw-rw-r--   0 samir     (1000) samir     (1000)     8143 2022-12-24 03:55:12.000000 django-treebeard-4.6.1/treebeard/forms.py
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.063439 django-treebeard-4.6.1/treebeard/locale/
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.063439 django-treebeard-4.6.1/treebeard/locale/de/
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.067439 django-treebeard-4.6.1/treebeard/locale/de/LC_MESSAGES/
--rw-rw-r--   0 samir     (1000) samir     (1000)     1669 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 samir     (1000) samir     (1000)     2370 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 samir     (1000) samir     (1000)      567 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/de/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 samir     (1000) samir     (1000)      921 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/de/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.063439 django-treebeard-4.6.1/treebeard/locale/es/
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.067439 django-treebeard-4.6.1/treebeard/locale/es/LC_MESSAGES/
--rw-rw-r--   0 samir     (1000) samir     (1000)      732 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 samir     (1000) samir     (1000)     1531 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/es/LC_MESSAGES/django.po
--rw-rw-r--   0 samir     (1000) samir     (1000)      374 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/es/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 samir     (1000) samir     (1000)      587 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/es/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.063439 django-treebeard-4.6.1/treebeard/locale/fr/
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.071439 django-treebeard-4.6.1/treebeard/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 samir     (1000) samir     (1000)     1654 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 samir     (1000) samir     (1000)     2407 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 samir     (1000) samir     (1000)      523 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/fr/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 samir     (1000) samir     (1000)      918 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/fr/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.063439 django-treebeard-4.6.1/treebeard/locale/hu/
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.071439 django-treebeard-4.6.1/treebeard/locale/hu/LC_MESSAGES/
--rwxrwxr-x   0 samir     (1000) samir     (1000)     1671 2022-12-24 03:55:12.000000 django-treebeard-4.6.1/treebeard/locale/hu/LC_MESSAGES/django.mo
--rwxrwxr-x   0 samir     (1000) samir     (1000)     2413 2022-12-24 03:55:12.000000 django-treebeard-4.6.1/treebeard/locale/hu/LC_MESSAGES/django.po
--rwxrwxr-x   0 samir     (1000) samir     (1000)      515 2022-12-24 03:55:12.000000 django-treebeard-4.6.1/treebeard/locale/hu/LC_MESSAGES/djangojs.mo
--rwxrwxr-x   0 samir     (1000) samir     (1000)      910 2022-12-24 03:55:12.000000 django-treebeard-4.6.1/treebeard/locale/hu/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.063439 django-treebeard-4.6.1/treebeard/locale/nl/
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.071439 django-treebeard-4.6.1/treebeard/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 samir     (1000) samir     (1000)     1512 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/nl/LC_MESSAGES/django.mo
--rw-rw-r--   0 samir     (1000) samir     (1000)     1845 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/nl/LC_MESSAGES/django.po
--rw-rw-r--   0 samir     (1000) samir     (1000)      532 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/nl/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 samir     (1000) samir     (1000)      660 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/nl/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.063439 django-treebeard-4.6.1/treebeard/locale/pl/
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.071439 django-treebeard-4.6.1/treebeard/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 samir     (1000) samir     (1000)      783 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 samir     (1000) samir     (1000)      880 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.063439 django-treebeard-4.6.1/treebeard/locale/ru/
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.071439 django-treebeard-4.6.1/treebeard/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 samir     (1000) samir     (1000)      874 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 samir     (1000) samir     (1000)     1676 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/ru/LC_MESSAGES/django.po
--rw-rw-r--   0 samir     (1000) samir     (1000)      445 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/ru/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 samir     (1000) samir     (1000)      661 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/locale/ru/LC_MESSAGES/djangojs.po
--rw-rw-r--   0 samir     (1000) samir     (1000)    21991 2023-01-02 03:54:59.000000 django-treebeard-4.6.1/treebeard/models.py
--rw-rw-r--   0 samir     (1000) samir     (1000)    46771 2023-02-05 04:15:52.000000 django-treebeard-4.6.1/treebeard/mp_tree.py
--rw-rw-r--   0 samir     (1000) samir     (1000)    25154 2023-01-02 05:32:16.000000 django-treebeard-4.6.1/treebeard/ns_tree.py
--rw-rw-r--   0 samir     (1000) samir     (1000)     3915 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/numconv.py
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.063439 django-treebeard-4.6.1/treebeard/static/
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.071439 django-treebeard-4.6.1/treebeard/static/treebeard/
--rw-rw-r--   0 samir     (1000) samir     (1000)     1020 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/static/treebeard/expand-collapse.png
--rw-rw-r--   0 samir     (1000) samir     (1000)     1416 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/static/treebeard/treebeard-admin.css
--rw-rw-r--   0 samir     (1000) samir     (1000)    15439 2023-01-02 03:54:59.000000 django-treebeard-4.6.1/treebeard/static/treebeard/treebeard-admin.js
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.063439 django-treebeard-4.6.1/treebeard/templates/
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.071439 django-treebeard-4.6.1/treebeard/templates/admin/
--rw-rw-r--   0 samir     (1000) samir     (1000)      756 2023-01-02 03:54:59.000000 django-treebeard-4.6.1/treebeard/templates/admin/tree_change_list.html
--rw-rw-r--   0 samir     (1000) samir     (1000)     1697 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/templates/admin/tree_change_list_results.html
--rw-rw-r--   0 samir     (1000) samir     (1000)      529 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/templates/admin/tree_list.html
--rw-rw-r--   0 samir     (1000) samir     (1000)      173 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/templates/admin/tree_list_results.html
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.071439 django-treebeard-4.6.1/treebeard/templatetags/
--rw-rw-r--   0 samir     (1000) samir     (1000)      259 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/templatetags/__init__.py
--rw-rw-r--   0 samir     (1000) samir     (1000)     8052 2023-01-02 03:54:59.000000 django-treebeard-4.6.1/treebeard/templatetags/admin_tree.py
--rw-rw-r--   0 samir     (1000) samir     (1000)     1581 2023-02-05 04:33:28.000000 django-treebeard-4.6.1/treebeard/templatetags/admin_tree_list.py
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.071439 django-treebeard-4.6.1/treebeard/tests/
--rw-rw-r--   0 samir     (1000) samir     (1000)        0 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/tests/__init__.py
--rw-rw-r--   0 samir     (1000) samir     (1000)      540 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/tests/admin.py
--rw-rw-r--   0 samir     (1000) samir     (1000)      257 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/tests/conftest.py
--rw-rw-r--   0 samir     (1000) samir     (1000)      258 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/tests/manage.py
-drwxrwxr-x   0 samir     (1000) samir     (1000)        0 2023-02-05 04:35:10.071439 django-treebeard-4.6.1/treebeard/tests/migrations/
--rw-rw-r--   0 samir     (1000) samir     (1000)    16440 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/tests/migrations/0001_initial.py
--rw-rw-r--   0 samir     (1000) samir     (1000)        0 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/tests/migrations/__init__.py
--rw-rw-r--   0 samir     (1000) samir     (1000)     7400 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/tests/models.py
--rw-rw-r--   0 samir     (1000) samir     (1000)     2913 2022-12-24 03:55:12.000000 django-treebeard-4.6.1/treebeard/tests/settings.py
--rw-rw-r--   0 samir     (1000) samir     (1000)     2183 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/tests/test_migrations.py
--rw-rw-r--   0 samir     (1000) samir     (1000)   106699 2023-02-05 04:33:28.000000 django-treebeard-4.6.1/treebeard/tests/test_treebeard.py
--rw-rw-r--   0 samir     (1000) samir     (1000)      140 2022-12-24 01:48:06.000000 django-treebeard-4.6.1/treebeard/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.747978 django-treebeard-4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-17 06:38:11.000000 django-treebeard-4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-17 06:38:11.000000 django-treebeard-4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:11.000000 django-treebeard-4.7/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-17 06:38:23.747978 django-treebeard-4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-17 06:38:11.000000 django-treebeard-4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-17 06:38:11.000000 django-treebeard-4.7/UPDATING
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.731978 django-treebeard-4.7/django_treebeard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-17 06:38:23.000000 django-treebeard-4.7/django_treebeard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-17 06:38:23.000000 django-treebeard-4.7/django_treebeard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 06:38:23.000000 django-treebeard-4.7/django_treebeard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 06:38:23.000000 django-treebeard-4.7/django_treebeard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 06:38:23.000000 django-treebeard-4.7/django_treebeard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.735978 django-treebeard-4.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.735978 django-treebeard-4.7/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.735978 django-treebeard-4.7/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/source/_ext/djangodocs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.735978 django-treebeard-4.7/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   116531 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/source/_static/treebeard-admin-advanced.png
+-rw-r--r--   0 runner    (1001) docker     (123)    96077 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/source/_static/treebeard-admin-basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/source/admin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/source/al_tree.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/source/caveats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/source/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/source/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/source/forms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/source/mp_tree.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/source/ns_tree.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/source/tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-17 06:38:11.000000 django-treebeard-4.7/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 06:38:23.747978 django-treebeard-4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-17 06:38:11.000000 django-treebeard-4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.735978 django-treebeard-4.7/treebeard/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/al_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.731978 django-treebeard-4.7/treebeard/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.731978 django-treebeard-4.7/treebeard/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.739978 django-treebeard-4.7/treebeard/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/de/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/de/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.731978 django-treebeard-4.7/treebeard/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.739978 django-treebeard-4.7/treebeard/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/es/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/es/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.731978 django-treebeard-4.7/treebeard/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.739978 django-treebeard-4.7/treebeard/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.731978 django-treebeard-4.7/treebeard/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.739978 django-treebeard-4.7/treebeard/locale/hu/LC_MESSAGES/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1671 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/hu/LC_MESSAGES/django.mo
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/hu/LC_MESSAGES/django.po
+-rwxr-xr-x   0 runner    (1001) docker     (123)      515 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/hu/LC_MESSAGES/djangojs.mo
+-rwxr-xr-x   0 runner    (1001) docker     (123)      910 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/hu/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.731978 django-treebeard-4.7/treebeard/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.739978 django-treebeard-4.7/treebeard/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/nl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/nl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.731978 django-treebeard-4.7/treebeard/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.739978 django-treebeard-4.7/treebeard/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.731978 django-treebeard-4.7/treebeard/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.739978 django-treebeard-4.7/treebeard/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/locale/ru/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 runner    (1001) docker     (123)    21991 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46771 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/mp_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25154 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/ns_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/numconv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.731978 django-treebeard-4.7/treebeard/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.739978 django-treebeard-4.7/treebeard/static/treebeard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/static/treebeard/expand-collapse.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/static/treebeard/treebeard-admin.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15439 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/static/treebeard/treebeard-admin.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.731978 django-treebeard-4.7/treebeard/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.743978 django-treebeard-4.7/treebeard/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/templates/admin/tree_change_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/templates/admin/tree_change_list_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/templates/admin/tree_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/templates/admin/tree_list_results.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.743978 django-treebeard-4.7/treebeard/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/templatetags/admin_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/templatetags/admin_tree_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.747978 django-treebeard-4.7/treebeard/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/tests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:23.747978 django-treebeard-4.7/treebeard/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106699 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/tests/test_treebeard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-17 06:38:11.000000 django-treebeard-4.7/treebeard/tests/urls.py
```

### Comparing `django-treebeard-4.6.1/LICENSE` & `django-treebeard-4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/PKG-INFO` & `django-treebeard-4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: django-treebeard
-Version: 4.6.1
+Version: 4.7
 Summary: Efficient tree implementations for Django
 Home-page: https://github.com/django-treebeard/django-treebeard/
 Author: Gustavo Picon
 Author-email: tabo@tabo.pe
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
@@ -63,12 +62,10 @@
 
 > <http://django-treebeard.readthedocs.io/en/latest/>
 
 ### Supported versions
 
 **django-treebeard** officially supports
 
--   Django 3.2, 4.0, 4.1
+-   Django 3.2, 4.1, 4.2
 -   Python 3.8 - 3.11
 -   PostgreSQL, MySQL, MSSQL, SQLite database back-ends.
-
-
```

### Comparing `django-treebeard-4.6.1/README.md` & `django-treebeard-4.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,10 +34,10 @@
 
 > <http://django-treebeard.readthedocs.io/en/latest/>
 
 ### Supported versions
 
 **django-treebeard** officially supports
 
--   Django 3.2, 4.0, 4.1
+-   Django 3.2, 4.1, 4.2
 -   Python 3.8 - 3.11
 -   PostgreSQL, MySQL, MSSQL, SQLite database back-ends.
```

### Comparing `django-treebeard-4.6.1/django_treebeard.egg-info/PKG-INFO` & `django-treebeard-4.7/django_treebeard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: django-treebeard
-Version: 4.6.1
+Version: 4.7
 Summary: Efficient tree implementations for Django
 Home-page: https://github.com/django-treebeard/django-treebeard/
 Author: Gustavo Picon
 Author-email: tabo@tabo.pe
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
@@ -63,12 +62,10 @@
 
 > <http://django-treebeard.readthedocs.io/en/latest/>
 
 ### Supported versions
 
 **django-treebeard** officially supports
 
--   Django 3.2, 4.0, 4.1
+-   Django 3.2, 4.1, 4.2
 -   Python 3.8 - 3.11
 -   PostgreSQL, MySQL, MSSQL, SQLite database back-ends.
-
-
```

### Comparing `django-treebeard-4.6.1/django_treebeard.egg-info/SOURCES.txt` & `django-treebeard-4.7/django_treebeard.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -9,21 +9,14 @@
 django_treebeard.egg-info/SOURCES.txt
 django_treebeard.egg-info/dependency_links.txt
 django_treebeard.egg-info/requires.txt
 django_treebeard.egg-info/top_level.txt
 docs/Makefile
 docs/README.md
 docs/make.bat
-docs/build/html/_images/treebeard-admin-advanced.png
-docs/build/html/_images/treebeard-admin-basic.png
-docs/build/html/_static/file.png
-docs/build/html/_static/minus.png
-docs/build/html/_static/plus.png
-docs/build/html/_static/treebeard-admin-advanced.png
-docs/build/html/_static/treebeard-admin-basic.png
 docs/source/admin.rst
 docs/source/al_tree.rst
 docs/source/api.rst
 docs/source/caveats.rst
 docs/source/changes.rst
 docs/source/conf.py
 docs/source/exceptions.rst
```

### Comparing `django-treebeard-4.6.1/docs/Makefile` & `django-treebeard-4.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/docs/README.md` & `django-treebeard-4.7/docs/README.md`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/docs/build/html/_images/treebeard-admin-advanced.png` & `django-treebeard-4.7/docs/source/_static/treebeard-admin-advanced.png`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/docs/build/html/_images/treebeard-admin-basic.png` & `django-treebeard-4.7/docs/source/_static/treebeard-admin-basic.png`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/docs/make.bat` & `django-treebeard-4.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/docs/source/admin.rst` & `django-treebeard-4.7/docs/source/admin.rst`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/docs/source/al_tree.rst` & `django-treebeard-4.7/docs/source/al_tree.rst`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/docs/source/api.rst` & `django-treebeard-4.7/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/docs/source/caveats.rst` & `django-treebeard-4.7/docs/source/caveats.rst`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/docs/source/conf.py` & `django-treebeard-4.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/docs/source/forms.rst` & `django-treebeard-4.7/docs/source/forms.rst`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/docs/source/index.rst` & `django-treebeard-4.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/docs/source/install.rst` & `django-treebeard-4.7/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/docs/source/mp_tree.rst` & `django-treebeard-4.7/docs/source/mp_tree.rst`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/docs/source/ns_tree.rst` & `django-treebeard-4.7/docs/source/ns_tree.rst`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/docs/source/tests.rst` & `django-treebeard-4.7/docs/source/tests.rst`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 tox
 ---
 
 ``django-treebeard`` uses `tox`_ to run the test suite in all the supported
 environments - permutations of:
 
   - Python 3.8 - 3.11
-  - Django 3.2, 4.0 and 4.1
+  - Django 3.2, 4.1 and 4.2
   - Sqlite, MySQL, PostgreSQL and MSSQL
 
 This means that there are a lot of permutations, which takes a long time.
 If you want to test only one or a few environments, use the `-e`
 option in `tox`_, like:
 
 .. code-block:: console
```

### Comparing `django-treebeard-4.6.1/docs/source/tutorial.rst` & `django-treebeard-4.7/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/setup.py` & `django-treebeard-4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Operating System :: OS Independent',
         'Topic :: Software Development :: Libraries',
```

### Comparing `django-treebeard-4.6.1/treebeard/__init__.py` & `django-treebeard-4.7/treebeard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
  9. python setup.py sdist bdist_wheel
 10. twine upload dist/*
 11. bump the version, append ".dev0" to __version__
 12. git add treebeard/__init__.py
 13. git commit -m 'Start with <version>'
 14. git push
 """
-__version__ = '4.6.1'
+__version__ = '4.7'
```

### Comparing `django-treebeard-4.6.1/treebeard/admin.py` & `django-treebeard-4.7/treebeard/admin.py`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/al_tree.py` & `django-treebeard-4.7/treebeard/al_tree.py`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/exceptions.py` & `django-treebeard-4.7/treebeard/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/forms.py` & `django-treebeard-4.7/treebeard/forms.py`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/de/LC_MESSAGES/django.mo` & `django-treebeard-4.7/treebeard/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/de/LC_MESSAGES/django.po` & `django-treebeard-4.7/treebeard/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/de/LC_MESSAGES/djangojs.mo` & `django-treebeard-4.7/treebeard/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/de/LC_MESSAGES/djangojs.po` & `django-treebeard-4.7/treebeard/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/es/LC_MESSAGES/django.mo` & `django-treebeard-4.7/treebeard/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/es/LC_MESSAGES/django.po` & `django-treebeard-4.7/treebeard/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/es/LC_MESSAGES/djangojs.po` & `django-treebeard-4.7/treebeard/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/fr/LC_MESSAGES/django.mo` & `django-treebeard-4.7/treebeard/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/fr/LC_MESSAGES/django.po` & `django-treebeard-4.7/treebeard/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/fr/LC_MESSAGES/djangojs.mo` & `django-treebeard-4.7/treebeard/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/fr/LC_MESSAGES/djangojs.po` & `django-treebeard-4.7/treebeard/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/hu/LC_MESSAGES/django.mo` & `django-treebeard-4.7/treebeard/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/hu/LC_MESSAGES/django.po` & `django-treebeard-4.7/treebeard/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/hu/LC_MESSAGES/djangojs.mo` & `django-treebeard-4.7/treebeard/locale/hu/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/hu/LC_MESSAGES/djangojs.po` & `django-treebeard-4.7/treebeard/locale/hu/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/nl/LC_MESSAGES/django.mo` & `django-treebeard-4.7/treebeard/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/nl/LC_MESSAGES/django.po` & `django-treebeard-4.7/treebeard/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/nl/LC_MESSAGES/djangojs.mo` & `django-treebeard-4.7/treebeard/locale/nl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/nl/LC_MESSAGES/djangojs.po` & `django-treebeard-4.7/treebeard/locale/nl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/pl/LC_MESSAGES/django.mo` & `django-treebeard-4.7/treebeard/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/pl/LC_MESSAGES/django.po` & `django-treebeard-4.7/treebeard/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/ru/LC_MESSAGES/django.mo` & `django-treebeard-4.7/treebeard/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/ru/LC_MESSAGES/django.po` & `django-treebeard-4.7/treebeard/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/locale/ru/LC_MESSAGES/djangojs.po` & `django-treebeard-4.7/treebeard/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/models.py` & `django-treebeard-4.7/treebeard/models.py`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/mp_tree.py` & `django-treebeard-4.7/treebeard/mp_tree.py`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/ns_tree.py` & `django-treebeard-4.7/treebeard/ns_tree.py`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/numconv.py` & `django-treebeard-4.7/treebeard/numconv.py`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/static/treebeard/expand-collapse.png` & `django-treebeard-4.7/treebeard/static/treebeard/expand-collapse.png`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/static/treebeard/treebeard-admin.css` & `django-treebeard-4.7/treebeard/static/treebeard/treebeard-admin.css`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/static/treebeard/treebeard-admin.js` & `django-treebeard-4.7/treebeard/static/treebeard/treebeard-admin.js`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/templates/admin/tree_change_list.html` & `django-treebeard-4.7/treebeard/templates/admin/tree_change_list.html`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/templates/admin/tree_change_list_results.html` & `django-treebeard-4.7/treebeard/templates/admin/tree_change_list_results.html`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/templates/admin/tree_list.html` & `django-treebeard-4.7/treebeard/templates/admin/tree_list.html`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/templatetags/admin_tree.py` & `django-treebeard-4.7/treebeard/templatetags/admin_tree.py`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/templatetags/admin_tree_list.py` & `django-treebeard-4.7/treebeard/templatetags/admin_tree_list.py`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/tests/admin.py` & `django-treebeard-4.7/treebeard/tests/admin.py`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/tests/migrations/0001_initial.py` & `django-treebeard-4.7/treebeard/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/tests/models.py` & `django-treebeard-4.7/treebeard/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/tests/settings.py` & `django-treebeard-4.7/treebeard/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/tests/test_migrations.py` & `django-treebeard-4.7/treebeard/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `django-treebeard-4.6.1/treebeard/tests/test_treebeard.py` & `django-treebeard-4.7/treebeard/tests/test_treebeard.py`

 * *Files identical despite different names*

