# Comparing `tmp/aa-srp-1.8.0.tar.gz` & `tmp/aa-srp-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-srp-1.8.0.tar", last modified: Tue Nov 30 07:48:17 2021, max compression
+gzip compressed data, was "aa-srp-1.9.0.tar", last modified: Sun Jan  2 20:40:57 2022, max compression
```

## Comparing `aa-srp-1.8.0.tar` & `aa-srp-1.9.0.tar`

### file list

```diff
@@ -1,161 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.587619 aa-srp-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     8827 2021-11-30 07:48:08.000000 aa-srp-1.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-11-30 07:48:08.000000 aa-srp-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      139 2021-11-30 07:48:08.000000 aa-srp-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10338 2021-11-30 07:48:17.587619 aa-srp-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7593 2021-11-30 07:48:08.000000 aa-srp-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.575619 aa-srp-1.8.0/aa_srp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10338 2021-11-30 07:48:17.000000 aa-srp-1.8.0/aa_srp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4498 2021-11-30 07:48:17.000000 aa-srp-1.8.0/aa_srp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-30 07:48:17.000000 aa-srp-1.8.0/aa_srp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-11-30 07:48:17.000000 aa-srp-1.8.0/aa_srp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-11-30 07:48:17.000000 aa-srp-1.8.0/aa_srp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.575619 aa-srp-1.8.0/aasrp/
--rw-r--r--   0 runner    (1001) docker     (121)      161 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2474 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      253 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     5822 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/form.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.579619 aa-srp-1.8.0/aasrp/helper/
--rw-r--r--   0 runner    (1001) docker     (121)     3283 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/helper/character.py
--rw-r--r--   0 runner    (1001) docker     (121)     1682 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/helper/eve_images.py
--rw-r--r--   0 runner    (1001) docker     (121)    14805 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/helper/icons.py
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/helper/notification.py
--rw-r--r--   0 runner    (1001) docker     (121)      976 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/helper/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.579619 aa-srp-1.8.0/aasrp/images/
--rw-r--r--   0 runner    (1001) docker     (121)   173017 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/images/aa-srp-dashboard-view-all.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   147341 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/images/aa-srp-dashboard.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   142292 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/images/aa-srp-request-details.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   314337 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/images/aa-srp-requests-overview.jpg
--rw-r--r--   0 runner    (1001) docker     (121)   333326 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/images/aa-srp-your-requests.jpg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.579619 aa-srp-1.8.0/aasrp/locale/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/locale/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.571619 aa-srp-1.8.0/aasrp/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.579619 aa-srp-1.8.0/aasrp/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     9444 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    16418 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.571619 aa-srp-1.8.0/aasrp/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.579619 aa-srp-1.8.0/aasrp/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    13056 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.571619 aa-srp-1.8.0/aasrp/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.579619 aa-srp-1.8.0/aasrp/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    13056 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.571619 aa-srp-1.8.0/aasrp/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.579619 aa-srp-1.8.0/aasrp/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    13049 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.571619 aa-srp-1.8.0/aasrp/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.579619 aa-srp-1.8.0/aasrp/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    13200 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.571619 aa-srp-1.8.0/aasrp/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.579619 aa-srp-1.8.0/aasrp/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    13049 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.571619 aa-srp-1.8.0/aasrp/management/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.579619 aa-srp-1.8.0/aasrp/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      688 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/management/commands/aasrp_load_eve.py
--rw-r--r--   0 runner    (1001) docker     (121)    10395 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/management/commands/aasrp_migrate_srp_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     4330 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/management/commands/aasrp_migrate_to_comments.py
--rw-r--r--   0 runner    (1001) docker     (121)     2234 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/management/commands/aasrp_update_db_relations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.583619 aa-srp-1.8.0/aasrp/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     7592 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     2936 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/migrations/0002_relations_update.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/migrations/0003_aasrprequest_reject_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/migrations/0004_aasrpusersettings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/migrations/0005_insurance.py
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/migrations/0006_related_names.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8061 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/providers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.575619 aa-srp-1.8.0/aasrp/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.575619 aa-srp-1.8.0/aasrp/static/aasrp/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.583619 aa-srp-1.8.0/aasrp/static/aasrp/css/
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/css/aa-bootstrap-fix.css
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/css/aa-bootstrap-fix.min.css
--rw-r--r--   0 runner    (1001) docker     (121)      229 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/css/aa-srp-form.css
--rw-r--r--   0 runner    (1001) docker     (121)      153 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/css/aa-srp-form.min.css
--rw-r--r--   0 runner    (1001) docker     (121)     2681 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/css/aa-srp.css
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/css/aa-srp.min.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.583619 aa-srp-1.8.0/aasrp/static/aasrp/javascript/
--rw-r--r--   0 runner    (1001) docker     (121)    11901 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/javascript/aa-srp-dashboard.js
--rw-r--r--   0 runner    (1001) docker     (121)     6058 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js
--rw-r--r--   0 runner    (1001) docker     (121)    19962 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/javascript/aa-srp-view-requests.js
--rw-r--r--   0 runner    (1001) docker     (121)    10039 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.575619 aa-srp-1.8.0/aasrp/static/aasrp/libs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.575619 aa-srp-1.8.0/aasrp/static/aasrp/libs/datatables/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.583619 aa-srp-1.8.0/aasrp/static/aasrp/libs/datatables/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)     5573 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/libs/datatables/plugins/dataTables.rowGroup.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     3250 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/libs/datatables/plugins/datetime.js
--rw-r--r--   0 runner    (1001) docker     (121)      746 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/libs/datatables/plugins/datetime.min.js
--rw-r--r--   0 runner    (1001) docker     (121)      384 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/libs/datatables/plugins/rowGroup.bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (121)      384 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/libs/datatables/plugins/rowGroup.dataTables.min.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.575619 aa-srp-1.8.0/aasrp/static/aasrp/libs/x-editable/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.575619 aa-srp-1.8.0/aasrp/static/aasrp/libs/x-editable/1.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.575619 aa-srp-1.8.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.583619 aa-srp-1.8.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/css/
--rw-r--r--   0 runner    (1001) docker     (121)    21137 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/css/bootstrap-editable.css
--rw-r--r--   0 runner    (1001) docker     (121)    17698 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/css/bootstrap-editable.min.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.583619 aa-srp-1.8.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/img/
--rw-r--r--   0 runner    (1001) docker     (121)      509 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/img/clear.png
--rw-r--r--   0 runner    (1001) docker     (121)     1849 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/img/loading.gif
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.583619 aa-srp-1.8.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/js/
--rw-r--r--   0 runner    (1001) docker     (121)   223714 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/js/bootstrap-editable.js
--rw-r--r--   0 runner    (1001) docker     (121)    89450 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/js/bootstrap-editable.min.js
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.575619 aa-srp-1.8.0/aasrp/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.583619 aa-srp-1.8.0/aasrp/templates/aasrp/
--rw-r--r--   0 runner    (1001) docker     (121)      401 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.583619 aa-srp-1.8.0/aasrp/templates/aasrp/bundles/
--rw-r--r--   0 runner    (1001) docker     (121)      320 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/bundles/bootstrap3-editable-css.html
--rw-r--r--   0 runner    (1001) docker     (121)      368 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/bundles/bootstrap3-editable-js.html
--rw-r--r--   0 runner    (1001) docker     (121)     4325 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/link_add.html
--rw-r--r--   0 runner    (1001) docker     (121)      910 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/link_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.575619 aa-srp-1.8.0/aasrp/templates/aasrp/modals/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.583619 aa-srp-1.8.0/aasrp/templates/aasrp/modals/dashboard/
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/modals/dashboard/delete_srp_link.html
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/modals/dashboard/disable_srp_link.html
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/modals/dashboard/enable_srp_link.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.587619 aa-srp-1.8.0/aasrp/templates/aasrp/modals/view_requests/
--rw-r--r--   0 runner    (1001) docker     (121)      975 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/modals/view_requests/accept_request.html
--rw-r--r--   0 runner    (1001) docker     (121)     2209 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/modals/view_requests/mark_complete_modal.html
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/modals/view_requests/reject_request.html
--rw-r--r--   0 runner    (1001) docker     (121)      975 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/modals/view_requests/remove_request.html
--rw-r--r--   0 runner    (1001) docker     (121)      832 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/modals/view_requests/request_details.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.575619 aa-srp-1.8.0/aasrp/templates/aasrp/partials/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.587619 aa-srp-1.8.0/aasrp/templates/aasrp/partials/dashboard/
--rw-r--r--   0 runner    (1001) docker     (121)      445 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/partials/dashboard/buttons.html
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/partials/dashboard/srp_links.html
--rw-r--r--   0 runner    (1001) docker     (121)      949 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/partials/dashboard/table.html
--rw-r--r--   0 runner    (1001) docker     (121)      897 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/partials/dashboard/user_settings.html
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/partials/dashboard/user_srp_requests.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.587619 aa-srp-1.8.0/aasrp/templates/aasrp/partials/form/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/partials/form/required_field_hint.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.587619 aa-srp-1.8.0/aasrp/templates/aasrp/partials/header/
--rw-r--r--   0 runner    (1001) docker     (121)      202 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/partials/header/h1.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.587619 aa-srp-1.8.0/aasrp/templates/aasrp/partials/link_add/
--rw-r--r--   0 runner    (1001) docker     (121)      779 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/partials/link_add/form.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.587619 aa-srp-1.8.0/aasrp/templates/aasrp/partials/link_edit/
--rw-r--r--   0 runner    (1001) docker     (121)      719 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/partials/link_edit/form.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.587619 aa-srp-1.8.0/aasrp/templates/aasrp/partials/request_srp/
--rw-r--r--   0 runner    (1001) docker     (121)      808 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/partials/request_srp/form.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.587619 aa-srp-1.8.0/aasrp/templates/aasrp/partials/view_requests/
--rw-r--r--   0 runner    (1001) docker     (121)     3151 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/partials/view_requests/overview.html
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/partials/view_requests/requests.html
--rw-r--r--   0 runner    (1001) docker     (121)      767 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/request_srp.html
--rw-r--r--   0 runner    (1001) docker     (121)     4320 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templates/aasrp/view_requests.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.587619 aa-srp-1.8.0/aasrp/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/templatetags/aasrp_versioned_static.py
--rw-r--r--   0 runner    (1001) docker     (121)     2909 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     2783 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    41163 2021-11-30 07:48:08.000000 aa-srp-1.8.0/aasrp/views.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-30 07:48:17.587619 aa-srp-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2428 2021-11-30 07:48:08.000000 aa-srp-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 07:48:17.587619 aa-srp-1.8.0/testauth/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-11-30 07:48:08.000000 aa-srp-1.8.0/testauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2021-11-30 07:48:08.000000 aa-srp-1.8.0/testauth/celery.py
--rw-r--r--   0 runner    (1001) docker     (121)     9385 2021-11-30 07:48:08.000000 aa-srp-1.8.0/testauth/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2021-11-30 07:48:08.000000 aa-srp-1.8.0/testauth/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2021-11-30 07:48:08.000000 aa-srp-1.8.0/testauth/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.503625 aa-srp-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     9066 2022-01-02 20:40:49.000000 aa-srp-1.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-01-02 20:40:49.000000 aa-srp-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-01-02 20:40:49.000000 aa-srp-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    10389 2022-01-02 20:40:57.503625 aa-srp-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7593 2022-01-02 20:40:49.000000 aa-srp-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aa_srp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10389 2022-01-02 20:40:57.000000 aa-srp-1.9.0/aa_srp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4462 2022-01-02 20:40:57.000000 aa-srp-1.9.0/aa_srp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-02 20:40:57.000000 aa-srp-1.9.0/aa_srp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-01-02 20:40:57.000000 aa-srp-1.9.0/aa_srp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-02 20:40:57.000000 aa-srp-1.9.0/aa_srp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.495624 aa-srp-1.9.0/aasrp/
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      793 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1456 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5859 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/form.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.495624 aa-srp-1.9.0/aasrp/helper/
+-rw-r--r--   0 runner    (1001) docker     (121)     2746 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/helper/character.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/helper/eve_images.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13218 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/helper/icons.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/helper/notification.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.495624 aa-srp-1.9.0/aasrp/images/
+-rw-r--r--   0 runner    (1001) docker     (121)   173017 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/images/aa-srp-dashboard-view-all.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)   147341 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/images/aa-srp-dashboard.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)   142292 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/images/aa-srp-request-details.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)   314337 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/images/aa-srp-requests-overview.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)   333326 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/images/aa-srp-your-requests.jpg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.495624 aa-srp-1.9.0/aasrp/locale/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/locale/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aasrp/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.495624 aa-srp-1.9.0/aasrp/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)     9444 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    16418 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aasrp/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.495624 aa-srp-1.9.0/aasrp/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    13056 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aasrp/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.495624 aa-srp-1.9.0/aasrp/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    13056 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aasrp/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.495624 aa-srp-1.9.0/aasrp/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    13049 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aasrp/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.495624 aa-srp-1.9.0/aasrp/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    13200 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aasrp/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.495624 aa-srp-1.9.0/aasrp/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    13049 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aasrp/management/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.499624 aa-srp-1.9.0/aasrp/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/management/commands/aasrp_load_eve.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9884 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/management/commands/aasrp_migrate_srp_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4152 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/management/commands/aasrp_migrate_to_comments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2176 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/management/commands/aasrp_update_db_relations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3206 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.499624 aa-srp-1.9.0/aasrp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     7610 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2954 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/migrations/0002_relations_update.py
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/migrations/0003_aasrprequest_reject_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1459 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/migrations/0004_aasrpusersettings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/migrations/0005_insurance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1435 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/migrations/0006_related_names.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8131 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/providers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aasrp/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aasrp/static/aasrp/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.499624 aa-srp-1.9.0/aasrp/static/aasrp/css/
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/css/aa-bootstrap-fix.css
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/css/aa-bootstrap-fix.min.css
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/css/aa-srp-form.css
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/css/aa-srp-form.min.css
+-rw-r--r--   0 runner    (1001) docker     (121)     2681 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/css/aa-srp.css
+-rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/css/aa-srp.min.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.499624 aa-srp-1.9.0/aasrp/static/aasrp/javascript/
+-rw-r--r--   0 runner    (1001) docker     (121)    11901 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/javascript/aa-srp-dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (121)     6058 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)    19962 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/javascript/aa-srp-view-requests.js
+-rw-r--r--   0 runner    (1001) docker     (121)    10039 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aasrp/static/aasrp/libs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aasrp/static/aasrp/libs/datatables/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.499624 aa-srp-1.9.0/aasrp/static/aasrp/libs/datatables/plugins/
+-rw-r--r--   0 runner    (1001) docker     (121)     5573 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/libs/datatables/plugins/dataTables.rowGroup.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3250 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/libs/datatables/plugins/datetime.js
+-rw-r--r--   0 runner    (1001) docker     (121)      746 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/libs/datatables/plugins/datetime.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/libs/datatables/plugins/rowGroup.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/libs/datatables/plugins/rowGroup.dataTables.min.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aasrp/static/aasrp/libs/x-editable/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aasrp/static/aasrp/libs/x-editable/1.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.499624 aa-srp-1.9.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/css/
+-rw-r--r--   0 runner    (1001) docker     (121)    21137 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/css/bootstrap-editable.css
+-rw-r--r--   0 runner    (1001) docker     (121)    17698 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/css/bootstrap-editable.min.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.499624 aa-srp-1.9.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/img/
+-rw-r--r--   0 runner    (1001) docker     (121)      509 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/img/clear.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1849 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/img/loading.gif
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.499624 aa-srp-1.9.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/js/
+-rw-r--r--   0 runner    (1001) docker     (121)   223714 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/js/bootstrap-editable.js
+-rw-r--r--   0 runner    (1001) docker     (121)    89450 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/js/bootstrap-editable.min.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aasrp/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.499624 aa-srp-1.9.0/aasrp/templates/aasrp/
+-rw-r--r--   0 runner    (1001) docker     (121)      401 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.499624 aa-srp-1.9.0/aasrp/templates/aasrp/bundles/
+-rw-r--r--   0 runner    (1001) docker     (121)      320 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/bundles/bootstrap3-editable-css.html
+-rw-r--r--   0 runner    (1001) docker     (121)      368 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/bundles/bootstrap3-editable-js.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4325 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1405 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/link_add.html
+-rw-r--r--   0 runner    (1001) docker     (121)      910 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/link_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aasrp/templates/aasrp/modals/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.503625 aa-srp-1.9.0/aasrp/templates/aasrp/modals/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/modals/dashboard/delete_srp_link.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/modals/dashboard/disable_srp_link.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/modals/dashboard/enable_srp_link.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.503625 aa-srp-1.9.0/aasrp/templates/aasrp/modals/view_requests/
+-rw-r--r--   0 runner    (1001) docker     (121)      975 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/modals/view_requests/accept_request.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2209 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/modals/view_requests/mark_complete_modal.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/modals/view_requests/reject_request.html
+-rw-r--r--   0 runner    (1001) docker     (121)      975 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/modals/view_requests/remove_request.html
+-rw-r--r--   0 runner    (1001) docker     (121)      832 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/modals/view_requests/request_details.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.491624 aa-srp-1.9.0/aasrp/templates/aasrp/partials/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.503625 aa-srp-1.9.0/aasrp/templates/aasrp/partials/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/partials/dashboard/buttons.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/partials/dashboard/srp_links.html
+-rw-r--r--   0 runner    (1001) docker     (121)      949 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/partials/dashboard/table.html
+-rw-r--r--   0 runner    (1001) docker     (121)      897 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/partials/dashboard/user_settings.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/partials/dashboard/user_srp_requests.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.503625 aa-srp-1.9.0/aasrp/templates/aasrp/partials/form/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/partials/form/required_field_hint.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.503625 aa-srp-1.9.0/aasrp/templates/aasrp/partials/header/
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/partials/header/h1.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.503625 aa-srp-1.9.0/aasrp/templates/aasrp/partials/link_add/
+-rw-r--r--   0 runner    (1001) docker     (121)      779 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/partials/link_add/form.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.503625 aa-srp-1.9.0/aasrp/templates/aasrp/partials/link_edit/
+-rw-r--r--   0 runner    (1001) docker     (121)      719 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/partials/link_edit/form.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.503625 aa-srp-1.9.0/aasrp/templates/aasrp/partials/request_srp/
+-rw-r--r--   0 runner    (1001) docker     (121)      808 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/partials/request_srp/form.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.503625 aa-srp-1.9.0/aasrp/templates/aasrp/partials/view_requests/
+-rw-r--r--   0 runner    (1001) docker     (121)     3151 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/partials/view_requests/overview.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/partials/view_requests/requests.html
+-rw-r--r--   0 runner    (1001) docker     (121)      767 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/request_srp.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4320 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templates/aasrp/view_requests.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.503625 aa-srp-1.9.0/aasrp/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/templatetags/aasrp_versioned_static.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2927 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2446 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40220 2022-01-02 20:40:49.000000 aa-srp-1.9.0/aasrp/views.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-02 20:40:57.503625 aa-srp-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-01-02 20:40:49.000000 aa-srp-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-02 20:40:57.503625 aa-srp-1.9.0/testauth/
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-01-02 20:40:49.000000 aa-srp-1.9.0/testauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2022-01-02 20:40:49.000000 aa-srp-1.9.0/testauth/celery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9427 2022-01-02 20:40:49.000000 aa-srp-1.9.0/testauth/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-01-02 20:40:49.000000 aa-srp-1.9.0/testauth/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2022-01-02 20:40:49.000000 aa-srp-1.9.0/testauth/wsgi.py
```

### Comparing `aa-srp-1.8.0/CHANGELOG.md` & `aa-srp-1.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,29 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/)
 
 
+## [1.9.0] - 2022-01-02
+
+### Added
+
+- Workaround for possible bug in AA-Discordbot (#41)
+
+### Changed
+
+- General code cleanup and modernisation
+- Switched to Alliance Auth App Utils for some helper functions
+
+### Removed
+
+- Non used code
+
 ## [1.8.0] - 2021-11-30
 
 ### Changed
 
 - Minimum requirements
   - Python 3.7
   - Alliance Auth v2.9.3
```

### Comparing `aa-srp-1.8.0/LICENSE` & `aa-srp-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/PKG-INFO` & `aa-srp-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: aa-srp
-Version: 1.8.0
+Version: 1.9.0
 Summary: Improved SRP Module for Alliance Auth
 Home-page: https://github.com/ppfeufer/aa-srp
 Author: Peter Pfeufer
 Author-email: development@ppfeufer.de
 License: GPLv3
 Project-URL: Issue / Bug Reports, https://github.com/ppfeufer/aa-srp/issues
 Project-URL: Changelog, https://github.com/ppfeufer/aa-srp/blob/master/CHANGELOG.md
-Project-URL: Release Notes, https://github.com/ppfeufer/aa-srp/releases/tag/v1.8.0
+Project-URL: Release Notes, https://github.com/ppfeufer/aa-srp/releases/tag/v1.9.0
 Project-URL: Git Repository, https://github.com/ppfeufer/aa-srp
 Description: # AA-SRP
         
         [![Version](https://img.shields.io/pypi/v/aa-srp?label=release)](https://pypi.org/project/aa-srp/)
         [![License](https://img.shields.io/github/license/ppfeufer/aa-srp)](https://github.com/ppfeufer/aa-srp/blob/master/LICENSE)
         [![Python](https://img.shields.io/pypi/pyversions/aa-srp)](https://pypi.org/project/aa-srp/)
         [![Django](https://img.shields.io/pypi/djversions/aa-srp?label=django)](https://pypi.org/project/aa-srp/)
@@ -201,11 +201,12 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```

### Comparing `aa-srp-1.8.0/README.md` & `aa-srp-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aa_srp.egg-info/PKG-INFO` & `aa-srp-1.9.0/aa_srp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: aa-srp
-Version: 1.8.0
+Version: 1.9.0
 Summary: Improved SRP Module for Alliance Auth
 Home-page: https://github.com/ppfeufer/aa-srp
 Author: Peter Pfeufer
 Author-email: development@ppfeufer.de
 License: GPLv3
 Project-URL: Issue / Bug Reports, https://github.com/ppfeufer/aa-srp/issues
 Project-URL: Changelog, https://github.com/ppfeufer/aa-srp/blob/master/CHANGELOG.md
-Project-URL: Release Notes, https://github.com/ppfeufer/aa-srp/releases/tag/v1.8.0
+Project-URL: Release Notes, https://github.com/ppfeufer/aa-srp/releases/tag/v1.9.0
 Project-URL: Git Repository, https://github.com/ppfeufer/aa-srp
 Description: # AA-SRP
         
         [![Version](https://img.shields.io/pypi/v/aa-srp?label=release)](https://pypi.org/project/aa-srp/)
         [![License](https://img.shields.io/github/license/ppfeufer/aa-srp)](https://github.com/ppfeufer/aa-srp/blob/master/LICENSE)
         [![Python](https://img.shields.io/pypi/pyversions/aa-srp)](https://pypi.org/project/aa-srp/)
         [![Django](https://img.shields.io/pypi/djversions/aa-srp?label=django)](https://pypi.org/project/aa-srp/)
@@ -201,11 +201,12 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
```

### Comparing `aa-srp-1.8.0/aa_srp.egg-info/SOURCES.txt` & `aa-srp-1.9.0/aa_srp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,21 @@
 aasrp/apps.py
 aasrp/auth_hooks.py
 aasrp/constants.py
 aasrp/form.py
 aasrp/managers.py
 aasrp/models.py
 aasrp/providers.py
-aasrp/tasks.py
 aasrp/urls.py
 aasrp/utils.py
 aasrp/views.py
 aasrp/helper/character.py
 aasrp/helper/eve_images.py
 aasrp/helper/icons.py
 aasrp/helper/notification.py
-aasrp/helper/urls.py
 aasrp/images/aa-srp-dashboard-view-all.jpg
 aasrp/images/aa-srp-dashboard.jpg
 aasrp/images/aa-srp-request-details.jpg
 aasrp/images/aa-srp-requests-overview.jpg
 aasrp/images/aa-srp-your-requests.jpg
 aasrp/locale/.gitkeep
 aasrp/locale/de/LC_MESSAGES/django.mo
```

### Comparing `aa-srp-1.8.0/aasrp/admin.py` & `aa-srp-1.9.0/aasrp/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Django admin declarations
 """
 
+# Django
 from django.contrib import admin
 
+# AA SRP
 from aasrp.models import AaSrpLink, AaSrpRequest, AaSrpRequestComment
 
 
 def custom_filter(title):
     """
     custom filter for model properties
     :param title:
```

### Comparing `aa-srp-1.8.0/aasrp/auth_hooks.py` & `aa-srp-1.9.0/aasrp/auth_hooks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
 hook into AA
 """
 
+# Django
 from django.utils.translation import ugettext_lazy as _
 
+# Alliance Auth
 from allianceauth import hooks
 from allianceauth.services.hooks import MenuItemHook, UrlHook
 
+# AA SRP
 from aasrp import __title__, urls
 from aasrp.managers import AaSrpManager
 
 
 class AaSrpMenuItem(MenuItemHook):  # pylint: disable=too-few-public-methods
     """
     This class ensures only authorized users will see the menu entry
```

### Comparing `aa-srp-1.8.0/aasrp/form.py` & `aa-srp-1.9.0/aasrp/form.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Form definitions
 """
 
+# Standard Library
 import re
 
+# Django
 from django import forms
 from django.forms import ModelForm
 from django.utils.safestring import mark_safe
 from django.utils.translation import ugettext_lazy as _
 
+# AA SRP
 from aasrp.constants import (
     EVETOOLS_KILLBOARD_BASE_URL,
     EVETOOLS_KILLBOARD_BASE_URL_REGEX,
     EVETOOLS_KILLBOARD_KILLMAIL_URL_REGEX,
     ZKILLBOARD_BASE_URL,
     ZKILLBOARD_BASE_URL_REGEX,
     ZKILLBOARD_KILLMAIL_URL_REGEX,
```

### Comparing `aa-srp-1.8.0/aasrp/helper/eve_images.py` & `aa-srp-1.9.0/aasrp/helper/eve_images.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 """
 eve images
 """
 
+# Alliance Auth
 from allianceauth.eveonline.evelinks.eveimageserver import (
     character_portrait_url,
     type_render_url,
 )
 from allianceauth.eveonline.models import EveCharacter
 
 
 def get_character_portrait_from_evecharacter(
     character: EveCharacter, size: int = 32, as_html: bool = False
 ) -> str:
     """
     get the character portrait from EveCharacter model
     :param size:
     :param character:
-    :param portrait_size:
+    :param size:
     :param as_html:
     :return:
     """
+
     portrait_url = character_portrait_url(
         character_id=character.character_id, size=size
     )
+    character_name = character.character_name
 
     return_value = portrait_url
 
     if as_html is True:
         return_value = (
-            '<img class="aasrp-character-portrait img-rounded" '
-            'src="{portrait_url}" alt="{character_name}">'.format(
-                portrait_url=portrait_url, character_name=character.character_name
-            )
+            f'<img class="aasrp-character-portrait img-rounded" '
+            f'src="{portrait_url}" alt="{character_name}">'
         )
 
     return return_value
 
 
 def get_type_render_url_from_type_id(
     evetype_id: int, size: int = 32, evetype_name: str = None, as_html: bool = False
@@ -44,24 +45,23 @@
     get type render from evetype_id
     :param evetype_id:
     :param size:
     :param evetype_name:
     :param as_html:
     :return:
     """
+
     render_url = type_render_url(type_id=evetype_id, size=size)
 
     return_value = render_url
 
     if as_html is True:
         alt_tag = ""
         if evetype_name is not None:
             alt_tag = f' alt="{evetype_name}"'
 
         return_value = (
-            '<img class="aasrp-evetype-icon img-rounded" '
-            'src="{render_url}"{alt_tag}>'.format(
-                render_url=render_url, alt_tag=alt_tag
-            )
+            f'<img class="aasrp-evetype-icon img-rounded" '
+            f'src="{render_url}"{alt_tag}>'
         )
 
     return return_value
```

### Comparing `aa-srp-1.8.0/aasrp/helper/icons.py` & `aa-srp-1.9.0/aasrp/helper/icons.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 some helper functions
 so we don't mess up other files too much
 """
 
+# Django
 from django.contrib.auth.decorators import login_required, permission_required
 from django.core.handlers.wsgi import WSGIRequest
 from django.urls import reverse
 from django.utils.translation import gettext_lazy as _
 
+# AA SRP
 from aasrp.models import AaSrpLink, AaSrpRequest, AaSrpRequestStatus, AaSrpStatus
 
 
 @login_required
 @permission_required(
     "aasrp.basic_access", "aasrp.manage_srp_requests", "aasrp.manage_srp"
 )
@@ -22,116 +24,98 @@
     :param srp_link:
     """
 
     actions = ""
 
     if srp_link.srp_status == AaSrpStatus.ACTIVE:
         button_request_url = reverse("aasrp:request_srp", args=[srp_link.srp_code])
+        btn_icon = '<i class="fas fa-hand-holding-usd"></i>'
+        btn_title = _("Request SRP")
         actions += (
-            '<a href="{btn_link}" '
-            'class="btn btn-success btn-sm btn-icon-aasrp" '
-            'title="{btn_title}">{btn_icon}</a>'.format(
-                btn_link=button_request_url,
-                btn_icon='<i class="fas fa-hand-holding-usd"></i>',
-                btn_title=_("Request SRP"),
-            )
+            f'<a href="{button_request_url}" '
+            f'class="btn btn-success btn-sm btn-icon-aasrp" '
+            f'title="{btn_title}">{btn_icon}</a>'
         )
 
     if request.user.has_perm("aasrp.manage_srp") or request.user.has_perm(
         "aasrp.manage_srp_requests"
     ):
         button_view_url = reverse("aasrp:view_srp_requests", args=[srp_link.srp_code])
+        btn_icon = '<i class="fas fa-eye"></i>'
+        btn_title = _("View SRP Requests")
         actions += (
-            '<a href="{btn_link}" '
-            'class="btn btn-primary btn-sm btn-icon-aasrp" '
-            'title="{btn_title}">{btn_icon}</a><br>'.format(
-                btn_link=button_view_url,
-                btn_icon='<i class="fas fa-eye"></i>',
-                btn_title=_("View SRP Requests"),
-            )
+            f'<a href="{button_view_url}" '
+            f'class="btn btn-primary btn-sm btn-icon-aasrp" '
+            f'title="{btn_title}">{btn_icon}</a><br>'
         )
 
         if srp_link.srp_status != AaSrpStatus.COMPLETED:
             if request.user.has_perm("aasrp.manage_srp"):
                 if srp_link.srp_status == AaSrpStatus.ACTIVE:
                     button_edit_url = reverse(
                         "aasrp:edit_srp_link", args=[srp_link.srp_code]
                     )
+                    btn_icon = '<i class="far fa-newspaper"></i>'
+                    btn_title = _("Add/Edit AAR Link")
                     actions += (
-                        '<a href="{btn_link}" '
-                        'class="btn btn-info btn-sm btn-icon-aasrp" '
-                        'title="{btn_title}">{btn_icon}</a>'.format(
-                            btn_link=button_edit_url,
-                            btn_icon='<i class="far fa-newspaper"></i>',
-                            btn_title=_("Add/Edit AAR Link"),
-                        )
+                        f'<a href="{button_edit_url}" '
+                        f'class="btn btn-info btn-sm btn-icon-aasrp" '
+                        f'title="{btn_title}">{btn_icon}</a>'
                     )
 
                     button_disable_url = reverse(
                         "aasrp:disable_srp_link", args=[srp_link.srp_code]
                     )
-
+                    btn_icon = '<i class="fas fa-ban"></i>'
+                    btn_title = _("Disable SRP Link")
+                    modal_id = "disable-srp-link"
                     data_name = srp_link.srp_name + " (" + srp_link.srp_code + ")"
 
                     actions += (
-                        '<a class="btn btn-warning btn-sm btn-icon-aasrp" '
-                        'title="{btn_title}" '
-                        'data-toggle="modal" '
-                        'data-target="#{modal_id}" '
-                        'data-url="{data_url}" '
-                        'data-name="{data_name}">{btn_icon}</a>'.format(
-                            data_url=button_disable_url,
-                            data_name=data_name,
-                            btn_icon='<i class="fas fa-ban"></i>',
-                            btn_title=_("Disable SRP Link"),
-                            modal_id="disable-srp-link",
-                        )
+                        f'<a class="btn btn-warning btn-sm btn-icon-aasrp" '
+                        f'title="{btn_title}" '
+                        f'data-toggle="modal" '
+                        f'data-target="#{modal_id}" '
+                        f'data-url="{button_disable_url}" '
+                        f'data-name="{data_name}">{btn_icon}</a>'
                     )
 
                 if srp_link.srp_status == AaSrpStatus.CLOSED:
                     button_enable_url = reverse(
                         "aasrp:enable_srp_link", args=[srp_link.srp_code]
                     )
-
+                    btn_icon = '<i class="fas fa-check"></i>'
+                    btn_title = _("Enable SRP Link")
+                    modal_id = "enable-srp-link"
                     data_name = srp_link.srp_name + " (" + srp_link.srp_code + ")"
 
                     actions += (
-                        '<a class="btn btn-success btn-sm btn-icon-aasrp" '
-                        'title="{btn_title}" '
-                        'data-toggle="modal" '
-                        'data-target="#{modal_id}" '
-                        'data-url="{data_url}" '
-                        'data-name="{data_name}">{btn_icon}</a>'.format(
-                            data_url=button_enable_url,
-                            data_name=data_name,
-                            btn_icon='<i class="fas fa-check"></i>',
-                            btn_title=_("Enable SRP Link"),
-                            modal_id="enable-srp-link",
-                        )
+                        f'<a class="btn btn-success btn-sm btn-icon-aasrp" '
+                        f'title="{btn_title}" '
+                        f'data-toggle="modal" '
+                        f'data-target="#{modal_id}" '
+                        f'data-url="{button_enable_url}" '
+                        f'data-name="{data_name}">{btn_icon}</a>'
                     )
 
                 button_remove_url = reverse(
                     "aasrp:delete_srp_link", args=[srp_link.srp_code]
                 )
-
+                btn_icon = '<i class="far fa-trash-alt"></i>'
+                btn_title = _("Remove SRP Link")
+                modal_id = "delete-srp-link"
                 data_name = srp_link.srp_name + " (" + srp_link.srp_code + ")"
 
                 actions += (
-                    '<a class="btn btn-danger btn-sm btn-icon-aasrp" '
-                    'title="{btn_title}" '
-                    'data-toggle="modal" '
-                    'data-target="#{modal_id}" '
-                    'data-url="{data_url}" '
-                    'data-name="{data_name}">{btn_icon}</a>'.format(
-                        data_url=button_remove_url,
-                        data_name=data_name,
-                        btn_icon='<i class="far fa-trash-alt"></i>',
-                        btn_title=_("Remove SRP Link"),
-                        modal_id="delete-srp-link",
-                    )
+                    f'<a class="btn btn-danger btn-sm btn-icon-aasrp" '
+                    f'title="{btn_title}" '
+                    f'data-toggle="modal" '
+                    f'data-target="#{modal_id}" '
+                    f'data-url="{button_remove_url}" '
+                    f'data-name="{data_name}">{btn_icon}</a>'
                 )
 
     return actions
 
 
 @login_required
 @permission_required("aasrp.basic_access")
@@ -139,49 +123,39 @@
     """
     get status icon for srp request
     :param request:
     :param srp_request:
     :return:
     """
 
+    request_status_icon_title = _("SRP Request Pending")
     srp_request_status_icon = (
-        '<button class="btn btn-info btn-sm btn-icon-aasrp btn-icon-aasrp-status" '
-        'title="{request_status_icon_title}">'
-        "{request_status_icon}"
-        "</button>".format(
-            request_status_icon='<i class="fas fa-clock"></i>',
-            request_status_icon_title=_("SRP Request Pending"),
-        )
+        f'<button class="btn btn-info btn-sm btn-icon-aasrp btn-icon-aasrp-status" '
+        f'title="{request_status_icon_title}">'
+        f'<i class="fas fa-clock"></i>'
+        f"</button>"
     )
     if srp_request.request_status == AaSrpRequestStatus.APPROVED:
+        btn_classes = "btn btn-success btn-sm btn-icon-aasrp btn-icon-aasrp-status"
+        request_status_icon_title = _("SRP Request Approved")
         srp_request_status_icon = (
-            '<button class="{btn_classes}" '
-            'title="{request_status_icon_title}">'
-            "{request_status_icon}"
-            "</button>".format(
-                btn_classes=(
-                    "btn btn-success btn-sm btn-icon-aasrp btn-icon-aasrp-status"
-                ),
-                request_status_icon='<i class="fas fa-thumbs-up"></i>',
-                request_status_icon_title=_("SRP Request Approved"),
-            )
+            f'<button class="{btn_classes}" '
+            f'title="{request_status_icon_title}">'
+            f'<i class="fas fa-thumbs-up"></i>'
+            f"</button>"
         )
 
     if srp_request.request_status == AaSrpRequestStatus.REJECTED:
+        btn_classes = "btn btn-danger btn-sm btn-icon-aasrp btn-icon-aasrp-status"
+        request_status_icon_title = _("SRP Request Rejected")
         srp_request_status_icon = (
-            '<button class="{btn_classes}" '
-            'title="{request_status_icon_title}">'
-            "{request_status_icon}"
-            "</button>".format(
-                btn_classes=(
-                    "btn btn-danger btn-sm btn-icon-aasrp btn-icon-aasrp-status"
-                ),
-                request_status_icon='<i class="fas fa-thumbs-down"></i>',
-                request_status_icon_title=_("SRP Request Rejected"),
-            )
+            f'<button class="{btn_classes}" '
+            f'title="{request_status_icon_title}">'
+            f'<i class="fas fa-thumbs-down"></i>'
+            f"</button>"
         )
 
     return srp_request_status_icon
 
 
 @login_required
 @permission_required("aasrp.basic_access")
@@ -196,27 +170,25 @@
     """
 
     button_request_details_url = reverse(
         "aasrp:ajax_srp_request_additional_information",
         args=[srp_link.srp_code, srp_request.request_code],
     )
 
+    title = _("SRP Request Details")
+    modal_button_confirm = _("Close")
+
     srp_request_details_icon = (
-        '<button data-link="{link}" '
-        'data-toggle="modal" '
-        'data-target="#srp-request-details" '
-        'data-modal-title="{title}" '
-        'data-modal-button-confirm="{modal_button_confirm}" '
-        'class="btn btn-primary btn-sm btn-icon-aasrp" '
-        'title="{title}">{icon}</button>'.format(
-            link=button_request_details_url,
-            icon='<i class="fas fa-info-circle"></i>',
-            title=_("SRP Request Details"),
-            modal_button_confirm=_("{fa_icon} Close".format(fa_icon="")),
-        )
+        f'<button data-link="{button_request_details_url}" '
+        f'data-toggle="modal" '
+        f'data-target="#srp-request-details" '
+        f'data-modal-title="{title}" '
+        f'data-modal-button-confirm="{modal_button_confirm}" '
+        f'class="btn btn-primary btn-sm btn-icon-aasrp" '
+        f'title="{title}"><i class="fas fa-info-circle"></i></button>'
     )
 
     return srp_request_details_icon
 
 
 @login_required
 @permission_required("aasrp.basic_access")
@@ -235,40 +207,34 @@
         args=[srp_link.srp_code, srp_request.request_code],
     )
 
     button_request_accept_state = ""
     if srp_request.request_status == AaSrpRequestStatus.APPROVED:
         button_request_accept_state = ' disabled="disabled"'
 
+    fa_icon_confirm = "<i class='fas fa-check'></i>"
+    fa_icon_cancel = "<i class='far fa-hand-paper'></i>"
+    icon = '<i class="fas fa-check"></i>'
+    title = _("Accept SRP Request")
+    modal_body = _("Are you sure you want to accept this SRP request?")
+    modal_button_cancel = _(f"{fa_icon_cancel} Cancel")
+    modal_button_confirm = _(f"{fa_icon_confirm} Accept SRP Request")
+    modal_button_confirm_classes = "btn btn-success btn-sm"
+
     srp_request_accept_icon = (
-        '<button data-link="{link}" '
-        'data-toggle="modal" '
-        'data-target="#srp-request-accept" '
-        'data-modal-title="{title}" '
-        'data-modal-body="{modal_body}" '
-        'data-modal-button-cancel="{modal_button_cancel}" '
-        'data-modal-button-confirm="{modal_button_confirm}" '
-        'data-modal-button-confirm-classes="{modal_button_confirm_classes}" '
-        'class="btn btn-success btn-sm btn-icon-aasrp" '
-        'title="{title}"{button_state}>{icon}</button>'.format(
-            link=button_request_accept_url,
-            icon='<i class="fas fa-check"></i>',
-            title=_("Accept SRP Request"),
-            modal_body=_("Are you sure you want to accept this SRP request?"),
-            modal_button_cancel=_(
-                "{fa_icon} Cancel".format(fa_icon="<i class='far fa-hand-paper'></i>")
-            ),
-            modal_button_confirm=_(
-                "{fa_icon} Accept SRP Request".format(
-                    fa_icon="<i class='fas fa-check'></i>"
-                )
-            ),
-            modal_button_confirm_classes="btn btn-success btn-sm",
-            button_state=button_request_accept_state,
-        )
+        f'<button data-link="{button_request_accept_url}" '
+        f'data-toggle="modal" '
+        f'data-target="#srp-request-accept" '
+        f'data-modal-title="{title}" '
+        f'data-modal-body="{modal_body}" '
+        f'data-modal-button-cancel="{modal_button_cancel}" '
+        f'data-modal-button-confirm="{modal_button_confirm}" '
+        f'data-modal-button-confirm-classes="{modal_button_confirm_classes}" '
+        f'class="btn btn-success btn-sm btn-icon-aasrp" '
+        f'title="{title}"{button_request_accept_state}>{icon}</button>'
     )
 
     return srp_request_accept_icon
 
 
 @login_required
 @permission_required("aasrp.basic_access")
@@ -287,40 +253,34 @@
         args=[srp_link.srp_code, srp_request.request_code],
     )
 
     button_request_reject_state = ""
     if srp_request.request_status == AaSrpRequestStatus.REJECTED:
         button_request_reject_state = ' disabled="disabled"'
 
+    fa_icon_confirm = "<i class='fas fa-ban'></i>"
+    fa_icon_cancel = "<i class='far fa-hand-paper'></i>"
+    icon = '<i class="fas fa-ban"></i>'
+    title = _("Reject SRP Request")
+    modal_body = _("Are you sure you want to reject this SRP request?")
+    modal_button_cancel = _(f"{fa_icon_cancel} Cancel")
+    modal_button_confirm = _(f"{fa_icon_confirm} Reject SRP Request")
+    modal_button_confirm_classes = "btn btn-warning btn-sm"
+
     srp_request_reject_icon = (
-        '<button data-link="{link}" '
-        'data-toggle="modal" '
-        'data-target="#srp-request-reject" '
-        'data-modal-title="{title}" '
-        'data-modal-body="{modal_body}" '
-        'data-modal-button-cancel="{modal_button_cancel}" '
-        'data-modal-button-confirm="{modal_button_confirm}" '
-        'data-modal-button-confirm-classes="{modal_button_confirm_classes}" '
-        'class="btn btn-warning btn-sm btn-icon-aasrp" '
-        'title="{title}"{button_state}>{icon}</button>'.format(
-            link=button_request_reject_url,
-            icon='<i class="fas fa-ban"></i>',
-            title=_("Reject SRP Request"),
-            modal_body=_("Are you sure you want to reject this SRP request?"),
-            modal_button_cancel=_(
-                "{fa_icon} Cancel".format(fa_icon="<i class='far fa-hand-paper'></i>")
-            ),
-            modal_button_confirm=_(
-                "{fa_icon} Reject SRP Request".format(
-                    fa_icon="<i class='fas fa-ban'></i>"
-                )
-            ),
-            modal_button_confirm_classes="btn btn-warning btn-sm",
-            button_state=button_request_reject_state,
-        )
+        f'<button data-link="{button_request_reject_url}" '
+        f'data-toggle="modal" '
+        f'data-target="#srp-request-reject" '
+        f'data-modal-title="{title}" '
+        f'data-modal-body="{modal_body}" '
+        f'data-modal-button-cancel="{modal_button_cancel}" '
+        f'data-modal-button-confirm="{modal_button_confirm}" '
+        f'data-modal-button-confirm-classes="{modal_button_confirm_classes}" '
+        f'class="btn btn-warning btn-sm btn-icon-aasrp" '
+        f'title="{title}"{button_request_reject_state}>{icon}</button>'
     )
 
     return srp_request_reject_icon
 
 
 @login_required
 @permission_required("aasrp.basic_access")
@@ -335,39 +295,34 @@
     """
 
     button_request_delete_url = reverse(
         "aasrp:ajax_srp_request_remove",
         args=[srp_link.srp_code, srp_request.request_code],
     )
 
+    fa_icon_confirm = "<i class='fas fa-trash-alt'></i>"
+    fa_icon_cancel = "<i class='far fa-hand-paper'></i>"
+    icon = '<i class="fas fa-trash-alt"></i>'
+    title = _("Remove SRP Request")
+    modal_body = _("Are you sure you want to remove this SRP request?")
+    modal_button_cancel = _(f"{fa_icon_cancel} Cancel")
+    modal_button_confirm = _(f"{fa_icon_confirm} Remove SRP Request")
+    modal_button_confirm_classes = "btn btn-danger btn-sm"
+
     srp_request_delete_icon = (
-        '<button data-link="{link}" '
-        'data-toggle="modal" '
-        'data-target="#srp-request-remove" '
-        'data-modal-title="{title}" '
-        'data-modal-body="{modal_body}" '
-        'data-modal-button-cancel="{modal_button_cancel}" '
-        'data-modal-button-confirm="{modal_button_confirm}" '
-        'data-modal-button-confirm-classes="{modal_button_confirm_classes}" '
-        'class="btn btn-danger btn-sm btn-icon-aasrp" '
-        'title="{title}">{icon}</button>'.format(
-            link=button_request_delete_url,
-            icon='<i class="fas fa-trash-alt"></i>',
-            title=_("Remove SRP Request"),
-            modal_body=_("Are you sure you want to remove this SRP request?"),
-            modal_button_cancel=_(
-                "{fa_icon} Cancel".format(fa_icon="<i class='far fa-hand-paper'></i>")
-            ),
-            modal_button_confirm=_(
-                "{fa_icon} Remove SRP Request".format(
-                    fa_icon="<i class='fas fa-trash-alt'></i>"
-                )
-            ),
-            modal_button_confirm_classes="btn btn-danger btn-sm",
-        )
+        f'<button data-link="{button_request_delete_url}" '
+        f'data-toggle="modal" '
+        f'data-target="#srp-request-remove" '
+        f'data-modal-title="{title}" '
+        f'data-modal-body="{modal_body}" '
+        f'data-modal-button-cancel="{modal_button_cancel}" '
+        f'data-modal-button-confirm="{modal_button_confirm}" '
+        f'data-modal-button-confirm-classes="{modal_button_confirm_classes}" '
+        f'class="btn btn-danger btn-sm btn-icon-aasrp" '
+        f'title="{title}">{icon}</button>'
     )
 
     return srp_request_delete_icon
 
 
 @login_required
 @permission_required("aasrp.manage_srp_requests", "aasrp.manage_srp")
```

### Comparing `aa-srp-1.8.0/aasrp/helper/notification.py` & `aa-srp-1.9.0/aasrp/helper/notification.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,54 @@
 """
 notifications helper
 """
 
+# Django
 from django.contrib.auth.models import User
 
+# Alliance Auth
 from allianceauth.notifications import notify
 
+# AA SRP
 from aasrp.app_settings import aa_discordnotify_active, allianceauth_discordbot_active
 
 
 def send_user_notification(user: User, level: str, title: str, message: str) -> None:
     """
     send notification to user
     this creates a notification in Auth and a PM in Discord when either
     AA-Discordbot or AA Discord Notifications are installed
     :param user:
     :param level:
     :param title:
     :param message:
     """
 
-    notify(
-        user=user,
-        title=title,
-        level=level,
-        message=message,
-    )
+    notify(user=user, title=title, level=level, message=message)
 
     # send a PM to the user on Discord if allianceauth-discordbot
     # is active and not aa-discordnotify
     if allianceauth_discordbot_active() and not aa_discordnotify_active():
+        # Third Party
         import aadiscordbot.tasks
 
-        aadiscordbot.tasks.send_direct_message_by_user_id.delay(
-            user_pk=user.pk, message_content=message
-        )
+        aadiscordbot.tasks.send_direct_message_by_user_id.delay(user.pk, message)
 
 
 def send_message_to_discord_channel(
     channel_id: int, message: str, embed: bool = False
 ) -> None:
     """
     sending a message to a discord channel
     if AA-Discordbot is installed
     :param channel_id:
     :param message:
     :param embed:
     """
 
     if allianceauth_discordbot_active():
+        # Third Party
         import aadiscordbot.tasks
 
         aadiscordbot.tasks.send_channel_message_by_discord_id.delay(
             channel_id, message, embed
         )
```

### Comparing `aa-srp-1.8.0/aasrp/images/aa-srp-dashboard-view-all.jpg` & `aa-srp-1.9.0/aasrp/images/aa-srp-dashboard-view-all.jpg`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/images/aa-srp-dashboard.jpg` & `aa-srp-1.9.0/aasrp/images/aa-srp-dashboard.jpg`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/images/aa-srp-request-details.jpg` & `aa-srp-1.9.0/aasrp/images/aa-srp-request-details.jpg`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/images/aa-srp-requests-overview.jpg` & `aa-srp-1.9.0/aasrp/images/aa-srp-requests-overview.jpg`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/images/aa-srp-your-requests.jpg` & `aa-srp-1.9.0/aasrp/images/aa-srp-your-requests.jpg`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/locale/de/LC_MESSAGES/django.mo` & `aa-srp-1.9.0/aasrp/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/locale/de/LC_MESSAGES/django.po` & `aa-srp-1.9.0/aasrp/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/locale/en/LC_MESSAGES/django.po` & `aa-srp-1.9.0/aasrp/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/locale/es/LC_MESSAGES/django.po` & `aa-srp-1.9.0/aasrp/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/locale/ko/LC_MESSAGES/django.po` & `aa-srp-1.9.0/aasrp/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/locale/ru/LC_MESSAGES/django.po` & `aa-srp-1.9.0/aasrp/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/locale/zh_Hans/LC_MESSAGES/django.po` & `aa-srp-1.9.0/aasrp/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/management/commands/aasrp_load_eve.py` & `aa-srp-1.9.0/aasrp/management/commands/aasrp_load_eve.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+# Standard Library
 import logging
 
+# Django
 from django.core.management import call_command
 from django.core.management.base import BaseCommand
 
+# Alliance Auth (External Libs)
+from app_utils.logging import LoggerAddTag
+
+# AA SRP
 from aasrp import __title__
 from aasrp.constants import EVE_CATEGORY_ID_SHIP
-from aasrp.utils import LoggerAddTag
 
 logger = LoggerAddTag(logging.getLogger(__name__), __title__)
 
 
 class Command(BaseCommand):
     help = "Preloads data required for this app from ESI"
```

### Comparing `aa-srp-1.8.0/aasrp/management/commands/aasrp_migrate_srp_data.py` & `aa-srp-1.9.0/aasrp/management/commands/aasrp_migrate_srp_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 """
 Migrate srp data from the built-in SRP module
 """
 
+# Django
 from django.core.management.base import BaseCommand
 from django.utils.crypto import get_random_string
 
+# Alliance Auth
 from allianceauth.srp.models import SrpFleetMain
+
+# Alliance Auth (External Libs)
 from eveuniverse.models import EveType
 
+# AA SRP
 from aasrp.helper.character import get_user_for_character
 from aasrp.managers import AaSrpManager
 from aasrp.models import (
     AaSrpLink,
     AaSrpRequest,
     AaSrpRequestComment,
     AaSrpRequestCommentType,
@@ -72,19 +77,15 @@
                     # also fix the missing SRP code, we need it!
                     srp_fleet.fleet_srp_code = get_random_string(
                         length=8
                     )  # 8 chars only because old SRP link
 
                 srp_fleet_srp_code = srp_fleet.fleet_srp_code
 
-                self.stdout.write(
-                    "Migrating SRP fleet {srp_code} ...".format(
-                        srp_code=srp_fleet_srp_code
-                    )
-                )
+                self.stdout.write(f"Migrating SRP fleet {srp_fleet_srp_code} ...")
 
                 try:
                     srp_link = AaSrpLink.objects.get(srp_code=srp_fleet_srp_code)
 
                     srp_links_skipped += 1
                 except AaSrpLink.DoesNotExist:
                     srp_link = AaSrpLink()
@@ -105,17 +106,15 @@
 
                     srp_links_migrated += 1
 
                     # get the new srp link object
                     srp_link = AaSrpLink.objects.get(srp_code=srp_fleet_srp_code)
 
                 self.stdout.write(
-                    "Migrating SRP requests for SRP fleet {srp_code} ...".format(
-                        srp_code=srp_fleet_srp_code
-                    )
+                    f"Migrating SRP requests for SRP fleet {srp_fleet_srp_code} ..."
                 )
                 srp_userrequests = srp_fleet.srpuserrequest_set.all()
 
                 for srp_userrequest in srp_userrequests:
                     # let's see if the creator is still valid
                     # returns None when the creators account has been deleted
                     # and no sentinel user can be created or obtained
@@ -196,36 +195,18 @@
                             )
                             srp_request_comment.creator = srp_userrequest_creator
                             srp_request_comment.save()
 
                             srp_requests_migrated += 1
 
         self.stdout.write("Migration finished.")
-
-        self.stdout.write(
-            "SRP links migrated: {srp_links_migrated}".format(
-                srp_links_migrated=srp_links_migrated
-            )
-        )
-        self.stdout.write(
-            "SRP links skipped: {srp_links_skipped}".format(
-                srp_links_skipped=srp_links_skipped
-            )
-        )
-
-        self.stdout.write(
-            "SRP requests migrated: {srp_requests_migrated}".format(
-                srp_requests_migrated=srp_requests_migrated
-            )
-        )
-        self.stdout.write(
-            "SRP requests skipped: {srp_requests_skipped}".format(
-                srp_requests_skipped=srp_requests_skipped
-            )
-        )
+        self.stdout.write(f"SRP links migrated: {srp_links_migrated}")
+        self.stdout.write(f"SRP links skipped: {srp_links_skipped}")
+        self.stdout.write(f"SRP requests migrated: {srp_requests_migrated}")
+        self.stdout.write(f"SRP requests skipped: {srp_requests_skipped}")
 
     def handle(self, *args, **options):
         """
         ask before running ...
         :param args:
         :param options:
         """
```

### Comparing `aa-srp-1.8.0/aasrp/management/commands/aasrp_migrate_to_comments.py` & `aa-srp-1.9.0/aasrp/management/commands/aasrp_migrate_to_comments.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Migrate comments from AaSrpRequest to AaSrpRequestComments
 """
 
+# Django
 from django.core.management import BaseCommand
 
+# AA SRP
 from aasrp.models import (
     AaSrpRequest,
     AaSrpRequestComment,
     AaSrpRequestCommentType,
     AaSrpRequestStatus,
 )
 
@@ -39,22 +41,20 @@
             self.style.WARNING(f"Found {srp_requests.count()} SRP requests.")
         )
 
         if srp_requests.count() > 0:
             for srp_request in srp_requests:
                 reject_reason = srp_request.reject_info
                 srp_info = srp_request.additional_info
+                request_code = srp_request.request_code
 
                 # migrate additional info
                 if srp_info != "":
                     self.stdout.write(
-                        "Updating Request Information "
-                        "for SRP request {request_code}".format(
-                            request_code=srp_request.request_code
-                        )
+                        f"Updating Request Information for SRP request {request_code}"
                     )
 
                     # check if there is already a request info
                     # for this request and remove it
                     AaSrpRequestComment.objects.filter(
                         srp_request=srp_request,
                         comment_type=AaSrpRequestCommentType.REQUEST_INFO,
@@ -76,18 +76,15 @@
 
                 # migrate reject reason
                 if (
                     srp_request.request_status == AaSrpRequestStatus.REJECTED
                     and reject_reason != ""
                 ):
                     self.stdout.write(
-                        "Updating Reject Information "
-                        "for SRP request {request_code}".format(
-                            request_code=srp_request.request_code
-                        )
+                        f"Updating Reject Information for SRP request {request_code}"
                     )
 
                     # check if there is already a reject comment
                     # for this request and remove it
                     AaSrpRequestComment.objects.filter(
                         srp_request=srp_request,
                         comment_type=AaSrpRequestCommentType.REJECT_REASON,
```

### Comparing `aa-srp-1.8.0/aasrp/management/commands/aasrp_update_db_relations.py` & `aa-srp-1.9.0/aasrp/management/commands/aasrp_update_db_relations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Update DB relations
 """
 
+# Django
 from django.core.management.base import BaseCommand
 
+# Alliance Auth (External Libs)
 from eveuniverse.models import EveType
 
+# AA SRP
 from aasrp.managers import AaSrpManager
 from aasrp.models import AaSrpRequest
 
 
 def get_input(text):
     """
     wrapped input to update DB relations
@@ -24,29 +27,23 @@
     def _update_relations(self) -> None:
         """
         updating relations in database
         :return:
         """
 
         srp_requests = AaSrpRequest.objects.filter(ship=None)
+        requests_count = srp_requests.count()
 
         self.stdout.write(
-            self.style.WARNING(
-                "{count} SRP requests need to be updated".format(
-                    count=srp_requests.count()
-                )
-            )
+            self.style.WARNING(f"{requests_count} SRP requests need to be updated")
         )
 
         for srp_request in srp_requests:
-            self.stdout.write(
-                "Updating SRP request {request_code}".format(
-                    request_code=srp_request.request_code
-                )
-            )
+            request_code = srp_request.request_code
+            self.stdout.write(f"Updating SRP request {request_code}")
 
             try:
                 srp_request__ship = EveType.objects.get(name=srp_request.ship_name)
             except EveType.DoesNotExist:
                 srp_kill_link = AaSrpManager.get_kill_id(srp_request.killboard_link)
 
                 (ship_type_id, ship_value, victim_id) = AaSrpManager.get_kill_data(
```

### Comparing `aa-srp-1.8.0/aasrp/managers.py` & `aa-srp-1.9.0/aasrp/managers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 """
 SRP Manager
 """
 
+# Third Party
 import requests
 
+# Django
 from django.contrib.auth.models import User
 from django.utils.translation import gettext_lazy as _
 
+# Alliance Auth
 from allianceauth.services.hooks import get_extension_logger
 
+# Alliance Auth (External Libs)
+from app_utils.logging import LoggerAddTag
+
+# AA SRP
 from aasrp import __title__
 from aasrp.constants import USERAGENT, ZKILLBOARD_API_URL
 from aasrp.models import AaSrpRequest, AaSrpRequestStatus
 from aasrp.providers import esi
-from aasrp.utils import LoggerAddTag
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 class AaSrpManager:
     """
     AaSrpManager
```

### Comparing `aa-srp-1.8.0/aasrp/migrations/0001_initial.py` & `aa-srp-1.9.0/aasrp/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Generated by Django 3.1.4 on 2020-12-28 13:30
 
+# Django
 import django.db.models.deletion
 import django.utils.timezone
 from django.conf import settings
 from django.db import migrations, models
 
+# AA SRP
 import aasrp.models
 
 
 class Migration(migrations.Migration):
 
     initial = True
```

### Comparing `aa-srp-1.8.0/aasrp/migrations/0002_relations_update.py` & `aa-srp-1.9.0/aasrp/migrations/0002_relations_update.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Generated by Django 3.1.5 on 2021-01-04 21:23
 
+# Django
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
+# AA SRP
 import aasrp.models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ("eveonline", "0012_index_additions"),
```

### Comparing `aa-srp-1.8.0/aasrp/migrations/0004_aasrpusersettings.py` & `aa-srp-1.9.0/aasrp/migrations/0004_aasrpusersettings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Generated by Django 3.1.7 on 2021-03-13 23:36
 
+# Django
 from django.conf import settings
 from django.db import migrations, models
 
+# AA SRP
 import aasrp.models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
```

### Comparing `aa-srp-1.8.0/aasrp/migrations/0005_insurance.py` & `aa-srp-1.9.0/aasrp/migrations/0005_insurance.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Generated by Django 3.2.2 on 2021-05-12 02:02
 
+# Django
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
```

### Comparing `aa-srp-1.8.0/aasrp/migrations/0006_related_names.py` & `aa-srp-1.9.0/aasrp/migrations/0006_related_names.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Generated by Django 3.2.6 on 2021-08-18 13:14
 
+# Django
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
```

### Comparing `aa-srp-1.8.0/aasrp/models.py` & `aa-srp-1.9.0/aasrp/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """
 Our Models
 """
 
+# Django
 from django.contrib.auth.models import User
 from django.db import models
 from django.utils import timezone
 from django.utils.translation import gettext as _
 
+# Alliance Auth
 from allianceauth.eveonline.models import EveCharacter
+
+# Alliance Auth (External Libs)
 from eveuniverse.models import EveType
 
 
 def get_sentinel_user():
     """
     get user or create one
     :return:
@@ -101,16 +105,16 @@
         null=True,
         blank=True,
         default=None,
         on_delete=models.SET(get_sentinel_user),
         help_text=_("Who created the SRP link?"),
     )
 
-    def __str__(self):
-        return self.srp_name
+    def __str__(self) -> str:
+        return str(self.srp_name)
 
     @property
     def total_cost(self):
         """
         total cost for this SRP link
         :return:
         """
```

### Comparing `aa-srp-1.8.0/aasrp/static/aasrp/css/aa-srp.css` & `aa-srp-1.9.0/aasrp/static/aasrp/css/aa-srp.css`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/static/aasrp/css/aa-srp.min.css` & `aa-srp-1.9.0/aasrp/static/aasrp/css/aa-srp.min.css`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/static/aasrp/javascript/aa-srp-dashboard.js` & `aa-srp-1.9.0/aasrp/static/aasrp/javascript/aa-srp-dashboard.js`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js` & `aa-srp-1.9.0/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/static/aasrp/javascript/aa-srp-view-requests.js` & `aa-srp-1.9.0/aasrp/static/aasrp/javascript/aa-srp-view-requests.js`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js` & `aa-srp-1.9.0/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/static/aasrp/libs/datatables/plugins/dataTables.rowGroup.min.js` & `aa-srp-1.9.0/aasrp/static/aasrp/libs/datatables/plugins/dataTables.rowGroup.min.js`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/static/aasrp/libs/datatables/plugins/datetime.js` & `aa-srp-1.9.0/aasrp/static/aasrp/libs/datatables/plugins/datetime.js`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/static/aasrp/libs/datatables/plugins/datetime.min.js` & `aa-srp-1.9.0/aasrp/static/aasrp/libs/datatables/plugins/datetime.min.js`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/css/bootstrap-editable.css` & `aa-srp-1.9.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/css/bootstrap-editable.css`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/css/bootstrap-editable.min.css` & `aa-srp-1.9.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/css/bootstrap-editable.min.css`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/img/loading.gif` & `aa-srp-1.9.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/img/loading.gif`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/js/bootstrap-editable.js` & `aa-srp-1.9.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/js/bootstrap-editable.js`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/js/bootstrap-editable.min.js` & `aa-srp-1.9.0/aasrp/static/aasrp/libs/x-editable/1.5.0/bootstrap3-editable/js/bootstrap-editable.min.js`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/dashboard.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/dashboard.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/link_add.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/link_add.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/link_edit.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/link_edit.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/modals/dashboard/delete_srp_link.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/modals/dashboard/delete_srp_link.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/modals/dashboard/disable_srp_link.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/modals/dashboard/disable_srp_link.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/modals/dashboard/enable_srp_link.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/modals/dashboard/enable_srp_link.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/modals/view_requests/accept_request.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/modals/view_requests/accept_request.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/modals/view_requests/mark_complete_modal.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/modals/view_requests/mark_complete_modal.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/modals/view_requests/reject_request.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/modals/view_requests/reject_request.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/modals/view_requests/remove_request.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/modals/view_requests/remove_request.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/modals/view_requests/request_details.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/modals/view_requests/request_details.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/partials/dashboard/srp_links.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/partials/dashboard/srp_links.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/partials/dashboard/table.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/partials/dashboard/table.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/partials/dashboard/user_settings.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/partials/dashboard/user_settings.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/partials/dashboard/user_srp_requests.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/partials/dashboard/user_srp_requests.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/partials/link_add/form.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/partials/link_add/form.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/partials/link_edit/form.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/partials/link_edit/form.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/partials/request_srp/form.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/partials/request_srp/form.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/partials/view_requests/overview.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/partials/view_requests/overview.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/partials/view_requests/requests.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/partials/view_requests/requests.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/request_srp.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/request_srp.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/templates/aasrp/view_requests.html` & `aa-srp-1.9.0/aasrp/templates/aasrp/view_requests.html`

 * *Files identical despite different names*

### Comparing `aa-srp-1.8.0/aasrp/urls.py` & `aa-srp-1.9.0/aasrp/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 aasrp url config
 """
 
+# Django
 from django.conf.urls import url
 
+# AA SRP
 from aasrp import views
 
 app_name: str = "aasrp"
 
 urlpatterns = [
     url(r"^$", views.dashboard, name="dashboard"),
     url(r"^all/$", views.dashboard, {"show_all_links": True}, name="all"),
```

### Comparing `aa-srp-1.8.0/aasrp/utils.py` & `aa-srp-1.9.0/aasrp/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,26 @@
 """
 utilities
 """
 
-import logging
-
+# Django
 from django.conf import settings
 from django.utils.functional import lazy
 from django.utils.html import format_html
 from django.utils.translation import gettext_lazy as _
 
+# Alliance Auth
 from allianceauth.authentication.admin import User
 from allianceauth.services.hooks import get_extension_logger
 
-from aasrp import __title__
-
-
-class LoggerAddTag(logging.LoggerAdapter):
-    """
-    add custom tag to a logger
-    """
-
-    def __init__(self, my_logger, prefix):
-        super().__init__(my_logger, {})
-        self.prefix = prefix
-
-    def process(self, msg, kwargs):
-        """
-        process log items
-        :param msg:
-        :param kwargs:
-        :return:
-        """
-
-        return f"[{self.prefix}] {msg}", kwargs
+# Alliance Auth (External Libs)
+from app_utils.logging import LoggerAddTag
 
+# AA SRP
+from aasrp import __title__
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 def clean_setting(
     name: str,
     default_value: object,
@@ -73,16 +56,16 @@
             isinstance(getattr(settings, name), required_type)
             and (min_value is None or getattr(settings, name) >= min_value)
             and (max_value is None or getattr(settings, name) <= max_value)
         ):
             cleaned_value = getattr(settings, name)
         else:
             logger.warning(
-                "You setting for {name} is not valid. Please correct it. "
-                "Using default for now: {value}".format(name=name, value=default_value)
+                f"You setting for {name} is not valid. Please correct it. "
+                f"Using default for now: {default_value}"
             )
             cleaned_value = default_value
 
     return cleaned_value
 
 
 # Format for output of datetime for this app
```

### Comparing `aa-srp-1.8.0/aasrp/views.py` & `aa-srp-1.9.0/aasrp/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 """
 the views
 """
 
+# Django
 from django.contrib import messages
 from django.contrib.auth.decorators import login_required, permission_required
 from django.core.handlers.wsgi import WSGIRequest
 from django.http import HttpResponse, JsonResponse
 from django.shortcuts import redirect, render
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.crypto import get_random_string
 from django.utils.translation import gettext_lazy as _
 
+# Alliance Auth
 from allianceauth.authentication.decorators import permissions_required
 from allianceauth.eveonline.models import EveCharacter
 from allianceauth.services.hooks import get_extension_logger
+
+# Alliance Auth (External Libs)
+from app_utils.logging import LoggerAddTag
+from app_utils.urls import reverse_absolute, site_absolute_url
 from eveuniverse.models import EveType
 
+# AA SRP
 from aasrp import __title__
-from aasrp.app_settings import AASRP_SRP_TEAM_DISCORD_CHANNEL, avoid_cdn, get_site_url
+from aasrp.app_settings import AASRP_SRP_TEAM_DISCORD_CHANNEL, avoid_cdn
 from aasrp.constants import SRP_REQUEST_NOTIFICATION_INQUIRY_NOTE, ZKILLBOARD_BASE_URL
 from aasrp.form import (
     AaSrpLinkForm,
     AaSrpLinkUpdateForm,
     AaSrpRequestForm,
     AaSrpRequestPayoutForm,
     AaSrpRequestRejectForm,
@@ -36,27 +43,26 @@
     get_srp_request_details_icon,
     get_srp_request_status_icon,
 )
 from aasrp.helper.notification import (
     send_message_to_discord_channel,
     send_user_notification,
 )
-from aasrp.helper.urls import reverse_absolute
 from aasrp.managers import AaSrpManager
 from aasrp.models import (
     AaSrpInsurance,
     AaSrpLink,
     AaSrpRequest,
     AaSrpRequestComment,
     AaSrpRequestCommentType,
     AaSrpRequestStatus,
     AaSrpStatus,
     AaSrpUserSettings,
 )
-from aasrp.utils import LoggerAddTag, get_main_character_from_user
+from aasrp.utils import get_main_character_from_user
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 def _attempt_to_re_add_ship_information_to_request(
     srp_request: AaSrpRequest,
 ) -> AaSrpRequest:
@@ -120,21 +126,17 @@
             user_settings.disable_notifications = user_settings_form.cleaned_data[
                 "disable_notifications"
             ]
             user_settings.save()
     else:
         user_settings_form = AaSrpUserSettingsForm(instance=user_settings)
 
-    logger_message = "Dashboard with available SRP links called by {user}".format(
-        user=request.user
-    )
+    logger_message = f"Dashboard with available SRP links called by {request.user}"
     if show_all_links is True:
-        logger_message = "Dashboard with all SRP links called by {user}".format(
-            user=request.user
-        )
+        logger_message = f"Dashboard with all SRP links called by {request.user}"
 
     logger.info(logger_message)
 
     context = {
         "avoid_cdn": avoid_cdn(),
         "show_all_links": show_all_links,
         "user_settings_form": user_settings_form,
@@ -152,46 +154,45 @@
     ajax request
     get all active srp links
     :param request:
     :param show_all_links:
     :return:
     """
 
-    data = list()
+    data = []
 
     srp_links = AaSrpLink.objects.prefetch_related(
         "fleet_commander",
         "creator",
         "creator__profile__main_character",
         "srp_requests",
     ).all()
 
     if not show_all_links:
         srp_links = srp_links.filter(srp_status=AaSrpStatus.ACTIVE)
 
     for srp_link in srp_links:
         aar_link = ""
         if srp_link.aar_link:
-            aar_link = '<a href="{aar_link}" target="_blank">{link_text}</a>'.format(
-                aar_link=srp_link.aar_link, link_text=_("Link")
-            )
+            aar_href = srp_link.aar_link
+            link_text = _("Link")
+            aar_link = f'<a href="{aar_href}" target="_blank">{link_text}</a>'
 
         srp_code_html = srp_link.srp_code
         if srp_link.srp_status == AaSrpStatus.ACTIVE:
+            css_classes = (
+                "aa-srp-fa-icon aa-srp-fa-icon-right copy-text-fa-icon far fa-copy"
+            )
+            srp_link_href = reverse_absolute(
+                "aasrp:request_srp", args=[srp_link.srp_code]
+            )
+            title = _("Copy SRP link to clipboard")
             srp_code_html += (
-                '<i class="{css_classes}" '
-                'data-clipboard-text="{srp_link}" title="{title}"></i>'
-            ).format(
-                css_classes=(
-                    "aa-srp-fa-icon aa-srp-fa-icon-right copy-text-fa-icon far fa-copy"
-                ),
-                srp_link=reverse_absolute(
-                    "aasrp:request_srp", args=[srp_link.srp_code]
-                ),
-                title=_("Copy SRP link to clipboard"),
+                f'<i class="{css_classes}" '
+                f'data-clipboard-text="{srp_link_href}" title="{title}"></i>'
             )
 
         actions = get_dashboard_action_icons(request=request, srp_link=srp_link)
 
         data.append(
             {
                 "srp_name": srp_link.srp_name,
@@ -217,15 +218,15 @@
     """
     ajax request
     get user srp requests
     :param request:
     :return:
     """
 
-    data = list()
+    data = []
 
     requests = (
         AaSrpRequest.objects.filter(creator=request.user)
         # .filter(ship__isnull=False)
         .prefetch_related(
             "creator",
             "creator__profile__main_character",
@@ -258,23 +259,21 @@
                 ship_render_icon_html = get_type_render_url_from_type_id(
                     evetype_id=srp_request.ship.id,
                     evetype_name=srp_request.ship.name,
                     size=32,
                     as_html=True,
                 )
 
+            zkb_link = srp_request.killboard_link
+            zkb_link_text = srp_request.ship.name
             killboard_link = (
-                '<a href="{zkb_link}" target="_blank">'
-                "{ship_render_icon_html}"
-                "<span>{zkb_link_text}</span>"
-                "</a>".format(
-                    zkb_link=srp_request.killboard_link,
-                    zkb_link_text=srp_request.ship.name,
-                    ship_render_icon_html=ship_render_icon_html,
-                )
+                f'<a href="{zkb_link}" target="_blank">'
+                f"{ship_render_icon_html}"
+                f"<span>{zkb_link_text}</span>"
+                f"</a>"
             )
 
         srp_request_status_icon = get_srp_request_status_icon(
             request=request, srp_request=srp_request
         )
 
         srp_request_details_icon = get_srp_request_details_icon(
@@ -370,26 +369,22 @@
     """
     add or edit AAR link
     :param request:
     :param srp_code:
     :return:
     """
 
-    logger.info(
-        "Edit SRP link form for SRP code {srp_code} called by {user}".format(
-            srp_code=srp_code, user=request.user
-        )
-    )
+    request_user = request.user
+
+    logger.info(f"Edit SRP link form for SRP code {srp_code} called by {request_user}")
 
     # check if the provided SRP code is valid
     if AaSrpLink.objects.filter(srp_code=srp_code).exists() is False:
         logger.error(
-            "Unable to locate SRP Fleet using code {srp_code} for user {user}".format(
-                srp_code=srp_code, user=request.user
-            )
+            f"Unable to locate SRP Fleet using code {srp_code} for user {request_user}"
         )
 
         messages.error(
             request,
             _(f"Unable to locate SRP code with ID {srp_code}"),
         )
 
@@ -425,36 +420,27 @@
 def request_srp(request: WSGIRequest, srp_code: str) -> HttpResponse:
     """
     srp request
     :param request:
     :param srp_code:
     """
 
-    logger.info(
-        "SRP request form for SRP code {srp_code} called by {user}".format(
-            user=request.user, srp_code=srp_code
-        )
-    )
+    request_user = request.user
+
+    logger.info(f"SRP request form for SRP code {srp_code} called by {request_user}")
 
     # check if the provided SRP code is valid
     if AaSrpLink.objects.filter(srp_code=srp_code).exists() is False:
         logger.error(
-            "Unable to locate SRP Fleet "
-            "using SRP code {srp_code} for user {user}".format(
-                srp_code=srp_code, user=request.user
-            )
+            f"Unable to locate SRP Fleet using SRP code {srp_code} for user {request_user}"
         )
 
         messages.error(
             request,
-            _(
-                "Unable to locate SRP Fleet using SRP code {srp_code}".format(
-                    srp_code=srp_code
-                )
-            ),
+            _(f"Unable to locate SRP Fleet using SRP code {srp_code}"),
         )
 
         return redirect("aasrp:dashboard")
 
     srp_link = AaSrpLink.objects.get(srp_code=srp_code)
 
     # check if the SRP link is still open
@@ -465,20 +451,17 @@
 
         return redirect("aasrp:dashboard")
 
     # if this is a POST request we need to process the form data
     if request.method == "POST":
         # create a form instance and populate it with data from the request
         form = AaSrpRequestForm(request.POST)
+        form_is_valid = form.is_valid()
 
-        logger.debug(
-            "Request type POST contains valid form: {form_is_valid}".format(
-                form_is_valid=form.is_valid()
-            )
-        )
+        logger.debug(f"Request type POST contains valid form: {form_is_valid}")
 
         # check whether it's valid:
         if form.is_valid():
             creator = request.user
             post_time = timezone.now()
 
             srp_request = AaSrpRequest()
@@ -491,19 +474,18 @@
                 srp_kill_link = AaSrpManager.get_kill_id(srp_request.killboard_link)
 
                 (ship_type_id, ship_value, victim_id) = AaSrpManager.get_kill_data(
                     srp_kill_link
                 )
             except ValueError:
                 # invalid killmail
+                killmail_link = srp_request.killboard_link
                 logger.debug(
-                    "User {user} submitted an invalid killmail link ({killmail_link}) "
-                    "or zKillboard server could not be reached".format(
-                        user=request.user, killmail_link=srp_request.killboard_link
-                    )
+                    f"User {request_user} submitted an invalid killmail link ({killmail_link}) "
+                    f"or zKillboard server could not be reached"
                 )
 
                 messages.error(
                     request,
                     _(
                         "Your SRP request Killmail link is invalid. "
                         f"Please make sure you are using {ZKILLBOARD_BASE_URL}"
@@ -550,37 +532,30 @@
                     insurance = AaSrpInsurance()
                     insurance.srp_request = srp_request
                     insurance.insurance_level = insurance_level["name"]
                     insurance.insurance_cost = insurance_level["cost"]
                     insurance.insurance_payout = insurance_level["payout"]
                     insurance.save()
 
+                user_name = request.user
+                character_name = srp_request__character
+                srp_name = srp_link.srp_name
+                srp_code = srp_request.request_code
                 logger.info(
-                    "Created SRP request on behalf of user {user_name} "
-                    "(character: {character_name}) for fleet name {srp_name} "
-                    "with SRP code {srp_code}".format(
-                        user_name=request.user,
-                        character_name=srp_request__character,
-                        srp_name=srp_link.srp_name,
-                        srp_code=srp_request.request_code,
-                    )
+                    f"Created SRP request on behalf of user {user_name} "
+                    f"(character: {character_name}) for fleet name {srp_name} "
+                    f"with SRP code {srp_code}"
                 )
 
-                messages.success(
-                    request,
-                    _(
-                        "Submitted SRP request for your {ship}.".format(
-                            ship=srp_request.ship.name
-                        )
-                    ),
-                )
+                ship = srp_request.ship.name
+                messages.success(request, _(f"Submitted SRP request for your {ship}."))
 
                 # send message to the srp team in their discord channel
                 if AASRP_SRP_TEAM_DISCORD_CHANNEL is not None:
-                    site_base_url = get_site_url()
+                    site_base_url = site_absolute_url()
                     request_code = srp_request.request_code
                     character_name = srp_request__character.character_name
                     ship_type = srp_request__ship.name
                     zkillboard_link = srp_request.killboard_link
                     additional_information = srp_request_comment.comment.replace(
                         "@", "{@}"
                     )
@@ -605,23 +580,23 @@
 
                     logger.info(
                         "Sending SRP request notification to the SRP team channel on "
                         "Discord"
                     )
 
                 return redirect("aasrp:dashboard")
-            else:
-                messages.error(
-                    request,
-                    _(
-                        f"Character {victim_id} does not belong to your Auth "
-                        "account. Please add this character as an alt to "
-                        "your main and try again."
-                    ),
-                )
+
+            messages.error(
+                request,
+                _(
+                    f"Character {victim_id} does not belong to your Auth "
+                    f"account. Please add this character as an alt to "
+                    f"your main and try again."
+                ),
+            )
 
             return redirect("aasrp:dashboard")
 
     # if a GET (or any other method) we'll create a blank form
     else:
         logger.debug(f"Returning blank SRP request form for {request.user}")
 
@@ -707,15 +682,15 @@
     """
     ajax request
     get datatable data
     :param srp_code:
     :param request:
     """
 
-    data = list()
+    data = []
 
     # srp_link = AaSrpLink.objects.get(srp_code=srp_code)
     # srp_requests = srp_link.srp_requests.all()
 
     srp_requests = AaSrpRequest.objects.filter(
         srp_link__srp_code__iexact=srp_code
     ).prefetch_related(
@@ -1024,15 +999,15 @@
 ) -> JsonResponse:
     """
     :param request:
     :param srp_code:
     :param srp_request_code:
     """
 
-    data = list()
+    data = []
 
     if request.method == "POST":
         try:
             srp_request = AaSrpRequest.objects.get(
                 request_code=srp_request_code, srp_link__srp_code=srp_code
             )
 
@@ -1060,15 +1035,15 @@
 ) -> JsonResponse:
     """
     :param request:
     :param srp_code:
     :param srp_request_code:
     """
 
-    data = list()
+    data = []
 
     try:
         srp_request = AaSrpRequest.objects.get(
             request_code=srp_request_code, srp_link__srp_code=srp_code
         )
 
         requester = srp_request.creator
@@ -1087,27 +1062,26 @@
         srp_request.request_status = AaSrpRequestStatus.APPROVED
         srp_request.save()
 
         user_settings = AaSrpUserSettings.objects.get(user=request.user)
 
         # check if the user has notifications activated (it's by default)
         if user_settings.disable_notifications is False:
+            ship_name = srp_request.ship.name
+            fleet_name = srp_request.srp_link.srp_name
+            srp_code = srp_request.srp_link.srp_code
+            request_code = srp_request.request_code
+            reviser = get_main_character_from_user(request.user)
+            inquiry_note = SRP_REQUEST_NOTIFICATION_INQUIRY_NOTE
             notification_message = (
-                "Your SRP request regarding your {ship_name} lost during "
-                "{fleet_name} has been approved.\n\n"
-                "Request Details:\nSRP-Code: {srp_code}\n"
-                "Request-Code: {request_code}\n"
-                "Reviser: {reviser}\n\n{inquiry_note}".format(
-                    ship_name=srp_request.ship.name,
-                    fleet_name=srp_request.srp_link.srp_name,
-                    srp_code=srp_request.srp_link.srp_code,
-                    request_code=srp_request.request_code,
-                    reviser=get_main_character_from_user(request.user),
-                    inquiry_note=SRP_REQUEST_NOTIFICATION_INQUIRY_NOTE,
-                )
+                f"Your SRP request regarding your {ship_name} lost during "
+                f"{fleet_name} has been approved.\n\n"
+                f"Request Details:\nSRP-Code: {srp_code}\n"
+                f"Request-Code: {request_code}\n"
+                f"Reviser: {reviser}\n\n{inquiry_note}"
             )
 
             send_user_notification(
                 user=requester,
                 level="success",
                 title=_("SRP Request Approved"),
                 message=notification_message,
@@ -1127,15 +1101,15 @@
 ) -> JsonResponse:
     """
     :param request:
     :param srp_code:
     :param srp_request_code:
     """
 
-    data = list()
+    data = []
 
     try:
         if request.method == "POST":
             # create a form instance and populate it with data from the request
             form = AaSrpRequestRejectForm(request.POST)
 
             # check whether it's valid:
@@ -1165,29 +1139,28 @@
                 srp_request_comment.creator = request.user
                 srp_request_comment.save()
 
                 user_settings = AaSrpUserSettings.objects.get(user=request.user)
 
                 # check if the user has notifications activated (it's by default)
                 if user_settings.disable_notifications is False:
+                    ship_name = srp_request.ship.name
+                    fleet_name = srp_request.srp_link.srp_name
+                    reject_info = reject_info
+                    srp_code = srp_request.srp_link.srp_code
+                    request_code = srp_request.request_code
+                    reviser = get_main_character_from_user(request.user)
+                    inquiry_note = SRP_REQUEST_NOTIFICATION_INQUIRY_NOTE
                     notification_message = (
-                        "Your SRP request regarding your {ship_name} lost during "
-                        "{fleet_name} has been rejected.\n\n"
-                        "Reason:\n{reject_info}\n\n"
-                        "Request Details:\nSRP-Code: {srp_code}\n"
-                        "Request-Code: {request_code}\n"
-                        "Reviser: {reviser}\n\n{inquiry_note}".format(
-                            ship_name=srp_request.ship.name,
-                            fleet_name=srp_request.srp_link.srp_name,
-                            reject_info=reject_info,
-                            srp_code=srp_request.srp_link.srp_code,
-                            request_code=srp_request.request_code,
-                            reviser=get_main_character_from_user(request.user),
-                            inquiry_note=SRP_REQUEST_NOTIFICATION_INQUIRY_NOTE,
-                        )
+                        f"Your SRP request regarding your {ship_name} lost during "
+                        f"{fleet_name} has been rejected.\n\n"
+                        f"Reason:\n{reject_info}\n\n"
+                        f"Request Details:\nSRP-Code: {srp_code}\n"
+                        f"Request-Code: {request_code}\n"
+                        f"Reviser: {reviser}\n\n{inquiry_note}"
                     )
 
                     send_user_notification(
                         user=requester,
                         level="danger",
                         title=_("SRP Request Rejected"),
                         message=notification_message,
@@ -1209,15 +1182,15 @@
 ) -> JsonResponse:
     """
     :param request:
     :param srp_code:
     :param srp_request_code:
     """
 
-    data = list()
+    data = []
 
     try:
         srp_request = AaSrpRequest.objects.get(
             request_code=srp_request_code, srp_link__srp_code=srp_code
         )
 
         srp_request.delete()
```

### Comparing `aa-srp-1.8.0/setup.py` & `aa-srp-1.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Setting up our app
 """
 
+# Standard Library
 import os
 
+# Third Party
 from setuptools import find_packages, setup
 
+# AA SRP
 from aasrp import __version__
 
 # Read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     project_long_description = f.read()
 
@@ -22,29 +25,34 @@
 project_license = "GPLv3"
 project_author = "Peter Pfeufer"
 project_author_email = "development@ppfeufer.de"
 project_git_url = "https://github.com/ppfeufer/aa-srp"
 project_issues_url = f"{project_git_url}/issues"
 project_changelog_url = f"{project_git_url}/blob/master/CHANGELOG.md"
 project_homepage_url = project_git_url
-project_install_requirements = ["allianceauth>=2.9.3", "django-eveuniverse>=0.8.2"]
+project_install_requirements = [
+    "allianceauth>=2.9.3",
+    "allianceauth-app-utils>=1.9.0",
+    "django-eveuniverse>=0.8.2",
+]
 project_python_requires = "~=3.7"
 project_classifiers = [
     "Environment :: Web Environment",
     "Framework :: Django",
     "Framework :: Django :: 3.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 
 # URLs are listed in reverse on Pypi
 project_urls = {
     "Issue / Bug Reports": project_issues_url,
```

### Comparing `aa-srp-1.8.0/testauth/settings.py` & `aa-srp-1.9.0/testauth/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # flake8: noqa
 
+# Standard Library
 import os
 
+# Third Party
 from celery.schedules import crontab
 
+# Django
 from django.contrib import messages
 
 INSTALLED_APPS = [
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
```

