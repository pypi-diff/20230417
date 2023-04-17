# Comparing `tmp/skip-django-pynotify-0.5.5.1.tar.gz` & `tmp/skip-django-pynotify-0.5.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-pynotify-0.5.5.1.tar", last modified: Wed Jan 18 23:39:07 2023, max compression
+gzip compressed data, was "skip-django-pynotify-0.5.5.2.tar", last modified: Mon Apr 17 11:54:22 2023, max compression
```

## Comparing `skip-django-pynotify-0.5.5.1.tar` & `skip-django-pynotify-0.5.5.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 23:39:07.332871 skip-django-pynotify-0.5.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-01-18 23:39:07.332871 skip-django-pynotify-0.5.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 23:39:07.328871 skip-django-pynotify-0.5.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3648 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/docs/example_project.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/docs/extra_tips.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/docs/history.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 23:39:07.328871 skip-django-pynotify-0.5.5.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/docs/images/pipeline.svg
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 23:39:07.332871 skip-django-pynotify-0.5.5.1/pynotify/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/dispatchers.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 23:39:07.328871 skip-django-pynotify-0.5.5.1/pynotify/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 23:39:07.328871 skip-django-pynotify-0.5.5.1/pynotify/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 23:39:07.332871 skip-django-pynotify-0.5.5.1/pynotify/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 23:39:07.332871 skip-django-pynotify-0.5.5.1/pynotify/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/migrations/0002_notification_extra_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/migrations/0003_related_object_name_not_required.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/migrations/0004_add_admin_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/migrations/0005_adminnotificationtemplate_is_active.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/migrations/0006_add_send_push.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/migrations/0007_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/migrations/0008_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/migrations/0009_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/notify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/receivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/pynotify/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-18 23:39:07.332871 skip-django-pynotify-0.5.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-01-18 23:38:52.000000 skip-django-pynotify-0.5.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 23:39:07.332871 skip-django-pynotify-0.5.5.1/skip_django_pynotify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-01-18 23:39:07.000000 skip-django-pynotify-0.5.5.1/skip_django_pynotify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-01-18 23:39:07.000000 skip-django-pynotify-0.5.5.1/skip_django_pynotify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 23:39:07.000000 skip-django-pynotify-0.5.5.1/skip_django_pynotify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 23:39:07.000000 skip-django-pynotify-0.5.5.1/skip_django_pynotify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-18 23:39:07.000000 skip-django-pynotify-0.5.5.1/skip_django_pynotify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-18 23:39:07.000000 skip-django-pynotify-0.5.5.1/skip_django_pynotify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.427822 skip-django-pynotify-0.5.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-17 11:54:22.427822 skip-django-pynotify-0.5.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.423822 skip-django-pynotify-0.5.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3648 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/example_project.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/extra_tips.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/history.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.423822 skip-django-pynotify-0.5.5.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/images/pipeline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.427822 skip-django-pynotify-0.5.5.2/pynotify/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/dispatchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.419822 skip-django-pynotify-0.5.5.2/pynotify/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.419822 skip-django-pynotify-0.5.5.2/pynotify/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.427822 skip-django-pynotify-0.5.5.2/pynotify/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.427822 skip-django-pynotify-0.5.5.2/pynotify/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0002_notification_extra_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0003_related_object_name_not_required.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0004_add_admin_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0005_adminnotificationtemplate_is_active.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0006_add_send_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0007_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0008_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/0009_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/notify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/pynotify/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-17 11:54:22.431822 skip-django-pynotify-0.5.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-17 11:54:11.000000 skip-django-pynotify-0.5.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:54:22.427822 skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-17 11:54:22.000000 skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-17 11:54:22.000000 skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:54:22.000000 skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:54:22.000000 skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 11:54:22.000000 skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 11:54:22.000000 skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/top_level.txt
```

### Comparing `skip-django-pynotify-0.5.5.1/CONTRIBUTING.rst` & `skip-django-pynotify-0.5.5.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/HISTORY.rst` & `skip-django-pynotify-0.5.5.2/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+Not released yet
+----------------
+
+* Add support for custom Notification model specification.
+
 0.5.5 (2023-01-03)
 ------------------
 
 * Add support for Python 3.10 and 3.11
 
 0.5.4 (2022-03-10)
 ------------------
```

### Comparing `skip-django-pynotify-0.5.5.1/LICENSE` & `skip-django-pynotify-0.5.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/PKG-INFO` & `skip-django-pynotify-0.5.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-pynotify
-Version: 0.5.5.1
+Version: 0.5.5.2
 Summary: General purpose notification library for Django
 Home-page: https://github.com/skip-pay/django-pynotify
 Author: Ondřej Kulatý
 Author-email: kulaty.o@gmail.com
 License: MIT license
 Keywords: django-pynotify
 Classifier: Development Status :: 3 - Alpha
@@ -66,14 +66,19 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+Not released yet
+----------------
+
+* Add support for custom Notification model specification.
+
 0.5.5 (2023-01-03)
 ------------------
 
 * Add support for Python 3.10 and 3.11
 
 0.5.4 (2022-03-10)
 ------------------
```

### Comparing `skip-django-pynotify-0.5.5.1/README.rst` & `skip-django-pynotify-0.5.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/docs/Makefile` & `skip-django-pynotify-0.5.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/docs/conf.py` & `skip-django-pynotify-0.5.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/docs/configuration.rst` & `skip-django-pynotify-0.5.5.2/docs/configuration.rst`

 * *Files 7% similar despite different names*

```diff
@@ -41,7 +41,11 @@
 * ``PYNOTIFY_TEMPLATE_PREFIX`` (default: ``''``)
 
     String that is prepended to any template just before rendering. Can be used to load custom tags/filters.
 
 * ``PYNOTIFY_TEMPLATE_TRANSLATE`` (default: ``False``)
 
     Boolean indicating if template string should be translated via ``gettext()`` before rendering.
+
+* ``PYNOTIFY_NOTIFICATION_MODEL`` (default: ``pynotify.Notification``)
+
+    String specifying a custom Notification model in '<app>.<model>' format. Currently, only proxy models are supported.
```

### Comparing `skip-django-pynotify-0.5.5.1/docs/example_project.rst` & `skip-django-pynotify-0.5.5.2/docs/example_project.rst`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/docs/extra_tips.rst` & `skip-django-pynotify-0.5.5.2/docs/extra_tips.rst`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/docs/images/pipeline.svg` & `skip-django-pynotify-0.5.5.2/docs/images/pipeline.svg`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/docs/installation.rst` & `skip-django-pynotify-0.5.5.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/docs/reference.rst` & `skip-django-pynotify-0.5.5.2/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/docs/usage.rst` & `skip-django-pynotify-0.5.5.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/pynotify/config.py` & `skip-django-pynotify-0.5.5.2/pynotify/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from django.conf import settings as django_settings
 
 
 class Settings:
     """
-    Holds default configuration values, the values can be overriden in settings with ``PYNOTIFY_`` prefix.
+    Holds default configuration values, the values can be overridden in settings with ``PYNOTIFY_`` prefix.
     """
     PREFIX = 'PYNOTIFY'
     DEFAULTS = {
         'AUTOLOAD_MODULES': None,
         'CELERY_TASK': 'pynotify.tasks.notification_task',
         'ENABLED': True,
+        'NOTIFICATION_MODEL': 'pynotify.Notification',
         'RECEIVER': 'pynotify.receivers.SynchronousReceiver',
         'RELATED_OBJECTS_ALLOWED_ATTRIBUTES': {'get_absolute_url', },
         'STRIP_HTML': False,
         'TEMPLATE_CHECK': False,
         'TEMPLATE_PREFIX': '',
         'TEMPLATE_TRANSLATE': False,
     }
```

### Comparing `skip-django-pynotify-0.5.5.1/pynotify/handlers.py` & `skip-django-pynotify-0.5.5.2/pynotify/handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections.abc import Iterable
 
 from django.core.exceptions import ImproperlyConfigured
 from django.utils.functional import cached_property
 
-from .helpers import register
-from .models import AdminNotificationTemplate, Notification, NotificationTemplate
+from .helpers import get_notification_model, register
+from .models import AdminNotificationTemplate, NotificationTemplate
 
 
 class HandlerMeta(type):
     """
     Registers handler for handling of signal defined in handler's ``Meta``.
     """
     def __new__(cls, name, bases, attrs):
@@ -98,15 +98,15 @@
         return True
 
     def _create_notification(self, recipient):
         """
         Creates notification for ``recipient``.
         """
         if self._can_create_notification(recipient):
-            return Notification.objects.create(
+            return get_notification_model().objects.create(
                 recipient=recipient,
                 template=self._template,
                 related_objects=self.get_related_objects(),
                 extra_data=self.get_extra_data(),
             )
 
     def _can_dispatch_notification(self, notification, dispatcher):
```

### Comparing `skip-django-pynotify-0.5.5.1/pynotify/locale/cs/LC_MESSAGES/django.mo` & `skip-django-pynotify-0.5.5.2/pynotify/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/pynotify/locale/cs/LC_MESSAGES/django.po` & `skip-django-pynotify-0.5.5.2/pynotify/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/pynotify/migrations/0001_initial.py` & `skip-django-pynotify-0.5.5.2/pynotify/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/pynotify/migrations/0004_add_admin_template.py` & `skip-django-pynotify-0.5.5.2/pynotify/migrations/0004_add_admin_template.py`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/pynotify/migrations/0008_migration.py` & `skip-django-pynotify-0.5.5.2/pynotify/migrations/0008_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/pynotify/models.py` & `skip-django-pynotify-0.5.5.2/pynotify/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/pynotify/notify.py` & `skip-django-pynotify-0.5.5.2/pynotify/notify.py`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/pynotify/receivers.py` & `skip-django-pynotify-0.5.5.2/pynotify/receivers.py`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/pynotify/serializers.py` & `skip-django-pynotify-0.5.5.2/pynotify/serializers.py`

 * *Files identical despite different names*

### Comparing `skip-django-pynotify-0.5.5.1/setup.py` & `skip-django-pynotify-0.5.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     license="MIT license",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='django-pynotify',
     name='skip-django-pynotify',
     packages=find_packages(include=['pynotify']),
     url='https://github.com/skip-pay/django-pynotify',
-    version='0.5.5.1',
+    version='0.5.5.2',
     zip_safe=False,
 )
```

### Comparing `skip-django-pynotify-0.5.5.1/skip_django_pynotify.egg-info/PKG-INFO` & `skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-pynotify
-Version: 0.5.5.1
+Version: 0.5.5.2
 Summary: General purpose notification library for Django
 Home-page: https://github.com/skip-pay/django-pynotify
 Author: Ondřej Kulatý
 Author-email: kulaty.o@gmail.com
 License: MIT license
 Keywords: django-pynotify
 Classifier: Development Status :: 3 - Alpha
@@ -66,14 +66,19 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+Not released yet
+----------------
+
+* Add support for custom Notification model specification.
+
 0.5.5 (2023-01-03)
 ------------------
 
 * Add support for Python 3.10 and 3.11
 
 0.5.4 (2022-03-10)
 ------------------
```

### Comparing `skip-django-pynotify-0.5.5.1/skip_django_pynotify.egg-info/SOURCES.txt` & `skip-django-pynotify-0.5.5.2/skip_django_pynotify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

