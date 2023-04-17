# Comparing `tmp/django-sloth-0.0.54.tar.gz` & `tmp/django-sloth-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sloth-0.0.54.tar", last modified: Fri Feb 10 13:46:46 2023, max compression
+gzip compressed data, was "dist/django-sloth-0.1.0.tar", last modified: Mon Apr 17 19:06:29 2023, max compression
```

## Comparing `django-sloth-0.0.54.tar` & `django-sloth-0.1.0.tar`

### file list

```diff
@@ -1,294 +1,448 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.775104 django-sloth-0.0.54/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-10 13:46:40.000000 django-sloth-0.0.54/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-02-10 13:46:46.775104 django-sloth-0.0.54/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.751104 django-sloth-0.0.54/django_sloth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-02-10 13:46:46.000000 django-sloth-0.0.54/django_sloth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-02-10 13:46:46.000000 django-sloth-0.0.54/django_sloth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 13:46:46.000000 django-sloth-0.0.54/django_sloth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-10 13:46:46.000000 django-sloth-0.0.54/django_sloth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-10 13:46:46.000000 django-sloth-0.0.54/django_sloth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-10 13:46:40.000000 django-sloth-0.0.54/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 13:46:46.775104 django-sloth-0.0.54/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-02-10 13:46:40.000000 django-sloth-0.0.54/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.751104 django-sloth-0.0.54/sloth/
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.751104 django-sloth-0.0.54/sloth/actions/
--rw-r--r--   0 runner    (1001) docker     (123)    28741 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/actions/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/actions/inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.751104 django-sloth-0.0.54/sloth/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.751104 django-sloth-0.0.54/sloth/api/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.751104 django-sloth-0.0.54/sloth/api/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.751104 django-sloth-0.0.54/sloth/api/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/management/commands/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/management/commands/reset_passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/management/commands/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/management/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/management/commands/sync_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.751104 django-sloth-0.0.54/sloth/api/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/migrations/0002_role_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/migrations/0003_alter_application_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/migrations/0004_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/migrations/0005_task_stopped_alter_task_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/migrations/0009_pushnotification.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/migrations/0010_alter_pushnotification_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/migrations/0011_alter_application_client_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/migrations/0012_authcode.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/migrations/0013_task_partial_task_total.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.747104 django-sloth-0.0.54/sloth/api/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.751104 django-sloth-0.0.54/sloth/api/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/static/js/api.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.747104 django-sloth-0.0.54/sloth/api/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.751104 django-sloth-0.0.54/sloth/api/templates/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/templates/api/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/api/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.751104 django-sloth-0.0.54/sloth/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.751104 django-sloth-0.0.54/sloth/app/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.755104 django-sloth-0.0.54/sloth/app/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/management/commands/selenium.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/management/commands/undeploy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.755104 django-sloth-0.0.54/sloth/app/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.755104 django-sloth-0.0.54/sloth/app/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/css/all.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/css/bootstrap-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/css/colorpick.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.755104 django-sloth-0.0.54/sloth/app/static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   111976 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    83304 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/css/icons.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.755104 django-sloth-0.0.54/sloth/app/static/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/css/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/css/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/css/jquery-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/css/leaflet.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/css/sloth.css
--rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/css/trumbowyg.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.747104 django-sloth-0.0.54/sloth/app/static/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.755104 django-sloth-0.0.54/sloth/app/static/icons/fontawesome/
--rw-r--r--   0 runner    (1001) docker     (123)   100170 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/icons/fontawesome/fontawesome.min.css
--rw-r--r--   0 runner    (1001) docker     (123)  1726692 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/icons/fontawesome/fontawesome.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.759104 django-sloth-0.0.54/sloth/app/static/icons/fontawesome/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/icons/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/icons/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/icons/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/icons/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.759104 django-sloth-0.0.54/sloth/app/static/icons/materialicons/
--rw-r--r--   0 runner    (1001) docker     (123)   174176 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   127220 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   155604 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/icons/materialicons/materialicons.css
--rw-r--r--   0 runner    (1001) docker     (123)   135988 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.759104 django-sloth-0.0.54/sloth/app/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    57420 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/images/click.png
--rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/images/hand.png
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/images/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.759104 django-sloth-0.0.54/sloth/app/static/images/images/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/images/images/badge.png
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/images/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/images/login.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    22817 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/images/no-image.png
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/images/sloth.png
--rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/images/user.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.763104 django-sloth-0.0.54/sloth/app/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/bootstrap.bundle.min.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     4098 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/colorpick.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.763104 django-sloth-0.0.54/sloth/app/static/js/i18n/
--rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/i18n/pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   520714 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/jquery.binarytransport.js
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/jquery.mask.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    80794 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/jquery.timepicker.js
--rw-r--r--   0 runner    (1001) docker     (123)   147555 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/leaflet.js
--rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/masonry.pkgd.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    43994 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/qr-scanner-worker.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/qr-scanner.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/qrcode.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18264 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/sloth.js
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/sw.js
--rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/tests.js
--rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/js/trumbowyg.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/report.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.747104 django-sloth-0.0.54/sloth/app/static/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.763104 django-sloth-0.0.54/sloth/app/static/themes/blue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.763104 django-sloth-0.0.54/sloth/app/static/themes/blue/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   115080 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/themes/blue/fonts/rawline-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)   121132 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/themes/blue/fonts/rawline-400i.woff
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/static/themes/blue/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.747104 django-sloth-0.0.54/sloth/app/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.767104 django-sloth-0.0.54/sloth/app/templates/app/
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.767104 django-sloth-0.0.54/sloth/app/templates/app/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/charts/bar.html
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/charts/column.html
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/charts/donut.html
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/charts/legend.html
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/charts/pie.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.767104 django-sloth-0.0.54/sloth/app/templates/app/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/dashboard/apps.html
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/dashboard/bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/dashboard/cards.html
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/dashboard/dashboards.html
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/dashboard/grids.html
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/dashboard/header.html
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/dashboard/links.html
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/dashboard/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/dashboard/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/dashboard/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/dashboard/shortcuts.html
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/dashboard/tools.html
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/default.html
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/form.html
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.767104 django-sloth-0.0.54/sloth/app/templates/app/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/inputs/picker.html
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/inputs/qrcode.html
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/list.html
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/messages.html
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/modal.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.767104 django-sloth-0.0.54/sloth/app/templates/app/queryset/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/queryset/accordion.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.767104 django-sloth-0.0.54/sloth/app/templates/app/queryset/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/queryset/actions/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/queryset/actions/batch.html
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/queryset/actions/global.html
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/queryset/calendar.html
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/queryset/cards.html
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/queryset/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/queryset/datatable.html
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/queryset/filter.html
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/queryset/filters.html
--rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/queryset/filters2.html
--rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/queryset/queryset.html
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/queryset/rows.html
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/queryset/timeline.html
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/report.html
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/select.html
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/statistics.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.767104 django-sloth-0.0.54/sloth/app/templates/app/themes/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/themes/dark.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.771104 django-sloth-0.0.54/sloth/app/templates/app/valueset/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/valueset/field.html
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/valueset/fieldset-group.html
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/valueset/fieldset-list.html
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/valueset/fieldset-tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/valueset/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/valueset/primitive.html
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/valueset/value.html
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/valueset/valueset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.771104 django-sloth-0.0.54/sloth/app/templates/app/views/
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/views/icons.html
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/views/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/app/views/roles.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.747104 django-sloth-0.0.54/sloth/app/templates/renderers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.771104 django-sloth-0.0.54/sloth/app/templates/renderers/badges/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/badges/badge.html
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/badges/boolean.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/badges/status.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.771104 django-sloth-0.0.54/sloth/app/templates/renderers/calendar/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/calendar/calendar.html
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/calendar/events.html
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/calendar/legend.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.771104 django-sloth-0.0.54/sloth/app/templates/renderers/documents/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/documents/document.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.771104 django-sloth-0.0.54/sloth/app/templates/renderers/images/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/images/banner.html
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/images/image.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.771104 django-sloth-0.0.54/sloth/app/templates/renderers/links/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/links/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/links/url.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.771104 django-sloth-0.0.54/sloth/app/templates/renderers/maps/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/maps/geolocation.html
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/maps/map.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.771104 django-sloth-0.0.54/sloth/app/templates/renderers/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/messages/custom.html
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/messages/danger.html
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/messages/message.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/messages/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/messages/success.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/messages/warning.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.771104 django-sloth-0.0.54/sloth/app/templates/renderers/photos/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/photos/photo.html
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/photos/round.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.771104 django-sloth-0.0.54/sloth/app/templates/renderers/programing/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/programing/strtable.html
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/programing/terminal.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.771104 django-sloth-0.0.54/sloth/app/templates/renderers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/utils/formatted.html
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/utils/progress.html
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/utils/qrcode.html
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templates/renderers/utils/steps.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.771104 django-sloth-0.0.54/sloth/app/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/templatetags/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/app/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.771104 django-sloth-0.0.54/sloth/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.775104 django-sloth-0.0.54/sloth/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20053 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    31970 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/core/queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/core/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/core/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17769 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/core/valueset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14587 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.775104 django-sloth-0.0.54/sloth/db/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.775104 django-sloth-0.0.54/sloth/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/db/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.775104 django-sloth-0.0.54/sloth/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.775104 django-sloth-0.0.54/sloth/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.775104 django-sloth-0.0.54/sloth/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.775104 django-sloth-0.0.54/sloth/test/selenium/
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/test/selenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/test/selenium/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.775104 django-sloth-0.0.54/sloth/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.775104 django-sloth-0.0.54/sloth/utils/formatter/
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/utils/formatter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.775104 django-sloth-0.0.54/sloth/utils/http/
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/utils/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.775104 django-sloth-0.0.54/sloth/utils/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/utils/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/utils/icons/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    53105 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/utils/icons/fontawesome.py
--rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/utils/icons/materialicons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:46.775104 django-sloth-0.0.54/sloth/utils/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/utils/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-02-10 13:46:40.000000 django-sloth-0.0.54/sloth/utils/log/sql.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.533568 django-sloth-0.1.0/
+-rw-r--r--   0 breno      (503) staff       (20)       89 2022-09-21 16:56:21.000000 django-sloth-0.1.0/MANIFEST.in
+-rw-r--r--   0 breno      (503) staff       (20)      677 2023-04-17 19:06:29.533095 django-sloth-0.1.0/PKG-INFO
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.002196 django-sloth-0.1.0/django_sloth.egg-info/
+-rw-r--r--   0 breno      (503) staff       (20)      677 2023-04-17 19:06:28.000000 django-sloth-0.1.0/django_sloth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (503) staff       (20)    16348 2023-04-17 19:06:28.000000 django-sloth-0.1.0/django_sloth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (503) staff       (20)        1 2023-04-17 19:06:28.000000 django-sloth-0.1.0/django_sloth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (503) staff       (20)      209 2023-04-17 19:06:28.000000 django-sloth-0.1.0/django_sloth.egg-info/requires.txt
+-rw-r--r--   0 breno      (503) staff       (20)       13 2023-04-17 19:06:28.000000 django-sloth-0.1.0/django_sloth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (503) staff       (20)      190 2023-04-15 21:16:20.000000 django-sloth-0.1.0/requirements.txt
+-rw-r--r--   0 breno      (503) staff       (20)       38 2023-04-17 19:06:29.533790 django-sloth-0.1.0/setup.cfg
+-rw-r--r--   0 breno      (503) staff       (20)     1140 2023-04-17 13:26:06.000000 django-sloth-0.1.0/setup.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.005640 django-sloth-0.1.0/sloth/
+-rw-r--r--   0 breno      (503) staff       (20)     6148 2022-09-25 20:28:22.000000 django-sloth-0.1.0/sloth/.DS_Store
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.008489 django-sloth-0.1.0/sloth/.idea/
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.009456 django-sloth-0.1.0/sloth/.idea/inspectionProfiles/
+-rw-r--r--   0 breno      (503) staff       (20)      174 2022-04-14 14:03:07.000000 django-sloth-0.1.0/sloth/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 breno      (503) staff       (20)      262 2022-04-14 14:03:07.000000 django-sloth-0.1.0/sloth/.idea/modules.xml
+-rw-r--r--   0 breno      (503) staff       (20)      323 2022-04-14 14:06:53.000000 django-sloth-0.1.0/sloth/.idea/sloth.iml
+-rw-r--r--   0 breno      (503) staff       (20)      137 2022-04-14 14:03:07.000000 django-sloth-0.1.0/sloth/.idea/workspace.xml
+-rw-r--r--   0 breno      (503) staff       (20)      378 2023-04-15 21:16:31.000000 django-sloth-0.1.0/sloth/Dockerfile
+-rw-r--r--   0 breno      (503) staff       (20)     4272 2023-04-14 20:36:45.000000 django-sloth-0.1.0/sloth/__init__.py
+-rw-r--r--   0 breno      (503) staff       (20)     5341 2023-04-17 12:58:08.000000 django-sloth-0.1.0/sloth/__main__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.013519 django-sloth-0.1.0/sloth/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)     2420 2022-06-14 14:03:53.000000 django-sloth-0.1.0/sloth/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     4432 2023-04-14 21:08:20.000000 django-sloth-0.1.0/sloth/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     4945 2023-04-16 18:59:00.000000 django-sloth-0.1.0/sloth/__pycache__/__main__.cpython-38.pyc
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.017684 django-sloth-0.1.0/sloth/actions/
+-rw-r--r--   0 breno      (503) staff       (20)    36880 2023-04-16 22:26:32.000000 django-sloth-0.1.0/sloth/actions/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.027727 django-sloth-0.1.0/sloth/actions/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)    19031 2022-06-14 14:12:29.000000 django-sloth-0.1.0/sloth/actions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    26352 2023-04-16 22:26:34.000000 django-sloth-0.1.0/sloth/actions/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1561 2022-06-14 14:12:29.000000 django-sloth-0.1.0/sloth/actions/__pycache__/fields.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1641 2023-04-14 21:08:20.000000 django-sloth-0.1.0/sloth/actions/__pycache__/fields.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     3933 2022-06-14 14:12:29.000000 django-sloth-0.1.0/sloth/actions/__pycache__/inputs.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     3987 2023-04-14 21:08:20.000000 django-sloth-0.1.0/sloth/actions/__pycache__/inputs.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      770 2023-04-14 20:36:45.000000 django-sloth-0.1.0/sloth/actions/fields.py
+-rw-r--r--   0 breno      (503) staff       (20)     3189 2023-04-14 20:36:45.000000 django-sloth-0.1.0/sloth/actions/inputs.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.033826 django-sloth-0.1.0/sloth/api/
+-rw-r--r--   0 breno      (503) staff       (20)     2716 2022-09-21 16:56:21.000000 django-sloth-0.1.0/sloth/api/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.045017 django-sloth-0.1.0/sloth/api/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)     2062 2022-06-14 14:12:29.000000 django-sloth-0.1.0/sloth/api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     2071 2022-09-21 17:02:37.000000 django-sloth-0.1.0/sloth/api/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     3564 2022-06-14 14:12:38.000000 django-sloth-0.1.0/sloth/api/__pycache__/actions.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    22582 2023-04-16 22:32:05.000000 django-sloth-0.1.0/sloth/api/__pycache__/actions.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    13232 2023-04-16 18:31:19.000000 django-sloth-0.1.0/sloth/api/__pycache__/dashboard.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     9382 2022-06-14 14:12:30.000000 django-sloth-0.1.0/sloth/api/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    14269 2023-04-14 21:19:11.000000 django-sloth-0.1.0/sloth/api/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1879 2022-06-14 14:12:38.000000 django-sloth-0.1.0/sloth/api/__pycache__/urls.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1275 2023-04-14 21:19:11.000000 django-sloth-0.1.0/sloth/api/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     2871 2022-06-14 14:12:38.000000 django-sloth-0.1.0/sloth/api/__pycache__/views.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     7927 2023-04-16 18:31:19.000000 django-sloth-0.1.0/sloth/api/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    18644 2023-04-16 22:32:03.000000 django-sloth-0.1.0/sloth/api/actions.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.045901 django-sloth-0.1.0/sloth/api/backends/
+-rw-r--r--   0 breno      (503) staff       (20)      567 2021-11-16 15:14:56.000000 django-sloth-0.1.0/sloth/api/backends/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.046674 django-sloth-0.1.0/sloth/api/backends/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)     1198 2021-11-16 15:15:26.000000 django-sloth-0.1.0/sloth/api/backends/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    13994 2023-04-16 17:49:25.000000 django-sloth-0.1.0/sloth/api/dashboard.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.047440 django-sloth-0.1.0/sloth/api/exceptions/
+-rw-r--r--   0 breno      (503) staff       (20)      406 2023-04-14 20:36:45.000000 django-sloth-0.1.0/sloth/api/exceptions/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.048440 django-sloth-0.1.0/sloth/api/exceptions/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)     1193 2023-04-14 21:08:20.000000 django-sloth-0.1.0/sloth/api/exceptions/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.049344 django-sloth-0.1.0/sloth/api/management/
+-rw-r--r--   0 breno      (503) staff       (20)        0 2021-11-06 08:00:01.000000 django-sloth-0.1.0/sloth/api/management/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.050960 django-sloth-0.1.0/sloth/api/management/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)      165 2022-06-14 22:16:06.000000 django-sloth-0.1.0/sloth/api/management/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      182 2021-11-17 09:16:01.000000 django-sloth-0.1.0/sloth/api/management/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.061356 django-sloth-0.1.0/sloth/api/management/commands/
+-rw-r--r--   0 breno      (503) staff       (20)        0 2021-11-06 08:00:10.000000 django-sloth-0.1.0/sloth/api/management/commands/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.070530 django-sloth-0.1.0/sloth/api/management/commands/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)      174 2022-06-14 22:16:06.000000 django-sloth-0.1.0/sloth/api/management/commands/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      191 2021-11-17 09:16:01.000000 django-sloth-0.1.0/sloth/api/management/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1436 2023-04-17 12:54:57.000000 django-sloth-0.1.0/sloth/api/management/commands/__pycache__/cloud.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1229 2022-06-11 10:00:43.000000 django-sloth-0.1.0/sloth/api/management/commands/__pycache__/query.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      787 2023-04-14 19:27:15.000000 django-sloth-0.1.0/sloth/api/management/commands/__pycache__/reset_passwords.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     2078 2023-04-16 13:23:51.000000 django-sloth-0.1.0/sloth/api/management/commands/__pycache__/startserver.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1495 2022-06-14 22:16:06.000000 django-sloth-0.1.0/sloth/api/management/commands/__pycache__/sync.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1794 2023-04-16 11:53:16.000000 django-sloth-0.1.0/sloth/api/management/commands/__pycache__/sync.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      668 2023-04-13 08:38:15.000000 django-sloth-0.1.0/sloth/api/management/commands/__pycache__/sync_roles.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1093 2023-04-17 12:54:46.000000 django-sloth-0.1.0/sloth/api/management/commands/cloud.py
+-rw-r--r--   0 breno      (503) staff       (20)      600 2022-09-21 16:56:21.000000 django-sloth-0.1.0/sloth/api/management/commands/query.py
+-rw-r--r--   0 breno      (503) staff       (20)      366 2023-04-16 10:21:59.000000 django-sloth-0.1.0/sloth/api/management/commands/reset_passwords.py
+-rw-r--r--   0 breno      (503) staff       (20)      345 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/management/commands/selenium.py
+-rw-r--r--   0 breno      (503) staff       (20)      542 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/management/commands/send_web_push_notification.py
+-rw-r--r--   0 breno      (503) staff       (20)     1382 2023-04-16 13:25:26.000000 django-sloth-0.1.0/sloth/api/management/commands/startserver.py
+-rw-r--r--   0 breno      (503) staff       (20)     1391 2023-04-16 11:53:02.000000 django-sloth-0.1.0/sloth/api/management/commands/sync.py
+-rw-r--r--   0 breno      (503) staff       (20)      279 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/management/commands/sync_roles.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.089290 django-sloth-0.1.0/sloth/api/migrations/
+-rw-r--r--   0 breno      (503) staff       (20)     3069 2021-11-16 15:14:56.000000 django-sloth-0.1.0/sloth/api/migrations/0001_initial.py
+-rw-r--r--   0 breno      (503) staff       (20)     1961 2022-09-21 16:56:21.000000 django-sloth-0.1.0/sloth/api/migrations/0002_role_user.py
+-rw-r--r--   0 breno      (503) staff       (20)      632 2022-09-21 16:56:21.000000 django-sloth-0.1.0/sloth/api/migrations/0003_alter_application_user.py
+-rw-r--r--   0 breno      (503) staff       (20)     1330 2022-09-21 16:56:21.000000 django-sloth-0.1.0/sloth/api/migrations/0004_task.py
+-rw-r--r--   0 breno      (503) staff       (20)      586 2022-09-21 16:56:21.000000 django-sloth-0.1.0/sloth/api/migrations/0005_task_stopped_alter_task_message.py
+-rw-r--r--   0 breno      (503) staff       (20)     2379 2022-09-21 16:56:21.000000 django-sloth-0.1.0/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
+-rw-r--r--   0 breno      (503) staff       (20)      638 2022-09-21 16:56:21.000000 django-sloth-0.1.0/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
+-rw-r--r--   0 breno      (503) staff       (20)      694 2022-09-21 16:56:21.000000 django-sloth-0.1.0/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
+-rw-r--r--   0 breno      (503) staff       (20)      966 2022-09-21 16:56:21.000000 django-sloth-0.1.0/sloth/api/migrations/0009_pushnotification.py
+-rw-r--r--   0 breno      (503) staff       (20)      667 2022-09-21 16:56:21.000000 django-sloth-0.1.0/sloth/api/migrations/0010_alter_pushnotification_user.py
+-rw-r--r--   0 breno      (503) staff       (20)      634 2022-09-21 16:56:21.000000 django-sloth-0.1.0/sloth/api/migrations/0011_alter_application_client_secret.py
+-rw-r--r--   0 breno      (503) staff       (20)     1089 2022-09-25 21:01:42.000000 django-sloth-0.1.0/sloth/api/migrations/0012_authcode.py
+-rw-r--r--   0 breno      (503) staff       (20)      559 2023-02-02 00:42:42.000000 django-sloth-0.1.0/sloth/api/migrations/0013_task_partial_task_total.py
+-rw-r--r--   0 breno      (503) staff       (20)     1325 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/migrations/0014_email.py
+-rw-r--r--   0 breno      (503) staff       (20)        0 2021-11-16 15:14:56.000000 django-sloth-0.1.0/sloth/api/migrations/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.115038 django-sloth-0.1.0/sloth/api/migrations/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)     2457 2022-06-14 14:12:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     2476 2021-11-16 15:15:19.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0001_initial.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1640 2022-06-14 14:12:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0002_role_user.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1663 2022-09-21 17:02:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0002_role_user.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      843 2022-06-14 14:12:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0003_alter_application_user.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      860 2022-09-21 17:02:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0003_alter_application_user.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1282 2022-06-14 14:12:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0004_task.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1299 2022-09-21 17:02:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0004_task.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      733 2022-06-14 14:12:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0005_task_stopped_alter_task_message.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      750 2022-09-21 17:02:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0005_task_stopped_alter_task_message.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1460 2022-05-12 12:21:58.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0006_remove_role_scope_type_role_active_alter_role_name_and_more.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1561 2022-06-14 14:12:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0006_role_active_alter_role_name_alter_role_scope_key_and_more.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1578 2022-09-21 17:02:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0006_role_active_alter_role_name_alter_role_scope_key_and_more.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      715 2022-05-12 12:35:19.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0007_alter_role_scope_key.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      784 2022-06-14 14:12:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0007_alter_scope_description_alter_task_error.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      801 2022-09-21 17:02:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0007_alter_scope_description_alter_task_error.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      791 2022-06-14 14:12:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0008_alter_application_available_scopes_and_more.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      808 2022-09-21 17:02:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0008_alter_application_available_scopes_and_more.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1122 2022-09-21 17:02:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0009_pushnotification.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      914 2022-09-21 17:02:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0010_alter_pushnotification_user.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      883 2022-09-21 17:02:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0011_alter_application_client_secret.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      706 2022-09-01 11:30:34.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0011_task_partial_task_total.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1199 2022-09-26 16:01:37.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0012_authcode.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      684 2023-02-02 11:11:34.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0013_task_partial_task_total.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1297 2023-04-15 21:36:20.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/0014_email.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      165 2022-06-14 14:12:39.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      182 2021-11-16 15:15:19.000000 django-sloth-0.1.0/sloth/api/migrations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    11023 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/models.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:28.981928 django-sloth-0.1.0/sloth/api/static/
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.134036 django-sloth-0.1.0/sloth/api/static/css/
+-rw-r--r--   0 breno      (503) staff       (20)    58578 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/css/all.min.css
+-rw-r--r--   0 breno      (503) staff       (20)    67289 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/css/bootstrap-icons.css
+-rw-r--r--   0 breno      (503) staff       (20)   155845 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/css/bootstrap.min.css
+-rw-r--r--   0 breno      (503) staff       (20)      909 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/css/colorpick.min.css
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.147740 django-sloth-0.1.0/sloth/api/static/css/fonts/
+-rw-r--r--   0 breno      (503) staff       (20)   107280 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
+-rw-r--r--   0 breno      (503) staff       (20)   116316 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
+-rw-r--r--   0 breno      (503) staff       (20)   112880 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
+-rw-r--r--   0 breno      (503) staff       (20)   111976 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 breno      (503) staff       (20)    83304 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 breno      (503) staff       (20)    30702 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/css/icons.svg
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.151281 django-sloth-0.1.0/sloth/api/static/css/images/
+-rw-r--r--   0 breno      (503) staff       (20)     6992 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 breno      (503) staff       (20)     6988 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 breno      (503) staff       (20)    35973 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/css/jquery-ui.css
+-rw-r--r--   0 breno      (503) staff       (20)    14670 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/css/leaflet.css
+-rw-r--r--   0 breno      (503) staff       (20)    16264 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/css/select2.min.css
+-rw-r--r--   0 breno      (503) staff       (20)     8470 2023-04-17 09:56:47.000000 django-sloth-0.1.0/sloth/api/static/css/sloth.css
+-rw-r--r--   0 breno      (503) staff       (20)    17867 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/css/trumbowyg.min.css
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.153040 django-sloth-0.1.0/sloth/api/static/icons/
+-rw-r--r--   0 breno      (503) staff       (20)     6148 2022-06-09 17:07:18.000000 django-sloth-0.1.0/sloth/api/static/icons/.DS_Store
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.160345 django-sloth-0.1.0/sloth/api/static/icons/fontawesome/
+-rw-r--r--   0 breno      (503) staff       (20)     6148 2022-06-09 17:34:53.000000 django-sloth-0.1.0/sloth/api/static/icons/fontawesome/.DS_Store
+-rw-r--r--   0 breno      (503) staff       (20)   100170 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/icons/fontawesome/fontawesome.min.css
+-rw-r--r--   0 breno      (503) staff       (20)  1726692 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/icons/fontawesome/fontawesome.min.js
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.187831 django-sloth-0.1.0/sloth/api/static/icons/fontawesome/webfonts/
+-rw-r--r--   0 breno      (503) staff       (20)   181852 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 breno      (503) staff       (20)   105536 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 breno      (503) staff       (20)    60520 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 breno      (503) staff       (20)    23940 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 breno      (503) staff       (20)    10556 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 breno      (503) staff       (20)     4960 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.198698 django-sloth-0.1.0/sloth/api/static/icons/materialicons/
+-rw-r--r--   0 breno      (503) staff       (20)   174176 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
+-rw-r--r--   0 breno      (503) staff       (20)   127220 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
+-rw-r--r--   0 breno      (503) staff       (20)   155604 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
+-rw-r--r--   0 breno      (503) staff       (20)     2152 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/icons/materialicons/materialicons.css
+-rw-r--r--   0 breno      (503) staff       (20)   135988 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.223337 django-sloth-0.1.0/sloth/api/static/images/
+-rw-r--r--   0 breno      (503) staff       (20)     6148 2022-09-25 20:28:22.000000 django-sloth-0.1.0/sloth/api/static/images/.DS_Store
+-rw-r--r--   0 breno      (503) staff       (20)    57420 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/images/click.png
+-rw-r--r--   0 breno      (503) staff       (20)    55448 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/images/hand.png
+-rw-r--r--   0 breno      (503) staff       (20)    10276 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/images/icon.png
+-rw-r--r--   0 breno      (503) staff       (20)     2435 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/images/icon.svg
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.227252 django-sloth-0.1.0/sloth/api/static/images/images/
+-rw-r--r--   0 breno      (503) staff       (20)      706 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/images/images/badge.png
+-rw-r--r--   0 breno      (503) staff       (20)     1862 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/images/images/icon.png
+-rw-r--r--   0 breno      (503) staff       (20)    45136 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/images/login.jpeg
+-rw-r--r--   0 breno      (503) staff       (20)    22817 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/images/logo.png
+-rw-r--r--   0 breno      (503) staff       (20)     3866 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/images/logo.svg
+-rw-r--r--   0 breno      (503) staff       (20)    21495 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/images/no-image.png
+-rw-r--r--   0 breno      (503) staff       (20)    23102 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/images/sloth.png
+-rw-r--r--   0 breno      (503) staff       (20)    13670 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/images/user.png
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.296532 django-sloth-0.1.0/sloth/api/static/js/
+-rw-r--r--   0 breno      (503) staff       (20)    88459 2023-02-12 02:54:27.000000 django-sloth-0.1.0/sloth/api/static/js/USA.json
+-rw-r--r--   0 breno      (503) staff       (20)     3694 2022-09-21 16:56:21.000000 django-sloth-0.1.0/sloth/api/static/js/api.js
+-rw-r--r--   0 breno      (503) staff       (20)    78743 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/bootstrap.bundle.min.js
+-rwxr-xr-x   0 breno      (503) staff       (20)     4098 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/colorpick.min.js
+-rw-r--r--   0 breno      (503) staff       (20)  1022939 2022-12-09 19:31:21.000000 django-sloth-0.1.0/sloth/api/static/js/echarts.min.js
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.297931 django-sloth-0.1.0/sloth/api/static/js/i18n/
+-rwxr-xr-x   0 breno      (503) staff       (20)      853 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/i18n/pt-BR.js
+-rw-r--r--   0 breno      (503) staff       (20)    89501 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/jquery-3.6.0.min.js
+-rw-r--r--   0 breno      (503) staff       (20)   520714 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/jquery-ui.js
+-rw-r--r--   0 breno      (503) staff       (20)     2516 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/jquery.binarytransport.js
+-rw-r--r--   0 breno      (503) staff       (20)     8327 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/jquery.mask.min.js
+-rw-r--r--   0 breno      (503) staff       (20)    80794 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/jquery.timepicker.js
+-rw-r--r--   0 breno      (503) staff       (20)   147555 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/leaflet.js
+-rw-r--r--   0 breno      (503) staff       (20)    24103 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/masonry.pkgd.min.js
+-rw-r--r--   0 breno      (503) staff       (20)    18453 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/popper.min.js
+-rw-r--r--   0 breno      (503) staff       (20)    43994 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/qr-scanner-worker.min.js
+-rw-r--r--   0 breno      (503) staff       (20)    15538 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/qr-scanner.min.js
+-rw-r--r--   0 breno      (503) staff       (20)    19927 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (503) staff       (20)    73163 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/select2.min.js
+-rw-r--r--   0 breno      (503) staff       (20)    15700 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/sloth.js
+-rw-r--r--   0 breno      (503) staff       (20)      723 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/sw.js
+-rw-r--r--   0 breno      (503) staff       (20)    10702 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/tests.js
+-rw-r--r--   0 breno      (503) staff       (20)    28280 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/static/js/trumbowyg.min.js
+-rw-r--r--   0 breno      (503) staff       (20)     1943 2023-04-16 09:54:18.000000 django-sloth-0.1.0/sloth/api/static/js/wpn.js
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.299143 django-sloth-0.1.0/sloth/api/tasks/
+-rw-r--r--   0 breno      (503) staff       (20)     2263 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/tasks/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.300320 django-sloth-0.1.0/sloth/api/tasks/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)     2768 2023-04-14 21:19:12.000000 django-sloth-0.1.0/sloth/api/tasks/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:28.989833 django-sloth-0.1.0/sloth/api/templates/
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.303782 django-sloth-0.1.0/sloth/api/templates/actions/
+-rw-r--r--   0 breno      (503) staff       (20)      777 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/actions/execute_query.html
+-rw-r--r--   0 breno      (503) staff       (20)      153 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/actions/execute_script.html
+-rw-r--r--   0 breno      (503) staff       (20)     1216 2023-04-16 10:13:58.000000 django-sloth-0.1.0/sloth/api/templates/actions/show_icons.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.304843 django-sloth-0.1.0/sloth/api/templates/api/
+-rw-r--r--   0 breno      (503) staff       (20)     1034 2021-11-16 15:14:56.000000 django-sloth-0.1.0/sloth/api/templates/api/index.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.310545 django-sloth-0.1.0/sloth/api/templates/charts/
+-rw-r--r--   0 breno      (503) staff       (20)     1551 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/charts/bar.html
+-rw-r--r--   0 breno      (503) staff       (20)     3052 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/charts/column.html
+-rw-r--r--   0 breno      (503) staff       (20)       47 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/charts/donut.html
+-rw-r--r--   0 breno      (503) staff       (20)      283 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/charts/legend.html
+-rw-r--r--   0 breno      (503) staff       (20)     1267 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/charts/pie.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.338105 django-sloth-0.1.0/sloth/api/templates/dashboard/
+-rw-r--r--   0 breno      (503) staff       (20)     4237 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/actions.html
+-rw-r--r--   0 breno      (503) staff       (20)     1324 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/apps.html
+-rw-r--r--   0 breno      (503) staff       (20)     3125 2023-04-16 10:06:23.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/base.html
+-rw-r--r--   0 breno      (503) staff       (20)     2066 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/bottom.html
+-rw-r--r--   0 breno      (503) staff       (20)     1173 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/cards.html
+-rw-r--r--   0 breno      (503) staff       (20)      481 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/dashboards.html
+-rw-r--r--   0 breno      (503) staff       (20)      120 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/default.html
+-rw-r--r--   0 breno      (503) staff       (20)      727 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/footer.html
+-rw-r--r--   0 breno      (503) staff       (20)     6998 2023-04-17 13:05:33.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/form.html
+-rw-r--r--   0 breno      (503) staff       (20)      749 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/grids.html
+-rw-r--r--   0 breno      (503) staff       (20)     1665 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/header.html
+-rw-r--r--   0 breno      (503) staff       (20)      710 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/links.html
+-rw-r--r--   0 breno      (503) staff       (20)      434 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/menu.html
+-rw-r--r--   0 breno      (503) staff       (20)      764 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/messages.html
+-rw-r--r--   0 breno      (503) staff       (20)     1113 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/modal.html
+-rw-r--r--   0 breno      (503) staff       (20)      718 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/plus.html
+-rw-r--r--   0 breno      (503) staff       (20)     4304 2023-04-16 09:41:01.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/report.html
+-rw-r--r--   0 breno      (503) staff       (20)     1287 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/search.html
+-rw-r--r--   0 breno      (503) staff       (20)     1367 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/settings.html
+-rw-r--r--   0 breno      (503) staff       (20)      757 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/shortcuts.html
+-rw-r--r--   0 breno      (503) staff       (20)      838 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/tasks.html
+-rw-r--r--   0 breno      (503) staff       (20)      716 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/dashboard/tools.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.346927 django-sloth-0.1.0/sloth/api/templates/inputs/
+-rw-r--r--   0 breno      (503) staff       (20)      701 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/inputs/picker.html
+-rw-r--r--   0 breno      (503) staff       (20)     1009 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/inputs/qrcode.html
+-rw-r--r--   0 breno      (503) staff       (20)      924 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/inputs/select.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.360822 django-sloth-0.1.0/sloth/api/templates/queryset/
+-rw-r--r--   0 breno      (503) staff       (20)     1685 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/queryset/accordion.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.364093 django-sloth-0.1.0/sloth/api/templates/queryset/actions/
+-rw-r--r--   0 breno      (503) staff       (20)      153 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/queryset/actions/actions.html
+-rw-r--r--   0 breno      (503) staff       (20)      154 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/queryset/actions/batch.html
+-rw-r--r--   0 breno      (503) staff       (20)      145 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/queryset/actions/global.html
+-rw-r--r--   0 breno      (503) staff       (20)     4442 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/queryset/calendar.html
+-rw-r--r--   0 breno      (503) staff       (20)     1823 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/queryset/cards.html
+-rw-r--r--   0 breno      (503) staff       (20)      190 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/queryset/checkbox.html
+-rw-r--r--   0 breno      (503) staff       (20)     2332 2023-04-17 09:22:36.000000 django-sloth-0.1.0/sloth/api/templates/queryset/datatable.html
+-rw-r--r--   0 breno      (503) staff       (20)     2930 2023-04-16 10:09:10.000000 django-sloth-0.1.0/sloth/api/templates/queryset/filter.html
+-rw-r--r--   0 breno      (503) staff       (20)     3013 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/queryset/filters.html
+-rw-r--r--   0 breno      (503) staff       (20)     8811 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/queryset/queryset.html
+-rw-r--r--   0 breno      (503) staff       (20)     2297 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/queryset/rows.html
+-rw-r--r--   0 breno      (503) staff       (20)     1250 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/queryset/scroll.html
+-rw-r--r--   0 breno      (503) staff       (20)     5097 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/queryset/statistics.html
+-rw-r--r--   0 breno      (503) staff       (20)     4511 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/queryset/timeline.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:28.989392 django-sloth-0.1.0/sloth/api/templates/renderers/
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.369964 django-sloth-0.1.0/sloth/api/templates/renderers/badges/
+-rw-r--r--   0 breno      (503) staff       (20)      165 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/badges/badge.html
+-rw-r--r--   0 breno      (503) staff       (20)      385 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/badges/boolean.html
+-rw-r--r--   0 breno      (503) staff       (20)      143 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/badges/primary.html
+-rw-r--r--   0 breno      (503) staff       (20)      151 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/badges/status.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.371074 django-sloth-0.1.0/sloth/api/templates/renderers/boolean/
+-rw-r--r--   0 breno      (503) staff       (20)      101 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/boolean/thumb.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.373554 django-sloth-0.1.0/sloth/api/templates/renderers/calendar/
+-rw-r--r--   0 breno      (503) staff       (20)     1997 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/calendar/calendar.html
+-rw-r--r--   0 breno      (503) staff       (20)       36 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/calendar/events.html
+-rw-r--r--   0 breno      (503) staff       (20)      229 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/calendar/legend.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.375969 django-sloth-0.1.0/sloth/api/templates/renderers/documents/
+-rw-r--r--   0 breno      (503) staff       (20)       63 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/documents/document.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.378796 django-sloth-0.1.0/sloth/api/templates/renderers/images/
+-rw-r--r--   0 breno      (503) staff       (20)       62 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/images/banner.html
+-rw-r--r--   0 breno      (503) staff       (20)       61 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/images/image.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.381592 django-sloth-0.1.0/sloth/api/templates/renderers/links/
+-rw-r--r--   0 breno      (503) staff       (20)       77 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/links/file.html
+-rw-r--r--   0 breno      (503) staff       (20)      146 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/links/url.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.386534 django-sloth-0.1.0/sloth/api/templates/renderers/maps/
+-rw-r--r--   0 breno      (503) staff       (20)      292 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/maps/geolocation.html
+-rw-r--r--   0 breno      (503) staff       (20)     4551 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/maps/map.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.400077 django-sloth-0.1.0/sloth/api/templates/renderers/messages/
+-rw-r--r--   0 breno      (503) staff       (20)      113 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/messages/custom.html
+-rw-r--r--   0 breno      (503) staff       (20)       78 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/messages/danger.html
+-rw-r--r--   0 breno      (503) staff       (20)      126 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/messages/message.html
+-rw-r--r--   0 breno      (503) staff       (20)       79 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/messages/primary.html
+-rw-r--r--   0 breno      (503) staff       (20)       79 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/messages/success.html
+-rw-r--r--   0 breno      (503) staff       (20)       79 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/messages/warning.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.401634 django-sloth-0.1.0/sloth/api/templates/renderers/photos/
+-rw-r--r--   0 breno      (503) staff       (20)      131 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/photos/photo.html
+-rw-r--r--   0 breno      (503) staff       (20)      171 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/photos/round.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.403151 django-sloth-0.1.0/sloth/api/templates/renderers/programing/
+-rw-r--r--   0 breno      (503) staff       (20)      764 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/programing/strtable.html
+-rw-r--r--   0 breno      (503) staff       (20)      152 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/programing/terminal.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.404619 django-sloth-0.1.0/sloth/api/templates/renderers/tags/
+-rw-r--r--   0 breno      (503) staff       (20)      276 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/tags/primary.html
+-rw-r--r--   0 breno      (503) staff       (20)      287 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/tags/tags.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.408757 django-sloth-0.1.0/sloth/api/templates/renderers/utils/
+-rw-r--r--   0 breno      (503) staff       (20)       16 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/utils/formatted.html
+-rw-r--r--   0 breno      (503) staff       (20)      214 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/utils/progress.html
+-rw-r--r--   0 breno      (503) staff       (20)      323 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/utils/qrcode.html
+-rw-r--r--   0 breno      (503) staff       (20)     2000 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/utils/steps.html
+-rw-r--r--   0 breno      (503) staff       (20)      601 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/renderers/utils/table.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.409623 django-sloth-0.1.0/sloth/api/templates/themes/
+-rw-r--r--   0 breno      (503) staff       (20)      635 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/themes/dark.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.422479 django-sloth-0.1.0/sloth/api/templates/valueset/
+-rw-r--r--   0 breno      (503) staff       (20)      152 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/valueset/2-column.html
+-rw-r--r--   0 breno      (503) staff       (20)      459 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/valueset/field.html
+-rw-r--r--   0 breno      (503) staff       (20)     2668 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/valueset/fieldset-group.html
+-rw-r--r--   0 breno      (503) staff       (20)     2536 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/valueset/fieldset-list.html
+-rw-r--r--   0 breno      (503) staff       (20)      110 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/valueset/fieldset-tab.html
+-rw-r--r--   0 breno      (503) staff       (20)     2980 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/valueset/fieldset.html
+-rw-r--r--   0 breno      (503) staff       (20)       47 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/valueset/primitive.html
+-rw-r--r--   0 breno      (503) staff       (20)     1025 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/valueset/value.html
+-rw-r--r--   0 breno      (503) staff       (20)     5702 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templates/valueset/valueset.html
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.424403 django-sloth-0.1.0/sloth/api/templatetags/
+-rw-r--r--   0 breno      (503) staff       (20)      162 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templatetags/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.426197 django-sloth-0.1.0/sloth/api/templatetags/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)      335 2023-04-14 21:19:12.000000 django-sloth-0.1.0/sloth/api/templatetags/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    10005 2023-04-14 21:19:12.000000 django-sloth-0.1.0/sloth/api/templatetags/__pycache__/tags.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     9110 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/templatetags/tags.py
+-rw-r--r--   0 breno      (503) staff       (20)     1361 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/api/urls.py
+-rw-r--r--   0 breno      (503) staff       (20)    11104 2023-04-16 17:49:25.000000 django-sloth-0.1.0/sloth/api/views.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:28.990855 django-sloth-0.1.0/sloth/app/
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.430846 django-sloth-0.1.0/sloth/app/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)      173 2023-04-14 19:27:14.000000 django-sloth-0.1.0/sloth/app/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     2177 2023-04-14 19:27:15.000000 django-sloth-0.1.0/sloth/app/__pycache__/actions.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    11325 2023-04-14 19:27:15.000000 django-sloth-0.1.0/sloth/app/__pycache__/dashboard.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      804 2023-04-14 19:27:15.000000 django-sloth-0.1.0/sloth/app/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     7660 2023-04-14 19:27:15.000000 django-sloth-0.1.0/sloth/app/__pycache__/views.cpython-38.pyc
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:28.991011 django-sloth-0.1.0/sloth/app/templatetags/
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.432581 django-sloth-0.1.0/sloth/app/templatetags/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)      335 2023-04-14 19:27:15.000000 django-sloth-0.1.0/sloth/app/templatetags/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     9340 2023-04-14 19:27:15.000000 django-sloth-0.1.0/sloth/app/templatetags/__pycache__/tags.cpython-38.pyc
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.434468 django-sloth-0.1.0/sloth/cloud/
+-rw-r--r--   0 breno      (503) staff       (20)        0 2023-04-14 14:44:20.000000 django-sloth-0.1.0/sloth/cloud/__init__.py
+-rwxr-xr-x   0 breno      (503) staff       (20)     6046 2023-04-16 19:02:42.000000 django-sloth-0.1.0/sloth/cloud/server.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.436557 django-sloth-0.1.0/sloth/conf/
+-rw-r--r--   0 breno      (503) staff       (20)        0 2023-04-09 08:16:34.000000 django-sloth-0.1.0/sloth/conf/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.443778 django-sloth-0.1.0/sloth/conf/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)      174 2023-04-09 08:18:50.000000 django-sloth-0.1.0/sloth/conf/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     2478 2023-04-16 17:40:08.000000 django-sloth-0.1.0/sloth/conf/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     2873 2023-04-16 14:01:26.000000 django-sloth-0.1.0/sloth/conf/settings.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.452664 django-sloth-0.1.0/sloth/core/
+-rw-r--r--   0 breno      (503) staff       (20)        0 2022-09-27 13:29:31.000000 django-sloth-0.1.0/sloth/core/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.477211 django-sloth-0.1.0/sloth/core/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)      155 2022-06-14 14:12:29.000000 django-sloth-0.1.0/sloth/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      174 2022-09-27 15:59:51.000000 django-sloth-0.1.0/sloth/core/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    15741 2022-06-14 14:12:29.000000 django-sloth-0.1.0/sloth/core/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    18022 2023-04-17 01:59:55.000000 django-sloth-0.1.0/sloth/core/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    22470 2022-06-14 14:12:29.000000 django-sloth-0.1.0/sloth/core/__pycache__/queryset.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    28835 2023-04-17 09:43:40.000000 django-sloth-0.1.0/sloth/core/__pycache__/queryset.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     8627 2022-06-14 14:12:29.000000 django-sloth-0.1.0/sloth/core/__pycache__/statistics.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    10343 2023-04-14 21:08:20.000000 django-sloth-0.1.0/sloth/core/__pycache__/statistics.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     2033 2022-06-14 14:12:29.000000 django-sloth-0.1.0/sloth/core/__pycache__/validation.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     2058 2022-09-21 17:02:37.000000 django-sloth-0.1.0/sloth/core/__pycache__/validation.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    10034 2022-06-14 14:12:29.000000 django-sloth-0.1.0/sloth/core/__pycache__/valueset.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    14149 2023-04-14 21:08:20.000000 django-sloth-0.1.0/sloth/core/__pycache__/valueset.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     4555 2022-06-14 14:12:38.000000 django-sloth-0.1.0/sloth/core/__pycache__/views.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     3410 2023-04-14 19:27:15.000000 django-sloth-0.1.0/sloth/core/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    21312 2023-04-17 01:59:53.000000 django-sloth-0.1.0/sloth/core/base.py
+-rw-r--r--   0 breno      (503) staff       (20)    37888 2023-04-17 09:43:39.000000 django-sloth-0.1.0/sloth/core/queryset.py
+-rw-r--r--   0 breno      (503) staff       (20)    10195 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/core/statistics.py
+-rw-r--r--   0 breno      (503) staff       (20)     2012 2022-09-21 16:56:21.000000 django-sloth-0.1.0/sloth/core/validation.py
+-rw-r--r--   0 breno      (503) staff       (20)    19939 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/core/valueset.py
+-rw-r--r--   0 breno      (503) staff       (20)        0 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/core/views.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.480250 django-sloth-0.1.0/sloth/db/
+-rw-r--r--   0 breno      (503) staff       (20)      487 2023-04-11 17:54:19.000000 django-sloth-0.1.0/sloth/db/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.482896 django-sloth-0.1.0/sloth/db/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)     1035 2022-06-14 14:12:29.000000 django-sloth-0.1.0/sloth/db/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      713 2023-04-11 17:54:27.000000 django-sloth-0.1.0/sloth/db/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.483960 django-sloth-0.1.0/sloth/db/models/
+-rw-r--r--   0 breno      (503) staff       (20)     9656 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/db/models/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.491171 django-sloth-0.1.0/sloth/db/models/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)    11266 2022-06-14 14:12:30.000000 django-sloth-0.1.0/sloth/db/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    12806 2023-04-14 21:19:11.000000 django-sloth-0.1.0/sloth/db/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    12390 2021-11-16 14:44:03.000000 django-sloth-0.1.0/sloth/db/models/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     3365 2021-11-16 14:44:30.000000 django-sloth-0.1.0/sloth/db/models/__pycache__/model.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    14439 2021-11-16 14:02:52.000000 django-sloth-0.1.0/sloth/db/models/__pycache__/query.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     7433 2021-11-16 14:02:52.000000 django-sloth-0.1.0/sloth/db/models/__pycache__/statistics.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     6051 2021-11-16 14:11:38.000000 django-sloth-0.1.0/sloth/db/models/__pycache__/values.cpython-38.pyc
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:28.993783 django-sloth-0.1.0/sloth/exceptions/
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.491983 django-sloth-0.1.0/sloth/exceptions/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)     1189 2023-04-14 19:27:14.000000 django-sloth-0.1.0/sloth/exceptions/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.493071 django-sloth-0.1.0/sloth/test/
+-rw-r--r--   0 breno      (503) staff       (20)     3185 2023-04-14 19:26:19.000000 django-sloth-0.1.0/sloth/test/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.493938 django-sloth-0.1.0/sloth/test/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)     3555 2023-04-16 11:34:14.000000 django-sloth-0.1.0/sloth/test/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.495822 django-sloth-0.1.0/sloth/test/selenium/
+-rw-r--r--   0 breno      (503) staff       (20)     4489 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/test/selenium/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.498901 django-sloth-0.1.0/sloth/test/selenium/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)     7028 2023-04-16 11:34:14.000000 django-sloth-0.1.0/sloth/test/selenium/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     9598 2023-04-16 11:34:14.000000 django-sloth-0.1.0/sloth/test/selenium/__pycache__/browser.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    10057 2023-04-14 19:26:19.000000 django-sloth-0.1.0/sloth/test/selenium/browser.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.500185 django-sloth-0.1.0/sloth/utils/
+-rw-r--r--   0 breno      (503) staff       (20)     4213 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/utils/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.501990 django-sloth-0.1.0/sloth/utils/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)     3902 2022-06-14 14:12:29.000000 django-sloth-0.1.0/sloth/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     4115 2023-04-14 21:08:20.000000 django-sloth-0.1.0/sloth/utils/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.502707 django-sloth-0.1.0/sloth/utils/formatter/
+-rw-r--r--   0 breno      (503) staff       (20)     2170 2023-04-14 20:36:46.000000 django-sloth-0.1.0/sloth/utils/formatter/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.505756 django-sloth-0.1.0/sloth/utils/formatter/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)     2150 2022-06-14 14:12:38.000000 django-sloth-0.1.0/sloth/utils/formatter/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     2243 2023-04-14 21:08:20.000000 django-sloth-0.1.0/sloth/utils/formatter/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.506673 django-sloth-0.1.0/sloth/utils/http/
+-rw-r--r--   0 breno      (503) staff       (20)     5181 2023-04-16 09:41:30.000000 django-sloth-0.1.0/sloth/utils/http/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.508569 django-sloth-0.1.0/sloth/utils/http/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)     5222 2022-06-14 14:12:29.000000 django-sloth-0.1.0/sloth/utils/http/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     5549 2023-04-16 10:01:23.000000 django-sloth-0.1.0/sloth/utils/http/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.513298 django-sloth-0.1.0/sloth/utils/icons/
+-rw-r--r--   0 breno      (503) staff       (20)        0 2021-10-24 14:05:49.000000 django-sloth-0.1.0/sloth/utils/icons/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.527060 django-sloth-0.1.0/sloth/utils/icons/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)      162 2022-06-14 14:12:38.000000 django-sloth-0.1.0/sloth/utils/icons/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      157 2021-10-24 14:05:51.000000 django-sloth-0.1.0/sloth/utils/icons/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    20486 2022-06-14 14:12:38.000000 django-sloth-0.1.0/sloth/utils/icons/__pycache__/bootstrap.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    28423 2021-10-24 17:36:48.000000 django-sloth-0.1.0/sloth/utils/icons/__pycache__/bootstrap.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    38757 2022-06-14 14:12:39.000000 django-sloth-0.1.0/sloth/utils/icons/__pycache__/fontawesome.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    52818 2022-09-21 17:02:39.000000 django-sloth-0.1.0/sloth/utils/icons/__pycache__/fontawesome.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    15541 2022-06-14 14:12:38.000000 django-sloth-0.1.0/sloth/utils/icons/__pycache__/materialicons.cpython-310.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    20652 2022-09-21 17:02:39.000000 django-sloth-0.1.0/sloth/utils/icons/__pycache__/materialicons.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)    28753 2021-10-24 17:36:45.000000 django-sloth-0.1.0/sloth/utils/icons/bootstrap.py
+-rw-r--r--   0 breno      (503) staff       (20)    53105 2022-09-21 16:56:21.000000 django-sloth-0.1.0/sloth/utils/icons/fontawesome.py
+-rw-r--r--   0 breno      (503) staff       (20)    20959 2022-09-21 16:56:21.000000 django-sloth-0.1.0/sloth/utils/icons/materialicons.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.528756 django-sloth-0.1.0/sloth/utils/log/
+-rw-r--r--   0 breno      (503) staff       (20)        0 2022-10-06 09:42:03.000000 django-sloth-0.1.0/sloth/utils/log/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.530945 django-sloth-0.1.0/sloth/utils/log/__pycache__/
+-rw-r--r--   0 breno      (503) staff       (20)      179 2022-12-21 12:07:30.000000 django-sloth-0.1.0/sloth/utils/log/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)     1205 2022-12-21 12:07:44.000000 django-sloth-0.1.0/sloth/utils/log/__pycache__/sql.cpython-38.pyc
+-rw-r--r--   0 breno      (503) staff       (20)      965 2022-10-06 09:42:03.000000 django-sloth-0.1.0/sloth/utils/log/sql.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.531953 django-sloth-0.1.0/themes/
+-rw-r--r--   0 breno      (503) staff       (20)        0 2023-02-23 16:57:36.000000 django-sloth-0.1.0/themes/__init__.py
+drwxr-xr-x   0 breno      (503) staff       (20)        0 2023-04-17 19:06:29.532492 django-sloth-0.1.0/themes/dsgovbr/
+-rw-r--r--   0 breno      (503) staff       (20)        0 2023-02-23 16:57:51.000000 django-sloth-0.1.0/themes/dsgovbr/__init__.py
```

### Comparing `django-sloth-0.0.54/setup.py` & `django-sloth-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open(os.path.join(root_dir, 'requirements.txt')) as file:
     requirements = file.read().strip().splitlines()
 
 os.chdir(root_dir)
 
 setup(
     name='django-sloth',
-    version='0.0.54',
+    version='0.1.0',
     packages=find_packages(),
     install_requires=requirements,
     extras_require={
         'dev': [],
         'production': [],
     },
     include_package_data=True,
```

### Comparing `django-sloth-0.0.54/sloth/__init__.py` & `django-sloth-0.1.0/sloth/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # file_name = os.path.join(os.path.dirname(__file__), 'app', 'static', 'icons', 'fontawesome', 'fontawesome.min.js')
 # if not os.path.exists(file_name):
 #     with zipfile.ZipFile('{}.zip'.format(file_name), 'r') as file:
 #         file.extractall(os.path.dirname(file_name))
 
 PROXIED_MODELS = []
 
+
 class RoleLookup:
     def __init__(self, instance):
         self.instance = instance
         self.lookups = []
 
     def role_lookups(self, *names, **scopes):
         self.lookups.append((names, scopes))
@@ -45,33 +46,34 @@
                                 scope_value = scope_value if type(scope_value) == int else scope_value.pk
                                 if role.scope_value == scope_value:
                                     return True
                     else:
                         return True
         return False
 
+
 def meta(verbose_name=None, renderer=None, **metadata):
     def decorate(func):
         if verbose_name:
             setattr(func, '__verbose_name__', verbose_name)
         if renderer:
             setattr(func, '__template__', renderer)
         if metadata:
             setattr(func, '__metadata__', metadata)
 
         return func
     return decorate
 
 
-def initilize():
+def initialize():
     for module in ('dashboard', 'actions'):
         for app_label in settings.INSTALLED_APPS:
             try:
                 __import__('{}.{}'.format(app_label, module), fromlist=app_label.split('.'))
-                # print('{} {} initilized!'.format(app_label, module))
+                # print('{} {} initialized!'.format(app_label, module))
             except ImportError as e:
                 if not e.name.endswith('dashboard') and not e.name.endswith('actions'):
                     raise e
             except BaseException as e:
                 raise e
     for model in apps.get_models():
         validate_model(model)
@@ -80,17 +82,25 @@
 class BaseManager(manager.BaseManager):
     def get_queryset(self):
         return super().get_queryset()
 
     def all(self):
         return self.get_queryset().all()
 
+    def view(self):
+        return self.get_queryset().view()
+
+    def __call__(self, model_name):
+        return apps.get_model(model_name).objects
+
 
 class Manager(BaseManager.from_queryset(QuerySet)):
-    pass
+
+    def __call__(self, model_name):
+        return apps.get_model(model_name)
 
 
 ___new___ = ModelBase.__new__
 
 
 def __new__(mcs, name, bases, attrs, **kwargs):
 
@@ -112,12 +122,9 @@
 
 
 ModelBase.__new__ = __new__
 models.QuerySet = QuerySet
 models.Manager = Manager
 
 setattr(options, 'DEFAULT_NAMES', options.DEFAULT_NAMES + (
-    'icon', 'fieldsets', 'select_template', 'select_fields', 'search_fields'
+    'icon', 'fieldsets', 'select_template', 'select_fields', 'search_fields', 'autouser'
 ))
-
-
-
```

### Comparing `django-sloth-0.0.54/sloth/actions/__init__.py` & `django-sloth-0.1.0/sloth/actions/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,60 @@
 # -*- coding: utf-8 -*-
+import datetime
 import math
 import re
 import traceback
-from decimal import Decimal
 from copy import deepcopy
+from decimal import Decimal
 from functools import lru_cache
-from django.contrib import auth
+
+from django.apps import apps
 from django.contrib import messages
-from django.conf import settings
-from django.http import HttpResponse
+from django.forms.models import ModelFormMetaclass
+from django.forms import *
+from .fields import *
+from django.http import HttpResponse, HttpResponseRedirect
 from django.template.loader import render_to_string
 from django.utils.safestring import mark_safe
 from django.utils.text import slugify
+
 from . import inputs
-from django import forms
-from django.forms.models import ModelFormMetaclass, ModelMultipleChoiceField
-from ..exceptions import JsonReadyResponseException, ReadyResponseException
-from ..utils import to_api_params, to_camel_case, to_snake_case
-from django.forms.fields import *
-from django.forms.widgets import *
 from .fields import *
-from django.core.exceptions import ValidationError
+from ..core.queryset import QuerySet
+from sloth.api.exceptions import JsonReadyResponseException, ReadyResponseException, HtmlReadyResponseException
+from ..utils import to_api_params, to_snake_case
 from ..utils.formatter import format_value
+from ..utils.http import FileResponse
 
 ACTIONS = {}
+EXPOSE = []
 
 
 class PermissionChecker:
 
     def __init__(self, request, instance=None, instantiator=None, metaclass=None):
         self.request = request
         self.instance = instance
         self.instantiator = instantiator
         self.metaclass = metaclass
 
     def has_permission(self, user):
-        pass
+        return self and user
+
+
+class ActionDefaultMetaClass:
+    modal = True
 
 
 class ActionMetaclass(ModelFormMetaclass):
     def __new__(mcs, name, bases, attrs):
         if 'Meta' in attrs:
             if hasattr(attrs['Meta'], 'model'):
+                if isinstance(attrs['Meta'].model, str):
+                    attrs['Meta'].model = apps.get_model(attrs['Meta'].model)
                 bases += forms.ModelForm,
             else:
                 bases += forms.Form,
             if not hasattr(attrs['Meta'], 'fields') and not hasattr(attrs['Meta'], 'exclude'):
                 form_fields = []
                 fieldsets = getattr(attrs['Meta'], 'fieldsets', {})
                 if fieldsets:
@@ -54,80 +63,119 @@
                             if isinstance(names, str):
                                 form_fields.append(names)
                             else:
                                 form_fields.extend(names)
                     setattr(attrs['Meta'], 'fields', form_fields)
                 else:
                     setattr(attrs['Meta'], 'exclude', ())
-        elif name != 'Action':
-            raise NotImplementedError('class {} must have a Meta class.'.format(name))
+        else:
+            bases += forms.Form,
+            attrs['Meta'] = ActionDefaultMetaClass
         cls = super().__new__(mcs, name, bases, attrs)
         ACTIONS[name] = cls
-        ACTIONS[name.lower()] = cls
         ACTIONS[to_snake_case(name)] = cls
+        if 'ActionView' in [k.__name__ for k in bases]:
+            EXPOSE.append(to_snake_case(name))
         return cls
 
 
+class RegionalDateWidget(DateInput):
+    input_type = 'date'
+
+    def render(self, name, value, attrs=None, renderer=None):
+        if isinstance(value, datetime.date):
+            value = value.isoformat()
+        attrs = attrs or {}
+        attrs.update({'autocomplete': 'off'})
+        html = super().render(name, value, attrs)
+        return mark_safe(html)
+
+
+class RegionalDateTimeWidget(DateTimeInput):
+    input_type = 'datetime-local'
+
+    def render(self, name, value, attrs=None, renderer=None):
+        if isinstance(value, datetime.datetime):
+            value = value.isoformat().split('.')[0]
+        attrs = attrs or {}
+        attrs.update({'step': '1'})
+        html = super().render(name, value, attrs)
+        return mark_safe(html)
+
+
 class Action(metaclass=ActionMetaclass):
 
     def __init__(self, *args, **kwargs):
+        self.path = None
         self.request = kwargs.pop('request', None)
         self.instantiator = kwargs.pop('instantiator', None)
-        self.instances = kwargs.pop('instances', ())
+        self.queryset = kwargs.pop('queryset', None)
+        self.instances = kwargs.pop('instances', None)
         self.metaclass = getattr(self, 'Meta')
-        self.output_data = None
-        self.on_change_data = {'show': [], 'hide': [], 'set': [], 'show_fieldset': [], 'hide_fieldset': []}
+
+        self.show_form = True
+        self.can_be_closed = False
+        self.can_be_reloaded = False
+        self.content = dict(top=[], left=[], center=[], right=[], bottom=[], info=[], alert=[])
+        self.on_change_data = dict(show=[], hide=[], set=[], show_fieldset=[], hide_fieldset=[])
 
         if forms.ModelForm in self.__class__.__bases__:
             self.instance = kwargs.get('instance', None)
-            if self.instances:
-                kwargs.update(instance=self.instances[0])
         else:
             self.instance = kwargs.pop('instance', None)
-            if self.instance is None:
-                if self.instances:
-                    self.instance = self.instances[0]
-            else:
-                if self.instances == ():
-                    self.instances = self.instance,
 
-        form_name = type(self).__name__
+        if self.has_url_posted_data():
+            for k in self.request.GET:
+                if k.startswith('post__'):
+                    if 'data' not in kwargs:
+                        kwargs['data'] = {}
+                    kwargs['data'][k.split('__')[-1]] = self.request.GET[k]
+
         if 'data' not in kwargs:
-            if form_name in self.request.GET or form_name in self.request.POST or self.request.path.startswith('/api/'):
+            if self.get_api_name() in self.request.GET or self.get_api_name() in self.request.POST or self.request.path.startswith('/api/'):
                 # if self.base_fields or self.requires_confirmation():
                 if self.request.method == 'GET' or self.requires_confirmation():
                     if self.get_method() == 'get':
                         data = self.request.GET or None
                     else:
                         data = self.request.POST or None
                 else:
                     data = self.request.POST
                 kwargs['data'] = data
                 kwargs['files'] = self.request.FILES or None
             else:
                 kwargs['data'] = None
 
         super().__init__(*args, **kwargs)
+        if self.instance is not None and hasattr(self.instance, 'autouser') and not self.instance.autouser_id:
+            self.instance.autouser = self.request.user
+            if 'autouser' in self.fields:
+                del self.fields['autouser']
+
+        for name in self.fields:
+            setattr(self, name, self.initial.get(name, None))
+        self.asynchronous = getattr(self.metaclass, 'asynchronous', None) and self.request.GET.get('synchronous') is None
+
+        related_field_name = getattr(self.metaclass, 'related_field', None)
+        if related_field_name:
+            setattr(self.instance, related_field_name, self.instantiator)
+            if related_field_name in self.fields:
+                del self.fields[related_field_name]
 
         for field_name in self.fields:
             field = self.fields[field_name]
-            if False and hasattr(field, 'queryset') and field.queryset.metadata['lookups']: # TODO
-                field.queryset = field.queryset.apply_role_lookups(self.request.user)
-                if field.queryset.count() == 1:
-                    field.initial = field.queryset.first().id
-                    field.widget = forms.HiddenInput()
-            if hasattr(field, 'queryset') and getattr(field, 'auto_user', False) and not self.request.user.is_superuser:
-                scope_type = '{}.{}'.format(
-                    field.queryset.model.metaclass().app_label, field.queryset.model.metaclass().model_name
-                )
-                pks = self.request.user.roles.filter(scope_type=scope_type).values_list('scope_value', flat=True)
-                field.queryset = field.queryset.model.objects.filter(pk__in=pks)
-                if len(pks) == 1:
-                    field.initial = pks.first()
-                    field.widget = forms.HiddenInput()
+            if hasattr(field, 'queryset'):
+                if not self.request.user.is_superuser and getattr(field, 'username_lookup', None):
+                    pks = list(field.queryset.filter(**{field.username_lookup: self.request.user}).values_list('pk', flat=True)[0:2])
+                    if len(pks) == 1:
+                        field.queryset = field.queryset.model.objects.filter(pk=pks[0])
+                        field.initial = pks[0]
+                        field.widget = forms.HiddenInput()
+                else:
+                    field.queryset = field.queryset.contextualize(self.request).apply_role_lookups(self.request.user)
             if hasattr(field, 'picker'):
                 grouper = field.picker if isinstance(field.picker, str) else None
                 if isinstance(field, forms.ModelMultipleChoiceField):
                     field.widget = inputs.MultiplePickInput(field.queryset, grouper=grouper)
                 else:
                     field.widget = inputs.PickInput(field.queryset, grouper=grouper)
 
@@ -137,37 +185,95 @@
         self.one_to_many = {}
 
         confirmation = self.requires_confirmation()
         if confirmation:
             help_text = confirmation if isinstance(confirmation, str) else ''
             self.fields['confirmation'] = forms.BooleanField(
                 label='', initial='on', required=False, help_text=help_text,
-                widget=forms.TextInput(attrs={'style': 'display:none'})
+                widget=forms.HiddenInput()
             )
 
+    def get_verbose_name(self):
+        return self.get_metadata().get('name')
+
+    def get_image(self):
+        return self.get_metadata().get('image')
+
+    def has_url_posted_data(self):
+        return 'post__{}'.format(self.get_api_name()) in self.request.GET
+
+    def closable(self, flag=True):
+        self.can_be_closed = flag
+
+    def reloadable(self, flag=True):
+        self.can_be_reloaded = flag
+
+    def info(self, text):
+        if text:
+            self.content['info'].append(text)
+
+    def alert(self, text):
+        if text:
+            self.content['alert'].append(text)
+
+    def parameters(self, index):
+        values = None
+        for token in self.request.path.split('/'):
+            if values is not None:
+                values.append((token))
+            if token.lower() == self.get_api_name():
+                values = []
+        return values[index] if values and len(values)>index else None
+
+    def objects(self, model_name):
+        return apps.get_model(model_name).objects.contextualize(self.request)
+
+    def clear(self):
+        self.show_form = False
+        for k, v in self.content.items():
+            if k != 'bottom':
+                v.clear()
+
+    def view(self):
+        return None
+
+    def append(self, item, position='center'):
+        if hasattr(item, 'contextualize'):
+            item.contextualize(self.request)
+        self.content[position].append(item.html())
+
+    def has_attr_permission(self, user, name):
+        attr = getattr(self, 'has_{}_permission'.format(name), None)
+        return attr is None or attr(user)
+
     def requires_confirmation(self):
         return getattr(self.metaclass, 'confirmation', False)
 
     @lru_cache
     def get_one_to_one_field_names(self):
         return self.instance.get_one_to_one_field_names() if self.instance else ()
 
     @lru_cache
     def get_one_to_many_field_names(self):
         return self.instance.get_one_to_many_field_names() if self.instance else ()
 
     def get_fieldsets(self):
+        related_field = getattr(self.instance, 'related_field', None) if self.instance is not None else None
+        if related_field and related_field in self.fields:
+            del self.fields[related_field]
         fieldsets = getattr(self.metaclass, 'fieldsets', None)
         if fieldsets is None:
             fieldsets = {}
             if self.fields:
                 field_names = [
-                    name for name in self.fields.keys()
-                    if name not in self.get_one_to_one_field_names()
-                       and name not in self.get_one_to_many_field_names()
+                    name for name in self.fields.keys() if (
+                            name not in self.get_one_to_one_field_names()
+                            and name not in self.get_one_to_many_field_names()
+                            and name not in ('confirmation', related_field)
+                    )
                 ]
                 if field_names:
                     fieldsets[None] = field_names
         else:
             fieldsets = dict(fieldsets)
         return fieldsets
 
@@ -180,14 +286,21 @@
                 if name in self.get_one_to_one_field_names():
                     # remove one-to-one fields from the form
                     self.one_to_one[name] = self.fields.pop(name)
                 if name in self.get_one_to_many_field_names():
                     # remove one-to-many fields from the form
                     self.one_to_many[name] = self.fields.pop(name)
 
+        pop = []
+        for name, names in fieldsets.items():
+            if len(names) == 1 and (names[0] in self.one_to_one.keys() or names[0] in self.one_to_many.keys()):
+                pop.append(name)
+        for name in pop:
+            del fieldsets[name]
+
         # configure one-to-one fields
         for one_to_one_field_name, one_to_one_field in self.one_to_one.items():
             field_list = []
             form_cls = one_to_one_field.queryset.model.add_form_cls()
             initial = one_to_one_field.queryset.model.objects.filter(
                 pk=getattr(self.instance, '{}_id'.format(one_to_one_field_name))
             ).values(
@@ -310,15 +423,15 @@
         if hasattr(super(), 'save'):
             super().save(*args, **kwargs)
 
         # save one-to-many fields
         for name in self.one_to_many:
             qs = getattr(self.instance, name)
             pks = list(qs.values_list('pk', flat=True))
-            for i in range(0, 6):
+            for i in range(0, 10):
                 key = '{}--{}'.format(name.upper(), i)
                 pk = self.data.get(key)
                 if pk:  # if checkbox is checked
                     if pk == 'on':
                         instance = qs.model()
                     else:
                         pks.remove(int(pk))
@@ -329,15 +442,15 @@
                     instance.save()
                     qs.add(instance)
             qs.filter(pk__in=pks).delete()
 
         if hasattr(self.instance, 'post_save'):
             self.instance.post_save()
 
-    def serialize(self, wrap=False, verbose=False):
+    def serialize(self, wrap=False):
         if self.response:
             return self.response
         if wrap:
             data = dict(type='form')
             form_fields = {}
             for field_name in self.fields:
                 field = self.fields[field_name]
@@ -362,106 +475,104 @@
         on_change = []
         for attr_name in dir(self):
             if attr_name.startswith('on_') and attr_name.endswith('_change'):
                 field_name = attr_name[3:-7]
                 on_change.append(field_name)
         return on_change
 
+    def get_allowed_attrs(self, recursive=True):
+        return []
+
+    @classmethod
+    def get_api_name(cls):
+        return to_snake_case(cls.__name__)
+
     @classmethod
     @lru_cache
-    def get_metadata(cls, path=None, inline=False, batch=False):
-        form_name = cls.__name__
+    def get_metadata(cls, path=None, target=None):
         metaclass = getattr(cls, 'Meta', None)
         if metaclass:
-            target = 'model'
-            name = getattr(metaclass, 'verbose_name', re.sub("([a-z])([A-Z])", "\g<1> \g<2>", form_name))
+            target = target
+            name = getattr(metaclass, 'verbose_name', re.sub("([a-z])([A-Z])", "\g<1> \g<2>", cls.__name__))
             submit = getattr(metaclass, 'submit_label', name)
             icon = getattr(metaclass, 'icon', None)
             ajax = getattr(metaclass, 'ajax', True)
             modal = getattr(metaclass, 'modal', True)
             style = getattr(metaclass, 'style', 'primary')
             method = getattr(metaclass, 'method', 'post')
+            auto_reload = getattr(metaclass, 'auto_reload', None)
+            image = getattr(metaclass, 'image', None)
         else:
-            target, name, submit, icon, ajax, modal, style, method = (
-                'model', 'Enviar', 'Enviar', None, True, 'modal', 'primary', 'get'
+            name, submit, icon, ajax, modal, style, method, auto_reload, image = (
+                'Enviar', 'Enviar', None, True, 'modal', 'primary', 'get', None, None
             )
         if path:
-            if inline or batch:
-                target = 'queryset' if batch else 'instance'
-                path = '{}{{id}}/{}/'.format(path, form_name)
+            path, *params = path.split('?')
+            if target in ('queryset', 'instance'):
+                path = '{}{{id}}/{}/'.format(path, cls.get_api_name())
             else:
-                path = '{}{}/'.format(path, form_name)
+                path = '{}{}/'.format(path, cls.get_api_name())
+            if params:
+                path = '{}?{}'.format(path, params[0])
         metadata = dict(
-            type='form', key=form_name, name=name, submit=submit, target=target,
-            method=method, icon=icon, style=style, ajax=ajax, path=path, modal=modal
+            type='form', key=cls.get_api_name(), name=name, submit=submit, target=target,
+            method=method, icon=icon, style=style, ajax=ajax, path=path, modal=modal,
+            auto_reload=auto_reload, image=image
         )
         return metadata
 
     def get_method(self):
         return getattr(self.metaclass, 'method', 'post') if hasattr(self, 'Meta') else 'post'
 
     def get_instructions(self):
         return None
 
-    def get_reload_areas(self):
-        reload = getattr(self.metaclass, 'reload', 'self')
-        if isinstance(reload, tuple):
-            return ','.join(reload)
-        return reload or ''
-
     def is_modal(self):
         return getattr(self.metaclass, 'modal', True) if hasattr(self, 'Meta') else True
 
     def has_permission(self, user):
         return user.is_superuser
 
     def check_permission(self, user):
         return user.is_superuser or self.has_permission(user)
 
     @classmethod
     def check_fake_permission(cls, request, instance=None, instantiator=None):
-        if request and not request.user.is_superuser:
+        if request:  # and not request.user.is_superuser
             checker = PermissionChecker(request, instance, instantiator, getattr(cls, 'Meta', None))
             has_permission = cls.has_permission(checker, request.user)
             return cls.check_permission(checker, request.user) if has_permission is None else has_permission
         return True
 
     def __str__(self):
         return self.html()
 
+    def get_alternative_links(self):
+        return []
+
     def html(self):
-        if self.response:
-            if 'html' in self.response:
-                return self.response['html']
-            else:
-                js = '<script>{}</script>'
-                if self.response['url'] == '.':
-                    display_messages = True
-                    js = js.format('$(document).reload();')
-                elif self.response['url'] == '..':
-                    display_messages = 'modal' in self.request.GET
-                    js = js.format('$(document).back();')
-                else:
-                    display_messages = False
-                    js = js.format('$(document).redirect("{}");'.format(self.response['url']))
-                html = render_to_string('app/messages.html', request=self.request) if display_messages else ''
-                return '<!---->{}{}<!---->'.format(js, html)
 
         for name, field in self.fields.items():
             classes = field.widget.attrs.get('class', '').split()
             if isinstance(field.widget, forms.CheckboxInput):
                 classes.append('form-check-input')
             elif isinstance(field.widget, forms.widgets.Input):
                 classes.append('form-control')
 
-            if isinstance(field, forms.DateTimeField):
-                classes.append('date-time-input')
-
             if isinstance(field, forms.DateField):
+                field.widget = RegionalDateWidget()
                 classes.append('date-input')
+                if name in self.initial and self.initial[name] and isinstance(self.initial[name], str) and '/' in self.initial[name]:
+                    self.initial[name] = datetime.datetime.strptime(self.initial[name], '%d/%m/%Y').strftime('%Y-%m-%m')
+
+            if isinstance(field, forms.DateTimeField):
+                field.widget = RegionalDateTimeWidget()
+                classes.append('date-time-input')
+                if name in self.initial and self.initial[name] and isinstance(self.initial[name], str) and '/' in self.initial[name]:
+                    self.initial[name] = datetime.datetime.strptime(self.initial[name], '%d/%m/%Y').strftime('%Y-%m-%m %H:%M')
 
             if isinstance(field, forms.DecimalField):
                 field.widget.input_type = 'text'
                 field.widget.rmask = getattr(field.widget, 'rmask', '#.##0,00')
                 if name in self.initial and self.initial[name] is not None:
                     self.initial[name] =  Decimal('%.2f' % self.initial[name])
 
@@ -476,16 +587,16 @@
                         pks.append(initial)
                     else:
                         pks.extend([obj.pk for obj in initial])
                 if self.data:
                     pks = [pk for pk in self.data.getlist(name) if pk]
                 if getattr(field, 'picker', None) is None:
                     field.queryset = field.queryset.filter(pk__in=pks) if pks else field.queryset.none()
-                field.widget.attrs['data-choices-url'] = '{}?action_choices={}'.format(
-                    self.request.path, name
+                field.widget.attrs['data-choices-url'] = '{}{}action_choices={}'.format(
+                    self.get_full_path(), '&' if '?' in self.get_full_path() else '?', name
                 )
 
             if getattr(field.widget, 'mask', None):
                 classes.append('masked-input')
                 field.widget.attrs['data-reverse'] = 'false'
                 field.widget.attrs['data-mask'] = getattr(field.widget, 'mask')
             if getattr(field.widget, 'rmask', None):
@@ -494,15 +605,15 @@
                 field.widget.attrs['data-mask'] = getattr(field.widget, 'rmask')
             if getattr(field.widget, 'formatted', False):
                 classes.append('html-input')
 
             field.widget.attrs['class'] = ' '.join(classes)
         return mark_safe(
             render_to_string(
-                ['app/form.html'], dict(
+                ['dashboard/form.html'], dict(
                     self=self, fieldsets=self.fieldsets
                 ),
                 request=self.request
             )
         )
 
     def show(self, *names):
@@ -539,18 +650,71 @@
                 value = v.pk
                 text = str(v)
             else:
                 value = format_value(v)
                 text = None
             self.on_change_data['set'].append(dict(name=k, value=value, text=text))
 
+    def check_ouput(self, output, submit=False):
+        from ..core.valueset import ValueSet
+        position = 'bottom' if submit else 'center'
+        if type(output) == dict:
+            template_name = 'actions/{}.html'.format(self.get_api_name())
+            self.content[position].append(render_to_string([template_name], output, request=self.request))
+        elif type(output) == str and output[-5:].split('.')[-1] in FileResponse.CONTENT_TYPES.keys():
+            raise ReadyResponseException(FileResponse(output))
+        elif type(output) in (str, int, float, Decimal, datetime.date):
+            raise ReadyResponseException(HttpResponse(str(output)))
+        elif isinstance(output, HttpResponse):
+            raise ReadyResponseException(output)
+        elif isinstance(output, ValueSet) or isinstance(output, QuerySet):
+            if submit:
+                path = '{}{}/'.format(self.request.path, 'submit') if self.request.POST else None
+            else:
+                path = '{}{}/'.format(self.request.path, 'view')
+            self.content[position].append(output.contextualize(self.request).html(path=path))
+        elif output is not None:
+            raise Exception()
+
+        if self.request.path.startswith('/app/') and self.response and submit:
+            js = '<script>{}</script>'
+            display_messages = True
+            url = self.response.get('url')
+            if self.response.get('dispose'):
+                js = js.format('fade{}({});'.format(self.get_metadata().get('key'), self.response.get('dispose')))
+            elif url == '.':
+                if 'modal' in self.request.GET:
+                    js = js.format('$(document).popup("{}");'.format(self.request.path))
+                else:
+                    js = js.format('$(document).refresh([]);'.format(self.get_metadata().get('key')))
+            elif url == '..':
+                display_messages = 'modal' in self.request.GET
+                js = js.format('$(document).back().refresh([]);')
+            elif url:
+                display_messages = False
+                js = js.format('$(document).redirect("{}");'.format(self.response['url']))
+            html = render_to_string('dashboard/messages.html', request=self.request) if display_messages else ''
+            raise ReadyResponseException(HttpResponse('<!---->{}{}<!---->'.format(js, html)))
+
+        if self.request.path.startswith('/app/') and self.response and not submit:
+            stack = self.request.session.get('stack', [])
+            url = self.response.get('url')
+            if url in ('.', '..') and len(stack) > 1:
+                url = stack[-2]
+            raise ReadyResponseException(HttpResponseRedirect(url))
+
+        return output
+
     def is_valid(self):
+        if self.asynchronous:
+            return False
+        self.check_ouput(self.view())
         for field in self.fields.values():
             if isinstance(field, forms.DecimalField):
-                field.clean = lambda value: value.replace('.', '').replace(',','.')
+                field.clean = lambda v: v.replace('.', '').replace(',', '.')
         self.load_fieldsets()
         if 'action_choices' in self.request.GET:
             raise JsonReadyResponseException(
                 self.choices(self.request.GET['action_choices'], q=self.request.GET.get('term'))
             )
         if 'on_change_field' in self.request.POST:
             for data in self.on_change_data.values():
@@ -574,91 +738,129 @@
         qs = qs.search(q=q) if q else qs
         items = [dict(id=value.id, text=str(value), html=value.get_select_display()) for value in qs[0:25]]
         return dict(
             total=total, page=1, pages=math.ceil((1.0 * total) / 25),
             q=q, items=items
         )
 
-    def redirect(self, url=None, message=None, style='success'):
+    def dispose(self, milleseconds=2000):
+        self.response.update(dispose=milleseconds)
+
+    def reload(self):
+        return self.redirect('.')
+
+    def message(self, text='Ação realizada com sucesso.', style='success', milleseconds=60000):
+        level = dict(success=messages.SUCCESS, warning=messages.WARNING, info=messages.INFO)[style]
+        if self.request.path.startswith('/app/'):
+            messages.add_message(self.request, level, text)
+        else:
+            self.response.update(message=dict(text=text, style=style, milleseconds=milleseconds))
+
+    def redirect(self, url=None):
         if url is None:
-            url = '..' if self.fields or self.is_modal() else '.'
-            # if url == '..' and not self.get_refresh():
-            #     url = '.'
+            url = '..' if getattr(self, 'fields', None) or self.is_modal() else '.'
         self.response.update(type='redirect', url=url)
-        if message is None:
-            message = getattr(self.metaclass, 'message', None)
-        if message and self.request.path.startswith('/app/'):
-            messages.add_message(self.request, messages.SUCCESS, message)
-            self.response.update(message=message, style=style)
+        if not self.get_metadata()['ajax']:
+            raise ReadyResponseException(HttpResponseRedirect(url))
 
-    def run(self, *tasks, message=None):
+    def run(self, *tasks):
         for task in tasks:
             task.start(self.request)
         if len(tasks) > 1:
-            self.redirect(message=message or 'Tarefas iniciadas com sucesso')
-        elif message:
-            self.redirect(message=message)
-        else:
-            self.redirect('/app/api/task/{}/'.format(task.task_id), message=message)
-
-    def display(self, data, template='app/default.html'):
-        if isinstance(data, dict):
-            ctx = data
+            self.redirect()
         else:
-            ctx = dict(form=self, data=data.contextualize(self.request).html())
-        self.response.update(
-            html=render_to_string([template], ctx, request=self.request)
-        )
+            self.redirect('/app/api/task/{}/'.format(task.task_id))
 
     def submit(self):
         if self.instances:
             for instance in self.instances:
                 self.instance = instance
                 self._post_clean()
                 self.save()
         else:
             self.save()
-        self.redirect(message='Ação realizada com sucesso.')
+        self.message('Ação realizada com sucesso.')
+        self.redirect()
 
     def process(self):
         try:
-            response = self.submit()
-            if isinstance(response, HttpResponse):
-                raise ReadyResponseException(response)
+            return self.check_ouput(self.submit(), True)
         except forms.ValidationError as e:
             if self.request.path.startswith('/app/'):
                 message = 'Corrija os erros indicados no formulário'
                 messages.add_message(self.request, messages.WARNING, message)
             self.add_error(None, e.message)
         except BaseException as e:
             if isinstance(e, ReadyResponseException):
                 raise e
+            if isinstance(e, JsonReadyResponseException):
+                raise e
+            if isinstance(e, HtmlReadyResponseException):
+                raise e
             traceback.print_exc()
             if self.request.path.startswith('/app/'):
                 message = 'Ocorreu um erro no servidor: {}'.format(e)
                 messages.add_message(self.request, messages.WARNING, message)
             self.add_error(None, message)
 
-    def display(self):
-        return None
-
-    def output(self, data, template=None):
-        if template:
-            self.output_data = render_to_string(template, data, request=self.request)
-        else:
-            self.output_data = data
-
     @classmethod
     def get_attr_metadata(cls, lookup):
         attr = getattr(cls, lookup)
         template = getattr(attr, '__template__', None)
         metadata = getattr(attr, '__metadata__', None)
         if template:
             if not template.endswith('.html'):
                 template = '{}.html'.format(template)
             if not template.startswith('.html'):
                 template = 'renderers/{}'.format(template)
         return getattr(attr, '__verbose_name__', lookup), False, template, metadata
 
-    def values(self, *names):
+    def value_set(self, *names):
         from sloth.core.base import ValueSet
-        return ValueSet(self, names)
+        return ValueSet(self, names)
+
+    @classmethod
+    @lru_cache
+    def action_form_cls(cls, action):
+        return ACTIONS.get(action)
+
+    def should_display_buttons(self):
+        return self.fields or self.submit.__func__ != Action.submit
+
+    # def dumps(self):
+    #     state = dict(instantiator=None, instance=None, instances=None)
+    #     if self.instantiator:
+    #         state['instantiator'] = '{}.{}'.format(
+    #             self.instantiator.metaclass().app_label,
+    #             self.instantiator.metaclass().model_name,
+    #         ), self.instantiator.id
+    #     if self.instance:
+    #         state['instance'] = '{}.{}'.format(
+    #             self.instance.metaclass().app_label,
+    #             self.instance.metaclass().model_name,
+    #         ), self.instance.id
+    #     if self.instances:
+    #         state['instances'] = self.instances.dumps()
+    #     from pprint import pprint;pprint(state)
+    #     return signing.dumps(base64.b64encode(zlib.compress(pickle.dumps(state))).decode())
+    #
+    # def loads(self, s):
+    #     state = pickle.loads(zlib.decompress(base64.b64decode(signing.loads(s).encode())))
+    #     if state['instantiator'] and state['instantiator'][1]:
+    #         self.instantiator = apps.get_model(state['instantiator'][0]).objects.get(pk=state['instantiator'][1])
+    #     if state['instance'] and state['instance'][1]:
+    #         self.instance = apps.get_model(state['instance'][0]).objects.get(pk=state['instance'][1])
+    #     if state['instances']:
+    #         self.instances = QuerySet.loads(state['instances'])
+
+    def get_full_path(self):
+        return self.path or self.request.get_full_path()
+
+    def contextualize(self, request):
+        return self
+
+    def apply_role_lookups(self, user):
+        return self
+
+
+class ActionView(Action):
+    pass
```

### Comparing `django-sloth-0.0.54/sloth/actions/fields.py` & `django-sloth-0.1.0/sloth/actions/fields.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from django import forms
+
 from . import inputs
 
 
 class QrCodeField(forms.CharField):
     def __init__(self, *args, **kwargs):
         kwargs.update(widget=inputs.QrCodeInput())
         super().__init__(*args, **kwargs)
 
 
 class ModelChoiceField(forms.ModelChoiceField):
     def __init__(self, *args, **kwargs):
-        self.auto_user = kwargs.pop('auto_user', False)
+        self.username_lookup = kwargs.pop('username_lookup', None)
         super().__init__(*args, **kwargs)
 
 
 class TextField(forms.CharField):
     def __init__(self, *args, **kwargs):
         kwargs.update(widget=forms.Textarea())
         super().__init__(*args, **kwargs)
```

### Comparing `django-sloth-0.0.54/sloth/actions/inputs.py` & `django-sloth-0.1.0/sloth/actions/inputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.forms import widgets
 from django.template.loader import render_to_string
 from django.utils.safestring import mark_safe
+
 from sloth.utils import colors
 
 
 class ColorInput(widgets.TextInput):
 
     def render(self, name, value, attrs=None, renderer=None):
         attrs['class'] = 'd-none'
@@ -26,15 +27,15 @@
             </script>
             <style>#colorPick{{z-index:99999;}}</style>
         '''.format(cpid, cpid, value or '#FFFFFF', name, colors())
         return mark_safe('{}\n{}'.format(html, extra))
 
 
 class PickInputMixin():
-    def __init__(self, queryset, template_name='app/inputs/picker.html', multiple=False, grouper=None, *args, **kwargs):
+    def __init__(self, queryset, template_name='inputs/picker.html', multiple=False, grouper=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.queryset = queryset
         self.template_name = template_name
         self.multiple = multiple
         self.grouper = grouper
 
     def value_from_datadict(self, data, files, name):
@@ -76,9 +77,9 @@
         super().__init__(*args, **kwargs)
 
 
 class QrCodeInput(widgets.TextInput):
 
     def render(self, name, value, attrs=None, **kwargs):
         widget = super().render(name, value, attrs=attrs, **kwargs)
-        output = render_to_string('app/inputs/qrcode.html', dict(widget=widget, name=name))
+        output = render_to_string('inputs/qrcode.html', dict(widget=widget, name=name))
         return mark_safe(output)
```

### Comparing `django-sloth-0.0.54/sloth/api/__init__.py` & `django-sloth-0.1.0/sloth/api/__init__.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/api/backends/__init__.py` & `django-sloth-0.1.0/sloth/api/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/api/management/commands/query.py` & `django-sloth-0.1.0/sloth/api/management/commands/query.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/api/management/commands/sync.py` & `django-sloth-0.1.0/sloth/api/management/commands/sync.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 
 import os
+
 from django.conf import settings
-from django.utils import termcolors
 from django.contrib.auth.models import User
 from django.core.management import call_command
 from django.core.management.base import BaseCommand
+from django.utils import termcolors
 
 
 def print_and_call(command, *args, **kwargs):
     kwargs.setdefault('interactive', True)
     print(termcolors.make_style(fg='cyan', opts=('bold',))('>>> {} {}{}'.format(
         command, ' '.join(args), ' '.join(['{}={}'.format(k, v) for k, v in list(kwargs.items())]))))
     call_command(command, *args, **kwargs)
@@ -25,11 +26,13 @@
         print_and_call('makemigrations', *app_labels)
         print_and_call('migrate')
 
         # if it is the production enverinoment, lets collect static files
         if os.path.exists(os.path.join(settings.BASE_DIR, 'logs')):
             print_and_call('collectstatic', clear=True, verbosity=0, interactive=False)
 
-        if 'DEFAULT_PASSWORD' in settings.SLOTH and not User.objects.exists():
-            password = settings.SLOTH['DEFAULT_PASSWORD']()
-            User.objects.create_superuser('admin', password=password)
+        if not User.objects.exists():
+            user = User.objects.create_superuser('admin')
+            password = settings.DEFAULT_PASSWORD(user)
+            user.set_password(password)
+            user.save()
             print('Superuser "admin" with password "{}" was created.'.format(password))
```

### Comparing `django-sloth-0.0.54/sloth/api/migrations/0001_initial.py` & `django-sloth-0.1.0/sloth/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/api/migrations/0002_role_user.py` & `django-sloth-0.1.0/sloth/api/migrations/0002_role_user.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/api/migrations/0003_alter_application_user.py` & `django-sloth-0.1.0/sloth/api/migrations/0003_alter_application_user.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/api/migrations/0004_task.py` & `django-sloth-0.1.0/sloth/api/migrations/0004_task.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/api/migrations/0005_task_stopped_alter_task_message.py` & `django-sloth-0.1.0/sloth/api/migrations/0005_task_stopped_alter_task_message.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py` & `django-sloth-0.1.0/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py` & `django-sloth-0.1.0/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py` & `django-sloth-0.1.0/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/api/migrations/0009_pushnotification.py` & `django-sloth-0.1.0/sloth/api/migrations/0009_pushnotification.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/api/migrations/0010_alter_pushnotification_user.py` & `django-sloth-0.1.0/sloth/api/migrations/0010_alter_pushnotification_user.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/api/migrations/0011_alter_application_client_secret.py` & `django-sloth-0.1.0/sloth/api/migrations/0011_alter_application_client_secret.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/api/migrations/0012_authcode.py` & `django-sloth-0.1.0/sloth/api/migrations/0012_authcode.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/api/migrations/0013_task_partial_task_total.py` & `django-sloth-0.1.0/sloth/api/migrations/0013_task_partial_task_total.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/api/models.py` & `django-sloth-0.1.0/sloth/api/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 # -*- coding: utf-8 -*-
+import json
+from datetime import datetime
 from django.apps import apps
+from django.conf import settings
 from oauth2_provider.models import AbstractApplication
-from django.contrib.auth.models import User as DjangoUser
+from django.contrib.auth.models import User as DjangoUser, AnonymousUser
 from sloth.db import models, meta
+from django.utils.html import strip_tags
+from django.core.mail import EmailMultiAlternatives
 
 
 def user_post_save(instance, created, **kwargs):
-    pass
+    user_role_name = getattr(settings, 'USER_ROLE_NAME', 'Usuário')
+    if not instance.roles.contains(user_role_name):
+        Role.objects.create(
+            user=instance, name=user_role_name, scope_type='auth.user', scope_key='pk', scope_value=instance.pk
+        )
 
 
 models.signals.post_save.connect(user_post_save, sender=DjangoUser)
 
 
 class UserManager(models.Manager):
     def all(self):
         return self.display(
             'username', 'get_name', 'is_superuser', 'get_roles_names'
-        ).actions('LoginAsUser').verbose_name('Usuários').attach(
+        ).actions('login_as_user', 'change_password').verbose_name('Usuários').attach(
             'active', 'inactive'
-        )
-
+        ).global_actions('export_csv', 'export_xls', 'print')
 
     def active(self):
         return self.all().filter(is_active=True).verbose_name('Ativos')
 
-
     def inactive(self):
         return self.all().filter(is_active=False).verbose_name('Inativos')
 
 
 class User(DjangoUser):
 
     objects = UserManager()
@@ -39,38 +46,54 @@
         verbose_name_plural = 'Usuários'
         fieldsets = {
             'Dados Gerais': (('first_name', 'last_name'), 'username', 'email'),
             'Dados de Acesso': (('is_superuser', 'is_staff', 'is_active'),)
         }
 
     def view(self):
-        return self.values('get_general_info', 'get_access_info', 'get_roles')
+        return self.value_set('get_general_info', 'get_access_info', 'get_roles').actions('print')
 
     def get_general_info(self):
-        return self.values(('first_name', 'last_name'), 'username', 'email').verbose_name('Dados Gerais')
+        return self.value_set(('first_name', 'last_name'), 'username', 'email').verbose_name('Dados Gerais')
 
     def get_access_info(self):
-        return self.values('is_superuser',).verbose_name('Dados de Acesso')
+        return self.value_set('is_superuser',).verbose_name('Dados de Acesso')
 
     def get_name(self):
         return '{} {}'.format(self.first_name or '', self.last_name or '')
 
     @meta('Papéis')
     def get_roles(self):
-        return self.roles.all().ignore('user')
+        return self.roles.all().ignore('user').global_actions('print')
 
     @meta('Papéis')
     def get_roles_names(self):
         return list(self.roles.values_list('name', flat=True).distinct())
 
     def save(self, *args, **kwargs):
         created = self.pk is None
         super().save(*args, **kwargs)
         user_post_save(self, created=created)
 
+class AuthCode(models.Model):
+    user = models.ForeignKey(
+        User,
+        on_delete=models.CASCADE,
+        verbose_name='Usuário'
+    )
+    secret = models.CharField(max_length=16, verbose_name='Chave')
+    active = models.BooleanField(verbose_name='Ativo', default=False)
+
+    class Meta:
+        verbose_name = 'Código de Autenticação'
+        verbose_name_plural = 'Códigos de Autenticação'
+
+    def __str__(self):
+        return self.secret
+
 
 class RoleManager(models.Manager):
 
     def all(self):
         return self.display(
             'user', 'name', 'active', 'scope_key', 'get_scope_value'
         ).actions(
@@ -93,31 +116,14 @@
             return False
         return self.filter(active=True, name__in=names).exists()
 
     def names(self):
         return self.values_list('name', flat=True).distinct()
 
 
-class AuthCode(models.Model):
-    user = models.ForeignKey(
-        User,
-        on_delete=models.CASCADE,
-        verbose_name='Usuário'
-    )
-    secret = models.CharField(max_length=16, verbose_name='Chave')
-    active = models.BooleanField(verbose_name='Ativo', default=False)
-
-    class Meta:
-        verbose_name = 'Código de Autenticação'
-        verbose_name_plural = 'Códigos de Autenticação'
-
-    def __str__(self):
-        return self.secret
-
-
 class Role(models.Model):
     user = models.ForeignKey(
         User,
         related_name='roles',
         null=True,
         blank=True,
         on_delete=models.CASCADE,
@@ -172,27 +178,27 @@
     def __str__(self):
         return self.name
 
     def get_access_tokens(self):
         return self.accesstoken_set.all().verbose_name('Tokens de Acesso')
 
     def general_data(self):
-        return self.values('id', 'name').verbose_name('Dados Gerais')
+        return self.value_set('id', 'name').verbose_name('Dados Gerais')
 
     def access_data(self):
-        return self.values('client_id', 'client_secret', 'authorization_grant_type').verbose_name('Dados de Acesso')
+        return self.value_set('client_id', 'client_secret', 'authorization_grant_type').verbose_name('Dados de Acesso')
 
     def view(self):
-        return self.values('general_data', 'access_data', 'default_scopes', 'available_scopes')
+        return self.value_set('general_data', 'access_data', 'default_scopes', 'available_scopes')
 
 
 class TaskManager(models.Manager):
     def all(self):
         return self.display(
-            'id', 'user', 'name', 'start', 'end', 'get_progress'
+            'id', 'user', 'name', 'start', 'end', 'get_progress', 'message'
         ).attach(
             'running', 'finished', 'unfinished', 'stopped'
         ).global_actions('ManageTaskExecution')
 
     @meta('Em Execução')
     def running(self):
         return self.all().filter(end__isnull=True, stopped=False).ignore('end')
@@ -241,35 +247,82 @@
     @meta('Mensagem', 'messages/message')
     def get_message(self):
         if self.error:
             return 'danger', self.error
         elif self.stopped:
             return 'warning', 'Interrompida pelo usuário'
         elif self.progress < 100:
-            return 'primary', 'Em execução'
+            return 'primary', self.message or 'Em execução'
         else:
             return 'success', self.message or 'Concluída'
 
     @meta('Progresso', renderer='utils/progress')
     def get_progress(self):
         return self.progress
 
+    @meta('Dados Gerais')
     def get_info(self):
-        return self.values(('name', 'user'))
+        return self.value_set(('name', 'user'))
 
     @meta('Processamento')
     def get_process(self):
-        return self.values(('start', 'end'), ('total', 'partial'), 'get_progress', 'get_message').reload(seconds=5, condition='in_progress', max_requests=360).actions('StopTask')
+        return self.value_set(('start', 'end'), ('total', 'partial'), 'get_progress', 'get_message').reload(seconds=5, condition='in_progress', max_requests=360).actions('StopTask')
 
     def in_progress(self):
         return self.end is None
 
     def view(self):
-        return self.values('get_info', 'get_process')
+        return self.value_set('get_info', 'get_process')
 
     def has_view_permission(self, user):
         return user.is_superuser or self.user == user
 
 
 class PushNotification(models.Model):
     user = models.OneToOneField(DjangoUser, verbose_name='Usuário', on_delete=models.CASCADE, related_name='push_notification')
     subscription = models.JSONField(verbose_name='Dados da Inscrição')
+
+
+class EmailManager(models.Manager):
+    def all(self):
+        return self.rows()
+
+    def send(self, to, subject, content, from_email=None):
+        to = [to] if isinstance(to, str) else list(to)
+        return self.create(from_email=from_email, to=', '.join(to), subject=subject, content=content)
+
+
+class Email(models.Model):
+    from_email = models.EmailField('Remetente')
+    to = models.TextField('Destinatário', help_text='Separar endereços de e-mail por ",".')
+    subject = models.CharField('Assunto')
+    content = models.TextField('Conteúdo', formatted=True)
+    sent_at = models.DateTimeField('Data/Hora', null=True)
+
+    objects = EmailManager()
+
+    class Meta:
+        icon = 'envelope'
+        verbose_name = 'E-mail'
+        verbose_name_plural = 'E-mails'
+        fieldsets = {
+            'Dados Gerais': ('from_email', 'subject', 'to'),
+            'Detalhamento': ('content',),
+        }
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def __str__(self):
+        return self.subject
+
+    def save(self, *args, **kwargs):
+        super().save(*args, **kwargs)
+        to = [email.strip() for email in self.to.split(',')]
+        msg = EmailMultiAlternatives(self.subject, strip_tags(self.content), self.from_email, to)
+        msg.attach_alternative(self.content, "text/html")
+        if msg.send(fail_silently=False):
+            self.sent_at = datetime.now()
+            super().save(*args, **kwargs)
+
+
+setattr(AnonymousUser, 'roles', Role.objects.none())
```

### Comparing `django-sloth-0.0.54/sloth/api/static/js/api.js` & `django-sloth-0.1.0/sloth/api/static/js/api.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/api/templates/api/index.html` & `django-sloth-0.1.0/sloth/api/templates/api/index.html`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/dashboard.py` & `django-sloth-0.1.0/sloth/core/statistics.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,248 +1,276 @@
-from django.conf import settings
-from django.http import HttpResponseRedirect
-from django.template.loader import render_to_string
-from django.utils.safestring import mark_safe
-
-from sloth.app.templatetags.tags import mobile
-from sloth.exceptions import ReadyResponseException
-from sloth.utils import pretty
-from.actions import ExecuteQuery, ExecuteScript
+# -*- coding: utf-8 -*-
 
-
-DASHBOARDS = []
+import json
+from decimal import Decimal
+from django.db.models.aggregates import Count
+from sloth.api.exceptions import HtmlReadyResponseException
+from django.template.loader import render_to_string
+from sloth.utils import pretty, colors
 
 
-class DashboardType(type):
+MONTHS = 'JAN', 'FEV', 'MAR', 'ABR', 'MAI', 'JUN', 'JUL', 'AGO', 'SET', 'OUT', 'NOV', 'DEZ'
 
-    def __new__(mcs, name, bases, attrs):
-        cls = type.__new__(mcs, name, bases, attrs)
-        DASHBOARDS.append(cls)
-        return cls
 
+class QuerySetStatistics(object):
 
-class Dashboard(metaclass=DashboardType):
+    def __init__(self, qs, x, y=None, func=None, z='id'):
+        self.qs = qs
+        self.x = x
+        self.y = y
+        self.func = func or Count
+        self.z = z
+        self._xfield = None
+        self._yfield = None
+        self._xdict = {}
+        self._ydict = {}
+        self._values_dict = None
+        self.cursor = 0
+        self.request = None
+        self.metadata = dict(uuid='123456', attr=None, source=None, template='', verbose_name=None)
+
+        if '__month' in x:
+            self._xdict = {i + 1: month for i, month in enumerate(MONTHS)}
+        if y and '__month' in y:
+            self._ydict = {i + 1: month for i, month in enumerate(MONTHS)}
+
+    def verbose_name(self, name):
+        self.metadata['verbose_name'] = pretty(name)
+        return self
 
-    def __init__(self, request):
-        self.redirect_url = None
-        self.redirect_message = None
+    def contextualize(self, request):
         self.request = request
-        self.data = dict(
-            info=[], warning=[], search=[], menu=[], links=[], shortcuts=[], cards=[],
-            floating=[], navigation=[], settings=[], center=[], right=[], actions=[], tools=[]
-        )
-        self.extra = {}
-        self.defined_apps = {}
-        self.enabled_apps = set()
-        if self.request.user.is_authenticated:
-            self.load(request)
-
-    def redirect(self, url, message=None):
-        self.redirect_url = url
-        self.redirect_message = message
-
-    def header(self, logo=None, title=None, text=None, shadow=True):
-        self.extra['header'] = dict(logo=logo, title=title, text=text, shadow=shadow)
-
-    def footer(self, title=None, text=None, version=None):
-        self.extra['footer'] = dict(title=title, text=text, version=version)
-
-    def to_item(self, model, count=True):
-        return
-
-    def _load(self, key, items, app=None, count=False):
-        allways = 'floating', 'navigation', 'settings', 'actions', 'menu', 'links', 'tools', 'search'
-        for cls in items:
-            add_item = True
-            if app:
-                self.enabled_apps.add(app)
-                add_item = self.request.session.get('app_name') == app
-            if add_item:
-                if hasattr(cls, 'check_fake_permission'):
-                    if cls.check_fake_permission(request=self.request):
-                        metadata = cls.get_metadata()
-                        self.data[key].append(dict(
-                            url='/app/action/{}/'.format(metadata['key']), modal=metadata['modal'],
-                            label=metadata['name'], icon=metadata['icon'], app=app
-                        ))
-                else:
-                    if self.request.user.is_superuser or cls.objects.all().has_permission(self.request.user):
-                        if key in allways or self.request.path == '/app/':
-                            url = cls.get_list_url('/app')
-                            for item in self.data[key]:
-                                add_item = add_item and not item['url'] == url
-                            if add_item:
-                                self.data[key].append(
-                                    dict(
-                                        url=url,
-                                        label=cls.metaclass().verbose_name_plural,
-                                        count=cls.objects.all().apply_role_lookups(self.request.user).count() if count else None,
-                                        icon=getattr(cls.metaclass(), 'icon', None),
-                                        app=app
-                                    )
-                                )
-
-    def _item(self, key, url, label, icon, count=None, app=None):
-        self.data[key].append(
-            dict(url=url, label=label, count=count, icon=icon, app=app)
-        )
-
-    def info(self, *items, app=None):
-        self._load('info', items, app=app)
-
-    def warning(self, *items, app=None):
-        self._load('warning', items, app=app)
-
-    def search(self, *items, app=None):
-        self._load('search', items, app=app)
-
-    def menu(self, *items, app=None):
-        if mobile(self.request):
-            self._load('search', items, app=app)
-        else:
-            self._load('menu', items, app=app)
-
-    def links(self, *items, app=None):
-        self._load('links', items, app=app)
-
-    def add_link(self, url, label, app=None):
-        self._item(self, 'links', url, label, app=app)
-
-    def shortcuts(self, *items, app=None):
-        self._load('shortcuts', items, app=app)
-
-    def add_shortcut(self, url, label, icon, app=None):
-        self._item(self, 'shortcut', url, label, icon, app=app)
-
-    def actions(self, *items, app=None):
-        if mobile(self.request):
-            self._load('search', items, app=app)
+        if self.qs.request is None:
+            self.qs.contextualize(request)
+        self.qs = self.qs.apply_role_lookups(request.user) if request else self.qs
+        if request and self.metadata['uuid'] == request.GET.get('uuid'):
+            self.process_request(request)
+        return self
+
+    def get_allowed_attrs(self, recursive=True):
+        return self.qs.get_allowed_attrs(recursive=recursive)
+
+    def _calc(self):
+        if self._values_dict is None:
+            self.calc()
+
+    def _xfield_display_value(self, value):
+        if hasattr(self._xfield, 'choices') and self._xfield.choices:
+            for choice in self._xfield.choices:
+                if choice[0] == value:
+                    return choice[1]
+        return value
+
+    def _yfield_display_value(self, value):
+        if hasattr(self._yfield, 'choices') and self._yfield.choices:
+            for choice in self._yfield.choices:
+                if choice[0] == value:
+                    return choice[1]
+        return value
+
+    def _clear(self):
+        self._xfield = None
+        self._yfield = None
+        self._xdict = {}
+        self._ydict = {}
+        self._values_dict = None
+
+    def attr(self, name):
+        self.metadata['attr'] = name
+        if self.metadata['verbose_name'] is None:
+            self.metadata['verbose_name'] = pretty(name)
+        return self
+
+    def source(self, name):
+        self.metadata['source'] = name
+        return self
+
+    def calc(self):
+        self._values_dict = {}
+        if self.y:
+            values_list = self.qs.values_list(self.x, self.y).annotate(self.func(self.z))
         else:
-            self._load('actions', items, app=app)
+            values_list = self.qs.values_list(self.x).annotate(self.func(self.z))
 
-    def add_action(self, url, label, icon, app=None):
-        if mobile(self.request):
-            self._item(self, 'search', url, label, icon, app=app)
+        self._xfield = self.qs.model.get_field(self.x.replace('__year', '').replace('__month', ''))
+        if self._xdict == {}:
+            xvalues = self.qs.values_list(self.x, flat=True).order_by(self.x).distinct()
+            if self._xfield.related_model:
+                self._xdict = {
+                    obj.pk: str(obj) for obj in self._xfield.related_model.objects.filter(pk__in=xvalues)
+                }
+            else:
+                self._xdict = {
+                    value: value for value in self.qs.values_list(self.x, flat=True)
+                }
+            if None in xvalues:
+                self._xdict[None] = 'Não-Informado'
+        if self.y:
+            self._yfield = self.qs.model.get_field(self.y.replace('__year', '').replace('__month', ''))
+            yvalues = self.qs.values_list(self.y, flat=True).order_by(self.y).distinct()
+            if self._ydict == {}:
+                if self._yfield.related_model:
+                    self._ydict = {
+                        obj.pk: str(obj) for obj in self._yfield.related_model.objects.filter(pk__in=yvalues)
+                    }
+                else:
+                    self._ydict = {
+                        value: value for value in yvalues
+                    }
+            self._values_dict = {(vx, vy): calc for vx, vy, calc in values_list}
+            if None in yvalues:
+                self._ydict[None] = 'Não-Informado'
         else:
-            self._item(self, 'actions', url, label, icon, app=app)
-
-    def add_app(self, label, icon, hide=False):
-        url = '/app/?toggle-application={}'.format(label)
-        self.defined_apps[label] = dict(label=label, icon=icon, hide=hide, url=url, enabled=False)
-
-    def cards(self, *items, app=None):
-        self._load('cards', items, app=app, count=True)
-
-    def floating(self, *items, app=None):
-        self._load('floating', items, app=app)
+            self._ydict = {}
+            self._values_dict = {(vx, None): calc for vx, calc in values_list}
 
-    def tools(self, *items, app=None):
-        self._load('tools', items, app=app)
-
-    def navigation(self, *items, app=None):
-        if mobile(self.request):
-            self._load('floating', items, app=app)
+    def tabulate(self):
+        self._calc()
+        rows = []
+        row = []
+        row.append('')
+        for info in self._xdict.values():
+            row.append(info)
+        rows.append(row)
+        for i in self._xdict:
+            row = []
+            for j in self._ydict:
+                if not row:
+                    row.append(self._ydict[j])
+                row.append(self._values_dict.get((i, j), 0))
+            rows.append(row)
+        return rows
+
+    def filter(self, **kwargs):
+        self._clear()
+        self.qs = self.qs.filter(**kwargs)
+        return self
+
+    def apply_role_lookups(self, user):
+        self._clear()
+        self.qs = self.qs.apply_role_lookups(user)
+        return self
+
+    def debug(self):
+        print(json.dumps(self.serialize(wrap=True), indent=4, ensure_ascii=False))
+
+    def serialize(self, wrap=True, path=None, lazy=False):
+        series = dict()
+        if not lazy:
+            self._calc()
+
+            formatter = {True: 'Sim', False: 'Não', None: ''}
+
+            def format_value(value):
+                return float(value) if isinstance(value, Decimal) else value
+
+            if self._ydict:
+                for i, (yk, yv) in enumerate(self._ydict.items()):
+                    data = []
+                    self.cursor = 0
+                    for j, (xk, xv) in enumerate(self._xdict.items()):
+                        data.append([formatter.get(xv, str(self._xfield_display_value(xv))), format_value(self._values_dict.get((xk, yk), 0)), self.nex_color()])
+                    series.update(**{formatter.get(yv, str(self._yfield_display_value(yv))): data})
+            else:
+                data = list()
+                for j, (xk, xv) in enumerate(self._xdict.items()):
+                    data.append([formatter.get(xv, str(self._xfield_display_value(xv))), format_value(self._values_dict.get((xk, None), 0)), self.nex_color()])
+                if data:
+                    series['default'] = data
+        if self.request and path is None:
+            prefix = self.request.path.split('/')[1]
+            path = self.request.path.replace('/{}'.format(prefix), '')
+        if wrap:
+            return dict(
+                type='statistics',
+                uuid=self.qs.metadata['uuid'],
+                name=self.qs.metadata['verbose_name'],
+                key=self.qs.metadata['attr'],
+                path=path,
+                series=series,
+                template=self.metadata['template'],
+                normalized=self.normalize(series),
+            )
         else:
-            self._load('navigation', items, app=app)
+            return series['default'] if 'default' in series else series
 
-    def add_navigation(self, url, label, icon, app=None):
-        if mobile(self.request):
-            self._item('floating', url, label, icon, app=app)
+    def process_request(self, request):
+        for item in self.qs.get_filters().values():
+            value = request.GET.get(item['key'])
+            if value:
+                if item['type'] in ('date', 'datetime'):
+                    value = datetime.datetime.strptime(value, '%d/%m/%Y')
+                if item['type'] == 'boolean':
+                    value = bool(int(value)) if value.isdigit() else value == 'true'
+                self.qs = self.qs.filter(**{item['key']: value})
+        raise HtmlReadyResponseException(self.html())
+
+    def html(self):
+        serialized = self.serialize(wrap=True)
+        if self.qs.metadata['is_admin']:
+            name = self.qs.model.metaclass().verbose_name_plural
+            data = dict(
+                type='object', name=str(name),
+                icon=None, data={self.qs.metadata['verbose_name']: serialized}, actions=[], attach=[], append={}
+            )
+            # print(json.dumps(data, indent=4, ensure_ascii=False))
+            return render_to_string('valueset/valueset.html', dict(data=data), request=self.request)
         else:
-            self._item('navigation', url, label, icon, app=app)
-
-    def settings(self, *items, app=None):
-        self._load('settings', items, app=app)
-
-    def append(self, data, aside=False, grid=1):
-        if self.request.path == '/app/':
-            if aside and hasattr(data, 'compact'):
-                data.compact()
-            if self.request.path == '/app/':
-                html = str(data.contextualize(self.request))
-                if aside:
-                    self.data['right'].append(html)
-                else:
-                    self.data['center'].append((grid, html))
-
-    def extend(self, template, aside=False, grid=1, **data):
-        if self.request.path == '/app/':
-            html = mark_safe(render_to_string(template, data, request=self.request))
-            if aside:
-                self.data['right'].append(html)
-            else:
-                self.data['center'].append((grid, html))
-
-    def load(self, request):
-        pass
-
-
-class AppDashboard(Dashboard):
-    def load(self, request):
-        self.tools(ExecuteQuery, ExecuteScript)
-
-
-class Dashboards:
-
-    def __init__(self, request):
-
-        self.request = request
-        self.data = dict(
-            info=[], warning=[], search=[], menu=[], links=[], shortcuts=[], cards=[],
-            floating=[], navigation=[], settings=[], center=[], right=[], actions=[], tools=[]
-        )
-        self.extra = dict(header={}, footer={})
-        self.apps = {}
-        self.data['navigation'].append(
-            dict(url='/app/', label='Principal', icon='house', app=None)
-        )
-        for cls in DASHBOARDS:
-            dashboard = cls(request)
-            if dashboard.redirect_url:
-                raise ReadyResponseException(HttpResponseRedirect(dashboard.redirect_url))
-            for key in dashboard.data:
-                self.data[key].extend(dashboard.data[key])
-            self.apps.update(dashboard.defined_apps)
-            if dashboard.extra:
-                self.extra.update(dashboard.extra)
-
-        if self.request.user.is_superuser:
-            self.superuser_search(self.data['search'])
-
-        for name in dashboard.enabled_apps:
-            self.apps[name]['enabled'] = True
-        if 'toggle-application' in request.GET:
-            for name in self.apps:
-                if name == request.GET['toggle-application']:
-                    if request.session.get('app_name') == name:
-                        del request.session['app_name']
-                        del request.session['app_icon']
-                    else:
-                        request.session['app_name'] = name
-                        request.session['app_icon'] = self.apps[name]['icon']
-                    request.session.save()
-                    break
-            raise ReadyResponseException(HttpResponseRedirect('/app/'))
-
-    def superuser_search(self, items):
-        from django.apps import apps
-        from .. import PROXIED_MODELS
-        for model in apps.get_models():
-            if model not in PROXIED_MODELS:
-                app_label = model.metaclass().app_label
-                model_name = model.metaclass().model_name
-                model_verbose_name_plural = model.metaclass().verbose_name_plural
-                icon = getattr(model.metaclass(), 'icon', None)
-                url = '/app/{}/{}/'.format(app_label, model_name)
-                add_item = True
-                for item in items:
-                    add_item = add_item and not item['url'] == url
-                if add_item:
-                    item = dict(label=pretty(str(model_verbose_name_plural)), description=None, url=url, icon=icon, subitems=[], app=None)
-                    items.append(item)
-        return items
+            return render_to_string('queryset/statistics.html', dict(data=serialized), request=self.request)
 
     def __str__(self):
-        return mark_safe(render_to_string('app/dashboard/dashboards.html', dict(data=self.data), request=self.request))
+        return self.html() if self.request else super().__str__()
 
+    def normalize(self, series):
+        if 'default' in series:
+            data = {'default': []}
+            total = sum([item[1] for item in series['default']])
+            start = 0
+            for item in series['default']:
+                percent = int(item[1] * 100 / total)
+                end = start + percent
+                data['default'].append(dict(
+                    description=item[0], percentage=percent,
+                    value=item[1], color=item[2], start=start, end=end
+                ))
+                start = end
+        else:
+            data = {}
+            max_value = 0
+            for key in series:
+                max_value = max(max([item[1] for item in series[key]]), max_value)
+            for key in series:
+                data[key] = []
+                total = sum([item[1] for item in series[key]])
+                for item in series[key]:
+                    data[key].append(dict(
+                        description=item[0], percentage=int(item[1] * 100 / total if total else 0),
+                        value=item[1], color=item[2]
+                    ))
+        return data
+
+    def chart(self, name):
+        self.metadata['template'] = 'charts/{}.html'.format(name)
+        return self
+
+    def pie_chart(self):
+        return self.chart('pie')
+
+    def donut_chart(self):
+        return self.chart('donut')
+
+    def bar_chart(self):
+        return self.chart('bar')
+
+    def column_chart(self):
+        return self.chart('column')
+
+    def nex_color(self):
+        color = colors()[self.cursor]
+        self.cursor += 1
+        if self.cursor == len(colors()):
+            self.cursor = 0
+        return color
 
+    def has_permission(self, user):
+        return user.is_superuser or self.qs.has_permission(user)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-sloth-0.0.54/sloth/app/static/css/all.min.css` & `django-sloth-0.1.0/sloth/api/static/css/all.min.css`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/css/bootstrap-icons.css` & `django-sloth-0.1.0/sloth/api/static/css/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/css/bootstrap.min.css` & `django-sloth-0.1.0/sloth/api/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/css/fonts/bootstrap-icons.woff` & `django-sloth-0.1.0/sloth/api/static/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/css/fonts/bootstrap-icons.woff2` & `django-sloth-0.1.0/sloth/api/static/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/css/icons.svg` & `django-sloth-0.1.0/sloth/api/static/css/icons.svg`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/css/images/ui-icons_444444_256x240.png` & `django-sloth-0.1.0/sloth/api/static/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/css/images/ui-icons_555555_256x240.png` & `django-sloth-0.1.0/sloth/api/static/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/css/jquery-ui.css` & `django-sloth-0.1.0/sloth/api/static/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/css/leaflet.css` & `django-sloth-0.1.0/sloth/api/static/css/leaflet.css`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/css/select2.min.css` & `django-sloth-0.1.0/sloth/api/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/css/trumbowyg.min.css` & `django-sloth-0.1.0/sloth/api/static/css/trumbowyg.min.css`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/icons/fontawesome/fontawesome.min.css` & `django-sloth-0.1.0/sloth/api/static/icons/fontawesome/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/icons/fontawesome/fontawesome.min.js` & `django-sloth-0.1.0/sloth/api/static/icons/fontawesome/fontawesome.min.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/icons/fontawesome/webfonts/fa-brands-400.ttf` & `django-sloth-0.1.0/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/icons/fontawesome/webfonts/fa-brands-400.woff2` & `django-sloth-0.1.0/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/icons/fontawesome/webfonts/fa-regular-400.ttf` & `django-sloth-0.1.0/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/icons/fontawesome/webfonts/fa-regular-400.woff2` & `django-sloth-0.1.0/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf` & `django-sloth-0.1.0/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2` & `django-sloth-0.1.0/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2` & `django-sloth-0.1.0/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2` & `django-sloth-0.1.0/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2` & `django-sloth-0.1.0/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/icons/materialicons/materialicons.css` & `django-sloth-0.1.0/sloth/api/static/icons/materialicons/materialicons.css`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2` & `django-sloth-0.1.0/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/images/click.png` & `django-sloth-0.1.0/sloth/api/static/images/click.png`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/images/hand.png` & `django-sloth-0.1.0/sloth/api/static/images/hand.png`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/images/icon.png` & `django-sloth-0.1.0/sloth/api/static/images/icon.png`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/images/icon.svg` & `django-sloth-0.1.0/sloth/api/static/images/icon.svg`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/images/images/badge.png` & `django-sloth-0.1.0/sloth/api/static/images/images/badge.png`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/images/images/icon.png` & `django-sloth-0.1.0/sloth/api/static/images/images/icon.png`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/images/login.jpeg` & `django-sloth-0.1.0/sloth/api/static/images/login.jpeg`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/images/logo.png` & `django-sloth-0.1.0/sloth/api/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/images/logo.svg` & `django-sloth-0.1.0/sloth/api/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/images/no-image.png` & `django-sloth-0.1.0/sloth/api/static/images/no-image.png`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/images/sloth.png` & `django-sloth-0.1.0/sloth/api/static/images/sloth.png`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/images/user.png` & `django-sloth-0.1.0/sloth/api/static/images/user.png`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/js/bootstrap.bundle.min.js` & `django-sloth-0.1.0/sloth/api/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/js/colorpick.min.js` & `django-sloth-0.1.0/sloth/api/static/js/colorpick.min.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/js/i18n/pt-BR.js` & `django-sloth-0.1.0/sloth/api/static/js/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/js/jquery-3.6.0.min.js` & `django-sloth-0.1.0/sloth/api/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/js/jquery-ui.js` & `django-sloth-0.1.0/sloth/api/static/js/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/js/jquery.binarytransport.js` & `django-sloth-0.1.0/sloth/api/static/js/jquery.binarytransport.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/js/jquery.mask.min.js` & `django-sloth-0.1.0/sloth/api/static/js/jquery.mask.min.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/js/jquery.timepicker.js` & `django-sloth-0.1.0/sloth/api/static/js/jquery.timepicker.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/js/leaflet.js` & `django-sloth-0.1.0/sloth/api/static/js/leaflet.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/js/masonry.pkgd.min.js` & `django-sloth-0.1.0/sloth/api/static/js/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/js/popper.min.js` & `django-sloth-0.1.0/sloth/api/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/js/qr-scanner-worker.min.js` & `django-sloth-0.1.0/sloth/api/static/js/qr-scanner-worker.min.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/js/qr-scanner.min.js` & `django-sloth-0.1.0/sloth/api/static/js/qr-scanner.min.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/js/qrcode.min.js` & `django-sloth-0.1.0/sloth/api/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/js/select2.min.js` & `django-sloth-0.1.0/sloth/api/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/static/js/sloth.js` & `django-sloth-0.1.0/sloth/api/static/js/sloth.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,7 @@
-$.datepicker.regional['pt-BR'] = {
-    monthNames: ['Janeiro', 'Fevereiro', 'Março', 'Abril', 'Maio', 'Junho', 'Julho', 'Agosto', 'Setembro', 'Outubro', 'Novembro', 'Dezembro'],
-    monthNamesShort: ['Jan', 'Fev', 'Mar', 'Abr', 'Mai', 'Jun', 'Jul', 'Ago', 'Set', 'Out', 'Nov', 'Dez'],
-    dayNames: ['Domingo', 'Segunda', 'Terça', 'Quarta', 'Quita', 'Sexta', 'Sábado'],
-    dayNamesShort: ['Dom', 'Seg', 'Ter', 'Qua', 'Qui', 'Sex', 'Sab'],
-    dayNamesMin: ['Do', 'Se', 'Te', 'Qu', 'Qu', 'Se', 'Sa']
-}
-$.datepicker.setDefaults(
-    $.extend({
-            'dateFormat': 'dd/mm/yy'
-        },
-        $.datepicker.regional['pt-BR']
-    )
-);
 jQuery.expr[':'].icontains = function(a, i, m) {
     return jQuery(a).text().toUpperCase()
         .indexOf(m[3].toUpperCase()) >= 0;
 };
 jQuery.fn.extend({
     request: function(url, method, data, callback, formcallback) {
         var xhr = $.ajax({
@@ -52,17 +38,18 @@
                     var a = document.createElement("a");
                     a.href = file;
                     if (contentType.indexOf('excel') >= 0) a.download = 'Download.xls';
                     else if (contentType.indexOf('pdf') >= 0) a.download = 'Download.pdf';
                     else if (contentType.indexOf('zip') >= 0) a.download = 'Download.zip';
                     else if (contentType.indexOf('json') >= 0) a.download = 'Download.json';
                     else if (contentType.indexOf('csv') >= 0) a.download = 'Download.csv';
+                    else if (contentType.indexOf('png') >= 0) a.download = 'Download.png';
                     document.body.appendChild(a);
                     a.click();
-                    $(document).back();
+                    $(document).back(true);
                 }
             },
             async: true,
             cache: true,
             contentType: false,
             processData: false,
             responseType: 'arraybuffer'
@@ -71,30 +58,58 @@
     open: function(url, method, data) {
         $(this).request(url, method || 'GET', data || {}, function(html) {
             $('main').html(html).initialize();
         });
     },
     popup: function(url, method, data) {
         $('.alert-dismissible').hide();
-        window['QUERYSET_RELOADER'] = window['reload' + $(this).data('uuid')];
         if (url.indexOf('?') > 0) url = url += '&modal=1'
         else url += '?modal=1'
         $(this).request(url, method || 'GET', data || {}, function(html) {
             $('#modal').find('.modal-body').html(html).initialize();
             if ($('.modal-body input[type=text]:first').length > 0) {
                 window.setTimeout(function() {
                     //$('.modal-body').find('input[type=text], input[type=number]').first().focus();
                 }, 200);
             }
             $('#modal').modal('show');
             document.getElementById('modal').addEventListener('hidden.bs.modal', function(event) {});
         });
     },
-    reload: function() {
-        document.location.reload();
+    reloadAreas(areas) {
+        if (areas != null) {
+            $('.reloadable-fieldset').map(function(i, item) {
+                if (areas.indexOf(item.id) >= 0 || areas.length == 0) {
+                    $.get($(item).data('path'), function(html) {
+                        if ($(item).find('.bi-chevron-right').length) {
+                            html = html.replace('bi-chevron-down', 'bi-chevron-right');
+                            console.log(html);
+                        }
+                        $(item).html(html).initialize();
+                    })
+                }
+            });
+            $('.reloadable-queryset').map(function(i, item) {
+                window['reload' + this.id]();
+            });
+        } else {
+            var url = document.location.pathname;
+            if ($(document).getCookie('current_tab')) url += '?tab=' + $(document).getCookie('current_tab');
+            $(document).open(url);
+        }
+        return this;
+    },
+    reload: function(id) {
+        if (id) {
+            $(this).request($(id).data('url'), 'GET', {}, function(html) {
+                $(id).html($(html).find(id).html()).initialize();
+            });
+        } else {
+            document.location.reload();
+        }
     },
     redirect: function(url) {
         $('#modal').modal('hide');
         document.location.href = url;
     },
     download: function(url) {
         alert(url);
@@ -103,30 +118,20 @@
         document.body.appendChild(a);
         a.click();
         $(document).back();
     },
     back: function(canceled) {
         if ($('#modal').is(':visible')) {
             $('#modal').modal('hide');
-            if (canceled == null) {
-                if (window['QUERYSET_RELOADER']) { // action in the scope of a queryset
-                    window['QUERYSET_RELOADER']();
-                    if (window['RELOAD_AREAS']) {
-                        // trigger refresh only if specific areas was defined
-                        if (window['RELOAD_AREAS'] != 'self') $(this).refresh(window['RELOAD_AREAS']);
-                    }
-                } else { // action in the scope of fieldset or object itself
-                    if (window['RELOAD_AREAS']) $(this).refresh(window['RELOAD_AREAS']);
-                }
-            }
         } else {
             //$(document).open(document.referrer);
             //window.history.pushState("string", "Title", document.referrer);
-            document.location.href = document.referrer;
+            if (!canceled) document.location.href = document.referrer;
         }
+        return this;
     },
     responsive: function() {
         $(this).find('.responsive-container > div').each(function(index) {
             var width = $(this).parent().width();
             if (width == 0) width = $(window).width(); // popup
             $(this).removeClass('n').removeClass('s').removeClass('m').removeClass('l');
             if (width > 900) {
@@ -147,15 +152,15 @@
         var match = document.cookie.match(new RegExp('(^| )' + name + '=([^;]+)'));
         if (match) return match[2];
     },
     setCookie: function(name, value) {
         document.cookie = name + "=" + value;
     },
     initialize: function() {
-        $(this).find('.popup').on('click', function(e) {
+        $(this).find('a.popup').on('click', function(e) {
             $(this).popup(this.href);
             e.preventDefault();
             return false;
         });
         $(this).find('.ajax').on('click', function(e) {
             $(this).open(this.href);
             e.preventDefault();
@@ -173,19 +178,15 @@
                     if (blob) {
                         data.delete(this.name);
                         data.append(this.name, blob, new Date().getTime() + '.' + blob.type.split('/')[1]);
                     }
                 });
             }
             $(document).request(form.action, method, data, function(html) {
-                if ($('#modal').is(':visible')) {
-                    $('#modal').find('.modal-body').html(html).initialize();
-                } else {
-                    $('main').html(html).initialize();
-                }
+                $(form).closest('.action-wrapper').html($(html).find('.action-wrapper').html()).initialize();
                 $(form).find('.btn-submit').removeClass('disabled').find('.spinner-border').addClass('d-none');
             });
             return false;
         });
         $(this).find('.field-controller').each(function(index) {
             var widgets = $('.' + this.name);
             $(this).on('click', function(e) {
@@ -240,28 +241,14 @@
                 placeholder: '',
                 ajax: ajax,
                 templateResult: function(item) {
                     return item.html ? $(item.html) : item.text
                 }
             }).on("select2:open", function(e) {});
         });
-        $(this).find('.date-input').not('.hasDatepicker').datepicker();
-        $(this).find('.date-time-input').not('.hasDatepicker').datetimepicker({
-            timeInput: true,
-            timeFormat: "hh:mm",
-            timeText: "Hora",
-            currentText: "Agora",
-            closeText: "Fechar"
-        });
-        $(this).find('.date-time-input').each(function() {
-            if (this.value) {
-                var tokens = this.value.split(':');
-                this.value = tokens[0] + ':' + tokens[1];
-            }
-        });
         $(this).find('.masked-input').each(function(index) {
             $(this).mask($(this).data('mask'), {
                 reverse: $(this).data('reverse')
             })
         });
         $(this).responsive();
         $(this).find('[data-toggle="tooltip"]').tooltip();
@@ -296,25 +283,28 @@
                     reader.readAsDataURL(imageFile);
                 }
             });
         });
         $(document).on('select2:open', () => {
             $(this).closest('.select2-search__field').focus();
         });
+        $('.fieldset-tab').map(function(i, item) {
+            var fieldsets = $(this).find('.reloadable-fieldset, .reloadable-queryset');
+            if (fieldsets.length == 1) fieldsets.find('.queryset-title, fieldset-title').hide();
+        });
         return this;
     },
+    areas: function() {
+        return $('.reloadable-fieldset').map(function(i, item) {
+            return item.id
+        }).get()
+    },
     refresh: function(areas) {
-        if (areas == 'self' || areas == 'True') {
-            var url = document.location.pathname;
-            if ($(document).getCookie('current_tab')) {
-                url += '?tab=' + $(document).getCookie('current_tab');
-            }
-            $(document).open(url);
-        } else {
-            var areas = areas.split(',');
+        if (areas.length == 0) areas = $(this).areas();
+        if (areas.length > 0) {
             var url = '?only=' + areas.join(',');
             $.get({
                 url: url,
                 success: function(html) {
                     $('.valueset-header').html($(html).find('.valueset-header'));
                     areas.forEach(function(attrName) {
                         var remote = $(html).find('#' + attrName);
@@ -327,14 +317,18 @@
                         }
                         remote.find('.fieldset-data').css('display', local.find('.fieldset-data').css('display'));
                         local.html(remote.html()).initialize();
                     });
                 }
             });
         }
+        // reload all querysets
+        $('.reloadable-queryset').map(function(i, item) {
+            window['reload' + this.id]();
+        });
     },
     dynamic: function(name, initial) {
         var form = $(this);
         var lastChangedValue = {};
         initial.hide.forEach(function(name) {
             form.find("input[name=" + name + "], select[name=" + name + "], textarea[name=" + name + "]").closest('.form-field').hide();
         });
@@ -375,79 +369,12 @@
             }
         );
     }
 });
 $(document).ready(function() {
     $(document).initialize();
     $('body').css('visibility', 'visible');
-    window['QUERYSET_RELOADER'] = window['RELOAD_AREAS'] = null;
     $(document).setCookie('current_tab', '');
 });
 $(window).resize(function() {
     $(document).responsive();
-});
-
-
-const applicationServerPublicKey = 'BLoLJSopQbe04v_zpegJmayhH2Px0EGzrFIlM0OedSOTYsMpO5YGmHOxbpPXdM09ttIuDaDTI86uC85JXZPpEtA';
-let swRegistration = null;
-
-function urlB64ToUint8Array(base64String) {
-    const padding = '='.repeat((4 - base64String.length % 4) % 4);
-    const base64 = (base64String + padding)
-        .replace(/\-/g, '+')
-        .replace(/_/g, '/');
-
-    const rawData = window.atob(base64);
-    const outputArray = new Uint8Array(rawData.length);
-
-    for (let i = 0; i < rawData.length; ++i) {
-        outputArray[i] = rawData.charCodeAt(i);
-    }
-    return outputArray;
-}
-
-if ('serviceWorker' in navigator && 'PushManager' in window) {
-    //console.log('Service Worker and Push is supported');
-    navigator.serviceWorker.register('/static/js/sw.js')
-        .then(function(swReg) {
-            //console.log('Service Worker is registered', swReg);
-            swRegistration = swReg;
-            //subscribeUser();
-        })
-        .catch(function(error) {
-            console.error('Service Worker Error', error);
-        });
-} else {
-    console.warn('Push messaging is not supported');
-}
-
-function subscribeUser() {
-    const applicationServerKey = urlB64ToUint8Array(applicationServerPublicKey);
-    swRegistration.pushManager.subscribe({
-        userVisibleOnly: true,
-        applicationServerKey: applicationServerKey
-    }).then(function(subscription) {
-        //console.log('User is subscribed:', subscription);
-        updateSubscriptionOnServer(subscription);
-    }).catch(function(err) {
-        //console.log('Failed to subscribe the user: ', err);
-    });
-}
-
-function updateSubscriptionOnServer(subscription) {
-    // TODO: Send subscription to application server
-    console.log(subscription);
-    subscriptionJson = JSON.stringify(subscription);
-    console.log(subscriptionJson);
-    if (subscription) {
-        console.log('inscrito');
-    } else {
-        console.log('não inscrito');
-    }
-    $.post('/app/push_subscription/', {
-            subscription: subscriptionJson
-        },
-        function(data) {
-            console.log(data);
-        }
-    );
-}
+});
```

### Comparing `django-sloth-0.0.54/sloth/app/static/js/sw.js` & `django-sloth-0.1.0/sloth/api/static/js/sw.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -12,14 +12,10 @@
     };
 
     event.waitUntil(self.registration.showNotification(title, options));
 });
 
 self.addEventListener('notificationclick', function(event) {
     console.log('[Service Worker] Notification click Received.');
-
     event.notification.close();
-
-    event.waitUntil(
-        clients.openWindow('http://petshop.aplicativo.click/app/login/')
-    );
+    //event.waitUntil(clients.openWindow('http://petshop.aplicativo.click/app/login/'));
 });
```

### Comparing `django-sloth-0.0.54/sloth/app/static/js/tests.js` & `django-sloth-0.1.0/sloth/api/static/js/tests.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -320,16 +320,16 @@
         }
         return element.parent()[0]
     }
     throw Error('Not found.')
 }
 
 function seeMessage(text) {
-    var message = $('.alert-success').first();
-    if (message.text().trim().indexOf(text) > 0) {
+    var message = $('.toast').first();
+    if (message.text().trim().indexOf(text) >= 0) {
         message.click();
         return message;
     } else {
         throw Error('Message not found.')
     }
 }
```

### Comparing `django-sloth-0.0.54/sloth/app/static/js/trumbowyg.min.js` & `django-sloth-0.1.0/sloth/api/static/js/trumbowyg.min.js`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/actions.html` & `django-sloth-0.1.0/sloth/api/templates/dashboard/actions.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 {% load tags %}
 {% if actions %}
-<div class="action-container" id="{{ target }}-{{ uuid }}-{{id}}">
-    {% if request|mobile or request|tablet %}
+<div class="action-container {{ target }}" id="{{ target }}-{{ uuid }}-{{id}}">
+    {% if compact or request|mobile or request|tablet or request.GET.compact %}
     {% with grouped_actions=actions|group_by_icon %}
         {% for action in grouped_actions.with_icon %}
             {% if  target != 'instance' or  target == 'instance' and action.key in enabled %}
-            <a href="/app{{ action.path }}"
-               data-url="/app{{ action.path }}"
+            <a href="{{ action.path }}"
+               data-url="{{ action.path }}"
                data-id="{{ id }}"
                data-uuid="{{ uuid }}"
                title="{{ action.submit }}"
                class="action-button btn btn-circle btn-outline-{{ action.style }} {{ target }} {% if target == 'queryset' %}disabled{% endif %} {% if action.modal %}popup{% endif %}">
                 {{ action.icon|icontag }}
             </a>
             {% endif %}
@@ -23,16 +23,16 @@
                     <i class="bi bi-three-dots text-primary"></i>
                 </a>
                 <ul class="dropdown-menu" aria-labelledby="dropdownMenuLink">
                     {% for action in grouped_actions.without_icon %}
                         {% if  target != 'instance' or  target == 'instance' and action.key in enabled %}
                         <li>
                             <a class="dropdown-item action-button {{ target }} {% if action.modal %}popup{% endif %}"
-                               href="/app{{ action.path }}"
-                               data-url="/app{{ action.path }}"
+                               href="{{ action.path }}"
+                               data-url="{{ action.path }}"
                                data-id="{{ id }}"
                                data-uuid="{{ uuid }}"
                                title="{{ action.submit }}">
                                 {{ action.icon|icontag }}
                                 {{ action.submit }}
                             </a>
                         </li>
@@ -42,40 +42,48 @@
             </div>
         {% endif %}
 
     {% endwith %}
     {% else %}
         {% for action in actions %}
             {% if  target != 'instance' or  target == 'instance' and action.key in enabled %}
-            <a href="/app{{ action.path }}"
-               data-url="/app{{ action.path }}"
+            <a href="{{ action.path }}"
+               data-url="{{ action.path }}"
                data-id="{{ id }}"
                data-uuid="{{ uuid }}"
                title="{{ action.submit }}"
                class="action-button btn btn-outline-{{ action.style }} {{ target }} {% if target == 'queryset' %}disabled{% endif %} {% if action.modal %}popup{% endif %}">
                 &nbsp;{{ action.icon|icontag }}
                 {% if target != 'instance' or not action.icon %}{{ action.submit }}{% endif %}&nbsp;
             </a>
             {% endif %}
         {% endfor %}
     {% endif %}
 </div>
 <script>
+    function actionURL(url){
+        var extra = '{{ request|post_querystring }}';
+        if(extra){
+            console.log(extra);
+            if(url.indexOf('?')>0) return url + '&' + extra;
+            else return url + '?' + extra;
+        } else { return url;}
+    }
     $('#{{ target }}-{{ uuid }}-{{id}}').find('.action-button').on('mouseenter', function(){
         if($(this).hasClass('instance')){
-            this.href = $(this).data('url').replace('{id}', $(this).data('id'));
+            this.href = actionURL($(this).data('url').replace('{id}', $(this).data('id')));
         }
         if($(this).hasClass('queryset')){
             var ids = $('#queryset-{{ uuid }}').find('.action-checkbox:checked').map(function(){
               return $(this).val();
             }).get().filter(function (id) { return id!='on' }).join('-');
-            this.href = $(this).data('url').replace('{id}', ids);
+            this.href = actionURL($(this).data('url').replace('{id}', '0-'+ids));
         }
         if($(this).hasClass('model')){
-            this.href = $(this).data('url');
+            this.href = actionURL($(this).data('url'));
         }
     });
 </script>
 {% endif %}
 
 
 <!--<script>document.getElementById('{{ target }}-{{ uuid }}').addEventListener('show.bs.dropdown', function () { $(this).find('ul').append(''); });</script>-->
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/base.html` & `django-sloth-0.1.0/sloth/api/templates/dashboard/base.html`

 * *Files 17% similar despite different names*

```diff
@@ -3,95 +3,77 @@
 <html lang="en">
   <head>
     <meta charset="utf-8">
     <meta name="viewport" content="minimal-ui, width=device-width, initial-scale=1, maximum-scale=1, user-scalable=0"/>
     <meta name="apple-mobile-web-app-capable" content="yes"/>
     <meta name="description" content="">
     <meta name="author" content="">
-    <title>{{ settings.SLOTH.NAME }}</title>
-    <link rel="manifest" href="/app/manifest/?v={{ settings.SLOTH.VERSION|stringformat:'s' }}">
-    {% if settings.SLOTH.ICON %}
-      <link rel="apple-touch-icon" sizes="128x128" href="{{ settings.SLOTH.ICON }}">
-    {% endif %}
-    {% if settings.SLOTH.FAVICON %}
-      <link rel="icon" sizes="192x192" href="{{ settings.SLOTH.FAVICON }}">
-    {% endif %}
+    <link rel="manifest" href="/app/manifest/?version={{ dashboard.data.footer.version }}">
     <link rel="stylesheet" href="/static/css/bootstrap.min.css">
     <link rel="stylesheet" href="/static/css/bootstrap-icons.css">
-    {% if 'materialicons' in settings.SLOTH.ICONS %}
-      <link rel="stylesheet" href="/static/icons/materialicons/materialicons.css">
-    {% endif %}
-    {% if 'fontawesome' in settings.SLOTH.ICONS %}
-      <link rel="stylesheet" href="/static/icons/fontawesome/fontawesome.min.css">
-    {% endif %}
     <link rel="stylesheet" href="/static/css/select2.min.css"/>
     <link rel="stylesheet" href="/static/css/colorpick.min.css">
     <link rel="stylesheet" href="/static/css/jquery-ui.css">
     <link rel="stylesheet" href="/static/css/trumbowyg.min.css"/>
     <link rel="stylesheet" href="/static/css/all.min.css"/>
-    <link rel="stylesheet" href="/static/css/sloth.css?v={{ settings.SLOTH.VERSION }}" />
+
+    {% if dashboard.data.navbar.title %}
+      <title>{{ dashboard.data.navbar.title }}</title>
+    {% endif %}
+    {% if dashboard.data.navbar.icon %}
+      <link rel="apple-touch-icon" sizes="128x128" href="{{ dashboard.data.navbar.icon }}">
+    {% endif %}
+    {% if dashboard.data.navbar.favicon %}
+      <link rel="icon" sizes="192x192" href="{{ dashboard.data.navbar.favicon }}">
+    {% endif %}
+
     <style>
-      body{
-        visibility:hidden;
-      }
-      main{
-        padding: {% if request|mobile %}0.25rem{% else %}1rem{% endif %}
-      }
+      body{visibility:hidden;}
+      main{padding: {% if request|mobile %}0.25rem{% else %}1rem{% endif %}}
     </style>
     {% if 0 %}
-      {% include "app/themes/dark.html" %}
+      {% include "themes/dark.html" %}
     {% endif %}
-    {% for url in settings.SLOTH.INCLUDE.CSS %}
-      <link rel="stylesheet" href="{{ url }}?v={{ settings.SLOTH.VERSION }}" />
+    {% for url in dashboard.data.styles %}
+      <link rel="stylesheet" href="{{ url }}?version={{ dashboard.data.footer.version }}" />
     {% endfor %}
 
     <script src="/static/js/jquery-3.6.0.min.js"></script>
     <script src="/static/js/select2.min.js"></script>
     <script src="/static/js/colorpick.min.js"></script>
     <script src="/static/js/i18n/pt-BR.js"></script>
     <script src="/static/js/popper.min.js"></script>
     <script src="/static/js/bootstrap.bundle.min.js"></script>
-    {% if 'fontawesome' in settings.SLOTH.ICONS %}
-      <script src="/static/icons/fontawesome/fontawesome.min.js"></script>
-    {% endif %}
     <script src="/static/js/jquery-ui.js"></script>
     <script src="/static/js/masonry.pkgd.min.js"></script>
-    <script src="/static/js/sloth.js?v=1.0.0"></script>
     <script src="/static/js/jquery.binarytransport.js"></script>
     <script src="/static/js/jquery.mask.min.js"></script>
-    <script src="/static/js/jquery.timepicker.js"></script>
     <script src="/static/js/trumbowyg.min.js"></script>
-
+    {% for url in dashboard.data.scripts %}
+      <script src="{{ url }}?version={{ dashboard.data.footer.version }}"></script>
+    {% endfor %}
     {% block extrahead %} {% endblock %}
 
   </head>
-  <body>
-
-    {% block header %}
-      {% include "app/dashboard/header.html" %}
-    {% endblock %}
+  <body id="{{ request.path|url_slug }}">
 
-    {% include "app/dashboard/menu.html" with data=dashboard.data %}
-    {% include "app/dashboard/links.html" with data=dashboard.data %}
+    {% block header %}{% include "dashboard/header.html" %}{% endblock %}
+    {% include "dashboard/menu.html" with data=dashboard.data %}
+    {% include "dashboard/links.html" with data=dashboard.data %}
 
       <main>
 {% endif %}
+
 {% block content %}
 {% endblock %}
-{% include "app/messages.html" %}
-{% for url in settings.SLOTH.INCLUDE.JS %}
-      <script src="{{ url }}?v={{ settings.SLOTH.VERSION }}"></script>
-{% endfor %}
-      <script src="/static/js/tests.js"></script>
+{% include "dashboard/messages.html" %}
 {% if not request|is_ajax %}
+        <script src="/static/js/tests.js"></script>
       </main>
-    {% if dashboard.data.menu %}
-
-    {% endif %}
     {% block footer %}
-    {% include "app/footer.html" %}
+    {% include "dashboard/footer.html" %}
     {% endblock %}
-    {% include "app/modal.html" %}
-    {% include "app/dashboard/bottom.html" %}
+    {% include "dashboard/modal.html" %}
+    {% include "dashboard/bottom.html" %}
   </body>
 </html>
 {% endif %}
```

#### html2text {}

```diff
@@ -1,33 +1,30 @@
 {% load tags %} {% if not request|is_ajax %}
 
 
 
 
- {% if settings.SLOTH.ICON %}
- {% endif %} {% if settings.SLOTH.FAVICON %}
- {% endif %}
 
- {% if 'materialicons' in settings.SLOTH.ICONS %}
- {% endif %} {% if 'fontawesome' in settings.SLOTH.ICONS %}
- {% endif %}
 
 
 
 
 
- {% if 0 %} {% include "app/themes/dark.html" %} {% endif %} {% for url in
-settings.SLOTH.INCLUDE.CSS %}
- {% endfor %}
- {% if 'fontawesome' in settings.SLOTH.ICONS %}
+
+
+ {% if dashboard.data.navbar.title %}
+{% endif %} {% if dashboard.data.navbar.icon %}
+ {% endif %} {% if dashboard.data.navbar.favicon %}
  {% endif %}
- {% block extrahead %} {% endblock %}
-{% block header %} {% include "app/dashboard/header.html" %} {% endblock %} {%
-include "app/dashboard/menu.html" with data=dashboard.data %} {% include "app/
-dashboard/links.html" with data=dashboard.data %}  {% endif %} {% block content
-%} {% endblock %} {% include "app/messages.html" %} {% for url in
-settings.SLOTH.INCLUDE.JS %}
+ {% if 0 %} {% include "themes/dark.html" %} {% endif %} {% for url in
+dashboard.data.styles %}
  {% endfor %}
- {% if not request|is_ajax %}  {% if dashboard.data.menu %} {% endif %} {%
-block footer %} {% include "app/footer.html" %} {% endblock %} {% include "app/
-modal.html" %} {% include "app/dashboard/bottom.html" %}
+ {% for url in dashboard.data.scripts %}
+ {% endfor %} {% block extrahead %} {% endblock %}
+{% block header %}{% include "dashboard/header.html" %}{% endblock %} {%
+include "dashboard/menu.html" with data=dashboard.data %} {% include
+"dashboard/links.html" with data=dashboard.data %}  {% endif %} {% block
+content %} {% endblock %} {% include "dashboard/messages.html" %} {% if not
+request|is_ajax %}
+  {% block footer %} {% include "dashboard/footer.html" %} {% endblock %} {%
+include "dashboard/modal.html" %} {% include "dashboard/bottom.html" %}
 {% endif %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/charts/bar.html` & `django-sloth-0.1.0/sloth/api/templates/charts/bar.html`

 * *Files 1% similar despite different names*

```diff
@@ -59,11 +59,11 @@
 </style>
 <div class="bar-chart">
     <dl class="barchart">
         {% for serie in series %}
         <dd class="percentage percentage-{{ forloop.counter }}"><span class="text">{{ serie.description }}</span></dd>
         {% endfor %}
     </dl>
-    {% include "app/charts/legend.html" %}
+    {% include "charts/legend.html" %}
 </div>
 <div class="clearfix"></div>
 {% endfor %}
```

#### html2text {}

```diff
@@ -1,4 +1,4 @@
 {% for key, series in data.normalized.items %}
 {% for serie in series %}
-{% include "app/charts/legend.html" %}
+{% include "charts/legend.html" %}
 {% endfor %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/charts/column.html` & `django-sloth-0.1.0/sloth/api/templates/charts/column.html`

 * *Files 2% similar despite different names*

```diff
@@ -102,13 +102,13 @@
         <div class="tick" style="height: 60px;"><p>60</p></div>
         <div class="tick" style="height: 60px;"><p>40</p></div>
         <div class="tick" style="height: 60px;"><p>20</p></div>
         <div class="tick" style="height: 60px; border-bottom:none"><p>0</p></div>
     </div>
     {% for key, series in data.normalized.items %}
     {% if forloop.first %}
-        {% include "app/charts/legend.html" %}
+        {% include "charts/legend.html" %}
     {% endif %}
     {% endfor %}
 </div>
 </div>
 <div class="clearfix"></div>
```

#### html2text {}

```diff
@@ -3,8 +3,8 @@
 100
 80
 60
 40
 20
 0
 {% for key, series in data.normalized.items %} {% if forloop.first %} {%
-include "app/charts/legend.html" %} {% endif %} {% endfor %}
+include "charts/legend.html" %} {% endif %} {% endfor %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/charts/pie.html` & `django-sloth-0.1.0/sloth/api/templates/charts/pie.html`

 * *Files 15% similar despite different names*

```diff
@@ -14,44 +14,34 @@
             {% if forloop.last %}
               {{ serie.color }} 0
             {% endif %}
           {% endfor %}
         );
       margin: auto;
       border-radius: 50%;
-     {% if compact or data.metadata.compact or request.GET.compact or request|mobile %}
-          width: 150;
-          height: 150;
-          margin-top: -62px;
-     {% else %}
-          width: 300;
-          height: 300;
-          margin-top: -125px;
-     {% endif %}
+      width: 150;
+      height: 150;
+      margin-top: -62px;
     }
     #container-{{ forloop.counter }} .pie-center{
-      {% if compact or data.metadata.compact or request.GET.compact or request|mobile %}
-          top: 50px;
-          width: 75px;
-          height: 75px;
-      {% else %}
-          top: 100px;
-          width: 150px;
-          height: 150px;
-      {% endif %}
+
+      top: 50px;
+      width: 75px;
+      height: 75px;
+
       position: relative;
       background: #FFF;
       border-radius: 50%;
       margin: auto;
       {% if donut is None %}visibility: hidden;{% endif %}
     }
 </style>
 <div style="width:100%" id="container-{{ forloop.counter }}">
     {% if key != 'default' %}
     <h5>{{ key }}</h5>
     {% endif %}
     <div class="pie-center"></div>
     <div class="pie-chart"></div>
-    {% include "app/charts/legend.html" %}
+    {% include "charts/legend.html" %}
 </div>
 <div class="clearfix"></div>
 {% endfor %}
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
 {% load tags %} {% for key, series in data.normalized.items %}
 {% if key != 'default' %}
 ** {{ key }} **
 {% endif %}
-{% include "app/charts/legend.html" %}
+{% include "charts/legend.html" %}
 {% endfor %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/dashboard/apps.html` & `django-sloth-0.1.0/sloth/api/templates/dashboard/apps.html`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/dashboard/bottom.html` & `django-sloth-0.1.0/sloth/api/templates/dashboard/bottom.html`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/dashboard/cards.html` & `django-sloth-0.1.0/sloth/api/templates/dashboard/cards.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 {% load tags %}
+{% if cards %}
 <style>
     .single_quick_activity .count_content {
         margin-left: 30px;
         text-align: left;
     }
     .single_quick_activity {
-        border-radius: 10px;
         -webkit-transition: 0.5s;
         padding: 10px;
         align-items: center;
         justify-content: center;
         margin-bottom: 10px;
         height: 120px;
-        box-shadow: 0 0.375rem 0.75rem rgb(140 152 164 / 8%);
-        border: 0.0625rem solid rgba(231,234,243,.7);
         transition: .3s;
     }
     .single_quick_activity i{
         font-size: 90px;
         float:left;
         margin-left: 20px;
         margin-right: 20px;
     }
 </style>
 
-<div class="row">
-    {% for item in data.cards %}
+<div class="row cards-wrapper">
+    {% for item in cards %}
         <div class="col-sm-12 col-md-6 col-lg-4" style="padding:3px">
             <a href="{{ item.url }}" style="text-decoration:none">
             <div class="single_quick_activity">
                 <div class="icon">
                     {{ item.icon|icontag }}
                 </div>
                 <div class="count_content">
@@ -37,7 +35,8 @@
                     <p class="text-primary">{{ item.label }}</p>
                 </div>
             </div>
             </a>
         </div>
     {% endfor %}
 </div>
+{% endif %}
```

#### html2text {}

```diff
@@ -1,6 +1,7 @@
-{% load tags %}
-{% for item in data.cards %}
+{% load tags %} {% if cards %}
+{% for item in cards %}
 {{_item.icon|icontag_}}
 ****_{{_item.count_}}_****
 {{_item.label_}}
 {% endfor %}
+{% endif %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/dashboard/grids.html` & `django-sloth-0.1.0/sloth/api/templates/dashboard/grids.html`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/dashboard/header.html` & `django-sloth-0.1.0/sloth/api/templates/dashboard/header.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 {% load tags %}
-{% if not request.GET.modal %}
-    {% if dashboard.extra.header.shadow %}
+{% if request.user.is_authenticated and not request.GET.modal %}
+    {% if dashboard.data.header.shadow %}
       <style>
         .navbar {box-shadow: 0 .125rem .25rem rgba(0,0,0,.075);}
       </style>
     {% endif %}
     <nav class="navbar navbar-expand">
       <div class="container-fluid">
-        <a class="navbar-brand" href="/app/">
-          {% if dashboard.extra.header.logo %}
-            <img height="30" src="{{ dashboard.extra.header.logo }}" style="border-radius:3px;">
+        <a class="navbar-brand" href="/app/dashboard/">
+          {% if dashboard.data.header.logo %}
+            <img height="30" src="{{ dashboard.data.header.logo }}" style="border-radius:3px;">
           {% endif %}
-          {% if dashboard.extra.header.title %}
-            <span>{{ dashboard.extra.header.title }}</span>
+          {% if dashboard.data.header.title %}
+            <span>{{ dashboard.data.header.title }}</span>
           {% endif %}
         </a>
-        {% if dashboard.extra.header.text and not request|mobile %}
-          {{ dashboard.extra.header.text }}
+        {% if dashboard.data.header.text and not request|mobile %}
+          {{ dashboard.data.header.text }}
         {% endif %}
 
         <div class="collapse navbar-collapse">
           <ul class="navbar-nav">
             {% for action in dashboard.data.actions %}
               <li class="nav-item">
                 <a class="nav-link" href="{{ action.url }}">
@@ -29,18 +29,20 @@
                 </a>
               </li>
             {% endfor %}
           </ul>
         </div>
 
         <div class="collapse navbar-collapse">
-          {% include "app/dashboard/search.html" %}
-          {% include "app/dashboard/tools.html" %}
-          {% include "app/dashboard/apps.html" %}
+          {% include "dashboard/search.html" %}
+          {% include "dashboard/tools.html" %}
+          {% include "dashboard/tasks.html" %}
+          {% include "dashboard/plus.html" %}
+          {% include "dashboard/apps.html" %}
           {% if request.user.is_authenticated %}
-          {% include "app/dashboard/settings.html" %}
+          {% include "dashboard/settings.html" %}
           {% endif %}
         </div>
 
       </div>
     </nav>
 {% endif %}
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
-{% load tags %} {% if not request.GET.modal %} {% if
-dashboard.extra.header.shadow %}
+{% load tags %} {% if request.user.is_authenticated and not request.GET.modal
+%} {% if dashboard.data.header.shadow %}
  {% endif %}
-{%_if_dashboard.extra.header.logo_%}_[{{_dashboard.extra.header.logo_}}]_{%
-endif_%}_{%_if_dashboard.extra.header.title_%}_{{_dashboard.extra.header.title
-}}_{%_endif_%} {% if dashboard.extra.header.text and not request|mobile %} {
-{ dashboard.extra.header.text }} {% endif %}
+{%_if_dashboard.data.header.logo_%}_[{{_dashboard.data.header.logo_}}]_{%_endif
+%}_{%_if_dashboard.data.header.title_%}_{{_dashboard.data.header.title_}}_{%
+endif_%} {% if dashboard.data.header.text and not request|mobile %} {
+{ dashboard.data.header.text }} {% endif %}
     * {% for action in dashboard.data.actions %}
     * {{_action.icon|icontag_}}_{{_action.label_}}
     * {% endfor %}
-{% include "app/dashboard/search.html" %} {% include "app/dashboard/tools.html"
-%} {% include "app/dashboard/apps.html" %} {% if request.user.is_authenticated
-%} {% include "app/dashboard/settings.html" %} {% endif %}
+{% include "dashboard/search.html" %} {% include "dashboard/tools.html" %} {%
+include "dashboard/tasks.html" %} {% include "dashboard/plus.html" %} {%
+include "dashboard/apps.html" %} {% if request.user.is_authenticated %} {%
+include "dashboard/settings.html" %} {% endif %}
  {% endif %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/dashboard/links.html` & `django-sloth-0.1.0/sloth/api/templates/dashboard/links.html`

 * *Files 16% similar despite different names*

```diff
@@ -4,29 +4,28 @@
     .app-title{
         float: left;
         font-size: 1.1rem;
     }
     .app-links-wrapper{
         float: right;
         text-align: right;
-        margin-bottom: 30px;
     }
     .app-links-wrapper a{
         margin: 5px;
         text-decoration: none;
     }
 </style>
 
 <div class="app-links m-2">
     <div class="app-title">
         {{ request.session.app_icon|icontag }} {{ request.session.app_name }}
     </div>
     <div class="app-links-wrapper">
     {% for item in data.links %}
-        <a href="{{ item.url }}" class="shortcut-link">
+        <a href="{{ item.url }}" class="shortcut-link {% if item.modal %}popup{% endif %}">
             {{ item.label }}
         </a>
     {% endfor %}
     </div>
 </div>
 <div class="clearfix"></div>
 {% endif %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/dashboard/search.html` & `django-sloth-0.1.0/sloth/api/templates/dashboard/search.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% load tags %}
 <input class="form-control me-2" id="search" name="search" type="search" placeholder="Buscar..." aria-label="Search" onclick="search(this)" onkeyup="search(this)" onfocus="search(this)" style="{% if not dashboard.data.search  %}visibility:hidden{% endif %}">
 <div class="search-results d-none" onmouseleave="$(this).addClass('d-none')">
 <ul class="list-group search-menu">
   {% for item in dashboard.data.search %}
   <li class="list-group-item d-flex justify-content-between align-items-start">
     <div class="ms-2 me-auto">
-      <div class="fw-bold">
+      <div>
         {% if item.subitems %}
           {{ item.label }}
         {% else %}
         <a class="item" href="{{ item.url }}">
           {{ item.label }}
         </a>
         {% endif %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/dashboard/shortcuts.html` & `django-sloth-0.1.0/sloth/api/templates/dashboard/shortcuts.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% load tags %}
-{% if data.shortcuts %}
+{% if shortcuts %}
 <style>
 .shortcut-wrapper {
     display: flex;
     flex-direction: row;
     flex-wrap: wrap;
     justify-content: center;
     align-content: stretch;
@@ -18,15 +18,15 @@
 }
 .shortcut-wrapper .shortcut-link i, .shortcut-wrapper .shortcut-link span{
     font-size: 2rem;
 }
 </style>
 
 <div class="shortcut-wrapper">
-{% for item in data.shortcuts %}
+{% for item in shortcuts %}
     <a href="{{ item.url }}" class="shortcut-link">
         <div>
           {{ item.icon|icontag }}
           <p>{{ item.label }}</p>
         </div>
     </a>
 {% endfor %}
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
-{% load tags %} {% if data.shortcuts %}
-{% for item in data.shortcuts %}
+{% load tags %} {% if shortcuts %}
+{% for item in shortcuts %}
 {{_item.icon|icontag_}}
 {{_item.label_}}
  {% endfor %}
 {% endif %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/dashboard/tools.html` & `django-sloth-0.1.0/sloth/api/templates/dashboard/plus.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,17 @@
 {% load tags %}
-{% if dashboard.data.tools %}
+{% if dashboard.data.plus %}
 <ul class="navbar-nav">
-  <li class="nav-item dropdown settings-dropdown">
+  <li class="nav-item dropdown add-dropdown">
     <a class="nav-link" href="#" id="navbarToolsDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false" title="Ferramentas" name="tools">
-      <i class="bi bi-tools"></i>
+      <i class="bi bi-plus-square"></i>
     </a>
     <ul class="dropdown-menu dropdown-menu-end" aria-labelledby="navbarToolsDropdown">
-      {% if request.user.is_superuser %}
-        <li>
-          <a target="_blank" class="dropdown-item" href="/app/icons/">
-            <i class="bi bi-palette"></i>
-            Ícones
-          </a>
-        </li>
-        <li><hr class="dropdown-divider"></li>
-      {% endif %}
-      {% for item in dashboard.data.tools %}
-      <li>
+      {% for item in dashboard.data.plus %}
+      <li style="text-align:center">
         <a class="dropdown-item {% if item.modal %}popup{% endif %}" href="{{ item.url }}">
           {{ item.icon|icontag }}
           {{ item.label }}
         </a>
       </li>
       {% endfor %}
     </ul>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/footer.html` & `django-sloth-0.1.0/sloth/api/templates/dashboard/footer.html`

 * *Files 20% similar despite different names*

```diff
@@ -6,22 +6,22 @@
     footer .footer-title{
         font-size: 90%;
     }
     footer .footer-text{
         font-size: 75%;
     }
 </style>
-{% if dashboard.extra.footer.title %}
+{% if dashboard.data.footer.title %}
     <footer>
         <div class="footer-title">
-            {{ dashboard.extra.footer.title }}
+            {{ dashboard.data.footer.title }}
         </div>
-        {% if dashboard.extra.footer.text %}
+        {% if dashboard.data.footer.text %}
             <div class="footer-text">
-                <div>{{ dashboard.extra.footer.text }}</div>
-                {% if dashboard.extra.footer.version %}
-                    <div>Versão {{ dashboard.extra.footer.version|stringformat:'s' }}</div>
+                <div>{{ dashboard.data.footer.text }}</div>
+                {% if dashboard.data.footer.version %}
+                    <div>Versão {{ dashboard.data.footer.version|stringformat:'s' }}</div>
                 {% endif %}
             </div>
         {% endif %}
     </footer>
 {% endif %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
- {% if dashboard.extra.footer.title %}
-{{ dashboard.extra.footer.title }}
-{% if dashboard.extra.footer.text %}
-{{ dashboard.extra.footer.text }}
-{% if dashboard.extra.footer.version %}
-VersÃ£o {{ dashboard.extra.footer.version|stringformat:'s' }}
+ {% if dashboard.data.footer.title %}
+{{ dashboard.data.footer.title }}
+{% if dashboard.data.footer.text %}
+{{ dashboard.data.footer.text }}
+{% if dashboard.data.footer.version %}
+VersÃ£o {{ dashboard.data.footer.version|stringformat:'s' }}
 {% endif %}
 {% endif %}  {% endif %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/inputs/picker.html` & `django-sloth-0.1.0/sloth/api/templates/inputs/picker.html`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/inputs/qrcode.html` & `django-sloth-0.1.0/sloth/api/templates/inputs/qrcode.html`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/modal.html` & `django-sloth-0.1.0/sloth/api/templates/dashboard/modal.html`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 		left: 0px;
     }
 	.modal.right .modal-dialog {
 		right: 0px;
 	}
 </style>
 <div class="modal" id="modal" aria-labelledby="exampleModalLabel" aria-hidden="true">
-  <div class="modal-dialog modal-dialog-centered" style="max-width:90%">
+  <div class="modal-dialog modal-dialog-centered" style="max-width:90%;width:800">
     <div class="modal-content">
       <div class="modal-body">
 
       </div>
     </div>
   </div>
 </div>
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/queryset/accordion.html` & `django-sloth-0.1.0/sloth/api/templates/queryset/accordion.html`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,24 @@
           <button class="accordion-button {% if True or not forloop.first %}collapsed{% endif %}" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne{{ data.uuid }}{{ forloop.counter }}" aria-expanded="true" aria-controls="collapseOne{{ data.uuid }}{{ forloop.counter }}">
             {{ row.description }}
           </button>
         </h2>
         <div id="collapseOne{{ data.uuid }}{{ forloop.counter }}" class="accordion-collapse collapse {% if False and forloop.first %}_show{% endif %}" aria-labelledby="heading{{ forloop.counter }}" data-bs-parent="#accordion{{ data.uuid }}">
           <div class="accordion-body">
             <div class="float-end">
-                {% include "app/queryset/checkbox.html" %}
+                {% include "queryset/checkbox.html" %}
             </div>
             <dl>
-            {% for k, v in row.data.items %}
-                <dt>{{ k }}</dt>
-                <dd>{% include 'app/valueset/value.html' %}</dd>
+            {% for v in row.data.values %}
+                <dt>{{ v.name }}</dt>
+                <dd>{% include 'valueset/value.html' %}</dd>
             {% endfor %}
             </dl>
             <div class="float-end">
-                {% include "app/actions.html" with uuid=data.uuid target="instance" actions=data.actions.instance id=row.id|stringformat:'s' enabled=row.actions  %}
+                {% include "dashboard/actions.html" with uuid=data.uuid target="instance" actions=data.actions.instance id=row.id|stringformat:'s' enabled=row.actions  %}
             </div>
             <div class="clearfix"></div>
           </div>
         </div>
       </div>
       {% endfor %}
     </div>
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/queryset/calendar.html` & `django-sloth-0.1.0/sloth/api/templates/queryset/calendar.html`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/queryset/cards.html` & `django-sloth-0.1.0/sloth/api/templates/queryset/datatable.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,146 @@
 00000000: 7b25 206c 6f61 6420 7461 6773 2025 7d0a  {% load tags %}.
-00000010: 0a7b 2520 6966 2064 6174 612e 6461 7461  .{% if data.data
-00000020: 2025 7d0a 3c64 6976 2063 6c61 7373 3d22   %}.<div class="
-00000030: 726f 7722 2069 643d 2272 6f77 2d7b 7b20  row" id="row-{{ 
-00000040: 6461 7461 2e75 7569 6420 7d7d 223e 0a20  data.uuid }}">. 
-00000050: 2020 207b 2520 7769 7468 2069 6d61 6765     {% with image
-00000060: 5f6b 6579 3d64 6174 612e 6461 7461 2e30  _key=data.data.0
-00000070: 2e64 6174 617c 696d 6167 655f 6b65 7920  .data|image_key 
-00000080: 257d 0a20 2020 2020 2020 207b 2520 666f  %}.        {% fo
-00000090: 7220 726f 7720 696e 2064 6174 612e 6461  r row in data.da
-000000a0: 7461 2025 7d0a 2020 2020 2020 2020 3c64  ta %}.        <d
-000000b0: 6976 2063 6c61 7373 3d22 7b25 2069 6620  iv class="{% if 
-000000c0: 6e6f 7420 636f 6d70 6163 7420 257d 636f  not compact %}co
-000000d0: 6c2d 736d 2d31 3220 636f 6c2d 6d64 2d34  l-sm-12 col-md-4
-000000e0: 2063 6f6c 2d6c 672d 337b 2520 656e 6469   col-lg-3{% endi
-000000f0: 6620 257d 223e 0a20 2020 2020 2020 2020  f %}">.         
-00000100: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
-00000110: 6172 6422 2073 7479 6c65 3d22 6d61 7267  ard" style="marg
-00000120: 696e 2d62 6f74 746f 6d3a 2031 3070 7822  in-bottom: 10px"
-00000130: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000140: 2020 7b25 2069 6620 696d 6167 655f 6b65    {% if image_ke
-00000150: 7920 257d 0a20 2020 2020 2020 2020 2020  y %}.           
-00000160: 2020 2020 2020 2020 207b 2520 666f 7220           {% for 
-00000170: 6b2c 2076 2069 6e20 726f 772e 6461 7461  k, v in row.data
-00000180: 2e69 7465 6d73 2025 7d0a 2020 2020 2020  .items %}.      
+00000010: 7b25 2069 6620 6461 7461 2e64 6174 6120  {% if data.data 
+00000020: 257d 0a20 2020 207b 2520 6966 2063 6f6d  %}.    {% if com
+00000030: 7061 6374 206f 7220 6461 7461 2e6d 6574  pact or data.met
+00000040: 6164 6174 612e 636f 6d70 6163 7420 6f72  adata.compact or
+00000050: 2072 6571 7565 7374 2e47 4554 2e63 6f6d   request.GET.com
+00000060: 7061 6374 206f 7220 7265 7175 6573 747c  pact or request|
+00000070: 6d6f 6269 6c65 206f 7220 7265 7175 6573  mobile or reques
+00000080: 747c 7461 626c 6574 2061 6e64 2064 6174  t|tablet and dat
+00000090: 612e 6d65 7461 6461 7461 2e64 6973 706c  a.metadata.displ
+000000a0: 6179 7c6c 656e 6774 6820 3e20 3220 257d  ay|length > 2 %}
+000000b0: 0a20 2020 2020 2020 203c 6872 3e0a 2020  .        <hr>.  
+000000c0: 2020 2020 2020 7b25 2066 6f72 2072 6f77        {% for row
+000000d0: 2069 6e20 6461 7461 2e64 6174 6120 257d   in data.data %}
+000000e0: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
+000000f0: 7620 636c 6173 733d 2266 6c6f 6174 2d65  v class="float-e
+00000100: 6e64 223e 0a20 2020 2020 2020 2020 2020  nd">.           
+00000110: 2020 2020 207b 2520 696e 636c 7564 6520       {% include 
+00000120: 2271 7565 7279 7365 742f 6368 6563 6b62  "queryset/checkb
+00000130: 6f78 2e68 746d 6c22 2025 7d0a 2020 2020  ox.html" %}.    
+00000140: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00000150: 2020 2020 2020 2020 2020 203c 646c 3e0a             <dl>.
+00000160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000170: 7b25 2066 6f72 2076 2069 6e20 726f 772e  {% for v in row.
+00000180: 6461 7461 2e76 616c 7565 7320 257d 0a20  data.values %}. 
 00000190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000001a0: 2020 7b25 2069 6620 6b20 3d3d 2069 6d61    {% if k == ima
-000001b0: 6765 5f6b 6579 2025 7d0a 2020 2020 2020  ge_key %}.      
-000001c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000001d0: 2020 2020 2020 3c69 6d67 2063 6c61 7373        <img class
-000001e0: 3d22 6361 7264 2d69 6d67 2d74 6f70 2220  ="card-img-top" 
-000001f0: 7372 633d 227b 7b20 762e 7661 6c75 657c  src="{{ v.value|
-00000200: 696d 6167 655f 7372 6320 7d7d 223e 0a20  image_src }}">. 
-00000210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000220: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
-00000230: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00000240: 2020 2020 2020 207b 2520 656e 6466 6f72         {% endfor
-00000250: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00000260: 2020 2020 7b25 2065 6e64 6966 2025 7d0a      {% endif %}.
-00000270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000280: 3c64 6976 2063 6c61 7373 3d22 6361 7264  <div class="card
-00000290: 2d62 6f64 7922 3e0a 2020 2020 2020 2020  -body">.        
-000002a0: 2020 2020 2020 2020 2020 2020 3c68 3520              <h5 
-000002b0: 636c 6173 733d 2263 6172 642d 7469 746c  class="card-titl
-000002c0: 6520 7465 7874 2d63 656e 7465 7222 3e7b  e text-center">{
-000002d0: 7b20 726f 772e 6465 7363 7269 7074 696f  { row.descriptio
-000002e0: 6e20 7d7d 3c2f 6835 3e0a 2020 2020 2020  n }}</h5>.      
-000002f0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00000300: 6976 2063 6c61 7373 3d22 666c 6f61 742d  iv class="float-
-00000310: 656e 6422 3e0a 2020 2020 2020 2020 2020  end">.          
-00000320: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00000330: 2069 6e63 6c75 6465 2022 6170 702f 7175   include "app/qu
-00000340: 6572 7973 6574 2f63 6865 636b 626f 782e  eryset/checkbox.
-00000350: 6874 6d6c 2220 257d 0a20 2020 2020 2020  html" %}.       
-00000360: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00000370: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00000380: 2020 2020 2020 2020 3c64 6c3e 0a20 2020          <dl>.   
-00000390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003a0: 2020 2020 207b 2520 666f 7220 6b2c 2076       {% for k, v
-000003b0: 2069 6e20 726f 772e 6461 7461 2e69 7465   in row.data.ite
-000003c0: 6d73 2025 7d0a 2020 2020 2020 2020 2020  ms %}.          
-000003d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003e0: 2020 7b25 2069 6620 6b20 213d 2069 6d61    {% if k != ima
-000003f0: 6765 5f6b 6579 2025 7d0a 2020 2020 2020  ge_key %}.      
-00000400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000410: 2020 2020 2020 2020 2020 3c64 743e 7b7b            <dt>{{
-00000420: 206b 207d 7d3c 2f64 743e 0a20 2020 2020   k }}</dt>.     
-00000430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000440: 2020 2020 2020 2020 2020 203c 6464 3e7b             <dd>{
-00000450: 2520 696e 636c 7564 6520 2761 7070 2f76  % include 'app/v
-00000460: 616c 7565 7365 742f 7661 6c75 652e 6874  alueset/value.ht
-00000470: 6d6c 2720 257d 3c2f 6464 3e0a 2020 2020  ml' %}</dd>.    
-00000480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000490: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-000004a0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-000004b0: 2020 2020 2020 2020 2020 2020 7b25 2065              {% e
-000004c0: 6e64 666f 7220 257d 0a20 2020 2020 2020  ndfor %}.       
-000004d0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-000004e0: 6c3e 0a20 2020 2020 2020 2020 2020 2020  l>.             
-000004f0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00000500: 733d 2266 6c6f 6174 2d65 6e64 223e 0a20  s="float-end">. 
-00000510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000520: 2020 2020 2020 207b 2520 696e 636c 7564         {% includ
-00000530: 6520 2261 7070 2f61 6374 696f 6e73 2e68  e "app/actions.h
-00000540: 746d 6c22 2077 6974 6820 7575 6964 3d64  tml" with uuid=d
-00000550: 6174 612e 7575 6964 2074 6172 6765 743d  ata.uuid target=
-00000560: 2269 6e73 7461 6e63 6522 2061 6374 696f  "instance" actio
-00000570: 6e73 3d64 6174 612e 6163 7469 6f6e 732e  ns=data.actions.
-00000580: 696e 7374 616e 6365 2069 643d 726f 772e  instance id=row.
-00000590: 6964 7c73 7472 696e 6766 6f72 6d61 743a  id|stringformat:
-000005a0: 2773 2720 656e 6162 6c65 643d 726f 772e  's' enabled=row.
-000005b0: 6163 7469 6f6e 7320 257d 0a20 2020 2020  actions %}.     
-000005c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000005d0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-000005e0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-000005f0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00000600: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00000610: 2020 2020 2020 207b 2520 656e 6466 6f72         {% endfor
-00000620: 2025 7d0a 2020 2020 7b25 2065 6e64 7769   %}.    {% endwi
-00000630: 7468 2025 7d0a 3c2f 6469 763e 0a7b 2520  th %}.</div>.{% 
-00000640: 656c 7365 2025 7d0a 3c64 6976 2063 6c61  else %}.<div cla
-00000650: 7373 3d22 616c 6572 7420 616c 6572 742d  ss="alert alert-
-00000660: 7072 696d 6172 7922 2072 6f6c 653d 2261  primary" role="a
-00000670: 6c65 7274 2220 7374 796c 653d 226d 6172  lert" style="mar
-00000680: 6769 6e2d 746f 703a 3330 7078 3b22 3e0a  gin-top:30px;">.
-00000690: 2020 2020 4e65 6e68 756d 2072 6567 6973      Nenhum regis
-000006a0: 7472 6f20 656e 636f 6e74 7261 646f 2e0a  tro encontrado..
-000006b0: 3c2f 6469 763e 0a7b 2520 656e 6469 6620  </div>.{% endif 
-000006c0: 257d                                     %}
+000001a0: 2020 203c 6474 3e3c 6c61 6265 6c3e 7b7b     <dt><label>{{
+000001b0: 2076 2e6e 616d 6520 7d7d 3c2f 6c61 6265   v.name }}</labe
+000001c0: 6c3e 3c2f 6474 3e0a 2020 2020 2020 2020  l></dt>.        
+000001d0: 2020 2020 2020 2020 2020 2020 3c64 643e              <dd>
+000001e0: 7b25 2069 6e63 6c75 6465 2027 7661 6c75  {% include 'valu
+000001f0: 6573 6574 2f76 616c 7565 2e68 746d 6c27  eset/value.html'
+00000200: 2025 7d3c 2f64 643e 0a20 2020 2020 2020   %}</dd>.       
+00000210: 2020 2020 2020 2020 207b 2520 656e 6466           {% endf
+00000220: 6f72 2025 7d0a 2020 2020 2020 2020 2020  or %}.          
+00000230: 2020 3c2f 646c 3e0a 2020 2020 2020 2020    </dl>.        
+00000240: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00000250: 666c 6f61 742d 656e 6422 3e0a 2020 2020  float-end">.    
+00000260: 2020 2020 2020 2020 2020 2020 7b25 2069              {% i
+00000270: 6e63 6c75 6465 2022 6461 7368 626f 6172  nclude "dashboar
+00000280: 642f 6163 7469 6f6e 732e 6874 6d6c 2220  d/actions.html" 
+00000290: 7769 7468 2075 7569 643d 6461 7461 2e75  with uuid=data.u
+000002a0: 7569 6420 7461 7267 6574 3d22 696e 7374  uid target="inst
+000002b0: 616e 6365 2220 6163 7469 6f6e 733d 6461  ance" actions=da
+000002c0: 7461 2e61 6374 696f 6e73 2e69 6e73 7461  ta.actions.insta
+000002d0: 6e63 6520 6964 3d72 6f77 2e69 647c 7374  nce id=row.id|st
+000002e0: 7269 6e67 666f 726d 6174 3a27 7327 2065  ringformat:'s' e
+000002f0: 6e61 626c 6564 3d72 6f77 2e61 6374 696f  nabled=row.actio
+00000300: 6e73 2020 257d 0a20 2020 2020 2020 2020  ns  %}.         
+00000310: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00000320: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00000330: 3d22 636c 6561 7266 6978 223e 3c2f 6469  ="clearfix"></di
+00000340: 763e 0a20 2020 2020 2020 2020 2020 203c  v>.            <
+00000350: 6872 3e0a 2020 2020 2020 2020 7b25 2065  hr>.        {% e
+00000360: 6e64 666f 7220 257d 0a20 2020 207b 2520  ndfor %}.    {% 
+00000370: 656c 7365 2025 7d0a 2020 2020 3c74 6162  else %}.    <tab
+00000380: 6c65 2063 6c61 7373 3d22 7461 626c 6522  le class="table"
+00000390: 3e0a 2020 2020 2020 2020 3c74 6865 6164  >.        <thead
+000003a0: 3e0a 2020 2020 2020 2020 3c74 723e 0a20  >.        <tr>. 
+000003b0: 2020 2020 2020 2020 2020 207b 2520 6966             {% if
+000003c0: 2064 6174 612e 6163 7469 6f6e 732e 7175   data.actions.qu
+000003d0: 6572 7973 6574 2025 7d0a 2020 2020 2020  eryset %}.      
+000003e0: 2020 2020 2020 3c74 6820 7363 6f70 653d        <th scope=
+000003f0: 2263 6f6c 2220 7769 6474 683d 2231 3070  "col" width="10p
+00000400: 7822 3e0a 2020 2020 2020 2020 2020 2020  x">.            
+00000410: 2020 2020 7b25 2069 6e63 6c75 6465 2022      {% include "
+00000420: 7175 6572 7973 6574 2f63 6865 636b 626f  queryset/checkbo
+00000430: 782e 6874 6d6c 2220 257d 0a20 2020 2020  x.html" %}.     
+00000440: 2020 2020 2020 203c 2f74 683e 0a20 2020         </th>.   
+00000450: 2020 2020 2020 2020 207b 2520 656e 6469           {% endi
+00000460: 6620 257d 0a20 2020 2020 2020 2020 2020  f %}.           
+00000470: 207b 2520 666f 7220 6c61 6265 6c2c 2064   {% for label, d
+00000480: 6973 706c 6179 2069 6e20 6461 7461 2e6d  isplay in data.m
+00000490: 6574 6164 6174 612e 6469 7370 6c61 792e  etadata.display.
+000004a0: 6974 656d 7320 257d 0a20 2020 2020 2020  items %}.       
+000004b0: 2020 2020 203c 7468 2073 636f 7065 3d22       <th scope="
+000004c0: 636f 6c22 3e7b 7b20 6469 7370 6c61 792e  col">{{ display.
+000004d0: 6e61 6d65 207d 7d3c 2f74 683e 0a20 2020  name }}</th>.   
+000004e0: 2020 2020 2020 2020 207b 2520 656e 6466           {% endf
+000004f0: 6f72 2025 7d0a 2020 2020 2020 2020 2020  or %}.          
+00000500: 2020 7b25 2069 6620 6461 7461 2e61 6374    {% if data.act
+00000510: 696f 6e73 2e69 6e73 7461 6e63 6520 616e  ions.instance an
+00000520: 6420 6e6f 7420 7072 696e 7420 257d 0a20  d not print %}. 
+00000530: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000540: 7468 2073 7479 6c65 3d22 7465 7874 2d61  th style="text-a
+00000550: 6c69 676e 3a63 656e 7465 7222 2073 636f  lign:center" sco
+00000560: 7065 3d22 636f 6c22 3e3c 2f74 683e 0a20  pe="col"></th>. 
+00000570: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
+00000580: 6469 6620 257d 0a20 2020 2020 2020 203c  dif %}.        <
+00000590: 2f74 723e 0a20 2020 2020 2020 203c 2f74  /tr>.        </t
+000005a0: 6865 6164 3e0a 2020 2020 2020 2020 3c74  head>.        <t
+000005b0: 626f 6479 3e0a 2020 2020 2020 2020 7b25  body>.        {%
+000005c0: 2066 6f72 2072 6f77 2069 6e20 6461 7461   for row in data
+000005d0: 2e64 6174 6120 257d 0a20 2020 2020 2020  .data %}.       
+000005e0: 203c 7472 3e0a 2020 2020 2020 2020 2020   <tr>.          
+000005f0: 2020 7b25 2069 6620 6461 7461 2e61 6374    {% if data.act
+00000600: 696f 6e73 2e71 7565 7279 7365 7420 257d  ions.queryset %}
+00000610: 0a20 2020 2020 2020 2020 2020 203c 7468  .            <th
+00000620: 2073 636f 7065 3d22 636f 6c22 2063 6c61   scope="col" cla
+00000630: 7373 3d22 616c 6967 6e2d 6d69 6464 6c65  ss="align-middle
+00000640: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00000650: 2020 207b 2520 696e 636c 7564 6520 2271     {% include "q
+00000660: 7565 7279 7365 742f 6368 6563 6b62 6f78  ueryset/checkbox
+00000670: 2e68 746d 6c22 2025 7d0a 2020 2020 2020  .html" %}.      
+00000680: 2020 2020 2020 3c2f 7468 3e0a 2020 2020        </th>.    
+00000690: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
+000006a0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000006b0: 7b25 2066 6f72 2076 2069 6e20 726f 772e  {% for v in row.
+000006c0: 6461 7461 2e76 616c 7565 7320 257d 0a20  data.values %}. 
+000006d0: 2020 2020 2020 2020 2020 203c 7464 2063             <td c
+000006e0: 6c61 7373 3d22 616c 6967 6e2d 6d69 6464  lass="align-midd
+000006f0: 6c65 223e 0a20 2020 2020 2020 2020 2020  le">.           
+00000700: 2020 2020 207b 2520 696e 636c 7564 6520       {% include 
+00000710: 2776 616c 7565 7365 742f 7661 6c75 652e  'valueset/value.
+00000720: 6874 6d6c 2720 257d 0a20 2020 2020 2020  html' %}.       
+00000730: 2020 2020 203c 2f74 643e 0a20 2020 2020       </td>.     
+00000740: 2020 2020 2020 207b 2520 656e 6466 6f72         {% endfor
+00000750: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+00000760: 7b25 2069 6620 6461 7461 2e61 6374 696f  {% if data.actio
+00000770: 6e73 2e69 6e73 7461 6e63 6520 616e 6420  ns.instance and 
+00000780: 6e6f 7420 7072 696e 7420 257d 0a20 2020  not print %}.   
+00000790: 2020 2020 2020 2020 203c 7464 2061 6c69           <td ali
+000007a0: 676e 3d22 6365 6e74 6572 2220 636c 6173  gn="center" clas
+000007b0: 733d 2261 6c69 676e 2d6d 6964 646c 6520  s="align-middle 
+000007c0: 696e 7374 616e 6365 2d61 6374 696f 6e73  instance-actions
+000007d0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+000007e0: 2020 207b 2520 696e 636c 7564 6520 2271     {% include "q
+000007f0: 7565 7279 7365 742f 6163 7469 6f6e 732f  ueryset/actions/
+00000800: 6163 7469 6f6e 732e 6874 6d6c 2220 257d  actions.html" %}
+00000810: 0a20 2020 2020 2020 2020 2020 203c 2f74  .            </t
+00000820: 643e 0a20 2020 2020 2020 2020 2020 207b  d>.            {
+00000830: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
+00000840: 2020 203c 2f74 723e 0a20 2020 2020 2020     </tr>.       
+00000850: 207b 2520 656e 6466 6f72 2025 7d0a 2020   {% endfor %}.  
+00000860: 2020 2020 2020 3c2f 7462 6f64 793e 0a20        </tbody>. 
+00000870: 2020 203c 2f74 6162 6c65 3e0a 2020 2020     </table>.    
+00000880: 7b25 2065 6e64 6966 2025 7d0a 7b25 2065  {% endif %}.{% e
+00000890: 6c73 6520 257d 0a20 2020 203c 6469 7620  lse %}.    <div 
+000008a0: 636c 6173 733d 2261 6c65 7274 2061 6c65  class="alert ale
+000008b0: 7274 2d70 7269 6d61 7279 2220 726f 6c65  rt-primary" role
+000008c0: 3d22 616c 6572 7422 2073 7479 6c65 3d22  ="alert" style="
+000008d0: 6d61 7267 696e 2d74 6f70 3a33 3070 783b  margin-top:30px;
+000008e0: 223e 0a20 2020 2020 204e 656e 6875 6d20  ">.      Nenhum 
+000008f0: 7265 6769 7374 726f 2065 6e63 6f6e 7472  registro encontr
+00000900: 6164 6f2e 0a20 2020 203c 2f64 6976 3e0a  ado..    </div>.
+00000910: 7b25 2065 6e64 6966 2025 7d0a            {% endif %}.
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/queryset/filter.html` & `django-sloth-0.1.0/sloth/api/templates/queryset/filter.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,174 +1,184 @@
-00000000: 3c64 6976 2063 6c61 7373 3d22 6669 6c74  <div class="filt
-00000010: 6572 207b 2520 6966 206d 6574 6164 6174  er {% if metadat
-00000020: 612e 6869 6464 656e 2025 7d64 2d6e 6f6e  a.hidden %}d-non
-00000030: 657b 2520 656e 6469 6620 257d 223e 0a20  e{% endif %}">. 
-00000040: 2020 203c 6c61 6265 6c3e 7b7b 206e 616d     <label>{{ nam
-00000050: 657c 7472 756e 6361 7465 6368 6172 733a  e|truncatechars:
-00000060: 3235 207d 7d3c 2f6c 6162 656c 3e0a 2020  25 }}</label>.  
-00000070: 2020 7b25 2069 6620 6d65 7461 6461 7461    {% if metadata
-00000080: 2e74 7970 6520 3d3d 2022 6368 6f69 6365  .type == "choice
-00000090: 7322 2025 7d0a 2020 2020 3c73 656c 6563  s" %}.    <selec
-000000a0: 7420 6e61 6d65 3d22 7b7b 206d 6574 6164  t name="{{ metad
-000000b0: 6174 612e 6b65 7920 7d7d 2220 636c 6173  ata.key }}" clas
-000000c0: 733d 227b 7b20 6d65 7461 6461 7461 2e6b  s="{{ metadata.k
-000000d0: 6579 207d 7d2d 7b7b 2064 6174 612e 7575  ey }}-{{ data.uu
-000000e0: 6964 207d 7d22 3e0a 2020 2020 2020 2020  id }}">.        
-000000f0: 7b25 2069 6620 6d65 7461 6461 7461 2e63  {% if metadata.c
-00000100: 686f 6963 6573 2025 7d0a 2020 2020 2020  hoices %}.      
-00000110: 2020 2020 2020 3c6f 7074 696f 6e20 7661        <option va
-00000120: 6c75 653d 2222 3e3c 2f6f 7074 696f 6e3e  lue=""></option>
-00000130: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
-00000140: 666f 7220 6368 6f69 6365 2069 6e20 6d65  for choice in me
-00000150: 7461 6461 7461 2e63 686f 6963 6573 2025  tadata.choices %
-00000160: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00000170: 2020 3c6f 7074 696f 6e20 7661 6c75 653d    <option value=
-00000180: 227b 7b20 6368 6f69 6365 2e69 647c 7374  "{{ choice.id|st
-00000190: 7269 6e67 666f 726d 6174 3a27 7327 207d  ringformat:'s' }
-000001a0: 7d22 3e7b 7b20 6368 6f69 6365 2e74 6578  }">{{ choice.tex
-000001b0: 7420 7d7d 3c2f 6f70 7469 6f6e 3e0a 2020  t }}</option>.  
-000001c0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-000001d0: 666f 7220 257d 0a20 2020 2020 2020 207b  for %}.        {
-000001e0: 2520 656c 7365 2025 7d0a 2020 2020 2020  % else %}.      
-000001f0: 2020 2020 2020 7b25 2069 6620 6d65 7461        {% if meta
-00000200: 6461 7461 2e76 616c 7565 2025 7d0a 2020  data.value %}.  
-00000210: 2020 2020 2020 2020 2020 2020 2020 3c6f                <o
-00000220: 7074 696f 6e20 7365 6c65 6374 6564 2076  ption selected v
-00000230: 616c 7565 3d22 7b7b 2076 616c 7565 207d  alue="{{ value }
-00000240: 7d22 3e7b 7b20 6d65 7461 6461 7461 2e76  }">{{ metadata.v
-00000250: 616c 7565 207d 7d3c 2f6f 7074 696f 6e3e  alue }}</option>
-00000260: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
-00000270: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
-00000280: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
-00000290: 203c 2f73 656c 6563 743e 0a20 2020 203c   </select>.    <
-000002a0: 7363 7269 7074 3e0a 2020 2020 2020 2024  script>.       $
-000002b0: 2827 2e7b 7b20 6d65 7461 6461 7461 2e6b  ('.{{ metadata.k
-000002c0: 6579 207d 7d2d 7b7b 2064 6174 612e 7575  ey }}-{{ data.uu
-000002d0: 6964 207d 7d27 292e 7365 6c65 6374 3228  id }}').select2(
-000002e0: 7b0a 2020 2020 2020 2020 7769 6474 683a  {.        width:
-000002f0: 2027 7265 736f 6c76 6527 2c0a 2020 2020   'resolve',.    
-00000300: 2020 2020 2020 6c61 6e67 7561 6765 3a20        language: 
-00000310: 2770 742d 4252 272c 0a20 2020 2020 2020  'pt-BR',.       
-00000320: 2020 2061 6c6c 6f77 436c 6561 723a 2074     allowClear: t
-00000330: 7275 652c 0a20 2020 2020 2020 2020 2070  rue,.          p
-00000340: 6c61 6365 686f 6c64 6572 3a20 2753 656c  laceholder: 'Sel
-00000350: 6563 696f 6e65 2075 6d61 206f 70c3 a7c3  ecione uma op...
-00000360: a36f 272c 0a20 2020 2020 2020 2020 207b  .o',.          {
-00000370: 2520 6966 206d 6574 6164 6174 612e 6368  % if metadata.ch
-00000380: 6f69 6365 7320 6973 204e 6f6e 6520 257d  oices is None %}
-00000390: 0a20 2020 2020 2020 2020 2061 6a61 783a  .          ajax:
-000003a0: 207b 0a20 2020 2020 2020 2020 2020 2075   {.            u
-000003b0: 726c 3a20 222f 6170 707b 7b20 6461 7461  rl: "/app{{ data
-000003c0: 2e70 6174 6820 7d7d 3f63 686f 6963 6573  .path }}?choices
-000003d0: 3d7b 7b20 6d65 7461 6461 7461 2e6b 6579  ={{ metadata.key
-000003e0: 207d 7d22 2c0a 2020 2020 2020 2020 2020   }}",.          
-000003f0: 2020 6461 7461 5479 7065 3a20 276a 736f    dataType: 'jso
-00000400: 6e27 2c0a 2020 2020 2020 2020 2020 2020  n',.            
-00000410: 6465 6c61 793a 2032 3530 2c0a 2020 2020  delay: 250,.    
-00000420: 2020 2020 2020 2020 6d69 6e69 6d75 6d49          minimumI
-00000430: 6e70 7574 4c65 6e67 7468 3a20 332c 0a20  nputLength: 3,. 
-00000440: 2020 2020 2020 2020 2020 2064 6174 613a             data:
-00000450: 2066 756e 6374 696f 6e20 2870 6172 616d   function (param
-00000460: 7329 207b 0a20 2020 2020 2020 2020 2020  s) {.           
-00000470: 2020 2072 6574 7572 6e20 7b20 7465 726d     return { term
-00000480: 3a20 7061 7261 6d73 2e74 6572 6d20 7d3b  : params.term };
-00000490: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
-000004a0: 2020 2020 2020 2020 2020 2020 7072 6f63              proc
-000004b0: 6573 7352 6573 756c 7473 3a20 6675 6e63  essResults: func
-000004c0: 7469 6f6e 2028 6461 7461 2920 7b0a 2020  tion (data) {.  
-000004d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000004e0: 726e 207b 2072 6573 756c 7473 3a20 6461  rn { results: da
-000004f0: 7461 2e69 7465 6d73 207d 3b0a 2020 2020  ta.items };.    
-00000500: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00000510: 2020 2020 2020 2074 656d 706c 6174 6552         templateR
-00000520: 6573 756c 743a 2066 756e 6374 696f 6e20  esult: function 
-00000530: 2864 6174 6129 207b 0a20 2020 2020 2020  (data) {.       
-00000540: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000550: 6461 7461 2e68 746d 6c20 7c7c 2027 4275  data.html || 'Bu
-00000560: 7363 616e 646f 2e2e 2e27 3b0a 2020 2020  scando...';.    
-00000570: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00000580: 2020 2020 2020 2074 656d 706c 6174 6553         templateS
-00000590: 656c 6563 7469 6f6e 3a20 6675 6e63 7469  election: functi
-000005a0: 6f6e 2028 6461 7461 2920 7b0a 2020 2020  on (data) {.    
-000005b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000005c0: 726e 2064 6174 612e 7465 7874 3b0a 2020  rn data.text;.  
-000005d0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-000005e0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-000005f0: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
-00000600: 2020 2020 207d 293b 0a20 2020 203c 2f73       });.    </s
-00000610: 6372 6970 743e 0a20 2020 207b 2520 656e  cript>.    {% en
-00000620: 6469 6620 257d 0a20 2020 207b 2520 6966  dif %}.    {% if
-00000630: 206d 6574 6164 6174 612e 7479 7065 203d   metadata.type =
-00000640: 3d20 2262 6f6f 6c65 616e 2220 257d 0a20  = "boolean" %}. 
-00000650: 2020 203c 7365 6c65 6374 206e 616d 653d     <select name=
-00000660: 227b 7b20 6d65 7461 6461 7461 2e6b 6579  "{{ metadata.key
-00000670: 207d 7d22 2063 6c61 7373 3d22 7b7b 206d   }}" class="{{ m
-00000680: 6574 6164 6174 612e 6b65 7920 7d7d 2d7b  etadata.key }}-{
-00000690: 7b20 6461 7461 2e75 7569 6420 7d7d 223e  { data.uuid }}">
-000006a0: 0a20 2020 2020 2020 203c 6f70 7469 6f6e  .        <option
-000006b0: 3e3c 2f6f 7074 696f 6e3e 0a20 2020 2020  ></option>.     
-000006c0: 2020 203c 6f70 7469 6f6e 207b 2520 6966     <option {% if
-000006d0: 206d 6574 6164 6174 612e 7661 6c75 6520   metadata.value 
-000006e0: 3d3d 2054 7275 6520 257d 7365 6c65 6374  == True %}select
-000006f0: 6564 7b25 2065 6e64 6966 2025 7d20 7661  ed{% endif %} va
-00000700: 6c75 653d 2231 223e 5369 6d3c 2f6f 7074  lue="1">Sim</opt
-00000710: 696f 6e3e 0a20 2020 2020 2020 203c 6f70  ion>.        <op
-00000720: 7469 6f6e 207b 2520 6966 206d 6574 6164  tion {% if metad
-00000730: 6174 612e 7661 6c75 6520 3d3d 2046 616c  ata.value == Fal
-00000740: 7365 2025 7d73 656c 6563 7465 647b 2520  se %}selected{% 
-00000750: 656e 6469 6620 257d 2076 616c 7565 3d22  endif %} value="
-00000760: 3022 3e4e c3a3 6f3c 2f6f 7074 696f 6e3e  0">N..o</option>
-00000770: 0a20 2020 203c 2f73 656c 6563 743e 0a20  .    </select>. 
-00000780: 2020 203c 7363 7269 7074 3e0a 2020 2020     <script>.    
-00000790: 2020 2020 2020 2024 2827 2e7b 7b20 6d65         $('.{{ me
-000007a0: 7461 6461 7461 2e6b 6579 207d 7d2d 7b7b  tadata.key }}-{{
-000007b0: 2064 6174 612e 7575 6964 207d 7d27 292e   data.uuid }}').
-000007c0: 7365 6c65 6374 3228 7b0a 2020 2020 2020  select2({.      
-000007d0: 2020 2020 2020 6c61 6e67 7561 6765 3a20        language: 
-000007e0: 2770 742d 4252 272c 0a20 2020 2020 2020  'pt-BR',.       
-000007f0: 2020 2020 2061 6c6c 6f77 436c 6561 723a       allowClear:
-00000800: 2074 7275 652c 0a20 2020 2020 2020 2020   true,.         
-00000810: 2020 2070 6c61 6365 686f 6c64 6572 3a20     placeholder: 
-00000820: 2753 656c 6563 696f 6e65 2075 6d61 206f  'Selecione uma o
-00000830: 70c3 a7c3 a36f 272c 0a20 2020 2020 2020  p....o',.       
-00000840: 2020 2020 7d29 3b0a 2020 2020 3c2f 7363      });.    </sc
-00000850: 7269 7074 3e0a 2020 2020 7b25 2065 6e64  ript>.    {% end
-00000860: 6966 2025 7d0a 2020 2020 7b25 2069 6620  if %}.    {% if 
-00000870: 6d65 7461 6461 7461 2e74 7970 6520 3d3d  metadata.type ==
-00000880: 2022 6461 7465 2220 6f72 206d 6574 6164   "date" or metad
-00000890: 6174 612e 7479 7065 203d 3d20 2264 6174  ata.type == "dat
-000008a0: 6574 696d 6522 2025 7d0a 2020 2020 3c69  etime" %}.    <i
-000008b0: 6e70 7574 2074 7970 653d 2274 6578 7422  nput type="text"
-000008c0: 206e 616d 653d 227b 7b20 6d65 7461 6461   name="{{ metada
-000008d0: 7461 2e6b 6579 207d 7d22 2063 6c61 7373  ta.key }}" class
-000008e0: 3d22 666f 726d 2d63 6f6e 7472 6f6c 207b  ="form-control {
-000008f0: 7b20 6d65 7461 6461 7461 2e6b 6579 207d  { metadata.key }
-00000900: 7d2d 7b7b 2064 6174 612e 7575 6964 207d  }-{{ data.uuid }
-00000910: 7d22 0a20 2020 2020 2020 2020 2020 706c  }".           pl
-00000920: 6163 6568 6f6c 6465 723d 2249 6e66 6f72  aceholder="Infor
-00000930: 6d65 2075 6d20 6461 7461 2220 7374 796c  me um data" styl
-00000940: 653d 2270 6164 6469 6e67 2d6c 6566 743a  e="padding-left:
-00000950: 3130 7078 223e 0a20 2020 203c 7363 7269  10px">.    <scri
-00000960: 7074 3e0a 2020 2020 2020 2020 2020 2020  pt>.            
-00000970: 2428 6675 6e63 7469 6f6e 2829 207b 0a20  $(function() {. 
-00000980: 2020 2020 2020 2020 2020 2020 2020 2024                 $
-00000990: 2827 2e7b 7b20 6d65 7461 6461 7461 2e6b  ('.{{ metadata.k
-000009a0: 6579 207d 7d2d 7b7b 2064 6174 612e 7575  ey }}-{{ data.uu
-000009b0: 6964 207d 7d27 292e 6461 7465 7069 636b  id }}').datepick
-000009c0: 6572 2824 2e64 6174 6570 6963 6b65 722e  er($.datepicker.
-000009d0: 7265 6769 6f6e 616c 5b27 7074 2d42 5227  regional['pt-BR'
-000009e0: 5d29 3b0a 2020 2020 2020 2020 2020 2020  ]);.            
-000009f0: 2020 2020 2428 272e 7b7b 206d 6574 6164      $('.{{ metad
-00000a00: 6174 612e 6b65 7920 7d7d 2d7b 7b20 6461  ata.key }}-{{ da
-00000a10: 7461 2e75 7569 6420 7d7d 2729 2e64 6174  ta.uuid }}').dat
-00000a20: 6570 6963 6b65 7228 2022 6f70 7469 6f6e  epicker( "option
-00000a30: 222c 2022 6461 7465 466f 726d 6174 222c  ", "dateFormat",
-00000a40: 2027 6464 2f6d 6d2f 7979 2729 3b0a 2020   'dd/mm/yy');.  
-00000a50: 2020 2020 2020 2020 2020 2020 2020 2428                $(
-00000a60: 272e 7b7b 206d 6574 6164 6174 612e 6b65  '.{{ metadata.ke
-00000a70: 7920 7d7d 2d7b 7b20 6461 7461 2e75 7569  y }}-{{ data.uui
-00000a80: 6420 7d7d 2729 2e64 6174 6570 6963 6b65  d }}').datepicke
-00000a90: 7228 2022 6f70 7469 6f6e 222c 2022 7769  r( "option", "wi
-00000aa0: 6474 6822 2c20 2727 293b 0a20 2020 2020  dth", '');.     
-00000ab0: 2020 2020 2020 207d 293b 0a20 2020 203c         });.    <
-00000ac0: 2f73 6372 6970 743e 0a20 2020 207b 2520  /script>.    {% 
-00000ad0: 656e 6469 6620 257d 0a3c 2f64 6976 3e    endif %}.</div>
+00000000: 7b25 206c 6f61 6420 7461 6773 2025 7d0a  {% load tags %}.
+00000010: 3c64 6976 2063 6c61 7373 3d22 6669 6c74  <div class="filt
+00000020: 6572 207b 2520 6966 206d 6574 6164 6174  er {% if metadat
+00000030: 612e 6869 6464 656e 2025 7d64 2d6e 6f6e  a.hidden %}d-non
+00000040: 657b 2520 656e 6469 6620 257d 223e 0a20  e{% endif %}">. 
+00000050: 2020 203c 6c61 6265 6c3e 7b7b 206d 6574     <label>{{ met
+00000060: 6164 6174 612e 6e61 6d65 7c74 7275 6e63  adata.name|trunc
+00000070: 6174 6563 6861 7273 3a32 3520 7d7d 3c2f  atechars:25 }}</
+00000080: 6c61 6265 6c3e 0a20 2020 207b 2520 6966  label>.    {% if
+00000090: 206d 6574 6164 6174 612e 7479 7065 203d   metadata.type =
+000000a0: 3d20 2263 686f 6963 6573 2220 257d 0a20  = "choices" %}. 
+000000b0: 2020 203c 7365 6c65 6374 206e 616d 653d     <select name=
+000000c0: 227b 7b20 6d65 7461 6461 7461 2e6b 6579  "{{ metadata.key
+000000d0: 207d 7d22 2063 6c61 7373 3d22 7b7b 206d   }}" class="{{ m
+000000e0: 6574 6164 6174 612e 6b65 7920 7d7d 2d7b  etadata.key }}-{
+000000f0: 7b20 6461 7461 2e75 7569 6420 7d7d 223e  { data.uuid }}">
+00000100: 0a20 2020 2020 2020 207b 2520 6966 206d  .        {% if m
+00000110: 6574 6164 6174 612e 6368 6f69 6365 7320  etadata.choices 
+00000120: 257d 0a20 2020 2020 2020 2020 2020 203c  %}.            <
+00000130: 6f70 7469 6f6e 2076 616c 7565 3d22 223e  option value="">
+00000140: 3c2f 6f70 7469 6f6e 3e0a 2020 2020 2020  </option>.      
+00000150: 2020 2020 2020 7b25 2066 6f72 2063 686f        {% for cho
+00000160: 6963 6520 696e 206d 6574 6164 6174 612e  ice in metadata.
+00000170: 6368 6f69 6365 7320 257d 0a20 2020 2020  choices %}.     
+00000180: 2020 2020 2020 2020 2020 203c 6f70 7469             <opti
+00000190: 6f6e 207b 2520 6966 206d 6574 6164 6174  on {% if metadat
+000001a0: 612e 7661 6c75 652e 3120 3d3d 2063 686f  a.value.1 == cho
+000001b0: 6963 652e 6964 2025 7d73 656c 6563 7465  ice.id %}selecte
+000001c0: 647b 2520 656e 6469 6620 257d 2076 616c  d{% endif %} val
+000001d0: 7565 3d22 7b7b 2063 686f 6963 652e 6964  ue="{{ choice.id
+000001e0: 7c73 7472 696e 6766 6f72 6d61 743a 2773  |stringformat:'s
+000001f0: 2720 7d7d 223e 7b7b 2063 686f 6963 652e  ' }}">{{ choice.
+00000200: 7465 7874 207d 7d3c 2f6f 7074 696f 6e3e  text }}</option>
+00000210: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
+00000220: 656e 6466 6f72 2025 7d0a 2020 2020 2020  endfor %}.      
+00000230: 2020 7b25 2065 6c73 6520 257d 0a20 2020    {% else %}.   
+00000240: 2020 2020 2020 2020 207b 2520 6966 206d           {% if m
+00000250: 6574 6164 6174 612e 7661 6c75 6520 257d  etadata.value %}
+00000260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000270: 203c 6f70 7469 6f6e 2073 656c 6563 7465   <option selecte
+00000280: 6420 7661 6c75 653d 227b 7b20 6d65 7461  d value="{{ meta
+00000290: 6461 7461 2e76 616c 7565 2e31 207d 7d22  data.value.1 }}"
+000002a0: 3e7b 7b20 6d65 7461 6461 7461 2e76 616c  >{{ metadata.val
+000002b0: 7565 2e30 207d 7d3c 2f6f 7074 696f 6e3e  ue.0 }}</option>
+000002c0: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
+000002d0: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
+000002e0: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
+000002f0: 203c 2f73 656c 6563 743e 0a20 2020 203c   </select>.    <
+00000300: 696e 7075 7420 7479 7065 3d22 6869 6464  input type="hidd
+00000310: 656e 2220 6964 3d22 7b7b 206d 6574 6164  en" id="{{ metad
+00000320: 6174 612e 6b65 7920 7d7d 3022 206e 616d  ata.key }}0" nam
+00000330: 653d 227b 7b20 6d65 7461 6461 7461 2e6b  e="{{ metadata.k
+00000340: 6579 207d 7d30 2220 7661 6c75 653d 227b  ey }}0" value="{
+00000350: 7b20 6d65 7461 6461 7461 2e76 616c 7565  { metadata.value
+00000360: 2e30 207d 7d22 3e3c 2f69 6e70 7574 3e0a  .0 }}"></input>.
+00000370: 2020 2020 3c73 6372 6970 743e 0a20 2020      <script>.   
+00000380: 2020 2020 2428 272e 7b7b 206d 6574 6164      $('.{{ metad
+00000390: 6174 612e 6b65 7920 7d7d 2d7b 7b20 6461  ata.key }}-{{ da
+000003a0: 7461 2e75 7569 6420 7d7d 2729 2e73 656c  ta.uuid }}').sel
+000003b0: 6563 7432 287b 0a20 2020 2020 2020 2077  ect2({.        w
+000003c0: 6964 7468 3a20 2772 6573 6f6c 7665 272c  idth: 'resolve',
+000003d0: 0a20 2020 2020 2020 2020 206c 616e 6775  .          langu
+000003e0: 6167 653a 2027 7074 2d42 5227 2c0a 2020  age: 'pt-BR',.  
+000003f0: 2020 2020 2020 2020 616c 6c6f 7743 6c65          allowCle
+00000400: 6172 3a20 7472 7565 2c0a 2020 2020 2020  ar: true,.      
+00000410: 2020 2020 706c 6163 6568 6f6c 6465 723a      placeholder:
+00000420: 2027 5365 6c65 6369 6f6e 6520 756d 6120   'Selecione uma 
+00000430: 6f70 c3a7 c3a3 6f27 2c0a 2020 2020 2020  op....o',.      
+00000440: 2020 2020 7b25 2069 6620 6d65 7461 6461      {% if metada
+00000450: 7461 2e63 686f 6963 6573 2069 7320 4e6f  ta.choices is No
+00000460: 6e65 2025 7d0a 2020 2020 2020 2020 2020  ne %}.          
+00000470: 616a 6178 3a20 7b0a 2020 2020 2020 2020  ajax: {.        
+00000480: 2020 2020 7572 6c3a 2066 756e 6374 696f      url: functio
+00000490: 6e20 2829 207b 7265 7475 726e 2022 7b7b  n () {return "{{
+000004a0: 2064 6174 612e 7061 7468 7c73 7461 7274   data.path|start
+000004b0: 5f71 7565 7279 7374 7269 6e67 207d 7d22  _querystring }}"
+000004c0: 2b24 2827 2366 6f72 6d2d 7b7b 2064 6174  +$('#form-{{ dat
+000004d0: 612e 7575 6964 207d 7d27 292e 7365 7269  a.uuid }}').seri
+000004e0: 616c 697a 6528 292b 2726 6368 6f69 6365  alize()+'&choice
+000004f0: 733d 7b7b 206d 6574 6164 6174 612e 6b65  s={{ metadata.ke
+00000500: 7920 7d7d 273b 7d2c 0a20 2020 2020 2020  y }}';},.       
+00000510: 2020 2020 2064 6174 6154 7970 653a 2027       dataType: '
+00000520: 6a73 6f6e 272c 0a20 2020 2020 2020 2020  json',.         
+00000530: 2020 2064 656c 6179 3a20 3235 302c 0a20     delay: 250,. 
+00000540: 2020 2020 2020 2020 2020 206d 696e 696d             minim
+00000550: 756d 496e 7075 744c 656e 6774 683a 2033  umInputLength: 3
+00000560: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
+00000570: 7461 3a20 6675 6e63 7469 6f6e 2028 7061  ta: function (pa
+00000580: 7261 6d73 2920 7b0a 2020 2020 2020 2020  rams) {.        
+00000590: 2020 2020 2020 7265 7475 726e 207b 2074        return { t
+000005a0: 6572 6d3a 2070 6172 616d 732e 7465 726d  erm: params.term
+000005b0: 207d 3b0a 2020 2020 2020 2020 2020 2020   };.            
+000005c0: 7d2c 0a20 2020 2020 2020 2020 2020 2070  },.            p
+000005d0: 726f 6365 7373 5265 7375 6c74 733a 2066  rocessResults: f
+000005e0: 756e 6374 696f 6e20 2864 6174 6129 207b  unction (data) {
+000005f0: 0a20 2020 2020 2020 2020 2020 2020 2072  .              r
+00000600: 6574 7572 6e20 7b20 7265 7375 6c74 733a  eturn { results:
+00000610: 2064 6174 612e 6974 656d 7320 7d3b 0a20   data.items };. 
+00000620: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00000630: 2020 2020 2020 2020 2020 7465 6d70 6c61            templa
+00000640: 7465 5265 7375 6c74 3a20 6675 6e63 7469  teResult: functi
+00000650: 6f6e 2028 6461 7461 2920 7b0a 2020 2020  on (data) {.    
+00000660: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00000670: 726e 2064 6174 612e 6874 6d6c 207c 7c20  rn data.html || 
+00000680: 2742 7573 6361 6e64 6f2e 2e2e 273b 0a20  'Buscando...';. 
+00000690: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+000006a0: 2020 2020 2020 2020 2020 7465 6d70 6c61            templa
+000006b0: 7465 5365 6c65 6374 696f 6e3a 2066 756e  teSelection: fun
+000006c0: 6374 696f 6e20 2864 6174 6129 207b 0a20  ction (data) {. 
+000006d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000006e0: 6574 7572 6e20 6461 7461 2e74 6578 743b  eturn data.text;
+000006f0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00000700: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00000710: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
+00000720: 0a20 2020 2020 2020 7d29 3b0a 2020 2020  .       });.    
+00000730: 2020 2024 2827 2e7b 7b20 6d65 7461 6461     $('.{{ metada
+00000740: 7461 2e6b 6579 207d 7d2d 7b7b 2064 6174  ta.key }}-{{ dat
+00000750: 612e 7575 6964 207d 7d27 292e 6f6e 2822  a.uuid }}').on("
+00000760: 7365 6c65 6374 323a 7365 6c65 6374 222c  select2:select",
+00000770: 2066 756e 6374 696f 6e28 6529 207b 0a20   function(e) {. 
+00000780: 2020 2020 2020 2024 2827 237b 7b20 6d65         $('#{{ me
+00000790: 7461 6461 7461 2e6b 6579 207d 7d30 2729  tadata.key }}0')
+000007a0: 2e76 616c 2824 2874 6869 7329 2e66 696e  .val($(this).fin
+000007b0: 6428 276f 7074 696f 6e3a 7365 6c65 6374  d('option:select
+000007c0: 6564 2729 2e74 6578 7428 292e 7472 696d  ed').text().trim
+000007d0: 2829 293b 0a20 2020 207d 293b 0a20 2020  ());.    });.   
+000007e0: 203c 2f73 6372 6970 743e 0a20 2020 207b   </script>.    {
+000007f0: 2520 656e 6469 6620 257d 0a20 2020 207b  % endif %}.    {
+00000800: 2520 6966 206d 6574 6164 6174 612e 7479  % if metadata.ty
+00000810: 7065 203d 3d20 2262 6f6f 6c65 616e 2220  pe == "boolean" 
+00000820: 257d 0a20 2020 203c 7365 6c65 6374 206e  %}.    <select n
+00000830: 616d 653d 227b 7b20 6d65 7461 6461 7461  ame="{{ metadata
+00000840: 2e6b 6579 207d 7d22 2063 6c61 7373 3d22  .key }}" class="
+00000850: 7b7b 206d 6574 6164 6174 612e 6b65 7920  {{ metadata.key 
+00000860: 7d7d 2d7b 7b20 6461 7461 2e75 7569 6420  }}-{{ data.uuid 
+00000870: 7d7d 223e 0a20 2020 2020 2020 203c 6f70  }}">.        <op
+00000880: 7469 6f6e 2073 656c 6563 7465 643e 3c2f  tion selected></
+00000890: 6f70 7469 6f6e 3e0a 2020 2020 2020 2020  option>.        
+000008a0: 3c6f 7074 696f 6e20 7b25 2069 6620 6d65  <option {% if me
+000008b0: 7461 6461 7461 2e76 616c 7565 203d 3d20  tadata.value == 
+000008c0: 5472 7565 2025 7d73 656c 6563 7465 647b  True %}selected{
+000008d0: 2520 656e 6469 6620 257d 2076 616c 7565  % endif %} value
+000008e0: 3d22 3122 3e53 696d 3c2f 6f70 7469 6f6e  ="1">Sim</option
+000008f0: 3e0a 2020 2020 2020 2020 3c6f 7074 696f  >.        <optio
+00000900: 6e20 7b25 2069 6620 6d65 7461 6461 7461  n {% if metadata
+00000910: 2e76 616c 7565 203d 3d20 4661 6c73 6520  .value == False 
+00000920: 257d 7365 6c65 6374 6564 7b25 2065 6e64  %}selected{% end
+00000930: 6966 2025 7d20 7661 6c75 653d 2230 223e  if %} value="0">
+00000940: 4ec3 a36f 3c2f 6f70 7469 6f6e 3e0a 2020  N..o</option>.  
+00000950: 2020 3c2f 7365 6c65 6374 3e0a 2020 2020    </select>.    
+00000960: 3c73 6372 6970 743e 0a20 2020 2020 2020  <script>.       
+00000970: 2020 2020 2428 272e 7b7b 206d 6574 6164      $('.{{ metad
+00000980: 6174 612e 6b65 7920 7d7d 2d7b 7b20 6461  ata.key }}-{{ da
+00000990: 7461 2e75 7569 6420 7d7d 2729 2e73 656c  ta.uuid }}').sel
+000009a0: 6563 7432 287b 0a20 2020 2020 2020 2020  ect2({.         
+000009b0: 2020 206c 616e 6775 6167 653a 2027 7074     language: 'pt
+000009c0: 2d42 5227 2c0a 2020 2020 2020 2020 2020  -BR',.          
+000009d0: 2020 616c 6c6f 7743 6c65 6172 3a20 7472    allowClear: tr
+000009e0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+000009f0: 706c 6163 6568 6f6c 6465 723a 2027 5365  placeholder: 'Se
+00000a00: 6c65 6369 6f6e 6520 756d 6120 6f70 c3a7  lecione uma op..
+00000a10: c3a3 6f27 2c0a 2020 2020 2020 2020 2020  ..o',.          
+00000a20: 207d 293b 0a20 2020 203c 2f73 6372 6970   });.    </scrip
+00000a30: 743e 0a20 2020 207b 2520 656e 6469 6620  t>.    {% endif 
+00000a40: 257d 0a20 2020 207b 2520 6966 206d 6574  %}.    {% if met
+00000a50: 6164 6174 612e 7479 7065 203d 3d20 2264  adata.type == "d
+00000a60: 6174 6522 206f 7220 6d65 7461 6461 7461  ate" or metadata
+00000a70: 2e74 7970 6520 3d3d 2022 6461 7465 7469  .type == "dateti
+00000a80: 6d65 2220 257d 0a20 2020 203c 696e 7075  me" %}.    <inpu
+00000a90: 7420 7479 7065 3d22 6461 7465 2220 6e61  t type="date" na
+00000aa0: 6d65 3d22 7b7b 206d 6574 6164 6174 612e  me="{{ metadata.
+00000ab0: 6b65 7920 7d7d 2220 7661 6c75 653d 227b  key }}" value="{
+00000ac0: 7b20 6d65 7461 6461 7461 2e76 616c 7565  { metadata.value
+00000ad0: 7c64 6566 6175 6c74 3a27 2720 7d7d 2220  |default:'' }}" 
+00000ae0: 636c 6173 733d 2266 6f72 6d2d 636f 6e74  class="form-cont
+00000af0: 726f 6c20 7b7b 206d 6574 6164 6174 612e  rol {{ metadata.
+00000b00: 6b65 7920 7d7d 2d7b 7b20 6461 7461 2e75  key }}-{{ data.u
+00000b10: 7569 6420 7d7d 220a 2020 2020 2020 2020  uid }}".        
+00000b20: 2020 2070 6c61 6365 686f 6c64 6572 3d22     placeholder="
+00000b30: 496e 666f 726d 6520 756d 2064 6174 6122  Informe um data"
+00000b40: 2073 7479 6c65 3d22 7061 6464 696e 672d   style="padding-
+00000b50: 6c65 6674 3a31 3070 7822 3e0a 2020 2020  left:10px">.    
+00000b60: 7b25 2065 6e64 6966 2025 7d0a 3c2f 6469  {% endif %}.</di
+00000b70: 763e                                     v>
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/queryset/filters.html` & `django-sloth-0.1.0/sloth/api/templates/queryset/filters.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,45 @@
 {% load tags %}
 <style>
-{% if not data.metadata.is_admin  %}
-    .search-and-filters .filters{
-        display: none;
-    }
-{% endif %}
-{% if compact or request.GET.compact or request|mobile %}
-    .search-and-filters .filter {
-        width: 100% !important;
-    }
-{% else %}
-    .search-and-filters .filter {
-        width: 250px !important;
-    }
+{% if data.metadata.collapsed  %}
+    #search-and-filters-{{ data.uuid }}.search-and-filters form{display: none}
 {% endif %}
 </style>
-{% if data.metadata.pagination.total %}
-    {% if data.metadata.search or data.metadata.filters %}
-        <div class="search-and-filters">
-            <form method="get" id="form-{{ data.uuid }}" action="/app{{ data.path }}">
+
+        <div class="search-and-filters" id="search-and-filters-{{ data.uuid }}">
+            <form method="get" id="form-{{ data.uuid }}" action="{{ data.path }}" style="{% if data.metadata.collapsed %}display:none{% endif %}">
                 <input type="hidden" name="uuid" value="{{ data.uuid }}">
                 <input type="hidden" name="is_admin" value="{% if data.metadata.is_admin %}1{% endif %}">
+                <input type="hidden" name="collapsed" value="{% if data.metadata.collapsed %}1{% endif %}" id="collapsed-{{ data.uuid }}">
                 <input type="hidden" name="page" value="{{ data.page }}" id="pagination-{{ data.uuid }}">
                 <input type="hidden" name="compact" value="{% if compact or request.GET.compact or request|mobile %}1{%endif%}">
-                <input type="hidden" name="subset" value="all" id="subset-{{ data.uuid }}">
+                <input type="hidden" name="subset" value="{{ data.metadata.subset }}" id="subset-{{ data.uuid }}">
                 <input type="hidden" name="selected-date" value="" id="selected-date-{{ data.uuid }}">
-
+                <!--{% for k, v in request.POST.items %}
+                    {% if k != 'csrfmiddlewaretoken' %}
+                        <input type="hidden" name="post__{{ k }}" value="{{ v }}">
+                    {% endif %}
+                {% endfor %}-->
                 {% if data.metadata.search or data.metadata.filters %}
                     <div class="filters" id="filters-{{ data.uuid }}">
                         {% if data.metadata.search %}
                             <div class="filter">
                                 <label>Busca</label>
-                                <input type="text" class="form-control" pattern=".{3,}" name="q" value="{{ request.GET.q|default:'' }}" id="searchbar" title="3 ou mais caracteres" onkeypress="if(event.which==13){reload{{ data.uuid }}(false);return false;}" placeholder="">
+                                <input type="text" class="form-control" pattern=".{3,}" name="q" value="{{ request.GET.q|default:'' }}" id="searchbar" title="3 ou mais caracteres" onkeypress="if(event.which==13){reload{{ data.uuid }}();return false;}" placeholder="">
                             </div>
                         {% endif %}
-                        {% for name, metadata in data.metadata.filters.items %}
-                            {% include "app/queryset/filter.html" %}
+                        {% for metadata in data.metadata.filters.values %}
+                            {% include "queryset/filter.html" %}
                         {% endfor %}
                         <div class="filter">
-                            <button type="button" class="btn btn-primary filter-button" onclick="$(this).find('.spinner-border').removeClass('d-none');$(this).find('i').addClass('d-none');$('#pagination-{{ data.uuid }}').val(1);reload{{ data.uuid }}(false)">
+                            <button type="button" class="btn btn-primary filter-button" onclick="$(this).find('.spinner-border').removeClass('d-none');$(this).find('i').addClass('d-none');$('#pagination-{{ data.uuid }}').val(1);reload{{ data.uuid }}()">
                                 <div class="spinner-border spinner-border-sm d-none" role="status">
                                   <span class="visually-hidden">Loading...</span>
                                 </div>
                                 <i class="bi bi-funnel"></i>
                                 Filtrar
                             </button>
                         </div>
                     </div>
                 {% endif %}
             </form>
         </div>
-    {% endif %}
-{% endif %}
```

#### html2text {}

```diff
@@ -1,12 +1,9 @@
 {% load tags %}
- {% if data.metadata.pagination.total %} {% if data.metadata.search or
-data.metadata.filters %}
-      {% if data.metadata.search or data.metadata.filters %}
+        {% if data.metadata.search or data.metadata.filters %}
 {% if data.metadata.search %}
 Busca [{{ request.GET.q|default:'' }}]
-{% endif %} {% for name, metadata in data.metadata.filters.items %} {% include
-"app/queryset/filter.html" %} {% endfor %}
+{% endif %} {% for metadata in data.metadata.filters.values %} {% include
+"queryset/filter.html" %} {% endfor %}
 Loading...
  Filtrar
 {% endif %}
-{% endif %} {% endif %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/queryset/queryset.html` & `django-sloth-0.1.0/sloth/api/templates/queryset/queryset.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,188 +1,170 @@
 {% load tags %}
-
-{% if not data.metadata.is_admin  %}
-<div class="card">
-        <div class="card-body">
-{% endif %}
-<div class="queryset" id="queryset-{{ data.uuid }}">
-    {% if data.name %}
-    {% if data.metadata.collapsed or compact %}
-        <div class="queryset-title" style="cursor:pointer" onclick="$(this).parent().find('.toogle-data').slideToggle();$(this).find('i').toggleClass('bi-chevron-down').toggleClass('bi-chevron-right');">
-            <h2><i class="bi bi-chevron-down"></i> {{ data.name }}</h2>
+<div>
+<div class="reloadable-queryset {% if not data.metadata.is_admin%}box{% endif %}" id="{{ data.key }}" data-path="{{ data.path }}">
+    <div class="queryset {% if data.metadata.is_admin %}admin-queryset{% endif %}" id="queryset-{{ data.uuid }}">
+        {% if data.name %}
+            {% if data.metadata.is_admin %}
+                <div class="queryset-title">
+                    <h2>{{ data.icon|icontag }} {{ data.name }}</h2>
+                </div>
+            {% else %}
+                <div class="queryset-title" style="cursor:pointer" onclick="$(this).parent().find('.toogle-data').slideToggle();$(this).find('i').toggleClass('bi-chevron-down').toggleClass('bi-chevron-right');">
+                    <h5><i class="bi bi-chevron-down"></i> {{ data.name }}</h5>
+                </div>
+            {% endif %}
+        {% endif %}
+        {% if not print %}
+        <div id="queryset-global-actions-{{ data.uuid }}" class="queryset-action-bar">
+            {% include "queryset/actions/global.html" %}
         </div>
-    {% else %}
-        <div class="queryset-title">
-            <h2>{{ data.icon|icontag }} {{ data.name }}</h2>
+        {% endif %}
+        <div class="clearfix"></div>
+        <div class="queryset-container toogle-data" id="queryset-container{{ data.uuid }}">
+        {% if data.attach and not print %}
+        <div class="clearfix"></div>
+        <div class="tabs-container mb-2" id="tabs-container-{{ data.uuid }}">
+            <ul class="nav nav-pills nav-fill">
+                {% for subset in data.attach.values %}
+              <li class="nav-item {{ subset.key }} {% if subset.active %}selected{% endif %}">
+                <a class="nav-link" aria-current="page" href="javascript:" onclick="$('#pagination-{{ data.uuid }}').val(1);reload{{ data.uuid }}('{{ subset.key }}')">
+                    <div class="spinner-border spinner-border-sm d-none" role="status">
+                      <span class="visually-hidden">Loading...</span>
+                    </div>
+                    <span class="nav-link-text">{{ subset.name }}</span>
+                    <span class="badge rounded-pill text-white bg-primary total-{{ subset.key }}">{{ subset.count }}</span>
+                </a>
+              </li>
+                {% endfor %}
+            </ul>
         </div>
-    {% endif %}
-    {% endif %}
-    <div id="queryset-global-actions-{{ data.uuid }}" class="queryset-action-bar">
-        {% include "app/queryset/actions/global.html" %}
-    </div>
-    <div class="clearfix"></div>
-    <div class="queryset-container toogle-data" id="queryset-container{{ data.uuid }}">
-    {% if data.attach %}
-    <div class="clearfix"></div>
-    <div class="tabs-container mb-2" id="tabs-container-{{ data.uuid }}">
-        <ul class="nav nav-pills nav-fill">
-            {% for subset in data.attach.values %}
-          <li class="nav-item {{ subset.key }} {% if subset.active %}selected{% endif %}">
-            <a class="nav-link" aria-current="page" href="javascript:" onclick="$('#pagination-{{ data.uuid }}').val(1);reload{{ data.uuid }}(false, '{{ subset.key }}')">
-                <div class="spinner-border spinner-border-sm d-none" role="status">
-                  <span class="visually-hidden">Loading...</span>
-                </div>
-                <span class="nav-link-text">{{ subset.name }}</span>
-                <span class="badge rounded-pill text-white bg-primary total-{{ subset.key }}">{{ subset.count }}</span>
-            </a>
-          </li>
-            {% endfor %}
-        </ul>
-    </div>
-    {% endif %}
+        {% endif %}
 
-    {% include "app/queryset/filters.html" %}
-    <div class="clearfix"></div>
-
-    <script>
-        function reload{{ data.uuid }}(attaches, subset){
-            $(document.body).addClass('page-loading');
-            if(attaches==null) attaches = true;
-            if(subset==null) subset = $('#subset-{{ data.uuid }}').val();
-            else $('#subset-{{ data.uuid }}').val(subset);
-            $('#tabs-container-{{ data.uuid }}').find('.nav-item.'+subset).find('.spinner-border').removeClass('d-none');
-            $('#tabs-container-{{ data.uuid }}').find('.nav-item').removeClass('selected')
-            $('#tabs-container-{{ data.uuid }}').find('.nav-item.'+subset).addClass('selected')
-            var data = $('#form-{{ data.uuid }}').serialize();
-            $.ajax({
-                url:'/app{{ data.path }}',
-                data:data,
-                success:function( html ) {
-                    var remote = $(html);
-                    $('#queryset-data-{{ data.uuid }}').html(
-                        remote.find('#queryset-data-{{ data.uuid }},.valueset-fieldsets,.fieldset-data').html()
-                    ).initialize();
-                    $('#queryset-global-actions-{{ data.uuid }}').html(
-                        remote.find('#queryset-global-actions-{{ data.uuid }}').html()
-                    ).initialize();
-                    $(document.body).removeClass('page-loading');
-                    $('#queryset-{{ data.uuid }}').find('.spinner-border').addClass('d-none');
-                    $('#queryset-{{ data.uuid }}').find('i').removeClass('d-none');
-                    $('#tabs-container-{{ data.uuid }}').find('.nav-item.'+subset).find('.spinner-border').addClass('d-none');
-                }
-            });
-            {% if data.attach %}
-            if(attaches){
-                $.ajax({
-                    dataType: 'json',
-                    url: '/app{{ data.path }}?attaches=',
-                    success:function( totals ) {
-                        for (const [key, value] of Object.entries(totals)) {
-                            if(value.count!=null) $('#tabs-container-{{ data.uuid }}').find('.total-'+key).html(value.count);
+        {% for action in data.actions.inline %}
+            {% action action.key data.instantiator action.path %}
+        {% endfor %}
+
+        {% if not print %}
+            {% include "queryset/filters.html" %}
+            <div class="clearfix"></div>
+            <script>
+                function reload{{ data.uuid }}(subset){
+                    $(document.body).addClass('page-loading');
+                    if(subset==null) subset = $('#subset-{{ data.uuid }}').val();
+                    $('#subset-{{ data.uuid }}').val(subset);
+                    $('#tabs-container-{{ data.uuid }}').find('.nav-item.'+subset).find('.spinner-border').removeClass('d-none');
+                    var data = $('#form-{{ data.uuid }}').serialize();
+                    $.ajax({
+                        url:'{{ data.path|safe }}?{{ request|post_querystring }}',
+                        data: data,
+                        success:function( html ) {
+                            $('#{{ data.key }}').html($(html).find('#{{ data.key }}').html()).initialize();
+                            $(document.body).removeClass('page-loading');
                         }
+                    });
+                }
+                function toggleActions{{ data.uuid }}(input){
+                    if(input.value=='on') $('#queryset-{{ data.uuid }}').find('.action-checkbox').prop('checked', input.checked);
+                    if($('#queryset-{{ data.uuid }}').find('.action-checkbox:checked').length>0){
+                        $('#queryset-{{ data.uuid }}').find('.dropdown-toggle.queryset').removeClass('disabled');
+                        $('#queryset-{{ data.uuid }}').find('.dropdown-toggle.instance, .dropdown-toggle.model').addClass('disabled');
+                        $('#queryset-{{ data.uuid }}').find('.btn.instance, .btn.model').addClass('disabled');
+                        $('#queryset-{{ data.uuid }}').find('.btn.queryset').removeClass('disabled');
+                    } else {
+                        $('#queryset-{{ data.uuid }}').find('.dropdown-toggle.queryset').addClass('disabled');
+                        $('#queryset-{{ data.uuid }}').find('.dropdown-toggle.model, .dropdown-toggle.instance').removeClass('disabled');
+                        $('#queryset-{{ data.uuid }}').find('.btn.instance, .btn.model').removeClass('disabled');
+                        $('#queryset-{{ data.uuid }}').find('.btn.queryset').addClass('disabled');
                     }
-                });
-            }
-            {% endif %}
-        }
-        function toggleActions{{ data.uuid }}(input){
-            if(input.value=='on') $('#queryset-{{ data.uuid }}').find('.action-checkbox').prop('checked', input.checked);
-            if($('#queryset-{{ data.uuid }}').find('.action-checkbox:checked').length>0){
-                $('#queryset-{{ data.uuid }}').find('.dropdown-toggle.queryset').removeClass('disabled');
-                $('#queryset-{{ data.uuid }}').find('.dropdown-toggle.instance, .dropdown-toggle.model').addClass('disabled');
-                $('#queryset-{{ data.uuid }}').find('.btn.instance, .btn.model').addClass('disabled');
-                $('#queryset-{{ data.uuid }}').find('.btn.queryset').removeClass('disabled');
-            } else {
-                $('#queryset-{{ data.uuid }}').find('.dropdown-toggle.queryset').addClass('disabled');
-                $('#queryset-{{ data.uuid }}').find('.dropdown-toggle.model, .dropdown-toggle.instance').removeClass('disabled');
-                $('#queryset-{{ data.uuid }}').find('.btn.instance, .btn.model').removeClass('disabled');
-                $('#queryset-{{ data.uuid }}').find('.btn.queryset').addClass('disabled');
-            }
-        }
-        function slideSearchAndFilters{{ data.uuid }}(a){
-            if(a) $(a).find('i:last-child').toggleClass('bi-chevron-up').toggleClass('bi-chevron-down');
-            if($('#filters-{{ data.uuid }}').css('display') == 'none'){
-                $('#filters-{{ data.uuid }}').slideDown();
-            } else {
-                $('#filters-{{ data.uuid }}').slideUp();
-            }
-        }
-    </script>
-
-    <div class="queryset-data" id="queryset-data-{{ data.uuid }}">
-
-{% if data.metadata.pagination.total or data.metadata.calendar %}
-<div class="clearfix" id="pagination-info-{{ data.uuid }}">
-    <div class="float-start">
-        <div class="mt-3 mb-3" style="font-size: 80%">
-            Exibindo {{ data.metadata.pagination.interval }} de
-            <strong>
-                {{ data.metadata.pagination.total }} registro{% if data.metadata.pagination.total > 1 %}s{% endif %}
-            </strong>
+                }
+                function slideSearchAndFilters{{ data.uuid }}(a){
+                    if(a) $(a).find('i:last-child').toggleClass('bi-chevron-up').toggleClass('bi-chevron-down');
+                    if($('#form-{{ data.uuid }}').css('display') == 'none'){
+                        $('#form-{{ data.uuid }}').slideDown();
+                        $('#collapsed-{{ data.uuid }}').val("");
+                    } else {
+                        $('#form-{{ data.uuid }}').slideUp();
+                        $('#collapsed-{{ data.uuid }}').val(1);
+                    }
+                }
+            </script>
+        {% endif %}
+
+        <div class="queryset-data" id="queryset-data-{{ data.uuid }}">
+
+    {% if data.metadata.pagination.total or data.metadata.calendar %}
+    <div class="clearfix" id="pagination-info-{{ data.uuid }}">
+        <div class="float-start">
+            <div class="mt-3 mb-3" style="font-size: 80%">
+                Exibindo
+                {% if data.metadata.pagination.total > data.metadata.pagination.interval.1 %}
+                    {{ data.metadata.pagination.interval.0 }} - {{ data.metadata.pagination.interval.1 }} de
+                {% endif %}
+                <strong>
+                    {{ data.metadata.pagination.total }} registro{% if data.metadata.pagination.total > 1 %}s{% endif %}
+                </strong>
+            </div>
         </div>
-    </div>
-    <div class="float-end">
-        <div class="mt-3 mb-3">
-            <!--<a href="/app{{ data.path }}?export=csv"><i class="bi bi-download"></i></a>-->
-            <!--<a href="/app{{ data.path }}?export=xls"><i class="bi bi-file-excel"></i></a>-->
-            <!--<a href="/app{{ data.path }}?export=pdf"><i class="bi bi-file-earmark-pdf"></i></a>-->
-            {% if data.metadata.search or data.metadata.filters %}
-            <a href="javascript:"><i class="bi bi-funnel" onclick="slideSearchAndFilters{{ data.uuid }}()"></i></a>
-            {% endif %}
-            <a href="javascript:"><i class="bi bi-arrow-clockwise" onclick="reload{{ data.uuid }}(false);"></i></a>
+        <div class="float-end">
+            <div class="mt-3 mb-3">
+                <!--<a href="{{ data.path }}?export=csv"><i class="bi bi-download"></i></a>-->
+                <!--<a href="{{ data.path }}?export=xls"><i class="bi bi-file-excel"></i></a>-->
+                <!--<a href="{{ data.path }}?export=pdf"><i class="bi bi-file-earmark-pdf"></i></a>-->
+                {% if data.metadata.search or data.metadata.filters %}
+                <a href="javascript:"><i class="bi bi-funnel" onclick="slideSearchAndFilters{{ data.uuid }}()"></i></a>
+                {% endif %}
+                <a href="javascript:"><i class="bi bi-arrow-clockwise" onclick="reload{{ data.uuid }}();"></i></a>
+            </div>
         </div>
     </div>
-</div>
-
-{% if data.metadata.calendar %}
-    {% include "app/queryset/calendar.html" with data=data %}
-{% endif %}
 
-{% if data.metadata.total is not None %}
-<div class="float-end">
-    <h3>Total: {{ data.metadata.total|format }}</h3>
-</div>
-<div class="clear-fix">&nbsp;</div>
-{% endif %}
+    {% if data.metadata.calendar %}
+        {% include "queryset/calendar.html" with data=data %}
+    {% endif %}
 
-{% endif %}
+    {% if data.metadata.aggregations %}
+        {% for aggregation in data.metadata.aggregations.values %}
+            <h3 style="float:right; margin-left: 20">{{ aggregation.name }}: {{ aggregation.value|format }}</h3>
+        {% endfor %}
+        <div class="clear-fix">&nbsp;</div>
+    {% endif %}
 
-{% if data.template %}
-    {% include data.template with data=data %}
-{% else %}
-    {% include "app/queryset/datatable.html" with data=data %}
-{% endif %}
-{% include "app/queryset/actions/batch.html" %}
-{% if data.metadata.pagination.pages|length > 1 %}
+    {% endif %}
 
-    <nav aria-label="Page navigation example">
-  <ul class="pagination" style="overflow-x:hidden">
-    {% for page in data.metadata.pagination.pages %}
-       {% if forloop.counter|add:3 == data.metadata.pagination.pages|length and not forloop.counter == 5 %}
-        <li class="page-item disabled">
-          <a class="page-link" href="#" tabindex="-1" aria-disabled="true">...</a>
-        </li>
-       {% endif %}
-        <li class="page-item {% if page == data.metadata.pagination.page %}active{% endif %}">
-            <a class="page-link" href="javascript:" onclick="$('#pagination-{{ data.uuid }}').val({{ page|stringformat:'s' }});reload{{ data.uuid }}(false);document.getElementById('pagination-info-{{ data.uuid }}').scrollIntoView();">
-                {{ page }}
-            </a>
-        </li>
-      {% if forloop.counter == 4 %}
-        <li class="page-item disabled">
-          <a class="page-link" href="#" tabindex="-1" aria-disabled="true">...</a>
-        </li>
-      {% endif %}
-    {% endfor %}
-  </ul>
-</nav>
-{% endif %}
+    {% if data.template %}
+        {% include data.template with data=data %}
+    {% else %}
+        {% include "queryset/datatable.html" with data=data %}
+    {% endif %}
+    {% include "queryset/actions/batch.html" %}
+    {% if data.metadata.pagination.pages|length > 1 and data.metadata.scrollable %}
 
-    </div>
+        <nav aria-label="Paginação">
+      <ul class="pagination" style="overflow-x:hidden">
+        {% for page in data.metadata.pagination.pages %}
+           {% if forloop.counter|add:3 == data.metadata.pagination.pages|length and not forloop.counter == 5 %}
+            <li class="page-item disabled">
+              <a class="page-link" href="#" tabindex="-1" aria-disabled="true">...</a>
+            </li>
+           {% endif %}
+            <li class="page-item {% if page == data.metadata.pagination.page %}active{% endif %}">
+                <a class="page-link" href="javascript:" onclick="$('#pagination-{{ data.uuid }}').val({{ page|stringformat:'s' }});reload{{ data.uuid }}();document.getElementById('pagination-info-{{ data.uuid }}').scrollIntoView();">
+                    {{ page }}
+                </a>
+            </li>
+          {% if forloop.counter == 4 %}
+            <li class="page-item disabled">
+              <a class="page-link" href="#" tabindex="-1" aria-disabled="true">...</a>
+            </li>
+          {% endif %}
+        {% endfor %}
+      </ul>
+    </nav>
+    {% endif %}
+        </div>
+        </div>
     </div>
 </div>
-{% if not data.metadata.is_admin  %}
-            </div>
-    </div>
+{% if data.metadata.scrollable %}
+    {% include "queryset/scroll.html" %}
 {% endif %}
-
-
+</div>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,39 +1,46 @@
-{% load tags %} {% if not data.metadata.is_admin %}
-{% endif %}
-{% if data.name %} {% if data.metadata.collapsed or compact %}
- {{ data.name }}
-{% else %}
+{% load tags %}
+{% if data.name %} {% if data.metadata.is_admin %}
 ***** {{ data.icon|icontag }} {{ data.name }} *****
-{% endif %} {% endif %}
-{% include "app/queryset/actions/global.html" %}
-{% if data.attach %}
+{% else %}
+ {{ data.name }}
+{% endif %} {% endif %} {% if not print %}
+{% include "queryset/actions/global.html" %}
+{% endif %}
+{% if data.attach and not print %}
     * {% for subset in data.attach.values %}
     * Loading...
       {{_subset.name_}}_{{_subset.count_}}
     * {% endfor %}
-{% endif %} {% include "app/queryset/filters.html" %}
+{% endif %} {% for action in data.actions.inline %} {% action action.key
+data.instantiator action.path %} {% endfor %} {% if not print %} {% include
+"queryset/filters.html" %}
+ {% endif %}
 {% if data.metadata.pagination.total or data.metadata.calendar %}
-Exibindo {{ data.metadata.pagination.interval }} de {
+Exibindo {% if data.metadata.pagination.total >
+data.metadata.pagination.interval.1 %} {{ data.metadata.pagination.interval.0
+}} - {{ data.metadata.pagination.interval.1 }} de {% endif %} {
 { data.metadata.pagination.total }} registro{% if
 data.metadata.pagination.total > 1 %}s{% endif %}
    {% if data.metadata.search or data.metadata.filters %}  {% endif %}
-{% if data.metadata.calendar %} {% include "app/queryset/calendar.html" with
-data=data %} {% endif %} {% if data.metadata.total is not None %}
-**** Total: {{ data.metadata.total|format }} ****
+{% if data.metadata.calendar %} {% include "queryset/calendar.html" with
+data=data %} {% endif %} {% if data.metadata.aggregations %} {% for aggregation
+in data.metadata.aggregations.values %}
+**** {{ aggregation.name }}: {{ aggregation.value|format }} ****
+{% endfor %}
  
 {% endif %} {% endif %} {% if data.template %} {% include data.template with
-data=data %} {% else %} {% include "app/queryset/datatable.html" with data=data
-%} {% endif %} {% include "app/queryset/actions/batch.html" %} {% if
-data.metadata.pagination.pages|length > 1 %}
+data=data %} {% else %} {% include "queryset/datatable.html" with data=data %}
+{% endif %} {% include "queryset/actions/batch.html" %} {% if
+data.metadata.pagination.pages|length > 1 and data.metadata.scrollable %}
     * {% for page in data.metadata.pagination.pages %} {% if
       forloop.counter|add:3 == data.metadata.pagination.pages|length and not
       forloop.counter == 5 %}
     * ...
     * {% endif %}
     * {{_page_}}
     * {% if forloop.counter == 4 %}
     * ...
     * {% endif %} {% endfor %}
  {% endif %}
-{% if not data.metadata.is_admin %}
-{% endif %}
+{% if data.metadata.scrollable %} {% include "queryset/scroll.html" %} {% endif
+%}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/queryset/rows.html` & `django-sloth-0.1.0/sloth/api/templates/queryset/rows.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% load tags %}
 {% if compact or data.metadata.compact or request.GET.compact or request|mobile %}
-    {% include "app/queryset/cards.html" with compact=True %}
+    {% include "queryset/cards.html" with compact=True %}
 {% else %}
 {% if data.data %}
 <div id="row-{{ data.uuid }}">
     {% with image_key=data.data.0.data|image_key %}
         {% for row in data.data %}
         <div>
             <div class="card" style="margin-bottom: 10px">
@@ -18,26 +18,26 @@
                                     {% endif %}
                                 {% endfor %}
                             {% endif %}
                         </div>
                         <div style="{% if image_key %}margin-left:220px;{% endif %}">
                             <h5 class="card-title text-left">{{ row.description }}</h5>
                             <div class="float-end">
-                                {% include "app/queryset/checkbox.html" %}
+                                {% include "queryset/checkbox.html" %}
                             </div>
                             <dl>
                                 {% for k, v in row.data.items %}
                                     {% if k != image_key %}
-                                        <dt>{{ k }}</dt>
-                                        <dd>{% include 'app/valueset/value.html' %}</dd>
+                                        <dt>{{ v.name }}</dt>
+                                        <dd>{% include 'valueset/value.html' %}</dd>
                                     {% endif %}
                                 {% endfor %}
                             </dl>
                             <div class="float-end">
-                                {% include "app/actions.html" with uuid=data.uuid target="instance" actions=data.actions.instance id=row.id|stringformat:'s' enabled=row.actions %}
+                                {% include "dashboard/actions.html" with uuid=data.uuid target="instance" actions=data.actions.instance id=row.id|stringformat:'s' enabled=row.actions %}
                             </div>
                         </div>
                     </div>
                 </div>
             </div>
         </div>
         {% endfor %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/queryset/timeline.html` & `django-sloth-0.1.0/sloth/api/templates/queryset/timeline.html`

 * *Files 2% similar despite different names*

```diff
@@ -154,24 +154,24 @@
         <div class="timeline-badge"><i class="glyphicon glyphicon-check"></i></div>
         <div class="timeline-panel">
             <div class="timeline-heading">
                 <h5 class="timeline-title">{{ row.description }}</h5>
             </div>
             <div class="timeline-body">
                 <div class="float-end">
-                    {% include "app/queryset/checkbox.html" %}
+                    {% include "queryset/checkbox.html" %}
                 </div>
                 <dl>
-                {% for k, v in row.data.items %}
-                    <dt>{{ k }}</dt>
-                    <dd>{% include 'app/valueset/value.html' %}</dd>
+                {% for v in row.data.values %}
+                    <dt>{{ v.name }}</dt>
+                    <dd>{% include 'valueset/value.html' %}</dd>
                 {% endfor %}
                 </dl>
                 <div class="float-end">
-                    {% include "app/actions.html" with uuid=data.uuid target="instance" actions=data.actions.instance id=row.id|stringformat:'s' enabled=row.actions  %}
+                    {% include "dashboard/actions.html" with uuid=data.uuid target="instance" actions=data.actions.instance id=row.id|stringformat:'s' enabled=row.actions  %}
                 </div>
                 <div class="clearfix"></div>
             </div>
         </div>
     </li>
     {% endfor %}
 </ul>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% load tags %} {% if data.data %}
     * {% for row in data.data %}
     * ** {{ row.description }} **
-      {% include "app/queryset/checkbox.html" %}
-      {% for k, v in row.data.items %}
-      {% include "app/actions.html" with uuid=data.uuid target="instance"
+      {% include "queryset/checkbox.html" %}
+      {% for v in row.data.values %}
+      {% include "dashboard/actions.html" with uuid=data.uuid target="instance"
       actions=data.actions.instance id=row.id|stringformat:'s'
       enabled=row.actions %}
     * {% endfor %}
 {% else %}
 Nenhum registro encontrado.
 {% endif %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/report.html` & `django-sloth-0.1.0/sloth/api/templates/dashboard/report.html`

 * *Files 11% similar despite different names*

```diff
@@ -5,17 +5,22 @@
     <meta charset="utf-8">
     <meta name="robots" content="NONE,NOARCHIVE">
     <meta name="pdfkit-page-size" content="Legal"/>
     <meta name="pdfkit-orientation" content="Portrait"/>
     <style>
 
         body {
-            font-size: 8pt;
-            line-height: 1.4em;
             font-family: 'Open Sans', sans-serif;
+            line-height: 1.4em;
+        }
+        h1, h2, h3, h4, h5, .header .title{
+            font-weight: bolder;
+        }
+        th, label, .fieldset-field-label{
+            font-weight: bold;
         }
         dd {
             border-bottom: 1px dashed #ccc;
             font-size: 9pt;
             font-weight: bold;
             margin-right: 5px;
             padding: 3px 0 10px;
@@ -28,37 +33,32 @@
         dt::after {
             content: ":";
         }
         h1 {
             font-size: 16pt;
             margin-bottom: 0;
             text-align: center;
-            padding: 5px;
+            text-transform: uppercase;
         }
         h2 {
             font-size: 14pt;
             text-align: center;
             text-transform: uppercase;
             vertical-align: bottom;
-            padding: 5px;
         }
-        h3 {
+        h3, h5 {
             font-size: 13pt;
             margin: 10px 0 0;
-            padding: 10px 0;
-        }
-        h4 {
-            font-size: 12pt;
-            font-weight: 400;
-            margin: 20px 0 0;
-            padding: 10px 0 0;
+            text-transform: uppercase;
+            padding-bottom: 5px;
         }
+
         .header .title{
             padding-top: 5px;
-            font-size: 14pt;
+            font-size: 24pt;
             font-weight: bold;
         }
         .header .subtitle{
             font-size: 11pt;
             font-weight: bold;
         }
         .header tr{
@@ -122,46 +122,65 @@
             border: 1px solid #ccc;
             line-height: 1em;
             padding: 5px;
         }
         .page-break{
             page-break-after: always;
         }
-        * {font-size: 100% !important;}
+        .responsive-container > div{
+            display: inline-block;
+            vertical-align: top;
+        }
+        .width-100{
+            width: 98.5%;
+        }
+        .width-50{
+            width: 48.9%;
+        }
+        .width-33{
+            width: 32.45%;
+        }
+        .width-25{
+            width: 24.2%;
+        }
+        .row>* {
+            width: 100%;
+            max-width: 100%;
+        }
         {% block style %}
         {% endblock %}
     </style>
 </head>
 
 <body>
 
 <header>
 {% block header %}
     <table class="header">
         <tr>
-            {% if settings.SLOTH.ICON %}
-                <td class="logo" width="200px"><img src="{{ settings.SLOTH.ICON }}"/></td>
+            {% if icon %}
+                <td class="logo" width="0"><img style="max-height:75px" src="{{ icon }}"/></td>
             {% endif %}
             <td align="center">
-                <div class="title">{{ settings.SLOTH.NAME }}</div>
+                <div class="title">{{ title }}</div>
                     <div class="subtitle">
                         {% block extra_header %}
 
                         {% endblock %}
                     </div>
                 <div>Emitido em {{ today }}</div>
             </td>
         </tr>
     </table>
 {% endblock %}
 </header>
 
 {% block content %}
 <section>
-    <h1 align="center">Relatório</h1>
+    {{ content|safe }}
 </section>
 {% endblock %}
 
 {% block footer %}
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
 
 
 
  {% block header %}
-                                   {{ settings.SLOTH.NAME }}
-[{{ settings.SLOTH.ICON }}] {% block extra_header %} {% endblock %}
-                                    Emitido em {{ today }}
-{% endblock %}  {% block content %}
-                            ****** Relatório ******
- {% endblock %} {% block footer %} {% endblock %}
+                           {{ title }}
+[{{ icon }}] {% block extra_header %} {% endblock %}
+                     Emitido em {{ today }}
+{% endblock %}  {% block content %}  {{ content|safe }}  {% endblock %} {%
+block footer %} {% endblock %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/select.html` & `django-sloth-0.1.0/sloth/api/templates/inputs/select.html`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/statistics.html` & `django-sloth-0.1.0/sloth/api/templates/queryset/statistics.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,104 +1,96 @@
 {% load tags %}
+<div class="reloadable-fieldset box" id="{{ data.key }}" data-path="{{ data.path }}">
 <div id="statistics-{{ data.uuid }}">
 {% if uuid is None or request.GET.uuid is None %}
-    <div class="card">
-        <div class="card-body">
-            {% if data.name %}
-            <div class="fieldset-title" onclick="$(this).parent().find('.toogle-data').slideToggle();$(this).find('i').toggleClass('bi-chevron-down').toggleClass('bi-chevron-right');">
-              <h5>
-                  <i class="bi bi-chevron-down"></i>
-                  {{ data.name }}
-              </h5>
-            </div>
-            {% endif %}
-            <div class="card-text fieldset-data toogle-data" id="{{ fieldset.name|slugify }}-statistics">
-{% endif %}
-{% if data.template %}
-    {% include data.template with data=data %}
-{% else %}
-{% if 0 %}
-<div class="search-and-filters">
-    <form method="get" id="form-{{ data.uuid }}" action="/app{{ data.path }}">
-        <input type="hidden" name="uuid" value="{{ data.uuid }}">
-        <div class="filters" id="filters-{{ data.uuid }}">
-            {% for name, metadata in data.filters.items %}
-                {% include "app/queryset/filter.html" %}
-            {% endfor %}
+    {% if data.name %}
+        <div class="fieldset-title" onclick="$(this).parent().find('.toogle-data').slideToggle();$(this).find('i').toggleClass('bi-chevron-down').toggleClass('bi-chevron-right');">
+          <h5><i class="bi bi-chevron-down"></i>{{ data.name }}</h5>
         </div>
-        <div class="filter">
-            <button type="button" class="btn btn-primary filter-button" onclick="$(this).find('.spinner-border').removeClass('d-none');$(this).find('i').addClass('d-none');reload{{ data.uuid }}(false)">
-                <div class="spinner-border spinner-border-sm d-none" role="status">
-                  <span class="visually-hidden">Loading...</span>
-                </div>
-                <i class="bi bi-funnel"></i>
-                Filtrar
-            </button>
-        </div>
-    </form>
-</div>
-<script>
-    function reload{{ data.uuid }}(attaches, subset){
-        $(document.body).addClass('page-loading');
-        var data = $('#form-{{ data.uuid }}').serialize();
-        $.ajax({
-            url:'/app{{ data.path }}',
-            data:data,
-            success:function( html ) {
-                $(document.body).removeClass('page-loading');
-                $('#statistics-{{ data.uuid }}').find('i').removeClass('d-none');
-                $('#statistics-{{ data.uuid }}').find('.spinner-border').addClass('d-none');
-                $('#statistics-{{ data.uuid }}').find('table').html($(html).find('table').html());
-            }
-        });
-    }
-</script>
+    {% endif %}
+    <div class="card-text fieldset-data toogle-data" id="{{ fieldset.name|slugify }}-statistics">
 {% endif %}
-<table class="table" style="overflow-x:auto">
-    {% if data.series.default %}
-        <thead>
-            <tr>
-                <td scope="col"></td>
-                <th scope="col" class="align-middle" style="text-align:center">Total</th>
-            </tr>
-        </thead>
-        {% for name, value, color in data.series.default %}
-        <tr>
-            <th scope="col">{{ name }}</th>
-            <td scope="col" class="align-middle" align="center">{{ value|format }}</td>
-        </tr>
-        {% endfor %}
-    {% else %}
         {% if data.series %}
-            {% for name, series in data.series.items %}
-                {% if forloop.first %}
-                    <thead>
-                    <tr>
-                        <td scope="col"></td>
-                        {% for name, value, color in series %}
-                            <th scope="col" class="align-middle" style="text-align:center">{{ name }}</th>
-                        {% endfor %}
-                    </tr>
-                    </thead>
+            {% if data.template %}
+                {% include data.template with data=data %}
+            {% else %}
+                {% if 0 %}
+                <div class="search-and-filters">
+                    <form method="get" id="form-{{ data.uuid }}" action="{{ data.path }}">
+                        <input type="hidden" name="uuid" value="{{ data.uuid }}">
+                        <div class="filters" id="filters-{{ data.uuid }}">
+                            {% for name, metadata in data.filters.items %}
+                                {% include "queryset/filter.html" %}
+                            {% endfor %}
+                        </div>
+                        <div class="filter">
+                            <button type="button" class="btn btn-primary filter-button" onclick="$(this).find('.spinner-border').removeClass('d-none');$(this).find('i').addClass('d-none');reload{{ data.uuid }}(false)">
+                                <div class="spinner-border spinner-border-sm d-none" role="status">
+                                  <span class="visually-hidden">Loading...</span>
+                                </div>
+                                <i class="bi bi-funnel"></i>
+                                Filtrar
+                            </button>
+                        </div>
+                    </form>
+                </div>
+                <script>
+                    function reload{{ data.uuid }}(attaches, subset){
+                        $(document.body).addClass('page-loading');
+                        var data = $('#form-{{ data.uuid }}').serialize();
+                        $.ajax({
+                            url:'{{ data.path }}',
+                            data:data,
+                            success:function( html ) {
+                                $(document.body).removeClass('page-loading');
+                                $('#statistics-{{ data.uuid }}').find('i').removeClass('d-none');
+                                $('#statistics-{{ data.uuid }}').find('.spinner-border').addClass('d-none');
+                                $('#statistics-{{ data.uuid }}').find('table').html($(html).find('table').html());
+                            }
+                        });
+                    }
+                </script>
                 {% endif %}
-                <tr>
-                    <th scope="col">{{ name }}</th>
-                    {% for name, value, color in series %}
-                        <td scope="col" class="align-middle" align="center">{{ value|format }}</td>
-                    {% endfor %}
-                </tr>
-            {% endfor %}
+                <table class="table" style="overflow-x:auto">
+                    {% if data.series.default %}
+                        <thead>
+                            <tr>
+                                <td scope="col"></td>
+                                <th scope="col" class="align-middle" style="text-align:center">Total</th>
+                            </tr>
+                        </thead>
+                        {% for name, value, color in data.series.default %}
+                        <tr>
+                            <th scope="col">{{ name }}</th>
+                            <td scope="col" class="align-middle" align="center">{{ value|format }}</td>
+                        </tr>
+                        {% endfor %}
+                    {% else %}
+                            {% for name, series in data.series.items %}
+                                {% if forloop.first %}
+                                    <thead>
+                                    <tr>
+                                        <td scope="col"></td>
+                                        {% for name, value, color in series %}
+                                            <th scope="col" class="align-middle" style="text-align:center">{{ name }}</th>
+                                        {% endfor %}
+                                    </tr>
+                                    </thead>
+                                {% endif %}
+                                <tr>
+                                    <th scope="col">{{ name }}</th>
+                                    {% for name, value, color in series %}
+                                        <td scope="col" class="align-middle" align="center">{{ value|format }}</td>
+                                    {% endfor %}
+                                </tr>
+                            {% endfor %}
+                    {% endif %}
+                </table>
+            {% endif %}
         {% else %}
-            <div class="alert alert-primary" role="alert" style="margin-top:30px;">
-              Nenhum registro encontrado.
-            </div>
+            <div class="alert alert-primary" role="alert">Nenhum registro encontrado.</div>
         {% endif %}
-    {% endif %}
-</table>
-
-{% endif %}
-{% if uuid is None or request.GET.uuid is None %}
-                </div>
-        </div>
     </div>
+{% if uuid is None or request.GET.uuid is None %}
 {% endif %}
+</div>
 </div>
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
 {% load tags %}
-{% if uuid is None or request.GET.uuid is None %}
-{% if data.name %}
- {{ data.name }}
+{% if uuid is None or request.GET.uuid is None %} {% if data.name %}
+{{ data.name }}
 {% endif %}
-{% endif %} {% if data.template %} {% include data.template with data=data %}
-{% else %} {% if 0 %}
-{% for name, metadata in data.filters.items %} {% include "app/queryset/
+{% endif %} {% if data.series %} {% if data.template %} {% include
+data.template with data=data %} {% else %} {% if 0 %}
+{% for name, metadata in data.filters.items %} {% include "queryset/
 filter.html" %} {% endfor %}
 Loading...
  Filtrar
  {% endif %}
            Total
 {{ name }} {{ value|format }}
            {{ name }}
 {{ name }} {{ value|format }}
-{% endif %} {% if uuid is None or request.GET.uuid is None %}
+{% endif %} {% else %}
+Nenhum registro encontrado.
 {% endif %}
+{% if uuid is None or request.GET.uuid is None %} {% endif %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/themes/dark.html` & `django-sloth-0.1.0/sloth/api/templates/themes/dark.html`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/valueset/fieldset-group.html` & `django-sloth-0.1.0/sloth/api/templates/valueset/fieldset-group.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,59 @@
 <div class="fieldset-group">
 <div class="fieldset-title">
     <h5>{{ item.name }}</h5>
 </div>
 <div class="fieldset-action-bar" style="margin-right:18px">
       {% if item.actions %}
-          {% include "app/actions.html" with uuid=item.uuid target="model" actions=item.actions   %}
+          {% include "dashboard/actions.html" with uuid=item.uuid target="model" actions=item.actions   %}
       {% endif %}
 </div>
 <ul class="nav nav-tabs fieldset-tabs" id="fieldset-group-{{ item.uuid }}">
-  {% for name, fieldset in item.data.items %}
+  {% for fieldset in item.data.values %}
       <li class="nav-item">
-          <a class="nav-link {{ name|slugify }} {% if forloop.first %}active{% endif %}" aria-current="page"
-             href="javascript:" onclick="reloadFieldsetGroup{{ item.uuid }}('{{ name|slugify }}', '{{ fieldset.path }}')">
+          <a class="nav-link {{ fieldset.key}} {% if forloop.first %}active{% endif %}" aria-current="page"
+             href="javascript:" onclick="reloadFieldsetGroup{{ item.uuid }}('{{ fieldset.key }}', '{{ fieldset.path }}', '{{ fieldset.type }}')">
               <div class="spinner-border spinner-border-sm d-none" role="status">
                   <span class="visually-hidden">Loading...</span>
               </div>
-              <span class="nav-link-text">{{ name }}</span>
+              <span class="nav-link-text">{{ fieldset.name }}</span>
           </a>
       </li>
   {% endfor %}
 </ul>
 <script>
-    function reloadFieldsetGroup{{ item.uuid }}(tab, path){
+    function hideTitles{{ item.uuid }}(){
+        $('#fieldset-group-{{ item.uuid }}-tab').find('.fieldset-title,.queryset-title').hide();
+    }
+    function reloadFieldsetGroup{{ item.uuid }}(tab, path, type){
         // $(document).setCookie('current_tab', tab);
         $(document.body).addClass('page-loading');
         $('#fieldset-group-{{ item.uuid }}').find('.nav-link.'+tab).find('.spinner-border').removeClass('d-none');
         $.ajax({
-            url:'/app'+path,
-            data:{},
+            url:path,
+            data:{tab:1},
             success:function( html ) {
                 $('#fieldset-group-{{ item.uuid }}-tab').html(html).initialize();
+                if(['fieldset', 'queryset', 'statistics'].indexOf(type)>-1) hideTitles{{ item.uuid }}();
                 $('#fieldset-group-{{ item.uuid }}').find('.nav-link').removeClass('active');
                 $('#fieldset-group-{{ item.uuid }}').find('.nav-link.'+tab).addClass('active');
                 $(document.body).removeClass('page-loading');
                 $('#fieldset-group-{{ item.uuid }}').find('.nav-link.'+tab).find('.spinner-border').addClass('d-none');
             }
         });
     }
  </script>
 <div class="fieldset-tab" id="fieldset-group-{{ item.uuid }}-tab">
 {% for name, item in item.data.items %}
     {% if forloop.first %}
         {% if item.type == 'fieldset-list' %}
-            {% for name, fieldset in item.data.items %}
-                {% include 'app/valueset/fieldset.html' with data=fieldset %}
+            {% for fieldset in item.data.values %}
+                {% include 'valueset/fieldset.html' with data=fieldset %}
             {% endfor %}
         {% else %}
-            {% include 'app/valueset/fieldset.html' with data=item %}
+            {% include 'valueset/fieldset.html' with data=item %}
         {% endif %}
     {% endif %}
 {% endfor %}
 </div>
+<script>hideTitles{{ item.uuid }}();</script>
 </div>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 ** {{ item.name }} **
-{% if item.actions %} {% include "app/actions.html" with uuid=item.uuid
+{% if item.actions %} {% include "dashboard/actions.html" with uuid=item.uuid
 target="model" actions=item.actions %} {% endif %}
-    * {% for name, fieldset in item.data.items %}
+    * {% for fieldset in item.data.values %}
     * Loading...
-      {{_name_}}
+      {{_fieldset.name_}}
     * {% endfor %}
 {% for name, item in item.data.items %} {% if forloop.first %} {% if item.type
-== 'fieldset-list' %} {% for name, fieldset in item.data.items %} {% include
-'app/valueset/fieldset.html' with data=fieldset %} {% endfor %} {% else %} {%
-include 'app/valueset/fieldset.html' with data=item %} {% endif %} {% endif %}
-{% endfor %}
+== 'fieldset-list' %} {% for fieldset in item.data.values %} {% include
+'valueset/fieldset.html' with data=fieldset %} {% endfor %} {% else %} {%
+include 'valueset/fieldset.html' with data=item %} {% endif %} {% endif %} {%
+endfor %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/valueset/fieldset-list.html` & `django-sloth-0.1.0/sloth/api/templates/valueset/fieldset-list.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 <div class="fieldset-list">
 <div class="fieldset-title">
     <h5>{{ item.name }}</h5>
 </div>
 <div class="fieldset-action-bar" style="margin-right:18px">
       {% if item.actions %}
-          {% include "app/actions.html" with uuid=item.uuid target="model" actions=item.actions   %}
+          {% include "dashboard/actions.html" with uuid=item.uuid target="model" actions=item.actions   %}
       {% endif %}
 </div>
+{% if item.template %}
+    {% include item.template with data=item.data %}
+{% else %}
 <ul class="nav nav-tabs fieldset-tabs" id="fieldset-list-{{ item.uuid }}">
-  {% for name, fieldset in item.data.items %}
+  {% for fieldset in item.data.values %}
       <li class="nav-item">
-          <a class="nav-link {{ name|slugify }} {% if forloop.first %}active{% endif %}" aria-current="page"
-             href="javascript:" onclick="reloadFieldsetList{{ item.uuid }}('{{ name|slugify }}', '{{ fieldset.path }}')">
+          <a class="nav-link {{ fieldset.key }} {% if forloop.first %}active{% endif %}" aria-current="page"
+             href="javascript:" onclick="reloadFieldsetList{{ item.uuid }}('{{ fieldset.key }}', '{{ fieldset.path }}', '{{ fieldset.type }}')">
               <div class="spinner-border spinner-border-sm d-none" role="status">
                   <span class="visually-hidden">Loading...</span>
               </div>
-              <span class="nav-link-text">{{ name }}</span>
+              <span class="nav-link-text">{{ fieldset.name }}</span>
           </a>
       </li>
   {% endfor %}
 </ul>
 <script>
-    function reloadFieldsetList{{ item.uuid }}(tab, path){
+    function hideTitles{{ item.uuid }}(){
+        $('#fieldset-list-{{ item.uuid }}-tab').find('.fieldset-title,.queryset-title').hide();
+    }
+    function reloadFieldsetList{{ item.uuid }}(tab, path, type){
         // $(document).setCookie('current_tab', tab);
         $(document.body).addClass('page-loading');
         $('#fieldset-list-{{ item.uuid }}').find('.nav-link.'+tab).find('.spinner-border').removeClass('d-none');
         $.ajax({
-            url:'/app'+path,
-            data:{},
+            url:path,
+            data:{tab:1},
             success:function( html ) {
                 $('#fieldset-list-{{ item.uuid }}-tab').html(html).initialize();
+                if(['fieldset', 'queryset', 'statistics'].indexOf(type)>-1) hideTitles{{ item.uuid }}();
                 $('#fieldset-list-{{ item.uuid }}').find('.nav-link').removeClass('active');
                 $('#fieldset-list-{{ item.uuid }}').find('.nav-link.'+tab).addClass('active');
                 $(document.body).removeClass('page-loading');
                 $('#fieldset-list-{{ item.uuid }}').find('.nav-link.'+tab).find('.spinner-border').addClass('d-none');
             }
         });
     }
  </script>
 <div class="fieldset-tab" id="fieldset-list-{{ item.uuid }}-tab">
-{% for name, item in item.data.items %}
-    {% if forloop.first %}
-        {% include 'app/valueset/fieldset.html' with data=item %}
-    {% endif %}
-{% endfor %}
+    {% for item in item.data.values %}
+        {% if forloop.first %}
+            {% include 'valueset/fieldset.html' with data=item %}
+        {% endif %}
+    {% endfor %}
+    <script>hideTitles{{ item.uuid }}();</script>
 </div>
+{% endif %}
 </div>
```

#### html2text {}

```diff
@@ -1,9 +1,12 @@
 ** {{ item.name }} **
-{% if item.actions %} {% include "app/actions.html" with uuid=item.uuid
+{% if item.actions %} {% include "dashboard/actions.html" with uuid=item.uuid
 target="model" actions=item.actions %} {% endif %}
-    * {% for name, fieldset in item.data.items %}
+{% if item.template %} {% include item.template with data=item.data %} {% else
+%}
+    * {% for fieldset in item.data.values %}
     * Loading...
-      {{_name_}}
+      {{_fieldset.name_}}
     * {% endfor %}
-{% for name, item in item.data.items %} {% if forloop.first %} {% include 'app/
-valueset/fieldset.html' with data=item %} {% endif %} {% endfor %}
+{% for item in item.data.values %} {% if forloop.first %} {% include 'valueset/
+fieldset.html' with data=item %} {% endif %} {% endfor %}
+{% endif %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/valueset/fieldset.html` & `django-sloth-0.1.0/sloth/api/templates/valueset/fieldset.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,76 +1,73 @@
 {% load tags %}
 {% if data.type == 'fieldset' %}
+    <div class="reloadable-fieldset box" id="{{ data.key }}" data-path="{{ data.path }}">
     {% if data.template %}
         {% include data.template with data=data %}
     {% else %}
-      <div class="card">
-        <div class="card-body">
           {% if data.name %}
           <div class="fieldset-title" onclick="$(this).parent().find('.toogle-data').slideToggle();$(this).find('i').toggleClass('bi-chevron-down').toggleClass('bi-chevron-right');">
               <h5>
-                  <i class="bi bi-chevron-down"></i>
+                  <i class="bi bi-{% if data.collapsed %}chevron-right{% else %}chevron-down{% endif %}"></i>
                   {{ data.name }}
               </h5>
           </div>
           {% endif %}
           <div class="fieldset-action-bar">
               {% if data.actions %}
-                  {% include "app/actions.html" with uuid=data.uuid target="model" actions=data.actions   %}
+                  {% include "dashboard/actions.html" with uuid=data.uuid target="model" actions=data.actions   %}
               {% endif %}
           </div>
-          <div class="card-text fieldset-data toogle-data" id="{{ data.name|slugify }}">
-              <table width="100%">
-                  <tr>
-                    {% if data.image %}
-                      <td style="width:0px;{% if request|mobile %}padding-bottom:20px;text-align:center;{% else %}padding-right:20px{% endif %}">
-                          <img width="200px" src="{{ data.image }}"/>
-                      </td>
-                    {% endif %}
-                  {% if request|mobile %}
-                  </tr><tr>
-                  {% endif %}
-                    <td>
-                      <div class="responsive-container">
-                          {% for k, v in data.data.items %}
-                                {% include 'app/valueset/field.html' with k=k v=v %}
-                          {% endfor %}
-                      </div>
-                    </td>
-                  </tr>
-              </table>
+          <div class="fieldset-data toogle-data" id="{{ data.name|slugify }}" style="{% if data.collapsed %}display:none{% endif %}">
+              {% for action in data.inline_actions %}
+                {% action action.key data.instance action.path %}
+              {% endfor %}
+
+              {% if data.image %}
+                <div style="display:flex">
+                  <div style="width:200px;margin-right:20px"><img width="200px" src="{{ data.image }}"/></div>
+                  <div style="width:calc(100% - 220px)">
+              {% endif %}
+                      <div class="responsive-container">{% for v in data.data.values %}{% include 'valueset/field.html' with v=v %}{% endfor %}</div>
+              {% if data.image %}
+                  </div>
+                </div>
+              {% endif %}
+
           </div>
-        </div>
-      </div>
+
       {% if data.refresh %}
           <script>
           {% if not request|is_ajax %}
                 var retry_{{ data.key }} = {{ data.refresh.retry }};
                 const interval_{{ data.key }} = setInterval(
-                    function(){$(document).refresh('{{ data.key }}')},
+                    function(){$(document).refresh(['{{ data.key }}'])},
                     {{ data.refresh.seconds }}000
                 );
           {% else %}
                 {% if data.refresh.retry %}
                     var retry_{{ data.key }} = retry_{{ data.key }} - 1;
                 {% else %}
                     var retry_{{ data.key }}=0;
                 {% endif %}
                 if(retry_{{ data.key }}==0) clearInterval(interval_{{ data.key }});
           {% endif %}
           </script>
       {% endif %}
     {% endif %}
+    </div>
 {% endif %}
 
 {% if data.type == 'queryset' %}
-    {% include 'app/queryset/queryset.html' with data=data title_class=title_class %}
+    {% include 'queryset/queryset.html' with data=data title_class=title_class %}
 {% endif %}
 
 {% if data.type == 'statistics' %}
-    {% include 'app/statistics.html' with data=data title_class=title_class %}
+    {% include 'queryset/statistics.html' with data=data title_class=title_class %}
 {% endif %}
 
 {% if data.type == 'primitive' %}
-    {% include 'app/valueset/primitive.html' with data=data %}
+    <div class="reloadable-fieldset" id="{{ data.key }}" data-path="{{ data.path }}">
+    {% include 'valueset/primitive.html' with data=data %}
+    </div>
 {% endif %}
```

#### html2text {}

```diff
@@ -1,17 +1,24 @@
-{% load tags %} {% if data.type == 'fieldset' %} {% if data.template %} {%
-include data.template with data=data %} {% else %}
-{% if data.name %}
+{% load tags %} {% if data.type == 'fieldset' %}
+{% if data.template %} {% include data.template with data=data %} {% else %} {%
+if data.name %}
  {{ data.name }}
 {% endif %}
-{% if data.actions %} {% include "app/actions.html" with uuid=data.uuid
+{% if data.actions %} {% include "dashboard/actions.html" with uuid=data.uuid
 target="model" actions=data.actions %} {% endif %}
+{% for action in data.inline_actions %} {% action action.key data.instance
+action.path %} {% endfor %} {% if data.image %}
 [{{ data.image }}]
-{% for k, v in data.data.items %} {% include 'app/valueset/field.html' with k=k
-v=v %} {% endfor %}
+{% endif %}
+{% for v in data.data.values %}{% include 'valueset/field.html' with v=v %}{%
+endfor %}
+{% if data.image %}
+{% endif %}
 {% if data.refresh %}
- {% endif %} {% endif %} {% endif %} {% if data.type == 'queryset' %} {%
-include 'app/queryset/queryset.html' with data=data title_class=title_class %}
-{% endif %} {% if data.type == 'statistics' %} {% include 'app/statistics.html'
-with data=data title_class=title_class %} {% endif %} {% if data.type ==
-'primitive' %} {% include 'app/valueset/primitive.html' with data=data %} {%
-endif %}
+ {% endif %} {% endif %}
+{% endif %} {% if data.type == 'queryset' %} {% include 'queryset/
+queryset.html' with data=data title_class=title_class %} {% endif %} {% if
+data.type == 'statistics' %} {% include 'queryset/statistics.html' with
+data=data title_class=title_class %} {% endif %} {% if data.type == 'primitive'
+%}
+{% include 'valueset/primitive.html' with data=data %}
+{% endif %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/valueset/value.html` & `django-sloth-0.1.0/sloth/api/templates/valueset/value.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 {% load tags %}
 
 {% if v|is_valueset %}
     <dl>
-    {% for k2, v2 in v.items %}
+    {% for v2 in v.values %}
         {% if v2.metadata.icon %}
             <dt></dt>
             <dd>
             {{ v2.metadata.icon|icontag }}
             {% if v2.template %}
                 {% include v2.template with value=v2.value metadata=v2.metadata %}
             {% else %}
                 {{ v2.value|format|linebreaksbr }}
             {% endif %}
             </dd>
         {% else %}
-            <dt>{{ k2 }}</dt>
+            <dt>{{ v2.name }}</dt>
             <dd>
                 {% if v2.template %}
                     {% include v2.template with value=v2.value metadata=v2.metadata %}
                 {% else %}
                     {{ v2.value|format|linebreaksbr }}
                 {% endif %}
             </dd>
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/app/valueset/valueset.html` & `django-sloth-0.1.0/sloth/api/templates/valueset/valueset.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 {% load tags %}
 <div class="valueset row clearfix">
     <div class="{% if append %}col-lg-9 col-md-8 col-sm-12{% else %}col{% endif %}">
+
+        {% include "dashboard/shortcuts.html" with shortcuts=data.instance.data.shortcuts %}
+        {% include "dashboard/cards.html" with cards=data.instance.data.cards %}
+
         <div class="valueset-header">
             <div class="valueset-title">
                 {% if data.title %}
                     <div class="valueset-title pb-1">
                         {% if data.title.template %}
                             {% include data.subtitle.template with value=data.title.value metadata=data.title.metadata %}
                         {% else %}
@@ -30,67 +34,91 @@
                         {% else %}
                             <div class="valueset-status-text">{{ data.status.value }}</div>
                         {% endif %}
                     </div>
                 {% endif %}
             </div>
             <div class="valueset-action-bar">
-                  {% if data.actions %}
-                      {% include "app/actions.html" with uuid=data.uuid target="model" actions=data.actions   %}
+                  {% if data.actions and not print %}
+                      {% include "dashboard/actions.html" with uuid=data.uuid target="model" actions=data.actions   %}
                   {% endif %}
             </div>
         </div>
 
         <div class="clearfix"></div>
+        {% for action in data.inline_actions %}
+            <div class="fieldset-inline-action">
+                {% action action.key data.instance action.path %}
+            </div>
+        {% endfor %}
 
         <div class="valueset-attaches">
             {% if data.attach %}
             <ul class="nav justify-content-center">
                 {% for item in data.attach %}
                   <li class="nav-item">
-                    <a class="nav-link" href="/app{{ item.path }}">{{ item.name }}</a>
+                    <a class="nav-link" href="{{ item.path }}">{{ item.name }}</a>
                   </li>
                 {% endfor %}
             </ul>
             {% endif %}
         </div>
-
-        <div class="valueset-fieldsets">
-        {% for name, item in data.data.items %}
-            <div class="fieldset" id="{{ item.key }}">
-                {% if item.type == 'fieldset-group' %}
-                    {% include 'app/valueset/fieldset-group.html' with item=item %}
-                {% endif %}
-                {% if item.type == 'fieldset-list' %}
-                    {% include 'app/valueset/fieldset-list.html' with item=item %}
-                {% endif %}
-                {% if item.type == 'fieldset' %}
-                    {% include 'app/valueset/fieldset.html' with data=item %}
-                {% endif %}
-                {% if item.type == 'queryset' %}
-                    {% include 'app/valueset/fieldset.html' with data=item %}
-                {% endif %}
-                {% if item.type == 'statistics' %}
-                    {% include 'app/valueset/fieldset.html' with data=item %}
-                {% endif %}
-                {% if item.type == 'primitive' %}
-                    {% if item.template %}
-                        {% include item.template with value=item.value metadata=item.metadata %}
-                    {% else %}
-                        {% include 'app/valueset/field.html' with k=name v=item %}
-                    {% endif %}
+        {% if data.template %}
+            {% include data.template with data=data.data %}
+        {% else %}
+            {% if data.data %}
+            <div class="valueset-fieldsets">
+                {% if data.data|has_only_primitive_fields %}
+                    <div class="box">
+                        {% for name, item in data.data.items %}
+                            {% if item.template %}
+                                {% include item.template with value=item.value metadata=item.metadata %}
+                            {% else %}
+                                {% include 'valueset/field.html' with v=item %}
+                            {% endif %}
+                        {% endfor %}
+                    </div>
+                {% else %}
+                    {% for name, item in data.data.items %}
+                        {% if item.type == 'fieldset-group' %}
+                            {% include 'valueset/fieldset-group.html' with item=item %}
+                        {% endif %}
+                        {% if item.type == 'fieldset-list' %}
+                            {% include 'valueset/fieldset-list.html' with item=item %}
+                        {% endif %}
+                        {% if item.type == 'fieldset' %}
+                            {% include 'valueset/fieldset.html' with data=item %}
+                        {% endif %}
+                        {% if item.type == 'queryset' %}
+                            {% include 'valueset/fieldset.html' with data=item %}
+                        {% endif %}
+                        {% if item.type == 'statistics' %}
+                            {% include 'valueset/fieldset.html' with data=item %}
+                        {% endif %}
+                        {% if item.type == 'primitive' %}
+                            <div class="reloadable-fieldset box" id="{{ item.key }}" data-path="{{ item.path }}">
+                            {% if item.template %}
+                                {% include item.template with value=item.value metadata=item.metadata %}
+                            {% else %}
+                                {% include 'valueset/field.html' with v=item %}
+                            {% endif %}
+                            </div>
+                        {% endif %}
+                    {% endfor %}
                 {% endif %}
             </div>
-        {% endfor %}
-        </div>
+            {% endif %}
+        {% endif %}
     </div>
     {% if data.append %}
     <div class="col-lg-3 col-md-4 col-sm-12 fieldset-side-panel">
         {% for name, item in data.append.items %}
-            {% include 'app/valueset/fieldset.html' with data=item compact=True %}
+            <div class="reloadable-fieldset" id="{{ item.key }}" data-path="{{ item.path }}?compact=1">
+                {% include 'valueset/fieldset.html' with data=item compact=True %}
+            </div>
         {% endfor %}
     </div>
     {% endif %}
 
 </div>
```

### Comparing `django-sloth-0.0.54/sloth/app/templates/renderers/calendar/calendar.html` & `django-sloth-0.1.0/sloth/api/templates/renderers/calendar/calendar.html`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/templates/renderers/maps/map.html` & `django-sloth-0.1.0/sloth/api/templates/renderers/maps/map.html`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/templates/renderers/programing/strtable.html` & `django-sloth-0.1.0/sloth/api/templates/renderers/programing/strtable.html`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/app/templates/renderers/utils/steps.html` & `django-sloth-0.1.0/sloth/api/templates/renderers/utils/steps.html`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 		border-left: solid 1px;
 		border-color: #BBB;
 		width: 1;
 		margin: auto;
 	}
 </style>
 
-{% if request|mobile or compact %}
+{% if request|mobile or compact or request.GET.compact %}
 <div class="steps-vertical">
     {% for step, date in value %}
         <div class="step">
             <div class="cicle {% if date %}active bg-primary border border-primary{% endif %}">{{ forloop.counter }}</div>
             <div class="text">{{ step }} {% if date %}<div class="text-date">{{ date }}</div>{% endif %}</div>
         </div>
         {% if not forloop.last %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% load tags %}
- {% if request|mobile or compact %}
+ {% if request|mobile or compact or request.GET.compact %}
 {% for step, date in value %}
 {{ forloop.counter }}
 {{ step }} {% if date %}
 {{ date }}
 {% endif %}
 {% if not forloop.last %}
 {% endif %} {% endfor %}
```

### Comparing `django-sloth-0.0.54/sloth/app/templatetags/tags.py` & `django-sloth-0.1.0/sloth/api/templatetags/tags.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # -*- coding: utf-8 -*-
 import locale
 import datetime
 import unicodedata
+from django import template
 from django.template import Library
 from django.utils.safestring import mark_safe
 from django.template.loader import render_to_string
 from sloth.utils.formatter import format_value
 from sloth.utils import colors, to_snake_case
 from sloth.actions import ACTIONS
 
 
 register = Library()
 
 
 @register.filter
+def breaklines(text):
+    return text.replace('\n', '<br>')
+
+
+@register.filter
 def is_ajax(request):
     return request.headers.get('x-requested-with') == 'XMLHttpRequest'
 
 
 @register.filter('format')
 def _format(value):
     return format_value(value)
@@ -264,8 +270,59 @@
 
 @register.filter
 def action_link(action_name):
     cls = ACTIONS[action_name]
     metadata = cls.get_metadata()
     return mark_safe('<a href="/app/action/{}/" class="{}">{}</a>'.format(
         to_snake_case(action_name), 'popup' if metadata['modal'] else '', metadata['name']
-    ))
+    ))
+
+
+@register.filter
+def url_slug(url):
+    return url[1:-1].replace('/', '__')
+
+
+@register.filter
+def post_querystring(request):
+    params = ['post__{}={}'.format(k, v) for k, v in request.POST.items() if k!='csrfmiddlewaretoken']
+    params.extend(['{}={}'.format(k, v) for k, v in request.GET.items() if k.startswith('post__') and k not in params])
+    return mark_safe('{}'.format('&'.join(params))) if params else ''
+
+
+@register.filter
+def start_querystring(path):
+    if '?' in path:
+        return mark_safe('{}&'.format(path))
+    return mark_safe('{}?'.format(path))
+
+
+@register.filter
+def has_only_primitive_fields(fieldset):
+    for value in fieldset.values():
+        if value['type'] != 'primitive':
+            return False
+    return True
+
+
+@register.tag
+def action(parser,token):
+    _, action_name, instantiator, fieldset_name = token.split_contents()
+    return ActionNode(action_name, instantiator, fieldset_name)
+
+
+class ActionNode(template.Node):
+    def __init__(self, action_name, instantiator, path=None):
+        self.request = template.Variable('request')
+        self.action_name = template.Variable(action_name)
+        self.instantiator = template.Variable(instantiator)
+        self.path = template.Variable(path)
+
+    def render(self, context):
+        request = self.request.resolve(context)
+        action_name = self.action_name.resolve(context)
+        instantiator = self.instantiator.resolve(context)
+        cls = ACTIONS[action_name]
+        form = cls(request=request, instantiator=instantiator)
+        form.path = self.path.resolve(context)
+        form.is_valid()
+        return form.html()
```

### Comparing `django-sloth-0.0.54/sloth/core/base.py` & `django-sloth-0.1.0/sloth/core/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,31 +44,32 @@
         from sloth import RoleLookup
         return RoleLookup(self).role_lookups(*names, **scopes)
 
     def has_permission(self, user):
         return user.is_superuser
 
     def has_view_permission(self, user):
-        return user.is_superuser or self.has_permission(user)
+        return user.is_superuser or self.has_permission(user) or self.is_autouser(user)
 
     def has_attr_permission(self, user, name):
         attr = getattr(self, 'has_{}_permission'.format(name), None)
-        return  attr is None or user.is_superuser or attr(user)
+        return attr is None or user.is_superuser or attr(user)
 
     def has_view_attr_permission(self, user, name):
         if user.is_superuser or self.has_permission(user):
             return True
         if self.is_view_attr(name) and self.has_view_permission(user):
             return True
         attr = getattr(self, 'has_{}_permission'.format(name), None)
         return attr(user) if attr else False
 
     def is_view_attr(self, name):
         if not hasattr(self.__class__, '__view__'):
             attr_names = []
+
             def append_attr_names(valueset):
                 names = list(valueset.metadata['names'].keys())
                 names.extend(valueset.metadata['append'])
                 names.extend(valueset.metadata['attach'])
                 # if all names starts with "get_" it is certainly a fieldset list or fieldset group
                 # if all([attr_name.startswith('get_') for attr_name in names]):
                 if valueset.has_children():
@@ -79,46 +80,44 @@
                             if isinstance(attr, ValueSet):
                                 append_attr_names(attr)
             append_attr_names(self.view())
             setattr(self.__class__, '__view__', attr_names)
         return name in getattr(self.__class__, '__view__')
 
     def has_add_permission(self, user):
-        return user.is_superuser or self.has_permission(user)
+        return user.is_superuser or self.has_permission(user) or (hasattr(self, 'autouser') and self.is_autouser(user))
 
     def has_edit_permission(self, user):
-        return user.is_superuser or self.has_permission(user)
+        return user.is_superuser or self.has_permission(user) or self.is_autouser(user)
 
     def has_delete_permission(self, user):
-        return user.is_superuser or self.has_permission(user)
+        return user.is_superuser or self.has_permission(user) or self.is_autouser(user)
+
+    def is_autouser(self, user):
+        return getattr(self, 'autouser', None) == user
 
     ### VISUALIZATION ###
 
-    def values(self, *names):
+    def value_set(self, *names):
         return ValueSet(self, names)
 
     def view(self):
         names = [field.name for field in self.metaclass().fields]
-        return self.values(*names)
+        return self.value_set(*names)
 
-    def display(self, name):
-        if name == 'self':
-            return self.view()
-        return self.values(name)
-
-    def serialize(self, wrap=True, verbose=True):
-        return self.view().serialize(wrap=wrap, verbose=verbose)
+    def serialize(self, wrap=True):
+        return self.view().serialize(wrap=wrap)
 
     def get_select_display(self):
         select_fields = getattr(type(self).metaclass(), 'select_fields', None)
         if select_fields:
             values = []
             for attr_name in select_fields:
                 values.append(getattr(self, attr_name))
-            return render_to_string('app/select.html', dict(obj=self, values=values))
+            return render_to_string('inputs/select.html', dict(obj=self, values=values))
         return None
 
     ### ROLE CREATION ###
 
     def get_role_tuples(self, ignore_active_condition=False):
         model = type(self)
         tuples = set()
@@ -156,18 +155,15 @@
             if scope_value:
                 user_id = User.objects.filter(username=username).values_list('id', flat=True).first()
                 scope_type = '{}.{}'.format(scope_type.metaclass().app_label, scope_type.metaclass().model_name)
                 if user_id is None:
                     user = User.objects.create(username=username)
                     if email:
                         user.email = email
-                    if 'DEFAULT_PASSWORD' in settings.SLOTH:
-                        default_password = settings.SLOTH['DEFAULT_PASSWORD'](user)
-                    else:
-                        default_password = '123' if settings.DEBUG else str(abs(hash(username)))
+                    default_password = settings.DEFAULT_PASSWORD(user)
                     user.set_password(default_password)
                     user.save()
                     user_id = user.id
                 role.objects.get_or_create(
                     user_id=user_id, name=scope_name,
                     scope_type=scope_type,
                     scope_key=scope_key, scope_value=scope_value
@@ -177,16 +173,19 @@
         for username, email, scope_name, scope_type, scope_key, scope_value in deleted_role_tuples:
             scope_type = '{}.{}'.format(scope_type.metaclass().app_label, scope_type.metaclass().model_name)
             role.objects.filter(
                 user__username=username, name=scope_name, scope_type=scope_type, scope_key=scope_key, scope_value=scope_value
             ).delete()
 
     @classmethod
-    def get_list_url(cls, prefix=''):
-        return '{}/{}/{}/'.format(prefix, cls.metaclass().app_label, cls.metaclass().model_name)
+    def get_list_url(cls, prefix='', subset='all'):
+        url = '{}/{}/{}/'.format(prefix, cls.metaclass().app_label, cls.metaclass().model_name)
+        if subset != 'all':
+            url = '{}{}/'.format(url, subset)
+        return url
 
     @classmethod
     def add_form_cls(cls):
         form_cls = cls.action_form_cls('{}{}'.format('Cadastrar', cls.__name__))
         if form_cls is None:
             class Add(Action):
                 class Meta:
@@ -251,23 +250,44 @@
                 fields = ()
                 verbose_name = 'Excluir {}'.format(cls.metaclass().verbose_name)
                 icon = 'x'
                 style = 'danger'
                 submit_label = 'Excluir'
                 confirmation = True
 
-            def save(self):
+            def submit(self):
                 self.instance.delete()
+                self.message('Exclusão realizada com sucesso.')
+                self.redirect('..')
 
             def has_permission(self, user):
                 return user.is_superuser or self.instance.has_delete_permission(user) or self.instance.has_permission(user)
 
         return Delete
 
     @classmethod
+    def relation_form_cls(cls, related_field):
+        _related_field = related_field
+
+        class Add(Action):
+            class Meta:
+                icon = 'plus'
+                modal = True
+                model = cls.get_field(_related_field).model
+                style = 'success'
+                related_field = _related_field
+                verbose_name = 'Adicionar {}'.format(cls.get_field(_related_field).model.metaclass().verbose_name)
+                fieldsets = getattr(cls.get_field(_related_field).model.metaclass(), 'fieldsets', None)
+
+            def has_permission(self, user):
+                return user.is_superuser or self.instantiator.has_edit_permission(user) or self.instantiator.has_permission(user)
+
+        return Add
+
+    @classmethod
     @lru_cache
     def action_form_cls(cls, action):
         if action.lower() == 'add':
             return cls.add_form_cls()
         elif action.lower() == 'edit':
             return cls.edit_form_cls()
         elif action.lower() == 'delete':
@@ -290,15 +310,15 @@
                 except FieldDoesNotExist:
                     pass
         return None
 
     @classmethod
     def default_list_fields(cls):
         list_display = getattr(cls.metaclass(), 'list_display', None)
-        return list_display or [field.name for field in cls.metaclass().fields[0:5] if field.name != 'id']
+        return list_display or [field.name for field in cls.metaclass().fields[0:5] if field.name != 'id' and '_ptr' not in field.name]
 
     @classmethod
     def default_filter_fields(cls, exclude=None):
         filters = getattr(cls.metaclass(), 'list_filter', None)
         if filters is None:
             filters = []
             for field in cls.metaclass().fields:
@@ -352,14 +372,17 @@
             elif isinstance(field, models.DateField):
                 param_format = 'date'
             elif isinstance(field, models.IntegerField) or isinstance(field, models.ForeignKey):
                 param_type = 'integer'
                 param_format = 'int32'
         return dict(type=param_type, format=param_format)
 
+    def get_allowed_attrs(self, recursive=True):
+        return self.view().get_allowed_attrs()
+
     @classmethod
     def get_api_paths(cls, request):
         instance = cls()
         instance.id = -1
         instance.init_one_to_one_fields()
         app_label = cls.metaclass().app_label
         if app_label == 'api':
@@ -461,7 +484,16 @@
                     'security': [dict(OAuth2=[], BasicAuth=[])]  # , BearerAuth=[], ApiKeyAuth=[]
                 }
         return paths
 
     @classmethod
     def metaclass(cls):
         return getattr(cls, '_meta')
+
+    def contextualize(self, request):
+        return self.view().contextualize(request)
+
+    def attr(self, name, source=False):
+        valueset = self.value_set(name).attr(name)
+        if source:
+            valueset = valueset.source(name)
+        return valueset
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-sloth-0.0.54/sloth/core/queryset.py` & `django-sloth-0.1.0/sloth/core/queryset.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,68 +2,102 @@
 
 import datetime
 import json
 import math
 import operator
 from functools import reduce
 from uuid import uuid1
-
+import zlib
+import pickle
+import base64
+from django.core import signing
 from django.conf import settings
 from django.contrib import messages
 from django.db import models
 from django.db.models import Q
 from django.db.models.aggregates import Sum, Count
 from django.template.loader import render_to_string
-from django.utils.text import slugify
-
+from django.apps import apps
 from sloth.utils.http import XlsResponse, CsvResponse
 from sloth.core.statistics import QuerySetStatistics
-from sloth.exceptions import JsonReadyResponseException, HtmlJsonReadyResponseException, ReadyResponseException
-from sloth.utils import getattrr, serialize, pretty, to_api_params
+from sloth.api.exceptions import JsonReadyResponseException, HtmlReadyResponseException, ReadyResponseException
+from sloth.utils import getattrr, serialize, pretty, to_snake_case
 
 
 class QuerySet(models.QuerySet):
 
     def __init__(self, *args, **kwargs):
         self.request = None
+        self.metadata = None
+        self.instantiator = None
         super().__init__(*args, **kwargs)
         self.reset()
 
     def reset(self):
-        limit = settings.SLOTH.get('LIST_PER_PAGE', 20)
         self.metadata = dict(uuid=uuid1().hex if self.model is None else self.model.__name__.lower(), subset=None,
-            display=[], view=[dict(name='self', modal=False, icon='search')], filters={}, dfilters={}, search=[],
-            page=1, limit=limit, interval='', total=0, ignore=[], only={}, is_admin=False, ordering=[],
-            actions=[], attach=[], template=None, attr=None, source=None, totalizer=None, calendar=None,
-            global_actions=[], batch_actions=[], lookups=[], collapsed=True, compact=False, verbose_name=None,
+            display=[], view=[], filters={}, dfilters={}, search=None,
+            page=1, limit=20, interval='', total=0, ignore=[], only={}, is_admin=False, ordering=[],
+            actions=[], attach=[], template=None, attr=None, source=None, aggregations=[], calendar=None,
+            global_actions=[], batch_actions=[], inline_actions=[], lookups=[], collapsed=True, compact=False,
+            verbose_name=None, related_field=None, scrollable=False
         )
+        if self.model and getattr(self.model.metaclass(), 'autouser', False):
+            self.lookups(autouser='pk')
+            self.ignore('autouser')
 
     def _clone(self):
         clone = super()._clone()
         clone.request = self.request
+        self.instantiator = self.instantiator
         clone.metadata = dict(self.metadata)
         return clone
 
+    def first(self):
+        obj = super().first()
+        if self.metadata['related_field'] and isinstance(obj, self.model):
+            obj.related_field = self.metadata['related_field']
+        return obj
+
+    def related_field(self, name):
+        self.metadata['related_field'] = name
+        return self.ignore(name)
+
     def role_lookups(self, *names, **scopes):
         for name in names:
             self.metadata['lookups'].append((name, scopes))
         return self
 
+    def lookups(self, name='Usuário', *names, **scopes):
+        self.role_lookups(*((name,) + names), **scopes)
+        return self
+
     def has_permission(self, user):
         if user.is_authenticated:
             return user.is_superuser or user.roles.contains(*(t[0] for t in self.metadata['lookups']))
         return False
 
     def has_attr_permission(self, user, name):
         if user.is_superuser:
             return True
         qs = self.model.objects.all()
         if name == 'all' or name in qs.metadata['attach']:
             return qs.has_permission(user)
-        return getattr(self, name)().has_permission(user)
+        return getattr(self._clone(), name)().has_permission(user)
+
+    def get_allowed_attrs(self, recursive=True):
+        allowed = []
+        for key in ('global_actions', 'actions', 'batch_actions', 'inline_actions'):
+            allowed.extend(self.metadata[key])
+        allowed.extend(self.metadata['attach'])
+        if recursive:
+            for attach in self.metadata['attach']:
+                allowed.extend(getattr(self._clone(), attach)().get_allowed_attrs(recursive=False))
+        for view in self.metadata['view']:
+            allowed.append('view' if view['name'] == 'self' else view['name'])
+        return allowed
 
     def apply_role_lookups(self, user):
         if user.is_superuser:
             return self
         else:
             for field_name, role_names in self.metadata['only'].items():
                 if not self.request.user.roles.contains(*role_names):
@@ -76,21 +110,24 @@
                         for scope_value in user.roles.filter(active=True, name=name, scope_key=scope_key).values_list('scope_value', flat=True):
                             lookups.append(Q(**{scope_value_attr: scope_value}))
                 else:
                     if user.roles.contains(name):
                         return self
             if lookups:
                 return self.filter(reduce(operator.__or__, lookups))
-            return self.none()
-        return self
+        return self.none() if self.metadata['is_admin'] else self
 
     def append(self, *names):
         from sloth.core.valueset import ValueSet
         return ValueSet(self, names)
 
+    def value_set(self, *names):
+        from sloth.core.valueset import ValueSet
+        return ValueSet(self, names)
+
     def get_list_display(self, add_id=False):
         if self.metadata['display']:
             list_display = self.metadata['display']
         else:
             list_display = self.model.default_list_fields()
         display = [name for name in list_display if name not in self.metadata['ignore']]
         if add_id:
@@ -102,35 +139,35 @@
             list_filter = []
         elif self.metadata['filters']:
             list_filter = self.metadata['filters']
         else:
             list_filter = self.model.default_filter_fields()
         return [name for name in list_filter if name not in self.metadata['ignore']]
 
-    def get_search(self, verbose=False):
+    def get_search(self):
         search = {}
-        if self.metadata['search'] is not None:
+        if self.metadata['search'] is None:
             for lookup in self.metadata['search'] or self.model.default_search_fields():
                 verbose_name = self.model.get_attr_metadata(lookup)[0]
-                search[verbose_name if verbose else lookup] = dict(key=lookup, name=verbose_name)
+                search[lookup] = dict(key=lookup, name=verbose_name)
         return search
 
-    def get_display(self, verbose=False):
+    def get_display(self):
         display = {}
         for lookup in self.get_list_display():
-            verbose_name, sort, template, metadata = self.model.get_attr_metadata(lookup)
-            display[pretty(verbose_name) if verbose else lookup] = dict(
-                key=lookup, name=pretty(verbose_name), sort=sort, template=template, metadata=metadata
+            verbose_name, sort, _, _ = self.model.get_attr_metadata(lookup)
+            display[lookup] = dict(
+                key=lookup, name=pretty(verbose_name), sort=sort#, template=template, metadata=metadata
             )
         return display
 
     def filter_form_cls(self):
-        return self.get_filters(verbose=False, as_form=True)
+        return self.get_filters(as_form=True)
 
-    def get_filters(self, verbose=False, as_form=False):
+    def get_filters(self, as_form=False):
         from sloth import actions
         filters = {}
         list_filter = self.get_list_filters()
         list_filter.extend(self.metadata['dfilters'])
         if self.metadata['calendar']:
             list_filter.append(self.metadata['calendar'])
         for lookup in list_filter:
@@ -144,42 +181,50 @@
             elif isinstance(formfield, actions.DateField):
                 filter_type = 'date'
             if lookup in self.metadata['dfilters']:
                 qs = self.order_by(lookup).values_list(lookup).distinct()[1:2]
                 if not qs:
                     continue
 
-            key = pretty(str(field.verbose_name)) if verbose else lookup
+            key = lookup
             name = pretty(str(field.verbose_name))
             if filter_type in ('datetime', 'date'):
                 for sublookup, symbol in dict(gte='>', lte='<').items():
-                    k = '{} {}'.format(symbol, key) if verbose else '{}__{}'.format(key, sublookup)
+                    k = '{}__{}'.format(key, sublookup)
                     n = '{} {}'.format(symbol, name)
                     hidden = lookup == self.metadata['calendar']
                     formfield = field.formfield(label=n, required=False)
-                    filters[k] = dict(key='{}__{}'.format(
-                        lookup, sublookup), name=n, type=filter_type, choices=None, hidden=hidden
+                    fkey = '{}__{}'.format(lookup, sublookup)
+                    filters[k] = dict(key=fkey, name=n, type=filter_type, choices=None, hidden=hidden, value=self.request.GET.get(fkey) if self.request else None
                     )
-                    if as_form:
-                        filters[k].update(formfield=formfield)
+            elif filter_type == 'choices':
+                value = None
+                if self.request and self.request.GET.get(lookup):
+                    value = [self.request.GET.get(f'{lookup}0'), self.request.GET.get(lookup)]
+                filters[key] = dict(key=lookup, name=name, type=filter_type, choices=None, hidden=False, value=value)
             else:
                 filters[key] = dict(
-                    key=lookup, name=name, type=filter_type, choices=None, hidden=False
+                    key=lookup, name=name, type=filter_type, choices=None, hidden=False, value=self.request.GET.get(lookup) if self.request else None
                 )
-                if as_form:
-                    filters[key].update(formfield=formfield)
+            if as_form:
+                filters[key].update(formfield=formfield)
+            if filter_type == 'boolean':
+                filters[key]['value'] = int(filters[key]['value']) if filters[key]['value'] else None
 
         ordering = []
         for lookup in self.metadata['ordering']:
             field = self.model.get_field(lookup)
             ordering.append(dict(id=lookup, text=field.verbose_name))
         if ordering:
-            key = 'Ordenação' if verbose else 'ordenacao'
+            value = None
+            key = 'ordering'
+            if self.request and self.request.GET.get(key):
+                value = [self.request.GET.get(f'{key}0'), self.request.GET.get(key)]
             filters[key] = dict(
-                key='ordering', name='Ordenação', type='choices', choices=ordering
+                key='ordering', name='Ordenação', type='choices', choices=ordering, value=value
             )
             if as_form:
                 choices = [(o['id'], [o['text']]) for o in ordering]
                 filters[key].update(formfield=actions.ChoiceField(label='Ordenação', choices=choices, required=False))
 
         if as_form:
             class FilterForm(actions.Action):
@@ -192,36 +237,40 @@
                     for key in filters:
                         self.fields[key] = filters[key]['formfield']
 
             return FilterForm
 
         return filters
 
-    def get_attach(self, verbose=False):
+    def get_attach(self):
+        if isinstance(self.metadata['attach'], dict):
+            return self.metadata['attach']
         attaches = {}
         if self.metadata['attach'] and not self.query.is_sliced:
             for i, name in enumerate(['all'] + self.metadata['attach']):
                 attr = getattr(self._clone(), name)
                 attach = attr()
                 if self.request and hasattr(attach, 'apply_role_lookups'):
                     attach = attach.apply_role_lookups(self.request.user)
                 if hasattr(attr, '__verbose_name__'):
                     verbose_name = attr.__verbose_name__
                 else:
                     verbose_name = attach.metadata['verbose_name'] or pretty(name)
+                active = self.request.GET.get('subset', 'all') if self.request else 'all'
                 if isinstance(attach, QuerySet):
-                    if name == 'all':
+                    if verbose_name.lower() == 'all':
                         verbose_name = 'Tudo'
-                    attaches[verbose_name if verbose else name] = dict(
-                        name=verbose_name, key=name, count=attach.count(), active=i == 0
+                    attaches[name] = dict(
+                        name=verbose_name, key=name, count=attach.count(), active=name == active
                     )
                 else:
-                    attaches[verbose_name if verbose else name] = dict(
-                        name=verbose_name, key=name, active=i == 0
+                    attaches[name] = dict(
+                        name=verbose_name, key=name, active=name == active
                     )
+        self.metadata['attach'] = attaches
         return attaches
 
     # choices function
 
     def choices(self, request):
         filter_lookup = request.GET['choices']
         q = request.GET.get('term')
@@ -289,56 +338,56 @@
             first_day_of_previous_month = first_day_of_previous_month - datetime.timedelta(days=1)
         first_day_of_next_month = last_day_of_month + datetime.timedelta(days=1)
         last_day_of_next_month = first_day_of_next_month + datetime.timedelta(days=1)
         while last_day_of_next_month.month == first_day_of_next_month.month:
             last_day_of_next_month = last_day_of_next_month + datetime.timedelta(days=1)
         last_day_of_next_month = last_day_of_next_month - datetime.timedelta(days=1)
         selected_date = self.request.GET.get('selected-date')
-        if  selected_date:
+        if selected_date:
             selected_date = datetime.datetime.strptime(selected_date, '%d/%m/%Y').date()
         # print(first_day_of_month, last_day_of_month)
         # print(first_day_of_previous_month, last_day_of_previous_month)
         # print(first_day_of_next_month, last_day_of_next_month)
         return dict(
             field=attr_name, days=days,
             previous=dict(first_day=first_day_of_previous_month, last_day=last_day_of_previous_month),
             next=dict(first_day=first_day_of_next_month, last_day=last_day_of_next_month),
             selected_date=selected_date, today=datetime.date.today()
         )
 
     # serialization function
 
-    def to_list(self, wrap=False, verbose=False, detail=True):
+    def to_list(self, wrap=False, detail=True):
         data = []
         for obj in self:
-            add_id = not wrap and not verbose
+            add_id = not wrap
             actions = self.get_obj_actions(obj)
             if self.request:
                 for view in self.metadata['view']:
                     if view['name'] == 'self':
                         has_view_permission = obj.has_view_permission(self.request.user)
                     else:
                         has_view_permission = obj.has_view_attr_permission(self.request.user, view['name'])
                     if self.request.user.is_superuser or has_view_permission or obj.has_permission(self.request.user):
                         actions.append(view['name'])
-            item = obj.values(*self.get_list_display(add_id=add_id)).load(wrap=False, verbose=verbose, detail=detail)
+            item = obj.value_set(*self.get_list_display(add_id=add_id)).load(wrap=False, detail=detail)
             data.append(dict(id=obj.id, description=str(obj), data=item, actions=actions) if wrap else item)
         return data
 
     def export(self, limit=100):
         data = []
         header = []
         for i, obj in enumerate(self[0:limit]):
             if i == 0:
                 for attr_name in self.get_list_display():
                     attr, value = getattrr(obj, attr_name)
-                    header.append(getattr(attr, 'verbose_name', attr_name))
+                    header.append(pretty(self.model.get_attr_metadata(attr_name)[0]).upper())
                 data.append(header)
             row = []
-            values = obj.values(*self.get_list_display()).load(wrap=False, verbose=False, detail=False).values()
+            values = obj.value_set(*self.get_list_display()).load(wrap=False, detail=False).values()
             for value in values:
                 if value is None:
                     value = ''
                 if isinstance(value, list) or isinstance(value, tuple) or hasattr(value, 'all'):
                     value = ', '.join([str(o) for o in value])
                 row.append(serialize(value))
             data.append(row)
@@ -349,168 +398,183 @@
         for form_name in self.metadata['actions']:
             form_cls = self.model.action_form_cls(form_name)
             if form_cls is None:
                 raise BaseException('Action does not exist: {}'.format(form_name))
             if self.request is None or form_cls.check_fake_permission(
                     request=self.request, instance=obj
             ):
-                actions.append(form_cls.__name__)
+                actions.append(form_cls.get_api_name())
         return actions
 
-    def serialize(self, path=None, wrap=False, verbose=True, lazy=False):
+    def serialize(self, path=None, wrap=False, lazy=False):
         if wrap:
             if self.metadata['verbose_name']:
                 verbose_name = self.metadata['verbose_name']
             elif self.metadata['attr']:
                 verbose_name = pretty(self.metadata['attr'])
             else:
                 verbose_name = pretty(self.model.metaclass().verbose_name_plural)
 
             for lookup in self.metadata['dfilters']:
                 qs = self.order_by(lookup).values_list(lookup).distinct()[1:2]
                 if not qs and lookup not in self.metadata['ignore']:
                     self.metadata['ignore'].append(lookup)
 
+            total = self.count()
             icon = getattr(self.model.metaclass(), 'icon', None)
-            search = self.get_search(verbose)
-            display = self.get_display(verbose)
-            filters = self.get_filters(verbose)
-            attach = self.get_attach(verbose) if self.metadata['attr'] is None else {}
+            search = self.get_search()
+            display = self.get_display()
+            filters = self.get_filters()
+            attach = self.get_attach() if self.metadata['attr'] is None else {}
             calendar = self.to_calendar() if self.metadata['calendar'] and not lazy else None
-            values = {} if lazy else self.paginate().to_list(wrap=wrap, verbose=verbose, detail=True)
+            values = {} if lazy else self.paginate().to_list(wrap=wrap, detail=True)
             pages = []
-            n_pages = ((self.count()-1) // self.metadata['limit']) + 1
+            n_pages = ((total-1) // self.metadata['limit']) + 1
             for page in range(0, n_pages):
                 if page < 4 or (page > self.metadata['page'] - 3 and page < self.metadata['page'] + 1) or page > n_pages - 5:
                     pages.append(page + 1)
             pagination = dict(
                 interval=self.metadata['interval'],
-                total=self.metadata['total'],
+                total=total,
                 page=self.metadata['page'],
                 pages=pages
             )
             data = dict(
-                uuid=self.metadata['uuid'], type='queryset',
-                name=verbose_name, key=None, icon=icon, count=n_pages,
+                uuid=self.metadata['uuid'], type='queryset', path=path,
+                name=verbose_name, key=self.metadata['uuid'], icon=icon, count=n_pages,
                 actions={}, metadata={}, data=values
             )
+            if self.request and self.request.path.startswith('/app/'):
+                data.update(instantiator=self.instantiator)
             if attach:
                 data.update(attach=attach)
 
-            # path where queryset is instantiated
-            if self.request:
-                prefix = self.request.path.split('/')[1]
-                if self.metadata['attr']:
-                    # if it is a relationship of an object. Ex: /base/servidor/3/get_ferias/
-                    path = self.request.path.replace('/{}'.format(prefix), '')
-                if path is None:
-                    if self.request:
-                        data.update(path=self.request.get_full_path().replace('/{}'.format(prefix), ''))
-                else:
-                    data.update(path=path)
-
             if not lazy:
+                collapsed = bool(self.request and self.request.GET.get('collapsed', self.metadata['collapsed']) or 0)
+                subset = self.request and self.request.GET.get('subset', 'all') or 'all'
                 data['metadata'].update(
                     search=search, display=display, filters=filters, pagination=pagination,
-                    collapsed=self.metadata['collapsed'], compact=self.metadata['compact'],
-                    is_admin=self.metadata['is_admin']
+                    collapsed=collapsed, subset=subset,
+                    compact=self.metadata['compact'], is_admin=self.metadata['is_admin']# , state=self.dumps()
                 )
                 if calendar:
                     data['metadata']['calendar'] = calendar
-                if self.metadata['totalizer']:
-                    data['metadata'].update(total=self.sum(self.metadata['totalizer']))
 
-                # path where actions will be executed
-                if path is None:
-                    path = '/{}/{}/'.format(
-                        self.model.metaclass().app_label, self.model.metaclass().model_name
-                    )
-                if self.metadata['subset']:
-                    path = '{}{}/'.format(path, self.metadata['subset'])
-                data['actions'].update(model=[], instance=[], queryset=[])
+                if self.metadata['aggregations']:
+                    aggregations = {}
+                    for aggregation in self.metadata['aggregations']:
+                        aggregations[aggregation] = dict(
+                            name=pretty(self.get_attr_metadata(aggregation)[0]),
+                            value=getattr(self, aggregation)()
+                        )
+                    data['metadata'].update(aggregations=aggregations)
+                if self.metadata['scrollable']:
+                    data['metadata'].update(scrollable=True)
+
+                data['actions'].update(model=[], instance=[], queryset=[], inline=[])
 
                 for view in self.metadata['view']:
                     if view['name'] == 'self':
                         view_suffix = ''
                         view_name = 'Visualizar'
                     else:
                         view_suffix = '{}/'.format(view['name'])
                         view_name = pretty(self.model.get_attr_metadata(view['name'])[0])
                     data['actions']['instance'].append(
                         dict(
                             type='view', key=view['name'], name=view_name, submit=view_name, target='instance',
                             method='get', icon=view['icon'], style='primary', ajax=False,
-                            modal=view['modal'], path='{}{{id}}/{}'.format(path, view_suffix)
+                            modal=view['modal'], path='{}{{id}}/{}'.format((path or '').split('?')[0], view_suffix)
                         )
                     )
-                for action_type in ('global_actions', 'actions', 'batch_actions'):
+                for action_type in ('global_actions', 'actions', 'batch_actions', 'inline_actions'):
+                    target = dict(global_actions='model', actions='instance', batch_actions='queryset', inline_actions='inline')[action_type]
                     for form_name in self.metadata[action_type]:
+                        if form_name == 'view':
+                            continue
                         form_cls = self.model.action_form_cls(form_name)
-                        if action_type == 'actions' or self.request is None or form_cls.check_fake_permission(
-                                request=self.request, instance=self.model(), instantiator=self._hints.get('instance')
-                        ):
-                            action = form_cls.get_metadata(
-                                path, inline=action_type == 'actions', batch=action_type == 'batch_actions'
-                            )
+                        has_permission = self.request is None or form_cls.check_fake_permission(
+                            request=self.request, instance=self.model(), instantiator=self._hints.get('instance')
+                        )
+                        if action_type == 'actions' or has_permission:
+                            action_path = path
+                            if self.request and self.request.GET.get('subset'):
+                                action_path = '{}{}/'.format(path, self.request.GET.get('subset'))
+                            action = form_cls.get_metadata(path, target)
                             data['actions'][action['target']].append(action)
+                if self.metadata['related_field']:
+                    form_cls = self.model.relation_form_cls(self.metadata['related_field'])
+                    has_permission = self.request is None or form_cls.check_fake_permission(
+                        request=self.request, instance=self.model(), instantiator=self._hints.get('instance')
+                    )
+                    if has_permission:
+                        action = form_cls.get_metadata(path, 'model')
+                        data['actions']['model'].append(action)
 
                 template = self.metadata['template']
                 if template is None:
                     template = getattr(self.model.metaclass(), 'list_template', None)
                 if template:
                     template = template if template.endswith('.html') else '{}.html'.format(template)
                     data.update(template=template)
+            # pprint(data)
             return data
         return self.to_list(detail=False)
 
     def debug(self):
-        print(json.dumps(self.serialize(wrap=True, verbose=True), indent=4, ensure_ascii=False))
+        print(json.dumps(self.serialize(wrap=True), indent=4, ensure_ascii=False))
 
     # metadata functions
 
-    def is_admin(self):
+    def admin(self):
         self.metadata['is_admin'] = True
         return self
 
-    def totalizer(self, name):
-        self.metadata['totalizer'] = name
+    def aggregations(self, *names):
+        self.metadata['aggregations'].extend(names)
         return self
 
     def verbose_name(self, name):
         # self.metadata['uuid'] = slugify(name).replace('-', '_')
         self.metadata['verbose_name'] = pretty(name)
         return self
 
-    def view(self, *names, modal=False, icon=None):
+    def preview(self, *names, modal=True, icon=None):
         for name in names:
             if name:
                 self.metadata['view'].append(dict(name=name, modal=modal, icon=icon))
             else:
                 self.metadata['view'].clear()
         return self
 
-    def display(self, *names):
+    def view(self):
+        return self.all()
+
+    def display(self, *names, add_default=False):
+        if add_default:
+            names = tuple(self.model.default_list_fields()) + names
         self.metadata['display'] = list(names)
         return self
 
     def search(self, *names, q=None):
-        if q:
+        if q is not None:
             lookups = []
             for search_field in self.metadata['search'] or self.model.default_search_fields():
                 lookups.append(Q(**{'{}__icontains'.format(search_field): q}))
             return self.filter(reduce(operator.__or__, lookups))
-        self.metadata['search'] = list(names) if names else None
+        else:
+            self.metadata['search'] = list(names) if names else []
         return self
 
     def filters(self, *names):
         self.metadata['filters'] = list(names) if names else None
         return self
 
     def dynamic_filters(self, *names):
-        self.metadata['dfilters'] = list(names)
+        self.metadata['dfilters'] = list(names) if names else None
         return self
 
     def ordering(self, *names):
         self.metadata['ordering'] = list(names)
         return self
 
     def limit_per_page(self, size):
@@ -518,198 +582,243 @@
         return self
 
     def renderer(self, name):
         self.metadata['template'] = name
         return self
 
     def attach(self, *names):
-        self.metadata['attach'] = list(names)
-        return self
+        qs = self._clone()
+        qs.metadata['attach'] = list(names)
+        return qs
 
     def ignore(self, *names):
         self.metadata['ignore'].extend(names)
         return self
 
-    def only(self, *names, role=None, roles=()):
-        if role or roles:
-            for name in names:
+    def only(self, *names, **kwargs):
+        if kwargs:
+            for name, role in kwargs.items():
                 if name not in self.metadata['only']:
                     self.metadata['only'][name] = []
-                if role:
-                    self.metadata['only'][name].append(role)
-                self.metadata['only'][name].extend(roles)
+                self.metadata['only'][name].append(role)
             return self
         return super().only(*names)
 
     def collapsed(self, flag=True):
         self.metadata['collapsed'] = flag
         return self
 
+    def expand(self):
+        return self.collapsed(False)
+
+    def template(self, name):
+        self.metadata['template'] = name if '.html' in name else '{}.html'.format(name)
+        return self
+
     def compact(self, flag=True):
         self.metadata['compact'] = flag
         return self
 
-    def attr(self, name):
+    def attr(self, name, source=False):
         self.metadata['attr'] = name
         self.metadata['uuid'] = name
         if self.metadata['verbose_name'] is None:
-            self.metadata['verbose_name'] = pretty(name)
-        return self
+            self.metadata['verbose_name'] = self.get_attr_metadata(name)[0]
+        if source:
+            self.metadata['is_admin'] = True
+            self.metadata['collapsed'] = False
+            self.metadata['verbose_name'] = self.get_attr_metadata(name)[0]
+        return getattr(self._clone(), name)()
+
+    @classmethod
+    def get_attr_metadata(cls, lookup):
+        attr = getattr(cls, lookup)
+        template = getattr(attr, '__template__', None)
+        metadata = getattr(attr, '__metadata__', None)
+        if template:
+            if not template.endswith('.html'):
+                template = '{}.html'.format(template)
+            if not template.startswith('.html'):
+                template = 'renderers/{}'.format(template)
+        return getattr(attr, '__verbose_name__', pretty(lookup)), False, template, metadata
 
     def source(self, name):
         self.metadata['source'] = name
         return self
 
     def page(self, n):
         self.metadata['page'] = n
         return self
 
     # action functions
 
-    def actions(self, *names):
-        self.metadata['actions'] = list(names)
+    def actions(self, *names, clear=False):
+        if clear:
+            self.metadata['actions'].clear()
+        for name in names:
+            if name == 'view':
+                self.metadata['view'].append(dict(name='self', modal=False, icon='search'))
+            elif to_snake_case(name) not in self.metadata['actions']:
+                self.metadata['actions'].append(to_snake_case(name))
+        return self
+
+    def global_actions(self, *names, clear=False):
+        if clear:
+            self.metadata['global_actions'].clear()
+        self.metadata['global_actions'].extend(
+            [to_snake_case(name) for name in names if to_snake_case(name) not in self.metadata['global_actions']]
+        )
         return self
 
-    def global_actions(self, *names):
-        self.metadata['global_actions'] = list(names)
+    def batch_actions(self, *names, clear=False):
+        if clear:
+            self.metadata['batch_actions'].clear()
+        self.metadata['batch_actions'].extend(
+            [to_snake_case(name) for name in names if to_snake_case(name) not in self.metadata['batch_actions']]
+        )
         return self
 
-    def batch_actions(self, *names):
-        self.metadata['batch_actions'] = list(names)
+    def inline_actions(self, *names, clear=False):
+        if clear:
+            self.metadata['inline_actions'].clear()
+        self.metadata['inline_actions'].extend(
+            [to_snake_case(name) for name in names if to_snake_case(name) not in self.metadata['inline_actions']]
+        )
         return self
 
     def default_actions(self):
         if self.metadata['attr'] is None:
-            self.metadata['actions'].extend(('edit', 'delete'))
-            self.metadata['global_actions'].extend(('add',))
+            self.actions('view', 'edit', 'delete')
+            self.global_actions('add')
         return self
 
     # search and pagination functions
 
-    def paginate(self):
-        if self.metadata['page'] != 1:
-            start = (self.metadata['page'] - 1) * self.metadata['limit']
-            end = start + self.metadata['limit']
-            self.metadata['interval'] = '{} - {}'.format(start + 1, end)
-            qs = self.order_by(*self.metadata['ordering'] or ['id'])[start:end]
+    def get_ordering(self):
+        ordering = self.request.GET.get('ordering') if self.request else None
+        if ordering:
+            return [ordering]
         else:
-            self.metadata['interval'] = '{} - {}'.format(0 + 1, self.metadata['limit'])
-            start = (self.metadata['page'] - 1) * self.metadata['limit']
-            end = start + self.metadata['limit']
-            self.metadata['interval'] = '{} - {}'.format(start + 1, end)
-            qs = self.filter(pk__in=self.values_list('pk', flat=True).order_by(*self.metadata['ordering'] or ['id'])[start:end])
+            return self.query.order_by or ['id']
 
+    def scrollable(self, flag=True):
+        self.metadata['scrollable'] = flag
+        return self.datatable()
+
+    def paginate(self):
+        qs = self
         if self.metadata['calendar'] and 'selected-date' in self.request.GET:
             selected_date = self.request.GET['selected-date']
             if selected_date:
                 lookups = {
                     '{}__gte'.format(self.metadata['calendar']): datetime.datetime.strptime(selected_date, '%d/%m/%Y').date(),
                     '{}__lt'.format(self.metadata['calendar']): datetime.datetime.strptime(selected_date, '%d/%m/%Y').date() + datetime.timedelta(days=1)
                 }
                 qs = qs.filter(**lookups)
 
+        if self.metadata['page'] != 1:
+            start = (self.metadata['page'] - 1) * self.metadata['limit']
+            end = start + self.metadata['limit']
+            self.metadata['interval'] = (start + 1, end)
+            qs = qs.order_by(*self.get_ordering())[start:end]
+        else:
+            self.metadata['interval'] = 0 + 1, self.metadata['limit']
+            start = (self.metadata['page'] - 1) * self.metadata['limit']
+            end = start + self.metadata['limit']
+            self.metadata['interval'] = start + 1, end
+            qs = qs.filter(pk__in=self.values_list('pk', flat=True)).order_by(*self.get_ordering())[start:end]
         return qs
 
     # rendering function
 
-    def html(self, path=None):
-        serialized = self.serialize(path=path, wrap=True, verbose=True)
+    def html(self, path=None, print=False):
+        serialized = self.serialize(path=path or self.request.path, wrap=True)
         if self.metadata['source']:
             if hasattr(self.metadata['source'], 'model'):
                 name = self.metadata['source'].model.metaclass().verbose_name_plural
             else:
                 name = self.metadata['source']
             data = dict(
                 type='object', name=str(name),
                 icon=None, data={serialized['name']: serialized}, actions=[], attach=[], append={}
             )
             # print(json.dumps(data, indent=4, ensure_ascii=False))
-            return render_to_string('app/valueset/valueset.html', dict(data=data), request=self.request)
+            return render_to_string('valueset/valueset.html', dict(data=data), request=self.request)
         return render_to_string(
-            'app/queryset/queryset.html',
-            dict(data=serialized, uuid=self.metadata['uuid'], messages=messages.get_messages(self.request)),
+            'queryset/queryset.html',
+            dict(data=serialized, uuid=self.metadata['uuid'], messages=messages.get_messages(self.request), print=print),
             request=self.request
         )
 
     def __str__(self):
         if self.request:
             return self.html()
         return super().__str__()
 
     # request functions
-
     def contextualize(self, request):
-        if request:
-            self.request = request
+        self.request = request
+        if request and request.user.is_superuser and 'autouser' in self.metadata['ignore']:
+            self.metadata['ignore'].remove('autouser')
+        if request and self.metadata['uuid'] == request.GET.get('uuid'):
             if 'choices' in request.GET:
                 raise JsonReadyResponseException(
-                    self.choices(request)
+                    self.process_request(request).choices(request)
                 )
-            if 'export' in request.GET:
-                export = request.GET['export']
-                if export == 'xls':
-                    raise ReadyResponseException(
-                        XlsResponse(
-                            [([self.model.metaclass().verbose_name_plural, self.export()])]
-                        )
-                    )
-                if export == 'csv':
-                    raise ReadyResponseException(
-                        CsvResponse(self.export())
-                    )
-            if 'attaches' in request.GET:
-                raise JsonReadyResponseException(self.get_attach())
-            if self.metadata['uuid'] == request.GET.get('uuid'):
-                component = self.process_request(request).apply_role_lookups(request.user)
-                if 'uuid' in request.GET:
-                    raise HtmlJsonReadyResponseException(component.html())
-                else:
-                    raise JsonReadyResponseException(component.serialize(verbose=False))
+            component = self.process_request(request).apply_role_lookups(request.user)
+            if request.path.startswith('/app/'):
+                raise HtmlReadyResponseException(component.html())
+            else:
+                meta = request.path.startswith('/meta/')
+                raise JsonReadyResponseException(component.serialize(wrap=meta))
             return self.apply_role_lookups(request.user)
         return self
 
     def process_request(self, request):
+        self.get_attach()
         from sloth.core.valueset import ValueSet
         page = 1
         attr_name = request.GET.get('subset', 'all')
         self.metadata['uuid'] = request.GET.get('uuid')
         if attr_name == 'all':
             attach = self
         else:
             self.metadata['subset'] = attr_name
-            attach = getattr(self, attr_name)()
+            attach = getattr(self._clone(), attr_name)()
         if isinstance(attach, QuerySet):
             qs = attach
             if self.metadata['ignore']:
                 qs.metadata['ignore'] = self.metadata['ignore']
         elif isinstance(attach, QuerySetStatistics):
             qs = attach.qs
         elif isinstance(attach, ValueSet):
             qs = attach.instance
         else:
             raise Exception()
-        qs.metadata.update(request=request)
-        for item in self.get_filters().values():
+        if request.path.startswith('/app/'):
+            qs.metadata.update(request=request)
+        for item in qs.get_filters().values():
             value = request.GET.get(item['key'])
             if value:
                 if item['key'] == 'ordering':
                     qs = qs.order_by(value)
                 else:
                     if item['type'] in ('date', 'datetime'):
-                        value = datetime.datetime.strptime(value, '%d/%m/%Y')
+                        value = datetime.datetime.strptime(value, '%d/%m/%Y' if '/' in value else '%Y-%m-%d')
                     if item['type'] == 'boolean':
                         value = bool(int(value)) if value.isdigit() else value == 'true'
-                    qs = qs.filter(**{item['key']: value})
+                    if item['key'] != request.GET.get('choices'):
+                        qs = qs.filter(**{item['key']: value})
         if 'q' in request.GET:
             qs = qs.search(q=request.GET['q'])
         if 'page' in request.GET:
             page = int(request.GET['page'] or 1)
         if isinstance(attach, QuerySet):
-            if request.GET.get('is_admin') and qs.metadata['attr'] is None and request.GET.get('subset') == 'all':
-                qs.default_actions()
+            # if request.GET.get('is_admin') and qs.metadata['attr'] is None and request.GET.get('subset') == 'all':
+            #     qs.default_actions()
             qs = qs.page(page)
             # qs.debug()
             return qs.distinct()
         if isinstance(attach, ValueSet):
             attach.instance = qs
             return attach
         else:
@@ -719,43 +828,68 @@
     # aggregation functions
 
     def count(self, x=None, y=None):
         if x:
             statistcs = QuerySetStatistics(self, x, y=y)
             return statistcs.contextualize(self.request)
         total = super().count()
-        self.metadata['total'] = total
         return total
 
     def sum(self, z, x=None, y=None):
         if x:
             if y:
                 statistcs = QuerySetStatistics(self, x, y=y, func=Sum, z=z)
             else:
                 statistcs = QuerySetStatistics(self, x, func=Sum, z=z)
             return statistcs.contextualize(self.request)
         return self.aggregate(sum=Sum(z))['sum'] or 0
 
     # rendering template functions
 
     def cards(self):
-        self.metadata['template'] = 'app/queryset/cards.html'
+        self.metadata['template'] = 'queryset/cards.html'
         return self
 
     def accordion(self):
-        self.metadata['template'] = 'app/queryset/accordion.html'
+        self.metadata['template'] = 'queryset/accordion.html'
         return self
 
     def datatable(self):
-        self.metadata['template'] = 'app/queryset/datatable.html'
+        self.metadata['template'] = 'queryset/datatable.html'
         return self
 
     def rows(self):
-        self.metadata['template'] = 'app/queryset/rows.html'
+        self.metadata['template'] = 'queryset/rows.html'
         return self
 
     def timeline(self):
-        self.metadata['template'] = 'app/queryset/timeline.html'
+        self.metadata['template'] = 'queryset/timeline.html'
         return self
 
     def normalize_email(self, email):
         return email
+
+    def dumps(self, add_metadata=True):
+        request = self.metadata.pop('request', None)
+        state = dict(app=self.model.metaclass().app_label, model=self.model.metaclass().model_name, query=self.query)
+        if add_metadata:
+            state.update(metadata=self.metadata)
+        s = signing.dumps(base64.b64encode(zlib.compress(pickle.dumps(state))).decode())
+        if request:
+            self.metadata['request'] = request
+        return s
+
+    @staticmethod
+    def loads(s):
+        state = pickle.loads(zlib.decompress(base64.b64decode(signing.loads(s).encode())))
+        model = apps.get_model(state['app'], state['model'])
+        query = state['query']
+        queryset = model.objects.none()
+        queryset.query = query
+        queryset.metadata = state['metadata']
+        return queryset
+
+    def action_form_cls(self, action):
+        return self.model.action_form_cls(action)
+
+    def get_full_path(self):
+        pass
```

### Comparing `django-sloth-0.0.54/sloth/core/validation.py` & `django-sloth-0.1.0/sloth/core/validation.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/core/valueset.py` & `django-sloth-0.1.0/sloth/core/valueset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # -*- coding: utf-8 -*-
 import json
 from uuid import uuid1
 import pprint
-
+from functools import lru_cache
 from django.db.models import Model
 from django.template.loader import render_to_string
-
+from sloth.actions import Action
 from sloth.core.queryset import QuerySet
 from sloth.core.statistics import QuerySetStatistics
-from sloth.utils import getattrr, serialize, pretty
+from sloth.utils import getattrr, serialize, pretty, to_snake_case
 
 
 def check_fieldsets_type(item):
     types = 'fieldset', 'fieldset-list', 'fieldset-group'
     for name, subitem in item.items():
         if 'type' in subitem and subitem['type'] in types:
             check_fieldsets_type(subitem['data'])
             subitem['type'] = check_fieldset_type(subitem)
 
 
 def check_fieldset_type(item):
     if is_fieldset_group(item['data']):
         first = item['data'][next(iter(item['data']))]
-        if first['type'] != 'fieldset-lit':
-            first['name'] = None
         return 'fieldset-group'
     elif is_fieldset_list(item['data']):
         return 'fieldset-list'
     else:
         return 'fieldset'
 
 
@@ -43,52 +41,65 @@
     for name, subitem in item.items():
         if 'type' in subitem and subitem['type'] == 'fieldset-list':
             return True
     return False
 
 
 class ValueSet(dict):
-    def __init__(self, instance, names, image=None):
+    def __init__(self, instance, names):
+        self.path = None
         self.request = None
         self.instance = instance
         self.metadata = dict(
             model=type(instance), names={}, metadata=[], actions=[], type=None, attr=None, source=None,
-            attach=[], append=[], image=image, template=None, primitive=False, verbose_name=None,
-            title=None, subtitle=None, status=None, icon=None, only={}, refresh={},
+            attach=[], append=[], image=None, template=None, primitive=False, verbose_name=None,
+            title=None, subtitle=None, status=None, icon=None, only={}, refresh={}, inline_actions=[],
+            cards=[], shortcuts=[], collapsed=False
         )
         for attr_name in names:
             if isinstance(attr_name, tuple):
                 for name in attr_name:
                     self.metadata['names'][name] = 100 // len(attr_name)
             else:
                 self.metadata['names'][attr_name] = 100
         super().__init__()
 
-    def only(self, name, role=None, roles=()):
-        if name not in self.metadata['only']:
-            self.metadata['only'][name] = []
-        if role:
+    def collapsed(self, flag=True):
+        self.metadata['collapsed'] = flag
+        return self
+
+    def expand(self):
+        return self.collapsed(False)
+
+    def only(self, **names):
+        for name, role in names.items():
+            if name not in self.metadata['only']:
+                self.metadata['only'][name] = []
             self.metadata['only'][name].append(role)
-        self.metadata['only'][name].extend(roles)
         return self
 
     def actions(self, *names):
-        self.metadata['actions'] = list(names)
+        self.metadata['actions'] = [to_snake_case(name) for name in names]
+        return self
+
+    def inline_actions(self, *names):
+        self.metadata['inline_actions'] = [to_snake_case(name) for name in names]
         return self
 
     def append(self, *names):
-        self.metadata['append'] = list(names)
+        self.metadata['append'] = [to_snake_case(name) for name in names]
         return self
 
     def attach(self, *names):
-        self.metadata['attach'] = list(names)
+        self.metadata['attach'] = [to_snake_case(name) for name in names]
         return self
 
     def image(self, image):
-        self.metadata['image'] = image
+        image_attr = getattr(self.instance, image)
+        self.metadata['image'] = image_attr() if callable(image_attr) else image_attr
         return self
 
     def title(self, title):
         self.metadata['title'] = title
         return self
 
     def subtitle(self, subtitle):
@@ -99,40 +110,59 @@
         self.metadata['status'] = status
         return self
 
     def renderer(self, name):
         self.metadata['template'] = name
         return self
 
+    def split(self, n=2):
+        return self.renderer('valueset/{}-column'.format(n))
+
     def verbose_name(self, name):
         self.metadata['verbose_name'] = pretty(name)
         return self
 
-    def attr(self, name):
+    def attr(self, name, source=False):
         self.metadata['attr'] = name
-        return self
+        self.metadata['names'] = {name: 100}
+        if source:
+            return self.source(name)
+        else:
+            return self
+
+    def get_allowed_attrs(self, recursive=True):
+        allowed = []
+        for key in ('actions', 'inline_actions', 'append', 'attach'):
+            allowed.extend(self.metadata[key])
+        allowed.extend([name for name in self.metadata['names'].keys() if name.startswith('get_')])
+        return allowed
 
     def source(self, name):
         self.metadata['source'] = name
         return self
 
     def reload(self, seconds=5, condition=None, max_requests=12):
         self.metadata['refresh'] = dict(seconds=seconds, condition=condition, retry=max_requests)
         return self
 
     def contextualize(self, request):
-        self.request = request
+        if request:
+            self.path = request.path
+            self.request = request
         return self
 
     def debug(self):
-        print(json.dumps(self.serialize(wrap=True, verbose=True), indent=4, ensure_ascii=False))
+        print(json.dumps(self.serialize(wrap=True), indent=4, ensure_ascii=False))
 
     def apply_role_lookups(self, user):
         return self
 
+    def action_form_cls(self, action):
+        return type(self.instance).action_form_cls(action)
+
     def has_permission(self, user):
         return user.is_superuser or self.instance.has_permission(user)
 
     def has_children(self):
         if type(self.instance):
             field_names = [field.name for field in self.instance.metaclass().fields]
             for name in self.metadata['names']:
@@ -153,21 +183,14 @@
                     return dict(seconds=refresh['seconds'], retry=refresh['retry'])
                 else:
                     return dict(seconds=refresh['seconds'], retry=0)
             else:
                 return dict(seconds=refresh['seconds'], retry=refresh['retry'])
         return {}
 
-    def get_path(self, attr_name):
-        if isinstance(self.instance, QuerySet):
-            metaclass = self.instance.model.metaclass()
-            return '/{}/{}/{}/'.format(metaclass.app_label,metaclass.model_name, attr_name)
-        metaclass = self.instance.metaclass()
-        return '/{}/{}/{}/{}/'.format(metaclass.app_label, metaclass.model_name,self.instance.pk, attr_name)
-
     def get_api_schema(self, recursive=False):
         schema = dict()
         for attr_name, width in self.metadata['names'].items():
             try:
                 attr, value = getattrr(self.instance, attr_name)
             except BaseException as e:
                 continue
@@ -179,115 +202,133 @@
                 schema[attr_name] = dict(type='object', properties=value.get_api_schema(recursive=True))
             else:
                 schema[attr_name] = self.instance.get_attr_api_type(attr_name)
         if recursive:
             return schema
         return dict(type='object', properties=schema)
 
-    def load(self, wrap=True, verbose=False, detail=False, deep=0):
-        only = []
+    def load(self, wrap=True, detail=False, deep=0):
         is_meta_api = False
         if self.request:
             is_meta_api = self.request.path.startswith('/meta/')
             if 'only' in self.request.GET:
-                only.extend(self.request.GET['only'].split(','))
+                self.metadata['names'] = {k: 100 for k in self.request.GET['only'].split(',') if hasattr(self.instance, k)}
                 self.request.GET._mutable = True
                 self.request.GET.pop('only')
                 self.request.GET._mutable = False
 
         if self.metadata['names']:
             for i, (attr_name, width) in enumerate(self.metadata['names'].items()):
-                if only and attr_name not in only:
-                    continue
                 if self.request and not self.request.user.is_superuser:
                     if self.metadata['only'] and attr_name in self.metadata['only']:
                         if not self.request.user.roles.contains(*self.metadata['only'][attr_name]):
                             continue
                 if self.request is None or self.instance.has_attr_permission(self.request.user, attr_name):
-                    lazy = wrap and (deep > 1 or (deep > 0 and i > 0))
+                    lazy = wrap and (deep > 1 or (deep > 0 and i > 0)) and self.metadata['template'] is None
                     attr, value = getattrr(self.instance, attr_name)
-                    path = self.get_path(attr_name)
+                    path = self.path
+                    if path and self.metadata['attr'] is None and attr_name != 'all':
+                        tokens = path.split('?')
+                        path = '{}{}/'.format(tokens[0], attr_name)
+                        if len(tokens) == 2:
+                            path = '{}?{}'.format(path, tokens[1])
+                    if self.request and self.request.META.get('QUERY_STRING') and 'only' not in self.request.META.get('QUERY_STRING'):
+                        path = '{}?{}'.format(path, self.request.META.get('QUERY_STRING').replace('?tab=1', ''))
                     if isinstance(value, QuerySet) or hasattr(value, '_queryset_class'):  # RelatedManager
                         qs = value if isinstance(value, QuerySet) else value.filter() # ManyRelatedManager
+                        qs.instantiator = self.instance
                         qs.metadata['uuid'] = attr_name
+                        qs.metadata['path'] = path
                         verbose_name = getattr(attr, '__verbose_name__', qs.metadata['verbose_name'] or pretty(attr_name))
-                        qs = qs.contextualize(self.request)
+                        template = getattr(attr, '__template__', None)
+                        template = 'renderers/{}.html'.format(template) if template else None
+                        if self.request:
+                            qs = qs.contextualize(self.request).apply_role_lookups(self.request.user)
                         if wrap:
-                            if self.metadata['primitive']:
-                                data = dict(value=serialize(qs), width=width, template=None, type='primitive', path=path)
+                            if template or (self.metadata['primitive'] and deep > 0):
+                                data = dict(value=serialize(qs), width=width, type='primitive', path=path, template=template)
                             else:
-                                data = qs.serialize(path=path, wrap=wrap, verbose=verbose, lazy=lazy)
-                            data.update(name=verbose_name if verbose else attr_name, key=attr_name)
+                                data = qs.serialize(path=path, wrap=wrap, lazy=lazy)
+                            data.update(name=verbose_name, key=attr_name)
                         else:
-                            if self.metadata['primitive']:  # one-to-many or many-to-many
-                                data = dict(value=serialize(qs), width=width, template=None, type='primitive', path=path)
+                            if self.metadata['primitive']:  # one-to-many or many-to-many (and deep > 0)
+                                data = dict(value=serialize(qs), width=width, type='primitive', path=path, template=template)
                             else:
                                 data = qs.to_list(detail=False)
                     elif isinstance(value, QuerySetStatistics):
                         statistics = value
                         verbose_name = getattr(attr, '__verbose_name__', statistics.metadata['verbose_name'] or pretty(attr_name))
                         statistics.contextualize(self.request)
                         data = statistics.serialize(path=path, wrap=wrap, lazy=lazy)
-                        data.update(name=verbose_name if verbose else attr_name, key=attr_name) if wrap else None
+                        data.update(name=verbose_name, key=attr_name) if wrap else None
                     elif isinstance(value, ValueSet):
                         valueset = value
                         verbose_name = getattr(attr, '__verbose_name__', valueset.metadata['verbose_name'] or pretty(attr_name))
                         valueset.contextualize(self.request)
                         key = attr_name
                         inner_deep = 0 if self.metadata['attr'] or (deep==1 and i==0) else deep+1
-                        valueset.load(wrap=wrap, verbose=verbose, detail=wrap and verbose or detail, deep=inner_deep)
+                        valueset.path = path
+                        valueset.load(wrap=wrap, detail=wrap or detail, deep=inner_deep)
                         if not valueset:
                             continue
                         refresh = valueset.refresh_data()
-                        data = dict(uuid=uuid1().hex, type='fieldset', name=verbose_name if verbose else attr_name,
-                            key=key, refresh=refresh, actions=[], data=valueset, path=path) if wrap else valueset
+                        collapsed = valueset.metadata['collapsed']
+                        data = dict(uuid=uuid1().hex, type='fieldset', name=verbose_name,
+                            key=key, refresh=refresh, actions=[], inline_actions=[], data=valueset, path=path, collapsed=collapsed
+                        ) if wrap else valueset
+                        if self.request and self.request.path.startswith('/app/'):
+                            data.update(instance=valueset.instance)
                         if wrap:
-                            for form_name in valueset.metadata['actions']:
-                                form_cls = self.instance.action_form_cls(form_name)
-                                if form_cls.check_fake_permission(self.request, self.instance, self.instance):
-                                    data['actions'].append(form_cls.get_metadata(path))
+                            for action_type in ('actions', 'inline_actions'):
+                                for form_name in valueset.metadata[action_type]:
+                                    form_cls = self.instance.action_form_cls(form_name)
+                                    if form_cls.check_fake_permission(self.request, self.instance, self.instance):
+                                        data[action_type].append(form_cls.get_metadata(path))
                             data.update(path=path)
                             if valueset.metadata['image']:
-                                image_attr = getattr(self.instance, valueset.metadata['image'])
-                                image = image_attr() if callable(image_attr) else image_attr
+                                image = valueset.metadata['image']
                                 if image:
                                     image = str(image)
                                     if not image.startswith('/') and not image.startswith('http'):
                                         image = '/media/{}'.format(image)
                                     data.update(image=image)
                             if valueset.metadata['template']:
                                 data.update(template='{}.html'.format(valueset.metadata['template']))
                     else:
+                        path = '{}{}/'.format(self.path, attr_name)
                         data = value
-                        verbose_name = None
+                        verbose_name = pretty(self.metadata['model'].get_attr_metadata(attr_name)[0])
                         self.metadata['primitive'] = True
                         if not wrap or is_meta_api:
                             data = serialize(data)
-                        if wrap and verbose or detail:
+                        if wrap or detail:
                             template = getattr(attr, '__template__', None)
                             metadata = getattr(attr, '__metadata__', None)
                             if template:
                                 template = 'renderers/{}.html'.format(template)
-                            data = dict(value=data, width=width, template=template, metadata=metadata, type='primitive', path=path)
-                    if verbose:
-                        attr_name = verbose_name or pretty(self.metadata['model'].get_attr_metadata(attr_name)[0])
+                            data = dict(key=attr_name, name=verbose_name, value=data, width=width, template=template, metadata=metadata, type='primitive', path=path)
+                    # if verbose:
+                    #     attr_name = verbose_name or pretty(self.metadata['model'].get_attr_metadata(attr_name)[0])
                     self[attr_name] = data
-        else:
+        elif isinstance(self.instance, Model):
             self['id'] = self.instance.id
             self[self.metadata['model'].__name__.lower()] = str(self.instance)
 
         return self
 
     def __str__(self):
         if self.request:
             return self.html()
         return json.dumps(self, indent=4, ensure_ascii=False)
 
-    def serialize(self, wrap=False, verbose=False):
-        self.load(wrap=wrap, verbose=verbose, detail=wrap and verbose)
+    def __repr__(self):
+        return 'Valueset <{}>'.format(self.instance)
+
+    def serialize(self, wrap=False):
+        self.load(wrap=wrap, detail=wrap)
         if wrap:
             check_fieldsets_type(self)
             # print(json.dumps(data, indent=4, ensure_ascii=False))
             if isinstance(self.instance, QuerySet):
                 name = self.instance.model.metaclass().verbose_name_plural
                 icon = getattr(self.instance.model.metaclass(), 'icon', None)
             elif isinstance(self.instance, Model):
@@ -295,89 +336,83 @@
                 icon = getattr(self.instance.metaclass(), 'icon', None)
             else:
                 name = ''
                 icon = None
             output = dict(
                 uuid=uuid1().hex, type='object', name=name
             )
+            if self.request and self.request.path.startswith('/app/'):
+                output.update(instance=self.instance)
             for key in ('title', 'subtitle', 'status'):
                 if self.metadata[key]:
                     value = getattr(self.instance, self.metadata[key])
-                    if self.metadata[key]:
-                        verbose_name, ordering, template, metadata = self.instance.get_attr_metadata(self.metadata[key])
-                    else:
-                        verbose_name, ordering, template, metadata = str(self.instance), None, None, {}
+                    value = value() if callable(value) else value
+                    verbose_name, ordering, template, metadata = self.instance.get_attr_metadata(self.metadata[key])
+                    if isinstance(value, QuerySet):
+                        value = [str(obj) for obj in value]
                     output[key] = dict(value=value, template=template, metadata=metadata)
 
-            output.update(icon=icon, data=self, actions=[], attach=[], append={})
-            for form_name in self.metadata['actions']:
-                form_cls = self.instance.action_form_cls(form_name)
-                if self.request is None or form_cls.check_fake_permission(
-                        request=self.request, instance=self.instance, instantiator=self.instance,
-                ):
-                    path = '/{}/{}/{}/'.format(
-                        self.instance.metaclass().app_label,
-                        self.instance.metaclass().model_name, self.instance.pk
-                    )
-                    output['actions'].append(form_cls.get_metadata(path))
+            output.update(icon=icon, data=self, actions=[], inline_actions=[], attach=[], append={})
+            for action_type in ('actions', 'inline_actions'):
+                for form_name in self.metadata[action_type]:
+                    form_cls = self.instance.action_form_cls(form_name)
+                    if self.request is None or form_cls.check_fake_permission(
+                            request=self.request, instance=self.instance, instantiator=self.instance,
+                    ):
+                        output[action_type].append(form_cls.get_metadata(self.path))
             for attr_name in self.metadata['attach']:
                 name = getattr(self.instance, attr_name)().metadata['verbose_name'] or pretty(attr_name)
-                path = '/{}/{}/{}/{}/'.format(
-                    self.instance.metaclass().app_label,
-                    self.instance.metaclass().model_name,
-                    self.instance.pk, attr_name
-                )
                 if self.request is None or self.instance.has_attr_permission(self.request.user, attr_name):
-                    output['attach'].append(dict(name=name, path=path))
+                    output['attach'].append(dict(name=name, path='{}{}/'.format(self.path, attr_name)))
             for attr_name in self.metadata['append']:
                 if self.request is None or self.instance.has_attr_permission(self.request.user, attr_name):
+                    template = getattr(getattr(self.instance, attr_name), '__template__', None)
                     output['append'].update(
-                        self.instance.values(attr_name).contextualize(
-                            self.request
-                        ).load(wrap=wrap, verbose=verbose)
+                        self.instance.value_set(attr_name).renderer(template).contextualize(self.request).load(wrap=wrap)
                     )
             return output
         else:
             if len(self.metadata['names']) == 1:
                 return self[list(self.metadata['names'].keys())[0]]
             return self
 
-    def html(self):
-        serialized = self.serialize(wrap=True, verbose=True)
+    def html(self, path=None, print=False):
+        self.path = path if path else self.path
+        serialized = self.serialize(wrap=True)
         if self.metadata['attr']:
             is_ajax = self.request.headers.get('x-requested-with') == 'XMLHttpRequest'
             is_modal = 'modal' in self.request.GET
             data = serialized['data'][next(iter(serialized['data']))]
             if data['type'] in ('fieldset-list', 'fieldset-group'):
                 data['name'] = serialized['name']
                 data['icon'] = serialized['icon']
             if data['type']=='fieldset':
                 if is_ajax and not is_modal:
-                    data['name'] = None
-                    template_name = 'app/valueset/fieldset.html'
+                    # if 'tab' in self.request.GET: data['name'] = None
+                    template_name = 'valueset/fieldset.html'
                 else:
-                    template_name, data = 'app/valueset/valueset.html', serialized
+                    template_name, data = 'valueset/valueset.html', serialized
             elif data['type']=='fieldset-list':
                 if self.metadata['source'] or is_modal:
-                    template_name = 'app/valueset/valueset.html'
+                    template_name = 'valueset/valueset.html'
                 else:
-                    template_name = 'app/valueset/fieldset-tab.html'
+                    template_name = 'valueset/fieldset-tab.html'
             elif data['type']=='queryset':
                 if self.metadata['source'] or is_modal:
-                    template_name, data = 'app/valueset/valueset.html', serialized
+                    template_name, data = 'valueset/valueset.html', serialized
                 else:
-                    data['name'] = None
-                    template_name = 'app/queryset/queryset.html'
+                    # if 'tab' in self.request.GET: data['name'] = None
+                    template_name = 'queryset/queryset.html'
             elif data['type']=='statistics':
                 if self.metadata['source'] or is_modal:
-                    template_name, data = 'app/valueset/valueset.html', serialized
+                    template_name, data = 'valueset/valueset.html', serialized
                 else:
-                    data['name'] = None
-                    template_name = 'app/statistics.html'
+                    # if 'tab' in self.request.GET: data['name'] = None
+                    template_name = 'queryset/statistics.html'
             elif data['type'] == 'primitive':
-                template_name = 'app/valueset/primitive.html'
+                template_name = 'valueset/primitive.html'
             else:
-                template_name = 'app/valueset/valueset.html'
+                template_name = 'valueset/valueset.html'
         else:
-            template_name, data = 'app/valueset/valueset.html', serialized
+            template_name, data = 'valueset/valueset.html', serialized
         # pprint.pprint(data)
-        return render_to_string(template_name, dict(data=data), request=self.request)
+        return render_to_string(template_name, dict(data=data, print=print), request=self.request)
```

### Comparing `django-sloth-0.0.54/sloth/db/models/__init__.py` & `django-sloth-0.1.0/sloth/db/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,41 +172,48 @@
         field.widget.formatted = self.formatted
         return field
 
 
 class ForeignKey(ForeignKey):
     def __init__(self, to, on_delete=CASCADE, **kwargs):
         self.picker = kwargs.pop('picker', None)
-        self.auto_user = kwargs.pop('auto_user', False)
+        self.username_lookup = kwargs.pop('username_lookup', None)
         super().__init__(to=to, on_delete=on_delete, **kwargs)
 
     def formfield(self, **kwargs):
         field = super().formfield(**kwargs)
         if self.picker:
             field.picker = self.picker
-        if self.auto_user:
-            field.auto_user = self.auto_user
+        if self.username_lookup:
+            field.username_lookup = self.username_lookup
         return field
 
 
 class CurrentUserField(ForeignKey):
     def __init__(self, *args, **kwargs):
         kwargs.update(to='auth.User')
         super().__init__(*args, **kwargs)
 
 
 class ManyToManyField(ManyToManyField):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, to, **kwargs):
+        if hasattr(to, 'model'):
+            self.queryset = to
+            to = to.model
+        else:
+            self.queryset = None
         self.picker = kwargs.pop('picker', None)
-        super().__init__(*args, **kwargs)
+        super().__init__(to, **kwargs)
 
     def formfield(self, **kwargs):
         field = super().formfield(**kwargs)
         if self.picker:
             field.picker = self.picker
+        if self.queryset:
+            field.queryset = self.queryset
         return field
 
 
 class OneToOneField(OneToOneField):
     def __init__(self, to, on_delete=SET_NULL, **kwargs):
         if kwargs.get('blank'):
             kwargs.update(null=True)
@@ -242,15 +249,23 @@
         super().__init__(*args, decimal_places=decimal_places, max_digits=max_digits, **kwargs)
 
 
 class Manager(QuerySet):
     pass
 
 
-class Model(models.Model, ModelMixin, metaclass=base.ModelBase):
+class ModelBase(base.ModelBase):
+    def __new__(mcs, name, bases, attrs):
+        cls = super().__new__(mcs, name, bases, attrs)
+        if cls.metaclass() and getattr(cls.metaclass(), 'autouser', False):
+            cls.add_to_class('autouser', models.ForeignKey('auth.user', verbose_name='Usuário', null=True, on_delete=models.CASCADE))
+        return cls
+
+
+class Model(models.Model, ModelMixin, metaclass=ModelBase):
 
     class Meta:
         abstract = True
 
     def pre_save(self, *args, **kwargs):
         setattr(self, '_pre_saved', True)
         if hasattr(self, '__roles__'):
@@ -282,8 +297,8 @@
         if hasattr(self, '__roles__') and hasattr(self, '_role_tuples'):
             self.sync_roles(getattr(self, '_role_tuples'))
 
     def __str__(self):
         for field in self.metaclass().fields:
             if isinstance(field, models.CharField):
                 return getattr(self, field.name)
-        return '{} #{}'.format(self.metaclass().verbose_name, self.pk)
+        return '{} #{}'.format(self.metaclass().verbose_name, self.pk)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-sloth-0.0.54/sloth/tasks/__init__.py` & `django-sloth-0.1.0/sloth/api/tasks/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import traceback
 import datetime
 from threading import Thread
 from django.core.cache import cache
-from ..api.models import Task as TaskModel
+from sloth.api.models import Task as TaskModel
 
 
 class Task(Thread):
 
     def __init__(self, *args, **kwargs):
         self.total = 0
         self.partial = 0
@@ -47,14 +47,17 @@
             self.total = len(iterable)
         for obj in iterable:
             if self.running():
                 yield obj
             else:
                 break
 
-    def finalize(self, text):
+    def message(self, text):
+        TaskModel.objects.filter(pk=self.task_id).update(message=text)
+
+    def finalize(self, text='Ação realizada com sucesso'):
         TaskModel.objects.filter(pk=self.task_id).update(message=text, end=datetime.datetime.now(), partial=self.partial)
 
     def error(self, text, exception=None):
         if exception:
             traceback.print_exc()
         TaskModel.objects.filter(pk=self.task_id).update(error=text, end=datetime.datetime.now(), partial=self.partial)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-sloth-0.0.54/sloth/test/__init__.py` & `django-sloth-0.1.0/sloth/test/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,63 +10,67 @@
 
 
 class ServerTestCase(StaticLiveServerTestCase):
 
     def __init__(self, *args, **kwargs):
         self.authorization = None
         self.debug = False
+        self.headers = {}
         super().__init__(*args, **kwargs)
 
-    def headers(self):
+    def get_headers(self, ):
         if self.authorization:
-            return {'Authorization': self.authorization}
+            headers = {'Authorization': self.authorization}
+            headers.update(self.headers)
+            return headers
         return None
 
     def log(self, method, url, data, response):
         if self.debug:
             print('{}: {}'.format(method, url))
             try:
                 if data:
                     print('Input:\n{}'.format(json.dumps(data, indent=4, ensure_ascii=False)))
                 print('Output:\n{}'.format(json.dumps(response.json(), indent=4, ensure_ascii=False)))
             except Exception:
+                print(response.text)
                 import traceback
                 print(traceback.format_exc())
                 print(data)
             print('\n')
 
     def url(self, path):
         if path.startswith('/o/'):
             return '{}{}'.format(self.live_server_url, path)
         return '{}{}'.format(self.live_server_url, path)
 
     def get(self, path, data=None, status_code=200):
         url = self.url(path)
-        response = requests.get(url, data=data, headers=self.headers())
+        response = requests.get(url, data=data, headers=self.get_headers())
         self.log('GET', url, data, response)
         self.assertEquals(response.status_code, status_code)
         return response.json()
 
     def post(self, path, data=None, status_code=200):
         url = self.url(path)
-        response = requests.post(url, data=data, headers=self.headers())
+        response = requests.post(url, data=data, headers=self.get_headers())
         self.log('POST', url, data, response)
         self.assertEquals(response.status_code, status_code)
         return response.json()
 
     def put(self, path, data=None, status_code=200):
         url = self.url(path)
-        response = requests.put(url, data=data, headers=self.headers())
+        response = requests.put(url, data=data, headers=self.get_headers())
         self.log('PUT', url, data, response)
         self.assertEquals(response.status_code, status_code)
         return response.json()
 
     def delete(self, path, data=None, status_code=200):
         url = self.url(path)
-        response = requests.delete(url, data=data, headers=self.headers())
+        response = requests.delete(url, data=data, headers=self.get_headers())
         self.log('DELETE', url, data, response)
         self.assertEquals(response.status_code, status_code)
         return response.json()
 
     def login(self, username, password):
         self.authorization = 'Basic {}'.format(
             base64.b64encode('{}:{}'.format(username, password).encode()).decode()
```

### Comparing `django-sloth-0.0.54/sloth/test/selenium/__init__.py` & `django-sloth-0.1.0/sloth/test/selenium/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         self.browser.click_tab(text)
 
     def click_icon(self, name):
         self.browser.click_icon(name)
 
     def login(self, username, password):
         self.current_username = username
-        self.open('/app/login/')
+        self.open('/app/dashboard/login/')
         self.enter('Login', username)
         self.enter('Senha', password)
         self.click_button('Acessar')
         self.wait()
 
     def logout(self):
         self.browser.logout()
```

### Comparing `django-sloth-0.0.54/sloth/test/selenium/browser.py` & `django-sloth-0.1.0/sloth/test/selenium/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,23 +150,22 @@
                     self.wait()
                     self.see(text, flag, count - 1)
                 else:
                     self.watch(e)
             if self.slowly:
                 self.wait(2)
 
-
     def see_message(self, text, count=4):
         self.print('See message {}'.format(text))
         try:
             self.execute_script("seeMessage('{}')".format(text))
         except WebDriverException as e:
             if count:
                 self.wait()
-                self.see_message(count - 1)
+                self.see_message(text, count - 1)
             else:
                 self.watch(e)
         if self.slowly:
             self.wait(2)
 
     def look_at_popup_window(self, count=4):
         self.print('Looking at popup window')
```

### Comparing `django-sloth-0.0.54/sloth/utils/__init__.py` & `django-sloth-0.1.0/sloth/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import re
 from django.conf import settings
 from decimal import Decimal
 from django.db.models.fields.files import FieldFile
 
 
 def to_snake_case(name):
-    return re.sub(r'(?<!^)(?=[A-Z])', '_', name).lower()
+    return name if name.islower() else re.sub(r'(?<!^)(?=[A-Z0-9])', '_', name).lower()
 
 
 def to_camel_case(name):
-    return  ''.join(word.title() for word in name.split('_'))
+    return ''.join(word.title() for word in name.split('_'))
 
 
 def getattrr(obj, args):
     if args == '__str__':
         attrs = [args]
     else:
         attrs = args.split('__')
```

### Comparing `django-sloth-0.0.54/sloth/utils/formatter/__init__.py` & `django-sloth-0.1.0/sloth/utils/formatter/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def format_value(obj):
     if obj not in (None, ''):
         if isinstance(obj, str):
             if obj[0] == '#' and len(obj) == 7:
                 style = 'float:left;width:20px;height: 20px; margin-right:5px;border-radius:5px'
                 return mark_safe('<div style="background-color:{};{}"></div>'.format(obj, style))
-            return obj
+            return mark_safe(obj)
         elif isinstance(obj, bool):
             return 'Sim' if obj else 'Não'
         elif isinstance(obj, datetime.datetime):
             return obj.strftime('%d/%m/%Y %H:%M')
         elif isinstance(obj, datetime.date):
             return obj.strftime('%d/%m/%Y')
         elif isinstance(obj, float):
@@ -34,15 +34,15 @@
             )
         elif isinstance(obj, dict):
             return mark_safe(
                 '<dl>{}</dl>'.format(''.join(['<dt>{}</dt><dd>{}</dd>'.format(k, format_value(v)) for k, v in obj.items()]))
             )
         elif isinstance(obj, FieldFile):
             return obj.url
-        return str(obj)
+        return mark_safe(str(obj))
     return '-'
 
 
 def format_decimal(value, decimal_places=2):
     str_format = '{{:,.{}f}}'.format(decimal_places)
     if value is not None:
         value = str_format.format(Decimal(value))
```

### Comparing `django-sloth-0.0.54/sloth/utils/http/__init__.py` & `django-sloth-0.1.0/sloth/utils/http/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,75 +2,24 @@
 import os
 import xlwt
 import csv
 import tempfile
 import datetime
 from tempfile import mktemp
 from django.conf import settings
-from django.http import HttpResponse
+from django.http import HttpResponse, JsonResponse
 from django.template.loader import render_to_string
 
 
-CONTENT_TYPES = {
-    'aac': 'audio/aac',
-    'abw': 'application/x-abiword',
-    'arc': 'application/octet-stream',
-    'avi': 'video/x-msvideo',
-    'bin': 'application/octet-stream',
-    'bz': 'application/x-bzip',
-    'bz2': 'application/x-bzip2',
-    'csh': 'application/x-csh',
-    'css': 'text/css',
-    'csv': 'text/csv',
-    'doc': 'application/msword',
-    'epub': 'application/epub+zip',
-    'gif': 'image/gif',
-    'htm': 'text/html',
-    'html': 'text/html',
-    'ico': 'image/x-icon',
-    'ics': 'text/calendar',
-    'jar': 'application/java-archive',
-    'jpeg': 'image/jpeg',
-    'jpg': 'image/jpeg',
-    'js': 'application/javascript',
-    'json': 'application/json',
-    'mid': 'audio/midi',
-    'midi': 'audio/midi',
-    'mpeg': 'video/mpeg',
-    'oga': 'audio/ogg',
-    'ogv': 'video/ogg',
-    'ogx': 'application/ogg',
-    'otf': 'font/otf',
-    'png': 'image/png',
-    'pdf': 'application/pdf',
-    'ppt': 'application/vnd.ms-powerpoint',
-    'rar': 'application/x-rar-compressed',
-    'rtf': 'application/rtf',
-    'sh': 'application/x-sh',
-    'svg': 'image/svg+xml',
-    'swf': 'application/x-shockwave-flash',
-    'tar': 'application/x-tar',
-    'tiff': 'image/tiff',
-    'ts': 'application/typescript',
-    'ttf': 'font/ttf',
-    'vsd': 'application/vnd.visio',
-    'wav': 'audio/x-wav',
-    'weba': 'audio/webm',
-    'webm': 'video/webm',
-    'webp': 'image/webp',
-    'woff': 'font/woff',
-    'woff2': 'font/woff2',
-    'xhtml': 'application/xhtml+xml',
-    'xls': 'application/vnd.ms-excel',
-    'xlsx': 'application/vnd.ms-excel',
-    'xml': 'application/xml',
-    'xul': 'application/vnd.mozilla.xul+xml',
-    'zip': 'application/zip',
-    '7z': 'application/x-7z-compressed'
-}
+class ApiResponse(JsonResponse):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self["Access-Control-Allow-Origin"] = "*"
+        self["Access-Control-Allow-Headers"] = "*"
+        self["X-Frame-Options"] = "SAMEORIGIN"
 
 
 class XlsResponse(HttpResponse):
     def __init__(self, data):
         wb = xlwt.Workbook(encoding='iso8859-1')
         for title, rows in data:
             sheet = wb.add_sheet(str(title))
@@ -88,48 +37,105 @@
 
 class CsvResponse(HttpResponse):
     def __init__(self, rows):
         path = mktemp()
         with open(path, 'w', encoding='iso8859-1') as output:
             writer = csv.writer(output)
             for row in rows:
-                writer.writerow([col.replace(' – ',  ' - ') for col in row])
+                writer.writerow([str(col).replace(' – ',  ' - ') for col in row])
         file = open(path, 'rb')
         content = file.read()
         file.close()
         super().__init__(content=content, content_type='application/csv')
         self['Content-Disposition'] = 'attachment; filename=Download.csv'
 
 
 class FileResponse(HttpResponse):
+    CONTENT_TYPES = {
+        'aac': 'audio/aac',
+        'abw': 'application/x-abiword',
+        'arc': 'application/octet-stream',
+        'avi': 'video/x-msvideo',
+        'bin': 'application/octet-stream',
+        'bz': 'application/x-bzip',
+        'bz2': 'application/x-bzip2',
+        'csh': 'application/x-csh',
+        'css': 'text/css',
+        'csv': 'text/csv',
+        'doc': 'application/msword',
+        'epub': 'application/epub+zip',
+        'gif': 'image/gif',
+        'htm': 'text/html',
+        'html': 'text/html',
+        'ico': 'image/x-icon',
+        'ics': 'text/calendar',
+        'jar': 'application/java-archive',
+        'jpeg': 'image/jpeg',
+        'jpg': 'image/jpeg',
+        'js': 'application/javascript',
+        'json': 'application/json',
+        'mid': 'audio/midi',
+        'midi': 'audio/midi',
+        'mpeg': 'video/mpeg',
+        'oga': 'audio/ogg',
+        'ogv': 'video/ogg',
+        'ogx': 'application/ogg',
+        'otf': 'font/otf',
+        'png': 'image/png',
+        'pdf': 'application/pdf',
+        'ppt': 'application/vnd.ms-powerpoint',
+        'rar': 'application/x-rar-compressed',
+        'rtf': 'application/rtf',
+        'sh': 'application/x-sh',
+        'svg': 'image/svg+xml',
+        'swf': 'application/x-shockwave-flash',
+        'tar': 'application/x-tar',
+        'tiff': 'image/tiff',
+        'ts': 'application/typescript',
+        'ttf': 'font/ttf',
+        'vsd': 'application/vnd.visio',
+        'wav': 'audio/x-wav',
+        'weba': 'audio/webm',
+        'webm': 'video/webm',
+        'webp': 'image/webp',
+        'woff': 'font/woff',
+        'woff2': 'font/woff2',
+        'xhtml': 'application/xhtml+xml',
+        'xls': 'application/vnd.ms-excel',
+        'xlsx': 'application/vnd.ms-excel',
+        'xml': 'application/xml',
+        'xul': 'application/vnd.mozilla.xul+xml',
+        'zip': 'application/zip',
+        '7z': 'application/x-7z-compressed'
+    }
 
     def __init__(self, file_path):
-        extension = file_path.split('.')[-1]
-        content_type = CONTENT_TYPES[extension]
+        file_name = file_path.split('/')[-1]
+        extension = file_name.split('.')[-1].lower()
+        content_type = FileResponse.CONTENT_TYPES[extension]
         with open(file_path, 'r+b') as file:
             content = file.read()
         super().__init__(content=content, content_type=content_type)
+        self['Content-Disposition'] = 'attachment; filename={}'.format(file_name)
 
 
 class HtmlToPdfResponse(HttpResponse):
 
     def __init__(self, html, landscape=False):
         import pdfkit
         file_name = tempfile.mktemp('.pdf')
         if landscape:
             html = html.replace('logo_if_portrait', 'logo_if_landscape')
             html = html.replace('content="Portrait"', 'content="Landscape"')
         html = html.replace('/media', settings.MEDIA_ROOT)
         html = html.replace('/static', '{}/{}/static'.format(settings.BASE_DIR, settings.BASE_DIR.name))
-        pdfkit.from_string(html, file_name)
+        pdfkit.from_string(html, file_name, options={"enable-local-file-access": ""})
         str_bytes = open(file_name, "rb").read()
         os.unlink(file_name)
         super().__init__(str_bytes, content_type='application/pdf')
 
 
 class PdfReportResponse(HtmlToPdfResponse):
-    def __init__(self, request, data, landscape=False, template='app/report.html'):
-        data.update(
-            today=datetime.date.today(), settings=settings
-        )
-        html = render_to_string([template], data, request=request)
+    def __init__(self, request, content, landscape=False, template='dashboard/report.html'):
+        context = dict(today=datetime.date.today(), title='Relatório', icon=None, content=content)
+        html = render_to_string([template], context, request=request)
         super().__init__(html, landscape=landscape)
```

### Comparing `django-sloth-0.0.54/sloth/utils/icons/bootstrap.py` & `django-sloth-0.1.0/sloth/utils/icons/bootstrap.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/utils/icons/fontawesome.py` & `django-sloth-0.1.0/sloth/utils/icons/fontawesome.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/utils/icons/materialicons.py` & `django-sloth-0.1.0/sloth/utils/icons/materialicons.py`

 * *Files identical despite different names*

### Comparing `django-sloth-0.0.54/sloth/utils/log/sql.py` & `django-sloth-0.1.0/sloth/utils/log/sql.py`

 * *Files identical despite different names*

