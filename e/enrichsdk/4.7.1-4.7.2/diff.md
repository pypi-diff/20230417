# Comparing `tmp/enrichsdk-4.7.1.tar.gz` & `tmp/enrichsdk-4.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enrichsdk-4.7.1.tar", last modified: Mon Apr 10 14:58:57 2023, max compression
+gzip compressed data, was "enrichsdk-4.7.2.tar", last modified: Mon Apr 17 03:51:59 2023, max compression
```

## Comparing `enrichsdk-4.7.1.tar` & `enrichsdk-4.7.2.tar`

### file list

```diff
@@ -1,329 +1,329 @@
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.539179 enrichsdk-4.7.1/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      806 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/LICENSE
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      203 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/MANIFEST.in
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3298 2023-04-10 14:58:57.539179 enrichsdk-4.7.1/PKG-INFO
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2182 2023-01-17 09:28:06.000000 enrichsdk-4.7.1/README.rst
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.463178 enrichsdk-4.7.1/enrichsdk/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1676 2023-04-07 09:22:12.000000 enrichsdk-4.7.1/enrichsdk/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.463178 enrichsdk-4.7.1/enrichsdk/api/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6446 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/api/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6001 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/api/draw.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.463178 enrichsdk-4.7.1/enrichsdk/app/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       35 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/app/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.463178 enrichsdk-4.7.1/enrichsdk/app/bases/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      369 2023-01-10 11:58:12.000000 enrichsdk-4.7.1/enrichsdk/app/bases/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.467178 enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      183 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      456 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/forms.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2875 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/models.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.455178 enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.455178 enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/enrichapp/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.467178 enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     9438 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_add.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    17335 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    19428 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       92 2022-11-14 13:05:48.000000 enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns_helper.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14153 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_dataset.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3129 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_detail.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14043 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    16391 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/workflow_index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    31979 2023-02-27 08:21:08.000000 enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/views.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.455178 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.455178 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.467178 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.471178 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      272 2023-02-17 05:17:51.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      300 2023-02-17 05:17:51.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button_function.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      212 2023-03-10 06:57:41.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_icon.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      389 2023-04-05 10:39:21.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_search.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1091 2023-02-17 05:17:51.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      694 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      771 2023-02-17 05:17:51.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2475 2023-02-17 05:17:51.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6749 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.471178 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3730 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3601 2023-04-07 09:20:32.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1387 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1591 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_key_value_pairs.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4433 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_linechart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7312 2023-04-10 08:43:47.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8014 2023-03-10 06:57:41.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_filters.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7251 2023-03-10 06:57:41.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_search.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2909 2023-04-07 09:20:24.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_text.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2980 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_widget_with_config.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      214 2023-01-17 09:28:06.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/help.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3417 2023-02-17 05:17:51.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/share.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1529 2023-01-17 08:20:08.000000 enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/sidebar_menu_icon.html
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.475178 enrichsdk-4.7.1/enrichsdk/app/bases/singlepageapp/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      183 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/app/bases/singlepageapp/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      130 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/app/bases/singlepageapp/forms.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/app/bases/singlepageapp/models.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.459178 enrichsdk-4.7.1/enrichsdk/app/bases/singlepageapp/templates/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.459178 enrichsdk-4.7.1/enrichsdk/app/bases/singlepageapp/templates/enrichapp/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.475178 enrichsdk-4.7.1/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2324 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/generic.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      119 2022-11-23 04:27:41.000000 enrichsdk-4.7.1/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/helper.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2224 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10005 2023-02-17 05:17:51.000000 enrichsdk-4.7.1/enrichsdk/app/bases/singlepageapp/views.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3186 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/app/utils.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.475178 enrichsdk-4.7.1/enrichsdk/app/widget/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/app/widget/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      635 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/app/widget/basewidget.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5121 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/app/widget/customcomponent.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3327 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/app/widget/customwidget.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.475178 enrichsdk-4.7.1/enrichsdk/commands/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      176 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/commands/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    11330 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/commands/config.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1431 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/commands/decorators.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3025 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/commands/helper.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2232 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/commands/log.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6436 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/commands/run.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.479178 enrichsdk-4.7.1/enrichsdk/contrib/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       45 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/contrib/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.479178 enrichsdk-4.7.1/enrichsdk/contrib/lib/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       82 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.479178 enrichsdk-4.7.1/enrichsdk/contrib/lib/assets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      227 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/assets/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    25017 2023-02-14 06:43:41.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/assets/anonymizer.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7017 2023-02-07 10:54:16.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/assets/changepoints.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5845 2023-01-10 09:26:26.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/assets/llmtextgen.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7224 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/assets/profilespec.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-16 05:19:04.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/assets/syndata.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3068 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/assets/timeseries_forecasting.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2717 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/catalog.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    26236 2023-01-03 13:19:44.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/logprocessor.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.479178 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      747 2023-04-05 10:39:21.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.483178 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/anomalies/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    33176 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/anomalies/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.483178 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/changepoints/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    33192 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/changepoints/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.483178 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/classifier/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    33641 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/classifier/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.483178 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/data_quality/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    18378 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/data_quality/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.483178 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/feature_compute/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4667 2023-04-04 16:04:30.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/feature_compute/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.483178 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/filebased_query_executor/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1615 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/filebased_query_executor/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    29587 2023-04-04 16:04:30.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/filebased_query_executor/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1743 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/filebased_query_executor/lib.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.483178 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/fileops/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      238 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/fileops/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5046 2023-04-04 16:04:30.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/fileops/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.483178 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/inmemory_query_executor/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    23726 2023-04-04 16:04:30.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/inmemory_query_executor/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.487178 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/metrics/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    17600 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/metrics/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.487178 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/notebook_executor/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      946 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/notebook_executor/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5391 2023-04-04 16:04:30.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/notebook_executor/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.487178 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/observability/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    33314 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/observability/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.487178 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/synthetic_data_generator/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    26037 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/synthetic_data_generator/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.487178 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/timeseries_forecaster/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    25318 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/timeseries_forecaster/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.487178 enrichsdk-4.7.1/enrichsdk/contrib/transforms/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      391 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/contrib/transforms/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.487178 enrichsdk-4.7.1/enrichsdk/contrib/transforms/fileops/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      769 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/contrib/transforms/fileops/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2309 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/contrib/transforms/fileops/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.487178 enrichsdk-4.7.1/enrichsdk/contrib/transforms/jsonsink/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      452 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/contrib/transforms/jsonsink/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7845 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/contrib/transforms/jsonsink/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.491178 enrichsdk-4.7.1/enrichsdk/contrib/transforms/jsonsource/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      514 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/contrib/transforms/jsonsource/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5451 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/contrib/transforms/jsonsource/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.491178 enrichsdk-4.7.1/enrichsdk/contrib/transforms/pqexport/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      909 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/contrib/transforms/pqexport/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     9384 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/contrib/transforms/pqexport/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.491178 enrichsdk-4.7.1/enrichsdk/contrib/transforms/sqlexport/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1450 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/contrib/transforms/sqlexport/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14007 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/contrib/transforms/sqlexport/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.491178 enrichsdk-4.7.1/enrichsdk/contrib/transforms/tablesink/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1187 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/contrib/transforms/tablesink/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     9446 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/contrib/transforms/tablesink/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.491178 enrichsdk-4.7.1/enrichsdk/contrib/transforms/tablesource/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1581 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/contrib/transforms/tablesource/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8317 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/contrib/transforms/tablesource/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.495178 enrichsdk-4.7.1/enrichsdk/core/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      909 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/core/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3428 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/core/frames.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    41276 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/core/mixins.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    52640 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/core/node.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3691 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/core/patch.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7222 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/core/render.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1292 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/core/res.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    32053 2023-04-05 10:39:21.000000 enrichsdk-4.7.1/enrichsdk/core/run.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14634 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/core/sdk.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6898 2023-03-09 06:57:39.000000 enrichsdk-4.7.1/enrichsdk/core/state.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1294 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/core/widgets.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.499179 enrichsdk-4.7.1/enrichsdk/datasets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      552 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/datasets/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    36181 2023-02-21 05:43:43.000000 enrichsdk-4.7.1/enrichsdk/datasets/discover.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    18149 2023-03-01 13:54:44.000000 enrichsdk-4.7.1/enrichsdk/datasets/doodle.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1389 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/datasets/generators.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.499179 enrichsdk-4.7.1/enrichsdk/extractors/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1703 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/extractors/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.499179 enrichsdk-4.7.1/enrichsdk/feature_compute/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    13231 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/feature_compute/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.499179 enrichsdk-4.7.1/enrichsdk/featurestore/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4502 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/featurestore/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10432 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/featurestore/schema.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.507178 enrichsdk-4.7.1/enrichsdk/lib/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    23694 2023-01-03 13:19:44.000000 enrichsdk-4.7.1/enrichsdk/lib/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4945 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/lib/context.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5827 2023-02-26 08:39:33.000000 enrichsdk-4.7.1/enrichsdk/lib/customer.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2069 2023-03-09 06:57:39.000000 enrichsdk-4.7.1/enrichsdk/lib/exceptions.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2903 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/enrichsdk/lib/integration.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      983 2023-01-10 09:26:26.000000 enrichsdk-4.7.1/enrichsdk/lib/misc.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      552 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/lib/permissions.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1212 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/lib/renderlib.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1357 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/lib/resources.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.507178 enrichsdk-4.7.1/enrichsdk/notebook/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8611 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/notebook/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      189 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/notebook/utils.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.507178 enrichsdk-4.7.1/enrichsdk/package/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    86072 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/package/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4194 2023-02-01 09:43:30.000000 enrichsdk-4.7.1/enrichsdk/package/lib.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1629 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/package/log.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14964 2023-01-03 13:19:44.000000 enrichsdk-4.7.1/enrichsdk/package/misc.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    23959 2023-03-09 06:57:39.000000 enrichsdk-4.7.1/enrichsdk/package/mock.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4322 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/package/validators.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.507178 enrichsdk-4.7.1/enrichsdk/policy/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7529 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/policy/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1608 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/policy/sdk.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.511179 enrichsdk-4.7.1/enrichsdk/quality/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2476 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/quality/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5666 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/quality/base.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      925 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/quality/exceptions.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4371 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/quality/expectations.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5157 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/quality/reconciliation.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4884 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/quality/transforms.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.511179 enrichsdk-4.7.1/enrichsdk/realtime/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      283 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/realtime/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2401 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/realtime/db.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      824 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/realtime/log.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5122 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/realtime/messaging.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4056 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/realtime/spark.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4869 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/realtime/transforms.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3173 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/realtime/workflow.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.511179 enrichsdk-4.7.1/enrichsdk/render/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10751 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/render/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.515179 enrichsdk-4.7.1/enrichsdk/scripts/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/scripts/__init__.py
--rwxrwxr-x   0 pingali   (1000) pingali   (1000)     4372 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/scripts/enrichcmd.py
--rwxrwxr-x   0 pingali   (1000) pingali   (1000)    44398 2023-04-05 10:51:48.000000 enrichsdk-4.7.1/enrichsdk/scripts/enrichpkg.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.515179 enrichsdk-4.7.1/enrichsdk/services/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1800 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/services/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.515179 enrichsdk-4.7.1/enrichsdk/tasks/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10443 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/tasks/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.515179 enrichsdk-4.7.1/enrichsdk/tasks/dummy_task/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1839 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/tasks/dummy_task/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8046 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/tasks/sdk.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.527179 enrichsdk-4.7.1/enrichsdk/templates/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       42 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/LICENSE.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       27 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/MANIFEST.in.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      370 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/README.md.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      383 2023-01-02 14:59:19.000000 enrichsdk-4.7.1/enrichsdk/templates/README_PIPELINE.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       53 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/README_TASK.md
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.527179 enrichsdk-4.7.1/enrichsdk/templates/airflow/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1476 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/airflow/contrib-pipeline-v1.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.527179 enrichsdk-4.7.1/enrichsdk/templates/appstore2.0/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3669 2023-01-17 08:20:08.000000 enrichsdk-4.7.1/enrichsdk/templates/appstore2.0/index.html.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.527179 enrichsdk-4.7.1/enrichsdk/templates/assets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4444 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/assets/datasets.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1340 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/config.json.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.531179 enrichsdk-4.7.1/enrichsdk/templates/dashboard/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      180 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/dashboard/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      384 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/dashboard/apps.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      189 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/dashboard/catalog.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      235 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/dashboard/custom.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3455 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/dashboard/persona.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      685 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/dashboard/tasks.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.531179 enrichsdk-4.7.1/enrichsdk/templates/dashboard/templates/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5168 2021-09-14 02:19:33.000000 enrichsdk-4.7.1/enrichsdk/templates/dashboard/templates/complex_result.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2405 2022-03-28 06:32:35.000000 enrichsdk-4.7.1/enrichsdk/templates/dashboard/templates/index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1273 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/dashboard/urls.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4684 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/dashboard/views.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.531179 enrichsdk-4.7.1/enrichsdk/templates/datasets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      311 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/datasets/manifest.json.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5999 2022-08-02 10:38:39.000000 enrichsdk-4.7.1/enrichsdk/templates/datasets.py.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      315 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/enrich.json.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.459178 enrichsdk-4.7.1/enrichsdk/templates/fixtures/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.531179 enrichsdk-4.7.1/enrichsdk/templates/fixtures/configs/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      419 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/fixtures/configs/1.json
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      421 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/fixtures/configs/2.json
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      854 2022-06-16 09:58:20.000000 enrichsdk-4.7.1/enrichsdk/templates/helloworld.node.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1180 2022-04-26 06:44:46.000000 enrichsdk-4.7.1/enrichsdk/templates/iris.node.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      231 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/manifest.json.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.531179 enrichsdk-4.7.1/enrichsdk/templates/metrics/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    12277 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/metrics/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1266 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/metrics/profilespec.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1248 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/pipelineconf.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1257 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/pipelinepyconf.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.531179 enrichsdk-4.7.1/enrichsdk/templates/prefect/
--rwxrwxr-x   0 pingali   (1000) pingali   (1000)     2693 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/prefect/default.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      916 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/pyscript.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5053 2021-09-21 13:30:07.000000 enrichsdk-4.7.1/enrichsdk/templates/query.node.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      225 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/repo.init.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       70 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/root.README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      286 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/root.enrich.json.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2599 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/rscript.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       22 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/setup.cfg.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      623 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/setup.py.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4378 2023-01-26 11:14:36.000000 enrichsdk-4.7.1/enrichsdk/templates/simpletransform.node.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3328 2023-02-07 03:49:08.000000 enrichsdk-4.7.1/enrichsdk/templates/singlepageapp.py.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.531179 enrichsdk-4.7.1/enrichsdk/templates/spark/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2273 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/spark/README.md
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.531179 enrichsdk-4.7.1/enrichsdk/templates/spark/configs/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       27 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/spark/configs/etl_config.json
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.531179 enrichsdk-4.7.1/enrichsdk/templates/spark/dependencies/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/spark/dependencies/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1444 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/spark/dependencies/enrich.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1267 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/spark/dependencies/logging.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4288 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/spark/dependencies/spark.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.535179 enrichsdk-4.7.1/enrichsdk/templates/spark/jobs/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3468 2022-12-08 14:18:41.000000 enrichsdk-4.7.1/enrichsdk/templates/spark/jobs/run_spark.py
--rwxrwxr-x   0 pingali   (1000) pingali   (1000)     1287 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/spark/run.sh
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      682 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/taskconf.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1921 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/tasklib.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2172 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/test_module.py.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7964 2022-06-27 05:08:43.000000 enrichsdk-4.7.1/enrichsdk/templates/transform.node.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.535179 enrichsdk-4.7.1/enrichsdk/templates/widgets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3056 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/barchart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1101 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/chart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       28 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/footer.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      384 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/fullpanel.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      139 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/gridelement.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       95 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/header.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1561 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/heatmap.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      548 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/hero.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1830 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/linechart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      373 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/mediumpanel.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      219 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/multicolumn_list.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       74 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/nextrow.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       70 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/sectionfooter.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      111 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/sectionheader.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      312 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/shortpanel.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      436 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/table.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       54 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/text.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      466 2021-09-12 13:54:25.000000 enrichsdk-4.7.1/enrichsdk/templates/widgets/trophy.html
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.539179 enrichsdk-4.7.1/enrichsdk/utils/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4402 2023-03-27 07:17:21.000000 enrichsdk-4.7.1/enrichsdk/utils/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3002 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/utils/excel.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6555 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/utils/redis.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1294 2022-12-08 14:18:42.000000 enrichsdk-4.7.1/enrichsdk/utils/sample.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-10 14:58:57.463178 enrichsdk-4.7.1/enrichsdk.egg-info/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3298 2023-04-10 14:58:57.000000 enrichsdk-4.7.1/enrichsdk.egg-info/PKG-INFO
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10897 2023-04-10 14:58:57.000000 enrichsdk-4.7.1/enrichsdk.egg-info/SOURCES.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        1 2023-04-10 14:58:57.000000 enrichsdk-4.7.1/enrichsdk.egg-info/dependency_links.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       64 2023-04-10 14:58:57.000000 enrichsdk-4.7.1/enrichsdk.egg-info/entry_points.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        1 2021-09-12 14:22:47.000000 enrichsdk-4.7.1/enrichsdk.egg-info/not-zip-safe
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      953 2023-04-10 14:58:57.000000 enrichsdk-4.7.1/enrichsdk.egg-info/requires.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       10 2023-04-10 14:58:57.000000 enrichsdk-4.7.1/enrichsdk.egg-info/top_level.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1391 2023-03-08 02:41:34.000000 enrichsdk-4.7.1/requirements.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      116 2023-04-10 14:58:57.539179 enrichsdk-4.7.1/setup.cfg
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3013 2023-04-10 12:30:17.000000 enrichsdk-4.7.1/setup.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      806 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/LICENSE
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      203 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/MANIFEST.in
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3298 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/PKG-INFO
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2182 2023-01-17 09:28:06.000000 enrichsdk-4.7.2/README.rst
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1676 2023-04-13 06:33:53.000000 enrichsdk-4.7.2/enrichsdk/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/api/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6446 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/api/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6001 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/api/draw.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/app/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       35 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/app/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/app/bases/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      369 2023-01-10 11:58:12.000000 enrichsdk-4.7.2/enrichsdk/app/bases/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      183 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      456 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/forms.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2875 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/models.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.087734 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.087734 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     9438 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_add.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    17335 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    19428 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       92 2022-11-14 13:05:48.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns_helper.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14153 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_dataset.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3129 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_detail.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14043 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    16391 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/workflow_index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    31979 2023-02-27 08:21:08.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/views.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.087734 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.087734 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      272 2023-02-17 05:17:51.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      300 2023-04-13 04:01:12.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button_function.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      212 2023-03-10 06:57:41.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_icon.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      389 2023-04-05 10:39:21.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_search.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1091 2023-02-17 05:17:51.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      694 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      771 2023-02-17 05:17:51.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2475 2023-02-17 05:17:51.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6992 2023-04-15 03:35:02.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3730 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4104 2023-04-14 03:48:35.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1387 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1591 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_key_value_pairs.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4433 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_linechart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7312 2023-04-13 05:31:25.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8014 2023-03-10 06:57:41.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_filters.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7251 2023-03-10 06:57:41.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_search.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3137 2023-04-13 13:27:08.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_text.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2980 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_widget_with_config.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      214 2023-01-17 09:28:06.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/help.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3417 2023-02-17 05:17:51.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/share.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1529 2023-01-17 08:20:08.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/sidebar_menu_icon.html
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      183 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      130 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/forms.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/models.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.087734 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/templates/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.087734 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/templates/enrichapp/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2324 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/generic.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      119 2022-11-23 04:27:41.000000 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/helper.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2224 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10036 2023-04-13 18:17:15.000000 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/views.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3186 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/app/utils.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/app/widget/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/app/widget/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      635 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/app/widget/basewidget.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5121 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/app/widget/customcomponent.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3327 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/app/widget/customwidget.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/commands/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      176 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/commands/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    11330 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/commands/config.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1431 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/commands/decorators.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3025 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/commands/helper.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2232 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/commands/log.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6436 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/commands/run.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       45 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       82 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      227 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    25017 2023-02-14 06:43:41.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/anonymizer.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7017 2023-02-07 10:54:16.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/changepoints.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5845 2023-01-10 09:26:26.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/llmtextgen.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7224 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/profilespec.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-16 05:19:04.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/syndata.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3068 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/timeseries_forecasting.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2717 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/catalog.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    26236 2023-01-03 13:19:44.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/logprocessor.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      747 2023-04-05 10:39:21.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/anomalies/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    33176 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/anomalies/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/changepoints/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    33192 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/changepoints/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/classifier/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    33641 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/classifier/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/data_quality/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    18378 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/data_quality/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/feature_compute/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4667 2023-04-04 16:04:30.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/feature_compute/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/filebased_query_executor/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1615 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/filebased_query_executor/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    29587 2023-04-04 16:04:30.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/filebased_query_executor/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1743 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/filebased_query_executor/lib.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/fileops/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      238 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/fileops/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5046 2023-04-04 16:04:30.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/fileops/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/inmemory_query_executor/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    23726 2023-04-04 16:04:30.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/inmemory_query_executor/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/metrics/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    17600 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/metrics/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/notebook_executor/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      946 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/notebook_executor/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5391 2023-04-04 16:04:30.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/notebook_executor/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/observability/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    33314 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/observability/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/synthetic_data_generator/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    26037 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/synthetic_data_generator/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/timeseries_forecaster/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    25318 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/timeseries_forecaster/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/transforms/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      391 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/transforms/fileops/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      769 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/fileops/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2309 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/fileops/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsink/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      452 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsink/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7845 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsink/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsource/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      514 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsource/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5451 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsource/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/contrib/transforms/pqexport/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      909 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/pqexport/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     9384 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/pqexport/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/contrib/transforms/sqlexport/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1450 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/sqlexport/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14007 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/sqlexport/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesink/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1187 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesink/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     9446 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesink/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesource/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1581 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesource/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8317 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesource/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/core/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      909 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/core/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3428 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/core/frames.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    41276 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/core/mixins.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    52640 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/core/node.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3691 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/core/patch.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7222 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/core/render.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1292 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/core/res.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    32053 2023-04-05 10:39:21.000000 enrichsdk-4.7.2/enrichsdk/core/run.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14634 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/core/sdk.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6898 2023-03-09 06:57:39.000000 enrichsdk-4.7.2/enrichsdk/core/state.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1294 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/core/widgets.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/datasets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      552 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/datasets/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    36181 2023-02-21 05:43:43.000000 enrichsdk-4.7.2/enrichsdk/datasets/discover.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    18149 2023-03-01 13:54:44.000000 enrichsdk-4.7.2/enrichsdk/datasets/doodle.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1389 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/datasets/generators.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/extractors/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1703 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/extractors/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/feature_compute/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    13231 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/feature_compute/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/featurestore/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4502 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/featurestore/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10432 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/featurestore/schema.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/lib/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    23696 2023-04-13 03:39:51.000000 enrichsdk-4.7.2/enrichsdk/lib/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4945 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/lib/context.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5827 2023-02-26 08:39:33.000000 enrichsdk-4.7.2/enrichsdk/lib/customer.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2069 2023-03-09 06:57:39.000000 enrichsdk-4.7.2/enrichsdk/lib/exceptions.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2903 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/lib/integration.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      983 2023-01-10 09:26:26.000000 enrichsdk-4.7.2/enrichsdk/lib/misc.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      552 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/lib/permissions.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1212 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/lib/renderlib.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1357 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/lib/resources.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/notebook/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8611 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/notebook/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      189 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/notebook/utils.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/package/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    86072 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/package/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4194 2023-02-01 09:43:30.000000 enrichsdk-4.7.2/enrichsdk/package/lib.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1629 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/package/log.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14964 2023-01-03 13:19:44.000000 enrichsdk-4.7.2/enrichsdk/package/misc.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    23959 2023-03-09 06:57:39.000000 enrichsdk-4.7.2/enrichsdk/package/mock.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4322 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/package/validators.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/policy/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7529 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/policy/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1608 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/policy/sdk.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/quality/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2476 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/quality/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5666 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/quality/base.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      925 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/quality/exceptions.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4371 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/quality/expectations.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5157 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/quality/reconciliation.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4884 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/quality/transforms.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/realtime/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      283 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/realtime/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2401 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/realtime/db.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      824 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/realtime/log.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5122 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/realtime/messaging.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4056 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/realtime/spark.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4869 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/realtime/transforms.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3173 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/realtime/workflow.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/render/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10751 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/render/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/scripts/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/scripts/__init__.py
+-rwxrwxr-x   0 pingali   (1000) pingali   (1000)     4372 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/scripts/enrichcmd.py
+-rwxrwxr-x   0 pingali   (1000) pingali   (1000)    44398 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/scripts/enrichpkg.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/services/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1800 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/services/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/tasks/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10443 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/tasks/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/tasks/dummy_task/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1839 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/tasks/dummy_task/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8046 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/tasks/sdk.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/templates/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       42 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/LICENSE.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       27 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/MANIFEST.in.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      370 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/README.md.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      383 2023-01-02 14:59:19.000000 enrichsdk-4.7.2/enrichsdk/templates/README_PIPELINE.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       53 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/README_TASK.md
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/templates/airflow/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1476 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/airflow/contrib-pipeline-v1.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/templates/appstore2.0/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3669 2023-01-17 08:20:08.000000 enrichsdk-4.7.2/enrichsdk/templates/appstore2.0/index.html.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/templates/assets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4444 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/assets/datasets.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1340 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/config.json.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/dashboard/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      180 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      384 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/apps.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      189 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/catalog.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      235 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/custom.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3455 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/persona.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      685 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/tasks.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/dashboard/templates/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5168 2021-09-14 02:19:33.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/templates/complex_result.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2405 2022-03-28 06:32:35.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/templates/index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1273 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/urls.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4684 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/views.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/datasets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      311 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/datasets/manifest.json.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5999 2022-08-02 10:38:39.000000 enrichsdk-4.7.2/enrichsdk/templates/datasets.py.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      315 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/enrich.json.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.087734 enrichsdk-4.7.2/enrichsdk/templates/fixtures/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/fixtures/configs/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      419 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/fixtures/configs/1.json
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      421 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/fixtures/configs/2.json
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      854 2022-06-16 09:58:20.000000 enrichsdk-4.7.2/enrichsdk/templates/helloworld.node.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1180 2022-04-26 06:44:46.000000 enrichsdk-4.7.2/enrichsdk/templates/iris.node.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      231 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/manifest.json.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/metrics/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    12277 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/metrics/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1266 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/metrics/profilespec.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1248 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/pipelineconf.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1257 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/pipelinepyconf.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/prefect/
+-rwxrwxr-x   0 pingali   (1000) pingali   (1000)     2693 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/prefect/default.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      916 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/pyscript.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5053 2021-09-21 13:30:07.000000 enrichsdk-4.7.2/enrichsdk/templates/query.node.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      225 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/repo.init.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       70 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/root.README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      286 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/root.enrich.json.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2599 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/rscript.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       22 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/setup.cfg.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      623 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/setup.py.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4378 2023-01-26 11:14:36.000000 enrichsdk-4.7.2/enrichsdk/templates/simpletransform.node.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3328 2023-02-07 03:49:08.000000 enrichsdk-4.7.2/enrichsdk/templates/singlepageapp.py.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/spark/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2273 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/spark/README.md
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/spark/configs/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       27 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/spark/configs/etl_config.json
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/spark/dependencies/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/spark/dependencies/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1444 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/spark/dependencies/enrich.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1267 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/spark/dependencies/logging.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4288 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/spark/dependencies/spark.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/spark/jobs/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3468 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/spark/jobs/run_spark.py
+-rwxrwxr-x   0 pingali   (1000) pingali   (1000)     1287 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/spark/run.sh
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      682 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/taskconf.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1921 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/tasklib.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2172 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/test_module.py.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7964 2022-06-27 05:08:43.000000 enrichsdk-4.7.2/enrichsdk/templates/transform.node.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/widgets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3056 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/barchart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1101 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/chart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       28 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/footer.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      384 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/fullpanel.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      139 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/gridelement.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       95 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/header.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1561 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/heatmap.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      548 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/hero.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1830 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/linechart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      373 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/mediumpanel.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      219 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/multicolumn_list.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       74 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/nextrow.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       70 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/sectionfooter.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      111 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/sectionheader.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      312 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/shortpanel.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      436 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/table.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       54 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/text.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      466 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/trophy.html
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/utils/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4402 2023-03-27 07:17:21.000000 enrichsdk-4.7.2/enrichsdk/utils/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3002 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/utils/excel.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6555 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/utils/redis.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1294 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/utils/sample.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk.egg-info/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3298 2023-04-17 03:51:58.000000 enrichsdk-4.7.2/enrichsdk.egg-info/PKG-INFO
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10897 2023-04-17 03:51:59.000000 enrichsdk-4.7.2/enrichsdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        1 2023-04-17 03:51:58.000000 enrichsdk-4.7.2/enrichsdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       64 2023-04-17 03:51:58.000000 enrichsdk-4.7.2/enrichsdk.egg-info/entry_points.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        1 2021-09-12 14:22:47.000000 enrichsdk-4.7.2/enrichsdk.egg-info/not-zip-safe
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      953 2023-04-17 03:51:58.000000 enrichsdk-4.7.2/enrichsdk.egg-info/requires.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       10 2023-04-17 03:51:58.000000 enrichsdk-4.7.2/enrichsdk.egg-info/top_level.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1391 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/requirements.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      116 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/setup.cfg
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3013 2023-04-13 06:33:53.000000 enrichsdk-4.7.2/setup.py
```

### Comparing `enrichsdk-4.7.1/LICENSE` & `enrichsdk-4.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/PKG-INFO` & `enrichsdk-4.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: enrichsdk
-Version: 4.7.1
+Version: 4.7.2
 Summary: Enrich Developer Kit
 Home-page: http://github.com/pingali/scribble-enrichsdk
 Author: Venkata Pingali
 Author-email: pingali@scribbledata.io
 License: All rights reserved
 Description: ==========
         Enrich SDK
```

### Comparing `enrichsdk-4.7.1/README.rst` & `enrichsdk-4.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/__init__.py` & `enrichsdk-4.7.2/enrichsdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 |_____|_| |_|_|  |_|\___|_| |_| |____/|____/|_|\_\
 
 </pre>
 
 """
 import os
 
-VERSION = "4.7.1"
+VERSION = "4.7.2"
 
 
 def _get_git_revision(path):
     revision_file = os.path.join(path, "refs", "heads", "master")
     if os.path.exists(revision_file):
         with open(revision_file) as fh:
             return fh.read().strip()[:7]
```

### Comparing `enrichsdk-4.7.1/enrichsdk/api/__init__.py` & `enrichsdk-4.7.2/enrichsdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/api/draw.py` & `enrichsdk-4.7.2/enrichsdk/api/draw.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/models.py` & `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/models.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_add.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_add.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_index.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_dataset.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_dataset.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_detail.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_detail.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_index.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/workflow_index.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/workflow_index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/policyapp/views.py` & `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/views.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 {% block breadcrumbs %}
 <div id="address_content" style="display: none">
     <ol class="breadcrumb mb-0" aria-label="breadcrumb">
       <li class="breadcrumb-item"><a href="{% url 'dashboard:home' %}">Enrich</a></li>
       <li class="breadcrumb-item"><a href="{% url 'dashboard:index' %}">Usecases</a></li>
       <li class="breadcrumb-item"><a href="{% url 'dashboard:usecase_detail' usecase.org.name %}">{{usecase.org.name}}</a></li>
       <li class="breadcrumb-item active"><a href="{% url basenamespace|add:':index' %}">{{spec.name}}</a></li>
+      {% if data.breadcrumb %}
+      <li class="breadcrumb-item active">{{data.breadcrumb}}</a></li>
+      {% endif %}
     </ol>
 </div>
 {% with tags=spec.tags|join:" " %}
 {% with knowledge=spec.name|add:' '|add:tags %}{{ block.super }}{% endwith %}
 {% endwith %}
 {% endblock breadcrumbs %}
 <!-- ============================= Address Bar End =============================== -->
@@ -96,15 +99,19 @@
               <img src="{% static 'gui2/appstore2/images/'|add:spec.icon|add:'.svg' %}" alt="" />
               {% else %}
               <img src="{% static 'gui2/appstore2/images/placholder.jpg' %}" alt="" />
               {% endif %}
             </div>
             <div class="hcb-text-box">
               <h3>{% translate  spec.name %} {% translate data.title %}</h3>
+	      {% if "description" in data %}
+	      <p> {% translate data.description %}</p>
+	      {% else %}
               <p> {% translate spec.description %}</p>
+	      {% endif %}
               {% include 'dashboard/_appusers.html' with usecase=usecase spec=spec %}
             </div>
           </div>
           <div class="hcb-right ms-auto">
           <form class="uniForm"  method="GET">
           <ul class="v-line-text-list d-flex flex-wrap">
               {% for k,values in data.header.components.items %}
@@ -161,19 +168,22 @@
                   </li>
                   {% endfor %}
                 </ul>
               </div>
             </div>
           </div>
           <div class="block-content padding-24">
-{#            {% if target == default_target %}#}
-                {% for widget in data.widgets %}
-                    {% include 'sharedapp/partials/'|add:widget.type|add:'.html' with usecase=usecase spec=spec widget=widget %}
-                {% endfor %}
-{#            {% endif %}#}
+            {% for widget in data.widgets %}
+	    {% if 'dict' in widget|get_type %}
+            {% include 'sharedapp/partials/'|add:widget.type|add:'.html' with usecase=usecase spec=spec widget=widget %}
+	    {% else %}
+	    {{widget|safe}}
+	    {% endif %}
+            {% endfor %}
+
           </div>
         </div>
       </div>
     </div>
   </div>
 </div>
```

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,26 @@
 {% load staticfiles %}
 {% load i18n %}
+{% load fontawesome %}
+
+<style>
+  .spinner-border{
+      width: 4.375rem;
+      height: 4.375rem;
+      position: fixed;
+      z-index: 999;
+      overflow: show;
+      margin: auto;
+      top: 0;
+      left: 0;
+      bottom: 0;
+      right: 0;
+      display: none;
+  }
+</style>
 
 <!--
 Jinja2 partial to render a form
 
 { % include 'sharedapp/partials/full_width_form.html' with usecase=usecase spec=spec widget=widget % }
 
 -->
@@ -26,17 +43,17 @@
     <div class="block-filter-option ms-auto d-flex align-items-center justify-content-center align-block-filter-option">
     </div>
   </div>
   <div id="collapseresults" class="crc-body accordion-collapse collapse show">
     <div class="cp-body">
       <div class="row mb-30">
 	{% if widget.method %}
-	<form class="uniForm"  method="{{widget.method}}">
+	<form class="uniForm"  method="{{widget.method}}" id="form{{widget.id}}">
         {% else %}
-	<form class="uniForm"  method="GET">
+	<form class="uniForm"  method="GET" id="form{{widget.id}}">
         {% endif %}
 	  {% if widget.method == "POST" %}
 	  {% csrf_token %}
 	  {% endif %}
 	  {% for name, value in widget.hidden_vars.items %}
 	  <input name="{{name}}" value="{{value}}" type="hidden"></input>
 	  {% endfor %}
@@ -64,22 +81,32 @@
                 <div class="form-group" id="single-text-{{widget.id}}">
                   <input type="text" class="form-control" id="{{element.name}}" name="{{element.name}}" value="{{element.value}}" placeholder="{{element.placeholder}}" required >
                 </div>
               </div>
             </div>
 	    {% endif %}
 	    {% endfor %}
-          <div class="v-box p-2 mt-3">
+            <div class="v-box p-2 mt-3">
               <div class="column">
-            <div class="form-group d-flex">
-              <button name="submit" id="submit" value="show" type="submit" class="btn btn-default" data-toggle="tooltip" data-placement="bottom" title="Search"><img src="{% static 'gui2/appstore2/images/play.svg' %}" alt="" />{% if 'submit' in widget %}{{widget.submit}}{% else %}Show{% endif %}</button>
-            </div>
+		<div class="form-group d-flex" id="formsubmitdiv">
+		  <button name="submit" id="submit" value="show" type="submit" class="btn btn-default" data-toggle="tooltip" data-placement="bottom"><img src="{% static 'gui2/appstore2/images/play.svg' %}" alt="" />{% if 'submit' in widget %}{{widget.submit}}{% else %}Show{% endif %}</button>
+		  <div class="spinner-border" role="status" id="spinner">
+		  </div>
+		</div>
               </div>
-          </div>
           </ul>
 	</form>
       </div>
     </div>
   </div>
 </div>
 
 
+{% if widget.spinner_on_submit %}
+  <script>
+    $('#form{{widget.id}}').submit(function() {
+	$("#spinner").show();
+    });
+
+</script>
+
+{% endif %}
```

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_key_value_pairs.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_key_value_pairs.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_linechart.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_linechart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_filters.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_filters.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_search.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_search.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_text.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_text.html`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 <!--
 Jinja2 partial to render an image
 
 { % include 'sharedapp/partials/full_width_text.html' with usecase=usecase spec=spec widget=widget % }
 
 -->
-<div class="block-widget-box width-all" id="{{widget.id}}">
+<div class="block-widget-box width-all mb-3" id="{{widget.id}}">
   <div class="block-filter-container d-flex flex-wrap align-items-center">
     <div class="crc-head-inside d-flex align-items-center">
       <div class="crc-head-icon"  data-bs-toggle="collapse" data-bs-target="#collapseresults_{{widget.id}}" aria-expanded="true">
         <img class="expand-open" src={% static 'gui2/appstore2/images/new-caret-icon-1.svg' %} alt="" />
         <img class="expand-add" src={% static 'gui2/appstore2/images/expand-add.svg' %} alt="" />
       </div>
       <div class="accor-right">
@@ -19,15 +19,20 @@
           <ul class="cp-text-list d-flex align-items-center">
             <li><b>{% translate widget.name %}</b></li>
           </ul>
             <p>{% translate widget.description %}</p>
         </div>
       </div>
     </div>
-    <div class="block-filter-option ms-auto d-flex align-items-center justify-content-center align-block-filter-option">
+    <div class="block-filter-option ms-auto d-flex align-items-center justify-content-end align-block-filter-option">
+      {% for k,values in widget.header_components.items %}
+      {% for v in  values %}
+      {% include 'sharedapp/components/'|add:v.template|add:'.html' with content=v widget=widget %}
+      {% endfor %}
+      {% endfor %}
     </div>
   </div>
   <div id="collapseresults_{{widget.id}}" class="crc-body accordion-collapse collapse show">
     <div class="cp-body">
 
     {% if widget.text %}
       <p>{{widget.text|safe}}</p>
```

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_widget_with_config.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_widget_with_config.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/share.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/share.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/sidebar_menu_icon.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/sidebar_menu_icon.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/generic.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/generic.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/index.html` & `enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/bases/singlepageapp/views.py` & `enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     def __str__(self):
         return f"[{self.name}] {self.verbose_name}"
 
     def get_readme(self):
         return """This is a generic single page app"""
 
     def get_template(self, spec, name):
-        return spec.get('templates',{}).get(name, self.templates[name])
+        return spec.get('templates',{}).get(name, self.templates.get(name, "Unable to find template"))
 
     def get_model(self, spec, name):
 
         from enrichapp.dashboard.globalapp import lib as globallib
 
         if (('models' in spec) and (name in spec['models'])):
             return spec['models'][name]
```

### Comparing `enrichsdk-4.7.1/enrichsdk/app/utils.py` & `enrichsdk-4.7.2/enrichsdk/app/utils.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/widget/basewidget.py` & `enrichsdk-4.7.2/enrichsdk/app/widget/basewidget.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/widget/customcomponent.py` & `enrichsdk-4.7.2/enrichsdk/app/widget/customcomponent.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/app/widget/customwidget.py` & `enrichsdk-4.7.2/enrichsdk/app/widget/customwidget.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/commands/config.py` & `enrichsdk-4.7.2/enrichsdk/commands/config.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/commands/decorators.py` & `enrichsdk-4.7.2/enrichsdk/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/commands/helper.py` & `enrichsdk-4.7.2/enrichsdk/commands/helper.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/commands/log.py` & `enrichsdk-4.7.2/enrichsdk/commands/log.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/commands/run.py` & `enrichsdk-4.7.2/enrichsdk/commands/run.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/assets/anonymizer.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/anonymizer.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/assets/changepoints.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/changepoints.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/assets/llmtextgen.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/llmtextgen.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/assets/profilespec.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/profilespec.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/assets/timeseries_forecasting.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/timeseries_forecasting.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/catalog.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/catalog.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/logprocessor.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/logprocessor.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/anomalies/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/anomalies/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/changepoints/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/changepoints/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/classifier/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/classifier/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/data_quality/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/data_quality/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/feature_compute/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/feature_compute/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/filebased_query_executor/README.md` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/filebased_query_executor/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/filebased_query_executor/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/filebased_query_executor/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/filebased_query_executor/lib.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/filebased_query_executor/lib.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/fileops/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/fileops/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/inmemory_query_executor/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/inmemory_query_executor/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/metrics/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/notebook_executor/README.md` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/notebook_executor/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/notebook_executor/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/notebook_executor/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/observability/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/observability/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/synthetic_data_generator/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/synthetic_data_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/lib/transforms/timeseries_forecaster/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/timeseries_forecaster/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/transforms/fileops/README.md` & `enrichsdk-4.7.2/enrichsdk/contrib/transforms/fileops/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/transforms/fileops/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/transforms/fileops/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/transforms/jsonsink/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsink/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/transforms/jsonsource/README.md` & `enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsource/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/transforms/jsonsource/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsource/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/transforms/pqexport/README.md` & `enrichsdk-4.7.2/enrichsdk/contrib/transforms/pqexport/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/transforms/pqexport/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/transforms/pqexport/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/transforms/sqlexport/README.md` & `enrichsdk-4.7.2/enrichsdk/contrib/transforms/sqlexport/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/transforms/sqlexport/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/transforms/sqlexport/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/transforms/tablesink/README.md` & `enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesink/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/transforms/tablesink/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesink/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/transforms/tablesource/README.md` & `enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesource/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/contrib/transforms/tablesource/__init__.py` & `enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesource/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/core/__init__.py` & `enrichsdk-4.7.2/enrichsdk/core/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/core/frames.py` & `enrichsdk-4.7.2/enrichsdk/core/frames.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/core/mixins.py` & `enrichsdk-4.7.2/enrichsdk/core/mixins.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/core/node.py` & `enrichsdk-4.7.2/enrichsdk/core/node.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/core/patch.py` & `enrichsdk-4.7.2/enrichsdk/core/patch.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/core/render.py` & `enrichsdk-4.7.2/enrichsdk/core/render.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/core/res.py` & `enrichsdk-4.7.2/enrichsdk/core/res.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/core/run.py` & `enrichsdk-4.7.2/enrichsdk/core/run.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/core/sdk.py` & `enrichsdk-4.7.2/enrichsdk/core/sdk.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/core/state.py` & `enrichsdk-4.7.2/enrichsdk/core/state.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/core/widgets.py` & `enrichsdk-4.7.2/enrichsdk/core/widgets.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/datasets/__init__.py` & `enrichsdk-4.7.2/enrichsdk/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/datasets/discover.py` & `enrichsdk-4.7.2/enrichsdk/datasets/discover.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/datasets/doodle.py` & `enrichsdk-4.7.2/enrichsdk/datasets/doodle.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/datasets/generators.py` & `enrichsdk-4.7.2/enrichsdk/datasets/generators.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/extractors/__init__.py` & `enrichsdk-4.7.2/enrichsdk/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/feature_compute/__init__.py` & `enrichsdk-4.7.2/enrichsdk/feature_compute/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/featurestore/__init__.py` & `enrichsdk-4.7.2/enrichsdk/featurestore/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/featurestore/schema.py` & `enrichsdk-4.7.2/enrichsdk/featurestore/schema.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/lib/__init__.py` & `enrichsdk-4.7.2/enrichsdk/lib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         cached_siteconf[filename] = siteconf
         if nature == "open":
             logger.warning("Successfully read siteconf but it is insecure")
         else:
             logger.warning("Successfully read secure siteconf")
     except:
         # sitelib may not be installed
-        logger.debug("Could not read secure siteconf. Falling back")
+        # logger.debug("Could not read secure siteconf. Falling back")
         try:
             # If this is a jsonx file, then try the json version of
             # the file.
             if filename.endswith("jsonx"):
                 filename = filename.replace("jsonx", "json")
             siteconf = json.load(open(filename))
             cached_siteconf[filename] = siteconf
```

### Comparing `enrichsdk-4.7.1/enrichsdk/lib/context.py` & `enrichsdk-4.7.2/enrichsdk/lib/context.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/lib/customer.py` & `enrichsdk-4.7.2/enrichsdk/lib/customer.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/lib/exceptions.py` & `enrichsdk-4.7.2/enrichsdk/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/lib/integration.py` & `enrichsdk-4.7.2/enrichsdk/lib/integration.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/lib/misc.py` & `enrichsdk-4.7.2/enrichsdk/lib/misc.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/lib/permissions.py` & `enrichsdk-4.7.2/enrichsdk/lib/permissions.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/lib/renderlib.py` & `enrichsdk-4.7.2/enrichsdk/lib/renderlib.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/lib/resources.py` & `enrichsdk-4.7.2/enrichsdk/lib/resources.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/notebook/__init__.py` & `enrichsdk-4.7.2/enrichsdk/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/package/__init__.py` & `enrichsdk-4.7.2/enrichsdk/package/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/package/lib.py` & `enrichsdk-4.7.2/enrichsdk/package/lib.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/package/log.py` & `enrichsdk-4.7.2/enrichsdk/package/log.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/package/misc.py` & `enrichsdk-4.7.2/enrichsdk/package/misc.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/package/mock.py` & `enrichsdk-4.7.2/enrichsdk/package/mock.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/package/validators.py` & `enrichsdk-4.7.2/enrichsdk/package/validators.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/policy/__init__.py` & `enrichsdk-4.7.2/enrichsdk/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/policy/sdk.py` & `enrichsdk-4.7.2/enrichsdk/policy/sdk.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/quality/__init__.py` & `enrichsdk-4.7.2/enrichsdk/quality/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/quality/base.py` & `enrichsdk-4.7.2/enrichsdk/quality/base.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/quality/exceptions.py` & `enrichsdk-4.7.2/enrichsdk/quality/exceptions.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/quality/expectations.py` & `enrichsdk-4.7.2/enrichsdk/quality/expectations.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/quality/reconciliation.py` & `enrichsdk-4.7.2/enrichsdk/quality/reconciliation.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/quality/transforms.py` & `enrichsdk-4.7.2/enrichsdk/quality/transforms.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/realtime/db.py` & `enrichsdk-4.7.2/enrichsdk/realtime/db.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/realtime/log.py` & `enrichsdk-4.7.2/enrichsdk/realtime/log.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/realtime/messaging.py` & `enrichsdk-4.7.2/enrichsdk/realtime/messaging.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/realtime/spark.py` & `enrichsdk-4.7.2/enrichsdk/realtime/spark.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/realtime/transforms.py` & `enrichsdk-4.7.2/enrichsdk/realtime/transforms.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/realtime/workflow.py` & `enrichsdk-4.7.2/enrichsdk/realtime/workflow.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/render/__init__.py` & `enrichsdk-4.7.2/enrichsdk/render/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/scripts/enrichcmd.py` & `enrichsdk-4.7.2/enrichsdk/scripts/enrichcmd.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/scripts/enrichpkg.py` & `enrichsdk-4.7.2/enrichsdk/scripts/enrichpkg.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/services/__init__.py` & `enrichsdk-4.7.2/enrichsdk/services/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/tasks/__init__.py` & `enrichsdk-4.7.2/enrichsdk/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/tasks/dummy_task/__init__.py` & `enrichsdk-4.7.2/enrichsdk/tasks/dummy_task/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/tasks/sdk.py` & `enrichsdk-4.7.2/enrichsdk/tasks/sdk.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/airflow/contrib-pipeline-v1.py` & `enrichsdk-4.7.2/enrichsdk/templates/airflow/contrib-pipeline-v1.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/appstore2.0/index.html.template` & `enrichsdk-4.7.2/enrichsdk/templates/appstore2.0/index.html.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/assets/datasets.py` & `enrichsdk-4.7.2/enrichsdk/templates/assets/datasets.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/config.json.template` & `enrichsdk-4.7.2/enrichsdk/templates/config.json.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/dashboard/persona.py` & `enrichsdk-4.7.2/enrichsdk/templates/dashboard/persona.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/dashboard/tasks.py` & `enrichsdk-4.7.2/enrichsdk/templates/dashboard/tasks.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/dashboard/templates/complex_result.html` & `enrichsdk-4.7.2/enrichsdk/templates/dashboard/templates/complex_result.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/dashboard/templates/index.html` & `enrichsdk-4.7.2/enrichsdk/templates/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/dashboard/urls.py` & `enrichsdk-4.7.2/enrichsdk/templates/dashboard/urls.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/dashboard/views.py` & `enrichsdk-4.7.2/enrichsdk/templates/dashboard/views.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/datasets.py.template` & `enrichsdk-4.7.2/enrichsdk/templates/datasets.py.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/helloworld.node.template` & `enrichsdk-4.7.2/enrichsdk/templates/helloworld.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/iris.node.template` & `enrichsdk-4.7.2/enrichsdk/templates/iris.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/metrics/__init__.py` & `enrichsdk-4.7.2/enrichsdk/templates/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/metrics/profilespec.py` & `enrichsdk-4.7.2/enrichsdk/templates/metrics/profilespec.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/pipelineconf.template` & `enrichsdk-4.7.2/enrichsdk/templates/pipelineconf.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/pipelinepyconf.template` & `enrichsdk-4.7.2/enrichsdk/templates/pipelinepyconf.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/prefect/default.py` & `enrichsdk-4.7.2/enrichsdk/templates/prefect/default.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/pyscript.template` & `enrichsdk-4.7.2/enrichsdk/templates/pyscript.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/query.node.template` & `enrichsdk-4.7.2/enrichsdk/templates/query.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/rscript.template` & `enrichsdk-4.7.2/enrichsdk/templates/rscript.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/setup.py.template` & `enrichsdk-4.7.2/enrichsdk/templates/setup.py.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/simpletransform.node.template` & `enrichsdk-4.7.2/enrichsdk/templates/simpletransform.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/singlepageapp.py.template` & `enrichsdk-4.7.2/enrichsdk/templates/singlepageapp.py.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/spark/README.md` & `enrichsdk-4.7.2/enrichsdk/templates/spark/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/spark/dependencies/enrich.py` & `enrichsdk-4.7.2/enrichsdk/templates/spark/dependencies/enrich.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/spark/dependencies/logging.py` & `enrichsdk-4.7.2/enrichsdk/templates/spark/dependencies/logging.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/spark/dependencies/spark.py` & `enrichsdk-4.7.2/enrichsdk/templates/spark/dependencies/spark.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/spark/jobs/run_spark.py` & `enrichsdk-4.7.2/enrichsdk/templates/spark/jobs/run_spark.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/spark/run.sh` & `enrichsdk-4.7.2/enrichsdk/templates/spark/run.sh`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/taskconf.template` & `enrichsdk-4.7.2/enrichsdk/templates/taskconf.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/tasklib.template` & `enrichsdk-4.7.2/enrichsdk/templates/tasklib.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/test_module.py.template` & `enrichsdk-4.7.2/enrichsdk/templates/test_module.py.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/transform.node.template` & `enrichsdk-4.7.2/enrichsdk/templates/transform.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/widgets/barchart.html` & `enrichsdk-4.7.2/enrichsdk/templates/widgets/barchart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/widgets/chart.html` & `enrichsdk-4.7.2/enrichsdk/templates/widgets/chart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/widgets/heatmap.html` & `enrichsdk-4.7.2/enrichsdk/templates/widgets/heatmap.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/widgets/hero.html` & `enrichsdk-4.7.2/enrichsdk/templates/widgets/hero.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/templates/widgets/linechart.html` & `enrichsdk-4.7.2/enrichsdk/templates/widgets/linechart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/utils/__init__.py` & `enrichsdk-4.7.2/enrichsdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/utils/excel.py` & `enrichsdk-4.7.2/enrichsdk/utils/excel.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/utils/redis.py` & `enrichsdk-4.7.2/enrichsdk/utils/redis.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk/utils/sample.py` & `enrichsdk-4.7.2/enrichsdk/utils/sample.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk.egg-info/PKG-INFO` & `enrichsdk-4.7.2/enrichsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: enrichsdk
-Version: 4.7.1
+Version: 4.7.2
 Summary: Enrich Developer Kit
 Home-page: http://github.com/pingali/scribble-enrichsdk
 Author: Venkata Pingali
 Author-email: pingali@scribbledata.io
 License: All rights reserved
 Description: ==========
         Enrich SDK
```

### Comparing `enrichsdk-4.7.1/enrichsdk.egg-info/SOURCES.txt` & `enrichsdk-4.7.2/enrichsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/enrichsdk.egg-info/requires.txt` & `enrichsdk-4.7.2/enrichsdk.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 glob2==0.7
 google-cloud-logging
 great-expectations
 humanize==0.5.1
 idna==2.8
 imblearn==0.0
 jsonschema>=3.2.0
-jupyter-core>=4.7.1
+jupyter-core>=4.7.2
 kafka-python==2.0.2
 logstash_formatter
 nbformat>=5.1.2
 openai
 pandas<1.5,>=1.3.5
 papermill>=2.3.4
 plotly>=4.0.0
@@ -38,15 +38,15 @@
 pyarrow>=0.9.0
 pyfiglet
 pyhive
 pykafka
 pykafka==2.8.0
 pymongo
 pytest-cov
-pytest>=4.7.1
+pytest>=4.7.2
 python-dateutil>=2.8.1
 python-json-logger==0.1.8
 pytz>=2020.1
 raven==6.6.0
 redis
 requests-oauthlib==0.8.0
 requests==2.26.0
```

### Comparing `enrichsdk-4.7.1/requirements.txt` & `enrichsdk-4.7.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.1/setup.py` & `enrichsdk-4.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("enrichsdk/__init__.py", "rb") as f:
     version = str(
         ast.literal_eval(_version_re.search(f.read().decode("utf-8")).group(1))
     )
 
 setup(
     name="enrichsdk",
-    version="4.7.1",
+    version="4.7.2",
     description="Enrich Developer Kit",
     long_description=readme,
     url="http://github.com/pingali/scribble-enrichsdk",
     author="Venkata Pingali",
     author_email="pingali@scribbledata.io",
     license="All rights reserved",
     scripts=[],
@@ -33,15 +33,15 @@
         "wheel",
         "click>=7.1.2",
         "aioitertools==0.8.0",
 
         "glob2==0.7",
         "requests==2.26.0",
         "requests-oauthlib==0.8.0",
-        "pytest>=4.7.1",
+        "pytest>=4.7.2",
         "pandas>=1.3.5,<1.5",
         "distributed==2.30.1",
         "idna==2.8",
         "coverage==5.5",
         "flake8",
         "raven==6.6.0",
         "python-json-logger==0.1.8",
@@ -71,15 +71,15 @@
         "scipy<=1.10.0",
         "seaborn",
         #"flask_cors",
         #'moto>=1.3.14',
         "prefect>=0.15.7,<0.15.11",
         "distro>=1.4.0",
         "gcsfs==0.6.0",
-        "jupyter-core>=4.7.1",
+        "jupyter-core>=4.7.2",
         "nbformat>=5.1.2",
         "tzlocal>=2.0.0",
         "texttable",
         "pykafka",
         "redis",
         "gitpython",
         "logstash_formatter",
```

