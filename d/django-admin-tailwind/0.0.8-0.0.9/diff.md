# Comparing `tmp/django-admin-tailwind-0.0.8.tar.gz` & `tmp/django-admin-tailwind-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-tailwind-0.0.8.tar", last modified: Wed Jul  7 15:39:11 2021, max compression
+gzip compressed data, was "django-admin-tailwind-0.0.9.tar", last modified: Wed Jul  7 15:42:14 2021, max compression
```

## Comparing `django-admin-tailwind-0.0.8.tar` & `django-admin-tailwind-0.0.9.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:39:11.729020 django-admin-tailwind-0.0.8/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)    35121 2020-12-20 13:19:23.000000 django-admin-tailwind-0.0.8/LICENSE
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      103 2021-07-05 09:47:59.000000 django-admin-tailwind-0.0.8/MANIFEST.in
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1892 2021-07-07 15:39:11.729020 django-admin-tailwind-0.0.8/PKG-INFO
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1117 2021-07-07 14:59:14.000000 django-admin-tailwind-0.0.8/README.rst
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:39:11.725020 django-admin-tailwind-0.0.8/app/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-06-08 16:00:47.000000 django-admin-tailwind-0.0.8/app/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      727 2021-07-07 15:18:09.000000 django-admin-tailwind-0.0.8/app/admin.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      128 2021-06-08 16:00:40.000000 django-admin-tailwind-0.0.8/app/apps.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      401 2021-06-03 12:03:35.000000 django-admin-tailwind-0.0.8/app/asgi.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:39:11.725020 django-admin-tailwind-0.0.8/app/fixtures/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-07-03 15:44:18.000000 django-admin-tailwind-0.0.8/app/fixtures/__init__.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:39:11.725020 django-admin-tailwind-0.0.8/app/management/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2020-12-20 13:19:29.000000 django-admin-tailwind-0.0.8/app/management/__init__.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:39:11.725020 django-admin-tailwind-0.0.8/app/management/commands/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2020-12-20 13:19:29.000000 django-admin-tailwind-0.0.8/app/management/commands/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1022 2021-07-03 15:54:58.000000 django-admin-tailwind-0.0.8/app/management/commands/init.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:39:11.725020 django-admin-tailwind-0.0.8/app/migrations/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1466 2021-07-03 15:45:05.000000 django-admin-tailwind-0.0.8/app/migrations/0001_initial.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-07-03 15:39:25.000000 django-admin-tailwind-0.0.8/app/migrations/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      762 2021-07-03 15:46:35.000000 django-admin-tailwind-0.0.8/app/models.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     4100 2021-07-07 15:07:01.000000 django-admin-tailwind-0.0.8/app/settings.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      757 2021-06-03 12:03:35.000000 django-admin-tailwind-0.0.8/app/urls.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      401 2021-06-03 12:03:35.000000 django-admin-tailwind-0.0.8/app/wsgi.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:39:11.725020 django-admin-tailwind-0.0.8/django_admin_tailwind/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       76 2021-06-03 12:03:35.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      194 2021-06-03 12:03:35.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/apps.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       96 2021-06-14 08:18:42.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/context.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:39:11.725020 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:39:11.725020 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      282 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/404.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     2402 2021-06-04 14:57:52.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/500.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     2080 2021-07-07 15:36:55.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/actions.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     2464 2021-06-04 14:57:52.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/app_index.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     4059 2021-06-10 14:04:48.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/app_list.html
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:39:11.721020 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/auth/
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:39:11.725020 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/auth/user/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      320 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/auth/user/add_form.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     2193 2021-06-10 12:03:18.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/auth/user/change_password.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)    23862 2021-07-07 15:06:23.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/base.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      642 2021-06-11 09:07:51.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/base_site.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     7082 2021-06-10 12:07:44.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/change_form.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      560 2021-06-11 08:07:56.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/change_form_object_tools.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     6980 2021-07-07 15:38:25.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/change_list.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      455 2021-07-05 09:56:57.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/change_list_object_tools.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     2508 2021-07-07 14:16:01.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/change_list_results.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      518 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/date_hierarchy.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     6812 2021-06-11 10:08:58.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/delete_confirmation.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     6460 2021-06-11 10:08:58.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/delete_selected_confirmation.html
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:39:11.725020 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/edit_inline/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     2554 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/edit_inline/stacked.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     4485 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/edit_inline/tabular.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      338 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/filter.html
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:39:11.725020 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/includes/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1829 2021-06-10 14:11:06.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/includes/fieldset.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      192 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/includes/object_delete_summary.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     7558 2021-06-08 13:25:50.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/index.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     2294 2021-06-04 14:57:52.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/invalid_setup.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     3835 2021-07-07 13:44:27.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/login.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      486 2021-07-07 13:40:00.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/nav_sidebar.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     5638 2021-06-11 08:41:39.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/object_history.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      714 2021-07-05 09:53:50.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/pagination.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      327 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/popup_response.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      209 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/prepopulated_fields_js.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1608 2021-07-07 15:24:04.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/search_form.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1641 2021-06-14 12:25:27.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/submit_line.html
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:39:11.729020 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/widgets/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      618 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/widgets/clearable_file_input.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      341 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/widgets/foreign_key_raw_id.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       54 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/widgets/many_to_many_raw_id.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       57 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/widgets/radio.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1490 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/widgets/related_widget_wrapper.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      238 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/widgets/split_datetime.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      218 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/widgets/url.html
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:39:11.729020 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/registration/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      518 2021-06-11 08:24:28.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/registration/logged_out.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      443 2021-06-11 08:28:49.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/registration/password_change_done.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     2481 2021-06-11 08:25:55.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/registration/password_change_form.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      246 2021-06-04 14:05:34.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/registration/password_reset_complete.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1059 2021-06-10 12:07:44.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/registration/password_reset_confirm.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      417 2021-06-04 12:59:47.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/registration/password_reset_done.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      612 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/registration/password_reset_email.html
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      647 2021-06-10 12:07:44.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templates/registration/password_reset_form.html
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:39:11.729020 django-admin-tailwind-0.0.8/django_admin_tailwind/templatetags/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-06-14 08:16:07.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templatetags/__init__.py
--rw-rw-r--   0 ariane    (1000) ariane    (1000)      179 2021-06-14 08:04:01.000000 django-admin-tailwind-0.0.8/django_admin_tailwind/templatetags/context.py
-drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:39:11.725020 django-admin-tailwind-0.0.8/django_admin_tailwind.egg-info/
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     1892 2021-07-07 15:39:11.000000 django-admin-tailwind-0.0.8/django_admin_tailwind.egg-info/PKG-INFO
--rw-rw-r--   0 ariane    (1000) ariane    (1000)     3571 2021-07-07 15:39:11.000000 django-admin-tailwind-0.0.8/django_admin_tailwind.egg-info/SOURCES.txt
--rw-rw-r--   0 ariane    (1000) ariane    (1000)        1 2021-07-07 15:39:11.000000 django-admin-tailwind-0.0.8/django_admin_tailwind.egg-info/dependency_links.txt
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       26 2021-07-07 15:39:11.000000 django-admin-tailwind-0.0.8/django_admin_tailwind.egg-info/top_level.txt
--rw-rw-r--   0 ariane    (1000) ariane    (1000)       38 2021-07-07 15:39:11.729020 django-admin-tailwind-0.0.8/setup.cfg
--rwxrwxr-x   0 ariane    (1000) ariane    (1000)     1231 2021-06-03 12:24:31.000000 django-admin-tailwind-0.0.8/setup.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:42:14.540435 django-admin-tailwind-0.0.9/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)    35121 2020-12-20 13:19:23.000000 django-admin-tailwind-0.0.9/LICENSE
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      103 2021-07-05 09:47:59.000000 django-admin-tailwind-0.0.9/MANIFEST.in
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1892 2021-07-07 15:42:14.540435 django-admin-tailwind-0.0.9/PKG-INFO
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1117 2021-07-07 14:59:14.000000 django-admin-tailwind-0.0.9/README.rst
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:42:14.536435 django-admin-tailwind-0.0.9/app/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-06-08 16:00:47.000000 django-admin-tailwind-0.0.9/app/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      727 2021-07-07 15:18:09.000000 django-admin-tailwind-0.0.9/app/admin.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      128 2021-06-08 16:00:40.000000 django-admin-tailwind-0.0.9/app/apps.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      401 2021-06-03 12:03:35.000000 django-admin-tailwind-0.0.9/app/asgi.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:42:14.536435 django-admin-tailwind-0.0.9/app/fixtures/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-07-03 15:44:18.000000 django-admin-tailwind-0.0.9/app/fixtures/__init__.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:42:14.536435 django-admin-tailwind-0.0.9/app/management/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2020-12-20 13:19:29.000000 django-admin-tailwind-0.0.9/app/management/__init__.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:42:14.536435 django-admin-tailwind-0.0.9/app/management/commands/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2020-12-20 13:19:29.000000 django-admin-tailwind-0.0.9/app/management/commands/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1022 2021-07-03 15:54:58.000000 django-admin-tailwind-0.0.9/app/management/commands/init.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:42:14.536435 django-admin-tailwind-0.0.9/app/migrations/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1466 2021-07-03 15:45:05.000000 django-admin-tailwind-0.0.9/app/migrations/0001_initial.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-07-03 15:39:25.000000 django-admin-tailwind-0.0.9/app/migrations/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      762 2021-07-03 15:46:35.000000 django-admin-tailwind-0.0.9/app/models.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     4100 2021-07-07 15:07:01.000000 django-admin-tailwind-0.0.9/app/settings.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      757 2021-06-03 12:03:35.000000 django-admin-tailwind-0.0.9/app/urls.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      401 2021-06-03 12:03:35.000000 django-admin-tailwind-0.0.9/app/wsgi.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:42:14.536435 django-admin-tailwind-0.0.9/django_admin_tailwind/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       76 2021-06-03 12:03:35.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      194 2021-06-03 12:03:35.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/apps.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       96 2021-06-14 08:18:42.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/context.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:42:14.536435 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:42:14.536435 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      282 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/404.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     2402 2021-06-04 14:57:52.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/500.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     2080 2021-07-07 15:36:55.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/actions.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     2464 2021-06-04 14:57:52.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/app_index.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     4031 2021-07-07 15:41:28.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/app_list.html
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:42:14.536435 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/auth/
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:42:14.536435 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/auth/user/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      320 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/auth/user/add_form.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     2193 2021-06-10 12:03:18.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/auth/user/change_password.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)    23862 2021-07-07 15:06:23.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/base.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      642 2021-06-11 09:07:51.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/base_site.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     7082 2021-06-10 12:07:44.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/change_form.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      560 2021-06-11 08:07:56.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/change_form_object_tools.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     6980 2021-07-07 15:38:25.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/change_list.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      455 2021-07-05 09:56:57.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/change_list_object_tools.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     2508 2021-07-07 14:16:01.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/change_list_results.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      518 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/date_hierarchy.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     6812 2021-06-11 10:08:58.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/delete_confirmation.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     6460 2021-06-11 10:08:58.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/delete_selected_confirmation.html
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:42:14.536435 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/edit_inline/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     2554 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/edit_inline/stacked.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     4485 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/edit_inline/tabular.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      338 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/filter.html
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:42:14.536435 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/includes/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1829 2021-06-10 14:11:06.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/includes/fieldset.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      192 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/includes/object_delete_summary.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     7558 2021-06-08 13:25:50.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/index.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     2294 2021-06-04 14:57:52.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/invalid_setup.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     3835 2021-07-07 13:44:27.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/login.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      486 2021-07-07 13:40:00.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/nav_sidebar.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     5638 2021-06-11 08:41:39.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/object_history.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      714 2021-07-05 09:53:50.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/pagination.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      327 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/popup_response.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      209 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/prepopulated_fields_js.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1608 2021-07-07 15:24:04.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/search_form.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1641 2021-06-14 12:25:27.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/submit_line.html
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:42:14.540435 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/widgets/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      618 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/widgets/clearable_file_input.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      341 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/widgets/foreign_key_raw_id.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       54 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/widgets/many_to_many_raw_id.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       57 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/widgets/radio.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1490 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/widgets/related_widget_wrapper.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      238 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/widgets/split_datetime.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      218 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/widgets/url.html
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:42:14.540435 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/registration/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      518 2021-06-11 08:24:28.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/registration/logged_out.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      443 2021-06-11 08:28:49.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/registration/password_change_done.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     2481 2021-06-11 08:25:55.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/registration/password_change_form.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      246 2021-06-04 14:05:34.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/registration/password_reset_complete.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1059 2021-06-10 12:07:44.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/registration/password_reset_confirm.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      417 2021-06-04 12:59:47.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/registration/password_reset_done.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      612 2021-06-03 13:42:09.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/registration/password_reset_email.html
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      647 2021-06-10 12:07:44.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templates/registration/password_reset_form.html
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:42:14.540435 django-admin-tailwind-0.0.9/django_admin_tailwind/templatetags/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        0 2021-06-14 08:16:07.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templatetags/__init__.py
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)      179 2021-06-14 08:04:01.000000 django-admin-tailwind-0.0.9/django_admin_tailwind/templatetags/context.py
+drwxrwxr-x   0 ariane    (1000) ariane    (1000)        0 2021-07-07 15:42:14.536435 django-admin-tailwind-0.0.9/django_admin_tailwind.egg-info/
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     1892 2021-07-07 15:42:14.000000 django-admin-tailwind-0.0.9/django_admin_tailwind.egg-info/PKG-INFO
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)     3571 2021-07-07 15:42:14.000000 django-admin-tailwind-0.0.9/django_admin_tailwind.egg-info/SOURCES.txt
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)        1 2021-07-07 15:42:14.000000 django-admin-tailwind-0.0.9/django_admin_tailwind.egg-info/dependency_links.txt
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       26 2021-07-07 15:42:14.000000 django-admin-tailwind-0.0.9/django_admin_tailwind.egg-info/top_level.txt
+-rw-rw-r--   0 ariane    (1000) ariane    (1000)       38 2021-07-07 15:42:14.540435 django-admin-tailwind-0.0.9/setup.cfg
+-rwxrwxr-x   0 ariane    (1000) ariane    (1000)     1231 2021-06-03 12:24:31.000000 django-admin-tailwind-0.0.9/setup.py
```

### Comparing `django-admin-tailwind-0.0.8/LICENSE` & `django-admin-tailwind-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/PKG-INFO` & `django-admin-tailwind-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-tailwind
-Version: 0.0.8
+Version: 0.0.9
 Summary: Django Admin Tailwind
 Home-page: https://github.com/Aleksi44/django-admin-tailwind
 Author: Alexis Le Baron
 Author-email: hello@snoweb.fr
 License: GPL-3.0
 Keywords: django django-admin tailwind
 Platform: linux
```

### Comparing `django-admin-tailwind-0.0.8/README.rst` & `django-admin-tailwind-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/app/admin.py` & `django-admin-tailwind-0.0.9/app/admin.py`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/app/management/commands/init.py` & `django-admin-tailwind-0.0.9/app/management/commands/init.py`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/app/migrations/0001_initial.py` & `django-admin-tailwind-0.0.9/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/app/models.py` & `django-admin-tailwind-0.0.9/app/models.py`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/app/settings.py` & `django-admin-tailwind-0.0.9/app/settings.py`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/app/urls.py` & `django-admin-tailwind-0.0.9/app/urls.py`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/500.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/500.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/actions.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/app_index.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/app_index.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/app_list.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/app_list.html`

 * *Files 8% similar despite different names*

```diff
@@ -20,20 +20,20 @@
                             </thead>
                             <tbody>
                             {% for model in app.models %}
 
                                 <tr class="flex items-center">
                                 {% if model.admin_url %}
                                     <td class="flex-grow">
-                                        <a class="break-all" href="{{ model.admin_url }}"
+                                        <a href="{{ model.admin_url }}"
                                                 {% if model.admin_url in request.path %}
                                            aria-current="page"{% endif %}>{{ model.name }}</a>
                                     </td>
                                 {% else %}
-                                    <td class="break-all flex-grow">
+                                    <td class="flex-grow">
                                         {{ model.name }}
                                     </td>
                                 {% endif %}
 
 
                                 <td class="p-4 flex-none">
                                     {% if model.add_url %}
```

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/auth/user/change_password.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/base.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/base_site.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/change_form.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/change_form_object_tools.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/change_form_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/change_list.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/change_list_results.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/date_hierarchy.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/date_hierarchy.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/delete_confirmation.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/delete_selected_confirmation.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/edit_inline/stacked.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/edit_inline/tabular.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/includes/fieldset.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/index.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/invalid_setup.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/invalid_setup.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/login.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/object_history.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/pagination.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/search_form.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/submit_line.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/widgets/clearable_file_input.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/admin/widgets/related_widget_wrapper.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/admin/widgets/related_widget_wrapper.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/registration/logged_out.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/registration/password_change_form.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/registration/password_reset_confirm.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/registration/password_reset_email.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind/templates/registration/password_reset_form.html` & `django-admin-tailwind-0.0.9/django_admin_tailwind/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind.egg-info/PKG-INFO` & `django-admin-tailwind-0.0.9/django_admin_tailwind.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-tailwind
-Version: 0.0.8
+Version: 0.0.9
 Summary: Django Admin Tailwind
 Home-page: https://github.com/Aleksi44/django-admin-tailwind
 Author: Alexis Le Baron
 Author-email: hello@snoweb.fr
 License: GPL-3.0
 Keywords: django django-admin tailwind
 Platform: linux
```

### Comparing `django-admin-tailwind-0.0.8/django_admin_tailwind.egg-info/SOURCES.txt` & `django-admin-tailwind-0.0.9/django_admin_tailwind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-tailwind-0.0.8/setup.py` & `django-admin-tailwind-0.0.9/setup.py`

 * *Files identical despite different names*

