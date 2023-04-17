# Comparing `tmp/django-form-surveys-1.8.0.tar.gz` & `tmp/django-form-surveys-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-form-surveys-1.8.0.tar", last modified: Wed Mar 15 09:12:59 2023, max compression
+gzip compressed data, was "django-form-surveys-1.8.1.tar", last modified: Mon Apr 17 04:17:11 2023, max compression
```

## Comparing `django-form-surveys-1.8.0.tar` & `django-form-surveys-1.8.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-15 09:12:59.583092 django-form-surveys-1.8.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1059 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6392 2023-03-15 09:12:59.579092 django-form-surveys-1.8.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5144 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-15 09:12:59.507093 django-form-surveys-1.8.0/django_form_surveys.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6392 2023-03-15 09:12:59.000000 django-form-surveys-1.8.0/django_form_surveys.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3478 2023-03-15 09:12:59.000000 django-form-surveys-1.8.0/django_form_surveys.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-15 09:12:59.000000 django-form-surveys-1.8.0/django_form_surveys.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-12-03 04:02:38.000000 django-form-surveys-1.8.0/django_form_surveys.egg-info/not-zip-safe
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       17 2023-03-15 09:12:59.000000 django-form-surveys-1.8.0/django_form_surveys.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-03-15 09:12:59.000000 django-form-surveys-1.8.0/django_form_surveys.egg-info/top_level.txt
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-15 09:12:59.535092 django-form-surveys-1.8.0/djf_surveys/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       81 2023-03-15 09:09:19.000000 django-form-surveys-1.8.0/djf_surveys/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      977 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/admin.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-15 09:12:59.539092 django-form-surveys-1.8.0/djf_surveys/admins/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/admins/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1298 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/admins/urls.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8146 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/admins/views.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1650 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/app_settings.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      194 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/apps.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      228 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/context_processors.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6449 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/forms.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-15 09:12:59.563092 django-form-surveys-1.8.0/djf_surveys/migrations/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3775 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/migrations/0001_initial.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      860 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/migrations/0002_auto_20220330_1033.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      553 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/migrations/0003_auto_20220330_1036.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      850 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/migrations/0004_auto_20220330_1112.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      377 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/migrations/0005_auto_20220404_1518.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      451 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/migrations/0006_survey_private_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      895 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/migrations/0007_auto_20220525_1126.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/migrations/0008_auto_20220721_0935.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      784 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/migrations/0009_auto_20220803_0927.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8956 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/migrations/0010_model_translation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      662 2022-12-26 04:31:54.000000 django-form-surveys-1.8.0/djf_surveys/migrations/0011_alter_question_key.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/migrations/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      611 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/mixin.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7066 2022-12-26 04:31:54.000000 django-form-surveys-1.8.0/djf_surveys/models.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-15 09:12:59.495093 django-form-surveys-1.8.0/djf_surveys/static/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-15 09:12:59.495093 django-form-surveys-1.8.0/djf_surveys/static/djf_surveys/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-15 09:12:59.563092 django-form-surveys-1.8.0/djf_surveys/static/djf_surveys/css/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      321 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/static/djf_surveys/css/rating.css
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-15 09:12:59.563092 django-form-surveys-1.8.0/djf_surveys/static/djf_surveys/images/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2962 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/static/djf_surveys/images/star-border.png
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2729 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/static/djf_surveys/images/star-fill.png
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7170 2022-12-26 04:13:44.000000 django-form-surveys-1.8.0/djf_surveys/summary.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-15 09:12:59.499093 django-form-surveys-1.8.0/djf_surveys/templates/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-15 09:12:59.563092 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-15 09:12:59.567092 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/admins/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1761 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/admins/form.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6956 2022-12-02 18:18:26.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/admins/form_preview.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      998 2022-12-02 18:12:38.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/admins/master.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      702 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/admins/question_form.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1793 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/admins/summary.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1490 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/admins/survey_list.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4238 2022-12-02 18:18:26.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/answer_list.html
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-15 09:12:59.567092 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/buttons/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      292 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/buttons/add_button.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      343 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/buttons/delete_button.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      309 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/buttons/edit_button.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      457 2022-12-02 18:18:26.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/buttons/share_button.html
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-15 09:12:59.571092 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1638 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/alert.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      326 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/alert_js.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2955 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/card_list_answer.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2779 2022-12-02 01:19:44.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/card_list_survey.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      347 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/empty_state.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3324 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/header_nav.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2386 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/modal_delete.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      774 2022-12-02 18:18:26.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/modal_delete_js.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5379 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/pagination.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      938 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/search_form.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      542 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/section_welcome.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      557 2022-12-02 18:18:26.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/share_link_button_js.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      557 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/star_border.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/star_fill.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      890 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/detail_result.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2015 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/form.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      786 2022-12-02 18:12:32.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/master.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1173 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/survey_list.html
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-15 09:12:59.579092 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/widgets/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      538 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      291 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/widgets/datepicker.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/widgets/radio_option.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1767 2023-03-15 09:08:50.000000 django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/widgets/star_rating.html
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-15 09:12:59.579092 django-form-surveys-1.8.0/djf_surveys/templatetags/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/templatetags/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      509 2023-03-15 09:08:50.000000 django-form-surveys-1.8.0/djf_surveys/templatetags/djf_survey_tags.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      396 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/tests.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      799 2022-12-02 18:18:26.000000 django-form-surveys-1.8.0/djf_surveys/urls.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2277 2023-03-15 09:08:50.000000 django-form-surveys-1.8.0/djf_surveys/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      550 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/djf_surveys/validators.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8190 2022-12-26 03:50:09.000000 django-form-surveys-1.8.0/djf_surveys/views.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      477 2022-10-24 00:52:04.000000 django-form-surveys-1.8.0/djf_surveys/widgets.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-03-15 09:12:59.583092 django-form-surveys-1.8.0/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3085 2022-12-01 07:58:14.000000 django-form-surveys-1.8.0/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.538561 django-form-surveys-1.8.1/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1059 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6392 2023-04-17 04:17:11.534561 django-form-surveys-1.8.1/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5144 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.466562 django-form-surveys-1.8.1/django_form_surveys.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6392 2023-04-17 04:17:11.000000 django-form-surveys-1.8.1/django_form_surveys.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3478 2023-04-17 04:17:11.000000 django-form-surveys-1.8.1/django_form_surveys.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-17 04:17:11.000000 django-form-surveys-1.8.1/django_form_surveys.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-12-03 04:02:38.000000 django-form-surveys-1.8.1/django_form_surveys.egg-info/not-zip-safe
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       17 2023-04-17 04:17:11.000000 django-form-surveys-1.8.1/django_form_surveys.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-04-17 04:17:11.000000 django-form-surveys-1.8.1/django_form_surveys.egg-info/top_level.txt
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.482561 django-form-surveys-1.8.1/djf_surveys/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       81 2023-04-17 04:12:08.000000 django-form-surveys-1.8.1/djf_surveys/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      977 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/admin.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.486561 django-form-surveys-1.8.1/djf_surveys/admins/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/admins/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1298 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/admins/urls.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8146 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/admins/views.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1650 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/app_settings.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      194 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/apps.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      228 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/context_processors.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6449 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/forms.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.498561 django-form-surveys-1.8.1/djf_surveys/migrations/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3775 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0001_initial.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      860 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0002_auto_20220330_1033.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      553 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0003_auto_20220330_1036.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      850 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0004_auto_20220330_1112.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      377 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0005_auto_20220404_1518.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      451 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0006_survey_private_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      895 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0007_auto_20220525_1126.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0008_auto_20220721_0935.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      784 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0009_auto_20220803_0927.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8956 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0010_model_translation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      662 2022-12-26 04:31:54.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0011_alter_question_key.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      611 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/mixin.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7182 2023-04-17 04:11:38.000000 django-form-surveys-1.8.1/djf_surveys/models.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.462562 django-form-surveys-1.8.1/djf_surveys/static/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.462562 django-form-surveys-1.8.1/djf_surveys/static/djf_surveys/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.498561 django-form-surveys-1.8.1/djf_surveys/static/djf_surveys/css/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      321 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/static/djf_surveys/css/rating.css
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.502561 django-form-surveys-1.8.1/djf_surveys/static/djf_surveys/images/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2962 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/static/djf_surveys/images/star-border.png
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2729 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/static/djf_surveys/images/star-fill.png
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7170 2022-12-26 04:13:44.000000 django-form-surveys-1.8.1/djf_surveys/summary.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.462562 django-form-surveys-1.8.1/djf_surveys/templates/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.502561 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.510561 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1761 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/form.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6956 2022-12-02 18:18:26.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/form_preview.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      998 2022-12-02 18:12:38.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/master.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      702 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/question_form.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1793 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/summary.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1490 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/survey_list.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4238 2022-12-02 18:18:26.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/answer_list.html
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.514561 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/buttons/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      292 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/buttons/add_button.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      343 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/buttons/delete_button.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      309 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/buttons/edit_button.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      457 2022-12-02 18:18:26.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/buttons/share_button.html
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.526561 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1638 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/alert.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      326 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/alert_js.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2955 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/card_list_answer.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2779 2022-12-02 01:19:44.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/card_list_survey.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      347 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/empty_state.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3324 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/header_nav.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2386 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/modal_delete.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      774 2022-12-02 18:18:26.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/modal_delete_js.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5379 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/pagination.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      938 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/search_form.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      542 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/section_welcome.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      557 2022-12-02 18:18:26.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/share_link_button_js.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      557 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/star_border.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/star_fill.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      890 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/detail_result.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2015 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/form.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      786 2022-12-02 18:12:32.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/master.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1173 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/survey_list.html
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.534561 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/widgets/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      538 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      291 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/widgets/datepicker.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/widgets/radio_option.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1767 2023-03-15 09:08:50.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/widgets/star_rating.html
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.534561 django-form-surveys-1.8.1/djf_surveys/templatetags/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templatetags/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      509 2023-03-15 09:08:50.000000 django-form-surveys-1.8.1/djf_surveys/templatetags/djf_survey_tags.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      396 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/tests.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      799 2022-12-02 18:18:26.000000 django-form-surveys-1.8.1/djf_surveys/urls.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2277 2023-03-15 09:08:50.000000 django-form-surveys-1.8.1/djf_surveys/utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      550 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/validators.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8190 2022-12-26 03:50:09.000000 django-form-surveys-1.8.1/djf_surveys/views.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      477 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/widgets.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-17 04:17:11.538561 django-form-surveys-1.8.1/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3085 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/setup.py
```

### Comparing `django-form-surveys-1.8.0/LICENSE` & `django-form-surveys-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/PKG-INFO` & `django-form-surveys-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-form-surveys
-Version: 1.8.0
+Version: 1.8.1
 Summary: A simple Django app to conduct Web-based survey
 Home-page: https://irfanpule.github.io/django-form-surveys
 Author: irfanpule
 Author-email: irfan.pule2@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-form-surveys-1.8.0/README.md` & `django-form-surveys-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/django_form_surveys.egg-info/PKG-INFO` & `django-form-surveys-1.8.1/django_form_surveys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-form-surveys
-Version: 1.8.0
+Version: 1.8.1
 Summary: A simple Django app to conduct Web-based survey
 Home-page: https://irfanpule.github.io/django-form-surveys
 Author: irfanpule
 Author-email: irfan.pule2@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-form-surveys-1.8.0/django_form_surveys.egg-info/SOURCES.txt` & `django-form-surveys-1.8.1/django_form_surveys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/admin.py` & `django-form-surveys-1.8.1/djf_surveys/admin.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/admins/urls.py` & `django-form-surveys-1.8.1/djf_surveys/admins/urls.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/admins/views.py` & `django-form-surveys-1.8.1/djf_surveys/admins/views.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/app_settings.py` & `django-form-surveys-1.8.1/djf_surveys/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/forms.py` & `django-form-surveys-1.8.1/djf_surveys/forms.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/migrations/0001_initial.py` & `django-form-surveys-1.8.1/djf_surveys/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/migrations/0002_auto_20220330_1033.py` & `django-form-surveys-1.8.1/djf_surveys/migrations/0002_auto_20220330_1033.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/migrations/0003_auto_20220330_1036.py` & `django-form-surveys-1.8.1/djf_surveys/migrations/0003_auto_20220330_1036.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/migrations/0004_auto_20220330_1112.py` & `django-form-surveys-1.8.1/djf_surveys/migrations/0004_auto_20220330_1112.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/migrations/0007_auto_20220525_1126.py` & `django-form-surveys-1.8.1/djf_surveys/migrations/0007_auto_20220525_1126.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/migrations/0008_auto_20220721_0935.py` & `django-form-surveys-1.8.1/djf_surveys/migrations/0008_auto_20220721_0935.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/migrations/0009_auto_20220803_0927.py` & `django-form-surveys-1.8.1/djf_surveys/migrations/0009_auto_20220803_0927.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/migrations/0010_model_translation.py` & `django-form-surveys-1.8.1/djf_surveys/migrations/0010_model_translation.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/migrations/0011_alter_question_key.py` & `django-form-surveys-1.8.1/djf_surveys/migrations/0011_alter_question_key.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/mixin.py` & `django-form-surveys-1.8.1/djf_surveys/mixin.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/models.py` & `django-form-surveys-1.8.1/djf_surveys/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -132,17 +132,21 @@
         verbose_name_plural = _("user answers")
         ordering = ["-updated_at"]
 
     def __str__(self):
         return str(self.id)
 
     def get_user_photo(self):
+        default_photo = "https://cdn.pixabay.com/photo/2015/10/05/22/37/blank-profile-picture-973460_960_720.png"
         if app_settings.SURVEY_USER_PHOTO_PROFILE:
-            return eval(app_settings.SURVEY_USER_PHOTO_PROFILE)
-        return "https://cdn.pixabay.com/photo/2015/10/05/22/37/blank-profile-picture-973460_960_720.png"
+            try:
+                return eval(app_settings.SURVEY_USER_PHOTO_PROFILE)
+            except:
+                return default_photo
+        return default_photo
 
 
 class Answer(BaseModel):
     question = models.ForeignKey(Question, related_name="answers", on_delete=models.CASCADE, verbose_name=_("question"))
     value = models.TextField(_("value"), help_text=_("The value of the answer given by the user."))
     user_answer = models.ForeignKey(UserAnswer, on_delete=models.CASCADE, verbose_name=_("user answer"))
```

### Comparing `django-form-surveys-1.8.0/djf_surveys/static/djf_surveys/images/star-border.png` & `django-form-surveys-1.8.1/djf_surveys/static/djf_surveys/images/star-border.png`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/static/djf_surveys/images/star-fill.png` & `django-form-surveys-1.8.1/djf_surveys/static/djf_surveys/images/star-fill.png`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/summary.py` & `django-form-surveys-1.8.1/djf_surveys/summary.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/admins/form.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/admins/form_preview.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/form_preview.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/admins/master.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/master.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/admins/question_form.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/question_form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/admins/summary.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/summary.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/admins/survey_list.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/survey_list.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/answer_list.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/answer_list.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/alert.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/alert.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/card_list_answer.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/card_list_answer.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/card_list_survey.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/card_list_survey.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/header_nav.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/header_nav.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/modal_delete.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/modal_delete.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/modal_delete_js.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/modal_delete_js.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/pagination.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/pagination.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/search_form.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/search_form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/section_welcome.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/section_welcome.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/share_link_button_js.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/share_link_button_js.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/components/star_border.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/star_border.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/detail_result.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/detail_result.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/form.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/master.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/master.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/survey_list.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/survey_list.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/widgets/radio_option.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/widgets/radio_option.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/templates/djf_surveys/widgets/star_rating.html` & `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/widgets/star_rating.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/urls.py` & `django-form-surveys-1.8.1/djf_surveys/urls.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/utils.py` & `django-form-surveys-1.8.1/djf_surveys/utils.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/validators.py` & `django-form-surveys-1.8.1/djf_surveys/validators.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/djf_surveys/views.py` & `django-form-surveys-1.8.1/djf_surveys/views.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.0/setup.py` & `django-form-surveys-1.8.1/setup.py`

 * *Files identical despite different names*

