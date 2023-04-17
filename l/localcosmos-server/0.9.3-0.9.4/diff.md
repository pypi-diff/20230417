# Comparing `tmp/localcosmos_server-0.9.3.tar.gz` & `tmp/localcosmos_server-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localcosmos_server-0.9.3.tar", last modified: Fri Apr 29 09:29:40 2022, max compression
+gzip compressed data, was "localcosmos_server-0.9.4.tar", last modified: Fri May 13 14:25:25 2022, max compression
```

## Comparing `localcosmos_server-0.9.3.tar` & `localcosmos_server-0.9.4.tar`

### file list

```diff
@@ -1,1498 +1,1498 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.178258 localcosmos_server-0.9.3/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2018-07-30 12:18:06.000000 localcosmos_server-0.9.3/LICENCE
--rw-r--r--   0 tom       (1000) tom       (1000)      563 2020-04-06 07:18:54.000000 localcosmos_server-0.9.3/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)      806 2022-04-29 09:29:40.178258 localcosmos_server-0.9.3/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      189 2019-11-15 15:44:36.000000 localcosmos_server-0.9.3/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.954262 localcosmos_server-0.9.3/localcosmos_server/
--rw-r--r--   0 tom       (1000) tom       (1000)       50 2022-04-29 09:29:11.000000 localcosmos_server-0.9.3/localcosmos_server/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      165 2019-11-14 15:30:50.000000 localcosmos_server-0.9.3/localcosmos_server/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      709 2019-09-10 12:32:06.000000 localcosmos_server-0.9.3/localcosmos_server/anycluster_schema_urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1711 2019-10-02 09:15:04.000000 localcosmos_server-0.9.3/localcosmos_server/anycluster_schema_views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.954262 localcosmos_server-0.9.3/localcosmos_server/api/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2019-03-25 10:52:36.000000 localcosmos_server-0.9.3/localcosmos_server/api/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1281 2019-03-25 11:25:56.000000 localcosmos_server-0.9.3/localcosmos_server/api/authentication.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2169 2020-01-14 16:23:50.000000 localcosmos_server-0.9.3/localcosmos_server/api/permissions.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1186 2019-10-01 14:23:52.000000 localcosmos_server-0.9.3/localcosmos_server/api/road_permissions.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3275 2020-03-23 08:27:04.000000 localcosmos_server-0.9.3/localcosmos_server/api/road_serializers.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7260 2020-11-14 08:46:40.000000 localcosmos_server-0.9.3/localcosmos_server/api/serializers.py
--rw-r--r--   0 tom       (1000) tom       (1000)      842 2020-04-22 10:24:04.000000 localcosmos_server-0.9.3/localcosmos_server/api/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10663 2020-04-23 06:54:44.000000 localcosmos_server-0.9.3/localcosmos_server/api/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.954262 localcosmos_server-0.9.3/localcosmos_server/app_admin/
--rw-r--r--   0 tom       (1000) tom       (1000)       73 2019-07-02 05:56:40.000000 localcosmos_server-0.9.3/localcosmos_server/app_admin/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2019-03-25 10:52:50.000000 localcosmos_server-0.9.3/localcosmos_server/app_admin/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)       92 2019-04-02 14:03:28.000000 localcosmos_server-0.9.3/localcosmos_server/app_admin/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)      399 2020-04-03 11:08:46.000000 localcosmos_server-0.9.3/localcosmos_server/app_admin/forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1559 2020-03-03 11:33:16.000000 localcosmos_server-0.9.3/localcosmos_server/app_admin/middleware.py
--rw-r--r--   0 tom       (1000) tom       (1000)       57 2019-03-25 10:52:50.000000 localcosmos_server-0.9.3/localcosmos_server/app_admin/models.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.950262 localcosmos_server-0.9.3/localcosmos_server/app_admin/static/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.950262 localcosmos_server-0.9.3/localcosmos_server/app_admin/static/app_admin/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.954262 localcosmos_server-0.9.3/localcosmos_server/app_admin/static/app_admin/css/
--rw-r--r--   0 tom       (1000) tom       (1000)      215 2019-10-15 09:37:58.000000 localcosmos_server-0.9.3/localcosmos_server/app_admin/static/app_admin/css/app_admin.css
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.954262 localcosmos_server-0.9.3/localcosmos_server/app_admin/static/app_admin/img/
--rw-r--r--   0 tom       (1000) tom       (1000)     5970 2019-09-19 12:05:20.000000 localcosmos_server-0.9.3/localcosmos_server/app_admin/static/app_admin/img/downarrow.svg
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.950262 localcosmos_server-0.9.3/localcosmos_server/app_admin/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.958262 localcosmos_server-0.9.3/localcosmos_server/app_admin/templates/app_admin/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.958262 localcosmos_server-0.9.3/localcosmos_server/app_admin/templates/app_admin/ajax/
--rw-r--r--   0 tom       (1000) tom       (1000)      883 2020-04-03 11:28:58.000000 localcosmos_server-0.9.3/localcosmos_server/app_admin/templates/app_admin/ajax/userbox.html
--rw-r--r--   0 tom       (1000) tom       (1000)     4682 2022-04-21 09:09:53.000000 localcosmos_server-0.9.3/localcosmos_server/app_admin/templates/app_admin/base.html
--rw-r--r--   0 tom       (1000) tom       (1000)      995 2019-11-19 16:08:36.000000 localcosmos_server-0.9.3/localcosmos_server/app_admin/templates/app_admin/home.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1017 2020-04-03 11:28:06.000000 localcosmos_server-0.9.3/localcosmos_server/app_admin/templates/app_admin/manage_app_user_role.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2474 2020-04-03 11:28:30.000000 localcosmos_server-0.9.3/localcosmos_server/app_admin/templates/app_admin/userlist.html
--rw-r--r--   0 tom       (1000) tom       (1000)      492 2019-10-09 07:37:30.000000 localcosmos_server-0.9.3/localcosmos_server/app_admin/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)      628 2019-10-01 13:20:58.000000 localcosmos_server-0.9.3/localcosmos_server/app_admin/view_mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4941 2020-02-18 11:38:24.000000 localcosmos_server-0.9.3/localcosmos_server/app_admin/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)      110 2019-03-25 08:50:38.000000 localcosmos_server-0.9.3/localcosmos_server/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)      242 2019-11-12 14:45:50.000000 localcosmos_server-0.9.3/localcosmos_server/context_processors.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.958262 localcosmos_server-0.9.3/localcosmos_server/datasets/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2019-03-25 09:05:02.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2019-03-25 09:05:02.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)       91 2019-06-24 06:12:48.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3295 2020-04-28 06:44:46.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/csv_export.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2106 2019-09-26 06:48:48.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/fields.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5333 2020-02-14 13:15:08.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/forms.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.958262 localcosmos_server-0.9.3/localcosmos_server/datasets/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     4026 2020-08-28 07:52:24.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2020-08-28 07:52:24.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)    18054 2020-08-28 07:52:24.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/models.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.950262 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.958262 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.958262 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/ajax/
--rw-r--r--   0 tom       (1000) tom       (1000)     1170 2020-08-28 07:52:24.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/ajax/dataset_box.html
--rw-r--r--   0 tom       (1000) tom       (1000)      277 2019-09-30 12:06:50.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/ajax/dataset_review_box.html
--rw-r--r--   0 tom       (1000) tom       (1000)     4532 2020-04-03 11:31:02.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/dataset_validation_routine.html
--rw-r--r--   0 tom       (1000) tom       (1000)      751 2019-11-19 12:33:10.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/edit_dataset.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1173 2020-04-03 11:31:34.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/list_datasets.html
--rw-r--r--   0 tom       (1000) tom       (1000)      891 2020-04-03 11:31:42.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/manage_dataset_validation_routine_step.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.958262 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/validation/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.958262 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/validation/ajax/
--rw-r--r--   0 tom       (1000) tom       (1000)     1185 2020-04-03 11:33:10.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/validation/ajax/dataset_form.html
--rw-r--r--   0 tom       (1000) tom       (1000)      342 2020-04-03 11:33:18.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/validation/ajax/delete_dataset.html
--rw-r--r--   0 tom       (1000) tom       (1000)      308 2020-04-03 11:33:24.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/validation/ajax/delete_dataset_image.html
--rw-r--r--   0 tom       (1000) tom       (1000)      372 2019-09-26 12:13:34.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/validation/ajax/large_modal_image.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1050 2020-04-03 11:33:42.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/validation/ajax/picture_field_images.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2424 2020-04-03 11:32:44.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/validation/expert_review.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.962262 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/widgets/
--rw-r--r--   0 tom       (1000) tom       (1000)     2070 2019-09-24 06:27:46.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/widgets/mobile_number_input.html
--rw-r--r--   0 tom       (1000) tom       (1000)    10059 2020-01-21 07:06:50.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/widgets/mobile_position_input.html
--rw-r--r--   0 tom       (1000) tom       (1000)      952 2020-04-03 11:34:44.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/widgets/picture_widget.html
--rw-r--r--   0 tom       (1000) tom       (1000)     3430 2019-10-09 12:40:06.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/widgets/select_datetime_widget.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1917 2019-10-01 06:38:48.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/urls.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.962262 localcosmos_server-0.9.3/localcosmos_server/datasets/validation/
--rw-r--r--   0 tom       (1000) tom       (1000)       72 2019-09-24 08:34:36.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/validation/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4704 2020-04-03 11:10:18.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/validation/base.py
--rw-r--r--   0 tom       (1000) tom       (1000)      482 2019-12-10 08:06:58.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/validation/forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1583 2020-04-03 11:11:28.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/validation/validators.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10209 2020-04-03 11:11:56.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8936 2019-09-26 07:22:28.000000 localcosmos_server-0.9.3/localcosmos_server/datasets/widgets.py
--rw-r--r--   0 tom       (1000) tom       (1000)      335 2019-03-14 15:26:54.000000 localcosmos_server-0.9.3/localcosmos_server/decorators.py
--rw-r--r--   0 tom       (1000) tom       (1000)      693 2019-09-20 10:46:38.000000 localcosmos_server-0.9.3/localcosmos_server/fields.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7092 2022-04-29 07:48:12.000000 localcosmos_server-0.9.3/localcosmos_server/forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1586 2019-09-23 14:42:28.000000 localcosmos_server-0.9.3/localcosmos_server/generic_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2414 2020-04-24 07:10:36.000000 localcosmos_server-0.9.3/localcosmos_server/global_urls.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.962262 localcosmos_server-0.9.3/localcosmos_server/google_cloud_api/
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2019-09-03 06:59:12.000000 localcosmos_server-0.9.3/localcosmos_server/google_cloud_api/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      162 2019-09-03 07:37:06.000000 localcosmos_server-0.9.3/localcosmos_server/google_cloud_api/serializers.py
--rw-r--r--   0 tom       (1000) tom       (1000)      349 2019-09-03 07:44:40.000000 localcosmos_server-0.9.3/localcosmos_server/google_cloud_api/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1888 2019-09-03 07:50:26.000000 localcosmos_server-0.9.3/localcosmos_server/google_cloud_api/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.950262 localcosmos_server-0.9.3/localcosmos_server/locale/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.950262 localcosmos_server-0.9.3/localcosmos_server/locale/de/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.962262 localcosmos_server-0.9.3/localcosmos_server/locale/de/LC_MESSAGES/
--rw-r--r--   0 tom       (1000) tom       (1000)    25465 2020-04-24 08:34:34.000000 localcosmos_server-0.9.3/localcosmos_server/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 tom       (1000) tom       (1000)    47980 2020-04-24 08:34:12.000000 localcosmos_server-0.9.3/localcosmos_server/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.950262 localcosmos_server-0.9.3/localcosmos_server/locale/en/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.962262 localcosmos_server-0.9.3/localcosmos_server/locale/en/LC_MESSAGES/
--rw-r--r--   0 tom       (1000) tom       (1000)      380 2020-04-24 08:34:34.000000 localcosmos_server-0.9.3/localcosmos_server/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 tom       (1000) tom       (1000)    37743 2020-04-24 08:32:22.000000 localcosmos_server-0.9.3/localcosmos_server/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 tom       (1000) tom       (1000)     1776 2020-04-25 08:33:16.000000 localcosmos_server-0.9.3/localcosmos_server/mails.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.962262 localcosmos_server-0.9.3/localcosmos_server/management/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2016-11-15 14:26:24.000000 localcosmos_server-0.9.3/localcosmos_server/management/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.962262 localcosmos_server-0.9.3/localcosmos_server/management/commands/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2016-11-15 14:26:24.000000 localcosmos_server-0.9.3/localcosmos_server/management/commands/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      775 2020-04-22 10:01:14.000000 localcosmos_server-0.9.3/localcosmos_server/management/commands/enable_staging_domain.py
--rw-r--r--   0 tom       (1000) tom       (1000)      931 2019-11-25 11:16:42.000000 localcosmos_server-0.9.3/localcosmos_server/middleware.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.962262 localcosmos_server-0.9.3/localcosmos_server/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     7449 2020-08-28 07:52:24.000000 localcosmos_server-0.9.3/localcosmos_server/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2020-08-28 07:52:24.000000 localcosmos_server-0.9.3/localcosmos_server/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)    19755 2020-08-28 07:52:24.000000 localcosmos_server-0.9.3/localcosmos_server/models.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.966262 localcosmos_server-0.9.3/localcosmos_server/online_content/
--rw-r--r--   0 tom       (1000) tom       (1000)    10003 2020-11-20 08:22:30.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/CMSObjects.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2019-03-25 10:52:36.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2019-03-25 10:52:36.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/admin.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.966262 localcosmos_server-0.9.3/localcosmos_server/online_content/api/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2019-03-25 10:52:36.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/api/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      418 2019-03-28 11:44:06.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/api/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5654 2020-01-15 07:58:08.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/api/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)      102 2019-04-02 14:43:56.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2232 2019-12-10 08:08:02.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/fields.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7707 2020-12-07 09:08:14.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/forms.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.966262 localcosmos_server-0.9.3/localcosmos_server/online_content/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)    10880 2020-08-28 07:52:24.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2020-08-28 07:52:24.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1230 2020-01-15 10:12:28.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)    39464 2020-08-28 07:52:24.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/models.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2618 2020-11-19 14:08:36.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/parser.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.950262 localcosmos_server-0.9.3/localcosmos_server/online_content/static/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.966262 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.974262 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/
--rw-r--r--   0 tom       (1000) tom       (1000)     1297 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/LICENSE.md
--rw-r--r--   0 tom       (1000) tom       (1000)      424 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/README.md
--rw-r--r--   0 tom       (1000) tom       (1000)   617478 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/ckeditor.js
--rw-r--r--   0 tom       (1000) tom       (1000)  4144258 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/ckeditor.js.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5597 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/index.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.974262 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/
--rw-r--r--   0 tom       (1000) tom       (1000)     1297 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/LICENSE.md
--rw-r--r--   0 tom       (1000) tom       (1000)      424 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/README.md
--rw-r--r--   0 tom       (1000) tom       (1000)   433388 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/ckeditor.js
--rw-r--r--   0 tom       (1000) tom       (1000)  2837712 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/ckeditor.js.map
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.982262 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/
--rw-r--r--   0 tom       (1000) tom       (1000)      797 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ar.js
--rw-r--r--   0 tom       (1000) tom       (1000)      804 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ast.js
--rw-r--r--   0 tom       (1000) tom       (1000)      764 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/bg.js
--rw-r--r--   0 tom       (1000) tom       (1000)      835 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/cs.js
--rw-r--r--   0 tom       (1000) tom       (1000)      778 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/da.js
--rw-r--r--   0 tom       (1000) tom       (1000)      861 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/de.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1122 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/el.js
--rw-r--r--   0 tom       (1000) tom       (1000)      727 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/en-au.js
--rw-r--r--   0 tom       (1000) tom       (1000)      786 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/eo.js
--rw-r--r--   0 tom       (1000) tom       (1000)      900 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/es.js
--rw-r--r--   0 tom       (1000) tom       (1000)      810 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/et.js
--rw-r--r--   0 tom       (1000) tom       (1000)      839 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/eu.js
--rw-r--r--   0 tom       (1000) tom       (1000)      787 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/fi.js
--rw-r--r--   0 tom       (1000) tom       (1000)      836 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/fr.js
--rw-r--r--   0 tom       (1000) tom       (1000)      884 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/gl.js
--rw-r--r--   0 tom       (1000) tom       (1000)      838 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/gu.js
--rw-r--r--   0 tom       (1000) tom       (1000)      790 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/hr.js
--rw-r--r--   0 tom       (1000) tom       (1000)      844 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/hu.js
--rw-r--r--   0 tom       (1000) tom       (1000)      956 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/it.js
--rw-r--r--   0 tom       (1000) tom       (1000)      957 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ja.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1517 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/km.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1392 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/kn.js
--rw-r--r--   0 tom       (1000) tom       (1000)      770 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ko.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1330 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ku.js
--rw-r--r--   0 tom       (1000) tom       (1000)      793 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/nb.js
--rw-r--r--   0 tom       (1000) tom       (1000)      863 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ne.js
--rw-r--r--   0 tom       (1000) tom       (1000)      831 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/nl.js
--rw-r--r--   0 tom       (1000) tom       (1000)      731 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/oc.js
--rw-r--r--   0 tom       (1000) tom       (1000)      787 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/pl.js
--rw-r--r--   0 tom       (1000) tom       (1000)      862 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/pt-br.js
--rw-r--r--   0 tom       (1000) tom       (1000)      843 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/pt.js
--rw-r--r--   0 tom       (1000) tom       (1000)      907 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ro.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1407 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ru.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1007 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/si.js
--rw-r--r--   0 tom       (1000) tom       (1000)      847 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/sk.js
--rw-r--r--   0 tom       (1000) tom       (1000)      856 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/sq.js
--rw-r--r--   0 tom       (1000) tom       (1000)      752 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/sv.js
--rw-r--r--   0 tom       (1000) tom       (1000)      861 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/tr.js
--rw-r--r--   0 tom       (1000) tom       (1000)      744 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/tt.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1155 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ug.js
--rw-r--r--   0 tom       (1000) tom       (1000)      972 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/uk.js
--rw-r--r--   0 tom       (1000) tom       (1000)      772 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/zh-cn.js
--rw-r--r--   0 tom       (1000) tom       (1000)      750 2018-05-22 14:15:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/zh.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.950262 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.982262 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/css/
--rw-r--r--   0 tom       (1000) tom       (1000)     9675 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/css/sample.css
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.982262 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/
--rw-r--r--   0 tom       (1000) tom       (1000)     6777 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/bg.png
--rw-r--r--   0 tom       (1000) tom       (1000)      937 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/github.svg
--rw-r--r--   0 tom       (1000) tom       (1000)    10702 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/logo.svg
--rw-r--r--   0 tom       (1000) tom       (1000)    51250 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/umbrellas.jpg
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.990261 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/
--rw-r--r--   0 tom       (1000) tom       (1000)     1818 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/af.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2255 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ar.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1881 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ast.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2177 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/az.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1835 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/bg.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1822 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ca.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2184 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/cs.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1953 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/da.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1877 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/de-ch.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2190 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/de.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2222 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/el.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1798 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/en-au.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1798 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/en-gb.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1865 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/eo.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2326 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/es.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2084 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/et.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1916 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/eu.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2921 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/fa.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1979 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/fi.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2326 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/fr.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2267 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/gl.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1909 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/gu.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2295 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/he.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2011 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/hr.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2176 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/hu.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1917 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/id.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2401 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/it.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2122 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ja.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2593 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/km.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2501 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/kn.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1850 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ko.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3343 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ku.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2210 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/lt.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2215 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/lv.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1796 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ms.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1920 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/nb.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4657 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ne.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2079 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/nl.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2089 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/no.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1802 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/oc.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2258 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/pl.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2152 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/pt-br.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1922 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/pt.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2123 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ro.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3398 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ru.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2078 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/si.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2129 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sk.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1835 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sl.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2004 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sq.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2055 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sr-latn.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3137 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sr.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1829 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sv.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2949 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/th.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2116 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/tr.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1815 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/tt.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2243 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ug.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3661 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/uk.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2351 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/vi.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1854 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/zh-cn.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1755 2020-03-24 14:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/zh.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1547 2019-04-02 13:59:36.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/online_content.css
--rw-r--r--   0 tom       (1000) tom       (1000)     2405 2018-11-26 15:24:22.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/online_content.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.950262 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.990261 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.990261 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/ajax/
--rw-r--r--   0 tom       (1000) tom       (1000)     1537 2020-04-03 11:38:50.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/ajax/image_microcontent_form.html
--rw-r--r--   0 tom       (1000) tom       (1000)       92 2018-12-24 09:28:26.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/ajax/reloaded_file_fields.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1146 2022-01-10 08:32:52.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/ajax/unpublish_template_content.html
--rw-r--r--   0 tom       (1000) tom       (1000)      997 2020-04-28 13:23:38.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/ajax/upload_custom_template.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1124 2020-04-03 11:35:30.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/ajax_filecontent_field.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.990261 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/ckeditor/
--rw-r--r--   0 tom       (1000) tom       (1000)      424 2020-04-16 06:22:46.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/ckeditor/layout-complex.js
--rw-r--r--   0 tom       (1000) tom       (1000)       55 2020-12-01 11:36:38.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/ckeditor/layout-simple.js
--rw-r--r--   0 tom       (1000) tom       (1000)      225 2018-07-04 15:11:50.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/content_managing_js.html
--rw-r--r--   0 tom       (1000) tom       (1000)      999 2020-04-28 13:01:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/create_template_content.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1533 2020-04-03 11:35:54.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/delete_microcontent.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1404 2020-12-07 07:35:42.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/filecontent_field.html
--rw-r--r--   0 tom       (1000) tom       (1000)      370 2018-07-04 15:23:04.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/filecontent_field_form.html
--rw-r--r--   0 tom       (1000) tom       (1000)     6856 2020-04-03 11:37:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/manage_template_content.html
--rw-r--r--   0 tom       (1000) tom       (1000)      758 2018-07-09 13:15:48.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/manage_template_content_extra_scripts.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2047 2019-10-09 12:21:00.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/online_content_base.html
--rw-r--r--   0 tom       (1000) tom       (1000)     4141 2020-04-03 11:38:10.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/template_content_list_entry.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1223 2020-04-03 11:38:20.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/textcontent_field.html
--rw-r--r--   0 tom       (1000) tom       (1000)     3539 2019-10-15 09:39:40.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/translate_template_content.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.994261 localcosmos_server-0.9.3/localcosmos_server/online_content/templatetags/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2018-06-01 14:17:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templatetags/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8634 2019-10-01 09:13:46.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/templatetags/online_content_tags.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3011 2020-04-28 12:13:16.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)      171 2020-04-28 11:55:50.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/utils.py
--rw-r--r--   0 tom       (1000) tom       (1000)    32882 2021-08-13 07:39:28.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3456 2019-11-18 14:41:48.000000 localcosmos_server-0.9.3/localcosmos_server/online_content/widgets.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1883 2019-10-01 13:22:14.000000 localcosmos_server-0.9.3/localcosmos_server/permission_rules.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.994261 localcosmos_server-0.9.3/localcosmos_server/server_control_panel/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2019-10-02 08:02:42.000000 localcosmos_server-0.9.3/localcosmos_server/server_control_panel/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2019-10-02 08:02:42.000000 localcosmos_server-0.9.3/localcosmos_server/server_control_panel/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      113 2019-10-02 08:02:42.000000 localcosmos_server-0.9.3/localcosmos_server/server_control_panel/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)      751 2020-04-03 11:15:28.000000 localcosmos_server-0.9.3/localcosmos_server/server_control_panel/forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)      940 2020-01-14 07:35:28.000000 localcosmos_server-0.9.3/localcosmos_server/server_control_panel/middleware.py
--rw-r--r--   0 tom       (1000) tom       (1000)       57 2019-10-02 08:02:42.000000 localcosmos_server-0.9.3/localcosmos_server/server_control_panel/models.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.950262 localcosmos_server-0.9.3/localcosmos_server/server_control_panel/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.994261 localcosmos_server-0.9.3/localcosmos_server/server_control_panel/templates/server_control_panel/
--rw-r--r--   0 tom       (1000) tom       (1000)      200 2019-10-09 12:05:02.000000 localcosmos_server-0.9.3/localcosmos_server/server_control_panel/templates/server_control_panel/app_api_status.html
--rw-r--r--   0 tom       (1000) tom       (1000)     3773 2020-04-03 11:39:44.000000 localcosmos_server-0.9.3/localcosmos_server/server_control_panel/templates/server_control_panel/base.html
--rw-r--r--   0 tom       (1000) tom       (1000)      750 2020-04-03 11:39:56.000000 localcosmos_server-0.9.3/localcosmos_server/server_control_panel/templates/server_control_panel/edit_app.html
--rw-r--r--   0 tom       (1000) tom       (1000)     4777 2020-04-03 11:41:06.000000 localcosmos_server-0.9.3/localcosmos_server/server_control_panel/templates/server_control_panel/home.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2508 2020-04-03 11:41:54.000000 localcosmos_server-0.9.3/localcosmos_server/server_control_panel/templates/server_control_panel/install_app.html
--rw-r--r--   0 tom       (1000) tom       (1000)      642 2019-11-18 13:51:32.000000 localcosmos_server-0.9.3/localcosmos_server/server_control_panel/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9781 2020-08-28 07:52:24.000000 localcosmos_server-0.9.3/localcosmos_server/server_control_panel/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1902 2020-04-06 07:19:42.000000 localcosmos_server-0.9.3/localcosmos_server/settings.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1480 2020-04-03 11:16:36.000000 localcosmos_server-0.9.3/localcosmos_server/setup_forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)      212 2019-11-11 14:22:30.000000 localcosmos_server-0.9.3/localcosmos_server/setup_urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1209 2019-11-11 14:29:58.000000 localcosmos_server-0.9.3/localcosmos_server/setup_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)      663 2018-10-17 12:26:46.000000 localcosmos_server-0.9.3/localcosmos_server/slugifier.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.994261 localcosmos_server-0.9.3/localcosmos_server/specifications/
--rw-r--r--   0 tom       (1000) tom       (1000)      650 2018-02-05 08:52:22.000000 localcosmos_server-0.9.3/localcosmos_server/specifications/DatasetJSON
--rw-r--r--   0 tom       (1000) tom       (1000)      457 2020-08-28 07:52:24.000000 localcosmos_server-0.9.3/localcosmos_server/specifications/TaxonJSON
--rw-r--r--   0 tom       (1000) tom       (1000)      277 2019-11-11 08:46:16.000000 localcosmos_server-0.9.3/localcosmos_server/specifications/TemporalJSON
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.994261 localcosmos_server-0.9.3/localcosmos_server/static/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.994261 localcosmos_server-0.9.3/localcosmos_server/static/fonts/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.994261 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Indie_Flower/
--rw-r--r--   0 tom       (1000) tom       (1000)    55300 2011-03-08 22:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Indie_Flower/IndieFlower-Regular.ttf
--rw-r--r--   0 tom       (1000) tom       (1000)    30372 2019-12-09 08:25:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Indie_Flower/IndieFlower-Regular.woff
--rw-r--r--   0 tom       (1000) tom       (1000)     4455 2011-03-08 22:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Indie_Flower/OFL.txt
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.018261 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/
--rw-r--r--   0 tom       (1000) tom       (1000)    11560 2013-01-08 22:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/LICENSE.txt
--rw-r--r--   0 tom       (1000) tom       (1000)   171072 2013-01-08 22:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0 tom       (1000) tom       (1000)    90428 2019-12-09 08:17:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Black.woff
--rw-r--r--   0 tom       (1000) tom       (1000)   177120 2013-01-08 22:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0 tom       (1000) tom       (1000)    98056 2019-12-09 08:17:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-BlackItalic.woff
--rw-r--r--   0 tom       (1000) tom       (1000)   170348 2013-01-08 22:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0 tom       (1000) tom       (1000)    90080 2019-12-09 08:17:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Bold.woff
--rw-r--r--   0 tom       (1000) tom       (1000)   174520 2013-01-08 22:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0 tom       (1000) tom       (1000)    96000 2019-12-09 08:17:48.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-BoldItalic.woff
--rw-r--r--   0 tom       (1000) tom       (1000)   173516 2013-01-08 22:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0 tom       (1000) tom       (1000)    95508 2019-12-09 08:17:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Italic.woff
--rw-r--r--   0 tom       (1000) tom       (1000)   170012 2013-01-08 22:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0 tom       (1000) tom       (1000)    89436 2019-12-09 08:18:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Light.woff
--rw-r--r--   0 tom       (1000) tom       (1000)   176184 2013-01-08 22:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0 tom       (1000) tom       (1000)    96712 2019-12-09 08:18:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-LightItalic.woff
--rw-r--r--   0 tom       (1000) tom       (1000)   171656 2013-01-08 22:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0 tom       (1000) tom       (1000)    90328 2019-12-09 08:18:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Medium.woff
--rw-r--r--   0 tom       (1000) tom       (1000)   176428 2013-01-08 22:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0 tom       (1000) tom       (1000)    97232 2019-12-09 08:18:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-MediumItalic.woff
--rw-r--r--   0 tom       (1000) tom       (1000)   171272 2013-01-08 22:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0 tom       (1000) tom       (1000)    89596 2019-12-09 08:18:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Regular.woff
--rw-r--r--   0 tom       (1000) tom       (1000)   171500 2013-01-08 22:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0 tom       (1000) tom       (1000)    87896 2019-12-09 08:18:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Thin.woff
--rw-r--r--   0 tom       (1000) tom       (1000)   175872 2013-01-08 22:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0 tom       (1000) tom       (1000)    94564 2019-12-09 08:18:36.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-ThinItalic.woff
--rw-r--r--   0 tom       (1000) tom       (1000)     6404 2019-12-09 08:26:44.000000 localcosmos_server-0.9.3/localcosmos_server/static/fonts/fonts.css
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.018261 localcosmos_server-0.9.3/localcosmos_server/static/images/
--rw-r--r--   0 tom       (1000) tom       (1000)     1000 2019-02-26 09:32:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/images/lclogo32.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1752 2020-04-23 06:44:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/images/local_cosmos_logo_40.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4881 2019-01-29 08:57:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/images/local_cosmos_logo_horizontal.png
--rw-r--r--   0 tom       (1000) tom       (1000)    32016 2019-09-02 13:08:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/images/spinner.gif
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.018261 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.950262 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.026261 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/
--rw-r--r--   0 tom       (1000) tom       (1000)    64548 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-grid.css
--rw-r--r--   0 tom       (1000) tom       (1000)   151749 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-grid.css.map
--rw-r--r--   0 tom       (1000) tom       (1000)    48488 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css
--rw-r--r--   0 tom       (1000) tom       (1000)   108539 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4897 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-reboot.css
--rw-r--r--   0 tom       (1000) tom       (1000)    76483 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-reboot.css.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4021 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css
--rw-r--r--   0 tom       (1000) tom       (1000)    32461 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 tom       (1000) tom       (1000)   192348 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap.css
--rw-r--r--   0 tom       (1000) tom       (1000)   492048 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap.css.map
--rw-r--r--   0 tom       (1000) tom       (1000)   155758 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap.min.css
--rw-r--r--   0 tom       (1000) tom       (1000)   625953 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap.min.css.map
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.038261 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/
--rw-r--r--   0 tom       (1000) tom       (1000)   222911 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.bundle.js
--rw-r--r--   0 tom       (1000) tom       (1000)   402249 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.bundle.js.map
--rw-r--r--   0 tom       (1000) tom       (1000)    78635 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js
--rw-r--r--   0 tom       (1000) tom       (1000)   311949 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 tom       (1000) tom       (1000)   131637 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.js
--rw-r--r--   0 tom       (1000) tom       (1000)   250568 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.js.map
--rw-r--r--   0 tom       (1000) tom       (1000)    58072 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.min.js
--rw-r--r--   0 tom       (1000) tom       (1000)   190253 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.min.js.map
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.038261 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/css/
--rw-r--r--   0 tom       (1000) tom       (1000)     1928 2022-04-25 10:19:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/css/localcosmos_server.css
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.038261 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/
--rw-r--r--   0 tom       (1000) tom       (1000)     7912 2016-11-06 13:33:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/Local-Cosmos-Logo.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2837 2018-07-09 07:40:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/add_image.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     1072 2022-04-20 09:47:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/arrow-tool-add.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4408 2022-04-20 10:19:51.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/arrow-tool-add.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      900 2022-04-20 09:48:47.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/arrow-tool-remove.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3934 2022-04-20 10:19:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/arrow-tool-remove.svg
--rw-------   0 tom       (1000) tom       (1000)      797 2022-04-19 08:28:51.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/arrow-tool.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3448 2022-04-19 08:29:01.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/arrow-tool.svg
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.058260 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/
--rw-r--r--   0 tom       (1000) tom       (1000)      171 2013-02-13 14:59:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/00.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ad.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ae.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/af.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ag.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ai.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/al.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 14:59:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/am.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/an.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      244 2013-02-13 14:59:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ao.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ar.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 15:00:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/as.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 14:59:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/at.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      378 2013-02-13 15:00:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/au.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 15:00:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/aw.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      376 2013-02-13 15:00:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ax.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/az.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ba.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 14:59:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/bb.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/bd.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 14:59:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/be.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      358 2013-02-13 14:59:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/bf.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/bg.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/bh.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      374 2013-02-13 15:00:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/bi.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/bj.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/bm.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      373 2013-02-13 15:00:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/bn.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 15:00:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/bo.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/br.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      351 2013-02-13 15:00:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/bs.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      377 2013-02-13 15:00:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/bt.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      376 2013-02-13 15:00:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/bv.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/bw.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/by.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/bz.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      376 2013-02-13 14:59:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ca.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      238 2013-02-13 14:59:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/catalonia.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/cc.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      243 2013-02-13 15:00:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/cd.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/cf.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 15:00:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/cg.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      332 2013-02-13 15:00:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ch.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 14:59:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ci.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ck.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/cl.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/cm.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/cn.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      353 2013-02-13 14:59:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/co.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 15:00:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/cr.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 14:59:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/cs.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 14:59:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/cu.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/cv.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 14:59:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/cx.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 14:59:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/cy.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/cz.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/de.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/dj.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      374 2013-02-13 14:59:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/dk.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/dm.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 14:59:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/do.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/dz.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ec.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ee.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/eg.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 15:00:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/eh.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      260 2013-02-13 14:59:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/en.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/england.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/er.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/es.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/et.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      171 2013-02-13 15:00:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/europeanunion.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/fam.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/fi.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/fj.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      372 2013-02-13 15:00:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/fk.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      377 2013-02-13 15:00:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/fm.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/fo.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/fr.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 15:00:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ga.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      260 2013-02-13 15:00:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/gb.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/gd.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      379 2013-02-13 15:00:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ge.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/gf.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      358 2013-02-13 15:00:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/gh.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 14:59:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/gi.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/gl.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/gm.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/gn.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      357 2013-02-13 15:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/gp.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/gq.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/gr.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 14:59:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/gs.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      374 2013-02-13 15:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/gt.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/gu.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      358 2013-02-13 14:59:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/gw.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/gy.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      373 2013-02-13 15:00:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/hk.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      378 2013-02-13 15:00:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/hm.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/hn.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/hr.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ht.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      357 2013-02-13 15:00:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/hu.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/id.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ie.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/il.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 14:59:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/in.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      373 2013-02-13 15:00:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/io.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/iq.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ir.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      373 2013-02-13 15:00:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/is.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/it.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ja.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 15:00:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/jm.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/jo.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/jp.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ke.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      373 2013-02-13 15:00:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/kg.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 14:59:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/kh.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 14:59:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ki.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      358 2013-02-13 15:00:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/km.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/kn.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/kp.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      385 2013-02-13 15:00:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/kr.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/kw.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      373 2013-02-13 15:00:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ky.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      374 2013-02-13 15:00:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/kz.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/la.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/lb.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      259 2013-02-13 15:00:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/lc.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 15:00:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/li.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      377 2013-02-13 15:00:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/lk.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/lr.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 14:59:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ls.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/lt.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/lu.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/lv.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ly.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ma.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 15:00:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/mc.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/md.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      238 2013-02-13 15:00:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/me.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      372 2013-02-13 15:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/mg.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/mh.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      382 2013-02-13 15:00:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/mk.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ml.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 15:00:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/mm.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 14:59:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/mn.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      378 2013-02-13 15:00:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/mo.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/mp.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      379 2013-02-13 15:00:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/mq.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      377 2013-02-13 15:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/mr.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 14:59:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ms.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/mt.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      358 2013-02-13 15:00:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/mu.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      372 2013-02-13 15:00:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/mv.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/mw.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/mx.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      375 2013-02-13 15:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/my.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/mz.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/na.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/nc.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ne.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      375 2013-02-13 14:59:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/nf.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ng.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ni.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/nl.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      376 2013-02-13 15:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/no.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      302 2013-02-13 15:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/np.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/nr.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/nu.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/nz.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/om.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/pa.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/pe.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/pf.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/pg.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ph.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      377 2013-02-13 14:59:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/pk.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 14:59:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/pl.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      374 2013-02-13 15:00:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/pm.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/pn.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/pr.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      358 2013-02-13 15:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ps.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/pt.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      374 2013-02-13 15:00:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/pw.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/py.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 14:59:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/qa.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/re.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ro.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      238 2013-02-13 15:00:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/rs.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 14:59:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ru.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 14:59:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/rw.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 14:59:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/sa.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/sb.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      357 2013-02-13 15:00:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/sc.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      378 2013-02-13 14:59:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/scotland.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      355 2013-02-13 15:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/sd.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/se.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/sg.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/sh.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/si.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      376 2013-02-13 15:00:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/sj.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/sk.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 14:59:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/sl.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/sm.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/sn.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      376 2013-02-13 14:59:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/so.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/sr.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 14:59:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/st.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/sv.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/sy.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/sz.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/tc.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/td.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 15:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/tf.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/tg.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/th.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/tj.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      372 2013-02-13 15:00:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/tk.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/tl.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 14:59:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/tm.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      375 2013-02-13 15:00:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/tn.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/to.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/tr.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      377 2013-02-13 15:00:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/tt.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/tv.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/tw.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/tz.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ua.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 14:59:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ug.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/um.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 14:59:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/us.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      373 2013-02-13 15:00:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/uy.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 14:59:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/uz.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/va.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 14:59:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/vc.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ve.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/vg.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      376 2013-02-13 15:00:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/vi.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/vn.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 15:00:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/vu.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      372 2013-02-13 15:00:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/wales.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      377 2013-02-13 15:00:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/wf.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 15:00:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ws.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      356 2013-02-13 14:59:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/ye.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      382 2013-02-13 15:00:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/yt.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/za.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      358 2013-02-13 15:00:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/zm.gif
--rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 15:00:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries/zw.gif
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.082260 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/
--rw-r--r--   0 tom       (1000) tom       (1000)     1933 2007-06-16 07:58:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_ASEAN.png
--rw-r--r--   0 tom       (1000) tom       (1000)      959 2007-06-16 07:58:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_African Union(OAS).png
--rw-r--r--   0 tom       (1000) tom       (1000)     2506 2007-06-16 07:58:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Arab League.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1888 2007-06-16 07:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_CARICOM.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2397 2007-06-16 07:58:46.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_CIS.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2387 2007-06-16 07:58:48.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Commonwealth.png
--rw-r--r--   0 tom       (1000) tom       (1000)      636 2007-06-16 07:58:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_England.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1847 2007-06-16 07:59:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_European Union.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2312 2007-06-16 07:59:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Islamic Conference.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1766 2008-07-16 19:21:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Kosovo.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1671 2007-06-16 07:59:44.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_NATO.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1202 2007-06-16 07:59:48.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Northern Cyprus.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1169 2007-06-19 18:05:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Northern Ireland.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1757 2007-06-16 07:59:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_OPEC.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4432 2008-11-02 15:41:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Olimpic Movement.png
--rw-r--r--   0 tom       (1000) tom       (1000)      501 2007-06-16 08:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Red Cross.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2434 2007-06-16 08:00:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Scotland.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1290 2007-06-16 08:00:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Somaliland.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2278 2007-06-16 08:01:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_United Nations.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2958 2007-06-16 08:01:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Wales.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1544 2007-06-16 07:58:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ad.png
--rw-r--r--   0 tom       (1000) tom       (1000)      837 2007-06-16 08:01:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ae.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2155 2007-06-16 07:58:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/af.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2089 2007-06-16 07:58:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ag.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2619 2007-06-19 09:59:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ai.png
--rw-r--r--   0 tom       (1000) tom       (1000)      787 2007-06-16 07:58:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/am.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1125 2007-10-11 14:48:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/an.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1540 2007-06-16 07:58:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ao.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1669 2007-06-16 07:58:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/aq.png
--rw-r--r--   0 tom       (1000) tom       (1000)      839 2007-06-16 07:58:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ar.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2554 2007-06-16 07:58:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/as.png
--rw-r--r--   0 tom       (1000) tom       (1000)      628 2007-06-16 07:58:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/at.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2623 2007-06-19 09:54:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/au.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1066 2007-06-16 07:58:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/aw.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1201 2007-06-16 07:58:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/az.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2343 2007-06-16 07:58:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ba.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1505 2007-06-16 07:58:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bb.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1447 2007-06-16 07:58:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bd.png
--rw-r--r--   0 tom       (1000) tom       (1000)      887 2007-06-16 07:58:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/be.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1071 2007-06-16 07:58:40.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bf.png
--rw-r--r--   0 tom       (1000) tom       (1000)      624 2007-06-16 07:58:40.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bg.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1256 2007-06-16 07:58:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bh.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2628 2007-06-16 07:58:40.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bi.png
--rw-r--r--   0 tom       (1000) tom       (1000)      773 2007-06-16 07:58:36.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bj.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2552 2007-10-11 14:37:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bm.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2408 2007-06-16 07:58:40.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bn.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1244 2007-06-16 07:58:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bo.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2549 2007-06-16 07:58:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/br.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1257 2007-06-16 07:58:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bs.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2351 2007-06-16 07:58:36.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bt.png
--rw-r--r--   0 tom       (1000) tom       (1000)      752 2007-06-16 07:58:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bw.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1467 2007-06-16 07:58:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/by.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2193 2007-06-16 07:58:36.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bz.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1484 2007-06-16 07:58:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ca.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2469 2007-06-16 07:58:48.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cd.png
--rw-r--r--   0 tom       (1000) tom       (1000)      986 2007-06-16 07:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cf.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1720 2007-06-16 07:58:48.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cg.png
--rw-r--r--   0 tom       (1000) tom       (1000)      828 2007-06-16 08:00:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ch.png
--rw-r--r--   0 tom       (1000) tom       (1000)      782 2007-06-16 07:58:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ci.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2683 2007-10-11 14:38:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ck.png
--rw-r--r--   0 tom       (1000) tom       (1000)      820 2007-06-16 07:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cl.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1131 2007-06-16 07:58:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cm.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1063 2007-06-16 07:58:46.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cn.png
--rw-r--r--   0 tom       (1000) tom       (1000)      676 2007-06-16 07:58:46.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/co.png
--rw-r--r--   0 tom       (1000) tom       (1000)      721 2007-06-16 07:58:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1508 2007-06-16 07:58:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cu.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1299 2007-06-16 07:58:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cv.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1125 2007-06-16 07:58:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cy.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1295 2007-06-16 07:58:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cz.png
--rw-r--r--   0 tom       (1000) tom       (1000)      809 2007-06-16 07:58:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/da.png
--rw-r--r--   0 tom       (1000) tom       (1000)      808 2007-06-16 07:59:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/de.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1456 2007-06-16 07:58:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/dj.png
--rw-r--r--   0 tom       (1000) tom       (1000)      809 2007-06-16 07:58:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/dk.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1946 2007-06-16 07:58:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/dm.png
--rw-r--r--   0 tom       (1000) tom       (1000)      830 2007-06-16 07:58:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/do.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1445 2007-06-16 07:58:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/dz.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1628 2007-06-16 07:58:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ec.png
--rw-r--r--   0 tom       (1000) tom       (1000)      781 2007-06-16 07:58:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ee.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1020 2007-06-16 07:58:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/eg.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1407 2007-06-16 08:01:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/eh.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2675 2007-06-16 08:01:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/en.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2588 2007-06-16 07:58:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/er.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1397 2007-06-16 08:00:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/es.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1646 2007-06-16 07:59:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/et.png
--rw-r--r--   0 tom       (1000) tom       (1000)      711 2007-06-16 07:59:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/fi.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2499 2007-06-16 07:59:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/fj.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1340 2007-06-16 07:59:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/fm.png
--rw-r--r--   0 tom       (1000) tom       (1000)      838 2007-06-16 07:59:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/fo.png
--rw-r--r--   0 tom       (1000) tom       (1000)      941 2007-06-16 07:59:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/fr.png
--rw-r--r--   0 tom       (1000) tom       (1000)      785 2007-06-16 07:59:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ga.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2675 2007-06-16 08:01:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gb.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2211 2007-06-16 07:59:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gd.png
--rw-r--r--   0 tom       (1000) tom       (1000)      841 2007-06-16 07:59:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ge.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1103 2008-07-16 18:40:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gg.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1146 2007-06-16 07:59:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gh.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1595 2007-10-11 14:39:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gi.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1206 2008-04-20 04:51:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gl.png
--rw-r--r--   0 tom       (1000) tom       (1000)      806 2007-06-16 07:59:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gm.png
--rw-r--r--   0 tom       (1000) tom       (1000)      962 2007-06-16 07:59:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gn.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1662 2008-04-20 04:56:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gp.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1569 2007-06-16 07:58:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gq.png
--rw-r--r--   0 tom       (1000) tom       (1000)      885 2007-06-16 07:59:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2038 2007-06-16 07:59:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gt.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1607 2007-10-11 14:39:46.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gu.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1121 2007-06-16 07:59:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gw.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2679 2007-06-16 07:59:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gy.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1748 2007-06-16 07:59:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/hk.png
--rw-r--r--   0 tom       (1000) tom       (1000)      955 2007-06-16 07:59:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/hn.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1319 2007-06-16 07:58:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/hr.png
--rw-r--r--   0 tom       (1000) tom       (1000)      784 2007-06-16 07:59:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ht.png
--rw-r--r--   0 tom       (1000) tom       (1000)      729 2007-06-16 07:59:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/hu.png
--rw-r--r--   0 tom       (1000) tom       (1000)      614 2007-06-16 07:59:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/id.png
--rw-r--r--   0 tom       (1000) tom       (1000)      882 2007-06-16 07:59:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ie.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1116 2007-06-16 07:59:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/il.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1660 2008-11-02 18:52:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/im.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1148 2007-06-16 07:59:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/in.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1158 2007-06-16 07:59:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/iq.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1372 2007-06-16 07:59:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ir.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1009 2007-06-16 07:59:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/is.png
--rw-r--r--   0 tom       (1000) tom       (1000)      861 2007-06-16 07:59:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/it.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1024 2007-06-16 07:59:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ja.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2382 2007-10-11 14:47:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/je.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2752 2007-06-16 07:59:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/jm.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1512 2007-06-16 07:59:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/jo.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1024 2007-06-16 07:59:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/jp.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1791 2007-06-19 17:44:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ke.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1610 2007-06-16 07:59:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/kg.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1440 2007-06-16 07:58:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/kh.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3269 2007-06-16 07:59:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ki.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1856 2007-06-16 07:58:48.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/km.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2324 2007-06-16 08:00:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/kn.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1436 2007-06-16 07:59:48.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/kp.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2129 2007-06-16 08:00:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/kr.png
--rw-r--r--   0 tom       (1000) tom       (1000)      987 2007-06-16 07:59:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/kw.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3021 2007-06-19 10:05:40.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ky.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2317 2007-06-16 07:59:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/kz.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1179 2007-06-16 07:59:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/la.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1274 2007-06-16 07:59:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/lb.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1600 2007-06-16 08:00:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/lc.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1242 2007-06-16 07:59:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/li.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2136 2007-06-16 08:00:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/lk.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1171 2007-06-16 07:59:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/lr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2216 2007-06-16 07:59:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ls.png
--rw-r--r--   0 tom       (1000) tom       (1000)      744 2007-06-16 07:59:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/lt.png
--rw-r--r--   0 tom       (1000) tom       (1000)      635 2007-06-16 07:59:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/lu.png
--rw-r--r--   0 tom       (1000) tom       (1000)      803 2007-06-16 07:59:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/lv.png
--rw-r--r--   0 tom       (1000) tom       (1000)      919 2007-06-16 07:59:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ly.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1109 2007-06-16 07:59:40.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ma.png
--rw-r--r--   0 tom       (1000) tom       (1000)      612 2007-06-16 07:59:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mc.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1655 2007-06-16 07:59:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/md.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1977 2007-06-16 07:59:40.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/me.png
--rw-r--r--   0 tom       (1000) tom       (1000)      742 2007-06-16 07:59:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mg.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2839 2007-06-16 07:59:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mh.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2996 2007-06-16 07:59:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mk.png
--rw-r--r--   0 tom       (1000) tom       (1000)      924 2007-06-16 07:59:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ml.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1631 2007-06-16 07:59:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mm.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1420 2007-06-16 07:59:40.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mn.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2333 2007-06-16 07:59:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mo.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2558 2008-04-20 04:58:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mq.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1602 2007-06-16 07:59:36.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2399 2007-10-11 14:48:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ms.png
--rw-r--r--   0 tom       (1000) tom       (1000)      869 2007-06-16 07:59:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mt.png
--rw-r--r--   0 tom       (1000) tom       (1000)      819 2007-06-16 07:59:36.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mu.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1115 2007-06-16 07:59:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mv.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1259 2007-07-06 08:48:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mw.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1555 2007-06-16 07:59:36.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mx.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1575 2007-06-16 07:59:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/my.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1733 2007-06-16 07:59:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mz.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2862 2007-06-16 07:59:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/na.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2114 2008-07-16 18:38:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/nc.png
--rw-r--r--   0 tom       (1000) tom       (1000)      878 2007-06-16 07:59:46.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ne.png
--rw-r--r--   0 tom       (1000) tom       (1000)      781 2007-06-16 07:59:48.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ng.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1026 2007-06-16 07:59:46.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ni.png
--rw-r--r--   0 tom       (1000) tom       (1000)      635 2007-06-16 07:59:44.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/nl.png
--rw-r--r--   0 tom       (1000) tom       (1000)      935 2007-06-16 07:59:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/no.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2026 2007-07-01 22:34:44.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/np.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1216 2007-06-16 07:59:44.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/nr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2182 2007-06-16 07:59:46.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/nz.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1145 2007-06-16 07:59:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/om.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1053 2007-06-16 07:59:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/pa.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1560 2007-06-16 07:59:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/pe.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1294 2007-10-11 14:39:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/pf.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2075 2007-06-16 07:59:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/pg.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1564 2007-06-16 07:59:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ph.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1448 2007-06-16 07:59:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/pk.png
--rw-r--r--   0 tom       (1000) tom       (1000)      491 2007-06-16 07:59:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/pl.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1398 2007-06-16 08:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/pr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1255 2007-06-16 07:59:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ps.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1797 2007-06-16 07:59:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/pt.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1313 2007-06-16 07:59:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/pw.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1052 2007-06-16 07:59:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/py.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1181 2007-06-16 08:00:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/qa.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1991 2008-04-20 05:02:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/re.png
--rw-r--r--   0 tom       (1000) tom       (1000)      900 2007-06-16 08:00:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ro.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1698 2007-06-16 08:00:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/rs.png
--rw-r--r--   0 tom       (1000) tom       (1000)      551 2007-06-16 08:00:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ru.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1079 2007-06-16 08:00:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/rw.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2035 2007-06-16 08:00:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sa.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2317 2007-06-16 08:00:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sb.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2177 2007-06-16 08:00:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sc.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1246 2007-06-16 08:00:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sd.png
--rw-r--r--   0 tom       (1000) tom       (1000)      906 2007-06-16 08:00:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/se.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1031 2007-06-16 08:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sg.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1041 2007-06-16 08:00:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/si.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1344 2007-06-16 08:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sk.png
--rw-r--r--   0 tom       (1000) tom       (1000)      655 2007-06-16 08:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sl.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1935 2007-06-16 08:00:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sm.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1223 2007-06-16 08:00:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sn.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1181 2007-06-16 08:00:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/so.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1747 2007-06-16 07:58:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sq.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1015 2007-06-16 08:00:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1282 2007-06-16 08:00:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/st.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1092 2007-06-16 07:58:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sv.png
--rw-r--r--   0 tom       (1000) tom       (1000)      978 2007-06-16 08:00:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sy.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2298 2007-06-16 08:00:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sz.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2503 2007-10-11 14:48:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tc.png
--rw-r--r--   0 tom       (1000) tom       (1000)      889 2007-06-16 07:58:44.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/td.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1085 2007-06-16 08:00:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tg.png
--rw-r--r--   0 tom       (1000) tom       (1000)      674 2007-06-16 08:00:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/th.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1158 2007-06-16 08:00:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tj.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1744 2007-06-16 08:00:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tl.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2070 2007-06-16 08:00:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tm.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1664 2007-06-16 08:00:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tn.png
--rw-r--r--   0 tom       (1000) tom       (1000)      787 2007-06-16 08:00:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/to.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1580 2007-06-16 08:00:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2351 2007-06-16 08:00:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tt.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2398 2007-06-16 08:00:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tv.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1309 2007-06-16 08:00:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tw.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2197 2007-06-16 08:00:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tz.png
--rw-r--r--   0 tom       (1000) tom       (1000)      737 2007-06-16 08:01:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ua.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1229 2007-06-16 08:01:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ug.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1101 2007-07-04 20:12:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/us.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1144 2007-06-16 08:01:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/uy.png
--rw-r--r--   0 tom       (1000) tom       (1000)      971 2007-06-16 08:01:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/uz.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1281 2007-06-16 08:01:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/va.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1381 2007-06-16 08:00:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/vc.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1108 2007-06-16 08:01:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ve.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2767 2007-10-11 14:37:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/vg.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2425 2007-10-11 14:48:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/vi.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1174 2007-06-16 08:01:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/vn.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2057 2007-06-16 08:01:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/vu.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1369 2007-06-16 08:00:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ws.png
--rw-r--r--   0 tom       (1000) tom       (1000)      696 2007-06-16 08:01:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ye.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2095 2007-06-16 08:00:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/za.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1209 2007-06-16 08:01:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/zm.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1746 2007-06-16 08:01:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/zw.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.130259 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/
--rw-r--r--   0 tom       (1000) tom       (1000)     4407 2008-01-09 14:16:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Algeria.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5651 2008-01-09 14:17:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/British_Virgin_Islands.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5884 2008-01-09 14:18:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Cayman_Islands.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2909 2008-01-09 14:18:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Chad.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4825 2008-01-09 14:18:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Comoros.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5032 2008-01-09 14:18:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Democratic_Republic_of_the_Congo.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4416 2008-01-09 14:19:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/French_Polynesia.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2913 2008-01-09 14:22:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Latvia.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3991 2008-01-09 14:23:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Micronesia.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3785 2008-01-09 14:24:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/North_Korea.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3797 2008-01-09 14:24:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Oman.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5479 2008-01-09 14:25:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Saint_Kitts_and_Nevis.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4012 2008-01-09 14:25:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Saint_Lucia.png
--rw-r--r--   0 tom       (1000) tom       (1000)     8662 2008-01-09 14:26:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Saint_Pierre.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3831 2008-01-09 14:26:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Saint_Vicent_and_the_Grenadines.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3592 2008-01-09 14:26:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Samoa.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3183 2008-01-09 14:27:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Soviet_Union.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5640 2008-01-09 14:27:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Sri_Lanka.png
--rw-r--r--   0 tom       (1000) tom       (1000)     8289 2008-01-09 14:28:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Tibet.png
--rw-r--r--   0 tom       (1000) tom       (1000)     6644 2008-01-09 14:28:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Tuvalu.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4421 2008-01-09 14:16:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ad.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2971 2008-01-09 14:28:44.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ae.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4786 2008-01-09 14:15:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/af.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5085 2008-01-09 14:16:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ag.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5469 2008-01-09 14:16:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ai.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5037 2008-01-09 14:15:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/al.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3002 2008-01-09 14:16:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/am.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3776 2008-01-09 14:24:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/an.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4127 2008-01-09 14:16:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ao.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3319 2008-01-09 14:16:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ar.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5785 2008-01-09 14:16:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/as.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2889 2008-01-09 14:16:36.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/at.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5985 2008-01-09 14:16:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/au.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3579 2008-01-09 14:16:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/aw.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3609 2008-01-09 14:16:40.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/az.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4854 2008-01-09 14:17:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ba.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3938 2008-01-09 14:16:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bb.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3854 2008-01-09 14:16:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bd.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2906 2008-01-09 14:17:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/be.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3349 2008-01-09 14:17:44.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bf.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2912 2008-01-09 14:17:40.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bg.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3591 2008-01-09 14:16:46.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bh.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5935 2008-01-09 14:17:48.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bi.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2958 2008-01-09 14:17:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bj.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5563 2008-01-09 14:17:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bm.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5350 2008-01-09 14:17:36.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bn.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3936 2008-01-09 14:17:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bo.png
--rw-r--r--   0 tom       (1000) tom       (1000)     6182 2008-01-09 14:17:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/br.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3563 2008-01-09 14:16:44.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bs.png
--rw-r--r--   0 tom       (1000) tom       (1000)     6629 2008-01-09 14:17:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bt.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2961 2008-01-09 14:17:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bw.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3913 2008-01-09 14:16:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/by.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5497 2008-01-09 14:17:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bz.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3895 2008-01-09 14:17:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ca.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3599 2008-01-09 14:18:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cf.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4046 2008-01-09 14:25:40.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cg.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3184 2008-01-09 14:27:46.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ch.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2894 2008-01-09 14:18:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ci.png
--rw-r--r--   0 tom       (1000) tom       (1000)     6864 2008-01-09 14:18:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ck.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3428 2008-01-09 14:18:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cl.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3314 2008-01-09 14:17:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cm.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3817 2008-01-09 14:18:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cn.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2957 2008-01-09 14:18:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/co.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2946 2008-01-09 14:18:36.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3986 2008-01-09 14:18:46.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cu.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4870 2008-01-09 14:18:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cv.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5479 2008-01-09 14:18:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cx.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3928 2008-01-09 14:18:48.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cy.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3887 2008-01-09 14:18:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cz.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2924 2008-01-09 14:20:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/de.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3823 2008-01-09 14:19:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/dj.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3045 2008-01-09 14:19:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/dk.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4408 2008-01-09 14:19:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/dm.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3053 2008-01-09 14:19:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/do.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3963 2008-01-09 14:19:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ec.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2925 2008-01-09 14:19:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ee.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3313 2008-01-09 14:19:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/eg.png
--rw-r--r--   0 tom       (1000) tom       (1000)     6236 2008-01-09 14:28:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/en.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5613 2008-01-09 14:19:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/er.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2935 2008-01-09 14:27:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/es.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3918 2008-01-09 14:19:36.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/et.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3077 2008-01-09 14:19:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/fi.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5640 2008-01-09 14:19:46.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/fj.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5688 2008-01-09 14:19:40.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/fk.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3352 2008-01-09 14:19:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/fo.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2892 2008-01-09 14:19:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/fr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2957 2008-01-09 14:20:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ga.png
--rw-r--r--   0 tom       (1000) tom       (1000)     6236 2008-01-09 14:28:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gb.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5287 2008-01-09 14:20:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gd.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4941 2008-01-09 14:20:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ge.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2892 2008-01-09 14:23:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gf.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3447 2008-01-09 14:20:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gh.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3821 2008-01-09 14:20:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gi.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3938 2008-01-09 14:20:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gl.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2935 2008-01-09 14:20:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gm.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2907 2008-01-09 14:20:40.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gn.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4360 2008-01-09 14:19:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gq.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3374 2008-01-09 14:20:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3967 2008-01-09 14:20:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gt.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4348 2008-01-09 14:20:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gu.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3281 2008-01-09 14:20:44.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gw.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5486 2008-01-09 14:20:48.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gy.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4659 2008-01-09 14:20:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/hk.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3283 2008-01-09 14:20:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/hn.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4128 2008-01-09 14:18:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/hr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2938 2008-01-09 14:20:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ht.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2894 2008-01-09 14:21:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/hu.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2881 2008-01-09 14:21:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/id.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2883 2008-01-09 14:21:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ie.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4091 2008-01-09 14:21:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/il.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3809 2008-01-09 14:21:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/in.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4008 2008-01-09 14:21:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/iq.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4982 2008-01-09 14:21:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ir.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3243 2008-01-09 14:21:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/is.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2889 2008-01-09 14:21:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/it.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4978 2008-01-09 14:21:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/jm.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3737 2008-01-09 14:21:40.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/jo.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3714 2008-01-09 14:21:36.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/jp.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4959 2008-01-09 14:21:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ke.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4575 2008-01-09 14:22:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/kg.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4819 2008-01-09 14:17:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/kh.png
--rw-r--r--   0 tom       (1000) tom       (1000)     7486 2008-01-09 14:21:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ki.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3339 2008-01-09 14:21:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/kw.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5088 2008-01-09 14:21:44.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/kz.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3667 2008-01-09 14:22:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/la.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4266 2008-01-09 14:22:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/lb.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3826 2008-01-09 14:22:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/li.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3559 2008-01-09 14:22:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/lr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5558 2008-01-09 14:22:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ls.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2945 2008-01-09 14:22:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/lt.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2904 2008-01-09 14:22:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/lu.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2873 2008-01-09 14:22:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ly.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3737 2008-01-09 14:23:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ma.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2905 2008-01-09 14:23:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mc.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4014 2008-01-09 14:23:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/md.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2928 2008-01-09 14:22:46.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mg.png
--rw-r--r--   0 tom       (1000) tom       (1000)     6053 2008-01-09 14:23:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mh.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5892 2008-01-09 14:22:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mk.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2910 2008-01-09 14:23:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ml.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4119 2008-01-09 14:23:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mm.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3552 2008-01-09 14:23:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mn.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5963 2008-01-09 14:22:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mo.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4412 2008-01-09 14:23:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5254 2008-01-09 14:23:46.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ms.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3411 2008-01-09 14:23:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mt.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2940 2008-01-09 14:23:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mu.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3631 2008-01-09 14:22:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mv.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3770 2008-01-09 14:22:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mw.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4229 2008-01-09 14:23:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mx.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4346 2008-01-09 14:22:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/my.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4511 2008-01-09 14:23:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mz.png
--rw-r--r--   0 tom       (1000) tom       (1000)     6560 2008-01-09 14:24:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/na.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3259 2008-01-09 14:24:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ne.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4302 2008-01-09 14:24:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/nf.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2898 2008-01-09 14:24:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ng.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3567 2008-01-09 14:24:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ni.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2937 2008-01-09 14:24:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/nl.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3283 2008-01-09 14:24:46.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/no.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5530 2008-01-09 14:24:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/np.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3565 2008-01-09 14:24:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/nr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4877 2008-01-09 14:24:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/nu.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5439 2008-01-09 14:24:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/nz.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3986 2008-01-09 14:25:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pa.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2898 2008-01-09 14:25:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pe.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5518 2008-01-09 14:25:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pg.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4326 2008-01-09 14:25:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ph.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4161 2008-01-09 14:24:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pk.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2891 2008-01-09 14:25:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pl.png
--rw-r--r--   0 tom       (1000) tom       (1000)     6397 2008-01-09 14:25:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pn.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4429 2008-01-09 14:25:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4803 2008-01-09 14:25:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pt.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3927 2008-01-09 14:25:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pw.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3673 2008-01-09 14:25:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/py.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3645 2008-01-09 14:25:36.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/qa.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2909 2008-01-09 14:25:44.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ro.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2928 2008-01-09 14:26:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/rs.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2941 2008-01-09 14:25:48.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ru.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4154 2008-01-09 14:25:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/rw.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5828 2008-01-09 14:26:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sa.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5260 2008-01-09 14:26:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sb.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4826 2008-01-09 14:26:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sc.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3569 2008-01-09 14:27:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sd.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3107 2008-01-09 14:27:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/se.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3936 2008-01-09 14:26:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sg.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5523 2008-01-09 14:27:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sh.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3804 2008-01-09 14:26:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/si.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4266 2008-01-09 14:26:48.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sk.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2944 2008-01-09 14:26:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sl.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2911 2008-01-09 14:26:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sm.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3332 2008-01-09 14:26:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sn.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3705 2008-01-09 14:27:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/so.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3438 2008-01-09 14:27:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4325 2008-01-09 14:26:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/st.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3621 2008-01-09 14:19:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sv.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3615 2008-01-09 14:27:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sy.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5551 2008-01-09 14:27:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sz.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5396 2008-01-09 14:28:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tc.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3529 2008-01-09 14:28:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tg.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2942 2008-01-09 14:28:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/th.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3497 2008-01-09 14:27:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tj.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4314 2008-01-09 14:28:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tl.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4960 2008-01-09 14:28:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tm.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4200 2008-01-09 14:28:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tn.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3222 2008-01-09 14:28:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/to.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4169 2008-01-09 14:28:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tr.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5314 2008-01-09 14:28:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tt.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4019 2008-01-09 14:27:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tw.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5086 2008-01-09 14:28:02.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tz.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2887 2008-01-09 14:28:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ua.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3711 2008-01-09 14:28:48.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ug.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5012 2008-01-09 14:29:08.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/us.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4421 2008-01-09 14:29:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/uy.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3712 2008-01-09 14:29:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/uz.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4810 2008-01-09 14:29:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/va.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3457 2008-01-09 14:29:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ve.png
--rw-r--r--   0 tom       (1000) tom       (1000)     7301 2008-01-09 14:29:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/vi.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3649 2008-01-09 14:29:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/vn.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5234 2008-01-09 14:29:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/vu.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4295 2008-01-09 14:29:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/wf.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2873 2008-01-09 14:29:34.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ye.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5558 2008-01-09 14:27:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/yt.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5252 2008-01-09 14:27:06.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/za.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3778 2008-01-09 14:29:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/zm.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4354 2008-01-09 14:29:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/zw.png
--rw-r--r--   0 tom       (1000) tom       (1000)      386 2022-04-19 07:52:49.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/crop-tool.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2144 2022-04-19 07:52:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/crop-tool.svg
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.130259 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/interactive-image-field/
--rw-r--r--   0 tom       (1000) tom       (1000)      883 2022-04-26 06:39:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/interactive-image-field/InteractiveImageField.css
--rw-r--r--   0 tom       (1000) tom       (1000)    46117 2022-04-29 08:25:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/interactive-image-field/InteractiveImageField.js
--rw-r--r--   0 tom       (1000) tom       (1000)    86927 2019-04-02 08:38:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/jquery-3.3.1.min.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.130259 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/js/
--rw-r--r--   0 tom       (1000) tom       (1000)     1239 2018-12-10 19:21:28.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/js/ajax_file_input.js
--rw-r--r--   0 tom       (1000) tom       (1000)    22466 2019-10-16 06:19:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/js/bootstrap3-typeahead.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1570 2018-11-26 15:47:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/js/django-ajax-csrf.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2176 2021-07-14 16:31:12.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/js/django-ajax.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3605 2021-08-13 07:36:20.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/js/jquery-taxon-autocomplete.js
--rw-r--r--   0 tom       (1000) tom       (1000)      964 2019-09-30 09:01:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/js/jquery-user-autocomplete.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1015 2019-09-26 07:50:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/js/localcosmos_server.js
--rw-r--r--   0 tom       (1000) tom       (1000)    20337 2018-06-11 12:10:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/js/popper.min.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.130259 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/konva/
--rw-r--r--   0 tom       (1000) tom       (1000)   157749 2022-04-27 12:18:11.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/konva/konva.min.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.130259 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/
--rw-r--r--   0 tom       (1000) tom       (1000)    55182 2017-07-24 08:54:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/Spin.gif
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.950262 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.138259 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/
--rw-r--r--   0 tom       (1000) tom       (1000)    64548 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-grid.css
--rw-r--r--   0 tom       (1000) tom       (1000)   151749 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-grid.css.map
--rw-r--r--   0 tom       (1000) tom       (1000)    48488 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css
--rw-r--r--   0 tom       (1000) tom       (1000)   108539 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4897 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-reboot.css
--rw-r--r--   0 tom       (1000) tom       (1000)    76483 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-reboot.css.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4021 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css
--rw-r--r--   0 tom       (1000) tom       (1000)    32461 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 tom       (1000) tom       (1000)   192348 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap.css
--rw-r--r--   0 tom       (1000) tom       (1000)   492048 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap.css.map
--rw-r--r--   0 tom       (1000) tom       (1000)   155758 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap.min.css
--rw-r--r--   0 tom       (1000) tom       (1000)   625953 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap.min.css.map
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.146259 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/
--rw-r--r--   0 tom       (1000) tom       (1000)   222911 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.bundle.js
--rw-r--r--   0 tom       (1000) tom       (1000)   402249 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.bundle.js.map
--rw-r--r--   0 tom       (1000) tom       (1000)    78635 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js
--rw-r--r--   0 tom       (1000) tom       (1000)   311949 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 tom       (1000) tom       (1000)   131637 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.js
--rw-r--r--   0 tom       (1000) tom       (1000)   250568 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.js.map
--rw-r--r--   0 tom       (1000) tom       (1000)    58072 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.min.js
--rw-r--r--   0 tom       (1000) tom       (1000)   190253 2019-02-13 13:47:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.min.js.map
--rw-r--r--   0 tom       (1000) tom       (1000)      157 2019-01-31 14:44:04.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/error_page.css
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.150259 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/jquery/
--rw-r--r--   0 tom       (1000) tom       (1000)    86927 2019-01-29 09:02:48.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/jquery/jquery-3.3.1.min.js
--rw-r--r--   0 tom       (1000) tom       (1000)   132382 2019-01-29 09:02:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/jquery/jquery-3.3.1.min.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1187 2016-11-11 17:35:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/lc_setup.css
--rw-r--r--   0 tom       (1000) tom       (1000)     7912 2016-11-06 13:33:32.000000 localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/logo100blue.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.950262 localcosmos_server-0.9.3/localcosmos_server/static/maps/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.158259 localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.158259 localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/images/
--rw-r--r--   0 tom       (1000) tom       (1000)     1259 2019-05-08 16:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/images/layers-2x.png
--rw-r--r--   0 tom       (1000) tom       (1000)      696 2019-05-08 16:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/images/layers.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2464 2019-05-08 16:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/images/marker-icon-2x.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1466 2019-05-08 16:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/images/marker-icon.png
--rw-r--r--   0 tom       (1000) tom       (1000)      618 2019-05-08 16:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/images/marker-shadow.png
--rw-r--r--   0 tom       (1000) tom       (1000)   405077 2019-05-08 16:01:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/leaflet-src.esm.js
--rw-r--r--   0 tom       (1000) tom       (1000)   770515 2019-05-08 16:01:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/leaflet-src.esm.js.map
--rw-r--r--   0 tom       (1000) tom       (1000)   406844 2019-05-08 16:01:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/leaflet-src.js
--rw-r--r--   0 tom       (1000) tom       (1000)   770609 2019-05-08 16:01:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/leaflet-src.js.map
--rw-r--r--   0 tom       (1000) tom       (1000)    14268 2019-05-08 16:00:10.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/leaflet.css
--rw-r--r--   0 tom       (1000) tom       (1000)   141833 2019-05-08 16:01:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/leaflet.js
--rw-r--r--   0 tom       (1000) tom       (1000)   195157 2019-05-08 16:01:22.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/leaflet.js.map
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.158259 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/
--rw-r--r--   0 tom       (1000) tom       (1000)     1727 2019-09-10 05:42:58.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Amphibia.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1945 2019-09-10 05:41:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Animalia.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1677 2019-09-10 05:44:44.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Anura.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1622 2019-09-10 05:46:16.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Arachnida.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1883 2019-09-10 05:47:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Arthropoda.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1395 2019-09-10 05:48:50.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Aves.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2042 2019-09-10 05:50:30.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Chordata.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1914 2019-09-10 05:51:42.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Coleoptera.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1793 2019-09-10 05:52:54.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Fungi.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1809 2019-09-10 05:54:26.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Holocephali,Elasmobranchii,Sarcopterygii,Actinopterygii.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2010 2019-09-10 05:55:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Insecta.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1619 2019-09-10 05:56:56.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Lepidoptera.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1667 2019-09-10 05:58:18.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Mammalia.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1712 2019-09-10 05:59:24.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Mollucsa.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1616 2019-09-10 06:00:38.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Odonata.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1617 2019-09-09 14:21:40.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Plantae.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1357 2019-09-09 14:12:14.000000 localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/marker_unknown.png
--rw-r--r--   0 tom       (1000) tom       (1000)     6405 2016-08-24 16:02:52.000000 localcosmos_server-0.9.3/localcosmos_server/static/noimage.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.170258 localcosmos_server-0.9.3/localcosmos_server/static/octicons/
--rw-r--r--   0 tom       (1000) tom       (1000)      366 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/alert.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      265 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/archive.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      135 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/arrow-both.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      144 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/arrow-down.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      145 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/arrow-left.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      145 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/arrow-right.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      142 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/arrow-small-down.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      142 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/arrow-small-left.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      142 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/arrow-small-right.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      142 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/arrow-small-up.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      144 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/arrow-up.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      297 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/beaker.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      311 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/bell.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      397 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/bold.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      352 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/book.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      366 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/bookmark.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      283 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/briefcase.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      686 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/broadcast.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      268 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/browser.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      438 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/bug.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      588 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/calendar.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      162 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/check.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      399 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/checklist.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      164 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/chevron-down.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      162 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/chevron-left.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      161 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/chevron-right.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      166 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/chevron-up.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      349 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/circle-slash.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      695 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/circuit-board.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      455 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/clippy.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      306 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/clock.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      429 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/cloud-download.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      429 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/cloud-upload.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      207 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/code.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      330 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/comment-discussion.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      237 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/comment.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      258 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/credit-card.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      132 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/dash.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      531 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/dashboard.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      524 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/database.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      376 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/dependent.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      299 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/desktop-download.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      269 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/device-camera-video.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      396 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/device-camera.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      272 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/device-desktop.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      307 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/device-mobile.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      246 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/diff-added.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      252 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/diff-ignored.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      273 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/diff-modified.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      231 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/diff-removed.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      239 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/diff-renamed.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      288 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/diff.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      239 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/ellipsis.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      685 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/eye-closed.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      327 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/eye.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      320 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/file-binary.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      304 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/file-code.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      234 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/file-directory.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      239 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/file-media.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      976 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/file-pdf.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      301 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/file-submodule.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      354 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/file-symlink-directory.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      339 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/file-symlink-file.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      348 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/file-zip.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      268 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/file.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      497 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/flame.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      320 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/fold-down.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      316 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/fold-up.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      329 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/fold.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      457 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/gear.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      788 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/gift.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      365 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/gist-secret.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      321 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/gist.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      772 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/git-branch.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      338 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/git-commit.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      643 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/git-compare.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      724 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/git-merge.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      693 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/git-pull-request.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      290 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/github-action.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     1874 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/globe.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      159 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/grabber.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      184 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/graph.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      362 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/heart.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      358 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/history.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      241 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/home.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      217 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/horizontal-rule.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      443 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/hubot.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      375 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/inbox.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      632 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/info.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      385 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/issue-closed.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      299 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/issue-opened.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      487 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/issue-reopened.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      247 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/italic.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      718 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/jersey.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      249 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/kebab-horizontal.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      247 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/kebab-vertical.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      461 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/key.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      486 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/keyboard.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      490 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/law.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      571 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/light-bulb.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      245 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/link-external.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      454 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/link.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      939 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/list-ordered.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      632 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/list-unordered.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      395 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/location.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      351 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/lock.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     1009 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/logo-gist.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     1945 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/logo-github.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      395 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/mail-read.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      285 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/mail.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      691 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/mark-github.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      324 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/markdown.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      466 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/megaphone.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      677 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/mention.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      213 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/milestone.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      288 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/mirror.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      548 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/mortar-board.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      360 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/mute.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      374 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/no-newline.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      254 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/note.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      708 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/octoface.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      531 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/organization.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      445 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/package.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      644 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/paintcan.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      242 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/pencil.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      334 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/person.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      273 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/pin.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      257 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/play.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      248 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/plug.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      148 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/plus-small.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      151 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/plus.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      170 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/primitive-dot.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      133 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/primitive-square.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      255 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/project.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      205 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/pulse.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      421 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/question.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      465 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/quote.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     1093 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/radio-tower.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      190 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/reply.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      400 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/repo-clone.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      276 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/repo-force-push.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      583 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/repo-forked.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      336 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/repo-pull.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      289 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/repo-push.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      367 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/repo-template-private.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      311 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/repo-template.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      312 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/repo.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      255 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/report.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      276 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/request-changes.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      599 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/rocket.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      236 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/rss.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      199 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/ruby.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      297 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/screen-full.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      366 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/screen-normal.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      403 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/search.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      532 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/server.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      395 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/settings.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      404 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/shield-check.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      330 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/shield-lock.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      465 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/shield-x.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      306 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/shield.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      272 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/sign-in.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      261 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/sign-out.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      281 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/skip.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      895 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/smiley.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      536 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/squirrel.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      202 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/star.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      223 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/stop.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      430 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/sync.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      419 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/tag.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      430 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/tasklist.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      425 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/telescope.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      275 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/terminal.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      333 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/text-size.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      376 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/three-bars.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      600 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/thumbsdown.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      610 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/thumbsup.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      542 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/tools.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      324 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/trashcan.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      136 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/triangle-down.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      134 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/triangle-left.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      136 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/triangle-right.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      140 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/triangle-up.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      320 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/unfold.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      619 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/unmute.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     1364 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/unverified.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      737 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/verified.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      319 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/versions.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      368 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/watch.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      237 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/x.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      148 1985-10-26 07:15:00.000000 localcosmos_server-0.9.3/localcosmos_server/static/octicons/zap.svg
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.174258 localcosmos_server-0.9.3/localcosmos_server/taxonomy/
--rw-r--r--   0 tom       (1000) tom       (1000)     2805 2020-09-04 07:10:42.000000 localcosmos_server-0.9.3/localcosmos_server/taxonomy/AppTaxonSearch.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2019-03-25 08:50:38.000000 localcosmos_server-0.9.3/localcosmos_server/taxonomy/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2342 2020-08-28 07:52:24.000000 localcosmos_server-0.9.3/localcosmos_server/taxonomy/fields.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1389 2019-12-10 08:05:46.000000 localcosmos_server-0.9.3/localcosmos_server/taxonomy/forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6758 2020-08-28 07:52:24.000000 localcosmos_server-0.9.3/localcosmos_server/taxonomy/generic.py
--rw-r--r--   0 tom       (1000) tom       (1000)    11867 2020-08-28 07:52:24.000000 localcosmos_server-0.9.3/localcosmos_server/taxonomy/lazy.py
--rw-r--r--   0 tom       (1000) tom       (1000)      531 2019-09-23 14:52:16.000000 localcosmos_server-0.9.3/localcosmos_server/taxonomy/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4559 2020-08-28 07:52:24.000000 localcosmos_server-0.9.3/localcosmos_server/taxonomy/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2497 2020-08-28 07:52:24.000000 localcosmos_server-0.9.3/localcosmos_server/taxonomy/widgets.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.174258 localcosmos_server-0.9.3/localcosmos_server/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)      259 2020-03-16 08:59:56.000000 localcosmos_server-0.9.3/localcosmos_server/templates/400.html
--rw-r--r--   0 tom       (1000) tom       (1000)      316 2019-02-27 08:46:14.000000 localcosmos_server-0.9.3/localcosmos_server/templates/403.html
--rw-r--r--   0 tom       (1000) tom       (1000)      286 2019-02-27 07:57:46.000000 localcosmos_server-0.9.3/localcosmos_server/templates/404.html
--rw-r--r--   0 tom       (1000) tom       (1000)      303 2019-02-27 07:57:50.000000 localcosmos_server-0.9.3/localcosmos_server/templates/500.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.174258 localcosmos_server-0.9.3/localcosmos_server/templates/anycluster/
--rw-r--r--   0 tom       (1000) tom       (1000)      493 2019-09-19 13:09:12.000000 localcosmos_server-0.9.3/localcosmos_server/templates/anycluster/clusterPopup.html
--rw-r--r--   0 tom       (1000) tom       (1000)     3234 2022-04-28 07:07:42.000000 localcosmos_server-0.9.3/localcosmos_server/templates/base.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.174258 localcosmos_server-0.9.3/localcosmos_server/templates/content_licencing/
--rw-r--r--   0 tom       (1000) tom       (1000)       86 2018-02-26 06:39:00.000000 localcosmos_server-0.9.3/localcosmos_server/templates/content_licencing/licencing_form.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.174258 localcosmos_server-0.9.3/localcosmos_server/templates/content_licencing/widgets/
--rw-r--r--   0 tom       (1000) tom       (1000)     1096 2019-10-09 13:30:06.000000 localcosmos_server-0.9.3/localcosmos_server/templates/content_licencing/widgets/licence_select_widget.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.950262 localcosmos_server-0.9.3/localcosmos_server/templates/django/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.950262 localcosmos_server-0.9.3/localcosmos_server/templates/django/forms/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.174258 localcosmos_server-0.9.3/localcosmos_server/templates/django/forms/widgets/
--rw-r--r--   0 tom       (1000) tom       (1000)      172 2018-05-22 12:17:28.000000 localcosmos_server-0.9.3/localcosmos_server/templates/django/forms/widgets/attrs.html
--rw-r--r--   0 tom       (1000) tom       (1000)       96 2019-10-01 08:40:08.000000 localcosmos_server-0.9.3/localcosmos_server/templates/django/forms/widgets/checkbox.html
--rw-r--r--   0 tom       (1000) tom       (1000)       97 2019-10-09 13:10:16.000000 localcosmos_server-0.9.3/localcosmos_server/templates/django/forms/widgets/file.html
--rw-r--r--   0 tom       (1000) tom       (1000)      243 2019-10-09 13:10:00.000000 localcosmos_server-0.9.3/localcosmos_server/templates/django/forms/widgets/input.html
--rw-r--r--   0 tom       (1000) tom       (1000)      406 2019-10-09 13:29:18.000000 localcosmos_server-0.9.3/localcosmos_server/templates/django/forms/widgets/select.html
--rw-r--r--   0 tom       (1000) tom       (1000)       48 2018-05-22 12:17:28.000000 localcosmos_server-0.9.3/localcosmos_server/templates/django/forms/widgets/text.html
--rw-r--r--   0 tom       (1000) tom       (1000)      166 2019-10-01 08:49:18.000000 localcosmos_server-0.9.3/localcosmos_server/templates/django/forms/widgets/textarea.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.174258 localcosmos_server-0.9.3/localcosmos_server/templates/el_pagination/
--rw-r--r--   0 tom       (1000) tom       (1000)      152 2019-09-30 11:54:52.000000 localcosmos_server-0.9.3/localcosmos_server/templates/el_pagination/current_link.html
--rw-r--r--   0 tom       (1000) tom       (1000)      187 2018-05-22 12:19:12.000000 localcosmos_server-0.9.3/localcosmos_server/templates/el_pagination/next_link.html
--rw-r--r--   0 tom       (1000) tom       (1000)      207 2021-07-25 12:28:38.000000 localcosmos_server-0.9.3/localcosmos_server/templates/el_pagination/page_link.html
--rw-r--r--   0 tom       (1000) tom       (1000)      187 2019-09-30 11:46:50.000000 localcosmos_server-0.9.3/localcosmos_server/templates/el_pagination/previous_link.html
--rw-r--r--   0 tom       (1000) tom       (1000)      429 2018-05-22 12:19:12.000000 localcosmos_server-0.9.3/localcosmos_server/templates/el_pagination/show_more.html
--rw-r--r--   0 tom       (1000) tom       (1000)      267 2019-09-30 11:59:12.000000 localcosmos_server-0.9.3/localcosmos_server/templates/el_pagination/show_pages.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.174258 localcosmos_server-0.9.3/localcosmos_server/templates/email/
--rw-r--r--   0 tom       (1000) tom       (1000)     7594 2020-04-24 08:20:18.000000 localcosmos_server-0.9.3/localcosmos_server/templates/email/registration_confirmation.html
--rw-r--r--   0 tom       (1000) tom       (1000)      787 2020-04-24 11:06:10.000000 localcosmos_server-0.9.3/localcosmos_server/templates/email/registration_confirmation.txt
--rw-r--r--   0 tom       (1000) tom       (1000)     1338 2020-03-16 09:09:30.000000 localcosmos_server-0.9.3/localcosmos_server/templates/error_base.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.174258 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.174258 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/api/
--rw-r--r--   0 tom       (1000) tom       (1000)      315 2019-12-09 13:59:26.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/api/delete_account.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.174258 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/api/legal/
--rw-r--r--   0 tom       (1000) tom       (1000)    15879 2020-04-21 14:55:30.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/api/legal/privacy_statement.html
--rw-r--r--   0 tom       (1000) tom       (1000)      348 2019-12-09 11:39:04.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/api/manage_account.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1227 2020-04-22 12:14:26.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/api/password_reset_form.html
--rw-r--r--   0 tom       (1000) tom       (1000)      790 2019-12-09 14:43:34.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/api/register_account.html
--rw-r--r--   0 tom       (1000) tom       (1000)     3398 2020-01-23 07:55:02.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/bootstrap_field.html
--rw-r--r--   0 tom       (1000) tom       (1000)      190 2019-10-01 09:15:46.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/bootstrap_form.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.174258 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/generic/
--rw-r--r--   0 tom       (1000) tom       (1000)     1390 2020-04-03 11:21:58.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/generic/delete_object.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.178258 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/legal/
--rw-r--r--   0 tom       (1000) tom       (1000)     1312 2020-05-11 08:32:06.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/legal/base.html
--rw-r--r--   0 tom       (1000) tom       (1000)      929 2020-04-24 07:44:54.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/legal/legal_notice.html
--rw-r--r--   0 tom       (1000) tom       (1000)      549 2020-04-24 07:55:48.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/legal/privacy_statement.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.178258 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/modals/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.178258 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/modals/footers/
--rw-r--r--   0 tom       (1000) tom       (1000)      213 2019-10-09 12:42:50.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/modals/footers/add_selected.html
--rw-r--r--   0 tom       (1000) tom       (1000)      122 2019-10-09 13:35:20.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/modals/footers/close.html
--rw-r--r--   0 tom       (1000) tom       (1000)      198 2019-10-09 13:35:30.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/modals/footers/delete.html
--rw-r--r--   0 tom       (1000) tom       (1000)      205 2020-04-03 11:22:44.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/modals/footers/save.html
--rw-r--r--   0 tom       (1000) tom       (1000)      204 2020-04-03 11:22:50.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/modals/footers/save_close.html
--rw-r--r--   0 tom       (1000) tom       (1000)      323 2019-09-19 13:04:32.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/modals/large_modal_base.html
--rw-r--r--   0 tom       (1000) tom       (1000)      405 2019-09-19 13:04:24.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/modals/large_modal_form.html
--rw-r--r--   0 tom       (1000) tom       (1000)      869 2019-09-20 08:50:12.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/modals/modal_base.html
--rw-r--r--   0 tom       (1000) tom       (1000)      322 2019-09-19 13:04:16.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/modals/modal_form.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.178258 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/
--rw-r--r--   0 tom       (1000) tom       (1000)      827 2020-04-03 11:23:34.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/loggedout.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1552 2020-04-03 11:23:52.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/login.html
--rw-r--r--   0 tom       (1000) tom       (1000)      450 2019-11-14 14:44:22.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/password_change_done.html
--rw-r--r--   0 tom       (1000) tom       (1000)      817 2019-11-14 14:44:26.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/password_change_form.html
--rw-r--r--   0 tom       (1000) tom       (1000)      545 2020-04-03 11:24:16.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/password_reset_complete.html
--rw-r--r--   0 tom       (1000) tom       (1000)      997 2020-04-03 11:24:26.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/password_reset_confirm.html
--rw-r--r--   0 tom       (1000) tom       (1000)      663 2019-11-14 14:44:40.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/password_reset_done.html
--rw-r--r--   0 tom       (1000) tom       (1000)      582 2020-04-22 12:58:14.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/password_reset_email.html
--rw-r--r--   0 tom       (1000) tom       (1000)      857 2019-11-14 14:44:44.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/password_reset_form.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.178258 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/setup/
--rw-r--r--   0 tom       (1000) tom       (1000)     1569 2020-05-11 08:28:24.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/setup/base.html
--rw-r--r--   0 tom       (1000) tom       (1000)      752 2020-04-03 11:25:14.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/setup/setup_superuser.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.178258 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/taxonomy/
--rw-r--r--   0 tom       (1000) tom       (1000)     1201 2020-04-03 11:25:38.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/taxonomy/manage_taxonomic_restrictions.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2031 2020-04-03 11:26:02.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/taxonomy/taxonomic_restrictions_form.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.178258 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/widgets/
--rw-r--r--   0 tom       (1000) tom       (1000)      919 2018-12-10 19:11:42.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/widgets/ajax_file_input.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1243 2020-04-03 11:26:34.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/widgets/app_theme_image_file_input.html
--rw-r--r--   0 tom       (1000) tom       (1000)      915 2022-04-28 07:09:31.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/widgets/crop_image_input.html
--rw-r--r--   0 tom       (1000) tom       (1000)      297 2019-10-09 13:14:46.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/widgets/image_input_with_preview.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.178258 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/widgets/taxonomy/
--rw-r--r--   0 tom       (1000) tom       (1000)       88 2019-09-20 13:20:16.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/widgets/taxonomy/taxon_autocomplete_widget.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2610 2020-04-17 07:58:52.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/widgets/taxonomy/taxon_autocomplete_widget_base.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1146 2020-04-03 11:26:54.000000 localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/widgets/two_step_file_input.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:40.178258 localcosmos_server-0.9.3/localcosmos_server/templatetags/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2016-03-22 12:09:42.000000 localcosmos_server-0.9.3/localcosmos_server/templatetags/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3621 2022-04-21 10:15:23.000000 localcosmos_server-0.9.3/localcosmos_server/templatetags/localcosmos_tags.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1164 2020-02-04 07:51:02.000000 localcosmos_server-0.9.3/localcosmos_server/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)      554 2019-10-01 06:46:50.000000 localcosmos_server-0.9.3/localcosmos_server/utils.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6820 2020-04-03 11:19:14.000000 localcosmos_server-0.9.3/localcosmos_server/validators.py
--rw-r--r--   0 tom       (1000) tom       (1000)      937 2020-02-17 12:00:18.000000 localcosmos_server-0.9.3/localcosmos_server/view_mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2632 2020-04-24 07:35:50.000000 localcosmos_server-0.9.3/localcosmos_server/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3871 2022-04-21 10:16:38.000000 localcosmos_server-0.9.3/localcosmos_server/widgets.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-04-29 09:29:39.954262 localcosmos_server-0.9.3/localcosmos_server.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)      806 2022-04-29 09:29:39.000000 localcosmos_server-0.9.3/localcosmos_server.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)    96106 2022-04-29 09:29:39.000000 localcosmos_server-0.9.3/localcosmos_server.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2022-04-29 09:29:39.000000 localcosmos_server-0.9.3/localcosmos_server.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      237 2022-04-29 09:29:39.000000 localcosmos_server-0.9.3/localcosmos_server.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       19 2022-04-29 09:29:39.000000 localcosmos_server-0.9.3/localcosmos_server.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2022-04-29 09:29:40.178258 localcosmos_server-0.9.3/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)     1281 2022-04-29 09:27:52.000000 localcosmos_server-0.9.3/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.720216 localcosmos_server-0.9.4/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2018-07-30 12:18:06.000000 localcosmos_server-0.9.4/LICENCE
+-rw-r--r--   0 tom       (1000) tom       (1000)      563 2020-04-06 07:18:54.000000 localcosmos_server-0.9.4/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)      804 2022-05-13 14:25:25.720216 localcosmos_server-0.9.4/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      189 2019-11-15 15:44:36.000000 localcosmos_server-0.9.4/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.576217 localcosmos_server-0.9.4/localcosmos_server/
+-rw-r--r--   0 tom       (1000) tom       (1000)       50 2022-05-13 14:24:02.000000 localcosmos_server-0.9.4/localcosmos_server/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      165 2019-11-14 15:30:50.000000 localcosmos_server-0.9.4/localcosmos_server/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      709 2019-09-10 12:32:06.000000 localcosmos_server-0.9.4/localcosmos_server/anycluster_schema_urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1711 2019-10-02 09:15:04.000000 localcosmos_server-0.9.4/localcosmos_server/anycluster_schema_views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.580217 localcosmos_server-0.9.4/localcosmos_server/api/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2019-03-25 10:52:36.000000 localcosmos_server-0.9.4/localcosmos_server/api/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1281 2019-03-25 11:25:56.000000 localcosmos_server-0.9.4/localcosmos_server/api/authentication.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2169 2020-01-14 16:23:50.000000 localcosmos_server-0.9.4/localcosmos_server/api/permissions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1186 2019-10-01 14:23:52.000000 localcosmos_server-0.9.4/localcosmos_server/api/road_permissions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3275 2020-03-23 08:27:04.000000 localcosmos_server-0.9.4/localcosmos_server/api/road_serializers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7260 2020-11-14 08:46:40.000000 localcosmos_server-0.9.4/localcosmos_server/api/serializers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      842 2020-04-22 10:24:04.000000 localcosmos_server-0.9.4/localcosmos_server/api/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10663 2020-04-23 06:54:44.000000 localcosmos_server-0.9.4/localcosmos_server/api/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.580217 localcosmos_server-0.9.4/localcosmos_server/app_admin/
+-rw-r--r--   0 tom       (1000) tom       (1000)       73 2019-07-02 05:56:40.000000 localcosmos_server-0.9.4/localcosmos_server/app_admin/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2019-03-25 10:52:50.000000 localcosmos_server-0.9.4/localcosmos_server/app_admin/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       92 2019-04-02 14:03:28.000000 localcosmos_server-0.9.4/localcosmos_server/app_admin/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      399 2020-04-03 11:08:46.000000 localcosmos_server-0.9.4/localcosmos_server/app_admin/forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1559 2020-03-03 11:33:16.000000 localcosmos_server-0.9.4/localcosmos_server/app_admin/middleware.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       57 2019-03-25 10:52:50.000000 localcosmos_server-0.9.4/localcosmos_server/app_admin/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.572217 localcosmos_server-0.9.4/localcosmos_server/app_admin/static/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.572217 localcosmos_server-0.9.4/localcosmos_server/app_admin/static/app_admin/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.580217 localcosmos_server-0.9.4/localcosmos_server/app_admin/static/app_admin/css/
+-rw-r--r--   0 tom       (1000) tom       (1000)      215 2019-10-15 09:37:58.000000 localcosmos_server-0.9.4/localcosmos_server/app_admin/static/app_admin/css/app_admin.css
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.580217 localcosmos_server-0.9.4/localcosmos_server/app_admin/static/app_admin/img/
+-rw-r--r--   0 tom       (1000) tom       (1000)     5970 2019-09-19 12:05:20.000000 localcosmos_server-0.9.4/localcosmos_server/app_admin/static/app_admin/img/downarrow.svg
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.572217 localcosmos_server-0.9.4/localcosmos_server/app_admin/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.580217 localcosmos_server-0.9.4/localcosmos_server/app_admin/templates/app_admin/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.580217 localcosmos_server-0.9.4/localcosmos_server/app_admin/templates/app_admin/ajax/
+-rw-r--r--   0 tom       (1000) tom       (1000)      883 2020-04-03 11:28:58.000000 localcosmos_server-0.9.4/localcosmos_server/app_admin/templates/app_admin/ajax/userbox.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     4682 2022-04-21 09:09:53.000000 localcosmos_server-0.9.4/localcosmos_server/app_admin/templates/app_admin/base.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      995 2019-11-19 16:08:36.000000 localcosmos_server-0.9.4/localcosmos_server/app_admin/templates/app_admin/home.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1017 2020-04-03 11:28:06.000000 localcosmos_server-0.9.4/localcosmos_server/app_admin/templates/app_admin/manage_app_user_role.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2474 2020-04-03 11:28:30.000000 localcosmos_server-0.9.4/localcosmos_server/app_admin/templates/app_admin/userlist.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      492 2019-10-09 07:37:30.000000 localcosmos_server-0.9.4/localcosmos_server/app_admin/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      628 2019-10-01 13:20:58.000000 localcosmos_server-0.9.4/localcosmos_server/app_admin/view_mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4941 2020-02-18 11:38:24.000000 localcosmos_server-0.9.4/localcosmos_server/app_admin/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      110 2019-03-25 08:50:38.000000 localcosmos_server-0.9.4/localcosmos_server/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      242 2019-11-12 14:45:50.000000 localcosmos_server-0.9.4/localcosmos_server/context_processors.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.580217 localcosmos_server-0.9.4/localcosmos_server/datasets/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2019-03-25 09:05:02.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2019-03-25 09:05:02.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       91 2019-06-24 06:12:48.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3295 2020-04-28 06:44:46.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/csv_export.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2106 2019-09-26 06:48:48.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/fields.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5333 2020-02-14 13:15:08.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/forms.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.580217 localcosmos_server-0.9.4/localcosmos_server/datasets/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4026 2020-08-28 07:52:24.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2020-08-28 07:52:24.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    18054 2020-08-28 07:52:24.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.572217 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.580217 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.580217 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/ajax/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1170 2020-08-28 07:52:24.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/ajax/dataset_box.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      277 2019-09-30 12:06:50.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/ajax/dataset_review_box.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     4532 2020-04-03 11:31:02.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/dataset_validation_routine.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      751 2019-11-19 12:33:10.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/edit_dataset.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1173 2020-04-03 11:31:34.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/list_datasets.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      891 2020-04-03 11:31:42.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/manage_dataset_validation_routine_step.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.580217 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/validation/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.580217 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/validation/ajax/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1185 2020-04-03 11:33:10.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/validation/ajax/dataset_form.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      342 2020-04-03 11:33:18.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/validation/ajax/delete_dataset.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      308 2020-04-03 11:33:24.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/validation/ajax/delete_dataset_image.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      372 2019-09-26 12:13:34.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/validation/ajax/large_modal_image.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1050 2020-04-03 11:33:42.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/validation/ajax/picture_field_images.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2424 2020-04-03 11:32:44.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/validation/expert_review.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.580217 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/widgets/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2070 2019-09-24 06:27:46.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/widgets/mobile_number_input.html
+-rw-r--r--   0 tom       (1000) tom       (1000)    10059 2020-01-21 07:06:50.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/widgets/mobile_position_input.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      952 2020-04-03 11:34:44.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/widgets/picture_widget.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     3430 2019-10-09 12:40:06.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/widgets/select_datetime_widget.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1917 2019-10-01 06:38:48.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/urls.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.584217 localcosmos_server-0.9.4/localcosmos_server/datasets/validation/
+-rw-r--r--   0 tom       (1000) tom       (1000)       72 2019-09-24 08:34:36.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/validation/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4704 2020-04-03 11:10:18.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/validation/base.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      482 2019-12-10 08:06:58.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/validation/forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1583 2020-04-03 11:11:28.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/validation/validators.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10209 2020-04-03 11:11:56.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8936 2019-09-26 07:22:28.000000 localcosmos_server-0.9.4/localcosmos_server/datasets/widgets.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      335 2019-03-14 15:26:54.000000 localcosmos_server-0.9.4/localcosmos_server/decorators.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      693 2019-09-20 10:46:38.000000 localcosmos_server-0.9.4/localcosmos_server/fields.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7092 2022-04-29 07:48:12.000000 localcosmos_server-0.9.4/localcosmos_server/forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1586 2019-09-23 14:42:28.000000 localcosmos_server-0.9.4/localcosmos_server/generic_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2414 2020-04-24 07:10:36.000000 localcosmos_server-0.9.4/localcosmos_server/global_urls.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.584217 localcosmos_server-0.9.4/localcosmos_server/google_cloud_api/
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2019-09-03 06:59:12.000000 localcosmos_server-0.9.4/localcosmos_server/google_cloud_api/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      162 2019-09-03 07:37:06.000000 localcosmos_server-0.9.4/localcosmos_server/google_cloud_api/serializers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      349 2019-09-03 07:44:40.000000 localcosmos_server-0.9.4/localcosmos_server/google_cloud_api/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1888 2019-09-03 07:50:26.000000 localcosmos_server-0.9.4/localcosmos_server/google_cloud_api/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.572217 localcosmos_server-0.9.4/localcosmos_server/locale/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.572217 localcosmos_server-0.9.4/localcosmos_server/locale/de/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.584217 localcosmos_server-0.9.4/localcosmos_server/locale/de/LC_MESSAGES/
+-rw-r--r--   0 tom       (1000) tom       (1000)    25465 2020-04-24 08:34:34.000000 localcosmos_server-0.9.4/localcosmos_server/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 tom       (1000) tom       (1000)    47980 2020-04-24 08:34:12.000000 localcosmos_server-0.9.4/localcosmos_server/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.572217 localcosmos_server-0.9.4/localcosmos_server/locale/en/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.584217 localcosmos_server-0.9.4/localcosmos_server/locale/en/LC_MESSAGES/
+-rw-r--r--   0 tom       (1000) tom       (1000)      380 2020-04-24 08:34:34.000000 localcosmos_server-0.9.4/localcosmos_server/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 tom       (1000) tom       (1000)    37743 2020-04-24 08:32:22.000000 localcosmos_server-0.9.4/localcosmos_server/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 tom       (1000) tom       (1000)     1776 2020-04-25 08:33:16.000000 localcosmos_server-0.9.4/localcosmos_server/mails.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.584217 localcosmos_server-0.9.4/localcosmos_server/management/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2016-11-15 14:26:24.000000 localcosmos_server-0.9.4/localcosmos_server/management/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.584217 localcosmos_server-0.9.4/localcosmos_server/management/commands/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2016-11-15 14:26:24.000000 localcosmos_server-0.9.4/localcosmos_server/management/commands/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      775 2020-04-22 10:01:14.000000 localcosmos_server-0.9.4/localcosmos_server/management/commands/enable_staging_domain.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      931 2019-11-25 11:16:42.000000 localcosmos_server-0.9.4/localcosmos_server/middleware.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.584217 localcosmos_server-0.9.4/localcosmos_server/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     7449 2020-08-28 07:52:24.000000 localcosmos_server-0.9.4/localcosmos_server/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2020-08-28 07:52:24.000000 localcosmos_server-0.9.4/localcosmos_server/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    19755 2020-08-28 07:52:24.000000 localcosmos_server-0.9.4/localcosmos_server/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.584217 localcosmos_server-0.9.4/localcosmos_server/online_content/
+-rw-r--r--   0 tom       (1000) tom       (1000)    10003 2020-11-20 08:22:30.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/CMSObjects.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2019-03-25 10:52:36.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2019-03-25 10:52:36.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/admin.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.584217 localcosmos_server-0.9.4/localcosmos_server/online_content/api/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2019-03-25 10:52:36.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/api/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      418 2019-03-28 11:44:06.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/api/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5654 2020-01-15 07:58:08.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/api/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      102 2019-04-02 14:43:56.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2232 2019-12-10 08:08:02.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/fields.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7707 2020-12-07 09:08:14.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/forms.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.584217 localcosmos_server-0.9.4/localcosmos_server/online_content/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)    10880 2020-08-28 07:52:24.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2020-08-28 07:52:24.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1230 2020-01-15 10:12:28.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    39464 2020-08-28 07:52:24.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2618 2020-11-19 14:08:36.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/parser.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.572217 localcosmos_server-0.9.4/localcosmos_server/online_content/static/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.584217 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.588217 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1297 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/LICENSE.md
+-rw-r--r--   0 tom       (1000) tom       (1000)      424 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/README.md
+-rw-r--r--   0 tom       (1000) tom       (1000)   617478 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/ckeditor.js
+-rw-r--r--   0 tom       (1000) tom       (1000)  4144258 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/ckeditor.js.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5597 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/index.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.588217 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1297 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/LICENSE.md
+-rw-r--r--   0 tom       (1000) tom       (1000)      424 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/README.md
+-rw-r--r--   0 tom       (1000) tom       (1000)   433388 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/ckeditor.js
+-rw-r--r--   0 tom       (1000) tom       (1000)  2837712 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/ckeditor.js.map
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.592217 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/
+-rw-r--r--   0 tom       (1000) tom       (1000)      797 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ar.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      804 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ast.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      764 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/bg.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      835 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/cs.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      778 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/da.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      861 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/de.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1122 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/el.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      727 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/en-au.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      786 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/eo.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      900 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/es.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      810 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/et.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      839 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/eu.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      787 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/fi.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      836 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/fr.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      884 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/gl.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      838 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/gu.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      790 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/hr.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      844 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/hu.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      956 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/it.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      957 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ja.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1517 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/km.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1392 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/kn.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      770 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ko.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1330 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ku.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      793 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/nb.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      863 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ne.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      831 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/nl.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      731 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/oc.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      787 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/pl.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      862 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/pt-br.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      843 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/pt.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      907 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ro.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1407 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ru.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1007 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/si.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      847 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/sk.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      856 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/sq.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      752 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/sv.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      861 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/tr.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      744 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/tt.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1155 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ug.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      972 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/uk.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      772 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/zh-cn.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      750 2018-05-22 14:15:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/zh.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.572217 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.592217 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/css/
+-rw-r--r--   0 tom       (1000) tom       (1000)     9675 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/css/sample.css
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.592217 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/
+-rw-r--r--   0 tom       (1000) tom       (1000)     6777 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/bg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      937 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/github.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)    10702 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/logo.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)    51250 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/umbrellas.jpg
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.600216 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1818 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/af.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2255 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ar.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1881 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ast.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2177 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/az.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1835 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/bg.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1822 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ca.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2184 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/cs.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1953 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/da.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1877 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/de-ch.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2190 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/de.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2222 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/el.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1798 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/en-au.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1798 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/en-gb.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1865 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/eo.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2326 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/es.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2084 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/et.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1916 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/eu.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2921 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/fa.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1979 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/fi.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2326 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/fr.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2267 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/gl.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1909 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/gu.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2295 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/he.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2011 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/hr.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2176 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/hu.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1917 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/id.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2401 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/it.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2122 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ja.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2593 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/km.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2501 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/kn.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1850 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ko.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3343 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ku.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2210 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/lt.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2215 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/lv.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1796 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ms.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1920 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/nb.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4657 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ne.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2079 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/nl.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2089 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/no.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1802 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/oc.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2258 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/pl.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2152 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/pt-br.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1922 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/pt.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2123 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ro.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3398 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ru.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2078 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/si.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2129 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sk.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1835 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sl.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2004 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sq.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2055 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sr-latn.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3137 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sr.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1829 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sv.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2949 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/th.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2116 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/tr.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1815 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/tt.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2243 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ug.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3661 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/uk.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2351 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/vi.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1854 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/zh-cn.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1755 2020-03-24 14:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/zh.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1547 2019-04-02 13:59:36.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/online_content.css
+-rw-r--r--   0 tom       (1000) tom       (1000)     2405 2018-11-26 15:24:22.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/online_content.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.572217 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.600216 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.600216 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/ajax/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1537 2020-04-03 11:38:50.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/ajax/image_microcontent_form.html
+-rw-r--r--   0 tom       (1000) tom       (1000)       92 2018-12-24 09:28:26.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/ajax/reloaded_file_fields.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1146 2022-01-10 08:32:52.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/ajax/unpublish_template_content.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      997 2020-04-28 13:23:38.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/ajax/upload_custom_template.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1124 2020-04-03 11:35:30.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/ajax_filecontent_field.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.600216 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/ckeditor/
+-rw-r--r--   0 tom       (1000) tom       (1000)      424 2020-04-16 06:22:46.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/ckeditor/layout-complex.js
+-rw-r--r--   0 tom       (1000) tom       (1000)       55 2020-12-01 11:36:38.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/ckeditor/layout-simple.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      225 2018-07-04 15:11:50.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/content_managing_js.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      999 2020-04-28 13:01:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/create_template_content.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1533 2020-04-03 11:35:54.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/delete_microcontent.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1404 2020-12-07 07:35:42.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/filecontent_field.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      370 2018-07-04 15:23:04.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/filecontent_field_form.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     6856 2020-04-03 11:37:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/manage_template_content.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      758 2018-07-09 13:15:48.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/manage_template_content_extra_scripts.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2047 2019-10-09 12:21:00.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/online_content_base.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     4141 2020-04-03 11:38:10.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/template_content_list_entry.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1223 2020-04-03 11:38:20.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/textcontent_field.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     3539 2019-10-15 09:39:40.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/translate_template_content.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.600216 localcosmos_server-0.9.4/localcosmos_server/online_content/templatetags/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2018-06-01 14:17:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templatetags/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8634 2019-10-01 09:13:46.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/templatetags/online_content_tags.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3011 2020-04-28 12:13:16.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      171 2020-04-28 11:55:50.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/utils.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    32882 2021-08-13 07:39:28.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3456 2019-11-18 14:41:48.000000 localcosmos_server-0.9.4/localcosmos_server/online_content/widgets.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1883 2019-10-01 13:22:14.000000 localcosmos_server-0.9.4/localcosmos_server/permission_rules.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.600216 localcosmos_server-0.9.4/localcosmos_server/server_control_panel/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2019-10-02 08:02:42.000000 localcosmos_server-0.9.4/localcosmos_server/server_control_panel/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2019-10-02 08:02:42.000000 localcosmos_server-0.9.4/localcosmos_server/server_control_panel/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      113 2019-10-02 08:02:42.000000 localcosmos_server-0.9.4/localcosmos_server/server_control_panel/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      751 2020-04-03 11:15:28.000000 localcosmos_server-0.9.4/localcosmos_server/server_control_panel/forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      940 2020-01-14 07:35:28.000000 localcosmos_server-0.9.4/localcosmos_server/server_control_panel/middleware.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       57 2019-10-02 08:02:42.000000 localcosmos_server-0.9.4/localcosmos_server/server_control_panel/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.572217 localcosmos_server-0.9.4/localcosmos_server/server_control_panel/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.600216 localcosmos_server-0.9.4/localcosmos_server/server_control_panel/templates/server_control_panel/
+-rw-r--r--   0 tom       (1000) tom       (1000)      200 2019-10-09 12:05:02.000000 localcosmos_server-0.9.4/localcosmos_server/server_control_panel/templates/server_control_panel/app_api_status.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     3773 2020-04-03 11:39:44.000000 localcosmos_server-0.9.4/localcosmos_server/server_control_panel/templates/server_control_panel/base.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      750 2020-04-03 11:39:56.000000 localcosmos_server-0.9.4/localcosmos_server/server_control_panel/templates/server_control_panel/edit_app.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     4777 2020-04-03 11:41:06.000000 localcosmos_server-0.9.4/localcosmos_server/server_control_panel/templates/server_control_panel/home.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2508 2020-04-03 11:41:54.000000 localcosmos_server-0.9.4/localcosmos_server/server_control_panel/templates/server_control_panel/install_app.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      642 2019-11-18 13:51:32.000000 localcosmos_server-0.9.4/localcosmos_server/server_control_panel/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9781 2020-08-28 07:52:24.000000 localcosmos_server-0.9.4/localcosmos_server/server_control_panel/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1902 2020-04-06 07:19:42.000000 localcosmos_server-0.9.4/localcosmos_server/settings.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1480 2020-04-03 11:16:36.000000 localcosmos_server-0.9.4/localcosmos_server/setup_forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      212 2019-11-11 14:22:30.000000 localcosmos_server-0.9.4/localcosmos_server/setup_urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1209 2019-11-11 14:29:58.000000 localcosmos_server-0.9.4/localcosmos_server/setup_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      663 2018-10-17 12:26:46.000000 localcosmos_server-0.9.4/localcosmos_server/slugifier.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.600216 localcosmos_server-0.9.4/localcosmos_server/specifications/
+-rw-r--r--   0 tom       (1000) tom       (1000)      650 2018-02-05 08:52:22.000000 localcosmos_server-0.9.4/localcosmos_server/specifications/DatasetJSON
+-rw-r--r--   0 tom       (1000) tom       (1000)      457 2020-08-28 07:52:24.000000 localcosmos_server-0.9.4/localcosmos_server/specifications/TaxonJSON
+-rw-r--r--   0 tom       (1000) tom       (1000)      277 2019-11-11 08:46:16.000000 localcosmos_server-0.9.4/localcosmos_server/specifications/TemporalJSON
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.600216 localcosmos_server-0.9.4/localcosmos_server/static/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.600216 localcosmos_server-0.9.4/localcosmos_server/static/fonts/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.600216 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Indie_Flower/
+-rw-r--r--   0 tom       (1000) tom       (1000)    55300 2011-03-08 22:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Indie_Flower/IndieFlower-Regular.ttf
+-rw-r--r--   0 tom       (1000) tom       (1000)    30372 2019-12-09 08:25:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Indie_Flower/IndieFlower-Regular.woff
+-rw-r--r--   0 tom       (1000) tom       (1000)     4455 2011-03-08 22:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Indie_Flower/OFL.txt
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.616217 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/
+-rw-r--r--   0 tom       (1000) tom       (1000)    11560 2013-01-08 22:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)   171072 2013-01-08 22:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0 tom       (1000) tom       (1000)    90428 2019-12-09 08:17:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Black.woff
+-rw-r--r--   0 tom       (1000) tom       (1000)   177120 2013-01-08 22:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0 tom       (1000) tom       (1000)    98056 2019-12-09 08:17:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-BlackItalic.woff
+-rw-r--r--   0 tom       (1000) tom       (1000)   170348 2013-01-08 22:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0 tom       (1000) tom       (1000)    90080 2019-12-09 08:17:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Bold.woff
+-rw-r--r--   0 tom       (1000) tom       (1000)   174520 2013-01-08 22:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0 tom       (1000) tom       (1000)    96000 2019-12-09 08:17:48.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-BoldItalic.woff
+-rw-r--r--   0 tom       (1000) tom       (1000)   173516 2013-01-08 22:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0 tom       (1000) tom       (1000)    95508 2019-12-09 08:17:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Italic.woff
+-rw-r--r--   0 tom       (1000) tom       (1000)   170012 2013-01-08 22:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0 tom       (1000) tom       (1000)    89436 2019-12-09 08:18:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Light.woff
+-rw-r--r--   0 tom       (1000) tom       (1000)   176184 2013-01-08 22:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0 tom       (1000) tom       (1000)    96712 2019-12-09 08:18:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-LightItalic.woff
+-rw-r--r--   0 tom       (1000) tom       (1000)   171656 2013-01-08 22:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0 tom       (1000) tom       (1000)    90328 2019-12-09 08:18:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Medium.woff
+-rw-r--r--   0 tom       (1000) tom       (1000)   176428 2013-01-08 22:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0 tom       (1000) tom       (1000)    97232 2019-12-09 08:18:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-MediumItalic.woff
+-rw-r--r--   0 tom       (1000) tom       (1000)   171272 2013-01-08 22:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0 tom       (1000) tom       (1000)    89596 2019-12-09 08:18:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Regular.woff
+-rw-r--r--   0 tom       (1000) tom       (1000)   171500 2013-01-08 22:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0 tom       (1000) tom       (1000)    87896 2019-12-09 08:18:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Thin.woff
+-rw-r--r--   0 tom       (1000) tom       (1000)   175872 2013-01-08 22:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0 tom       (1000) tom       (1000)    94564 2019-12-09 08:18:36.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-ThinItalic.woff
+-rw-r--r--   0 tom       (1000) tom       (1000)     6404 2019-12-09 08:26:44.000000 localcosmos_server-0.9.4/localcosmos_server/static/fonts/fonts.css
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.620216 localcosmos_server-0.9.4/localcosmos_server/static/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1000 2019-02-26 09:32:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/images/lclogo32.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1752 2020-04-23 06:44:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/images/local_cosmos_logo_40.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4881 2019-01-29 08:57:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/images/local_cosmos_logo_horizontal.png
+-rw-r--r--   0 tom       (1000) tom       (1000)    32016 2019-09-02 13:08:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/images/spinner.gif
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.620216 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.572217 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.620216 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/
+-rw-r--r--   0 tom       (1000) tom       (1000)    64548 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-grid.css
+-rw-r--r--   0 tom       (1000) tom       (1000)   151749 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-grid.css.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    48488 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css
+-rw-r--r--   0 tom       (1000) tom       (1000)   108539 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4897 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-reboot.css
+-rw-r--r--   0 tom       (1000) tom       (1000)    76483 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-reboot.css.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4021 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css
+-rw-r--r--   0 tom       (1000) tom       (1000)    32461 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 tom       (1000) tom       (1000)   192348 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap.css
+-rw-r--r--   0 tom       (1000) tom       (1000)   492048 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap.css.map
+-rw-r--r--   0 tom       (1000) tom       (1000)   155758 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap.min.css
+-rw-r--r--   0 tom       (1000) tom       (1000)   625953 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap.min.css.map
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.624217 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/
+-rw-r--r--   0 tom       (1000) tom       (1000)   222911 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.bundle.js
+-rw-r--r--   0 tom       (1000) tom       (1000)   402249 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.bundle.js.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    78635 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js
+-rw-r--r--   0 tom       (1000) tom       (1000)   311949 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 tom       (1000) tom       (1000)   131637 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.js
+-rw-r--r--   0 tom       (1000) tom       (1000)   250568 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.js.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    58072 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.min.js
+-rw-r--r--   0 tom       (1000) tom       (1000)   190253 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.min.js.map
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.624217 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/css/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1928 2022-04-25 10:19:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/css/localcosmos_server.css
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.624217 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)     7912 2016-11-06 13:33:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/Local-Cosmos-Logo.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2837 2018-07-09 07:40:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/add_image.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     1072 2022-04-20 09:47:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/arrow-tool-add.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4408 2022-04-20 10:19:51.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/arrow-tool-add.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      900 2022-04-20 09:48:47.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/arrow-tool-remove.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3934 2022-04-20 10:19:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/arrow-tool-remove.svg
+-rw-------   0 tom       (1000) tom       (1000)      797 2022-04-19 08:28:51.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/arrow-tool.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3448 2022-04-19 08:29:01.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/arrow-tool.svg
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.644217 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/
+-rw-r--r--   0 tom       (1000) tom       (1000)      171 2013-02-13 14:59:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/00.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ad.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ae.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/af.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ag.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ai.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/al.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 14:59:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/am.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/an.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      244 2013-02-13 14:59:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ao.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ar.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 15:00:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/as.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 14:59:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/at.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      378 2013-02-13 15:00:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/au.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 15:00:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/aw.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      376 2013-02-13 15:00:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ax.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/az.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ba.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 14:59:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/bb.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/bd.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 14:59:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/be.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      358 2013-02-13 14:59:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/bf.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/bg.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/bh.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      374 2013-02-13 15:00:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/bi.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/bj.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/bm.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      373 2013-02-13 15:00:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/bn.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 15:00:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/bo.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/br.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      351 2013-02-13 15:00:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/bs.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      377 2013-02-13 15:00:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/bt.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      376 2013-02-13 15:00:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/bv.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/bw.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/by.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/bz.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      376 2013-02-13 14:59:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ca.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      238 2013-02-13 14:59:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/catalonia.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/cc.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      243 2013-02-13 15:00:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/cd.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/cf.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 15:00:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/cg.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      332 2013-02-13 15:00:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ch.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 14:59:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ci.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ck.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/cl.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/cm.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/cn.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      353 2013-02-13 14:59:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/co.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 15:00:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/cr.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 14:59:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/cs.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 14:59:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/cu.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/cv.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 14:59:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/cx.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 14:59:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/cy.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/cz.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/de.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/dj.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      374 2013-02-13 14:59:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/dk.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/dm.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 14:59:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/do.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/dz.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ec.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ee.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/eg.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 15:00:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/eh.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      260 2013-02-13 14:59:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/en.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/england.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/er.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/es.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/et.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      171 2013-02-13 15:00:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/europeanunion.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/fam.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/fi.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/fj.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      372 2013-02-13 15:00:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/fk.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      377 2013-02-13 15:00:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/fm.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/fo.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/fr.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 15:00:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ga.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      260 2013-02-13 15:00:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/gb.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/gd.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      379 2013-02-13 15:00:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ge.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/gf.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      358 2013-02-13 15:00:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/gh.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 14:59:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/gi.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/gl.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/gm.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/gn.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      357 2013-02-13 15:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/gp.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/gq.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/gr.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 14:59:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/gs.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      374 2013-02-13 15:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/gt.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/gu.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      358 2013-02-13 14:59:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/gw.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/gy.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      373 2013-02-13 15:00:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/hk.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      378 2013-02-13 15:00:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/hm.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/hn.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/hr.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ht.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      357 2013-02-13 15:00:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/hu.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/id.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ie.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/il.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 14:59:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/in.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      373 2013-02-13 15:00:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/io.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/iq.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ir.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      373 2013-02-13 15:00:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/is.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/it.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ja.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 15:00:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/jm.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/jo.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/jp.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ke.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      373 2013-02-13 15:00:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/kg.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 14:59:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/kh.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 14:59:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ki.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      358 2013-02-13 15:00:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/km.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/kn.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/kp.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      385 2013-02-13 15:00:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/kr.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/kw.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      373 2013-02-13 15:00:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ky.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      374 2013-02-13 15:00:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/kz.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/la.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/lb.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      259 2013-02-13 15:00:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/lc.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 15:00:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/li.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      377 2013-02-13 15:00:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/lk.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/lr.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 14:59:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ls.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/lt.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/lu.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/lv.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ly.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ma.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 15:00:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/mc.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/md.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      238 2013-02-13 15:00:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/me.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      372 2013-02-13 15:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/mg.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/mh.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      382 2013-02-13 15:00:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/mk.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ml.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 15:00:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/mm.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 14:59:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/mn.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      378 2013-02-13 15:00:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/mo.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/mp.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      379 2013-02-13 15:00:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/mq.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      377 2013-02-13 15:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/mr.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 14:59:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ms.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/mt.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      358 2013-02-13 15:00:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/mu.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      372 2013-02-13 15:00:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/mv.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/mw.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/mx.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      375 2013-02-13 15:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/my.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/mz.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/na.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/nc.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ne.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      375 2013-02-13 14:59:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/nf.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ng.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ni.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/nl.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      376 2013-02-13 15:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/no.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      302 2013-02-13 15:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/np.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/nr.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/nu.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/nz.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/om.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/pa.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/pe.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/pf.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/pg.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ph.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      377 2013-02-13 14:59:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/pk.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 14:59:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/pl.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      374 2013-02-13 15:00:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/pm.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/pn.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/pr.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      358 2013-02-13 15:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ps.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/pt.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      374 2013-02-13 15:00:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/pw.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/py.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 14:59:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/qa.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/re.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ro.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      238 2013-02-13 15:00:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/rs.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 14:59:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ru.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 14:59:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/rw.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 14:59:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/sa.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/sb.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      357 2013-02-13 15:00:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/sc.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      378 2013-02-13 14:59:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/scotland.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      355 2013-02-13 15:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/sd.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/se.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/sg.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/sh.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      362 2013-02-13 15:00:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/si.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      376 2013-02-13 15:00:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/sj.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/sk.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 14:59:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/sl.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/sm.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/sn.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      376 2013-02-13 14:59:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/so.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/sr.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 14:59:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/st.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/sv.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/sy.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/sz.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/tc.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/td.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 15:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/tf.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/tg.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/th.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/tj.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      372 2013-02-13 15:00:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/tk.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/tl.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 14:59:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/tm.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      375 2013-02-13 15:00:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/tn.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/to.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/tr.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      377 2013-02-13 15:00:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/tt.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      361 2013-02-13 15:00:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/tv.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 15:00:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/tw.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 2013-02-13 15:00:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/tz.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      360 2013-02-13 15:00:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ua.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      359 2013-02-13 14:59:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ug.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      371 2013-02-13 15:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/um.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 2013-02-13 14:59:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/us.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      373 2013-02-13 15:00:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/uy.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 14:59:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/uz.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      369 2013-02-13 15:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/va.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 14:59:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/vc.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2013-02-13 15:00:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ve.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      368 2013-02-13 15:00:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/vg.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      376 2013-02-13 15:00:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/vi.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      370 2013-02-13 15:00:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/vn.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 15:00:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/vu.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      372 2013-02-13 15:00:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/wales.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      377 2013-02-13 15:00:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/wf.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 15:00:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ws.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      356 2013-02-13 14:59:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/ye.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      382 2013-02-13 15:00:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/yt.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      363 2013-02-13 15:00:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/za.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      358 2013-02-13 15:00:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/zm.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)      365 2013-02-13 15:00:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries/zw.gif
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.668217 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1933 2007-06-16 07:58:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_ASEAN.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      959 2007-06-16 07:58:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_African Union(OAS).png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2506 2007-06-16 07:58:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Arab League.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1888 2007-06-16 07:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_CARICOM.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2397 2007-06-16 07:58:46.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_CIS.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2387 2007-06-16 07:58:48.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Commonwealth.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      636 2007-06-16 07:58:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_England.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1847 2007-06-16 07:59:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_European Union.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2312 2007-06-16 07:59:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Islamic Conference.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1766 2008-07-16 19:21:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Kosovo.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1671 2007-06-16 07:59:44.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_NATO.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1202 2007-06-16 07:59:48.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Northern Cyprus.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1169 2007-06-19 18:05:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Northern Ireland.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1757 2007-06-16 07:59:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_OPEC.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4432 2008-11-02 15:41:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Olimpic Movement.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      501 2007-06-16 08:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Red Cross.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2434 2007-06-16 08:00:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Scotland.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1290 2007-06-16 08:00:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Somaliland.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2278 2007-06-16 08:01:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_United Nations.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2958 2007-06-16 08:01:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Wales.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1544 2007-06-16 07:58:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ad.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      837 2007-06-16 08:01:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ae.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2155 2007-06-16 07:58:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/af.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2089 2007-06-16 07:58:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ag.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2619 2007-06-19 09:59:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ai.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      787 2007-06-16 07:58:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/am.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1125 2007-10-11 14:48:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/an.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1540 2007-06-16 07:58:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ao.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1669 2007-06-16 07:58:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/aq.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      839 2007-06-16 07:58:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ar.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2554 2007-06-16 07:58:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/as.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      628 2007-06-16 07:58:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/at.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2623 2007-06-19 09:54:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/au.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1066 2007-06-16 07:58:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/aw.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1201 2007-06-16 07:58:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/az.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2343 2007-06-16 07:58:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ba.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1505 2007-06-16 07:58:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bb.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1447 2007-06-16 07:58:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bd.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      887 2007-06-16 07:58:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/be.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1071 2007-06-16 07:58:40.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bf.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      624 2007-06-16 07:58:40.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1256 2007-06-16 07:58:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bh.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2628 2007-06-16 07:58:40.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bi.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      773 2007-06-16 07:58:36.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bj.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2552 2007-10-11 14:37:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2408 2007-06-16 07:58:40.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1244 2007-06-16 07:58:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bo.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2549 2007-06-16 07:58:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/br.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1257 2007-06-16 07:58:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bs.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2351 2007-06-16 07:58:36.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bt.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      752 2007-06-16 07:58:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bw.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1467 2007-06-16 07:58:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/by.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2193 2007-06-16 07:58:36.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bz.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1484 2007-06-16 07:58:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ca.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2469 2007-06-16 07:58:48.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cd.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      986 2007-06-16 07:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cf.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1720 2007-06-16 07:58:48.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      828 2007-06-16 08:00:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ch.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      782 2007-06-16 07:58:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ci.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2683 2007-10-11 14:38:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ck.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      820 2007-06-16 07:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cl.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1131 2007-06-16 07:58:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1063 2007-06-16 07:58:46.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      676 2007-06-16 07:58:46.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/co.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      721 2007-06-16 07:58:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1508 2007-06-16 07:58:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cu.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1299 2007-06-16 07:58:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cv.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1125 2007-06-16 07:58:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cy.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1295 2007-06-16 07:58:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cz.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      809 2007-06-16 07:58:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/da.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      808 2007-06-16 07:59:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/de.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1456 2007-06-16 07:58:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/dj.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      809 2007-06-16 07:58:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/dk.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1946 2007-06-16 07:58:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/dm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      830 2007-06-16 07:58:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/do.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1445 2007-06-16 07:58:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/dz.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1628 2007-06-16 07:58:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ec.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      781 2007-06-16 07:58:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ee.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1020 2007-06-16 07:58:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/eg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1407 2007-06-16 08:01:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/eh.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2675 2007-06-16 08:01:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/en.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2588 2007-06-16 07:58:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/er.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1397 2007-06-16 08:00:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/es.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1646 2007-06-16 07:59:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/et.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      711 2007-06-16 07:59:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/fi.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2499 2007-06-16 07:59:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/fj.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1340 2007-06-16 07:59:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/fm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      838 2007-06-16 07:59:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/fo.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      941 2007-06-16 07:59:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/fr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      785 2007-06-16 07:59:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ga.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2675 2007-06-16 08:01:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gb.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2211 2007-06-16 07:59:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gd.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      841 2007-06-16 07:59:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ge.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1103 2008-07-16 18:40:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1146 2007-06-16 07:59:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gh.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1595 2007-10-11 14:39:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gi.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1206 2008-04-20 04:51:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gl.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      806 2007-06-16 07:59:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      962 2007-06-16 07:59:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1662 2008-04-20 04:56:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gp.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1569 2007-06-16 07:58:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gq.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      885 2007-06-16 07:59:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2038 2007-06-16 07:59:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gt.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1607 2007-10-11 14:39:46.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gu.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1121 2007-06-16 07:59:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gw.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2679 2007-06-16 07:59:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gy.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1748 2007-06-16 07:59:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/hk.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      955 2007-06-16 07:59:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/hn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1319 2007-06-16 07:58:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/hr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      784 2007-06-16 07:59:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ht.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      729 2007-06-16 07:59:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/hu.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      614 2007-06-16 07:59:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/id.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      882 2007-06-16 07:59:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ie.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1116 2007-06-16 07:59:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/il.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1660 2008-11-02 18:52:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/im.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1148 2007-06-16 07:59:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/in.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1158 2007-06-16 07:59:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/iq.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1372 2007-06-16 07:59:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ir.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1009 2007-06-16 07:59:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/is.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      861 2007-06-16 07:59:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/it.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1024 2007-06-16 07:59:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ja.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2382 2007-10-11 14:47:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/je.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2752 2007-06-16 07:59:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/jm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1512 2007-06-16 07:59:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/jo.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1024 2007-06-16 07:59:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/jp.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1791 2007-06-19 17:44:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ke.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1610 2007-06-16 07:59:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/kg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1440 2007-06-16 07:58:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/kh.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3269 2007-06-16 07:59:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ki.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1856 2007-06-16 07:58:48.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/km.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2324 2007-06-16 08:00:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/kn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1436 2007-06-16 07:59:48.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/kp.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2129 2007-06-16 08:00:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/kr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      987 2007-06-16 07:59:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/kw.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3021 2007-06-19 10:05:40.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ky.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2317 2007-06-16 07:59:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/kz.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1179 2007-06-16 07:59:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/la.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1274 2007-06-16 07:59:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/lb.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1600 2007-06-16 08:00:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/lc.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1242 2007-06-16 07:59:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/li.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2136 2007-06-16 08:00:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/lk.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1171 2007-06-16 07:59:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/lr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2216 2007-06-16 07:59:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ls.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      744 2007-06-16 07:59:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/lt.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      635 2007-06-16 07:59:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/lu.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      803 2007-06-16 07:59:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/lv.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      919 2007-06-16 07:59:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ly.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1109 2007-06-16 07:59:40.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ma.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      612 2007-06-16 07:59:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mc.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1655 2007-06-16 07:59:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/md.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1977 2007-06-16 07:59:40.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/me.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      742 2007-06-16 07:59:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2839 2007-06-16 07:59:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mh.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2996 2007-06-16 07:59:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mk.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      924 2007-06-16 07:59:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ml.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1631 2007-06-16 07:59:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1420 2007-06-16 07:59:40.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2333 2007-06-16 07:59:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mo.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2558 2008-04-20 04:58:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mq.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1602 2007-06-16 07:59:36.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2399 2007-10-11 14:48:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ms.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      869 2007-06-16 07:59:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mt.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      819 2007-06-16 07:59:36.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mu.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1115 2007-06-16 07:59:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mv.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1259 2007-07-06 08:48:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mw.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1555 2007-06-16 07:59:36.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mx.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1575 2007-06-16 07:59:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/my.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1733 2007-06-16 07:59:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mz.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2862 2007-06-16 07:59:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/na.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2114 2008-07-16 18:38:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/nc.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      878 2007-06-16 07:59:46.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ne.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      781 2007-06-16 07:59:48.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ng.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1026 2007-06-16 07:59:46.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ni.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      635 2007-06-16 07:59:44.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/nl.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      935 2007-06-16 07:59:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/no.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2026 2007-07-01 22:34:44.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/np.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1216 2007-06-16 07:59:44.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/nr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2182 2007-06-16 07:59:46.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/nz.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1145 2007-06-16 07:59:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/om.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1053 2007-06-16 07:59:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/pa.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1560 2007-06-16 07:59:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/pe.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1294 2007-10-11 14:39:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/pf.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2075 2007-06-16 07:59:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/pg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1564 2007-06-16 07:59:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ph.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1448 2007-06-16 07:59:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/pk.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      491 2007-06-16 07:59:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/pl.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1398 2007-06-16 08:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/pr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1255 2007-06-16 07:59:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ps.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1797 2007-06-16 07:59:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/pt.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1313 2007-06-16 07:59:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/pw.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1052 2007-06-16 07:59:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/py.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1181 2007-06-16 08:00:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/qa.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1991 2008-04-20 05:02:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/re.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      900 2007-06-16 08:00:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ro.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1698 2007-06-16 08:00:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/rs.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      551 2007-06-16 08:00:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ru.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1079 2007-06-16 08:00:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/rw.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2035 2007-06-16 08:00:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sa.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2317 2007-06-16 08:00:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sb.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2177 2007-06-16 08:00:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sc.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1246 2007-06-16 08:00:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sd.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      906 2007-06-16 08:00:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/se.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1031 2007-06-16 08:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1041 2007-06-16 08:00:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/si.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1344 2007-06-16 08:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sk.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      655 2007-06-16 08:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sl.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1935 2007-06-16 08:00:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1223 2007-06-16 08:00:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1181 2007-06-16 08:00:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/so.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1747 2007-06-16 07:58:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sq.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1015 2007-06-16 08:00:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1282 2007-06-16 08:00:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/st.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1092 2007-06-16 07:58:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sv.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      978 2007-06-16 08:00:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sy.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2298 2007-06-16 08:00:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sz.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2503 2007-10-11 14:48:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tc.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      889 2007-06-16 07:58:44.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/td.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1085 2007-06-16 08:00:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      674 2007-06-16 08:00:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/th.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1158 2007-06-16 08:00:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tj.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1744 2007-06-16 08:00:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tl.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2070 2007-06-16 08:00:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1664 2007-06-16 08:00:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      787 2007-06-16 08:00:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/to.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1580 2007-06-16 08:00:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2351 2007-06-16 08:00:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tt.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2398 2007-06-16 08:00:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tv.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1309 2007-06-16 08:00:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tw.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2197 2007-06-16 08:00:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tz.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      737 2007-06-16 08:01:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ua.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1229 2007-06-16 08:01:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ug.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1101 2007-07-04 20:12:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/us.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1144 2007-06-16 08:01:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/uy.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      971 2007-06-16 08:01:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/uz.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1281 2007-06-16 08:01:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/va.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1381 2007-06-16 08:00:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/vc.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1108 2007-06-16 08:01:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ve.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2767 2007-10-11 14:37:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/vg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2425 2007-10-11 14:48:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/vi.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1174 2007-06-16 08:01:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/vn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2057 2007-06-16 08:01:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/vu.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1369 2007-06-16 08:00:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ws.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      696 2007-06-16 08:01:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ye.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2095 2007-06-16 08:00:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/za.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1209 2007-06-16 08:01:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/zm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1746 2007-06-16 08:01:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/zw.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.684217 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4407 2008-01-09 14:16:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Algeria.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5651 2008-01-09 14:17:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/British_Virgin_Islands.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5884 2008-01-09 14:18:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Cayman_Islands.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2909 2008-01-09 14:18:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Chad.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4825 2008-01-09 14:18:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Comoros.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5032 2008-01-09 14:18:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Democratic_Republic_of_the_Congo.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4416 2008-01-09 14:19:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/French_Polynesia.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2913 2008-01-09 14:22:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Latvia.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3991 2008-01-09 14:23:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Micronesia.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3785 2008-01-09 14:24:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/North_Korea.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3797 2008-01-09 14:24:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Oman.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5479 2008-01-09 14:25:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Saint_Kitts_and_Nevis.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4012 2008-01-09 14:25:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Saint_Lucia.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     8662 2008-01-09 14:26:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Saint_Pierre.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3831 2008-01-09 14:26:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Saint_Vicent_and_the_Grenadines.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3592 2008-01-09 14:26:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Samoa.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3183 2008-01-09 14:27:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Soviet_Union.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5640 2008-01-09 14:27:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Sri_Lanka.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     8289 2008-01-09 14:28:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Tibet.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     6644 2008-01-09 14:28:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Tuvalu.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4421 2008-01-09 14:16:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ad.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2971 2008-01-09 14:28:44.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ae.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4786 2008-01-09 14:15:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/af.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5085 2008-01-09 14:16:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ag.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5469 2008-01-09 14:16:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ai.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5037 2008-01-09 14:15:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/al.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3002 2008-01-09 14:16:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/am.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3776 2008-01-09 14:24:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/an.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4127 2008-01-09 14:16:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ao.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3319 2008-01-09 14:16:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ar.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5785 2008-01-09 14:16:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/as.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2889 2008-01-09 14:16:36.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/at.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5985 2008-01-09 14:16:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/au.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3579 2008-01-09 14:16:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/aw.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3609 2008-01-09 14:16:40.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/az.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4854 2008-01-09 14:17:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ba.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3938 2008-01-09 14:16:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bb.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3854 2008-01-09 14:16:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bd.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2906 2008-01-09 14:17:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/be.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3349 2008-01-09 14:17:44.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bf.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2912 2008-01-09 14:17:40.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3591 2008-01-09 14:16:46.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bh.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5935 2008-01-09 14:17:48.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bi.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2958 2008-01-09 14:17:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bj.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5563 2008-01-09 14:17:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5350 2008-01-09 14:17:36.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3936 2008-01-09 14:17:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bo.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     6182 2008-01-09 14:17:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/br.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3563 2008-01-09 14:16:44.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bs.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     6629 2008-01-09 14:17:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bt.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2961 2008-01-09 14:17:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bw.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3913 2008-01-09 14:16:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/by.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5497 2008-01-09 14:17:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bz.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3895 2008-01-09 14:17:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ca.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3599 2008-01-09 14:18:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cf.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4046 2008-01-09 14:25:40.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3184 2008-01-09 14:27:46.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ch.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2894 2008-01-09 14:18:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ci.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     6864 2008-01-09 14:18:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ck.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3428 2008-01-09 14:18:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cl.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3314 2008-01-09 14:17:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3817 2008-01-09 14:18:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2957 2008-01-09 14:18:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/co.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2946 2008-01-09 14:18:36.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3986 2008-01-09 14:18:46.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cu.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4870 2008-01-09 14:18:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cv.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5479 2008-01-09 14:18:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cx.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3928 2008-01-09 14:18:48.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cy.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3887 2008-01-09 14:18:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cz.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2924 2008-01-09 14:20:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/de.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3823 2008-01-09 14:19:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/dj.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3045 2008-01-09 14:19:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/dk.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4408 2008-01-09 14:19:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/dm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3053 2008-01-09 14:19:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/do.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3963 2008-01-09 14:19:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ec.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2925 2008-01-09 14:19:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ee.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3313 2008-01-09 14:19:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/eg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     6236 2008-01-09 14:28:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/en.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5613 2008-01-09 14:19:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/er.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2935 2008-01-09 14:27:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/es.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3918 2008-01-09 14:19:36.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/et.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3077 2008-01-09 14:19:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/fi.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5640 2008-01-09 14:19:46.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/fj.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5688 2008-01-09 14:19:40.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/fk.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3352 2008-01-09 14:19:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/fo.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2892 2008-01-09 14:19:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/fr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2957 2008-01-09 14:20:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ga.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     6236 2008-01-09 14:28:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gb.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5287 2008-01-09 14:20:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gd.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4941 2008-01-09 14:20:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ge.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2892 2008-01-09 14:23:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gf.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3447 2008-01-09 14:20:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gh.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3821 2008-01-09 14:20:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gi.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3938 2008-01-09 14:20:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gl.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2935 2008-01-09 14:20:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2907 2008-01-09 14:20:40.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4360 2008-01-09 14:19:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gq.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3374 2008-01-09 14:20:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3967 2008-01-09 14:20:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gt.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4348 2008-01-09 14:20:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gu.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3281 2008-01-09 14:20:44.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gw.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5486 2008-01-09 14:20:48.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gy.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4659 2008-01-09 14:20:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/hk.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3283 2008-01-09 14:20:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/hn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4128 2008-01-09 14:18:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/hr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2938 2008-01-09 14:20:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ht.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2894 2008-01-09 14:21:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/hu.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2881 2008-01-09 14:21:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/id.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2883 2008-01-09 14:21:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ie.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4091 2008-01-09 14:21:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/il.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3809 2008-01-09 14:21:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/in.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4008 2008-01-09 14:21:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/iq.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4982 2008-01-09 14:21:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ir.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3243 2008-01-09 14:21:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/is.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2889 2008-01-09 14:21:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/it.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4978 2008-01-09 14:21:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/jm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3737 2008-01-09 14:21:40.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/jo.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3714 2008-01-09 14:21:36.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/jp.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4959 2008-01-09 14:21:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ke.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4575 2008-01-09 14:22:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/kg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4819 2008-01-09 14:17:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/kh.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     7486 2008-01-09 14:21:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ki.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3339 2008-01-09 14:21:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/kw.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5088 2008-01-09 14:21:44.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/kz.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3667 2008-01-09 14:22:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/la.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4266 2008-01-09 14:22:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/lb.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3826 2008-01-09 14:22:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/li.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3559 2008-01-09 14:22:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/lr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5558 2008-01-09 14:22:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ls.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2945 2008-01-09 14:22:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/lt.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2904 2008-01-09 14:22:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/lu.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2873 2008-01-09 14:22:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ly.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3737 2008-01-09 14:23:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ma.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2905 2008-01-09 14:23:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mc.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4014 2008-01-09 14:23:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/md.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2928 2008-01-09 14:22:46.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     6053 2008-01-09 14:23:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mh.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5892 2008-01-09 14:22:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mk.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2910 2008-01-09 14:23:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ml.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4119 2008-01-09 14:23:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3552 2008-01-09 14:23:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5963 2008-01-09 14:22:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mo.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4412 2008-01-09 14:23:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5254 2008-01-09 14:23:46.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ms.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3411 2008-01-09 14:23:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mt.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2940 2008-01-09 14:23:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mu.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3631 2008-01-09 14:22:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mv.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3770 2008-01-09 14:22:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mw.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4229 2008-01-09 14:23:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mx.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4346 2008-01-09 14:22:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/my.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4511 2008-01-09 14:23:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mz.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     6560 2008-01-09 14:24:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/na.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3259 2008-01-09 14:24:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ne.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4302 2008-01-09 14:24:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/nf.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2898 2008-01-09 14:24:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ng.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3567 2008-01-09 14:24:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ni.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2937 2008-01-09 14:24:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/nl.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3283 2008-01-09 14:24:46.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/no.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5530 2008-01-09 14:24:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/np.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3565 2008-01-09 14:24:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/nr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4877 2008-01-09 14:24:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/nu.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5439 2008-01-09 14:24:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/nz.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3986 2008-01-09 14:25:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pa.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2898 2008-01-09 14:25:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pe.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5518 2008-01-09 14:25:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4326 2008-01-09 14:25:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ph.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4161 2008-01-09 14:24:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pk.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2891 2008-01-09 14:25:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pl.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     6397 2008-01-09 14:25:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4429 2008-01-09 14:25:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4803 2008-01-09 14:25:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pt.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3927 2008-01-09 14:25:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pw.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3673 2008-01-09 14:25:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/py.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3645 2008-01-09 14:25:36.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/qa.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2909 2008-01-09 14:25:44.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ro.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2928 2008-01-09 14:26:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/rs.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2941 2008-01-09 14:25:48.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ru.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4154 2008-01-09 14:25:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/rw.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5828 2008-01-09 14:26:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sa.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5260 2008-01-09 14:26:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sb.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4826 2008-01-09 14:26:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sc.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3569 2008-01-09 14:27:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sd.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3107 2008-01-09 14:27:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/se.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3936 2008-01-09 14:26:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5523 2008-01-09 14:27:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sh.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3804 2008-01-09 14:26:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/si.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4266 2008-01-09 14:26:48.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sk.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2944 2008-01-09 14:26:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sl.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2911 2008-01-09 14:26:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3332 2008-01-09 14:26:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3705 2008-01-09 14:27:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/so.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3438 2008-01-09 14:27:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4325 2008-01-09 14:26:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/st.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3621 2008-01-09 14:19:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sv.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3615 2008-01-09 14:27:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sy.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5551 2008-01-09 14:27:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sz.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5396 2008-01-09 14:28:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tc.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3529 2008-01-09 14:28:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tg.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2942 2008-01-09 14:28:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/th.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3497 2008-01-09 14:27:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tj.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4314 2008-01-09 14:28:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tl.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4960 2008-01-09 14:28:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4200 2008-01-09 14:28:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3222 2008-01-09 14:28:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/to.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4169 2008-01-09 14:28:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tr.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5314 2008-01-09 14:28:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tt.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4019 2008-01-09 14:27:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tw.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5086 2008-01-09 14:28:02.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tz.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2887 2008-01-09 14:28:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ua.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3711 2008-01-09 14:28:48.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ug.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5012 2008-01-09 14:29:08.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/us.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4421 2008-01-09 14:29:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/uy.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3712 2008-01-09 14:29:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/uz.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4810 2008-01-09 14:29:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/va.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3457 2008-01-09 14:29:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ve.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     7301 2008-01-09 14:29:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/vi.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3649 2008-01-09 14:29:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/vn.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5234 2008-01-09 14:29:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/vu.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4295 2008-01-09 14:29:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/wf.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2873 2008-01-09 14:29:34.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ye.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5558 2008-01-09 14:27:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/yt.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5252 2008-01-09 14:27:06.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/za.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3778 2008-01-09 14:29:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/zm.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4354 2008-01-09 14:29:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/zw.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      386 2022-04-19 07:52:49.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/crop-tool.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2144 2022-04-19 07:52:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/crop-tool.svg
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.684217 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/interactive-image-field/
+-rw-r--r--   0 tom       (1000) tom       (1000)      883 2022-04-26 06:39:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/interactive-image-field/InteractiveImageField.css
+-rw-r--r--   0 tom       (1000) tom       (1000)    49259 2022-05-05 15:59:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/interactive-image-field/InteractiveImageField.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    86927 2019-04-02 08:38:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/jquery-3.3.1.min.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.684217 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/js/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1239 2018-12-10 19:21:28.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/js/ajax_file_input.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    22466 2019-10-16 06:19:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/js/bootstrap3-typeahead.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1570 2018-11-26 15:47:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/js/django-ajax-csrf.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2176 2021-07-14 16:31:12.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/js/django-ajax.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3605 2021-08-13 07:36:20.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/js/jquery-taxon-autocomplete.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      964 2019-09-30 09:01:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/js/jquery-user-autocomplete.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1015 2019-09-26 07:50:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/js/localcosmos_server.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    20337 2018-06-11 12:10:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/js/popper.min.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.684217 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/konva/
+-rw-r--r--   0 tom       (1000) tom       (1000)   157749 2022-04-27 12:18:11.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/konva/konva.min.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.688217 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/
+-rw-r--r--   0 tom       (1000) tom       (1000)    55182 2017-07-24 08:54:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/Spin.gif
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.572217 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.688217 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/
+-rw-r--r--   0 tom       (1000) tom       (1000)    64548 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-grid.css
+-rw-r--r--   0 tom       (1000) tom       (1000)   151749 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-grid.css.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    48488 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css
+-rw-r--r--   0 tom       (1000) tom       (1000)   108539 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4897 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-reboot.css
+-rw-r--r--   0 tom       (1000) tom       (1000)    76483 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-reboot.css.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4021 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css
+-rw-r--r--   0 tom       (1000) tom       (1000)    32461 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 tom       (1000) tom       (1000)   192348 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap.css
+-rw-r--r--   0 tom       (1000) tom       (1000)   492048 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap.css.map
+-rw-r--r--   0 tom       (1000) tom       (1000)   155758 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap.min.css
+-rw-r--r--   0 tom       (1000) tom       (1000)   625953 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap.min.css.map
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.688217 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/
+-rw-r--r--   0 tom       (1000) tom       (1000)   222911 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.bundle.js
+-rw-r--r--   0 tom       (1000) tom       (1000)   402249 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.bundle.js.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    78635 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js
+-rw-r--r--   0 tom       (1000) tom       (1000)   311949 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 tom       (1000) tom       (1000)   131637 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.js
+-rw-r--r--   0 tom       (1000) tom       (1000)   250568 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.js.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    58072 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.min.js
+-rw-r--r--   0 tom       (1000) tom       (1000)   190253 2019-02-13 13:47:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.min.js.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      157 2019-01-31 14:44:04.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/error_page.css
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.688217 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/jquery/
+-rw-r--r--   0 tom       (1000) tom       (1000)    86927 2019-01-29 09:02:48.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/jquery/jquery-3.3.1.min.js
+-rw-r--r--   0 tom       (1000) tom       (1000)   132382 2019-01-29 09:02:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/jquery/jquery-3.3.1.min.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1187 2016-11-11 17:35:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/lc_setup.css
+-rw-r--r--   0 tom       (1000) tom       (1000)     7912 2016-11-06 13:33:32.000000 localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/logo100blue.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.572217 localcosmos_server-0.9.4/localcosmos_server/static/maps/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.692216 localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.692216 localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1259 2019-05-08 16:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/images/layers-2x.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      696 2019-05-08 16:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/images/layers.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2464 2019-05-08 16:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/images/marker-icon-2x.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1466 2019-05-08 16:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/images/marker-icon.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      618 2019-05-08 16:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/images/marker-shadow.png
+-rw-r--r--   0 tom       (1000) tom       (1000)   405077 2019-05-08 16:01:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/leaflet-src.esm.js
+-rw-r--r--   0 tom       (1000) tom       (1000)   770515 2019-05-08 16:01:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/leaflet-src.esm.js.map
+-rw-r--r--   0 tom       (1000) tom       (1000)   406844 2019-05-08 16:01:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/leaflet-src.js
+-rw-r--r--   0 tom       (1000) tom       (1000)   770609 2019-05-08 16:01:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/leaflet-src.js.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    14268 2019-05-08 16:00:10.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/leaflet.css
+-rw-r--r--   0 tom       (1000) tom       (1000)   141833 2019-05-08 16:01:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/leaflet.js
+-rw-r--r--   0 tom       (1000) tom       (1000)   195157 2019-05-08 16:01:22.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/leaflet.js.map
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.696216 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1727 2019-09-10 05:42:58.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Amphibia.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1945 2019-09-10 05:41:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Animalia.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1677 2019-09-10 05:44:44.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Anura.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1622 2019-09-10 05:46:16.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Arachnida.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1883 2019-09-10 05:47:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Arthropoda.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1395 2019-09-10 05:48:50.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Aves.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2042 2019-09-10 05:50:30.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Chordata.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1914 2019-09-10 05:51:42.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Coleoptera.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1793 2019-09-10 05:52:54.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Fungi.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1809 2019-09-10 05:54:26.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Holocephali,Elasmobranchii,Sarcopterygii,Actinopterygii.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2010 2019-09-10 05:55:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Insecta.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1619 2019-09-10 05:56:56.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Lepidoptera.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1667 2019-09-10 05:58:18.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Mammalia.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1712 2019-09-10 05:59:24.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Mollucsa.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1616 2019-09-10 06:00:38.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Odonata.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1617 2019-09-09 14:21:40.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Plantae.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1357 2019-09-09 14:12:14.000000 localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/marker_unknown.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     6405 2016-08-24 16:02:52.000000 localcosmos_server-0.9.4/localcosmos_server/static/noimage.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.712216 localcosmos_server-0.9.4/localcosmos_server/static/octicons/
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/alert.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      265 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/archive.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      135 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/arrow-both.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      144 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/arrow-down.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      145 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/arrow-left.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      145 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/arrow-right.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      142 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/arrow-small-down.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      142 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/arrow-small-left.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      142 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/arrow-small-right.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      142 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/arrow-small-up.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      144 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/arrow-up.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      297 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/beaker.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      311 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/bell.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      397 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/bold.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      352 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/book.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/bookmark.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      283 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/briefcase.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      686 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/broadcast.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      268 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/browser.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      438 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/bug.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      588 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/calendar.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      162 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/check.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      399 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/checklist.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      164 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/chevron-down.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      162 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/chevron-left.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      161 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/chevron-right.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      166 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/chevron-up.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      349 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/circle-slash.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      695 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/circuit-board.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      455 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/clippy.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      306 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/clock.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      429 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/cloud-download.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      429 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/cloud-upload.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      207 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/code.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      330 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/comment-discussion.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      237 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/comment.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      258 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/credit-card.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      132 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/dash.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      531 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/dashboard.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      524 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/database.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      376 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/dependent.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      299 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/desktop-download.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      269 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/device-camera-video.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      396 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/device-camera.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      272 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/device-desktop.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      307 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/device-mobile.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      246 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/diff-added.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      252 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/diff-ignored.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      273 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/diff-modified.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      231 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/diff-removed.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      239 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/diff-renamed.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      288 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/diff.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      239 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/ellipsis.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      685 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/eye-closed.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      327 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/eye.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      320 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/file-binary.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      304 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/file-code.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      234 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/file-directory.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      239 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/file-media.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      976 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/file-pdf.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      301 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/file-submodule.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      354 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/file-symlink-directory.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      339 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/file-symlink-file.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      348 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/file-zip.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      268 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/file.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      497 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/flame.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      320 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/fold-down.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      316 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/fold-up.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      329 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/fold.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      457 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/gear.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      788 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/gift.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      365 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/gist-secret.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      321 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/gist.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      772 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/git-branch.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      338 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/git-commit.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      643 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/git-compare.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      724 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/git-merge.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      693 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/git-pull-request.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      290 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/github-action.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     1874 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/globe.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      159 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/grabber.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      184 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/graph.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      362 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/heart.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      358 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/history.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      241 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/home.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      217 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/horizontal-rule.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      443 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/hubot.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      375 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/inbox.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      632 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/info.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      385 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/issue-closed.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      299 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/issue-opened.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      487 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/issue-reopened.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      247 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/italic.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      718 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/jersey.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      249 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/kebab-horizontal.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      247 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/kebab-vertical.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      461 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/key.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      486 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/keyboard.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      490 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/law.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      571 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/light-bulb.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      245 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/link-external.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      454 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/link.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      939 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/list-ordered.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      632 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/list-unordered.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      395 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/location.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      351 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/lock.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     1009 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/logo-gist.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     1945 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/logo-github.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      395 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/mail-read.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      285 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/mail.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      691 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/mark-github.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      324 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/markdown.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      466 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/megaphone.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      677 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/mention.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      213 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/milestone.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      288 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/mirror.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      548 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/mortar-board.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      360 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/mute.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      374 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/no-newline.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      254 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/note.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      708 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/octoface.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      531 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/organization.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      445 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/package.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      644 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/paintcan.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      242 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/pencil.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      334 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/person.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      273 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/pin.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      257 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/play.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      248 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/plug.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      148 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/plus-small.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      151 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/plus.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      170 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/primitive-dot.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      133 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/primitive-square.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      255 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/project.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      205 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/pulse.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      421 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/question.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      465 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/quote.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     1093 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/radio-tower.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      190 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/reply.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      400 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/repo-clone.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      276 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/repo-force-push.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      583 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/repo-forked.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      336 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/repo-pull.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      289 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/repo-push.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      367 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/repo-template-private.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      311 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/repo-template.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      312 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/repo.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      255 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/report.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      276 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/request-changes.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      599 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/rocket.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      236 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/rss.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      199 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/ruby.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      297 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/screen-full.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      366 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/screen-normal.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      403 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/search.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      532 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/server.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      395 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/settings.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      404 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/shield-check.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      330 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/shield-lock.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      465 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/shield-x.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      306 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/shield.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      272 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/sign-in.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      261 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/sign-out.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      281 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/skip.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      895 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/smiley.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      536 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/squirrel.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      202 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/star.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      223 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/stop.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      430 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/sync.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      419 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/tag.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      430 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/tasklist.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      425 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/telescope.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      275 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/terminal.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      333 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/text-size.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      376 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/three-bars.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      600 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/thumbsdown.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      610 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/thumbsup.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      542 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/tools.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      324 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/trashcan.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      136 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/triangle-down.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      134 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/triangle-left.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      136 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/triangle-right.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      140 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/triangle-up.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      320 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/unfold.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      619 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/unmute.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     1364 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/unverified.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      737 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/verified.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      319 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/versions.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      368 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/watch.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      237 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/x.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      148 1985-10-26 07:15:00.000000 localcosmos_server-0.9.4/localcosmos_server/static/octicons/zap.svg
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.712216 localcosmos_server-0.9.4/localcosmos_server/taxonomy/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2805 2020-09-04 07:10:42.000000 localcosmos_server-0.9.4/localcosmos_server/taxonomy/AppTaxonSearch.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2019-03-25 08:50:38.000000 localcosmos_server-0.9.4/localcosmos_server/taxonomy/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2342 2020-08-28 07:52:24.000000 localcosmos_server-0.9.4/localcosmos_server/taxonomy/fields.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1389 2019-12-10 08:05:46.000000 localcosmos_server-0.9.4/localcosmos_server/taxonomy/forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6758 2020-08-28 07:52:24.000000 localcosmos_server-0.9.4/localcosmos_server/taxonomy/generic.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    12334 2022-05-13 14:06:05.000000 localcosmos_server-0.9.4/localcosmos_server/taxonomy/lazy.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      531 2019-09-23 14:52:16.000000 localcosmos_server-0.9.4/localcosmos_server/taxonomy/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4559 2022-05-13 14:09:27.000000 localcosmos_server-0.9.4/localcosmos_server/taxonomy/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2497 2020-08-28 07:52:24.000000 localcosmos_server-0.9.4/localcosmos_server/taxonomy/widgets.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.716216 localcosmos_server-0.9.4/localcosmos_server/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)      259 2020-03-16 08:59:56.000000 localcosmos_server-0.9.4/localcosmos_server/templates/400.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      316 2019-02-27 08:46:14.000000 localcosmos_server-0.9.4/localcosmos_server/templates/403.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      286 2019-02-27 07:57:46.000000 localcosmos_server-0.9.4/localcosmos_server/templates/404.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      303 2019-02-27 07:57:50.000000 localcosmos_server-0.9.4/localcosmos_server/templates/500.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.716216 localcosmos_server-0.9.4/localcosmos_server/templates/anycluster/
+-rw-r--r--   0 tom       (1000) tom       (1000)      493 2019-09-19 13:09:12.000000 localcosmos_server-0.9.4/localcosmos_server/templates/anycluster/clusterPopup.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     3234 2022-04-28 07:07:42.000000 localcosmos_server-0.9.4/localcosmos_server/templates/base.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.716216 localcosmos_server-0.9.4/localcosmos_server/templates/content_licencing/
+-rw-r--r--   0 tom       (1000) tom       (1000)       86 2018-02-26 06:39:00.000000 localcosmos_server-0.9.4/localcosmos_server/templates/content_licencing/licencing_form.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.716216 localcosmos_server-0.9.4/localcosmos_server/templates/content_licencing/widgets/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1096 2019-10-09 13:30:06.000000 localcosmos_server-0.9.4/localcosmos_server/templates/content_licencing/widgets/licence_select_widget.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.576217 localcosmos_server-0.9.4/localcosmos_server/templates/django/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.576217 localcosmos_server-0.9.4/localcosmos_server/templates/django/forms/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.716216 localcosmos_server-0.9.4/localcosmos_server/templates/django/forms/widgets/
+-rw-r--r--   0 tom       (1000) tom       (1000)      172 2018-05-22 12:17:28.000000 localcosmos_server-0.9.4/localcosmos_server/templates/django/forms/widgets/attrs.html
+-rw-r--r--   0 tom       (1000) tom       (1000)       96 2019-10-01 08:40:08.000000 localcosmos_server-0.9.4/localcosmos_server/templates/django/forms/widgets/checkbox.html
+-rw-r--r--   0 tom       (1000) tom       (1000)       97 2019-10-09 13:10:16.000000 localcosmos_server-0.9.4/localcosmos_server/templates/django/forms/widgets/file.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      243 2019-10-09 13:10:00.000000 localcosmos_server-0.9.4/localcosmos_server/templates/django/forms/widgets/input.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      406 2019-10-09 13:29:18.000000 localcosmos_server-0.9.4/localcosmos_server/templates/django/forms/widgets/select.html
+-rw-r--r--   0 tom       (1000) tom       (1000)       48 2018-05-22 12:17:28.000000 localcosmos_server-0.9.4/localcosmos_server/templates/django/forms/widgets/text.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      166 2019-10-01 08:49:18.000000 localcosmos_server-0.9.4/localcosmos_server/templates/django/forms/widgets/textarea.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.716216 localcosmos_server-0.9.4/localcosmos_server/templates/el_pagination/
+-rw-r--r--   0 tom       (1000) tom       (1000)      152 2019-09-30 11:54:52.000000 localcosmos_server-0.9.4/localcosmos_server/templates/el_pagination/current_link.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      187 2018-05-22 12:19:12.000000 localcosmos_server-0.9.4/localcosmos_server/templates/el_pagination/next_link.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      207 2021-07-25 12:28:38.000000 localcosmos_server-0.9.4/localcosmos_server/templates/el_pagination/page_link.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      187 2019-09-30 11:46:50.000000 localcosmos_server-0.9.4/localcosmos_server/templates/el_pagination/previous_link.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      429 2018-05-22 12:19:12.000000 localcosmos_server-0.9.4/localcosmos_server/templates/el_pagination/show_more.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      267 2019-09-30 11:59:12.000000 localcosmos_server-0.9.4/localcosmos_server/templates/el_pagination/show_pages.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.716216 localcosmos_server-0.9.4/localcosmos_server/templates/email/
+-rw-r--r--   0 tom       (1000) tom       (1000)     7594 2020-04-24 08:20:18.000000 localcosmos_server-0.9.4/localcosmos_server/templates/email/registration_confirmation.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      787 2020-04-24 11:06:10.000000 localcosmos_server-0.9.4/localcosmos_server/templates/email/registration_confirmation.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)     1338 2020-03-16 09:09:30.000000 localcosmos_server-0.9.4/localcosmos_server/templates/error_base.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.716216 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.716216 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/api/
+-rw-r--r--   0 tom       (1000) tom       (1000)      315 2019-12-09 13:59:26.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/api/delete_account.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.716216 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/api/legal/
+-rw-r--r--   0 tom       (1000) tom       (1000)    15879 2020-04-21 14:55:30.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/api/legal/privacy_statement.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      348 2019-12-09 11:39:04.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/api/manage_account.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1227 2020-04-22 12:14:26.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/api/password_reset_form.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      790 2019-12-09 14:43:34.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/api/register_account.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     3398 2020-01-23 07:55:02.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/bootstrap_field.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      190 2019-10-01 09:15:46.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/bootstrap_form.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.716216 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/generic/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1390 2020-04-03 11:21:58.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/generic/delete_object.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.716216 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/legal/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1312 2020-05-11 08:32:06.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/legal/base.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      929 2020-04-24 07:44:54.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/legal/legal_notice.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      549 2020-04-24 07:55:48.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/legal/privacy_statement.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.716216 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/modals/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.716216 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/modals/footers/
+-rw-r--r--   0 tom       (1000) tom       (1000)      213 2019-10-09 12:42:50.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/modals/footers/add_selected.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      122 2019-10-09 13:35:20.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/modals/footers/close.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      198 2019-10-09 13:35:30.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/modals/footers/delete.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      205 2020-04-03 11:22:44.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/modals/footers/save.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      204 2020-04-03 11:22:50.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/modals/footers/save_close.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      323 2019-09-19 13:04:32.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/modals/large_modal_base.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      405 2019-09-19 13:04:24.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/modals/large_modal_form.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      869 2019-09-20 08:50:12.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/modals/modal_base.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      322 2019-09-19 13:04:16.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/modals/modal_form.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.716216 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/
+-rw-r--r--   0 tom       (1000) tom       (1000)      827 2020-04-03 11:23:34.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/loggedout.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1552 2020-04-03 11:23:52.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/login.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      450 2019-11-14 14:44:22.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/password_change_done.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      817 2019-11-14 14:44:26.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/password_change_form.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      545 2020-04-03 11:24:16.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/password_reset_complete.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      997 2020-04-03 11:24:26.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/password_reset_confirm.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      663 2019-11-14 14:44:40.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/password_reset_done.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      582 2020-04-22 12:58:14.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/password_reset_email.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      857 2019-11-14 14:44:44.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/password_reset_form.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.716216 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/setup/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1569 2020-05-11 08:28:24.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/setup/base.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      752 2020-04-03 11:25:14.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/setup/setup_superuser.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.716216 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/taxonomy/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1201 2020-04-03 11:25:38.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/taxonomy/manage_taxonomic_restrictions.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2031 2020-04-03 11:26:02.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/taxonomy/taxonomic_restrictions_form.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.720216 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/widgets/
+-rw-r--r--   0 tom       (1000) tom       (1000)      919 2018-12-10 19:11:42.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/widgets/ajax_file_input.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1243 2020-04-03 11:26:34.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/widgets/app_theme_image_file_input.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      915 2022-04-28 07:09:31.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/widgets/crop_image_input.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      297 2019-10-09 13:14:46.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/widgets/image_input_with_preview.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.720216 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/widgets/taxonomy/
+-rw-r--r--   0 tom       (1000) tom       (1000)       88 2019-09-20 13:20:16.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/widgets/taxonomy/taxon_autocomplete_widget.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2610 2020-04-17 07:58:52.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/widgets/taxonomy/taxon_autocomplete_widget_base.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1146 2020-04-03 11:26:54.000000 localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/widgets/two_step_file_input.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.720216 localcosmos_server-0.9.4/localcosmos_server/templatetags/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2016-03-22 12:09:42.000000 localcosmos_server-0.9.4/localcosmos_server/templatetags/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3621 2022-04-21 10:15:23.000000 localcosmos_server-0.9.4/localcosmos_server/templatetags/localcosmos_tags.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1164 2020-02-04 07:51:02.000000 localcosmos_server-0.9.4/localcosmos_server/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      554 2019-10-01 06:46:50.000000 localcosmos_server-0.9.4/localcosmos_server/utils.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6820 2020-04-03 11:19:14.000000 localcosmos_server-0.9.4/localcosmos_server/validators.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      937 2020-02-17 12:00:18.000000 localcosmos_server-0.9.4/localcosmos_server/view_mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2632 2020-04-24 07:35:50.000000 localcosmos_server-0.9.4/localcosmos_server/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3871 2022-04-21 10:16:38.000000 localcosmos_server-0.9.4/localcosmos_server/widgets.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2022-05-13 14:25:25.576217 localcosmos_server-0.9.4/localcosmos_server.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)      804 2022-05-13 14:25:25.000000 localcosmos_server-0.9.4/localcosmos_server.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)    96106 2022-05-13 14:25:25.000000 localcosmos_server-0.9.4/localcosmos_server.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2022-05-13 14:25:25.000000 localcosmos_server-0.9.4/localcosmos_server.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)      237 2022-05-13 14:25:25.000000 localcosmos_server-0.9.4/localcosmos_server.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       19 2022-05-13 14:25:25.000000 localcosmos_server-0.9.4/localcosmos_server.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2022-05-13 14:25:25.720216 localcosmos_server-0.9.4/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)     1281 2022-05-13 14:23:52.000000 localcosmos_server-0.9.4/setup.py
```

### Comparing `localcosmos_server-0.9.3/MANIFEST.in` & `localcosmos_server-0.9.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/PKG-INFO` & `localcosmos_server-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localcosmos_server
-Version: 0.9.3
+Version: 0.9.4
 Summary: LocalCosmos Private Server. Run your own server for localcosmos.org apps.
 Home-page: https://github.com/SiSol-Systems/localcosmos-server
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,localcosmos,localcosmos server,biodiversity
 Platform: OS Independent
@@ -19,9 +19,7 @@
 ==================
 
 Private Server for localcosmos.org apps
 
 Documentation
 -------------
 Documentation and Tutorial: https://localcosmos-server.readthedocs.io/en/latest/
-
-
```

### Comparing `localcosmos_server-0.9.3/localcosmos_server/anycluster_schema_urls.py` & `localcosmos_server-0.9.4/localcosmos_server/anycluster_schema_urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/anycluster_schema_views.py` & `localcosmos_server-0.9.4/localcosmos_server/anycluster_schema_views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/api/authentication.py` & `localcosmos_server-0.9.4/localcosmos_server/api/authentication.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/api/permissions.py` & `localcosmos_server-0.9.4/localcosmos_server/api/permissions.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/api/road_permissions.py` & `localcosmos_server-0.9.4/localcosmos_server/api/road_permissions.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/api/road_serializers.py` & `localcosmos_server-0.9.4/localcosmos_server/api/road_serializers.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/api/serializers.py` & `localcosmos_server-0.9.4/localcosmos_server/api/serializers.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/api/urls.py` & `localcosmos_server-0.9.4/localcosmos_server/api/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/api/views.py` & `localcosmos_server-0.9.4/localcosmos_server/api/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/app_admin/middleware.py` & `localcosmos_server-0.9.4/localcosmos_server/app_admin/middleware.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/app_admin/static/app_admin/img/downarrow.svg` & `localcosmos_server-0.9.4/localcosmos_server/app_admin/static/app_admin/img/downarrow.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/app_admin/templates/app_admin/ajax/userbox.html` & `localcosmos_server-0.9.4/localcosmos_server/app_admin/templates/app_admin/ajax/userbox.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/app_admin/templates/app_admin/base.html` & `localcosmos_server-0.9.4/localcosmos_server/app_admin/templates/app_admin/base.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/app_admin/templates/app_admin/home.html` & `localcosmos_server-0.9.4/localcosmos_server/app_admin/templates/app_admin/home.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/app_admin/templates/app_admin/manage_app_user_role.html` & `localcosmos_server-0.9.4/localcosmos_server/app_admin/templates/app_admin/manage_app_user_role.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/app_admin/templates/app_admin/userlist.html` & `localcosmos_server-0.9.4/localcosmos_server/app_admin/templates/app_admin/userlist.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/app_admin/view_mixins.py` & `localcosmos_server-0.9.4/localcosmos_server/app_admin/view_mixins.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/app_admin/views.py` & `localcosmos_server-0.9.4/localcosmos_server/app_admin/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/csv_export.py` & `localcosmos_server-0.9.4/localcosmos_server/datasets/csv_export.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/fields.py` & `localcosmos_server-0.9.4/localcosmos_server/datasets/fields.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/forms.py` & `localcosmos_server-0.9.4/localcosmos_server/datasets/forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/migrations/0001_initial.py` & `localcosmos_server-0.9.4/localcosmos_server/datasets/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/models.py` & `localcosmos_server-0.9.4/localcosmos_server/datasets/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/ajax/dataset_box.html` & `localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/ajax/dataset_box.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/dataset_validation_routine.html` & `localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/dataset_validation_routine.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/edit_dataset.html` & `localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/edit_dataset.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/list_datasets.html` & `localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/list_datasets.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/manage_dataset_validation_routine_step.html` & `localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/manage_dataset_validation_routine_step.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/validation/ajax/dataset_form.html` & `localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/validation/ajax/dataset_form.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/validation/ajax/picture_field_images.html` & `localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/validation/ajax/picture_field_images.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/validation/expert_review.html` & `localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/validation/expert_review.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/widgets/mobile_number_input.html` & `localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/widgets/mobile_number_input.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/widgets/mobile_position_input.html` & `localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/widgets/mobile_position_input.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/widgets/picture_widget.html` & `localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/widgets/picture_widget.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/templates/datasets/widgets/select_datetime_widget.html` & `localcosmos_server-0.9.4/localcosmos_server/datasets/templates/datasets/widgets/select_datetime_widget.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/urls.py` & `localcosmos_server-0.9.4/localcosmos_server/datasets/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/validation/base.py` & `localcosmos_server-0.9.4/localcosmos_server/datasets/validation/base.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/validation/validators.py` & `localcosmos_server-0.9.4/localcosmos_server/datasets/validation/validators.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/views.py` & `localcosmos_server-0.9.4/localcosmos_server/datasets/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/datasets/widgets.py` & `localcosmos_server-0.9.4/localcosmos_server/datasets/widgets.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/fields.py` & `localcosmos_server-0.9.4/localcosmos_server/fields.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/forms.py` & `localcosmos_server-0.9.4/localcosmos_server/forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/generic_views.py` & `localcosmos_server-0.9.4/localcosmos_server/generic_views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/global_urls.py` & `localcosmos_server-0.9.4/localcosmos_server/global_urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/google_cloud_api/views.py` & `localcosmos_server-0.9.4/localcosmos_server/google_cloud_api/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/locale/de/LC_MESSAGES/django.mo` & `localcosmos_server-0.9.4/localcosmos_server/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/locale/de/LC_MESSAGES/django.po` & `localcosmos_server-0.9.4/localcosmos_server/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/locale/en/LC_MESSAGES/django.po` & `localcosmos_server-0.9.4/localcosmos_server/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/mails.py` & `localcosmos_server-0.9.4/localcosmos_server/mails.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/management/commands/enable_staging_domain.py` & `localcosmos_server-0.9.4/localcosmos_server/management/commands/enable_staging_domain.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/middleware.py` & `localcosmos_server-0.9.4/localcosmos_server/middleware.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/migrations/0001_initial.py` & `localcosmos_server-0.9.4/localcosmos_server/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/models.py` & `localcosmos_server-0.9.4/localcosmos_server/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/CMSObjects.py` & `localcosmos_server-0.9.4/localcosmos_server/online_content/CMSObjects.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/api/views.py` & `localcosmos_server-0.9.4/localcosmos_server/online_content/api/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/fields.py` & `localcosmos_server-0.9.4/localcosmos_server/online_content/fields.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/forms.py` & `localcosmos_server-0.9.4/localcosmos_server/online_content/forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/migrations/0001_initial.py` & `localcosmos_server-0.9.4/localcosmos_server/online_content/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/mixins.py` & `localcosmos_server-0.9.4/localcosmos_server/online_content/mixins.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/models.py` & `localcosmos_server-0.9.4/localcosmos_server/online_content/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/parser.py` & `localcosmos_server-0.9.4/localcosmos_server/online_content/parser.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/LICENSE.md` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/LICENSE.md`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/ckeditor.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/ckeditor.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/ckeditor.js.map` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/ckeditor.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/index.html` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/index.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/LICENSE.md` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/LICENSE.md`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/ckeditor.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/ckeditor.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/ckeditor.js.map` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/ckeditor.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ar.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ar.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ast.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ast.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/bg.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/bg.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/cs.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/cs.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/da.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/da.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/de.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/de.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/el.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/el.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/en-au.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/en-au.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/eo.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/eo.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/es.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/es.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/et.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/et.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/eu.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/eu.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/fi.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/fi.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/fr.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/fr.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/gl.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/gl.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/gu.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/gu.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/hr.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/hr.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/hu.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/hu.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/it.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/it.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ja.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ja.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/km.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/km.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/kn.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/kn.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ko.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ko.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ku.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ku.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/nb.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/nb.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ne.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ne.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/nl.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/nl.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/oc.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/oc.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/pl.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/pl.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/pt-br.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/pt-br.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/pt.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/pt.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ro.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ro.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ru.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ru.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/si.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/si.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/sk.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/sk.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/sq.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/sq.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/sv.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/sv.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/tr.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/tr.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/tt.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/tt.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ug.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/ug.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/uk.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/uk.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/zh-cn.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/zh-cn.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/zh.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/old/translations/zh.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/css/sample.css` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/css/sample.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/bg.png` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/bg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/github.svg` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/github.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/logo.svg` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/logo.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/umbrellas.jpg` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/sample/img/umbrellas.jpg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/af.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/af.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ar.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ar.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ast.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ast.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/az.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/az.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/bg.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/bg.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ca.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ca.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/cs.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/cs.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/da.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/da.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/de-ch.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/de-ch.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/de.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/de.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/el.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/el.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/en-au.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/en-au.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/en-gb.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/en-gb.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/eo.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/eo.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/es.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/es.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/et.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/et.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/eu.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/eu.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/fa.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/fa.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/fi.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/fi.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/fr.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/fr.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/gl.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/gl.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/gu.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/gu.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/he.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/he.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/hr.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/hr.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/hu.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/hu.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/id.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/id.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/it.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/it.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ja.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ja.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/km.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/km.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/kn.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/kn.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ko.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ko.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ku.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ku.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/lt.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/lt.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/lv.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/lv.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ms.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ms.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/nb.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/nb.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ne.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ne.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/nl.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/nl.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/no.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/no.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/oc.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/oc.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/pl.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/pl.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/pt-br.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/pt-br.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/pt.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/pt.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ro.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ro.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ru.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ru.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/si.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/si.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sk.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sk.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sl.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sl.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sq.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sq.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sr-latn.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sr-latn.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sr.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sr.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sv.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/sv.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/th.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/th.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/tr.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/tr.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/tt.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/tt.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ug.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/ug.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/uk.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/uk.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/vi.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/vi.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/zh-cn.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/zh-cn.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/zh.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/ckeditor5-build-classic/translations/zh.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/online_content.css` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/online_content.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/static/online_content/online_content.js` & `localcosmos_server-0.9.4/localcosmos_server/online_content/static/online_content/online_content.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/ajax/image_microcontent_form.html` & `localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/ajax/image_microcontent_form.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/ajax/unpublish_template_content.html` & `localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/ajax/unpublish_template_content.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/ajax/upload_custom_template.html` & `localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/ajax/upload_custom_template.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/ajax_filecontent_field.html` & `localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/ajax_filecontent_field.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/create_template_content.html` & `localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/create_template_content.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/delete_microcontent.html` & `localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/delete_microcontent.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/filecontent_field.html` & `localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/filecontent_field.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/manage_template_content.html` & `localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/manage_template_content.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/manage_template_content_extra_scripts.html` & `localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/manage_template_content_extra_scripts.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/online_content_base.html` & `localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/online_content_base.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/template_content_list_entry.html` & `localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/template_content_list_entry.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/textcontent_field.html` & `localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/textcontent_field.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/templates/online_content/translate_template_content.html` & `localcosmos_server-0.9.4/localcosmos_server/online_content/templates/online_content/translate_template_content.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/templatetags/online_content_tags.py` & `localcosmos_server-0.9.4/localcosmos_server/online_content/templatetags/online_content_tags.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/urls.py` & `localcosmos_server-0.9.4/localcosmos_server/online_content/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/views.py` & `localcosmos_server-0.9.4/localcosmos_server/online_content/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/online_content/widgets.py` & `localcosmos_server-0.9.4/localcosmos_server/online_content/widgets.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/permission_rules.py` & `localcosmos_server-0.9.4/localcosmos_server/permission_rules.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/server_control_panel/forms.py` & `localcosmos_server-0.9.4/localcosmos_server/server_control_panel/forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/server_control_panel/middleware.py` & `localcosmos_server-0.9.4/localcosmos_server/server_control_panel/middleware.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/server_control_panel/templates/server_control_panel/base.html` & `localcosmos_server-0.9.4/localcosmos_server/server_control_panel/templates/server_control_panel/base.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/server_control_panel/templates/server_control_panel/edit_app.html` & `localcosmos_server-0.9.4/localcosmos_server/server_control_panel/templates/server_control_panel/edit_app.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/server_control_panel/templates/server_control_panel/home.html` & `localcosmos_server-0.9.4/localcosmos_server/server_control_panel/templates/server_control_panel/home.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/server_control_panel/templates/server_control_panel/install_app.html` & `localcosmos_server-0.9.4/localcosmos_server/server_control_panel/templates/server_control_panel/install_app.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/server_control_panel/urls.py` & `localcosmos_server-0.9.4/localcosmos_server/server_control_panel/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/server_control_panel/views.py` & `localcosmos_server-0.9.4/localcosmos_server/server_control_panel/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/settings.py` & `localcosmos_server-0.9.4/localcosmos_server/settings.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/setup_forms.py` & `localcosmos_server-0.9.4/localcosmos_server/setup_forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/setup_views.py` & `localcosmos_server-0.9.4/localcosmos_server/setup_views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/slugifier.py` & `localcosmos_server-0.9.4/localcosmos_server/slugifier.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/specifications/DatasetJSON` & `localcosmos_server-0.9.4/localcosmos_server/specifications/DatasetJSON`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Indie_Flower/IndieFlower-Regular.ttf` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Indie_Flower/IndieFlower-Regular.ttf`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Indie_Flower/IndieFlower-Regular.woff` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Indie_Flower/IndieFlower-Regular.woff`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Indie_Flower/OFL.txt` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Indie_Flower/OFL.txt`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/LICENSE.txt` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Black.ttf` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Black.woff` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Black.woff`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-BlackItalic.ttf` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-BlackItalic.woff` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-BlackItalic.woff`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Bold.ttf` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Bold.woff` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Bold.woff`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-BoldItalic.ttf` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-BoldItalic.woff` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Italic.ttf` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Italic.woff` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Italic.woff`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Light.ttf` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Light.woff` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Light.woff`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-LightItalic.ttf` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-LightItalic.woff` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Medium.ttf` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Medium.woff` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Medium.woff`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-MediumItalic.ttf` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-MediumItalic.woff` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Regular.ttf` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Regular.woff` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Regular.woff`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Thin.ttf` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-Thin.woff` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-Thin.woff`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-ThinItalic.ttf` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/Roboto/Roboto-ThinItalic.woff` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/Roboto/Roboto-ThinItalic.woff`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/fonts/fonts.css` & `localcosmos_server-0.9.4/localcosmos_server/static/fonts/fonts.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/images/lclogo32.png` & `localcosmos_server-0.9.4/localcosmos_server/static/images/lclogo32.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/images/local_cosmos_logo_40.png` & `localcosmos_server-0.9.4/localcosmos_server/static/images/local_cosmos_logo_40.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/images/local_cosmos_logo_horizontal.png` & `localcosmos_server-0.9.4/localcosmos_server/static/images/local_cosmos_logo_horizontal.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/images/spinner.gif` & `localcosmos_server-0.9.4/localcosmos_server/static/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-grid.css` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-grid.css.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-reboot.css` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-reboot.css.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap.css` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap.css.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap.min.css` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap.min.css.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.bundle.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.bundle.js.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.js.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.min.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.min.js.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/bootstrap-4.3.1-dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/css/localcosmos_server.css` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/css/localcosmos_server.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/Local-Cosmos-Logo.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/Local-Cosmos-Logo.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/add_image.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/add_image.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/arrow-tool-add.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/arrow-tool-add.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/arrow-tool-add.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/arrow-tool-add.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/arrow-tool-remove.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/arrow-tool-remove.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/arrow-tool-remove.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/arrow-tool-remove.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/arrow-tool.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/arrow-tool.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/arrow-tool.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/arrow-tool.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_ASEAN.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_ASEAN.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_African Union(OAS).png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_African Union(OAS).png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Arab League.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Arab League.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_CARICOM.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_CARICOM.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_CIS.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_CIS.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Commonwealth.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Commonwealth.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_England.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_England.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_European Union.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_European Union.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Islamic Conference.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Islamic Conference.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Kosovo.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Kosovo.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_NATO.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_NATO.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Northern Cyprus.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Northern Cyprus.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Northern Ireland.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Northern Ireland.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_OPEC.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_OPEC.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Olimpic Movement.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Olimpic Movement.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Scotland.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Scotland.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Somaliland.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Somaliland.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_United Nations.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_United Nations.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/_Wales.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/_Wales.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ad.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ad.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ae.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ae.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/af.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/af.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ag.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ag.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ai.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ai.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/am.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/am.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/an.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/an.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ao.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ao.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/aq.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/aq.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ar.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ar.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/as.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/as.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/at.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/at.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/au.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/au.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/aw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/aw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/az.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/az.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ba.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ba.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bb.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bb.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bd.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bd.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/be.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/be.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bf.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bf.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bh.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bh.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bi.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bi.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bj.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bj.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bo.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bo.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/br.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/br.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bs.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bs.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bt.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bt.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/by.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/by.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/bz.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/bz.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ca.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ca.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cd.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cd.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cf.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cf.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ch.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ch.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ci.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ci.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ck.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ck.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cl.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cl.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/co.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/co.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cu.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cu.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cv.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cv.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cy.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cy.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/cz.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/cz.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/da.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/da.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/de.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/de.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/dj.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/dj.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/dk.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/dk.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/dm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/dm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/do.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/do.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/dz.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/dz.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ec.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ec.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ee.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ee.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/eg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/eg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/eh.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/eh.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/en.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/en.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/er.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/er.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/es.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/es.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/et.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/et.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/fi.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/fi.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/fj.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/fj.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/fm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/fm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/fo.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/fo.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/fr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/fr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ga.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ga.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gb.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gb.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gd.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gd.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ge.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ge.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gh.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gh.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gi.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gi.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gl.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gl.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gp.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gp.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gq.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gq.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gt.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gt.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gu.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gu.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/gy.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/gy.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/hk.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/hk.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/hn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/hn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/hr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/hr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ht.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ht.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/hu.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/hu.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/id.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/id.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ie.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ie.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/il.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/il.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/im.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/im.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/in.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/in.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/iq.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/iq.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ir.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ir.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/is.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/is.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/it.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/it.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ja.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ja.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/je.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/je.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/jm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/jm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/jo.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/jo.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/jp.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/jp.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ke.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ke.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/kg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/kg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/kh.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/kh.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ki.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ki.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/km.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/km.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/kn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/kn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/kp.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/kp.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/kr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/kr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/kw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/kw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ky.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ky.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/kz.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/kz.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/la.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/la.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/lb.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/lb.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/lc.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/lc.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/li.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/li.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/lk.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/lk.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/lr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/lr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ls.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ls.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/lt.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/lt.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/lu.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/lu.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/lv.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/lv.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ly.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ly.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ma.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ma.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mc.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mc.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/md.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/md.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/me.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/me.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mh.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mh.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mk.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mk.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ml.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ml.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mo.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mo.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mq.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mq.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ms.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ms.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mt.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mt.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mu.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mu.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mv.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mv.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mx.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mx.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/my.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/my.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/mz.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/mz.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/na.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/na.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/nc.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/nc.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ne.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ne.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ng.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ng.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ni.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ni.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/nl.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/nl.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/no.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/no.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/np.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/np.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/nr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/nr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/nz.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/nz.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/om.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/om.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/pa.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/pa.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/pe.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/pe.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/pf.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/pf.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/pg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/pg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ph.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ph.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/pk.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/pk.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/pr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/pr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ps.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ps.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/pt.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/pt.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/pw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/pw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/py.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/py.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/qa.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/qa.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/re.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/re.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ro.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ro.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/rs.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/rs.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ru.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ru.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/rw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/rw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sa.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sa.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sb.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sb.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sc.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sc.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sd.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sd.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/se.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/se.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/si.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/si.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sk.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sk.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sl.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sl.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/so.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/so.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sq.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sq.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/st.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/st.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sv.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sv.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sy.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sy.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/sz.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/sz.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tc.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tc.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/td.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/td.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/th.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/th.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tj.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tj.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tl.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tl.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/to.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/to.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tt.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tt.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tv.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tv.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/tz.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/tz.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ua.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ua.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ug.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ug.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/us.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/us.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/uy.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/uy.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/uz.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/uz.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/va.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/va.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/vc.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/vc.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ve.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ve.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/vg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/vg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/vi.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/vi.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/vn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/vn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/vu.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/vu.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ws.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ws.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/ye.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/ye.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/za.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/za.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/zm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/zm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_big/zw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_big/zw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Algeria.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Algeria.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/British_Virgin_Islands.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/British_Virgin_Islands.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Cayman_Islands.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Cayman_Islands.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Chad.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Chad.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Comoros.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Comoros.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Democratic_Republic_of_the_Congo.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Democratic_Republic_of_the_Congo.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/French_Polynesia.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/French_Polynesia.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Latvia.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Latvia.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Micronesia.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Micronesia.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/North_Korea.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/North_Korea.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Oman.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Oman.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Saint_Kitts_and_Nevis.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Saint_Kitts_and_Nevis.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Saint_Lucia.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Saint_Lucia.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Saint_Pierre.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Saint_Pierre.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Saint_Vicent_and_the_Grenadines.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Saint_Vicent_and_the_Grenadines.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Samoa.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Samoa.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Soviet_Union.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Soviet_Union.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Sri_Lanka.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Sri_Lanka.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Tibet.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Tibet.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/Tuvalu.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/Tuvalu.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ad.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ad.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ae.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ae.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/af.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/af.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ag.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ag.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ai.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ai.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/al.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/al.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/am.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/am.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/an.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/an.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ao.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ao.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ar.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ar.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/as.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/as.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/at.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/at.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/au.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/au.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/aw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/aw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/az.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/az.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ba.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ba.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bb.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bb.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bd.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bd.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/be.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/be.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bf.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bf.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bh.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bh.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bi.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bi.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bj.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bj.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bo.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bo.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/br.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/br.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bs.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bs.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bt.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bt.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/by.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/by.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/bz.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/bz.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ca.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ca.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cf.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cf.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ch.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ch.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ci.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ci.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ck.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ck.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cl.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cl.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/co.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/co.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cu.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cu.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cv.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cv.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cx.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cx.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cy.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cy.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/cz.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/cz.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/de.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/de.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/dj.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/dj.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/dk.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/dk.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/dm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/dm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/do.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/do.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ec.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ec.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ee.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ee.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/eg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/eg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/en.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/en.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/er.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/er.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/es.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/es.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/et.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/et.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/fi.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/fi.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/fj.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/fj.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/fk.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/fk.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/fo.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/fo.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/fr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/fr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ga.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ga.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gb.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gb.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gd.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gd.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ge.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ge.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gf.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gf.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gh.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gh.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gi.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gi.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gl.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gl.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gq.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gq.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gt.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gt.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gu.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gu.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/gy.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/gy.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/hk.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/hk.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/hn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/hn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/hr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/hr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ht.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ht.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/hu.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/hu.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/id.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/id.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ie.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ie.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/il.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/il.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/in.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/in.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/iq.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/iq.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ir.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ir.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/is.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/is.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/it.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/it.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/jm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/jm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/jo.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/jo.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/jp.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/jp.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ke.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ke.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/kg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/kg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/kh.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/kh.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ki.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ki.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/kw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/kw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/kz.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/kz.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/la.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/la.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/lb.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/lb.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/li.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/li.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/lr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/lr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ls.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ls.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/lt.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/lt.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/lu.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/lu.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ly.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ly.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ma.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ma.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mc.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mc.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/md.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/md.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mh.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mh.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mk.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mk.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ml.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ml.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mo.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mo.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ms.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ms.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mt.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mt.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mu.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mu.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mv.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mv.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mx.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mx.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/my.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/my.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/mz.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/mz.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/na.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/na.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ne.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ne.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/nf.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/nf.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ng.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ng.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ni.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ni.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/nl.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/nl.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/no.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/no.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/np.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/np.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/nr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/nr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/nu.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/nu.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/nz.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/nz.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pa.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pa.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pe.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pe.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ph.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ph.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pk.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pk.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pl.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pl.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pt.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pt.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/pw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/pw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/py.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/py.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/qa.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/qa.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ro.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ro.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/rs.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/rs.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ru.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ru.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/rw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/rw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sa.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sa.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sb.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sb.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sc.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sc.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sd.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sd.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/se.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/se.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sh.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sh.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/si.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/si.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sk.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sk.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sl.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sl.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/so.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/so.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/st.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/st.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sv.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sv.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sy.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sy.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/sz.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/sz.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tc.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tc.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tg.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tg.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/th.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/th.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tj.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tj.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tl.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tl.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/to.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/to.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tr.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tr.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tt.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tt.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/tz.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/tz.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ua.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ua.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ug.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ug.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/us.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/us.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/uy.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/uy.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/uz.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/uz.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/va.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/va.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ve.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ve.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/vi.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/vi.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/vn.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/vn.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/vu.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/vu.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/wf.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/wf.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/ye.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/ye.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/yt.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/yt.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/za.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/za.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/zm.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/zm.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/countries_huge/zw.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/countries_huge/zw.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/images/crop-tool.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/images/crop-tool.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/interactive-image-field/InteractiveImageField.css` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/interactive-image-field/InteractiveImageField.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/interactive-image-field/InteractiveImageField.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/interactive-image-field/InteractiveImageField.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -60,22 +60,25 @@
         this.featuresInput = featuresInput;
 
         this.options = {
             "arrowsEnalbed": true,
             "greyAreaFillColor": "rgba(0,0,0,0.5)",
             "relativeArrowStrokeWidth": 0.02,
             "relativeArrowLength": 0.5,
-            "defaultArrowColor": "#000000"
+            "defaultArrowColor": "#000000",
+            "cropMode": "contains", // contained: crop area contained inside image, contains: crop area contains image (can be larger than image)
+            "stageBackground": "#FFFFFF" // only used if cropMode == "contains"
         };
 
         for (let key in options) {
             this.options[key] = options[key];
         }
 
         this.stage = null;
+        this.konvaImage = null;
         this.cropArea = null;
         this.cropAreaGrey = null;
         this.image = null;
 
         this.cropLayer = null;
         this.cropAreaTransformLayer = null;
         this.arrowLayer = null;
@@ -127,24 +130,30 @@
 
     createHTML() {
         this.imageContainer = document.createElement("div");
         this.imageContainer.id = "InterActiveImageField-image";
         this.container.prepend(this.imageContainer);
     }
 
+    /*
+     * The origin (0/0) of the coordinate system which the crop paramters refer to is the top left corner of the image
+     * this way, the stage can be altered without compromising the validity of the crop parameters
+     */
     setCropParametersInputValue() {
         if (this.cropArea != null) {
 
             let reverseScalingFactor = 1 / this.getScalingFactor();
 
             let cropAreaRect = this.cropArea.getClientRect();
 
+            let imageRect = this.konvaImage.getClientRect();
+
             var data = {
-                "x": Math.round(cropAreaRect.x * reverseScalingFactor),
-                "y": Math.round(cropAreaRect.y * reverseScalingFactor),
+                "x": Math.round((cropAreaRect.x - imageRect.x) * reverseScalingFactor),
+                "y": Math.round((cropAreaRect.y - imageRect.y) * reverseScalingFactor),
                 "width": Math.round(cropAreaRect.width * reverseScalingFactor),
                 "height": Math.round(cropAreaRect.height * reverseScalingFactor),
                 "rotate": 0,
                 "scaleX": 1,
                 "scaleY": 1
             };
 
@@ -226,54 +235,93 @@
             self.onImageLoad(event);
         };
 
         this.image.src = imageSrc;
 
     }
 
+
     addStage() {
 
-        let originalHeight = this.image.height;
+        let stageWidth = this.imageContainer.offsetWidth;
+        let stageHeight = stageWidth;
 
-        let scalingFactor = this.getScalingFactor();
+        if (this.options.cropMode == "contained") {
 
-        if (this.DEBUG == true) {
-            console.log("[InteractiveImageField] loading stage. image height: " + this.image.height + " , image width : " + this.image.width + " scalingFactor: " + scalingFactor);
-        }
+            let originalHeight = this.image.height;
 
-        let imageCanvasWidth = this.imageContainer.offsetWidth;
-        let imageCanvasHeight = parseInt(originalHeight * scalingFactor);
+            let scalingFactor = this.getScalingFactor();
 
-        if (this.stage != null) {
-            this.stage.destroy();
+            if (this.DEBUG == true) {
+                console.log("[InteractiveImageField] loading stage. image height: " + this.image.height + " , image width : " + this.image.width + " scalingFactor: " + scalingFactor);
+            }
+
+            stageHeight = parseInt(originalHeight * scalingFactor);
+
+
+            if (this.DEBUG == true) {
+                console.log("instantiating Konva.Stage width: " + stageWidth + " height: " + stageHeight);
+            }
         }
 
-        if (this.DEBUG == true) {
-            console.log("instantiating Konva.Stage width: " + imageCanvasWidth + " height: " + imageCanvasHeight);
+        if (this.stage != null) {
+            this.stage.destroy();
         }
 
         this.stage = new Konva.Stage({
             container: this.imageContainer.id, // id of container <div>
-            width: imageCanvasWidth,
-            height: imageCanvasHeight
+            width: stageWidth,
+            height: stageHeight
         });
     }
 
+    // if the image contains the crop area, the image has the same size like the stage
+    // if the crop area contains the image (crop area can extend image), only one dimension (height or width) fits into the stage and equals the stage
     addKonvaImage() {
 
-        let konvaImage = new Konva.Image({
+        // in "contained" mode, the image dimensions equal the stage dimensions
+        let imageWidth = this.stage.width();
+        let imageHeight = this.stage.height();
+        let offsetX = 0;
+        let offsetY = 0;
+
+        // in "contains" mode, the stage is square and the image fits into the stage
+        if (this.options.cropMode == "contains") {
+            // crop area contains image
+
+            let scalingFactor = this.getScalingFactor();
+
+            imageWidth = this.image.width * scalingFactor;
+            imageHeight = this.image.height * scalingFactor;
+
+            offsetX = (this.stage.width() / 2) - (imageWidth / 2)
+            offsetY = (this.stage.height() / 2) - (imageHeight / 2)
+        }
+
+        this.konvaImage = new Konva.Image({
+            x: offsetX,
+            y: offsetY,
+            image: this.image,
+            width: imageWidth,
+            height: imageHeight
+        });
+
+        let imageLayer = new Konva.Layer();
+
+        let background = new Konva.Rect({
             x: 0,
             y: 0,
-            image: this.image,
             width: this.stage.width(),
-            height: this.stage.height()
+            height: this.stage.height(),
+            fill: this.options.stageBackground
         });
 
-        let imageLayer = new Konva.Layer();
-        imageLayer.add(konvaImage);
+        imageLayer.add(background);
+
+        imageLayer.add(this.konvaImage);
 
         this.stage.add(imageLayer);
 
     }
 
     onCropAreaMove() {
 
@@ -311,14 +359,15 @@
     // crop area consists of a tranformer (rectangle), and 4 grey, translucent rectangles outside the crop area
     addCropArea(resetCropArea) {
 
         let self = this;
 
         let scalingFactor = this.getScalingFactor()
 
+        // 1 pixel tolerance
         let initialCropSquareLength = Math.min(this.stage.width(), this.stage.height());
 
         // add the crop area
         let cropParameters = {
             x: 0,
             y: 0,
             width: initialCropSquareLength,
@@ -339,16 +388,16 @@
 
             if (cropSquareLength > initialCropSquareLength) {
                 cropSquareLength = initialCropSquareLength;
             }
 
             cropParameters = {
 
-                x: cropParametersInputValue.x * scalingFactor,
-                y: cropParametersInputValue.y * scalingFactor,
+                x: (cropParametersInputValue.x * scalingFactor) + this.konvaImage.x(),
+                y: (cropParametersInputValue.y * scalingFactor) + this.konvaImage.y(),
                 width: cropSquareLength,
                 height: cropSquareLength
 
             };
         }
 
         this.cropArea = new Konva.Rect({
@@ -396,23 +445,31 @@
             flipEnabled: false,
             rotateEnabled: false,
             keepRatio: true,
             centeredScaling: false,
             enabledAnchors: ['top-left', 'top-right', 'bottom-left', 'bottom-right'],
             shouldOverdrawWholeArea: true,
             boundBoxFunc: (oldBox, newBox) => {
+
                 const box = this.getClientRect(newBox);
                 const isOut =
                     box.x < 0 ||
                     box.y < 0 ||
-                    box.x + box.width > this.stage.width() ||
-                    box.y + box.height > this.stage.height();
+                    Math.round(box.x + box.width) > this.stage.width() ||
+                    Math.round(box.y + box.height) > this.stage.height();
                 // if new bounding box is out of visible viewport, let's just skip transforming
                 // this logic can be improved by still allow some transforming if we have small available space
+                // apply Math.round() to prevent scaling the rect resulting box.x + box.width in something like 300.00000003 while stage.width() being 300
                 if (isOut) {
+
+                    if (this.DEBUG == true) {
+                        console.log(box.x + box.width + "   VS stage " + this.stage.width())
+                        console.log("[InteractiveImageField] isOut, using old box");
+                    }
+
                     return oldBox;
                 }
                 return newBox;
             }
         });
 
         this.cropTransformer.on('dragmove', function() {
@@ -1103,27 +1160,45 @@
 
         this.activeArrow = arrow;
 
         this.toolbar.activateArrowMode();
     }
 
     // helper methods
+    // the scaling factor describes the scaling of the image, which is necessary to fit it into the stage
+    // if cropArea contains the image, the larger dimension of width/height defines the scaling factor
     getScalingFactor() {
 
         if (this.DEBUG == true) {
             console.log("[InteractiveImageField] calculating scaling factor. container.offsetWidth: " + this.container.offsetWidth + " stage: " + this.stage + " image width: " + this.image.width);
         }
 
+        let scalingFactor = null;
+
         let stageWidth = this.container.offsetWidth;
 
         if (this.stage != null) {
             stageWidth = this.stage.width();
         }
 
-        return stageWidth / this.image.width;
+        if (this.options.cropMode == "contains") {
+            // stage is present
+            let stageHeight = this.stage.height();
+
+
+            if (this.image.height >= this.image.width) {
+                scalingFactor = stageHeight / this.image.height;
+            } else {
+                scalingFactor = stageWidth / this.image.width;
+            }
+        } else {
+            scalingFactor = stageWidth / this.image.width;
+        }
+
+        return scalingFactor;
     }
 
     getClientRect(rotatedBox) {
 
         const {
             x,
             y,
```

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/jquery-3.3.1.min.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/js/ajax_file_input.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/js/ajax_file_input.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/js/bootstrap3-typeahead.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/js/bootstrap3-typeahead.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/js/django-ajax-csrf.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/js/django-ajax-csrf.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/js/django-ajax.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/js/django-ajax.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/js/jquery-taxon-autocomplete.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/js/jquery-taxon-autocomplete.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/js/jquery-user-autocomplete.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/js/jquery-user-autocomplete.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/js/localcosmos_server.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/js/localcosmos_server.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/js/popper.min.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/konva/konva.min.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/konva/konva.min.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/Spin.gif` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/Spin.gif`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-grid.css` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-grid.css.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-reboot.css` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-reboot.css.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap.css` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap.css.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap.min.css` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap.min.css.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.bundle.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.bundle.js.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.js.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.min.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.min.js.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/bootstrap-4.3.1-dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/jquery/jquery-3.3.1.min.js` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/jquery/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/jquery/jquery-3.3.1.min.map` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/jquery/jquery-3.3.1.min.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/lc_setup.css` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/lc_setup.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/localcosmos_server/setup/logo100blue.png` & `localcosmos_server-0.9.4/localcosmos_server/static/localcosmos_server/setup/logo100blue.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/images/layers-2x.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/images/layers-2x.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/images/layers.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/images/layers.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/images/marker-icon-2x.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/images/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/images/marker-icon.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/images/marker-shadow.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/leaflet-src.esm.js` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/leaflet-src.esm.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/leaflet-src.esm.js.map` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/leaflet-src.esm.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/leaflet-src.js` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/leaflet-src.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/leaflet-src.js.map` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/leaflet-src.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/leaflet.css` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/leaflet.css`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/leaflet.js` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/leaflet.js`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/leaflet/leaflet.js.map` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/leaflet/leaflet.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Amphibia.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Amphibia.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Animalia.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Animalia.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Anura.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Anura.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Arachnida.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Arachnida.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Arthropoda.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Arthropoda.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Aves.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Aves.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Chordata.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Chordata.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Coleoptera.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Coleoptera.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Fungi.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Fungi.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Holocephali,Elasmobranchii,Sarcopterygii,Actinopterygii.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Holocephali,Elasmobranchii,Sarcopterygii,Actinopterygii.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Insecta.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Insecta.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Lepidoptera.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Lepidoptera.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Mammalia.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Mammalia.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Mollucsa.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Mollucsa.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Odonata.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Odonata.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/Plantae.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/Plantae.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/maps/markers/marker_unknown.png` & `localcosmos_server-0.9.4/localcosmos_server/static/maps/markers/marker_unknown.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/noimage.png` & `localcosmos_server-0.9.4/localcosmos_server/static/noimage.png`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/broadcast.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/broadcast.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/calendar.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/calendar.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/circuit-board.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/circuit-board.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/dashboard.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/dashboard.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/database.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/database.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/eye-closed.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/eye-closed.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/file-pdf.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/file-pdf.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/gift.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/gift.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/git-branch.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/git-branch.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/git-compare.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/git-compare.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/git-merge.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/git-merge.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/git-pull-request.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/git-pull-request.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/globe.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/globe.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/info.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/info.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/jersey.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/jersey.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/light-bulb.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/light-bulb.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/list-ordered.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/list-ordered.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/list-unordered.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/list-unordered.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/logo-gist.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/logo-gist.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/logo-github.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/logo-github.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/mark-github.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/mark-github.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/mention.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/mention.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/mortar-board.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/mortar-board.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/octoface.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/octoface.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/organization.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/organization.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/paintcan.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/paintcan.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/radio-tower.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/radio-tower.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/repo-forked.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/repo-forked.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/rocket.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/rocket.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/server.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/server.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/smiley.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/smiley.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/squirrel.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/squirrel.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/thumbsdown.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/thumbsdown.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/thumbsup.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/thumbsup.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/tools.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/tools.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/unmute.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/unmute.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/unverified.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/unverified.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/static/octicons/verified.svg` & `localcosmos_server-0.9.4/localcosmos_server/static/octicons/verified.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/taxonomy/AppTaxonSearch.py` & `localcosmos_server-0.9.4/localcosmos_server/taxonomy/AppTaxonSearch.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/taxonomy/fields.py` & `localcosmos_server-0.9.4/localcosmos_server/taxonomy/fields.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/taxonomy/forms.py` & `localcosmos_server-0.9.4/localcosmos_server/taxonomy/forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/taxonomy/generic.py` & `localcosmos_server-0.9.4/localcosmos_server/taxonomy/generic.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/taxonomy/lazy.py` & `localcosmos_server-0.9.4/localcosmos_server/taxonomy/lazy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import urllib.request, json, codecs # gbif_id
 from urllib.parse import quote_plus
 from http.client import RemoteDisconnected
 
+from django.conf import settings
+
+SUPPORTED_LAZY_TAXONOMY_SOURCES = [db[0] for db in settings.LAZY_TAXONOMY_SOURCES]
+
 ##################################################################################################################
 #
 # LazyTaxon
 # - the LazyTaxon class is the only taxon class that should be used directly by LocalCosmos
 # - it is compatible with all taxonomic sources
 # - LazyTaxon.source has to point to the source it comes from, eg taxonomy.sources.col
 #
@@ -30,28 +34,20 @@
 
             # these values change across tree versions
             self.name_uuid = str(self.instance.name_uuid)
             self.taxon_nuid = self.instance.taxon_nuid
 
             self.origin = self.instance.__class__.__name__
 
-            # if the instance has an attribute taxon_source it derives from ModelWithTaxonCommon
-            # if the instance has an attribute source_id it derives from the DB - might be deprecated
+            taxon_source = self.get_taxon_source(self.instance)
 
-            if hasattr(self.instance, 'taxon_source'):
-                self.taxon_source = self.instance.taxon_source                
+            if not taxon_source:
+                raise ValueError('Non-taxonomic instance passed to LazyTaxon. Could not determine taxon_source.')
 
-            # in this case, it is a taxon directly from the taxonomic database
-            elif hasattr(self.instance, 'source_id'):
-                # remove ".models" from module
-                self.taxon_source = ('.').join(self.instance.__module__.split('.')[:-1])
-                #self.taxon_source = 'taxonomy.sources.%s' % self.instance._meta.app_label
-            
-            else:
-                raise ValueError('Non-taxonomic instance passed to LazyTaxon')
+            self.taxon_source = taxon_source
 
 
         elif 'taxon_latname' in kwargs and 'taxon_author' in kwargs and 'taxon_source' in kwargs and 'taxon_nuid' in kwargs and 'name_uuid' in kwargs:
             self.taxon_latname = kwargs['taxon_latname']
             self.taxon_author = kwargs['taxon_author']
             self.taxon_source = kwargs['taxon_source']
             self.taxon_include_descendants = kwargs.get('taxon_include_descendants', False)
@@ -59,14 +55,36 @@
             self.taxon_nuid = kwargs['taxon_nuid']
             self.name_uuid = kwargs['name_uuid']
 
         else:
             raise ValueError('Unable to instantiate LazyTaxon, improper parameters given: %s' %kwargs)
 
 
+    def get_taxon_source(self, instance):
+
+        taxon_source = None
+        
+        # if the instance has an attribute taxon_source it derives from ModelWithTaxonCommon
+        # if the instance has an attribute source_id it derives from the DB - might be deprecated
+
+        if hasattr(instance, 'taxon_source'):
+            taxon_source = instance.taxon_source                
+
+        # in this case, it is a taxon directly from the taxonomic database
+        else:
+            # remove ".models" from module
+            taxon_source = ('.').join(instance.__module__.split('.')[:-1])
+            #self.taxon_source = 'taxonomy.sources.%s' % instance._meta.app_label
+
+            if taxon_source not in SUPPORTED_LAZY_TAXONOMY_SOURCES:
+                raise ValueError('unsupported taxonomic source passed to LazyTaxon: {0}'.format(taxon_source))
+        
+        return taxon_source
+    
+
     def gbif_nubKey(self):
 
         gbif_nubKey = None
 
         url = 'http://api.gbif.org/v1/species?name=%s' % quote_plus(self.taxon_latname.encode('utf-8'))
 
         request = urllib.request.Request(url)
```

### Comparing `localcosmos_server-0.9.3/localcosmos_server/taxonomy/urls.py` & `localcosmos_server-0.9.4/localcosmos_server/taxonomy/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/taxonomy/views.py` & `localcosmos_server-0.9.4/localcosmos_server/taxonomy/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/taxonomy/widgets.py` & `localcosmos_server-0.9.4/localcosmos_server/taxonomy/widgets.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/base.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/base.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/content_licencing/widgets/licence_select_widget.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/content_licencing/widgets/licence_select_widget.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/email/registration_confirmation.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/email/registration_confirmation.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/email/registration_confirmation.txt` & `localcosmos_server-0.9.4/localcosmos_server/templates/email/registration_confirmation.txt`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/error_base.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/error_base.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/api/legal/privacy_statement.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/api/legal/privacy_statement.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/api/password_reset_form.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/api/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/api/register_account.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/api/register_account.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/bootstrap_field.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/bootstrap_field.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/generic/delete_object.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/generic/delete_object.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/legal/base.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/legal/base.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/legal/legal_notice.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/legal/legal_notice.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/legal/privacy_statement.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/legal/privacy_statement.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/modals/modal_base.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/modals/modal_base.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/loggedout.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/loggedout.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/login.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/login.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/password_change_form.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/password_reset_complete.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/password_reset_confirm.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/password_reset_done.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/password_reset_email.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/registration/password_reset_form.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/setup/base.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/setup/base.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/setup/setup_superuser.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/setup/setup_superuser.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/taxonomy/manage_taxonomic_restrictions.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/taxonomy/manage_taxonomic_restrictions.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/taxonomy/taxonomic_restrictions_form.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/taxonomy/taxonomic_restrictions_form.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/widgets/ajax_file_input.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/widgets/ajax_file_input.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/widgets/app_theme_image_file_input.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/widgets/app_theme_image_file_input.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/widgets/crop_image_input.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/widgets/crop_image_input.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/widgets/taxonomy/taxon_autocomplete_widget_base.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/widgets/taxonomy/taxon_autocomplete_widget_base.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templates/localcosmos_server/widgets/two_step_file_input.html` & `localcosmos_server-0.9.4/localcosmos_server/templates/localcosmos_server/widgets/two_step_file_input.html`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/templatetags/localcosmos_tags.py` & `localcosmos_server-0.9.4/localcosmos_server/templatetags/localcosmos_tags.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/urls.py` & `localcosmos_server-0.9.4/localcosmos_server/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/utils.py` & `localcosmos_server-0.9.4/localcosmos_server/utils.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/validators.py` & `localcosmos_server-0.9.4/localcosmos_server/validators.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/view_mixins.py` & `localcosmos_server-0.9.4/localcosmos_server/view_mixins.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/views.py` & `localcosmos_server-0.9.4/localcosmos_server/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server/widgets.py` & `localcosmos_server-0.9.4/localcosmos_server/widgets.py`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/localcosmos_server.egg-info/PKG-INFO` & `localcosmos_server-0.9.4/localcosmos_server.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localcosmos-server
-Version: 0.9.3
+Version: 0.9.4
 Summary: LocalCosmos Private Server. Run your own server for localcosmos.org apps.
 Home-page: https://github.com/SiSol-Systems/localcosmos-server
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,localcosmos,localcosmos server,biodiversity
 Platform: OS Independent
@@ -19,9 +19,7 @@
 ==================
 
 Private Server for localcosmos.org apps
 
 Documentation
 -------------
 Documentation and Tutorial: https://localcosmos-server.readthedocs.io/en/latest/
-
-
```

### Comparing `localcosmos_server-0.9.3/localcosmos_server.egg-info/SOURCES.txt` & `localcosmos_server-0.9.4/localcosmos_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localcosmos_server-0.9.3/setup.py` & `localcosmos_server-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     'django-cors-headers==3.5.0',
     'Pillow',
     'matplotlib',
 ]
 
 setup(
     name='localcosmos_server',
-    version='0.9.3',
+    version='0.9.4',
     description='LocalCosmos Private Server. Run your own server for localcosmos.org apps.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='The MIT License',
     platforms=['OS Independent'],
     keywords='django, localcosmos, localcosmos server, biodiversity',
     author='Thomas Uher',
```

