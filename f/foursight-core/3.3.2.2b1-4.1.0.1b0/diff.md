# Comparing `tmp/foursight_core-3.3.2.2b1.tar.gz` & `tmp/foursight_core-4.1.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-3.3.2.2b1.tar", max compression
+gzip compressed data, was "foursight_core-4.1.0.1b0.tar", max compression
```

## Comparing `foursight_core-3.3.2.2b1.tar` & `foursight_core-4.1.0.1b0.tar`

### file list

```diff
@@ -1,75 +1,135 @@
--rw-r--r--   0        0        0     1083 2023-03-16 23:10:55.184688 foursight_core-3.3.2.2b1/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/app.py
--rw-r--r--   0        0        0   101502 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/app_utils.py
--rw-r--r--   0        0        0     2571 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     4439 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/decorators.py
--rw-r--r--   0        0        0    15050 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/deploy.py
--rw-r--r--   0        0        0     8302 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/environment.py
--rw-r--r--   0        0        0    11792 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/exceptions.py
--rw-r--r--   0        0        0     4034 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8377 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/package.py
--rw-r--r--   0        0        0    11705 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     6990 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    23203 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3038 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6315 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28316 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20652 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     2921 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     5745 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     5904 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     3257 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9524 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0    71354 2023-03-16 23:10:55.192688 foursight_core-3.3.2.2b1/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    10359 2023-03-16 23:10:55.196688 foursight_core-3.3.2.2b1/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-03-16 23:10:55.196688 foursight_core-3.3.2.2b1/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    30540 2023-03-16 23:10:55.196688 foursight_core-3.3.2.2b1/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4861 2023-03-16 23:10:55.196688 foursight_core-3.3.2.2b1/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-03-16 23:10:55.196688 foursight_core-3.3.2.2b1/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-03-16 23:10:55.196688 foursight_core-3.3.2.2b1/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-03-16 23:10:55.196688 foursight_core-3.3.2.2b1/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-03-16 23:10:55.196688 foursight_core-3.3.2.2b1/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11735 2023-03-16 23:10:55.196688 foursight_core-3.3.2.2b1/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1911785 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/routes.py
--rw-r--r--   0        0        0    22442 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/run_result.py
--rw-r--r--   0        0        0     6330 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     1402 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/scripts/decrypt_accounts_file.py
--rw-r--r--   0        0        0     1406 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/scripts/encrypt_accounts_file.py
--rw-r--r--   0        0        0     5370 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20540 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-03-16 23:10:55.204688 foursight_core-3.3.2.2b1/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1194 2023-03-16 23:10:55.208688 foursight_core-3.3.2.2b1/pyproject.toml
--rw-r--r--   0        0        0     1129 1970-01-01 00:00:00.000000 foursight_core-3.3.2.2b1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-09-07 10:08:59.753994 foursight_core-4.1.0.1b0/LICENSE.txt
+-rw-r--r--   0        0        0    10825 2022-11-20 13:33:58.544911 foursight_core-4.1.0.1b0/foursight_core/'
+-rw-r--r--   0        0        0        0 2022-09-07 10:08:59.760120 foursight_core-4.1.0.1b0/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-03-30 11:22:44.920863 foursight_core-4.1.0.1b0/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0     8523 2023-02-23 17:12:48.834947 foursight_core-4.1.0.1b0/foursight_core/adfasdfad
+-rw-r--r--   0        0        0       69 2023-04-16 14:05:52.759877 foursight_core-4.1.0.1b0/foursight_core/app.py
+-rw-r--r--   0        0        0   105730 2023-04-16 14:04:58.418881 foursight_core-4.1.0.1b0/foursight_core/app_utils.py
+-rw-r--r--   0        0        0   101241 2022-12-02 19:01:09.085977 foursight_core-4.1.0.1b0/foursight_core/app_utils.py---
+-rw-r--r--   0        0        0    97799 2022-11-22 14:52:55.397982 foursight_core-4.1.0.1b0/foursight_core/app_utils.py-deb
+-rw-r--r--   0        0        0    97949 2022-11-23 13:18:09.708092 foursight_core-4.1.0.1b0/foursight_core/app_utils.py-debug
+-rw-r--r--   0        0        0   101943 2023-03-29 22:48:31.801408 foursight_core-4.1.0.1b0/foursight_core/app_utils.py-debugg
+-rw-r--r--   0        0        0    12620 2022-11-30 14:04:39.423857 foursight_core-4.1.0.1b0/foursight_core/asdf
+-rw-r--r--   0        0        0     2571 2023-03-30 11:22:44.922092 foursight_core-4.1.0.1b0/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2022-09-07 10:08:59.760846 foursight_core-4.1.0.1b0/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2022-09-07 10:08:59.760916 foursight_core-4.1.0.1b0/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-03-31 17:00:42.022944 foursight_core-4.1.0.1b0/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-03-30 11:22:44.922592 foursight_core-4.1.0.1b0/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     4452 2023-04-10 14:14:30.704500 foursight_core-4.1.0.1b0/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-03-31 17:00:42.023738 foursight_core-4.1.0.1b0/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-03-31 17:00:42.024190 foursight_core-4.1.0.1b0/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-03-31 17:00:42.024311 foursight_core-4.1.0.1b0/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2022-09-07 10:08:59.761273 foursight_core-4.1.0.1b0/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-03-30 11:22:44.922849 foursight_core-4.1.0.1b0/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-03-30 11:22:44.923050 foursight_core-4.1.0.1b0/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2022-09-07 10:08:59.761552 foursight_core-4.1.0.1b0/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-03-31 17:00:42.024438 foursight_core-4.1.0.1b0/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-03-31 17:00:42.024598 foursight_core-4.1.0.1b0/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11437 2022-11-20 14:31:38.983954 foursight_core-4.1.0.1b0/foursight_core/d
+-rw-r--r--   0        0        0    11929 2023-03-31 17:00:42.024812 foursight_core-4.1.0.1b0/foursight_core/decorators.py
+-rw-r--r--   0        0        0    12565 2022-11-28 19:43:36.821773 foursight_core-4.1.0.1b0/foursight_core/decorators.py-new
+-rw-r--r--   0        0        0    15050 2023-03-31 17:00:42.025145 foursight_core-4.1.0.1b0/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8302 2023-04-16 04:32:00.359540 foursight_core-4.1.0.1b0/foursight_core/environment.py
+-rw-r--r--   0        0        0    11792 2023-03-31 17:00:42.025932 foursight_core-4.1.0.1b0/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2022-09-07 10:08:59.762246 foursight_core-4.1.0.1b0/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5146 2023-04-10 14:14:30.704795 foursight_core-4.1.0.1b0/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-04-10 14:14:30.705142 foursight_core-4.1.0.1b0/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-03-31 17:00:42.026791 foursight_core-4.1.0.1b0/foursight_core/mapping.json
+-rw-r--r--   0        0        0    95074 2022-11-15 14:26:15.846985 foursight_core-4.1.0.1b0/foursight_core/okk
+-rw-r--r--   0        0        0     1014 2023-03-30 11:22:44.924884 foursight_core-4.1.0.1b0/foursight_core/package.py
+-rw-r--r--   0        0        0     4846 2022-10-18 15:27:01.122701 foursight_core-4.1.0.1b0/foursight_core/react/api/'
+-rw-r--r--   0        0        0    26281 2022-12-06 19:54:26.692542 foursight_core-4.1.0.1b0/foursight_core/react/api/:w
+-rw-r--r--   0        0        0     5122 2022-10-19 18:25:39.526281 foursight_core-4.1.0.1b0/foursight_core/react/api/]:w
+-rw-r--r--   0        0        0    16866 2022-10-19 15:30:53.424281 foursight_core-4.1.0.1b0/foursight_core/react/api/adsfa
+-rw-r--r--   0        0        0    46462 2022-11-19 15:11:20.178519 foursight_core-4.1.0.1b0/foursight_core/react/api/alkd
+-rw-r--r--   0        0        0    32044 2022-10-21 15:56:11.928913 foursight_core-4.1.0.1b0/foursight_core/react/api/asav
+-rw-r--r--   0        0        0    28883 2022-10-19 18:32:59.913329 foursight_core-4.1.0.1b0/foursight_core/react/api/asdf
+-rw-r--r--   0        0        0    12150 2022-12-08 18:15:25.696290 foursight_core-4.1.0.1b0/foursight_core/react/api/asdff
+-rw-r--r--   0        0        0    13838 2023-04-16 14:05:39.122944 foursight_core-4.1.0.1b0/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0    14143 2023-03-31 15:18:53.676413 foursight_core-4.1.0.1b0/foursight_core/react/api/auth.py-deb
+-rw-r--r--   0        0        0     7091 2023-04-16 14:14:05.368090 foursight_core-4.1.0.1b0/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0     1163 2022-12-26 13:33:51.355358 foursight_core-4.1.0.1b0/foursight_core/react/api/aws_logs.py
+-rw-r--r--   0        0        0    23203 2023-03-31 17:00:42.028111 foursight_core-4.1.0.1b0/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3038 2023-03-31 17:00:42.028307 foursight_core-4.1.0.1b0/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6315 2023-03-31 17:00:42.028636 foursight_core-4.1.0.1b0/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28316 2023-03-31 17:00:42.029013 foursight_core-4.1.0.1b0/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    30044 2023-01-03 14:40:15.527405 foursight_core-4.1.0.1b0/foursight_core/react/api/checks.py---
+-rw-r--r--   0        0        0    28530 2022-12-07 15:57:38.726495 foursight_core-4.1.0.1b0/foursight_core/react/api/checks.py-new
+-rw-r--r--   0        0        0    20652 2023-03-31 17:00:42.029767 foursight_core-4.1.0.1b0/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     2921 2023-03-30 11:28:40.583613 foursight_core-4.1.0.1b0/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     5745 2023-03-31 17:00:42.030106 foursight_core-4.1.0.1b0/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-03-31 17:00:42.030271 foursight_core-4.1.0.1b0/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-03-31 17:00:42.030388 foursight_core-4.1.0.1b0/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4783 2023-03-31 17:00:42.030600 foursight_core-4.1.0.1b0/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0    58991 2022-12-25 17:24:38.880437 foursight_core-4.1.0.1b0/foursight_core/react/api/foo
+-rw-r--r--   0        0        0     3257 2023-03-31 17:00:42.030761 foursight_core-4.1.0.1b0/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0    13097 2022-11-07 19:29:38.049301 foursight_core-4.1.0.1b0/foursight_core/react/api/hama
+-rw-r--r--   0        0        0    44446 2022-11-18 16:41:20.868752 foursight_core-4.1.0.1b0/foursight_core/react/api/hmm
+-rw-r--r--   0        0        0     3516 2023-03-31 17:00:42.030910 foursight_core-4.1.0.1b0/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9524 2023-03-31 17:00:42.031263 foursight_core-4.1.0.1b0/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0    14646 2022-10-23 19:06:03.352206 foursight_core-4.1.0.1b0/foursight_core/react/api/ok
+-rw-r--r--   0        0        0    27126 2022-12-07 16:03:28.375164 foursight_core-4.1.0.1b0/foursight_core/react/api/oklk
+-rw-r--r--   0        0        0    17397 2022-10-19 18:57:09.208083 foursight_core-4.1.0.1b0/foursight_core/react/api/okok
+-rw-r--r--   0        0        0    15418 2022-10-23 19:08:13.968538 foursight_core-4.1.0.1b0/foursight_core/react/api/okokok
+-rw-r--r--   0        0        0    37016 2022-11-12 14:03:53.287757 foursight_core-4.1.0.1b0/foursight_core/react/api/okokokok
+-rw-r--r--   0        0        0    39205 2022-11-12 19:00:46.033390 foursight_core-4.1.0.1b0/foursight_core/react/api/okokokokok
+-rw-r--r--   0        0        0    29102 2022-12-07 19:03:24.489085 foursight_core-4.1.0.1b0/foursight_core/react/api/ot
+-rw-r--r--   0        0        0    74253 2023-04-17 03:34:17.104104 foursight_core-4.1.0.1b0/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    45701 2022-10-21 14:29:00.904736 foursight_core-4.1.0.1b0/foursight_core/react/api/react_api.py-
+-rw-r--r--   0        0        0    30313 2022-10-21 17:36:32.520832 foursight_core-4.1.0.1b0/foursight_core/react/api/react_api.py--
+-rw-r--r--   0        0        0    71345 2023-01-23 23:30:44.383522 foursight_core-4.1.0.1b0/foursight_core/react/api/react_api.py----
+-rw-r--r--   0        0        0    46990 2022-11-22 14:51:44.189069 foursight_core-4.1.0.1b0/foursight_core/react/api/react_api.py-deb
+-rw-r--r--   0        0        0    24458 2022-10-22 23:24:49.505751 foursight_core-4.1.0.1b0/foursight_core/react/api/react_api.py-saaave
+-rw-r--r--   0        0        0    11336 2023-04-10 14:14:40.711249 foursight_core-4.1.0.1b0/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0    11721 2023-03-31 15:18:58.965799 foursight_core-4.1.0.1b0/foursight_core/react/api/react_api_base.py-deb
+-rw-r--r--   0        0        0    10435 2022-10-22 23:25:02.692255 foursight_core-4.1.0.1b0/foursight_core/react/api/react_app.py-saaave
+-rw-r--r--   0        0        0     8025 2023-03-31 17:00:42.033249 foursight_core-4.1.0.1b0/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0     5576 2022-10-19 22:12:16.865537 foursight_core-4.1.0.1b0/foursight_core/react/api/react_route_utils.py-
+-rw-r--r--   0        0        0     7471 2022-10-22 19:19:42.543417 foursight_core-4.1.0.1b0/foursight_core/react/api/react_route_utils.py.save
+-rw-r--r--   0        0        0    31570 2023-04-16 23:01:06.114489 foursight_core-4.1.0.1b0/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0    12876 2022-10-22 19:00:58.268720 foursight_core-4.1.0.1b0/foursight_core/react/api/react_routes.py.save
+-rw-r--r--   0        0        0     4861 2023-03-31 17:00:42.034179 foursight_core-4.1.0.1b0/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0     5027 2022-10-17 22:40:41.733498 foursight_core-4.1.0.1b0/foursight_core/react/api/react_ui.py-bak
+-rw-r--r--   0        0        0     4206 2022-10-17 22:47:29.529384 foursight_core-4.1.0.1b0/foursight_core/react/api/react_ui.py-debug
+-rw-r--r--   0        0        0    56415 2022-12-15 17:41:55.903970 foursight_core-4.1.0.1b0/foursight_core/react/api/sa
+-rw-r--r--   0        0        0    42517 2022-11-15 20:10:51.305457 foursight_core-4.1.0.1b0/foursight_core/react/api/sav
+-rw-r--r--   0        0        0    16885 2022-10-19 15:44:40.693752 foursight_core-4.1.0.1b0/foursight_core/react/api/save
+-rw-r--r--   0        0        0   274720 2022-12-09 23:44:54.837473 foursight_core-4.1.0.1b0/foursight_core/react/api/x
+-rw-r--r--   0        0        0    31785 2022-10-21 15:29:37.208969 foursight_core-4.1.0.1b0/foursight_core/react/api/xx
+-rw-r--r--   0        0        0    56739 2022-12-15 20:17:56.533252 foursight_core-4.1.0.1b0/foursight_core/react/api/xxy
+-rw-r--r--   0        0        0     5921 2022-10-21 16:32:06.326758 foursight_core-4.1.0.1b0/foursight_core/react/api/xyz
+-rw-r--r--   0        0        0      806 2023-03-31 17:00:42.034293 foursight_core-4.1.0.1b0/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-04-17 11:24:11.660114 foursight_core-4.1.0.1b0/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-04-17 11:24:11.657555 foursight_core-4.1.0.1b0/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-04-17 11:24:02.786608 foursight_core-4.1.0.1b0/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11735 2023-04-17 11:24:11.556386 foursight_core-4.1.0.1b0/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1917119 2023-04-17 11:24:11.556598 foursight_core-4.1.0.1b0/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-03-31 17:00:42.046642 foursight_core-4.1.0.1b0/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-03-31 17:00:42.047578 foursight_core-4.1.0.1b0/foursight_core/routes.py
+-rw-r--r--   0        0        0    22442 2023-03-31 17:00:42.047831 foursight_core-4.1.0.1b0/foursight_core/run_result.py
+-rw-r--r--   0        0        0    22924 2022-11-21 20:22:40.475142 foursight_core-4.1.0.1b0/foursight_core/run_result.py-deb
+-rw-r--r--   0        0        0     6330 2023-03-31 17:00:42.048014 foursight_core-4.1.0.1b0/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0    95791 2022-11-15 19:33:17.290307 foursight_core-4.1.0.1b0/foursight_core/sav
+-rw-r--r--   0        0        0     5282 2023-03-31 17:00:42.048163 foursight_core-4.1.0.1b0/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     6458 2022-11-04 14:38:30.182413 foursight_core-4.1.0.1b0/foursight_core/schedule_decorator.py-
+-rw-r--r--   0        0        0     1402 2023-03-31 17:00:42.048268 foursight_core-4.1.0.1b0/foursight_core/scripts/decrypt_accounts_file.py
+-rw-r--r--   0        0        0     1406 2023-03-31 17:00:42.048339 foursight_core-4.1.0.1b0/foursight_core/scripts/encrypt_accounts_file.py
+-rw-r--r--   0        0        0       65 2022-11-14 16:31:57.489442 foursight_core-4.1.0.1b0/foursight_core/scripts/p
+-rw-r--r--   0        0        0      797 2022-11-17 17:02:52.436871 foursight_core-4.1.0.1b0/foursight_core/scripts/save/decrypt_accounts_file.py
+-rw-r--r--   0        0        0      801 2022-11-17 17:02:55.810728 foursight_core-4.1.0.1b0/foursight_core/scripts/save/encrypt_accounts_file.py
+-rw-r--r--   0        0        0     5370 2023-03-31 17:00:42.048769 foursight_core-4.1.0.1b0/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-03-30 11:23:29.553404 foursight_core-4.1.0.1b0/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-03-30 11:26:56.704948 foursight_core-4.1.0.1b0/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-04-10 14:14:30.716241 foursight_core-4.1.0.1b0/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2022-09-07 10:08:59.763471 foursight_core-4.1.0.1b0/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-03-30 11:28:21.582264 foursight_core-4.1.0.1b0/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2022-09-07 10:08:59.763671 foursight_core-4.1.0.1b0/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-03-30 11:26:56.705625 foursight_core-4.1.0.1b0/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-03-30 11:26:56.705764 foursight_core-4.1.0.1b0/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-03-30 11:26:56.706033 foursight_core-4.1.0.1b0/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-03-30 11:26:56.706216 foursight_core-4.1.0.1b0/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1489 2023-03-29 22:45:57.789020 foursight_core-4.1.0.1b0/foursight_core/x
+-rw-r--r--   0        0        0      231 2023-02-23 19:48:15.449939 foursight_core-4.1.0.1b0/foursight_core/x.py]
+-rw-r--r--   0        0        0     1531 2023-04-17 11:40:07.344751 foursight_core-4.1.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0     1854 1970-01-01 00:00:00.000000 foursight_core-4.1.0.1b0/setup.py
+-rw-r--r--   0        0        0     1163 1970-01-01 00:00:00.000000 foursight_core-4.1.0.1b0/PKG-INFO
```

### Comparing `foursight_core-3.3.2.2b1/LICENSE.txt` & `foursight_core-4.1.0.1b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/abstract_connection.py` & `foursight_core-4.1.0.1b0/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/app_utils.py` & `foursight_core-4.1.0.1b0/foursight_core/app_utils.py-debugg`

 * *Files 1% similar despite different names*

```diff
@@ -1448,28 +1448,41 @@
         put_uuid = put_data.get('uuid', datetime.datetime.utcnow().isoformat())
         putCheck = self.CheckResult(connection, check, init_uuid=put_uuid)
         # set valid fields from the PUT body. should this be dynamic?
         # if status is not included, it will be set to ERROR
         for field in ['title', 'status', 'summary', 'description', 'brief_output', 'full_output', 'admin_output']:
             put_content = put_data.get(field)
             prev_content = getattr(putCheck, field, None)
+            #xyzzy
+            if field == 'full_output':
+                print('xyzzy/1')
+                print(put_content)
+                print(prev_content)
+                print('xyzzy/2')
+            #xyzzy
             if put_content:
                 # append attribute data for _output fields if there are pre-existing
                 # values originating from an existing put_uuid
                 if prev_content and field in ['full_output', 'brief_output', 'admin_output']:
                     # will be list, dict, or string. make sure they are same type
                     if isinstance(prev_content, dict) and isinstance(put_content, dict):
                         prev_content.update(put_content)
                     elif isinstance(prev_content, list) and isinstance(put_content, list):
                         prev_content.extend(put_content)
                     elif isinstance(prev_content, str) and isinstance(put_content, str):
                         prev_content = prev_content + put_content
                     else:
                         # cannot append, just update with new
                         prev_content = put_content
+                    #xyzzy
+                    if field == 'full_output':
+                        print('xyzzy/3')
+                        print(prev_content)
+                        print('xyzzy/4')
+                    #xyzzy
                     setattr(putCheck, field, prev_content)
                 else:
                     setattr(putCheck, field, put_content)
         # set 'primary' kwarg so that the result is stored as 'latest'
         putCheck.kwargs = {'primary': True, 'uuid': put_uuid}
         stored = putCheck.store_result()
         response.body = {
```

### Comparing `foursight_core-3.3.2.2b1/foursight_core/buckets.py` & `foursight_core-4.1.0.1b0/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/check_schema.py` & `foursight_core-4.1.0.1b0/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/check_utils.py` & `foursight_core-4.1.0.1b0/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.1.0.1b0/foursight_core/checks/access_key_expiration_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         except Exception:
             continue  # user not found
         user_uuid = user['uuid']
         access_keys = search_metadata(f'/search/?type=AccessKey&description={kp_name}&user.uuid={user_uuid}'
                                       f'&sort=-date_created', key=connection.ff_keys)
         # generate new key
         access_key_req = {'user': user_uuid, 'description': kp_name}
-        access_key_res = post_metadata('/access_key', access_key_req, key=connection.ff_keys)
+        access_key_res = post_metadata(access_key_req, 'access-keys', key=connection.ff_keys)['@graph'][0]
         s3_obj = {'secret': access_key_res['secret_access_key'],
                   'key': access_key_res['access_key_id'],
                   'server': s3.url}
         s3.s3_put_secret(s3_obj, kp_name)
         full_output['successfully_generated'].append(email)
         # clear out old keys after generating new one
         for access_key in access_keys:  # note this search result was computed before the new key was added
```

### Comparing `foursight_core-3.3.2.2b1/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.1.0.1b0/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/checks/ecs_checks.py` & `foursight_core-4.1.0.1b0/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.1.0.1b0/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.1.0.1b0/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.1.0.1b0/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/checks/scaling_checks.py` & `foursight_core-4.1.0.1b0/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/checks/test_checks.py` & `foursight_core-4.1.0.1b0/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/decorators.py` & `foursight_core-4.1.0.1b0/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/deploy.py` & `foursight_core-4.1.0.1b0/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/environment.py` & `foursight_core-4.1.0.1b0/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/es_connection.py` & `foursight_core-4.1.0.1b0/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/exceptions.py` & `foursight_core-4.1.0.1b0/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/fs_connection.py` & `foursight_core-4.1.0.1b0/foursight_core/fs_connection.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,17 @@
+import os
+
+import redis.exceptions
 from foursight_core.s3_connection import S3Connection
 from foursight_core.es_connection import ESConnection
+from dcicutils.misc_utils import PRINT
 from dcicutils.s3_utils import s3Utils
 from dcicutils.env_utils import full_env_name, is_stg_or_prd_env
+from dcicutils.redis_utils import create_redis_client
+from dcicutils.redis_tools import RedisBase, RedisSessionToken
 
 
 class FSConnection(object):
     """
     Contains the foursight (FS) and fourfront (FF) connections needed to
     communicate with both services. Contains fields that link to the FF keys,
     and s3 connection, as well as the FS s3_connection. They are:
@@ -36,14 +42,26 @@
             'es': es
         }
         # FOURFRONT information
         self.ff_server = fs_environ_info['fourfront']
         self.ff_env = fs_environ_info['ff_env']
         self.ff_es = fs_environ_info['es']
         self.ff_bucket = fs_environ_info['bucket']
+        try:
+            if 'redis' in fs_environ_info:
+                self.redis = RedisBase(create_redis_client(url=fs_environ_info['redis']))
+            elif 'REDIS_HOST' in os.environ:  # temporary patch in until env config is fully sorted - Will
+                self.redis = RedisBase(create_redis_client(url=os.environ['REDIS_HOST']))
+            else:
+                self.redis = None
+        except redis.exceptions.ConnectionError:
+            PRINT('Cannot connect to Redis')
+            PRINT('This error is expected when deploying with remote (ElastiCache) Redis')
+        PRINT(self.redis)
+        PRINT(os.environ.get('REDIS_HOST', 'no-redis-host'))
         if not test:
             self.ff_s3 = s3Utils(env=self.ff_env)
             try:  # TODO: make this configurable from env variables?
                 self.ff_keys = self.ff_s3.get_access_keys('access_key_foursight')
             except Exception as e:
                 raise Exception('Could not initiate connection to Fourfront; it is probably a bad ff_env. '
                       'You gave: %s. Error message: %s' % (self.ff_env, str(e)))
@@ -80,7 +98,15 @@
             return self.connections['es'].test_connection()
         return False
 
     def es_info(self):
         """ Returns basic info about the Elasticsearch server. """
         if self.connections['es']:
             return self.connections['es'].info()
+
+    def redis_info(self):
+        """ Returns basic info about the Redis server """
+        return self.redis.info() if self.redis else None
+
+    def get_redis_base(self):
+        """ Returns handle to FS Redis Base object """
+        return self.redis
```

### Comparing `foursight_core-3.3.2.2b1/foursight_core/identity.py` & `foursight_core-4.1.0.1b0/foursight_core/identity.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,16 @@
     # This maps key names in the global application configuration (GAC) to names used here.
     IDENTITY_KEY_MAP_REQUIRED = {
         "ENCODED_AUTH0_CLIENT": "CLIENT_ID",
         "ENCODED_AUTH0_SECRET": "CLIENT_SECRET",
         "ENCODED_ES_SERVER": "ES_HOST",
     }
     IDENTITY_KEY_MAP_OPTIONAL = {
-        "ENCODED_S3_ENCRYPT_KEY_ID": "S3_ENCRYPT_KEY_ID"
+        "ENCODED_S3_ENCRYPT_KEY_ID": "S3_ENCRYPT_KEY_ID",
+        "ENCODED_REDIS_SERVER": "REDIS_HOST"
     }
 
     apply_identity(identity_kind=GLOBAL_APPLICATION_CONFIGURATION, rename_keys=IDENTITY_KEY_MAP_REQUIRED)
     try:
         apply_identity(identity_kind=GLOBAL_APPLICATION_CONFIGURATION, rename_keys=IDENTITY_KEY_MAP_OPTIONAL)
     except (KeyError, ValueError):
         pass
```

### Comparing `foursight_core-3.3.2.2b1/foursight_core/mapping.json` & `foursight_core-4.1.0.1b0/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/package.py` & `foursight_core-4.1.0.1b0/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/auth.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,88 @@
+import os
 import boto3
 import logging
 import time
+import redis
 from typing import Optional
+from dcicutils.redis_utils import create_redis_client
+from dcicutils.redis_tools import RedisBase, RedisSessionToken, SESSION_TOKEN_COOKIE
+from dcicutils.env_utils import full_env_name
+from dcicutils.misc_utils import ignored, PRINT
 from ...app import app
 from .cookie_utils import read_cookie
 from .envs import Envs
 from .jwt_utils import JWT_AUDIENCE_PROPERTY_NAME, JWT_SUBJECT_PROPERTY_NAME, jwt_decode, jwt_encode
 from .misc_utils import get_request_domain
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
+# Constant for authtoken derived from JWT to give info about the user to
+# the front-end
+AUTH_TOKEN_COOKIE = 'authtoken'
+
+
 class Auth:
 
     def __init__(self, auth0_client: str, auth0_secret: str, envs: Envs):
         self._auth0_client = auth0_client
         self._auth0_secret = auth0_secret
         self._envs = envs
+        # acquired from identity or env variable locally
+        try:
+            self._redis = RedisBase(create_redis_client(
+                url=os.environ['REDIS_HOST'])
+            ) if 'REDIS_HOST' in os.environ else None
+        except redis.exceptions.ConnectionError:
+            PRINT('Cannot connect to Redis')
+            PRINT('This error is expected when deploying with remote (ElastiCache) Redis')
+            self._redis = None
 
     _cached_aws_credentials = {}
 
+    def get_redis_handler(self):
+        """
+        Returns a handler to Redis or None if not in use
+        """
+        return self._redis
+
+    @classmethod
+    def get_redis_namespace(cls, env: str) -> str:
+        ignored(env)
+        # As of April 2023 simply use a static non-per-environment namespace for the Redis
+        # auth token; this is so we can switch among different environments in Foursight
+        # with the same login session, as it was working before the Redis auth work;
+        return "foursight"
+
     def authorize(self, request: dict, env: Optional[str] = None) -> dict:
         """
         Verifies that the given request is authenticated AND authorized, based on the authtoken
         cookie (a JWT-signed-encoded value) in the given request. If so, returns the verified and
         decoded authtoken as a dictionary. If not, returns a dictionary indicating not authorized
         and/or not authenticated, and containing the basic info from the authtoken.
         """
         try:
+            # Read the c4_st token (new Redis session token if Redis is in use)
+            if self._redis:
+                c4_st = read_cookie(request, SESSION_TOKEN_COOKIE)
+                redis_session_token = RedisSessionToken.from_redis(
+                    redis_handler=self._redis,
+                    namespace=self.get_redis_namespace(env),
+                    token=c4_st
+                )
+                # if this session token is not valid, nothing else is to be trusted, so bail here
+                if (not redis_session_token or
+                        not redis_session_token.validate_session_token(redis_handler=self._redis)):
+                    return self._create_unauthenticated_response(request, "missing-or-invalid-session-token")
 
-            # Read the authtoken cookie.
+            # Read the authtoken cookie (will always be present).
 
-            authtoken = read_cookie(request, "authtoken")
+            authtoken = read_cookie(request, AUTH_TOKEN_COOKIE)
             if not authtoken:
                 return self._create_unauthenticated_response(request, "no-authtoken")
 
             # Decode the authtoken cookie.
 
             authtoken_decoded = self.decode_authtoken(authtoken)
             if not authtoken_decoded:
```

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/auth0_config.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/auth0_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,17 @@
         "scope": "openid email",
         "prompt": "select_account",
         "connections": ["github", "google-oauth2"]
     }
 
     def __init__(self, portal_url: str) -> None:
         if not portal_url:
-            raise ValueError("Portal URL required for Auth0Config usage.")
+            portal_url = ""
+            logger.error("Portal URL required for Auth0Config usage.")
+            # raise ValueError("Portal URL required for Auth0Config usage.")
         self._portal_url = portal_url
         self._config_url = f"{portal_url}{'/' if not portal_url.endswith('/') else ''}auth0_config?format=json"
         self._config_data = {}
         self._config_raw_data = {}
 
     def get_portal_url(self) -> str:
         return self._portal_url
```

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/aws_network.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/aws_s3.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/checks.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/cognito.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/encryption.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/envs.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/envs.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,19 +7,14 @@
 from dcicutils.misc_utils import find_association
 from .gac import Gac
 from .misc_utils import memoize
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
-_TEMPORARY_HACK_FOR_DEBUGGING_TO_ALLOW_DAVID_MICHAELS_FOR_ANY_ENV_20230316 = True
-
-def _temporary_hack_for_debugging_to_allow_david_michaels_for_any_env_20230316(email: str) -> bool:
-    return _TEMPORARY_HACK_FOR_DEBUGGING_TO_ALLOW_DAVID_MICHAELS_FOR_ANY_ENV_20230316 and email == "david_michaels@hms.harvard.edu"
-
 
 # TODO
 # Rationalize this with dcicutil.utils env_utils functions for name versions, normalizations, comparisons.
 # Did at least some of this (below, e.g. find_known_env, is_same_env); but see if we can perhaps get away
 # from even having to keep these (5) name versions around (i.e. name, short_name, full_name, public_name,
 # foursight_name); the UI currently relies on these.
 class Envs:
@@ -69,48 +64,38 @@
         return False
 
     @memoize
     def is_same_env(self, env_a: str, env_b: str) -> bool:
         return foursight_env_name(env_a) == foursight_env_name(env_b)
 
     def get_user_auth_info(self, email: str) -> Tuple[list, str, str]:
-        print(f'xyzzy/get_user_auth_info/enter: [{email}]')
         """
         Returns a tuple containing (in left-right order): the list of known environments,
         i.e the list of annotated environment name objects; the list of allowed environment
         names for the given user/email, via the users store in ElasticSearch; and since we're
         getting the user record anyways, the first/last name of the user, for display only.
         """
         allowed_envs = []
         first_name = None
         last_name = None
         for known_env in self._known_envs:
             try:
                 # Note we must lower case the email to find the user. This is because all emails
                 # in the database are lowercased; it causes issues with OAuth if we don't do this.
-                print(f'xyzzy/get_user_auth_info/a: [{known_env}]')
                 user = ff_utils.get_metadata('users/' + email.lower(),
                                              ff_env=known_env["full_name"], add_on="frame=object&datastore=database")
-                print(f'xyzzy/get_user_auth_info/b: [{known_env}]')
-                print(user)
-                if _temporary_hack_for_debugging_to_allow_david_michaels_for_any_env_20230316(email) or self._is_user_allowed_access(user):
+                if self._is_user_allowed_access(user):
                     # Since this is in a loop, for each env, this setup here will end up getting first/last name
                     # from the last env in the loop; doesn't really matter, just pick one set; this is just for
                     # informational/display purposes in the UI.
                     first_name = user.get("first_name")
                     last_name = user.get("last_name")
                     allowed_envs.append(known_env["full_name"])
             except Exception as e:
                 logger.warning(f"Exception getting allowed envs for {email}: {e}")
-                if _temporary_hack_for_debugging_to_allow_david_michaels_for_any_env_20230316(email):
-                    print(f'xyzzy/get_user_auth_info/c: temporary hack for debugging to allow david_michaels@hms.harvard.edu access any environment.')
-                    first_name = "David"
-                    last_name = "Michaels"
-                    allowed_envs.append(known_env["full_name"])
-        print(f'xyzzy/get_user_auth_info/return: {allowed_envs} [{first_name}] [{last_name}]')
         return allowed_envs, first_name, last_name
 
     @staticmethod
     def _is_user_allowed_access(user: Optional[dict]) -> bool:
         return user and Envs._is_user_in_one_or_more_groups(user, ["admin", "foursight"])
 
     @staticmethod
```

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/gac.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/misc_utils.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/react_api.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/react_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,32 +9,37 @@
 import requests
 import socket
 import time
 from typing import Optional
 import urllib.parse
 from itertools import chain
 from dcicutils.env_utils import EnvUtils, get_foursight_bucket, get_foursight_bucket_prefix, full_env_name
+from dcicutils.env_utils import get_portal_url as env_utils_get_portal_url
 from dcicutils import ff_utils
 from dcicutils.misc_utils import ignored
 from dcicutils.obfuscation_utils import obfuscate_dict
+from dcicutils.redis_tools import RedisSessionToken, SESSION_TOKEN_COOKIE
+from dcicutils.ssl_certificate_utils import get_ssl_certificate_info
 from ...app import app
+from .auth import AUTH_TOKEN_COOKIE
+from .auth import Auth
 from .aws_network import (
     aws_get_network, aws_get_security_groups,
     aws_get_security_group_rules, aws_get_subnets, aws_get_vpcs, aws_network_cache_clear
 )
 from .aws_s3 import AwsS3
 from .aws_stacks import (
     aws_get_stack, aws_get_stacks,
     aws_get_stack_outputs, aws_get_stack_parameters,
     aws_get_stack_resources, aws_get_stack_template,
     aws_stacks_cache_clear
 )
 from .checks import Checks
 from .cognito import clear_cognito_cache, get_cognito_oauth_config, handle_cognito_oauth_callback
-from .cookie_utils import create_delete_cookie_string
+from .cookie_utils import create_delete_cookie_string, read_cookie
 from .datetime_utils import convert_uptime_to_datetime, convert_utc_datetime_to_useastern_datetime_string
 from .encryption import Encryption
 from .encoding_utils import base64_decode_to_json
 from .gac import Gac
 from .misc_utils import (
     get_base_url,
     is_running_locally,
@@ -237,17 +242,28 @@
         """
         authorize_response = self._auth.authorize(request, env)
         if not authorize_response or not authorize_response["authorized"]:
             body = {"status": "Already logged out."}
         else:
             body = {"status": "Logged out."}
         domain, context = app.core.get_domain_and_context(request)
-        authtoken_cookie_deletion = create_delete_cookie_string(request=request, name="authtoken", domain=domain)
+        authtoken_cookie_deletion = create_delete_cookie_string(request=request, name=AUTH_TOKEN_COOKIE, domain=domain)
+        c4_st_cookie_deletion = create_delete_cookie_string(request=request, name=SESSION_TOKEN_COOKIE, domain=domain)
         redirect_url = self.get_redirect_url(request, env, domain, context)
-        headers = {"Set-Cookie": authtoken_cookie_deletion}
+        # always delete both cookies on logout
+        headers = {"Set-Cookie": [authtoken_cookie_deletion, c4_st_cookie_deletion]}
+        redis_handler = self._auth.get_redis_handler()
+        if redis_handler:
+            redis_session_token = RedisSessionToken.from_redis(
+                redis_handler=redis_handler,
+                namespace=Auth.get_redis_namespace(env),
+                token=read_cookie(request, SESSION_TOKEN_COOKIE)
+            )
+            if redis_session_token:
+                redis_session_token.delete_session_token(redis_handler=redis_handler)
         return self.create_redirect_response(location=redirect_url, body=body, headers=headers)
 
     def reactapi_header(self, request: dict, env: str) -> Response:
         """
         Called from react_routes for endpoint: GET /{env}/header
         Note that this in an UNPROTECTED route.
         """
@@ -267,60 +283,90 @@
             data["auth"]["known_envs"] = self._envs.get_known_envs_with_gac_names()
         else:
             known_envs_default = self._envs.find_known_env(self._envs.get_default_env())
             known_envs_actual_count = self._envs.get_known_envs_count()
             data["auth"]["known_envs"] = [known_envs_default]
             data["auth"]["known_envs_actual_count"] = known_envs_actual_count
         data["auth"]["default_env"] = self._envs.get_default_env()
+        if not data["portal"]["url"]:
+            # Here we did not get a Portal URL from the to app.core.get_portal_url (via _reactapi_header_nocache).
+            # That call ends up ultimately calling the Portal health endpoint (via s3Utils.get_synthetic_env_config
+            # via environment.get_environment_and_bucket_info). So there may have been a problem with the Portal,
+            # e.g. bad SSL certificate; we will get the Portal URL by other means, and from get get its SSL
+            # certificate to help diagnose any problem with that. C4-1017 (April 2023).
+            try:
+                portal_url = app.core.get_portal_url(env or default_env, raise_exception=True)
+                data["portal"]["url"] = portal_url
+            except Exception as e:
+                e = str(e)
+                data["portal"]["exception"] = e
+                if "cert" in e.lower():
+                    data["portal"]["ssl_certificate_error"] = True
+                portal_url = env_utils_get_portal_url(env)
+                data["portal"]["url"] = portal_url
+                data["portal"]["ssl_certificate"] = get_ssl_certificate_info(portal_url)
         data["timestamp"] = convert_utc_datetime_to_useastern_datetime_string(datetime.datetime.utcnow())
         return self.create_success_response(data)
 
     def _reactapi_header_nocache(self, request: dict, env: str) -> dict:
         """
         No-cache version of above reactapi_header function.
         """
         domain, context = app.core.get_domain_and_context(request)
         stage_name = app.core.stage.get_stage()
         default_env = self._envs.get_default_env()
         aws_credentials = self._auth.get_aws_credentials(env or default_env)
-        portal_url = get_base_url(app.core.get_portal_url(env or default_env))
+        portal_url = app.core.get_portal_url(env or default_env)
+        portal_base_url = get_base_url(portal_url)
         response = {
             "app": {
                 "title": app.core.html_main_title,
                 "package": app.core.APP_PACKAGE_NAME,
                 "stage": stage_name,
                 "version": app.core.get_app_version(),
                 "domain": domain,
                 "context": context,
                 "stack": self._get_stack_name(),
                 "local": is_running_locally(request),
                 "credentials": {
-                    "aws_account_number": aws_credentials["aws_account_number"],
+                    "aws_account_number": aws_credentials.get("aws_account_number"),
                     "aws_account_name": aws_credentials.get("aws_account_name"),
                     "re_captcha_key": os.environ.get("reCaptchaKey", None)
                 },
                 "launched": app.core.init_load_time,
                 "deployed": app.core.get_lambda_last_modified(),
                 "accounts_file": self._get_accounts_file(),
                 "accounts_file_from_s3": self._get_accounts_file_from_s3()
             },
             "versions": self._get_versions_object(),
             "portal": {
                 "url": app.core.get_portal_url(env or default_env),
-                "health_url": portal_url + "/health?format=json",
-                "health_ui_url": portal_url + "/health"
+                "health_url": portal_base_url + "/health?format=json",
+                "health_ui_url": portal_base_url + "/health"
             },
             "s3": {
                 "bucket_org": os.environ.get("ENCODED_S3_BUCKET_ORG", os.environ.get("S3_BUCKET_ORG", None)),
                 "global_env_bucket": os.environ.get("GLOBAL_ENV_BUCKET", os.environ.get("GLOBAL_BUCKET_ENV", None)),
                 "encrypt_key_id": os.environ.get("S3_ENCRYPT_KEY_ID", None)
             }
         }
         return response
 
+    def reactapi_certificates(self, request: dict, args: Optional[dict] = None) -> Response:
+        expires_soon_days = int(args.get("soon", "0")) if args else 0
+        foursight_url = self.foursight_instance_url(request)
+        portal_url = env_utils_get_portal_url(self._envs.get_default_env())
+        foursight_ssl_certificate_info = get_ssl_certificate_info(foursight_url, expires_soon_days=expires_soon_days)
+        portal_ssl_certificate_info = get_ssl_certificate_info(portal_url, expires_soon_days=expires_soon_days)
+        response = {
+            "foursight_ssl_certificate": foursight_ssl_certificate_info,
+            "portal_ssl_certificate": portal_ssl_certificate_info
+        }
+        return self.create_success_response(response)
+
     @memoize
     def _get_env_and_bucket_info(self, env: str, stage_name: str) -> dict:
         return sort_dictionary_by_case_insensitive_keys(
             obfuscate_dict(app.core.environment.get_environment_and_bucket_info(env, stage_name)))
 
     @memoize
     def _get_check_result_bucket_name(self, env: str) -> Optional[str]:
```

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/react_api_base.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/react_api_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import copy
 import datetime
 import json
 import requests
 from typing import Optional, Union
 import urllib.parse
 from dcicutils.misc_utils import get_error_message
+from dcicutils.redis_tools import RedisSessionToken, SESSION_TOKEN_COOKIE
 from ...app import app
 from ...route_prefixes import ROUTE_PREFIX
-from .auth import Auth
+from .auth import Auth, AUTH_TOKEN_COOKIE
 from .auth0_config import Auth0Config
 from .cookie_utils import create_set_cookie_string, read_cookie
 from .datetime_utils import convert_datetime_to_time_t
 from .envs import Envs
 from .misc_utils import (
     get_request_arg,
     is_running_locally,
@@ -125,15 +126,15 @@
 
     def react_authentication_callback(self, request: dict, env: str) -> Response:
         """
         Called by the main authentication callback function (app_utils.auth0_callback)
         if the above is_react_authentication_callback returns True. Performs the actual
         Auth0 authentication for login via the Auth0 (HTTP POST) API. If successful,
         returns a redirect response (to the UI) with a cookie setting for the login
-        authtoken. If unsuccessful, returnes a forbidden (HTTP 403) response.
+        authtoken. If unsuccessful, returns a forbidden (HTTP 403) response.
         """
 
         auth0_code = get_request_arg(request, "code")
         auth0_domain = self._auth0_config.get_domain()
         auth0_client = self._auth0_config.get_client()
         auth0_secret = self._auth0_config.get_secret()
         if not (auth0_code and auth0_domain and auth0_client and auth0_secret):
@@ -162,18 +163,32 @@
             return self.create_forbidden_response()
 
         jwt_expires_in = auth0_response_json.get("expires_in")
         jwt_expires_at = convert_datetime_to_time_t(datetime.datetime.utcnow() +
                                                     datetime.timedelta(seconds=jwt_expires_in))
         domain, context = app.core.get_domain_and_context(request)
         authtoken = self._auth.create_authtoken(jwt, jwt_expires_at, domain)
-        authtoken_cookie = create_set_cookie_string(request, name="authtoken",
+        authtoken_cookie = create_set_cookie_string(request, name=AUTH_TOKEN_COOKIE,
                                                     value=authtoken,
                                                     domain=domain,
                                                     expires=jwt_expires_at, http_only=False)
+
+        # if Redis is in use, create and return session token as well
+        redis_handler = self._auth.get_redis_handler()
+        if redis_handler:
+            redis_session_token = RedisSessionToken(
+                namespace=Auth.get_redis_namespace(env), jwt=jwt
+            )
+            redis_session_token.store_session_token(redis_handler=redis_handler)
+            c4_st_cookie = create_set_cookie_string(request, name=SESSION_TOKEN_COOKIE,
+                                                    value=redis_session_token.get_session_token(),
+                                                    domain=domain,
+                                                    expires=str(datetime.datetime.utcnow() +
+                                                                redis_session_token.get_expiration()))
+            authtoken_cookie = [authtoken_cookie, c4_st_cookie]
         redirect_url = self.get_redirect_url(request, env, domain, context)
         return self.create_redirect_response(location=redirect_url, headers={"Set-Cookie": authtoken_cookie})
 
     def react_authorize(self, request: dict, env: Optional[str]) -> dict:
         """
         Exposed for call from "route" decorator for endpoint authentication protection.
         """
```

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/react_routes.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/react_routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,35 @@
     def reactapi_route_header_noenv() -> Response:  # noqa: implicit @staticmethod via @route
         """
         Note that this in an UNPROTECTED route.
         No-env version of above /{env}/header route.
         """
         return app.core.reactapi_header(app.current_request.to_dict(), app.core.get_default_env())
 
+    @route("/{env}/certificates", authorize=False)
+    def reactapi_route_certificates(env: str) -> Response:  # noqa: implicit @staticmethod via @route
+        """
+        Note that this in an UNPROTECTED route.
+        Returns SSL certificate info about this Foursight instance and its associated Portal instance.
+        """
+        ignored(env)
+        #args = get_request_args(request_dict)
+        #return app.core.reactapi_certificates(app.current_request.to_dict(), args)
+        return ReactRoutes.reactapi_route_certificates_noenv()
+
+    @route("/certificates", authorize=False)
+    def reactapi_route_certificates_noenv() -> Response:  # noqa: implicit @staticmethod via @route
+        """
+        Note that this in an UNPROTECTED route.
+        Returns SSL certificate info about this Foursight instance and its associated Portal instance.
+        """
+        request_dict = app.current_request.to_dict()
+        args = get_request_args(request_dict)
+        return app.core.reactapi_certificates(request_dict, args)
+
     # ----------------------------------------------------------------------------------------------
     # Foursight React API routes PROTECTED by authorization/authentication.
     # ----------------------------------------------------------------------------------------------
 
     @route("/{env}/info", authorize=True)
     def reactapi_route_info(env: str) -> Response:  # noqa: implicit @staticmethod via @route
         """
```

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/react_ui.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.1.0.1b0/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/ui/index.html` & `foursight_core-4.1.0.1b0/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.1.0.1b0/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.1.0.1b0/foursight_core/react/ui/static/js/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.373b6a1c.js.LICENSE.txt */
+/*! For license information please see main.2e9d1952.js.LICENSE.txt */
 (function() {
     var __webpack_modules__ = {
             4189: function(e, t) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 })
@@ -1525,17 +1525,17 @@
                     return t.set(e, n), n
                 }
             },
             7918: function(e, t, n) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
-                }), n(8679).__exportStar(n(5524), t)
+                }), n(8679).__exportStar(n(4325), t)
             },
-            5524: function(e, t, n) {
+            4325: function(e, t, n) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.supportsZeroByteGCM = t.supportsSubtleCrypto = t.supportsSecureRandom = t.supportsWebCrypto = void 0;
                 var r = n(8679),
                     o = ["decrypt", "digest", "encrypt", "exportKey", "generateKey", "importKey", "sign", "verify"];
 
@@ -9303,15 +9303,15 @@
                     i.default.get(n, (function(e, n) {
                         !e && n && n.entry && n.entry[0] ? t(null, n.entry[0].displayName) : t({})
                     }))
                 }, t.url = function(e, t) {
                     if (e = l(e), !(0, a.validateEmail)(e)) return t({});
                     t(null, "https://secure.gravatar.com/avatar/" + u(e) + "?d=404&s=160")
                 };
-                var r = s(n(8839)),
+                var r = s(n(5524)),
                     o = s(n(6070)),
                     i = s(n(1558)),
                     a = n(183);
 
                 function s(e) {
                     return e && e.__esModule ? e : {
                         default: e
@@ -25493,15 +25493,15 @@
 
                 function l(e, t, r) {
                     for (var o, i, a = [], s = t; s < r; s += 3) o = (e[s] << 16 & 16711680) + (e[s + 1] << 8 & 65280) + (255 & e[s + 2]), a.push(n[(i = o) >> 18 & 63] + n[i >> 12 & 63] + n[i >> 6 & 63] + n[63 & i]);
                     return a.join("")
                 }
                 r["-".charCodeAt(0)] = 62, r["_".charCodeAt(0)] = 63
             },
-            8839: function(e, t, n) {
+            5524: function(e, t, n) {
                 var r;
                 ! function(o) {
                     "use strict";
 
                     function i(e, t) {
                         var n = (65535 & e) + (65535 & t);
                         return (e >> 16) + (t >> 16) + (n >> 16) << 16 | 65535 & n
@@ -46508,14 +46508,18 @@
                         timeZoneName: "short"
                     }).replace(" at ", " | ");
                     var n = Ar().toLocaleDateString(void 0, {
                         timeZoneName: "short"
                     }).slice(-3);
                     return ("0" + e.getHours()).slice(-2) + ":" + ("0" + e.getMinutes()).slice(-2) + ":" + ("0" + e.getSeconds()).slice(-2) + " " + n
                 },
+                FromNow: function(e) {
+                    var t = !(arguments.length > 1 && void 0 !== arguments[1]) || arguments[1];
+                    return Or(Ar(), e, t, null, null, "from now")
+                },
                 ToDateTime: zr,
                 Now: function() {
                     return Ar()
                 }
             },
             Pr = Ur;
 
@@ -47077,14 +47081,15 @@
                 Diamond: String.fromCodePoint(10070),
                 Dot: String.fromCodePoint(8226),
                 DoNotEnter: String.fromCodePoint(8861),
                 DownArrow: String.fromCodePoint(8595),
                 DownArrowFat: String.fromCodePoint(9660),
                 DownArrowHollow: String.fromCodePoint(5121),
                 EmptySet: String.fromCodePoint(8709),
+                LeftArrow: String.fromCodePoint(8592),
                 RightArrow: String.fromCodePoint(8594),
                 RightArrowFat: String.fromCodePoint(9658),
                 RightArrowHollow: String.fromCodePoint(5125),
                 Refresh: String.fromCodePoint(8635),
                 Search: String.fromCodePoint(128269),
                 Star: String.fromCodePoint(10030),
                 UpArrow: String.fromCodePoint(8593),
@@ -56522,2598 +56527,41 @@
                         onData: function(e) {
                             return n(e)
                         },
                         cache: !0
                     })
                 }
             },
-            qa = function(e) {
-                var t, n, r = co(),
-                    o = Va(),
-                    i = so(Br.IsLoggedIn() ? zt.Url("/info") : null);
-                Hr.NoteLastUrl(r);
-                var a = fe();
-
-                function s() {
-                    return At.IsKnown(At.Current(), r)
-                }
-
-                function u(e) {
-                    return At.Equals(At.Current(), e)
-                }
-
-                function l(e) {
-                    return At.IsDefault(e, r)
-                }
-
-                function c() {
-                    return At.PreferredName(At.Default(r), r)
-                }
-
-                function d(e, t) {
-                    var n;
-                    if (!st.IsNonEmptyObject(t)) return "Fetching ...";
-                    var r = null === (n = t.known_envs) || void 0 === n ? void 0 : n.filter((function(t) {
-                        return At.Equals(t, e)
-                    }));
-                    return st.IsNonEmptyArray(r) && r[0].gac_name || "GAC name unknown"
-                }
-
-                function f(e, t) {
-                    var n;
-                    if (!st.IsNonEmptyObject(t)) return !1;
-                    var r = null === (n = t.known_envs) || void 0 === n ? void 0 : n.filter((function(t) {
-                        return At.Equals(t, e)
-                    }));
-                    return st.IsNonEmptyArray(r) && r[0].gac_name
-                }
-                var p = s() && At.IsAllowed(At.Current(), r) ? "box" : "box warning";
-
-                function h(e) {
-                    return {
-                        fontWeight: e === At.Current() ? "bold" : "inherit"
-                    }
-                }
-                return r.error ? (0, Fr.jsx)(Xi, {
-                    error: r.error,
-                    message: "Error loading users from Foursight API"
-                }) : r.loading ? (0, Fr.jsx)(Fr.Fragment, {
-                    children: "Loading ..."
-                }) : (0, Fr.jsx)("div", {
-                    children: (0, Fr.jsxs)("div", {
-                        className: "container",
-                        children: [!Br.IsLoggedIn(r) && s() ? (0, Fr.jsxs)("div", {
-                            className: "box warning",
-                            style: {
-                                margin: "0pt",
-                                padding: "10pt",
-                                marginBottom: "8pt"
-                            },
-                            children: [(0, Fr.jsx)("span", {
-                                className: "pointer",
-                                onClick: function() {
-                                    return a(kr.Path("/login?auth=1"))
-                                },
-                                style: {
-                                    fontSize: "large",
-                                    color: "inherit"
-                                },
-                                children: (0, Fr.jsxs)("b", {
-                                    children: [Do.Warning, "\xa0\xa0Not Logged In"]
-                                })
-                            }), " ", (0, Fr.jsx)("br", {}), (0, Fr.jsx)(Ji, {
-                                top: "6pt",
-                                bottom: "6pt"
-                            }), (0, Fr.jsxs)("small", {
-                                children: ["Click ", (0, Fr.jsx)(Oe, {
-                                    to: kr.Path("/login", !!s() || r, r),
-                                    style: {
-                                        cursor: "pointer",
-                                        color: "inherit"
-                                    },
-                                    children: (0, Fr.jsx)("b", {
-                                        children: (0, Fr.jsx)("u", {
-                                            children: "here"
-                                        })
-                                    })
-                                }), " to go to the ", (0, Fr.jsx)(Oe, {
-                                    to: kr.Path("/login", !!s() || r, r),
-                                    style: {
-                                        cursor: "pointer",
-                                        color: "inherit"
-                                    },
-                                    children: (0, Fr.jsx)("b", {
-                                        children: "login"
-                                    })
-                                }), " page."]
-                            })]
-                        }) : (0, Fr.jsx)("span", {}), (0, Fr.jsx)("b", {
-                            children: "Environment"
-                        }), s() ? (0, Fr.jsx)(Fr.Fragment, {
-                            children: (0, Fr.jsxs)("div", {
-                                className: p,
-                                style: {
-                                    marginBottom: "8pt",
-                                    padding: "10pt"
-                                },
-                                children: ["Current environment: ", (0, Fr.jsx)("b", {
-                                    children: At.PreferredName(At.Current(), r)
-                                }), Br.IsLoggedIn(r) && !At.IsAllowed(At.Current(), r) && (0, Fr.jsxs)("span", {
-                                    style: {
-                                        color: "red"
-                                    },
-                                    children: ["\xa0", (0, Fr.jsx)("b", {
-                                        children: Do.RightArrow
-                                    }), " You do not have permission for this environment ", (0, Fr.jsx)("b", {
-                                        children: Do.Warning
-                                    })]
-                                })]
-                            })
-                        }) : (0, Fr.jsx)(Fr.Fragment, {
-                            children: (0, Fr.jsxs)("div", {
-                                className: "box warning",
-                                style: {
-                                    marginBottom: "8pt",
-                                    padding: "10pt"
-                                },
-                                children: [At.Current() && "env" !== At.Current() ? (0, Fr.jsxs)(Fr.Fragment, {
-                                    children: ["Unknown environment: ", (0, Fr.jsx)("b", {
-                                        style: {
-                                            color: "darkred"
-                                        },
-                                        children: At.Current()
-                                    })]
-                                }) : (0, Fr.jsx)(Fr.Fragment, {
-                                    children: "No environment specified in URL!"
-                                }), (0, Fr.jsx)("br", {}), (0, Fr.jsxs)("small", {
-                                    children: ["Click ", (0, Fr.jsx)(Oe, {
-                                        to: kr.Path("/env", c()),
-                                        onClick: function() {
-                                            return o(c())
-                                        },
-                                        style: {
-                                            fontWeight: "bold",
-                                            color: "darkred"
-                                        },
-                                        children: "here"
-                                    }), " to use this default environment: \xa0", (0, Fr.jsx)(Oe, {
-                                        to: kr.Path("/env", c()),
-                                        onClick: function() {
-                                            return o(c())
-                                        },
-                                        style: {
-                                            fontWeight: "bold",
-                                            color: "darkred"
-                                        },
-                                        children: c()
-                                    })]
-                                })]
-                            })
-                        }), (0, Fr.jsx)("b", {
-                            children: "Available Environments"
-                        }), " ", (null === (t = r.auth) || void 0 === t ? void 0 : t.known_envs_actual_count) > (null === (n = At.KnownEnvs(r)) || void 0 === n ? void 0 : n.length) && (0, Fr.jsxs)("small", {
-                            children: ["\xa0(", r.auth.known_envs_actual_count, ")"]
-                        }), (0, Fr.jsx)("div", {
-                            className: p,
-                            style: {
-                                margin: "0pt",
-                                padding: "10pt"
-                            },
-                            children: (0, Fr.jsxs)("table", {
-                                style: {
-                                    color: "inherit"
-                                },
-                                children: [(0, Fr.jsx)("thead", {}), (0, Fr.jsx)("tbody", {
-                                    children: At.KnownEnvs(r).map((function(e, t) {
-                                        return (0, Fr.jsxs)("tr", {
-                                            children: [(0, Fr.jsxs)("td", {
-                                                style: {
-                                                    fontWeight: u(e) ? "bold" : "normal",
-                                                    color: s(e.public_name) ? u(e) ? "black" : "inherit" : "red",
-                                                    verticalAlign: "top"
-                                                },
-                                                children: [u(e) ? (0, Fr.jsx)(Fr.Fragment, {
-                                                    children: (0, Fr.jsxs)("span", {
-                                                        id: "tooltip-env-current-check",
-                                                        style: {
-                                                            color: Br.IsLoggedIn(r) && !At.IsAllowed(e, r) ? "red" : "inherit"
-                                                        },
-                                                        children: [Do.Check, "\xa0\xa0"]
-                                                    })
-                                                }) : (0, Fr.jsx)(Fr.Fragment, {
-                                                    children: (0, Fr.jsxs)("span", {
-                                                        style: {
-                                                            color: At.IsAllowed(e, r) ? "inherit" : "red"
-                                                        },
-                                                        children: [Do.Dot, "\xa0\xa0"]
-                                                    })
-                                                }), (0, Fr.jsx)(Yi, {
-                                                    id: "tooltip-env-current-check",
-                                                    position: "bottom",
-                                                    text: "This is your current environment."
-                                                })]
-                                            }), (0, Fr.jsxs)("td", {
-                                                children: [Br.IsLoggedIn(r) && !At.IsAllowed(e, r) ? (0, Fr.jsx)(Fr.Fragment, {
-                                                    children: (0, Fr.jsxs)("span", {
-                                                        style: {
-                                                            color: "red"
-                                                        },
-                                                        children: [(0, Fr.jsx)(Oe, {
-                                                            id: "tooltip-env-nopermission",
-                                                            to: kr.Path("/env", At.PreferredName(e, r)),
-                                                            onClick: function() {
-                                                                return o(At.PreferredName(e, r))
-                                                            },
-                                                            style: {
-                                                                color: "inherit",
-                                                                textDecoration: u(e) ? "underline" : "normal"
-                                                            },
-                                                            children: (0, Fr.jsx)("b", {
-                                                                children: At.PreferredName(e, r)
-                                                            })
-                                                        }), l(e) && (0, Fr.jsxs)("span", {
-                                                            style: {
-                                                                color: "black"
-                                                            },
-                                                            children: ["\xa0", (0, Fr.jsx)("b", {
-                                                                children: Do.RightArrow
-                                                            }), "This is the default environment ", Do.Star]
-                                                        }), "\xa0", (0, Fr.jsx)("b", {
-                                                            children: Do.RightArrow
-                                                        }), " You do not have permission for this environment ", (0, Fr.jsx)("b", {
-                                                            children: Do.Warning
-                                                        }), (0, Fr.jsx)(Yi, {
-                                                            id: "tooltip-env-nopermission",
-                                                            position: "bottom",
-                                                            text: "You do not have permission for this environment."
-                                                        })]
-                                                    })
-                                                }) : (0, Fr.jsx)(Fr.Fragment, {
-                                                    children: u(e) ? (0, Fr.jsxs)(Fr.Fragment, {
-                                                        children: [(0, Fr.jsxs)("span", {
-                                                            style: {
-                                                                color: "black"
-                                                            },
-                                                            children: [(0, Fr.jsx)(Oe, {
-                                                                id: u(e) ? "tooltip-env-current" : "",
-                                                                to: kr.Path("/env", At.PreferredName(e, r)),
-                                                                onClick: function() {
-                                                                    return o(At.PreferredName(e, r))
-                                                                },
-                                                                style: {
-                                                                    color: "inherit"
-                                                                },
-                                                                children: (0, Fr.jsx)("b", {
-                                                                    children: (0, Fr.jsx)("u", {
-                                                                        children: At.PreferredName(e, r)
-                                                                    })
-                                                                })
-                                                            }), l(e) && (0, Fr.jsxs)("span", {
-                                                                children: ["\xa0", (0, Fr.jsx)("b", {
-                                                                    children: Do.RightArrow
-                                                                }), " This is the default environment ", Do.Star]
-                                                            })]
-                                                        }), (0, Fr.jsx)(Yi, {
-                                                            id: "tooltip-env-current",
-                                                            position: "bottom",
-                                                            text: "This is your current environment."
-                                                        })]
-                                                    }) : (0, Fr.jsx)(Fr.Fragment, {
-                                                        children: (0, Fr.jsxs)("span", {
-                                                            children: [(0, Fr.jsx)(Oe, {
-                                                                id: "tooltip-env-default-".concat(e.full_name),
-                                                                to: kr.Path("/env", At.PreferredName(e, r)),
-                                                                onClick: function() {
-                                                                    return o(At.PreferredName(e, r))
-                                                                },
-                                                                style: {
-                                                                    color: "inherit"
-                                                                },
-                                                                children: (0, Fr.jsx)("b", {
-                                                                    children: At.PreferredName(e, r)
-                                                                })
-                                                            }), l(e) && (0, Fr.jsxs)("span", {
-                                                                style: {
-                                                                    color: "black"
-                                                                },
-                                                                children: ["\xa0", (0, Fr.jsx)("b", {
-                                                                    children: Do.RightArrow
-                                                                }), " This is the default environment ", Do.Star]
-                                                            }), (0, Fr.jsx)(Yi, {
-                                                                id: "tooltip-env-default-".concat(e.full_name),
-                                                                position: "top",
-                                                                text: "This is the default environment."
-                                                            })]
-                                                        })
-                                                    })
-                                                }), (0, Fr.jsx)("br", {}), "Full Name: ", (0, Fr.jsx)("span", {
-                                                    style: h(e.full_name),
-                                                    children: e.full_name
-                                                }), " ", (0, Fr.jsx)("br", {}), "Short Name: ", (0, Fr.jsx)("span", {
-                                                    style: h(e.short_name),
-                                                    children: e.short_name
-                                                }), " ", (0, Fr.jsx)("br", {}), "Public Name: ", (0, Fr.jsx)("span", {
-                                                    style: h(e.public_name),
-                                                    children: e.public_name
-                                                }), " ", (0, Fr.jsx)("br", {}), Br.IsLoggedIn() && (0, Fr.jsxs)(Fr.Fragment, {
-                                                    children: ["GAC Name: ", d(e, i.data), " ", (0, Fr.jsx)("br", {}), s() && f(e, i.data) && (0, Fr.jsxs)(Fr.Fragment, {
-                                                        children: [(0, Fr.jsxs)("select", {
-                                                            style: {
-                                                                border: "0",
-                                                                background: "transparent",
-                                                                WebkitAppearance: "none"
-                                                            },
-                                                            onChange: function(t) {
-                                                                return function(e, t) {
-                                                                    var n = e.target.value;
-                                                                    a(kr.Path("/gac/" + n, t))
-                                                                }(t, At.PreferredName(e, r))
-                                                            },
-                                                            children: [(0, Fr.jsxs)("option", {
-                                                                children: ["GAC Compare ", Do.DownArrow]
-                                                            }), At.KnownEnvs(r).map((function(e) {
-                                                                return (0, Fr.jsx)("option", {
-                                                                    children: At.PreferredName(e, r)
-                                                                }, Dr()())
-                                                            }))]
-                                                        }), (0, Fr.jsx)("br", {})]
-                                                    }), t < At.KnownEnvs(r).length - 1 && (0, Fr.jsx)("br", {})]
-                                                })]
-                                            })]
-                                        }, Dr()())
-                                    }))
-                                })]
-                            })
-                        }), Br.IsLoggedIn(r) && (0, Fr.jsx)("div", {
-                            style: {
-                                marginTop: "8pt"
-                            }
-                        })]
-                    })
-                })
-            },
-            Ja = function(e) {
-                var t = co();
-                return t.loading ? null : (0, Fr.jsxs)(Fr.Fragment, {
-                    children: [(0, Fr.jsx)("br", {}), (0, Fr.jsx)("table", {
-                        width: "100%",
-                        children: (0, Fr.jsxs)("tbody", {
-                            children: [(0, Fr.jsx)("tr", {
-                                style: {
-                                    backgroundColor: "darkred",
-                                    height: "1px"
-                                },
-                                children: (0, Fr.jsx)("td", {})
-                            }), (0, Fr.jsx)("tr", {
-                                children: (0, Fr.jsx)("td", {
-                                    align: "center",
-                                    style: {
-                                        paddingTop: "2px",
-                                        paddingBottom: "6px"
-                                    },
-                                    children: (0, Fr.jsx)("a", {
-                                        href: kr.PortalLink(t),
-                                        target: "_blank",
-                                        rel: "noreferrer",
-                                        children: (0, Fr.jsx)("img", {
-                                            alt: "harvard",
-                                            src: Ut.Harvard(),
-                                            height: "46"
-                                        })
-                                    })
-                                })
-                            }), (0, Fr.jsx)("tr", {
-                                style: {
-                                    backgroundColor: "darkred",
-                                    height: "1px"
-                                },
-                                children: (0, Fr.jsx)("td", {})
-                            })]
-                        })
-                    })]
-                })
-            },
-            Ka = function(e) {
-                var t = co();
-                return (0, Fr.jsx)(Fr.Fragment, {
-                    children: (0, Fr.jsx)("div", {
-                        className: "container",
-                        id: "login_container",
-                        children: (0, Fr.jsxs)("div", {
-                            className: "boxstyle check-error",
-                            style: {
-                                margin: "20pt",
-                                padding: "10pt"
-                            },
-                            children: [(0, Fr.jsx)("b", {
-                                children: "Forbidden response from server."
-                            }), ".  ", (0, Fr.jsx)("br", {}), "You seem to be logged in but the server does not seem to think so. ", (0, Fr.jsx)("br", {}), "Try ", (0, Fr.jsx)("span", {
-                                onClick: function() {
-                                    return Zr()
-                                },
-                                style: {
-                                    cursor: "pointer"
-                                },
-                                children: (0, Fr.jsx)("u", {
-                                    children: "logging out"
-                                })
-                            }), " and logging in again.", (0, Fr.jsx)("br", {}), (0, Fr.jsxs)("small", {
-                                children: ["Click ", (0, Fr.jsx)(Oe, {
-                                    to: kr.Path("/login", At.Current(t)),
-                                    style: {
-                                        color: "darkred"
-                                    },
-                                    children: (0, Fr.jsx)("b", {
-                                        children: "here"
-                                    })
-                                }), " to go to the ", (0, Fr.jsx)(Oe, {
-                                    to: kr.Path("/login", At.Current(t)),
-                                    children: (0, Fr.jsx)("b", {
-                                        style: {
-                                            color: "darkred"
-                                        },
-                                        children: "login"
-                                    })
-                                }), " page."]
-                            })]
-                        })
-                    })
-                })
-            },
-            Xa = function() {
-                var e = a(ra(), 2),
-                    t = e[0],
-                    n = e[1];
-                return (0, Fr.jsxs)(Fr.Fragment, {
-                    children: [(0, Fr.jsx)("img", {
-                        id: "tooltip-readonly",
-                        alt: "lock",
-                        src: t ? Ut.Lock() : Ut.Unlock(),
-                        style: {
-                            height: "35",
-                            cursor: "pointer"
-                        },
-                        onClick: function() {
-                            return n(!t)
-                        }
-                    }), (0, Fr.jsx)(Yi, {
-                        id: "tooltip-readonly",
-                        position: "bottom",
-                        text: "You are in ".concat(t ? "readonly" : "read/write", " mode. Click to enter ").concat(t ? "read/write" : "readonly", " mode.")
-                    })]
-                })
-            },
-            $a = function(e) {
-                var t = e.header,
-                    n = Ft.LightenDarkenColor(Ft.GetBackgroundColor(), -10),
-                    r = function(e) {
-                        var t = e.path,
-                            n = e.label;
-                        return (0, Fr.jsx)(Fr.Fragment, {
-                            children: kr.CurrentLogicalPath() === t ? (0, Fr.jsxs)("span", {
-                                style: {
-                                    fontWeight: "bold"
-                                },
-                                children: [n, "\xa0", Do.Check]
-                            }) : (0, Fr.jsx)(Oe, {
-                                to: kr.Path(t),
-                                children: n
-                            }, t)
-                        })
-                    },
-                    o = function() {
-                        return (0, Fr.jsx)("div", {
-                            style: {
-                                height: "1px",
-                                marginTop: "1pt",
-                                marginBottom: "1pt",
-                                marginLeft: "6pt",
-                                marginRight: "6pt",
-                                background: "var(--box-fg)"
-                            }
-                        })
-                    };
-                return (0, Fr.jsx)(Fr.Fragment, {
-                    children: (0, Fr.jsxs)("span", {
-                        className: "dropdown",
-                        children: [(0, Fr.jsx)("span", {
-                            className: "dropdown-button",
-                            children: (0, Fr.jsx)("img", {
-                                alt: "menu",
-                                style: {
-                                    marginLeft: "-4px",
-                                    marginTop: "-1px"
-                                },
-                                src: Ut.MenuIcon(),
-                                height: "20"
-                            })
-                        }), (0, Fr.jsxs)("div", {
-                            className: "dropdown-content",
-                            id: "dropdown-content-id",
-                            style: {
-                                background: n
-                            },
-                            children: [(0, Fr.jsx)(r, {
-                                path: "/home",
-                                label: "Home"
-                            }), (0, Fr.jsx)(r, {
-                                path: "/info",
-                                label: "General Info"
-                            }), (0, Fr.jsx)(r, {
-                                path: "/checks",
-                                label: "Checks"
-                            }), (0, Fr.jsx)(o, {}), (0, Fr.jsx)(r, {
-                                path: "/aws/infrastructure",
-                                label: "Infrastructure"
-                            }), (0, Fr.jsx)(r, {
-                                path: "/aws/s3",
-                                label: "S3"
-                            }), (0, Fr.jsx)(r, {
-                                path: "/users",
-                                label: "Users"
-                            }), (0, Fr.jsx)(o, {}), (0, Fr.jsx)(r, {
-                                path: "/env",
-                                label: "Environments"
-                            }), (0, Fr.jsx)(r, {
-                                path: "/accounts",
-                                label: "Accounts"
-                            }), (0, Fr.jsx)(r, {
-                                path: "/login",
-                                label: Br.IsLoggedIn(t) ? "Session" : "Login"
-                            })]
-                        })]
-                    })
-                })
-            },
-            es = function(e) {
-                var t, n, r, o, i = e.header;
-
-                function a(e) {
-                    return e ? {
-                        textDecoration: "none",
-                        color: "black",
-                        fontWeight: "bold"
-                    } : {
-                        textDecoration: "none",
-                        color: Ft.GetForegroundColor(),
-                        fontWeight: "normal"
-                    }
-                }
-                return (0, Fr.jsxs)(Fr.Fragment, {
-                    children: [(0, Fr.jsx)(ze, {
-                        to: kr.Path("/home"),
-                        style: function(e) {
-                            return a(e.isActive)
-                        },
-                        children: "HOME"
-                    }), "\xa0|\xa0", (0, Fr.jsx)(ze, {
-                        to: kr.Path("/info"),
-                        style: function(e) {
-                            return a(e.isActive)
-                        },
-                        children: "INFO"
-                    }), "\xa0|\xa0", (0, Fr.jsx)(ze, {
-                        to: kr.Path("/checks"),
-                        style: function(e) {
-                            return a(e.isActive)
-                        },
-                        children: "CHECKS"
-                    }), "\xa0|\xa0", (0, Fr.jsx)(ze, {
-                        to: kr.Path("/env"),
-                        style: function(e) {
-                            return a(e.isActive)
-                        },
-                        children: "ENV"
-                    }), "\xa0|\xa0", (0, Fr.jsxs)("a", {
-                        target: "_blank",
-                        rel: "noreferrer",
-                        id: "tooltip-header-portal",
-                        style: {
-                            textDecoration: "none",
-                            color: "darkgreen"
-                        },
-                        href: kr.PortalLink(i),
-                        children: ["PORTAL ", (0, Fr.jsx)("span", {
-                            className: "fa fa-external-link",
-                            style: {
-                                position: "relative",
-                                bottom: "-1px",
-                                fontSize: "14px"
-                            }
-                        })]
-                    }), "\xa0|\xa0", (0, Fr.jsxs)("a", {
-                        target: "_blank",
-                        rel: "noreferrer",
-                        id: "tooltip-header-aws",
-                        style: {
-                            textDecoration: "none",
-                            color: "darkgreen"
-                        },
-                        href: "https://" + (null === (t = i.app) || void 0 === t ? void 0 : t.credentials.aws_account_number) + ".signin.aws.amazon.com/console/",
-                        children: ["AWS ", (0, Fr.jsx)("span", {
-                            className: "fa fa-external-link",
-                            style: {
-                                position: "relative",
-                                bottom: "-1px",
-                                fontSize: "14px"
-                            }
-                        })]
-                    }), (0, Fr.jsx)(Yi, {
-                        id: "tooltip-header-portal",
-                        position: "bottom",
-                        text: "Open portal (in new tab)."
-                    }), (0, Fr.jsx)(Yi, {
-                        id: "tooltip-header-aws",
-                        position: "bottom",
-                        text: "Open AWS console for (".concat(null !== (n = i.app) && void 0 !== n && n.credentials.aws_account_name ? (null === (r = i.app) || void 0 === r ? void 0 : r.credentials.aws_account_name) + "/" : "").concat(null === (o = i.app) || void 0 === o ? void 0 : o.credentials.aws_account_number, ") account (in new tab).")
-                    })]
-                })
-            },
-            ts = function(e) {
-                var t = e.header;
-                return (0, Fr.jsxs)("span", {
-                    children: [(0, Fr.jsx)($a, {
-                        header: t
-                    }), (0, Fr.jsx)(Fr.Fragment, {
-                        children: "\xa0|\xa0"
-                    }), (0, Fr.jsx)(es, {
-                        header: t
-                    })]
-                })
-            },
-            ns = function(e) {
-                var n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, w, j, x, N, I, D, S, L, k = co(),
-                    C = Va(),
-                    E = fe(),
-                    _ = a(So(), 1)[0],
-                    T = At.IsFoursightFourfront(k) ? "#14533C" : "#143C53",
-                    A = Ft.LightenDarkenColor(Ft.GetBackgroundColor(), -10);
-                return (0, Fr.jsx)(Fr.Fragment, {
-                    children: k.loading ? (0, Fr.jsxs)("div", {
-                        style: {
-                            width: "100%"
-                        },
-                        children: [(0, Fr.jsx)("table", {
-                            style: {
-                                width: "100%",
-                                height: "42px",
-                                background: Br.IsLoggedIn(k) ? T : "#444444"
-                            },
-                            children: (0, Fr.jsx)("tbody", {
-                                children: (0, Fr.jsxs)("tr", {
-                                    children: [(0, Fr.jsx)("td", {
-                                        width: "1%",
-                                        style: {
-                                            height: "42px",
-                                            paddingLeft: "2pt",
-                                            whiteSpace: "nowrap"
-                                        },
-                                        children: (0, Fr.jsx)("div", {
-                                            style: {
-                                                width: "200px"
-                                            }
-                                        })
-                                    }), (0, Fr.jsx)("td", {
-                                        width: "98%",
-                                        align: "center",
-                                        style: {
-                                            fontSize: "16pt",
-                                            color: "white",
-                                            nowrap: "1"
-                                        },
-                                        children: k.error ? (0, Fr.jsx)("span", {
-                                            children: (0, Fr.jsx)("b", {
-                                                style: {
-                                                    color: "red"
-                                                },
-                                                children: "Foursight Load Error"
-                                            })
-                                        }) : (0, Fr.jsx)("span", {
-                                            children: (0, Fr.jsx)("i", {
-                                                style: {
-                                                    color: "yellow"
-                                                },
-                                                children: "Foursight Loading ..."
-                                            })
-                                        })
-                                    }), (0, Fr.jsx)("td", {
-                                        width: "1%",
-                                        align: "right",
-                                        children: (0, Fr.jsxs)("span", {
-                                            style: {
-                                                position: "relative",
-                                                bottom: "5pt"
-                                            },
-                                            children: ["\xa0", (0, Fr.jsx)(wo, {
-                                                loading: k.loading && !k.error,
-                                                color: "yellow",
-                                                size: 150,
-                                                style: {
-                                                    marginRight: "20px"
-                                                }
-                                            })]
-                                        })
-                                    })]
-                                })
-                            })
-                        }), (0, Fr.jsx)("table", {
-                            style: {
-                                width: "100%",
-                                height: "22px",
-                                background: "lightgray"
-                            },
-                            children: (0, Fr.jsxs)("tbody", {
-                                children: [(0, Fr.jsx)("tr", {
-                                    children: (0, Fr.jsx)("td", {
-                                        style: {
-                                            height: "27px",
-                                            paddingLeft: "2pt",
-                                            whiteSpace: "nowrap",
-                                            background: "lightgray"
-                                        }
-                                    })
-                                }), (0, Fr.jsx)("tr", {
-                                    children: (0, Fr.jsx)("td", {
-                                        style: {
-                                            height: "20px",
-                                            paddingLeft: "2pt",
-                                            whiteSpace: "nowrap",
-                                            background: "lightyellow"
-                                        }
-                                    })
-                                })]
-                            })
-                        })]
-                    }) : (0, Fr.jsxs)(t.Fragment, {
-                        children: [(0, Fr.jsxs)("div", {
-                            style: {
-                                width: "100%",
-                                background: T
-                            },
-                            children: [(0, Fr.jsx)("table", {
-                                width: "100%",
-                                cellPadding: "0",
-                                cellSpacing: "0",
-                                children: (0, Fr.jsx)("tbody", {
-                                    children: (0, Fr.jsxs)("tr", {
-                                        children: [(0, Fr.jsx)("td", {
-                                            width: "38%",
-                                            style: {
-                                                paddingLeft: "2pt",
-                                                whiteSpace: "nowrap"
-                                            },
-                                            children: (0, Fr.jsx)("a", {
-                                                href: kr.PortalLink(k),
-                                                target: "_blank",
-                                                rel: "noreferrer",
-                                                children: At.IsFoursightFourfront(k) ? (0, Fr.jsx)("span", {
-                                                    children: (0, Fr.jsx)("img", {
-                                                        alt: "foursight",
-                                                        style: {
-                                                            marginLeft: "14px",
-                                                            marginTop: "5px",
-                                                            marginBottom: "5px"
-                                                        },
-                                                        src: Ut.FoursightFourfrontLogo(),
-                                                        height: "32",
-                                                        width: "44"
-                                                    })
-                                                }) : (0, Fr.jsx)("span", {
-                                                    children: (0, Fr.jsx)("img", {
-                                                        alt: "foursight",
-                                                        src: Ut.FoursightCgapLogo(),
-                                                        width: "130"
-                                                    })
-                                                })
-                                            })
-                                        }), (0, Fr.jsx)("td", {
-                                            width: "24%",
-                                            align: "center",
-                                            style: {
-                                                whiteSpace: "nowrap"
-                                            },
-                                            children: (0, Fr.jsx)("div", {
-                                                style: {
-                                                    fontSize: "20pt",
-                                                    color: "white",
-                                                    cursor: "pointer"
-                                                },
-                                                onClick: function() {
-                                                    return E(kr.Path("/home"))
-                                                },
-                                                children: "dev" === (null === (n = k.app) || void 0 === n ? void 0 : n.stage) ? (0, Fr.jsx)(Fr.Fragment, {
-                                                    children: null !== (r = k.app) && void 0 !== r && r.local ? (0, Fr.jsxs)(Fr.Fragment, {
-                                                        children: [(0, Fr.jsx)("span", {
-                                                            title: "Running locally.",
-                                                            style: {
-                                                                position: "relative",
-                                                                bottom: "3pt",
-                                                                color: "yellow",
-                                                                fontSize: "17pt"
-                                                            },
-                                                            children: Do.DoNotEnter
-                                                        }), "\xa0", (0, Fr.jsx)("span", {
-                                                            title: "Stage is DEV. Running locally",
-                                                            style: {
-                                                                position: "relative",
-                                                                bottom: "1pt",
-                                                                color: "yellow",
-                                                                fontSize: "26pt"
-                                                            },
-                                                            children: Do.Atom
-                                                        }), "\xa0\xa0", (0, Fr.jsx)("span", {
-                                                            className: "title-font",
-                                                            style: {
-                                                                position: "relative",
-                                                                bottom: "3pt",
-                                                                color: "white",
-                                                                fontWeight: "bold"
-                                                            },
-                                                            children: null === (o = k.app) || void 0 === o ? void 0 : o.title.toUpperCase()
-                                                        }), "\xa0\xa0", (0, Fr.jsx)("span", {
-                                                            title: "Stage is DEV. Running locally",
-                                                            style: {
-                                                                position: "relative",
-                                                                bottom: "1pt",
-                                                                color: "yellow",
-                                                                fontSize: "24pt"
-                                                            },
-                                                            children: Do.Atom
-                                                        }), "\xa0", (0, Fr.jsx)("span", {
-                                                            title: "Running locally.",
-                                                            style: {
-                                                                position: "relative",
-                                                                bottom: "3pt",
-                                                                color: "yellow",
-                                                                fontSize: "17pt"
-                                                            },
-                                                            children: Do.DoNotEnter
-                                                        }), "\xa0\xa0"]
-                                                    }) : (0, Fr.jsxs)(Fr.Fragment, {
-                                                        children: [(0, Fr.jsx)("span", {
-                                                            title: "Stage is DEV.",
-                                                            style: {
-                                                                position: "relative",
-                                                                bottom: "1pt",
-                                                                color: "yellow",
-                                                                fontSize: "24pt"
-                                                            },
-                                                            children: Do.Atom
-                                                        }), "\xa0\xa0", (0, Fr.jsx)("span", {
-                                                            className: "title-font",
-                                                            style: {
-                                                                position: "relative",
-                                                                bottom: "2pt",
-                                                                color: "white",
-                                                                fontWeight: "bold"
-                                                            },
-                                                            children: null === (i = k.app) || void 0 === i ? void 0 : i.title.toUpperCase()
-                                                        }), "\xa0\xa0", (0, Fr.jsx)("span", {
-                                                            title: "Stage is DEV.",
-                                                            style: {
-                                                                position: "relative",
-                                                                bottom: "1pt",
-                                                                color: "yellow",
-                                                                fontSize: "24pt"
-                                                            },
-                                                            children: Do.Atom
-                                                        }), "\xa0"]
-                                                    })
-                                                }) : (0, Fr.jsx)(Fr.Fragment, {
-                                                    children: null !== (s = k.app) && void 0 !== s && s.local ? (0, Fr.jsxs)(Fr.Fragment, {
-                                                        children: [(0, Fr.jsx)("span", {
-                                                            title: "Running locally.",
-                                                            style: {
-                                                                position: "relative",
-                                                                bottom: "2pt",
-                                                                color: "yellow",
-                                                                fontSize: "17pt"
-                                                            },
-                                                            children: Do.DoNotEnter
-                                                        }), "\xa0\xa0", (0, Fr.jsx)("span", {
-                                                            className: "title-font",
-                                                            style: {
-                                                                position: "relative",
-                                                                bottom: "1pt",
-                                                                color: "white",
-                                                                fontWeight: "bold"
-                                                            },
-                                                            children: null === (u = k.app) || void 0 === u ? void 0 : u.title.toUpperCase()
-                                                        }), "\xa0\xa0", (0, Fr.jsx)("span", {
-                                                            title: "Running locally.",
-                                                            style: {
-                                                                position: "relative",
-                                                                bottom: "2pt",
-                                                                color: "yellow",
-                                                                fontSize: "17pt"
-                                                            },
-                                                            children: Do.DoNotEnter
-                                                        }), "\xa0\xa0"]
-                                                    }) : (0, Fr.jsxs)(Fr.Fragment, {
-                                                        children: [(0, Fr.jsx)("span", {
-                                                            className: "title-font",
-                                                            style: {
-                                                                position: "relative",
-                                                                bottom: "1pt",
-                                                                color: "white",
-                                                                fontWeight: "bold"
-                                                            },
-                                                            children: null === (l = k.app) || void 0 === l ? void 0 : l.title.toUpperCase()
-                                                        }), "\xa0\xa0"]
-                                                    })
-                                                })
-                                            })
-                                        }), (0, Fr.jsxs)("td", {
-                                            width: "38%",
-                                            style: {
-                                                paddingRight: "10pt",
-                                                whiteSpace: "nowrap",
-                                                color: "#D6EAF8"
-                                            },
-                                            align: "right",
-                                            children: [(0, Fr.jsx)("small", {
-                                                children: (0, Fr.jsx)(aa.FormatDateTime, {
-                                                    verbose: !0,
-                                                    timezone: !1
-                                                })
-                                            }), (null === (c = k.app) || void 0 === c || null === (d = c.credentials) || void 0 === d ? void 0 : d.aws_account_name) && (0, Fr.jsxs)(Fr.Fragment, {
-                                                children: ["\xa0|\xa0", (0, Fr.jsx)(Oe, {
-                                                    id: "tooltip-header-account",
-                                                    to: kr.Path("/login"),
-                                                    style: {
-                                                        textDecoration: "none",
-                                                        color: "inherit"
-                                                    },
-                                                    children: (0, Fr.jsx)("b", {
-                                                        children: null === (f = k.app) || void 0 === f || null === (p = f.credentials) || void 0 === p || null === (h = p.aws_account_name) || void 0 === h ? void 0 : h.replace(/^cgap-/, "")
-                                                    })
-                                                }), (0, Fr.jsx)(Yi, {
-                                                    id: "tooltip-header-account",
-                                                    position: "bottom",
-                                                    text: "AWS account number: ".concat(null === (g = k.app) || void 0 === g || null === (y = g.credentials) || void 0 === y ? void 0 : y.aws_account_number)
-                                                })]
-                                            }), Br.IsLoggedIn(k) ? (0, Fr.jsxs)("span", {
-                                                children: ["\xa0|\xa0", (0, Fr.jsx)("span", {
-                                                    style: {
-                                                        cursor: "pointer",
-                                                        color: "#D6EAF8"
-                                                    },
-                                                    onClick: function() {
-                                                        return Zr()
-                                                    },
-                                                    children: "LOGOUT"
-                                                })]
-                                            }) : (0, Fr.jsxs)("span", {
-                                                children: ["\xa0|\xa0", (0, Fr.jsx)(Oe, {
-                                                    to: kr.Path("/login?auth", At.Current(k)),
-                                                    style: {
-                                                        cursor: "pointer",
-                                                        color: "#D6EAF8"
-                                                    },
-                                                    id: "tooltip-header-nologin",
-                                                    children: "LOGIN"
-                                                }), (0, Fr.jsx)(Yi, {
-                                                    id: "tooltip-header-nologin",
-                                                    position: "bottom",
-                                                    text: "Not logged in. Click to login."
-                                                })]
-                                            })]
-                                        })]
-                                    })
-                                })
-                            }), (0, Fr.jsx)("table", {
-                                width: "100%",
-                                cellPadding: "0",
-                                cellSpacing: "0",
-                                children: (0, Fr.jsxs)("tbody", {
-                                    children: [(0, Fr.jsxs)("tr", {
-                                        style: {
-                                            background: A
-                                        },
-                                        children: [(0, Fr.jsx)("td", {
-                                            width: "49%",
-                                            style: {
-                                                paddingLeft: "10pt",
-                                                paddingTop: "3pt",
-                                                paddingBottom: "3pt",
-                                                whiteSpace: "nowrap"
-                                            },
-                                            children: (0, Fr.jsx)(ts, {
-                                                header: k
-                                            })
-                                        }), (0, Fr.jsx)("td", {
-                                            width: "2%",
-                                            align: "center",
-                                            style: {
-                                                whiteSpace: "nowrap",
-                                                margin: "0 auto"
-                                            },
-                                            children: (0, Fr.jsxs)("a", {
-                                                target: "_blank",
-                                                rel: "noreferrer",
-                                                href: "https://pypi.org/project/" + (At.IsFoursightFourfront(k) ? "foursight" : "foursight-cgap") + "/" + (null === (m = k.app) || void 0 === m ? void 0 : m.version) + "/",
-                                                children: [(0, Fr.jsx)("b", {
-                                                    style: {
-                                                        textDecoration: "none",
-                                                        color: "#263A48",
-                                                        paddingRight: "8pt"
-                                                    },
-                                                    id: "tooltip-header-version",
-                                                    children: null === (v = k.app) || void 0 === v ? void 0 : v.version
-                                                }), (0, Fr.jsx)(Yi, {
-                                                    id: "tooltip-header-version",
-                                                    position: "bottom",
-                                                    text: (null !== (M = k.app) && void 0 !== M && M.deployed ? "Deployed: ".concat(null === (b = k.app) || void 0 === b ? void 0 : b.deployed, ". ") : "") + "Launched: " + (null === (w = k.app) || void 0 === w ? void 0 : w.launched),
-                                                    size: "x-small"
-                                                })]
-                                            })
-                                        }), (0, Fr.jsxs)("td", {
-                                            width: "49%",
-                                            style: {
-                                                paddingRight: "10pt",
-                                                paddingTop: "2pt",
-                                                paddingBottom: "1pt",
-                                                whiteSpace: "nowrap"
-                                            },
-                                            align: "right",
-                                            nowrap: "1",
-                                            children: ["cognito" !== At.Current() && At.KnownEnvs(k).length > 0 ? (0, Fr.jsxs)(Fr.Fragment, {
-                                                children: [(0, Fr.jsxs)("span", {
-                                                    className: "dropdown",
-                                                    children: [(0, Fr.jsx)(Yi, {
-                                                        id: "tooltip-header-env",
-                                                        position: "left",
-                                                        size: "small",
-                                                        text: "Environments",
-                                                        shape: "squared",
-                                                        nopad: !0
-                                                    }), (0, Fr.jsx)("b", {
-                                                        id: "tooltip-header-env",
-                                                        className: "dropdown-button",
-                                                        style: {
-                                                            color: !At.IsKnown(At.Current(), k) || Br.IsLoggedIn(k) && !At.IsAllowed(At.Current(), k) ? "red" : "#143c53"
-                                                        },
-                                                        children: At.Current() || "unknown-env"
-                                                    }), (0, Fr.jsxs)("div", {
-                                                        className: "dropdown-content",
-                                                        id: "dropdown-content-id",
-                                                        style: {
-                                                            background: A
-                                                        },
-                                                        children: [At.KnownEnvs(k).map((function(e) {
-                                                            return At.Equals(e, At.Current()) ? (0, Fr.jsxs)("span", {
-                                                                children: [At.PreferredName(e, k), "\xa0\xa0", Do.Check, !At.IsAllowed(e, k) && Br.IsLoggedIn(k) && (0, Fr.jsxs)(Fr.Fragment, {
-                                                                    children: ["\xa0\xa0", Do.Warning]
-                                                                })]
-                                                            }, e.full_name) : At.IsAllowed(e, k) ? (0, Fr.jsx)(Oe, {
-                                                                onClick: function() {
-                                                                    return C(At.PreferredName(e))
-                                                                },
-                                                                to: {
-                                                                    pathname: "/redirect"
-                                                                },
-                                                                state: {
-                                                                    url: At.IsKnown(At.Current(), k) ? kr.Path(null, At.PreferredName(e, k)) : kr.Path("/env", At.PreferredName(At.Default(k), k))
-                                                                },
-                                                                children: At.PreferredName(e, k)
-                                                            }, e.full_name) : (0, Fr.jsxs)(Oe, {
-                                                                to: kr.Path("/env", At.PreferredName(e, k)),
-                                                                children: [At.PreferredName(e, k), !At.IsAllowed(e, k) && Br.IsLoggedIn(k) && (0, Fr.jsxs)(Fr.Fragment, {
-                                                                    children: ["\xa0\xa0", Do.Warning]
-                                                                })]
-                                                            }, e.public_name)
-                                                        })), (0, Fr.jsx)("div", {
-                                                            height: "1",
-                                                            style: {
-                                                                marginTop: "2px",
-                                                                height: "1px",
-                                                                background: "darkblue"
-                                                            }
-                                                        }), (0, Fr.jsx)(Oe, {
-                                                            id: "__envinfo__",
-                                                            to: kr.Path("/env"),
-                                                            onClick: function() {
-                                                                document.getElementById("__envinfo__").style.fontWeight = "normal"
-                                                            },
-                                                            children: "Environments"
-                                                        })]
-                                                    })]
-                                                }), "\xa0|\xa0"]
-                                            }) : (0, Fr.jsx)(Fr.Fragment, {
-                                                children: "cognito" !== At.Current() ? (0, Fr.jsxs)(Fr.Fragment, {
-                                                    children: [(0, Fr.jsx)("b", {
-                                                        style: {
-                                                            color: T
-                                                        },
-                                                        children: At.Current()
-                                                    }), "\xa0|\xa0"]
-                                                }) : (0, Fr.jsx)(Fr.Fragment, {
-                                                    children: (0, Fr.jsx)("b", {
-                                                        style: {
-                                                            color: T
-                                                        },
-                                                        children: At.PreferredName(At.Default(k))
-                                                    })
-                                                })
-                                            }), "prod" === (null === (j = k.app) || void 0 === j ? void 0 : j.stage) ? (0, Fr.jsxs)(Fr.Fragment, {
-                                                children: [(0, Fr.jsx)("b", {
-                                                    id: "tooltip-header-stage-prod",
-                                                    style: {
-                                                        color: "darkred"
-                                                    },
-                                                    children: null === (x = k.app) || void 0 === x ? void 0 : x.stage
-                                                }), " \xa0|\xa0", (0, Fr.jsx)(Yi, {
-                                                    id: "tooltip-header-stage-prod",
-                                                    position: "bottom",
-                                                    text: "Deployment stage: PROD"
-                                                })]
-                                            }) : (0, Fr.jsx)(Fr.Fragment, {}), "dev" === (null === (N = k.app) || void 0 === N ? void 0 : N.stage) ? (0, Fr.jsxs)(Fr.Fragment, {
-                                                children: [(0, Fr.jsx)("b", {
-                                                    id: "tooltip-header-stage-dev",
-                                                    style: {
-                                                        color: "darkgreen"
-                                                    },
-                                                    children: null === (I = k.app) || void 0 === I ? void 0 : I.stage
-                                                }), " \xa0|\xa0", (0, Fr.jsx)(Yi, {
-                                                    id: "tooltip-header-stage-dev",
-                                                    position: "bottom",
-                                                    text: "Deployment stage: DEV"
-                                                })]
-                                            }) : (0, Fr.jsx)(Fr.Fragment, {}), "prod" !== (null === (D = k.app) || void 0 === D ? void 0 : D.stage) && "dev" !== (null === (S = k.app) || void 0 === S ? void 0 : S.stage) ? (0, Fr.jsxs)(Fr.Fragment, {
-                                                children: [(0, Fr.jsxs)("b", {
-                                                    id: "tooltip-header-stage",
-                                                    children: [null === (L = k.app) || void 0 === L ? void 0 : L.stage, "}"]
-                                                }), " \xa0|\xa0", (0, Fr.jsx)(Yi, {
-                                                    id: "tooltip-header-stage",
-                                                    position: "bottom",
-                                                    text: "Deployment stage: {header.app?.stage}"
-                                                })]
-                                            }) : (0, Fr.jsx)(Fr.Fragment, {}), Br.IsLoggedIn(k) ? (0, Fr.jsx)(Fr.Fragment, {
-                                                children: Br.LoggedInUser(k) ? (0, Fr.jsxs)(Fr.Fragment, {
-                                                    children: [(0, Fr.jsx)(Oe, {
-                                                        to: kr.Path("/login"),
-                                                        id: "tooltip-header-logged-in",
-                                                        style: {
-                                                            textDecoration: "none"
-                                                        },
-                                                        children: (0, Fr.jsx)("b", {
-                                                            style: {
-                                                                color: "darkblue"
-                                                            },
-                                                            children: Br.LoggedInUser(k)
-                                                        })
-                                                    }), (0, Fr.jsx)(Yi, {
-                                                        id: "tooltip-header-logged-in",
-                                                        position: "bottom",
-                                                        text: "Logged in ".concat(Pr.Ago(Br.LoggedInAt()))
-                                                    }), Br.LoggedInViaGoogle(k) ? (0, Fr.jsx)(Fr.Fragment, {
-                                                        children: (0, Fr.jsxs)("span", {
-                                                            children: [(0, Fr.jsx)("img", {
-                                                                id: "tooltip-header-login-google",
-                                                                alt: "google",
-                                                                style: {
-                                                                    marginLeft: "9px",
-                                                                    marginRight: "0",
-                                                                    marginBottom: "2px"
-                                                                },
-                                                                src: Ut.GoogleLoginLogo(),
-                                                                height: "15"
-                                                            }), (0, Fr.jsx)(Yi, {
-                                                                id: "tooltip-header-login-google",
-                                                                position: "bottom",
-                                                                text: "Logged in via Google authentication."
-                                                            })]
-                                                        })
-                                                    }) : (0, Fr.jsx)(Fr.Fragment, {
-                                                        children: Br.LoggedInViaGitHub(k) && (0, Fr.jsxs)(Fr.Fragment, {
-                                                            children: [(0, Fr.jsx)("span", {
-                                                                id: "tooltip-header-login-github",
-                                                                children: (0, Fr.jsx)("img", {
-                                                                    alt: "github",
-                                                                    style: {
-                                                                        marginLeft: "5px",
-                                                                        marginRight: "-4px",
-                                                                        marginBottom: "2px"
-                                                                    },
-                                                                    src: Ut.GitHubLoginLogo(),
-                                                                    height: "19"
-                                                                })
-                                                            }), (0, Fr.jsx)(Yi, {
-                                                                id: "tooltip-header-login-github",
-                                                                position: "bottom",
-                                                                text: "Logged in via GitHub authentication."
-                                                            })]
-                                                        })
-                                                    })]
-                                                }) : (0, Fr.jsx)(Fr.Fragment, {
-                                                    children: (0, Fr.jsx)("b", {
-                                                        style: {
-                                                            color: "darkred"
-                                                        },
-                                                        children: "UNKNOWN USER"
-                                                    })
-                                                })
-                                            }) : (0, Fr.jsxs)(Fr.Fragment, {
-                                                children: [(0, Fr.jsx)(Oe, {
-                                                    to: kr.Path("/login", At.Current(k)),
-                                                    style: {
-                                                        textDecoration: "none"
-                                                    },
-                                                    children: (0, Fr.jsx)("b", {
-                                                        style: {
-                                                            color: "darkblue"
-                                                        },
-                                                        id: "tooltip-header-nologin-2",
-                                                        children: "NOT LOGGED IN"
-                                                    })
-                                                }), (0, Fr.jsx)(Yi, {
-                                                    id: "tooltip-header-nologin-2",
-                                                    position: "bottom",
-                                                    text: "Not logged in. Click to login."
-                                                })]
-                                            })]
-                                        })]
-                                    }), (0, Fr.jsxs)("tr", {
-                                        children: [(0, Fr.jsx)("td", {
-                                            style: {
-                                                background: "lightyellow",
-                                                color: "darkred",
-                                                padding: "3pt"
-                                            },
-                                            colSpan: "1",
-                                            children: (0, Fr.jsxs)("i", {
-                                                style: {
-                                                    fontSize: "small"
-                                                },
-                                                children: ["This is the ", (0, Fr.jsx)("b", {
-                                                    children: "new"
-                                                }), " Foursight ", (0, Fr.jsx)("b", {
-                                                    children: "React"
-                                                }), ". For the ", (0, Fr.jsx)("b", {
-                                                    children: "legacy"
-                                                }), " Foursight click ", (0, Fr.jsx)("a", {
-                                                    href: At.LegacyFoursightLink(k),
-                                                    style: {
-                                                        color: "inherit"
-                                                    },
-                                                    children: (0, Fr.jsx)("b", {
-                                                        children: (0, Fr.jsx)("u", {
-                                                            children: "here"
-                                                        })
-                                                    })
-                                                }), "."]
-                                            })
-                                        }), (0, Fr.jsx)("td", {
-                                            style: {
-                                                background: "lightyellow"
-                                            }
-                                        }), (0, Fr.jsx)("td", {
-                                            style: {
-                                                background: "lightyellow",
-                                                color: "darkred",
-                                                fontSize: "small"
-                                            },
-                                            children: (0, Fr.jsx)("table", {
-                                                width: "100%",
-                                                children: (0, Fr.jsx)("tbody", {
-                                                    children: (0, Fr.jsxs)("tr", {
-                                                        children: [(0, Fr.jsx)("td", {
-                                                            style: {
-                                                                float: "right",
-                                                                width: "98%",
-                                                                whiteSpace: "nowrap",
-                                                                align: "right"
-                                                            },
-                                                            align: "right",
-                                                            children: _.length > 0 && (0, Fr.jsx)(Fr.Fragment, {
-                                                                children: (0, Fr.jsx)("span", {
-                                                                    children: (0, Fr.jsx)(No, {
-                                                                        loading: _.length > 0,
-                                                                        color: "darkred",
-                                                                        label: "",
-                                                                        size: 150,
-                                                                        style: {
-                                                                            marginRight: "20px"
-                                                                        }
-                                                                    })
-                                                                })
-                                                            })
-                                                        }), (0, Fr.jsx)("td", {
-                                                            style: {
-                                                                width: "1%",
-                                                                color: "darkred"
-                                                            },
-                                                            children: _.length > 0 && (0, Fr.jsxs)("small", {
-                                                                children: ["\xa0\xa0[", _.length, "]"]
-                                                            })
-                                                        }), (0, Fr.jsx)("td", {
-                                                            style: {
-                                                                color: "darkred",
-                                                                textAlign: "right",
-                                                                paddingRight: "10pt",
-                                                                width: "1%",
-                                                                fontSize: "small",
-                                                                fontStyle: "italic",
-                                                                whiteSpace: "nowrap"
-                                                            },
-                                                            children: kr.IsLocal() && (0, Fr.jsxs)(Fr.Fragment, {
-                                                                children: ["\xa0\xa0", Je.IsLocalCrossOrigin() ? (0, Fr.jsx)(Fr.Fragment, {
-                                                                    children: "Running locally cross-origin"
-                                                                }) : (0, Fr.jsx)(Fr.Fragment, {
-                                                                    children: "Running locally"
-                                                                })]
-                                                            })
-                                                        })]
-                                                    })
-                                                })
-                                            })
-                                        })]
-                                    }), (0, Fr.jsx)("tr", {
-                                        children: (0, Fr.jsx)("td", {
-                                            style: {
-                                                height: "1px",
-                                                background: "darkblue"
-                                            }
-                                        })
-                                    })]
-                                })
-                            })]
-                        }), (0, Fr.jsxs)("div", {
-                            style: {
-                                float: "right",
-                                marginRight: "7pt",
-                                marginTop: "6pt"
-                            },
-                            children: [!1, (0, Fr.jsx)("div", {
-                                children: (0, Fr.jsx)("table", {
-                                    children: (0, Fr.jsx)("tbody", {
-                                        children: (0, Fr.jsx)("tr", {
-                                            children: (0, Fr.jsx)("td", {
-                                                style: {
-                                                    paddingLeft: "10pt"
-                                                },
-                                                children: (0, Fr.jsx)(Xa, {})
-                                            })
-                                        })
-                                    })
-                                })
-                            })]
-                        })]
-                    })
-                })
-            },
-            rs = function(e) {
-                var n = e.children,
-                    r = a((0, t.useState)({
-                        loading: !0
-                    }), 2),
-                    o = r[0],
-                    i = r[1];
-                return so("/header", {
-                    onData: function(e) {
-                        e.loading = !1, i(e), At.IsFoursightFourfront(e) ? Ft.SetFoursightFourfront() : Ft.SetFoursightCgap()
-                    },
-                    onError: function(e) {
-                        i((function(e) {
-                            return Ye(Ye({}, e), {
-                                error: !0
-                            })
-                        }))
-                    },
-                    cache: !0
-                }), (0, Fr.jsx)(lo.Provider, {
-                    value: [o, i],
-                    children: n
-                })
-            },
-            os = function(e) {
-                var n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, w, j = co(),
-                    x = (At.IsFoursightFourfront(j) ? "foursight" : "foursight-cgap") + ": " + (null === j || void 0 === j || null === (n = j.versions) || void 0 === n ? void 0 : n.foursight_core) + " | foursight-core: " + (null === j || void 0 === j || null === (r = j.versions) || void 0 === r ? void 0 : r.foursight) + " | dcicutils: " + (null === j || void 0 === j || null === (o = j.versions) || void 0 === o ? void 0 : o.dcicutils),
-                    N = {
-                        id: "".concat(null === (i = j.app) || void 0 === i || null === (s = i.credentials) || void 0 === s ? void 0 : s.aws_account_name, ":").concat(null === j || void 0 === j || null === (u = j.app) || void 0 === u ? void 0 : u.stage),
-                        name: null === (l = j.app) || void 0 === l || null === (c = l.credentials) || void 0 === c ? void 0 : c.aws_account_name,
-                        stage: null === (d = j.app) || void 0 === d ? void 0 : d.stage
-                    },
-                    I = a((0, t.useState)(!1), 2),
-                    D = I[0],
-                    S = I[1];
-                return (0, Fr.jsx)(Fr.Fragment, {
-                    children: (0, Fr.jsxs)("div", {
-                        className: "container",
-                        style: {
-                            marginTop: "-16pt"
-                        },
-                        children: [(0, Fr.jsxs)("div", {
-                            className: "box lighten",
-                            style: {
-                                margin: "20pt",
-                                padding: "10pt"
-                            },
-                            children: [(0, Fr.jsxs)("b", {
-                                style: {
-                                    fontSize: "x-large"
-                                },
-                                children: ["Welcome to Foursight \xa0", (0, Fr.jsxs)("span", {
-                                    style: {
-                                        fontWeight: "normal"
-                                    },
-                                    children: ["(", At.IsFoursightFourfront(j) ? "Fourfront" : "CGAP", ")"]
-                                })]
-                            }), (0, Fr.jsxs)("div", {
-                                style: {
-                                    float: "right",
-                                    fontSize: "x-small",
-                                    textAlign: "right",
-                                    marginTop: "-3pt",
-                                    marginRight: "2pt"
-                                },
-                                children: [(0, Fr.jsxs)("span", {
-                                    id: "tooltip-home-versions",
-                                    children: ["Foursight Version: ", (0, Fr.jsx)("b", {
-                                        children: null === j || void 0 === j || null === (f = j.versions) || void 0 === f ? void 0 : f.foursight
-                                    })]
-                                }), " ", (0, Fr.jsx)("br", {}), (0, Fr.jsx)(Yi, {
-                                    id: "tooltip-home-versions",
-                                    position: "top",
-                                    size: "small",
-                                    text: x
-                                }), null !== j && void 0 !== j && null !== (p = j.app) && void 0 !== p && null !== (h = p.credentials) && void 0 !== h && h.aws_account_name ? (0, Fr.jsxs)(Fr.Fragment, {
-                                    children: [(0, Fr.jsxs)("span", {
-                                        id: "tooltip-home-aws-account",
-                                        children: ["AWS Account: ", (0, Fr.jsx)("b", {
-                                            children: null === j || void 0 === j || null === (g = j.app) || void 0 === g || null === (y = g.credentials) || void 0 === y ? void 0 : y.aws_account_name
-                                        })]
-                                    }), " ", (0, Fr.jsx)("br", {}), (0, Fr.jsx)(Yi, {
-                                        id: "tooltip-home-aws-account",
-                                        position: "top",
-                                        size: "small",
-                                        text: "AWS Account Number: " + (null === j || void 0 === j || null === (m = j.app) || void 0 === m || null === (v = m.credentials) || void 0 === v ? void 0 : v.aws_account_number)
-                                    })]
-                                }) : (0, Fr.jsxs)(Fr.Fragment, {
-                                    children: [(0, Fr.jsxs)("span", {
-                                        children: ["AWS Account: ", (0, Fr.jsx)("b", {
-                                            children: null === j || void 0 === j || null === (M = j.app) || void 0 === M || null === (b = M.credentials) || void 0 === b ? void 0 : b.aws_account_number
-                                        })]
-                                    }), " ", (0, Fr.jsx)("br", {})]
-                                }), "Foursight Stage: ", (0, Fr.jsx)("b", {
-                                    children: null === j || void 0 === j || null === (w = j.app) || void 0 === w ? void 0 : w.stage
-                                }), " ", (0, Fr.jsx)("br", {})]
-                            }), (0, Fr.jsx)(Ji, {
-                                top: "10pt",
-                                bottom: "4pt"
-                            }), "This is the ", (0, Fr.jsx)("b", {
-                                children: "new"
-                            }), " React version of Foursight. To use the previous version click ", (0, Fr.jsx)("b", {
-                                children: (0, Fr.jsx)("a", {
-                                    href: At.LegacyFoursightLink(j),
-                                    style: {
-                                        color: "inherit"
-                                    },
-                                    children: (0, Fr.jsx)("u", {
-                                        children: "here"
-                                    })
-                                })
-                            }), ".", (0, Fr.jsx)("span", {
-                                id: "tooltip-account-summary",
-                                style: {
-                                    float: "right",
-                                    marginTop: "-3pt"
-                                },
-                                className: "pointer",
-                                onClick: function() {
-                                    return S(!D)
-                                },
-                                children: (0, Fr.jsx)("img", {
-                                    alt: "settings",
-                                    src: Ut.SettingsRedIcon(),
-                                    height: "28"
-                                })
-                            }), (0, Fr.jsx)(Yi, {
-                                id: "tooltip-account-summary",
-                                position: "top",
-                                size: "small",
-                                text: "Click to " + (D ? "hide" : "show") + " account summary."
-                            }), (0, Fr.jsx)(Ji, {
-                                top: "4pt",
-                                bottom: "10pt"
-                            }), D && (0, Fr.jsx)(Fr.Fragment, {
-                                children: (0, Fr.jsx)("div", {
-                                    style: {
-                                        marginBottom: "12pt"
-                                    },
-                                    children: (0, Fr.jsx)(Wi, {
-                                        account: N,
-                                        header: j,
-                                        decrementAccountCount: function() {},
-                                        all: !0,
-                                        brighten: !0
-                                    })
-                                })
-                            }), (0, Fr.jsx)("p", {}), (0, Fr.jsxs)("ul", {
-                                children: [(0, Fr.jsxs)("li", {
-                                    children: [" To view Foursight ", (0, Fr.jsx)("b", {
-                                        children: (0, Fr.jsx)(qi, {
-                                            to: "/checks",
-                                            children: "checks"
-                                        })
-                                    }), " click ", (0, Fr.jsx)("b", {
-                                        children: (0, Fr.jsx)(qi, {
-                                            to: "/checks",
-                                            children: (0, Fr.jsx)("u", {
-                                                children: "here"
-                                            })
-                                        })
-                                    }), ".  "]
-                                }), (0, Fr.jsxs)("li", {
-                                    children: [" To view Foursight ", (0, Fr.jsx)("b", {
-                                        children: (0, Fr.jsx)(qi, {
-                                            to: "/info",
-                                            children: "general"
-                                        })
-                                    }), " info click ", (0, Fr.jsx)("b", {
-                                        children: (0, Fr.jsx)(qi, {
-                                            to: "/info",
-                                            children: (0, Fr.jsx)("u", {
-                                                children: "here"
-                                            })
-                                        })
-                                    }), ".  "]
-                                }), (0, Fr.jsxs)("li", {
-                                    children: [" To view Foursight ", (0, Fr.jsx)("b", {
-                                        children: (0, Fr.jsx)(qi, {
-                                            to: "/env",
-                                            children: "environments"
-                                        })
-                                    }), " info click ", (0, Fr.jsx)("b", {
-                                        children: (0, Fr.jsx)(qi, {
-                                            to: "/env",
-                                            children: (0, Fr.jsx)("u", {
-                                                children: "here"
-                                            })
-                                        })
-                                    }), ". "]
-                                }), (0, Fr.jsxs)("li", {
-                                    children: [" To view Foursight ", (0, Fr.jsx)("b", {
-                                        children: (0, Fr.jsx)(qi, {
-                                            to: "/users",
-                                            children: "users"
-                                        })
-                                    }), " click ", (0, Fr.jsx)("b", {
-                                        children: (0, Fr.jsx)(qi, {
-                                            to: "/users",
-                                            children: (0, Fr.jsx)("u", {
-                                                children: "here"
-                                            })
-                                        })
-                                    }), ".  "]
-                                }), (0, Fr.jsxs)("li", {
-                                    children: [" To view ", (0, Fr.jsx)("b", {
-                                        children: (0, Fr.jsx)(qi, {
-                                            to: "/aws/s3",
-                                            children: "AWS S3"
-                                        })
-                                    }), " info click ", (0, Fr.jsx)("b", {
-                                        children: (0, Fr.jsx)(qi, {
-                                            to: "/aws/s3",
-                                            children: (0, Fr.jsx)("u", {
-                                                children: "here"
-                                            })
-                                        })
-                                    }), ".  "]
-                                }), (0, Fr.jsxs)("li", {
-                                    children: [" To view ", (0, Fr.jsx)("b", {
-                                        children: (0, Fr.jsx)(qi, {
-                                            to: "/aws/infrastructure",
-                                            children: "AWS infrastructure"
-                                        })
-                                    }), " info click ", (0, Fr.jsx)("b", {
-                                        children: (0, Fr.jsx)(qi, {
-                                            to: "/aws/infrastructure",
-                                            children: (0, Fr.jsx)("u", {
-                                                children: "here"
-                                            })
-                                        })
-                                    }), ".  "]
-                                })]
-                            })]
-                        }), (0, Fr.jsxs)("div", {
-                            className: "box thickborder",
-                            style: {
-                                margin: "20pt",
-                                padding: "10pt",
-                                marginTop: "-10pt"
-                            },
-                            children: ["You are logged in as: ", (0, Fr.jsx)(Ki, {}), (0, Fr.jsx)("br", {}), "To view your ", (0, Fr.jsx)("b", {
-                                children: (0, Fr.jsx)(qi, {
-                                    to: "/login",
-                                    children: "session"
-                                })
-                            }), " info click ", (0, Fr.jsx)("b", {
-                                children: (0, Fr.jsx)(qi, {
-                                    to: "/login",
-                                    children: (0, Fr.jsx)("u", {
-                                        children: "here"
-                                    })
-                                })
-                            }), ". ", (0, Fr.jsx)("br", {}), "To ", (0, Fr.jsx)("b", {
-                                onClick: Zr,
-                                children: (0, Fr.jsx)(qi, {
-                                    children: "logout"
-                                })
-                            }), " click ", (0, Fr.jsx)("b", {
-                                onClick: Zr,
-                                children: (0, Fr.jsx)(qi, {
-                                    children: (0, Fr.jsx)("u", {
-                                        children: "here"
-                                    })
-                                })
-                            }), "."]
-                        }), (0, Fr.jsx)(Fr.Fragment, {
-                            children: (0, Fr.jsxs)("div", {
-                                className: "box lighten",
-                                style: {
-                                    fontSize: "small",
-                                    margin: "20pt",
-                                    padding: "5pt 10pt 5pt 10pt",
-                                    marginTop: "-10pt"
-                                },
-                                children: ["Click ", (0, Fr.jsx)("a", {
-                                    href: kr.Path("/accounts?all=true"),
-                                    rel: "noreferrer",
-                                    target: "_blank",
-                                    style: {
-                                        color: "var(--box-fg)"
-                                    },
-                                    children: (0, Fr.jsx)("b", {
-                                        children: "here"
-                                    })
-                                }), " to view all ", (0, Fr.jsx)("a", {
-                                    href: kr.Path("/accounts?all=true"),
-                                    style: {
-                                        color: "var(--box-fg)"
-                                    },
-                                    rel: "noreferrer",
-                                    target: "_blank",
-                                    children: (0, Fr.jsx)("b", {
-                                        children: "known accounts"
-                                    })
-                                }), ".", (0, Fr.jsx)($i, {
-                                    href: kr.Path("/accounts?all=true"),
-                                    bold: !0,
-                                    style: {
-                                        marginLeft: "6pt"
-                                    }
-                                })]
-                            })
-                        })]
-                    })
-                })
-            },
-            is = function(e) {
-                var n = e.title,
-                    r = e.show,
-                    o = void 0 === r || r,
-                    i = e.info,
-                    s = e.children,
-                    u = a((0, t.useState)(o), 2),
-                    l = u[0],
-                    c = u[1];
-                return (0, Fr.jsx)(Fr.Fragment, {
-                    children: (0, Fr.jsx)("div", {
-                        className: "container",
-                        children: l ? (0, Fr.jsxs)(Fr.Fragment, {
-                            children: [(0, Fr.jsx)("b", {
-                                onClick: function() {
-                                    return c(!1)
-                                },
-                                style: {
-                                    cursor: "pointer"
-                                },
-                                children: n
-                            }), " \xa0", (0, Fr.jsx)("span", {
-                                onClick: function() {
-                                    return c(!1)
-                                },
-                                style: {
-                                    cursor: "pointer"
-                                },
-                                children: Do.DownArrow
-                            }), "Versions" === n && (0, Fr.jsxs)("b", {
-                                id: "tooltip-info-refresh",
-                                style: {
-                                    float: "right",
-                                    cursor: "pointer"
-                                },
-                                onClick: i.refresh,
-                                children: [Do.Refresh, "\xa0"]
-                            }), (0, Fr.jsx)(Yi, {
-                                id: "tooltip-info-refresh",
-                                position: "bottom",
-                                size: "small",
-                                text: "Click to refresh."
-                            }), (0, Fr.jsx)("ul", {
-                                className: "top-level-list",
-                                children: (0, Fr.jsx)("div", {
-                                    className: "box",
-                                    style: {
-                                        paddingLeft: "8pt",
-                                        paddingTop: "6pt",
-                                        paddingBottom: "8pt"
-                                    },
-                                    children: s
-                                })
-                            })]
-                        }) : (0, Fr.jsxs)(Fr.Fragment, {
-                            children: [(0, Fr.jsx)("b", {
-                                onClick: function() {
-                                    return c(!0)
-                                },
-                                style: {
-                                    cursor: "pointer"
-                                },
-                                children: n
-                            }), " \xa0", (0, Fr.jsx)("span", {
-                                onClick: function() {
-                                    return c(!0)
-                                },
-                                style: {
-                                    cursor: "pointer"
-                                },
-                                children: Do.UpArrow
-                            }), (0, Fr.jsxs)("div", {
-                                className: "box",
-                                children: ["Click ", (0, Fr.jsx)("span", {
-                                    onClick: function() {
-                                        return c(!0)
-                                    },
-                                    style: {
-                                        cursor: "pointer"
-                                    },
-                                    children: (0, Fr.jsx)("b", {
-                                        children: "here"
-                                    })
-                                }), " to ", (0, Fr.jsx)("span", {
-                                    onClick: function() {
-                                        return c(!0)
-                                    },
-                                    style: {
-                                        cursor: "pointer"
-                                    },
-                                    children: "show"
-                                }), "."]
-                            })]
-                        })
-                    })
-                })
-            },
-            as = function(e) {
-                var t = e.name,
-                    n = e.value,
-                    r = e.monospace,
-                    o = void 0 !== r && r,
-                    i = e.copy,
-                    a = void 0 === i || i,
-                    s = e.size,
-                    u = void 0 === s ? "4" : s,
-                    l = e.pypi,
-                    c = void 0 === l ? null : l,
-                    d = e.github,
-                    f = void 0 === d ? null : d,
-                    p = e.elasticsearch,
-                    h = void 0 !== p && p,
-                    g = e.python,
-                    y = void 0 !== g && g,
-                    m = (e.chalice, e.check),
-                    v = void 0 !== m && m,
-                    M = e.link,
-                    b = void 0 === M ? null : M,
-                    w = e.optional,
-                    j = void 0 !== w && w;
-                var x = {
-                        fontSize: "11pt",
-                        fontFamily: o ? "monospace" : "inherit",
-                        fontWeight: "bold",
-                        wordWrap: "break-word",
-                        cursor: a ? "copy" : "inherit",
-                        align: "left"
-                    },
-                    N = a ? {
-                        onClick: function() {
-                            return Vi.Copy(t)
-                        }
-                    } : {},
-                    I = v ? (0, Fr.jsxs)("span", {
-                        children: ["\xa0", (0, Fr.jsx)("b", {
-                            style: {
-                                fontSize: "13pt",
-                                color: "green"
-                            },
-                            children: Do.Check
-                        })]
-                    }) : (0, Fr.jsx)("span", {}),
-                    D = c ? (0, Fr.jsxs)("span", {
-                        children: [(0, Fr.jsx)("a", {
-                            target: "_blank",
-                            rel: "noreferrer",
-                            href: "https://pypi.org/project/" + t + "/" + n + "/",
-                            children: (0, Fr.jsx)("img", {
-                                alt: "pypi",
-                                src: Ut.PyPi(),
-                                height: "21"
-                            })
-                        }), "\xa0"]
-                    }) : (0, Fr.jsx)("span", {}),
-                    S = f ? (0, Fr.jsxs)("span", {
-                        children: [(0, Fr.jsx)("a", {
-                            target: "_blank",
-                            rel: "noreferrer",
-                            href: "https://github.com/" + f + "/" + ("dcicutils" === t ? "utils" : t) + "/releases/tag/" + ("chalice" !== t ? "v" : "") + n,
-                            children: (0, Fr.jsx)("img", {
-                                alt: "github",
-                                src: Ut.GitHub(),
-                                height: "15"
-                            })
-                        }), "\xa0"]
-                    }) : (0, Fr.jsx)("span", {}),
-                    L = h ? (0, Fr.jsxs)("span", {
-                        children: [(0, Fr.jsx)("a", {
-                            target: "_blank",
-                            rel: "noreferrer",
-                            href: "https://www.elastic.co/guide/en/elasticsearch/reference/".concat(function(e) {
-                                var t = null === e || void 0 === e ? void 0 : e.split(".");
-                                return (null === t || void 0 === t ? void 0 : t.length) >= 2 ? t[0] + "." + t[1] : e
-                            }(n), "/release-notes-").concat(n, ".html"),
-                            style: {
-                                marginLeft: "-2px"
-                            },
-                            children: (0, Fr.jsx)("img", {
-                                alt: "github",
-                                src: Ut.ElasticsearchLogo(),
-                                height: "18"
-                            })
-                        }), "\xa0"]
-                    }) : (0, Fr.jsx)("span", {}),
-                    k = y ? (0, Fr.jsxs)("span", {
-                        children: [(0, Fr.jsx)("a", {
-                            target: "_blank",
-                            rel: "noreferrer",
-                            href: "https://docs.python.org/release/" + n + "/",
-                            children: (0, Fr.jsx)("img", {
-                                alt: "python",
-                                src: Ut.Python(),
-                                height: "19"
-                            })
-                        }), "\xa0"]
-                    }) : (0, Fr.jsx)("span", {}),
-                    C = (0, Fr.jsx)("span", {});
-                return (0, Fr.jsx)(Fr.Fragment, {
-                    children: (0, Fr.jsx)("div", {
-                        style: {
-                            marginTop: "1px"
-                        },
-                        children: !j || n ? (0, Fr.jsxs)("div", {
-                            className: "row",
-                            children: [(0, Fr.jsx)("div", {
-                                className: "col-sm-" + u,
-                                children: (0, Fr.jsxs)("div", {
-                                    style: {
-                                        fontSize: "11pt",
-                                        fontFamily: "inherit",
-                                        fontWeight: "normal",
-                                        padding: "0px",
-                                        align: "left"
-                                    },
-                                    children: [t, ":"]
-                                })
-                            }), (0, Fr.jsxs)("div", Ye(Ye({
-                                id: t,
-                                className: "col-sm-8",
-                                style: x,
-                                align: "left"
-                            }, N), {}, {
-                                children: [D, S, L, k, C, b && n ? (0, Fr.jsx)("span", {
-                                    children: (0, Fr.jsx)(Oe, {
-                                        to: b,
-                                        children: n
-                                    })
-                                }) : (0, Fr.jsx)("span", {
-                                    children: st.IsNonEmptyObject(n) ? (0, Fr.jsx)(Fr.Fragment, {
-                                        children: n
-                                    }) : (0, Fr.jsx)(Fr.Fragment, {
-                                        children: n || (0, Fr.jsx)("span", {
-                                            children: Do.EmptySet
-                                        })
-                                    })
-                                }), I]
-                            }))]
-                        }) : (0, Fr.jsx)("span", {})
-                    })
-                })
-            },
-            ss = function() {
-                var e, n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, w, j, x, N, I, D, S, L, k, C, E, _, T, A, O, z, U, P, R = co(),
-                    B = so("/info"),
-                    F = a((0, t.useState)(!1), 2),
-                    Y = F[0],
-                    Q = F[1],
-                    G = a((0, t.useState)(!1), 2),
-                    W = G[0],
-                    H = G[1],
-                    Z = a((0, t.useState)(!1), 2),
-                    V = Z[0],
-                    q = Z[1],
-                    J = oa();
-                return B.error ? (0, Fr.jsx)(Xi, {
-                    error: B.error,
-                    message: "Error loading info from Foursight API"
-                }) : (0, Fr.jsxs)("div", {
-                    className: "container",
-                    children: [(0, Fr.jsxs)(is, {
-                        info: B,
-                        title: "Versions",
-                        children: [(0, Fr.jsx)(as, {
-                            name: null === (e = R.app) || void 0 === e ? void 0 : e.package,
-                            value: null === (n = R.versions) || void 0 === n ? void 0 : n.foursight,
-                            monospace: !0,
-                            copy: !0,
-                            pypi: !0,
-                            github: At.IsFoursightFourfront(R) ? "4dn-dcic" : "dbmi-bgm",
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "foursight-core",
-                            value: null === (r = R.versions) || void 0 === r ? void 0 : r.foursight_core,
-                            monospace: !0,
-                            copy: !0,
-                            pypi: !0,
-                            github: "4dn-dcic",
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "dcicutils",
-                            value: null === (o = R.versions) || void 0 === o ? void 0 : o.dcicutils,
-                            monospace: !0,
-                            copy: !0,
-                            pypi: !0,
-                            github: "4dn-dcic",
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "tibanna",
-                            value: null === (i = R.versions) || void 0 === i ? void 0 : i.tibanna,
-                            monospace: !0,
-                            copy: !0,
-                            size: "2",
-                            pypi: !0
-                        }), (0, Fr.jsx)(as, {
-                            name: "tibanna-ff",
-                            value: null === (s = R.versions) || void 0 === s ? void 0 : s.tibanna_ff,
-                            monospace: !0,
-                            copy: !0,
-                            size: "2",
-                            pypi: !0
-                        }), (0, Fr.jsx)(as, {
-                            name: "chalice",
-                            value: null === (u = R.versions) || void 0 === u ? void 0 : u.chalice,
-                            monospace: !0,
-                            copy: !0,
-                            chalice: !0,
-                            size: "2",
-                            pypi: !0,
-                            github: "aws"
-                        }), (0, Fr.jsx)(as, {
-                            name: "python",
-                            value: null === (l = R.versions) || void 0 === l ? void 0 : l.python,
-                            monospace: !0,
-                            copy: !0,
-                            python: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "elasticsearch-server",
-                            value: (null === (c = R.versions) || void 0 === c ? void 0 : c.elasticsearch_server) || (null === (d = B.data) || void 0 === d || null === (f = d.versions) || void 0 === f ? void 0 : f.elasticsearch_server),
-                            monospace: !0,
-                            copy: !0,
-                            size: "2",
-                            elasticsearch: !0
-                        }), (0, Fr.jsx)(as, {
-                            name: "elasticsearch",
-                            value: null === (p = R.versions) || void 0 === p ? void 0 : p.elasticsearch,
-                            monospace: !0,
-                            copy: !0,
-                            size: "2",
-                            pypi: !0
-                        }), (0, Fr.jsx)(as, {
-                            name: "elasticsearch-dsl",
-                            value: null === (h = R.versions) || void 0 === h ? void 0 : h.elasticsearch_dsl,
-                            monospace: !0,
-                            copy: !0,
-                            size: "2",
-                            pypi: !0
-                        })]
-                    }), (0, Fr.jsxs)(is, {
-                        info: B,
-                        title: "Credentials Info",
-                        children: [(0, Fr.jsx)(as, {
-                            name: "AWS Account Number",
-                            value: B.get("app.credentials.aws_account_number"),
-                            monospace: !0,
-                            copy: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "AWS User ARN",
-                            value: B.get("app.credentials.aws_user_arn"),
-                            monospace: !0,
-                            copy: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "AWS Access Key ID",
-                            value: B.get("app.credentials.aws_access_key_id"),
-                            monospace: !0,
-                            copy: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "AWS Region Name",
-                            value: B.get("app.credentials.aws_region"),
-                            monospace: !0,
-                            copy: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Auth0 Client ID",
-                            value: B.get("app.credentials.auth0_client_id"),
-                            monospace: !0,
-                            copy: !0,
-                            size: "2"
-                        })]
-                    }), (0, Fr.jsxs)(is, {
-                        info: B,
-                        title: "Resources",
-                        children: [(0, Fr.jsx)(as, {
-                            name: "Foursight Server",
-                            value: B.get("server.foursight"),
-                            monospace: !0,
-                            copy: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Portal Server",
-                            value: B.get("server.portal"),
-                            monospace: !0,
-                            copy: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "ElasticSearch Server",
-                            value: B.get("server.es"),
-                            monospace: !0,
-                            copy: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "RDS Server",
-                            value: B.get("server.rds"),
-                            monospace: !0,
-                            copy: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "SQS Server",
-                            value: B.get("server.sqs"),
-                            monospace: !0,
-                            copy: !0,
-                            size: "2"
-                        })]
-                    }), (0, Fr.jsxs)(is, {
-                        info: B,
-                        title: "Environment Names",
-                        children: [(0, Fr.jsx)(as, {
-                            name: "Environment Name",
-                            value: At.RegularName(At.Current(), R),
-                            monospace: !0,
-                            copy: !0,
-                            size: "3"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Environment Name (Full)",
-                            value: At.FullName(At.Current(), R),
-                            monospace: !0,
-                            copy: !0,
-                            size: "3"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Environment Name (Short)",
-                            value: At.ShortName(At.Current(), R),
-                            monospace: !0,
-                            copy: !0,
-                            size: "3"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Environment Name (Public)",
-                            value: At.PublicName(At.Current(), R),
-                            monospace: !0,
-                            copy: !0,
-                            size: "3"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Environment Name (Foursight)",
-                            value: At.FoursightName(At.Current(), R),
-                            monospace: !0,
-                            copy: !0,
-                            size: "3"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Environment Name (Preferred)",
-                            value: At.PreferredName(At.Current(R), R),
-                            monospace: !0,
-                            copy: !0,
-                            size: "3"
-                        })]
-                    }), (0, Fr.jsxs)(is, {
-                        info: B,
-                        title: "Bucket Names",
-                        children: [(0, Fr.jsx)(as, {
-                            name: "Global Environment Bucket",
-                            value: B.get("buckets.env"),
-                            monospace: !0,
-                            copy: !0,
-                            size: "3"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Foursight Bucket Name",
-                            value: B.get("buckets.foursight"),
-                            monospace: !0,
-                            copy: !0,
-                            size: "3"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Foursight Bucket Prefix",
-                            value: B.get("buckets.foursight_prefix"),
-                            monospace: !0,
-                            copy: !0,
-                            size: "3"
-                        })]
-                    }), (0, Fr.jsx)(is, {
-                        info: B,
-                        title: "Environment & Bucket Names",
-                        children: (0, Fr.jsx)("pre", {
-                            className: "box",
-                            style: {
-                                border: "0",
-                                margin: "0",
-                                padding: "8",
-                                paddingBottom: "8",
-                                marginTop: "0"
-                            },
-                            children: (0, Fr.jsxs)("span", {
-                                children: [qr.Format(B.get("buckets.info")), (null === (g = B.get("buckets.info")) || void 0 === g ? void 0 : g.length) > 1 ? (0, Fr.jsx)("div", {
-                                    style: {
-                                        height: "1px",
-                                        marginTop: "6px",
-                                        marginBottom: "6px",
-                                        background: "black"
-                                    }
-                                }) : (0, Fr.jsx)("span", {})]
-                            }, Dr()())
-                        })
-                    }), (0, Fr.jsx)(is, {
-                        info: B,
-                        title: "Ecosystem",
-                        show: !1,
-                        children: (0, Fr.jsx)("pre", {
-                            className: "box",
-                            style: {
-                                border: "0",
-                                margin: "0",
-                                paddingTop: "8",
-                                paddingBottom: "8",
-                                marginTop: "0"
-                            },
-                            children: qr.Format(B.get("buckets.ecosystem"))
-                        })
-                    }), (0, Fr.jsxs)(is, {
-                        info: B,
-                        title: "Authentication/Authorization Info",
-                        show: !1,
-                        children: [(0, Fr.jsx)(as, {
-                            name: "Email",
-                            value: null === (y = Br.Token()) || void 0 === y ? void 0 : y.user,
-                            monospace: !0,
-                            copy: !0,
-                            check: null === (m = Br.Token()) || void 0 === m ? void 0 : m.user_verified,
-                            link: kr.Path("/users/" + Br.LoggedInUser(R), !0),
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "First Name",
-                            value: null === (v = Br.Token()) || void 0 === v ? void 0 : v.first_name,
-                            monospace: !0,
-                            copy: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Last Name",
-                            value: null === (M = Br.Token()) || void 0 === M ? void 0 : M.last_name,
-                            monospace: !0,
-                            copy: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Environments",
-                            value: null === (b = Br.Token()) || void 0 === b ? void 0 : b.allowed_envs.join(", "),
-                            monospace: !0,
-                            copy: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Audience",
-                            value: null === (w = Br.Token()) || void 0 === w ? void 0 : w.aud,
-                            monospace: !0,
-                            copy: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Issued At",
-                            monospace: !0,
-                            copy: !0,
-                            size: "2",
-                            value: (0, Fr.jsx)(aa.FormatDuration, {
-                                start: null === (j = Br.Token()) || void 0 === j ? void 0 : j.authenticated_at,
-                                verbose: !0,
-                                fallback: "just now",
-                                suffix: "ago",
-                                tooltip: !0,
-                                prefix: "datetime"
-                            })
-                        }), (0, Fr.jsx)(as, {
-                            name: "Expires At",
-                            monospace: !0,
-                            copy: !0,
-                            size: "2",
-                            value: (0, Fr.jsx)(aa.FormatDuration, {
-                                end: null === (x = Br.Token()) || void 0 === x ? void 0 : x.authenticated_until,
-                                verbose: !0,
-                                fallback: "now",
-                                suffix: "from now",
-                                tooltip: !0,
-                                prefix: "datetime"
-                            })
-                        }), (0, Fr.jsx)("hr", {
-                            style: {
-                                borderTop: "1px solid darkblue",
-                                marginTop: "8",
-                                marginBottom: "8"
-                            }
-                        }), Y ? (0, Fr.jsxs)(Fr.Fragment, {
-                            children: [(0, Fr.jsx)("small", {
-                                onClick: function() {
-                                    return Q(!1)
-                                },
-                                style: {
-                                    cursor: "pointer",
-                                    color: "inherit"
-                                },
-                                children: (0, Fr.jsxs)("b", {
-                                    children: [(0, Fr.jsx)("u", {
-                                        children: "AuthToken"
-                                    }), "\xa0", Do.DownArrow]
-                                })
-                            }), (0, Fr.jsxs)("pre", {
-                                style: {
-                                    filter: "brightness(1.05)",
-                                    background: "inherit",
-                                    color: "inherit",
-                                    fontWeight: "bold",
-                                    marginTop: "6pt"
-                                },
-                                children: [(0, Fr.jsx)("span", {
-                                    style: {
-                                        fontSize: "0",
-                                        opacity: "0"
-                                    },
-                                    id: "authtoken",
-                                    children: Tr.Str(Br.Token())
-                                }), (0, Fr.jsx)("img", {
-                                    src: Ut.Clipboard(),
-                                    alt: "copy",
-                                    onClick: function() {
-                                        return Vi.Copy("authtoken")
-                                    },
-                                    style: {
-                                        float: "right",
-                                        height: "20px",
-                                        cursor: "copy"
-                                    }
-                                }), qr.Format(Br.Token())]
-                            })]
-                        }) : (0, Fr.jsxs)(Fr.Fragment, {
-                            children: [(0, Fr.jsx)("small", {
-                                onClick: function() {
-                                    return Q(!0)
-                                },
-                                style: {
-                                    cursor: "pointer",
-                                    color: "darkblue"
-                                },
-                                children: (0, Fr.jsxs)("b", {
-                                    children: [(0, Fr.jsx)("u", {
-                                        children: "AuthToken"
-                                    }), "\xa0", Do.UpArrow]
-                                })
-                            }), (0, Fr.jsx)("br", {})]
-                        })]
-                    }), B.get("environ.AWS_LAMBDA_LOG_GROUP_NAME") && B.get("environ.AWS_LAMBDA_LOG_STREAM_NAME") && (0, Fr.jsx)(Fr.Fragment, {
-                        children: (0, Fr.jsxs)(is, {
-                            info: B,
-                            title: "Logs",
-                            children: [(0, Fr.jsx)(as, {
-                                name: "Log Group",
-                                value: B.get("environ.AWS_LAMBDA_LOG_GROUP_NAME"),
-                                monospace: !0,
-                                size: "2"
-                            }), (0, Fr.jsx)(as, {
-                                name: "Log Stream",
-                                value: B.get("environ.AWS_LAMBDA_LOG_STREAM_NAME"),
-                                monospace: !0,
-                                size: "2"
-                            })]
-                        })
-                    }), B.get("app.lambda") && (0, Fr.jsxs)(is, {
-                        info: B,
-                        title: "Lambda",
-                        show: !1,
-                        children: [(0, Fr.jsx)(as, {
-                            name: "Name",
-                            value: B.get("app.lambda.lambda_name"),
-                            monospace: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Function",
-                            value: B.get("app.lambda.lambda_function_name"),
-                            monospace: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "ARN",
-                            value: B.get("app.lambda.lambda_function_arn"),
-                            monospace: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "S3 Location",
-                            value: B.get("app.lambda.lambda_code_s3_bucket") + "/" + B.get("app.lambda.lambda_code_s3_bucket_key"),
-                            monospace: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Size",
-                            value: B.get("app.lambda.lambda_code_size"),
-                            monospace: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Modified",
-                            value: Pr.FormatDateTime(B.get("app.lambda.lambda_modified")),
-                            monospace: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Role",
-                            value: B.get("app.lambda.lambda_role"),
-                            monospace: !0,
-                            size: "2"
-                        })]
-                    }), (0, Fr.jsxs)(is, {
-                        info: B,
-                        title: "Miscellany",
-                        children: [V ? (0, Fr.jsxs)(Fr.Fragment, {
-                            children: [(0, Fr.jsx)("div", {
-                                id: "tooltip-info-reloading",
-                                style: {
-                                    float: "right"
-                                },
-                                children: (0, Fr.jsx)(No, {
-                                    condition: V,
-                                    label: "",
-                                    color: "darkblue"
-                                })
-                            }), (0, Fr.jsx)(Yi, {
-                                id: "tooltip-info-reloading",
-                                position: "bottom",
-                                size: "small",
-                                text: "Reloading the Foursight app."
-                            })]
-                        }) : (0, Fr.jsxs)(Fr.Fragment, {
-                            children: [(0, Fr.jsx)("b", {
-                                onClick: function() {
-                                    return q(!0), void J("/__reloadlambda__", {
-                                        onDone: function() {
-                                            return q(!1)
-                                        }
-                                    })
-                                },
-                                id: "tooltip-info-reload",
-                                style: {
-                                    float: "right",
-                                    cursor: "pointer"
-                                },
-                                children: Do.Refresh
-                            }), (0, Fr.jsx)(Yi, {
-                                id: "tooltip-info-reload",
-                                position: "bottom",
-                                size: "small",
-                                text: "Click here to reload the Foursight app."
-                            })]
-                        }), (0, Fr.jsxs)("div", {
-                            id: "tooltip-info-clear",
-                            style: {
-                                float: "right",
-                                marginTop: "-1px",
-                                marginRight: "4pt",
-                                cursor: "pointer"
-                            },
-                            children: ["\xa0\xa0", (0, Fr.jsx)("img", {
-                                alt: "Clear Cache",
-                                src: Ut.ClearCache(),
-                                height: "19",
-                                onClick: function() {
-                                    J(zt.Url("/__clearcache__", !1))
-                                }
-                            })]
-                        }), (0, Fr.jsx)(Yi, {
-                            id: "tooltip-info-clear",
-                            position: "bottom",
-                            size: "small",
-                            text: "Click to clear any server-side caches."
-                        }), (0, Fr.jsx)(as, {
-                            name: "App Deployed At",
-                            value: zt.IsLocal() ? "running locally" + (Je.IsLocalCrossOrigin() ? " (cross-origin)" : "") : (null === (N = R.app) || void 0 === N ? void 0 : N.deployed) + Pr.FormatDuration(null === (I = R.app) || void 0 === I ? void 0 : I.deployed, new Date, !0, "just now", "|", "ago"),
-                            monospace: !0,
-                            copy: !0,
-                            optional: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "App Launched At",
-                            value: (null === (D = R.app) || void 0 === D ? void 0 : D.launched) + Pr.FormatDuration(null === (S = R.app) || void 0 === S ? void 0 : S.launched, new Date, !0, "just now", "|", "ago"),
-                            monospace: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Page Loaded At",
-                            value: B.get("page.loaded") + Pr.FormatDuration(B.get("page.loaded"), new Date, !0, "just now", "|", "ago"),
-                            monospace: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Package",
-                            value: null === (L = R.app) || void 0 === L ? void 0 : L.package,
-                            monospace: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Stage",
-                            value: null === (k = R.app) || void 0 === k ? void 0 : k.stage,
-                            monospace: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Environment",
-                            value: At.Current(),
-                            monospace: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Domain",
-                            value: null === (C = R.app) || void 0 === C ? void 0 : C.domain,
-                            monospace: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Context",
-                            value: null === (E = R.app) || void 0 === E ? void 0 : E.context,
-                            monospace: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Path",
-                            value: B.get("page.path"),
-                            monospace: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Endpoint",
-                            value: B.get("page.endpoint"),
-                            monospace: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Client (React UI)",
-                            value: kr.BaseUrl(),
-                            monospace: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Server (React API)",
-                            value: zt.BaseUrl(),
-                            monospace: !0,
-                            size: "2"
-                        }), (0, Fr.jsx)(as, {
-                            name: "Checks File",
-                            value: null === (_ = B.data) || void 0 === _ || null === (T = _.checks) || void 0 === T ? void 0 : T.file,
-                            monospace: !0,
-                            size: "2"
-                        }), (null === (A = R.app) || void 0 === A ? void 0 : A.accounts_file) && (0, Fr.jsx)(as, {
-                            name: "Accounts File",
-                            value: null === (O = R.app) || void 0 === O ? void 0 : O.accounts_file,
-                            monospace: !0,
-                            size: "2"
-                        }), (null === (z = R.app) || void 0 === z ? void 0 : z.accounts_file_from_s3) && (0, Fr.jsx)(as, {
-                            name: "Accounts File (S3)",
-                            value: null === (U = R.app) || void 0 === U ? void 0 : U.accounts_file_from_s3,
-                            monospace: !0,
-                            size: "2"
-                        })]
-                    }), (0, Fr.jsx)(is, {
-                        info: B,
-                        title: "GAC: ".concat(B.get("gac.name")),
-                        show: !1,
-                        children: B.get("gac.values") ? (0, Fr.jsx)("span", {
-                            children: Object.keys(B.get("gac.values")).map((function(e) {
-                                return (0, Fr.jsx)(as, {
-                                    name: e,
-                                    value: B.get("gac.values")[e],
-                                    monospace: !0,
-                                    copy: !0
-                                }, e)
-                            }))
-                        }) : (0, Fr.jsx)("span", {})
-                    }), (0, Fr.jsx)(is, {
-                        info: B,
-                        title: "Environment Variables",
-                        show: !1,
-                        children: B.get("environ") ? (0, Fr.jsx)("span", {
-                            children: Object.keys(B.get("environ")).map((function(e) {
-                                return (0, Fr.jsx)(as, {
-                                    name: e,
-                                    value: B.get("environ")[e],
-                                    monospace: !0,
-                                    copy: !0
-                                }, e)
-                            }))
-                        }) : (0, Fr.jsx)("span", {})
-                    }), (null === (P = R.app) || void 0 === P ? void 0 : P.accounts) && (0, Fr.jsx)("div", {
-                        className: "container",
-                        style: {
-                            marginTop: "4pt"
-                        },
-                        children: W ? (0, Fr.jsx)(Fr.Fragment, {
-                            children: (0, Fr.jsx)(Hi, {})
-                        }) : (0, Fr.jsxs)(Fr.Fragment, {
-                            children: [(0, Fr.jsx)("b", {
-                                onClick: function() {
-                                    return H(!0)
-                                },
-                                style: {
-                                    cursor: "pointer"
-                                },
-                                children: "Show Accounts"
-                            }), (0, Fr.jsxs)("div", {
-                                className: "box",
-                                children: ["Click ", (0, Fr.jsx)("b", {
-                                    onClick: function() {
-                                        return H(!0)
-                                    },
-                                    style: {
-                                        cursor: "pointer"
-                                    },
-                                    children: "here"
-                                }), " to ", (0, Fr.jsx)("span", {
-                                    onClick: function() {
-                                        return H(!0)
-                                    },
-                                    style: {
-                                        cursor: "pointer"
-                                    },
-                                    children: "show"
-                                }), "."]
-                            })]
-                        })
-                    })]
-                })
-            },
-            us = function(e, t) {
-                return us = Object.setPrototypeOf || {
+            qa = __webpack_require__(9712),
+            Ja = function(e, t) {
+                return Ja = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
                     for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n])
-                }, us(e, t)
+                }, Ja(e, t)
             };
 
-        function ls(e, t) {
+        function Ka(e, t) {
             function n() {
                 this.constructor = e
             }
-            us(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+            Ja(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
         }
-        var cs, ds, fs, ps = function() {
-            return ps = Object.assign || function(e) {
+        var Xa, $a, es, ts = function() {
+            return ts = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, ps.apply(this, arguments)
+            }, ts.apply(this, arguments)
         };
 
-        function hs(e, t, n, r) {
+        function ns(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -59133,15 +56581,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function gs(e, t) {
+        function rs(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -59209,15 +56657,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function ys(e, t) {
+        function os(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -59231,50 +56679,50 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function ms(e) {
+        function is(e) {
             return e && !!["provider"].find((function(t) {
                 return e.hasOwnProperty(t)
             }))
         }
 
-        function vs(e) {
+        function as(e) {
             return void 0 !== e.redirectSignIn
         }! function(e) {
             e.Cognito = "COGNITO", e.Google = "Google", e.Facebook = "Facebook", e.Amazon = "LoginWithAmazon", e.Apple = "SignInWithApple"
-        }(cs || (cs = {})),
+        }(Xa || (Xa = {})),
         function(e) {
             e.NoConfig = "noConfig", e.MissingAuthConfig = "missingAuthConfig", e.EmptyUsername = "emptyUsername", e.InvalidUsername = "invalidUsername", e.EmptyPassword = "emptyPassword", e.EmptyCode = "emptyCode", e.SignUpError = "signUpError", e.NoMFA = "noMFA", e.InvalidMFA = "invalidMFA", e.EmptyChallengeResponse = "emptyChallengeResponse", e.NoUserSession = "noUserSession", e.Default = "default", e.DeviceConfig = "deviceConfig", e.NetworkError = "networkError", e.AutoSignInError = "autoSignInError"
-        }(ds || (ds = {})),
+        }($a || ($a = {})),
         function(e) {
             e.API_KEY = "API_KEY", e.AWS_IAM = "AWS_IAM", e.OPENID_CONNECT = "OPENID_CONNECT", e.AMAZON_COGNITO_USER_POOLS = "AMAZON_COGNITO_USER_POOLS", e.AWS_LAMBDA = "AWS_LAMBDA"
-        }(fs || (fs = {}));
-        var Ms = function(e, t) {
-            return Ms = Object.setPrototypeOf || {
+        }(es || (es = {}));
+        var ss = function(e, t) {
+            return ss = Object.setPrototypeOf || {
                 __proto__: []
             }
             instanceof Array && function(e, t) {
                 e.__proto__ = t
             } || function(e, t) {
                 for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n])
-            }, Ms(e, t)
+            }, ss(e, t)
         };
-        var bs = function() {
-            return bs = Object.assign || function(e) {
+        var us = function() {
+            return us = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, bs.apply(this, arguments)
+            }, us.apply(this, arguments)
         };
 
-        function ws(e, t, n, r) {
+        function ls(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -59294,15 +56742,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function js(e, t) {
+        function cs(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -59370,15 +56818,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function xs(e) {
+        function ds(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -59386,15 +56834,15 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function Ns(e, t) {
+        function fs(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -59408,58 +56856,58 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function Is() {
-            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Ns(arguments[t]));
+        function ps() {
+            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(fs(arguments[t]));
             return e
         }
-        var Ds, Ss = {
+        var hs, gs = {
             VERBOSE: 1,
             DEBUG: 2,
             INFO: 3,
             WARN: 4,
             ERROR: 5
         };
         ! function(e) {
             e.DEBUG = "DEBUG", e.ERROR = "ERROR", e.INFO = "INFO", e.WARN = "WARN", e.VERBOSE = "VERBOSE"
-        }(Ds || (Ds = {}));
-        var Ls = function() {
+        }(hs || (hs = {}));
+        var ys = function() {
                 function e(e, t) {
-                    void 0 === t && (t = Ds.WARN), this.name = e, this.level = t, this._pluggables = []
+                    void 0 === t && (t = hs.WARN), this.name = e, this.level = t, this._pluggables = []
                 }
                 return e.prototype._padding = function(e) {
                     return e < 10 ? "0" + e : "" + e
                 }, e.prototype._ts = function() {
                     var e = new Date;
                     return [this._padding(e.getMinutes()), this._padding(e.getSeconds())].join(":") + "." + e.getMilliseconds()
                 }, e.prototype.configure = function(e) {
                     return e ? (this._config = e, this._config) : this._config
                 }, e.prototype._log = function(t) {
                     for (var n, r, o = [], i = 1; i < arguments.length; i++) o[i - 1] = arguments[i];
                     var a = this.level;
                     e.LOG_LEVEL && (a = e.LOG_LEVEL), "undefined" !== typeof window && window.LOG_LEVEL && (a = window.LOG_LEVEL);
-                    var s = Ss[a],
-                        u = Ss[t];
+                    var s = gs[a],
+                        u = gs[t];
                     if (u >= s) {
                         var l = console.log.bind(console);
-                        t === Ds.ERROR && console.error && (l = console.error.bind(console)), t === Ds.WARN && console.warn && (l = console.warn.bind(console));
+                        t === hs.ERROR && console.error && (l = console.error.bind(console)), t === hs.WARN && console.warn && (l = console.warn.bind(console));
                         var c = "[" + t + "] " + this._ts() + " " + this.name,
                             d = "";
                         if (1 === o.length && "string" === typeof o[0]) l(d = c + " - " + o[0]);
                         else if (1 === o.length) d = c + " " + o[0], l(c, o[0]);
                         else if ("string" === typeof o[0]) {
                             var f = o.slice(1);
                             1 === f.length && (f = f[0]), d = c + " - " + o[0] + " " + f, l(c + " - " + o[0], f)
                         } else d = c + " " + o, l(c, o);
                         try {
-                            for (var p = xs(this._pluggables), h = p.next(); !h.done; h = p.next()) {
+                            for (var p = ds(this._pluggables), h = p.next(); !h.done; h = p.next()) {
                                 var g = h.value,
                                     y = {
                                         message: d,
                                         timestamp: Date.now()
                                     };
                                 g.pushLogs([y])
                             }
@@ -59473,78 +56921,78 @@
                             } finally {
                                 if (n) throw n.error
                             }
                         }
                     }
                 }, e.prototype.log = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Is([Ds.INFO], e))
+                    this._log.apply(this, ps([hs.INFO], e))
                 }, e.prototype.info = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Is([Ds.INFO], e))
+                    this._log.apply(this, ps([hs.INFO], e))
                 }, e.prototype.warn = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Is([Ds.WARN], e))
+                    this._log.apply(this, ps([hs.WARN], e))
                 }, e.prototype.error = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Is([Ds.ERROR], e))
+                    this._log.apply(this, ps([hs.ERROR], e))
                 }, e.prototype.debug = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Is([Ds.DEBUG], e))
+                    this._log.apply(this, ps([hs.DEBUG], e))
                 }, e.prototype.verbose = function() {
                     for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                    this._log.apply(this, Is([Ds.VERBOSE], e))
+                    this._log.apply(this, ps([hs.VERBOSE], e))
                 }, e.prototype.addPluggable = function(e) {
                     e && "Logging" === e.getCategoryName() && (this._pluggables.push(e), e.configure(this._config))
                 }, e.prototype.listPluggables = function() {
                     return this._pluggables
                 }, e.LOG_LEVEL = null, e
             }(),
-            ks = new Ls("Hub"),
-            Cs = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default";
-        var Es = function() {
+            ms = new ys("Hub"),
+            vs = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default";
+        var Ms = function() {
                 function e(e) {
                     this.listeners = [], this.patterns = [], this.protectedChannels = ["core", "auth", "api", "analytics", "interactions", "pubsub", "storage", "ui", "xr"], this.name = e
                 }
                 return e.prototype._remove = function(e, t) {
                     if (e instanceof RegExp) {
                         var n = this.patterns.find((function(t) {
                             return t.pattern.source === e.source
                         }));
-                        if (!n) return void ks.warn("No listeners for " + e);
-                        this.patterns = Is(this.patterns.filter((function(e) {
+                        if (!n) return void ms.warn("No listeners for " + e);
+                        this.patterns = ps(this.patterns.filter((function(e) {
                             return e !== n
                         })))
                     } else {
                         var r = this.listeners[e];
-                        if (!r) return void ks.warn("No listeners for " + e);
-                        this.listeners[e] = Is(r.filter((function(e) {
+                        if (!r) return void ms.warn("No listeners for " + e);
+                        this.listeners[e] = ps(r.filter((function(e) {
                             return e.callback !== t
                         })))
                     }
                 }, e.prototype.remove = function(e, t) {
                     this._remove(e, t)
                 }, e.prototype.dispatch = function(e, t, n, r) {
-                    (void 0 === n && (n = ""), this.protectedChannels.indexOf(e) > -1) && (r === Cs || ks.warn("WARNING: " + e + " is protected and dispatching on it can have unintended consequences"));
+                    (void 0 === n && (n = ""), this.protectedChannels.indexOf(e) > -1) && (r === vs || ms.warn("WARNING: " + e + " is protected and dispatching on it can have unintended consequences"));
                     var o = {
                         channel: e,
-                        payload: bs({}, t),
+                        payload: us({}, t),
                         source: n,
                         patternInfo: []
                     };
                     try {
                         this._toListeners(o)
                     } catch (i) {
-                        ks.error(i)
+                        ms.error(i)
                     }
                 }, e.prototype.listen = function(e, t, n) {
                     var r, o = this;
                     if (void 0 === n && (n = "noname"), function(e) {
                             return void 0 !== e.onHubCapsule
-                        }(t)) ks.warn("WARNING onHubCapsule is Deprecated. Please pass in a callback."), r = t.onHubCapsule.bind(t);
+                        }(t)) ms.warn("WARNING onHubCapsule is Deprecated. Please pass in a callback."), r = t.onHubCapsule.bind(t);
                     else {
                         if ("function" !== typeof t) throw new Error("No callback supplied to Hub");
                         r = t
                     }
                     if (e instanceof RegExp) this.patterns.push({
                         pattern: e,
                         callback: r
@@ -59560,115 +57008,115 @@
                         o._remove(e, r)
                     }
                 }, e.prototype._toListeners = function(e) {
                     var t = e.channel,
                         n = e.payload,
                         r = this.listeners[t];
                     if (r && r.forEach((function(r) {
-                            ks.debug("Dispatching to " + t + " with ", n);
+                            ms.debug("Dispatching to " + t + " with ", n);
                             try {
                                 r.callback(e)
                             } catch (o) {
-                                ks.error(o)
+                                ms.error(o)
                             }
                         })), this.patterns.length > 0) {
-                        if (!n.message) return void ks.warn("Cannot perform pattern matching without a message key");
+                        if (!n.message) return void ms.warn("Cannot perform pattern matching without a message key");
                         var o = n.message;
                         this.patterns.forEach((function(t) {
                             var n = o.match(t.pattern);
                             if (n) {
-                                var r = Ns(n).slice(1),
-                                    i = bs(bs({}, e), {
+                                var r = fs(n).slice(1),
+                                    i = us(us({}, e), {
                                         patternInfo: r
                                     });
                                 try {
                                     t.callback(i)
                                 } catch (a) {
-                                    ks.error(a)
+                                    ms.error(a)
                                 }
                             }
                         }))
                     }
                 }, e
             }(),
-            _s = new Es("__default__"),
-            Ts = {},
-            As = function() {
+            bs = new Ms("__default__"),
+            ws = {},
+            js = function() {
                 function e() {}
                 return e.setItem = function(e, t) {
-                    return Ts[e] = t, Ts[e]
+                    return ws[e] = t, ws[e]
                 }, e.getItem = function(e) {
-                    return Object.prototype.hasOwnProperty.call(Ts, e) ? Ts[e] : void 0
+                    return Object.prototype.hasOwnProperty.call(ws, e) ? ws[e] : void 0
                 }, e.removeItem = function(e) {
-                    return delete Ts[e]
+                    return delete ws[e]
                 }, e.clear = function() {
-                    return Ts = {}
+                    return ws = {}
                 }, e
             }(),
-            Os = function() {
+            xs = function() {
                 function e() {
                     try {
                         this.storageWindow = window.localStorage, this.storageWindow.setItem("aws.amplify.test-ls", 1), this.storageWindow.removeItem("aws.amplify.test-ls")
                     } catch (e) {
-                        this.storageWindow = As
+                        this.storageWindow = js
                     }
                 }
                 return e.prototype.getStorage = function() {
                     return this.storageWindow
                 }, e
             }(),
-            zs = function() {
+            Ns = function() {
                 return {
                     isBrowser: "undefined" !== typeof window && "undefined" !== typeof window.document,
                     isNode: "undefined" !== typeof process && null != process.versions && null != process.versions.node
                 }
             },
-            Us = new Ls("Util"),
-            Ps = function(e) {
+            Is = new ys("Util"),
+            Ds = function(e) {
                 function t(t) {
                     var n = e.call(this, t) || this;
                     return n.nonRetryable = !0, n
                 }
                 return function(e, t) {
                     function n() {
                         this.constructor = e
                     }
-                    Ms(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+                    ss(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
                 }(t, e), t
             }(Error);
-        var Rs = 3e5;
-        var Bs = function(e, t, n, r) {
-                return void 0 === n && (n = Rs),
+        var Ss = 3e5;
+        var Ls = function(e, t, n, r) {
+                return void 0 === n && (n = Ss),
                     function(e, t, n, r) {
-                        return ws(this, void 0, void 0, (function() {
+                        return ls(this, void 0, void 0, (function() {
                             var o = this;
-                            return js(this, (function(i) {
+                            return cs(this, (function(i) {
                                 if ("function" !== typeof e) throw Error("functionToRetry must be a function");
                                 return [2, new Promise((function(i, a) {
-                                    return ws(o, void 0, void 0, (function() {
+                                    return ls(o, void 0, void 0, (function() {
                                         var o, s, u, l, c, d, f;
-                                        return js(this, (function(p) {
+                                        return cs(this, (function(p) {
                                             switch (p.label) {
                                                 case 0:
                                                     o = 0, s = !1, l = function() {}, r && r.then((function() {
                                                         s = !0, clearTimeout(u), l()
                                                     })), d = function() {
                                                         var r, d, f, p;
-                                                        return js(this, (function(h) {
+                                                        return cs(this, (function(h) {
                                                             switch (h.label) {
                                                                 case 0:
-                                                                    o++, Us.debug(e.name + " attempt #" + o + " with this vars: " + JSON.stringify(t)), h.label = 1;
+                                                                    o++, Is.debug(e.name + " attempt #" + o + " with this vars: " + JSON.stringify(t)), h.label = 1;
                                                                 case 1:
-                                                                    return h.trys.push([1, 3, , 7]), r = {}, d = i, [4, e.apply(void 0, Is(t))];
+                                                                    return h.trys.push([1, 3, , 7]), r = {}, d = i, [4, e.apply(void 0, ps(t))];
                                                                 case 2:
                                                                     return [2, (r.value = d.apply(void 0, [h.sent()]), r)];
                                                                 case 3:
-                                                                    return f = h.sent(), c = f, Us.debug("error on " + e.name, f), (g = f) && g.nonRetryable ? (Us.debug(e.name + " non retryable error", f), [2, {
+                                                                    return f = h.sent(), c = f, Is.debug("error on " + e.name, f), (g = f) && g.nonRetryable ? (Is.debug(e.name + " non retryable error", f), [2, {
                                                                         value: a(f)
-                                                                    }]) : (p = n(o, t, f), Us.debug(e.name + " retrying in " + p + " ms"), !1 === p || s ? [2, {
+                                                                    }]) : (p = n(o, t, f), Is.debug(e.name + " retrying in " + p + " ms"), !1 === p || s ? [2, {
                                                                         value: a(f)
                                                                     }] : [3, 4]);
                                                                 case 4:
                                                                     return [4, new Promise((function(e) {
                                                                         l = e, u = setTimeout(l, p)
                                                                     }))];
                                                                 case 5:
@@ -59690,147 +57138,147 @@
                                             }
                                         }))
                                     }))
                                 }))]
                             }))
                         }))
                     }(e, t, function(e) {
-                        return void 0 === e && (e = Rs),
+                        return void 0 === e && (e = Ss),
                             function(t) {
                                 var n = 100 * Math.pow(2, t) + 100 * Math.random();
                                 return !(n > e) && n
                             }
                     }(n), r)
             },
-            Fs = new Ls("CognitoCredentials"),
-            Ys = new Promise((function(e, t) {
-                return zs().isBrowser ? (window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null) ? (Fs.debug("google api already loaded"), e()) : void setTimeout((function() {
+            ks = new ys("CognitoCredentials"),
+            Cs = new Promise((function(e, t) {
+                return Ns().isBrowser ? (window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null) ? (ks.debug("google api already loaded"), e()) : void setTimeout((function() {
                     return e()
-                }), 2e3) : (Fs.debug("not in the browser, directly resolved"), e())
+                }), 2e3) : (ks.debug("not in the browser, directly resolved"), e())
             })),
-            Qs = function() {
+            Es = function() {
                 function e() {
                     this.initialized = !1, this.refreshGoogleToken = this.refreshGoogleToken.bind(this), this._refreshGoogleTokenImpl = this._refreshGoogleTokenImpl.bind(this)
                 }
                 return e.prototype.refreshGoogleToken = function() {
-                    return ws(this, void 0, void 0, (function() {
-                        return js(this, (function(e) {
+                    return ls(this, void 0, void 0, (function() {
+                        return cs(this, (function(e) {
                             switch (e.label) {
                                 case 0:
-                                    return this.initialized ? [3, 2] : (Fs.debug("need to wait for the Google SDK loaded"), [4, Ys]);
+                                    return this.initialized ? [3, 2] : (ks.debug("need to wait for the Google SDK loaded"), [4, Cs]);
                                 case 1:
-                                    e.sent(), this.initialized = !0, Fs.debug("finish waiting"), e.label = 2;
+                                    e.sent(), this.initialized = !0, ks.debug("finish waiting"), e.label = 2;
                                 case 2:
                                     return [2, this._refreshGoogleTokenImpl()]
                             }
                         }))
                     }))
                 }, e.prototype._refreshGoogleTokenImpl = function() {
                     var e = null;
-                    return zs().isBrowser && (e = window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null), e ? new Promise((function(t, n) {
+                    return Ns().isBrowser && (e = window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null), e ? new Promise((function(t, n) {
                         e.getAuthInstance().then((function(e) {
-                            e || (Fs.debug("google Auth undefined"), n(new Ps("google Auth undefined")));
+                            e || (ks.debug("google Auth undefined"), n(new Ds("google Auth undefined")));
                             var r = e.currentUser.get();
-                            r.isSignedIn() ? (Fs.debug("refreshing the google access token"), r.reloadAuthResponse().then((function(e) {
+                            r.isSignedIn() ? (ks.debug("refreshing the google access token"), r.reloadAuthResponse().then((function(e) {
                                 var n = e.id_token,
                                     r = e.expires_at;
                                 t({
                                     token: n,
                                     expires_at: r
                                 })
                             })).catch((function(e) {
-                                e && "network_error" === e.error ? n("Network error reloading google auth response") : n(new Ps("Failed to reload google auth response"))
-                            }))) : n(new Ps("User is not signed in with Google"))
+                                e && "network_error" === e.error ? n("Network error reloading google auth response") : n(new Ds("Failed to reload google auth response"))
+                            }))) : n(new Ds("User is not signed in with Google"))
                         })).catch((function(e) {
-                            Fs.debug("Failed to refresh google token", e), n(new Ps("Failed to refresh google token"))
+                            ks.debug("Failed to refresh google token", e), n(new Ds("Failed to refresh google token"))
                         }))
-                    })) : (Fs.debug("no gapi auth2 available"), Promise.reject("no gapi auth2 available"))
+                    })) : (ks.debug("no gapi auth2 available"), Promise.reject("no gapi auth2 available"))
                 }, e
             }(),
-            Gs = new Ls("CognitoCredentials"),
-            Ws = new Promise((function(e, t) {
-                return zs().isBrowser ? window.FB ? (Gs.debug("FB SDK already loaded"), e()) : void setTimeout((function() {
+            _s = new ys("CognitoCredentials"),
+            Ts = new Promise((function(e, t) {
+                return Ns().isBrowser ? window.FB ? (_s.debug("FB SDK already loaded"), e()) : void setTimeout((function() {
                     return e()
-                }), 2e3) : (Gs.debug("not in the browser, directly resolved"), e())
+                }), 2e3) : (_s.debug("not in the browser, directly resolved"), e())
             })),
-            Hs = function() {
+            As = function() {
                 function e() {
                     this.initialized = !1, this.refreshFacebookToken = this.refreshFacebookToken.bind(this), this._refreshFacebookTokenImpl = this._refreshFacebookTokenImpl.bind(this)
                 }
                 return e.prototype.refreshFacebookToken = function() {
-                    return ws(this, void 0, void 0, (function() {
-                        return js(this, (function(e) {
+                    return ls(this, void 0, void 0, (function() {
+                        return cs(this, (function(e) {
                             switch (e.label) {
                                 case 0:
-                                    return this.initialized ? [3, 2] : (Gs.debug("need to wait for the Facebook SDK loaded"), [4, Ws]);
+                                    return this.initialized ? [3, 2] : (_s.debug("need to wait for the Facebook SDK loaded"), [4, Ts]);
                                 case 1:
-                                    e.sent(), this.initialized = !0, Gs.debug("finish waiting"), e.label = 2;
+                                    e.sent(), this.initialized = !0, _s.debug("finish waiting"), e.label = 2;
                                 case 2:
                                     return [2, this._refreshFacebookTokenImpl()]
                             }
                         }))
                     }))
                 }, e.prototype._refreshFacebookTokenImpl = function() {
                     var e = null;
-                    if (zs().isBrowser && (e = window.FB), !e) {
+                    if (Ns().isBrowser && (e = window.FB), !e) {
                         var t = "no fb sdk available";
-                        return Gs.debug(t), Promise.reject(new Ps(t))
+                        return _s.debug(t), Promise.reject(new Ds(t))
                     }
                     return new Promise((function(t, n) {
                         e.getLoginStatus((function(e) {
                             if (e && e.authResponse) {
                                 var r = e.authResponse,
                                     o = r.accessToken,
                                     i = 1e3 * r.expiresIn + (new Date).getTime();
                                 if (!o) {
                                     a = "the jwtToken is undefined";
-                                    Gs.debug(a), n(new Ps(a))
+                                    _s.debug(a), n(new Ds(a))
                                 }
                                 t({
                                     token: o,
                                     expires_at: i
                                 })
                             } else {
                                 var a = "no response from facebook when refreshing the jwt token";
-                                Gs.debug(a), n(new Ps(a))
+                                _s.debug(a), n(new Ds(a))
                             }
                         }), {
                             scope: "public_profile,email"
                         })
                     }))
                 }, e
             }(),
-            Zs = new Qs,
-            Vs = new Hs,
-            qs = new Ls("Amplify"),
-            Js = new(function() {
+            Os = new Es,
+            zs = new As,
+            Us = new ys("Amplify"),
+            Ps = new(function() {
                 function e() {
-                    this._components = [], this._config = {}, this._modules = {}, this.Auth = null, this.Analytics = null, this.API = null, this.Credentials = null, this.Storage = null, this.I18n = null, this.Cache = null, this.PubSub = null, this.Interactions = null, this.Pushnotification = null, this.UI = null, this.XR = null, this.Predictions = null, this.DataStore = null, this.Geo = null, this.Notifications = null, this.Logger = Ls, this.ServiceWorker = null
+                    this._components = [], this._config = {}, this._modules = {}, this.Auth = null, this.Analytics = null, this.API = null, this.Credentials = null, this.Storage = null, this.I18n = null, this.Cache = null, this.PubSub = null, this.Interactions = null, this.Pushnotification = null, this.UI = null, this.XR = null, this.Predictions = null, this.DataStore = null, this.Geo = null, this.Notifications = null, this.Logger = ys, this.ServiceWorker = null
                 }
                 return e.prototype.register = function(e) {
-                    qs.debug("component registered in amplify", e), this._components.push(e), "function" === typeof e.getModuleName ? (this._modules[e.getModuleName()] = e, this[e.getModuleName()] = e) : qs.debug("no getModuleName method for component", e), e.configure(this._config)
+                    Us.debug("component registered in amplify", e), this._components.push(e), "function" === typeof e.getModuleName ? (this._modules[e.getModuleName()] = e, this[e.getModuleName()] = e) : Us.debug("no getModuleName method for component", e), e.configure(this._config)
                 }, e.prototype.configure = function(e) {
                     var t = this;
-                    return e ? (this._config = Object.assign(this._config, e), qs.debug("amplify config", this._config), Object.entries(this._modules).forEach((function(e) {
-                        var n = Ns(e, 2),
+                    return e ? (this._config = Object.assign(this._config, e), Us.debug("amplify config", this._config), Object.entries(this._modules).forEach((function(e) {
+                        var n = fs(e, 2),
                             r = (n[0], n[1]);
                         Object.keys(r).forEach((function(e) {
                             t._modules[e] && (r[e] = t._modules[e])
                         }))
                     })), this._components.map((function(e) {
                         e.configure(t._config)
                     })), this._config) : this._config
                 }, e.prototype.addPluggable = function(e) {
                     e && e.getCategory && "function" === typeof e.getCategory && this._components.map((function(t) {
                         t.addPluggable && "function" === typeof t.addPluggable && t.addPluggable(e)
                     }))
                 }, e
             }());
 
-        function Ks(e, t, n, r) {
+        function Rs(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -59850,15 +57298,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Xs(e, t) {
+        function Bs(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -59926,15 +57374,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function $s(e, t) {
+        function Fs(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -59947,42 +57395,42 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var eu = function(e, t) {
-            return eu = Object.setPrototypeOf || {
+        var Ys = function(e, t) {
+            return Ys = Object.setPrototypeOf || {
                 __proto__: []
             }
             instanceof Array && function(e, t) {
                 e.__proto__ = t
             } || function(e, t) {
                 for (var n in t) Object.prototype.hasOwnProperty.call(t, n) && (e[n] = t[n])
-            }, eu(e, t)
+            }, Ys(e, t)
         };
 
-        function tu(e, t) {
+        function Qs(e, t) {
             if ("function" !== typeof t && null !== t) throw new TypeError("Class extends value " + String(t) + " is not a constructor or null");
 
             function n() {
                 this.constructor = e
             }
-            eu(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+            Ys(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
         }
-        var nu = function() {
-            return nu = Object.assign || function(e) {
+        var Gs = function() {
+            return Gs = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, nu.apply(this, arguments)
+            }, Gs.apply(this, arguments)
         };
 
-        function ru(e, t, n, r) {
+        function Ws(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -60002,15 +57450,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function ou(e, t) {
+        function Hs(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -60079,15 +57527,15 @@
                         }
                     }([i, s])
                 }
             }
         }
         Object.create;
 
-        function iu(e, t) {
+        function Zs(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -60100,312 +57548,312 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var au, su, uu, lu, cu, du, fu, pu, hu, gu, yu, mu, vu, Mu, bu, wu, ju, xu, Nu, Iu, Du, Su, Lu, ku, Cu, Eu, _u, Tu, Au, Ou, zu, Uu, Pu, Ru, Bu, Fu, Yu, Qu, Gu, Wu, Hu, Zu, Vu, qu, Ju, Ku, Xu, $u, el, tl, nl, rl, ol, il, al, sl, ul;
+        var Vs, qs, Js, Ks, Xs, $s, eu, tu, nu, ru, ou, iu, au, su, uu, lu, cu, du, fu, pu, hu, gu, yu, mu, vu, Mu, bu, wu, ju, xu, Nu, Iu, Du, Su, Lu, ku, Cu, Eu, _u, Tu, Au, Ou, zu, Uu, Pu, Ru, Bu, Fu, Yu, Qu, Gu, Wu, Hu, Zu, Vu, qu, Ju;
         Object.create;
         ! function(e) {
             e.AUTHENTICATED_ROLE = "AuthenticatedRole", e.DENY = "Deny"
+        }(Vs || (Vs = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return Gs({}, e)
+            }
+        }(qs || (qs = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return Gs({}, e)
+            }
+        }(Js || (Js = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return Gs({}, e)
+            }
+        }(Ks || (Ks = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return Gs({}, e)
+            }
+        }(Xs || (Xs = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return Gs({}, e)
+            }
+        }($s || ($s = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return Gs({}, e)
+            }
+        }(eu || (eu = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return Gs({}, e)
+            }
+        }(tu || (tu = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return Gs({}, e)
+            }
+        }(nu || (nu = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return Gs({}, e)
+            }
+        }(ru || (ru = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return Gs({}, e)
+            }
+        }(ou || (ou = {})),
+        function(e) {
+            e.ACCESS_DENIED = "AccessDenied", e.INTERNAL_SERVER_ERROR = "InternalServerError"
+        }(iu || (iu = {})),
+        function(e) {
+            e.filterSensitiveLog = function(e) {
+                return Gs({}, e)
+            }
         }(au || (au = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(su || (su = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(uu || (uu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(lu || (lu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(cu || (cu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(du || (du = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(fu || (fu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(pu || (pu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(hu || (hu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(gu || (gu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(yu || (yu = {})),
         function(e) {
-            e.ACCESS_DENIED = "AccessDenied", e.INTERNAL_SERVER_ERROR = "InternalServerError"
+            e.filterSensitiveLog = function(e) {
+                return Gs({}, e)
+            }
         }(mu || (mu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(vu || (vu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Mu || (Mu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(bu || (bu = {})),
         function(e) {
-            e.filterSensitiveLog = function(e) {
-                return nu({}, e)
-            }
+            e.CONTAINS = "Contains", e.EQUALS = "Equals", e.NOT_EQUAL = "NotEqual", e.STARTS_WITH = "StartsWith"
         }(wu || (wu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(ju || (ju = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(xu || (xu = {})),
         function(e) {
-            e.filterSensitiveLog = function(e) {
-                return nu({}, e)
-            }
+            e.RULES = "Rules", e.TOKEN = "Token"
         }(Nu || (Nu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Iu || (Iu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Du || (Du = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Su || (Su = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Lu || (Lu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(ku || (ku = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Cu || (Cu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Eu || (Eu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(_u || (_u = {})),
         function(e) {
-            e.CONTAINS = "Contains", e.EQUALS = "Equals", e.NOT_EQUAL = "NotEqual", e.STARTS_WITH = "StartsWith"
+            e.filterSensitiveLog = function(e) {
+                return Gs({}, e)
+            }
         }(Tu || (Tu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Au || (Au = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Ou || (Ou = {})),
         function(e) {
-            e.RULES = "Rules", e.TOKEN = "Token"
+            e.filterSensitiveLog = function(e) {
+                return Gs({}, e)
+            }
         }(zu || (zu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Uu || (Uu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Pu || (Pu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Ru || (Ru = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Bu || (Bu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Fu || (Fu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Yu || (Yu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Qu || (Qu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Gu || (Gu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Wu || (Wu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Hu || (Hu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Zu || (Zu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(Vu || (Vu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
         }(qu || (qu = {})),
         function(e) {
             e.filterSensitiveLog = function(e) {
-                return nu({}, e)
-            }
-        }(Ju || (Ju = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return nu({}, e)
-            }
-        }(Ku || (Ku = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return nu({}, e)
-            }
-        }(Xu || (Xu = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return nu({}, e)
+                return Gs({}, e)
             }
-        }($u || ($u = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return nu({}, e)
-            }
-        }(el || (el = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return nu({}, e)
-            }
-        }(tl || (tl = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return nu({}, e)
-            }
-        }(nl || (nl = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return nu({}, e)
-            }
-        }(rl || (rl = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return nu({}, e)
-            }
-        }(ol || (ol = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return nu({}, e)
-            }
-        }(il || (il = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return nu({}, e)
-            }
-        }(al || (al = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return nu({}, e)
-            }
-        }(sl || (sl = {})),
-        function(e) {
-            e.filterSensitiveLog = function(e) {
-                return nu({}, e)
-            }
-        }(ul || (ul = {}));
-        var ll = function() {
+        }(Ju || (Ju = {}));
+        var Ku = function() {
             function e(e) {
                 this.statusCode = e.statusCode, this.headers = e.headers || {}, this.body = e.body
             }
             return e.isInstance = function(e) {
                 if (!e) return !1;
                 var t = e;
                 return "number" === typeof t.statusCode && "object" === typeof t.headers
             }, e
         }();
-        var cl = function() {
-            return cl = Object.assign || function(e) {
+        var Xu = function() {
+            return Xu = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, cl.apply(this, arguments)
+            }, Xu.apply(this, arguments)
         };
 
-        function dl(e, t) {
+        function $u(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -60418,44 +57866,44 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var fl = function() {
+        var el = function() {
             function e(e) {
                 this.method = e.method || "GET", this.hostname = e.hostname || "localhost", this.port = e.port, this.query = e.query || {}, this.headers = e.headers || {}, this.body = e.body, this.protocol = e.protocol ? ":" !== e.protocol.substr(-1) ? e.protocol + ":" : e.protocol : "https:", this.path = e.path ? "/" !== e.path.charAt(0) ? "/" + e.path : e.path : "/"
             }
             return e.isInstance = function(e) {
                 if (!e) return !1;
                 var t = e;
                 return "method" in t && "protocol" in t && "hostname" in t && "path" in t && "object" === typeof t.query && "object" === typeof t.headers
             }, e.prototype.clone = function() {
-                var t, n = new e(cl(cl({}, this), {
-                    headers: cl({}, this.headers)
+                var t, n = new e(Xu(Xu({}, this), {
+                    headers: Xu({}, this.headers)
                 }));
                 return n.query && (n.query = (t = n.query, Object.keys(t).reduce((function(e, n) {
                     var r, o = t[n];
-                    return cl(cl({}, e), ((r = {})[n] = Array.isArray(o) ? function() {
-                        for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(dl(arguments[t]));
+                    return Xu(Xu({}, e), ((r = {})[n] = Array.isArray(o) ? function() {
+                        for (var e = [], t = 0; t < arguments.length; t++) e = e.concat($u(arguments[t]));
                         return e
                     }(o) : o, r))
                 }), {}))), n
             }, e
         }();
-        var pl = function(e, t) {
-                return ru(void 0, void 0, void 0, (function() {
+        var tl = function(e, t) {
+                return Ws(void 0, void 0, void 0, (function() {
                     var n, r, o, i, a, s, u, l, c, d, f, p, h, g, y;
-                    return ou(this, (function(m) {
+                    return Hs(this, (function(m) {
                         switch (m.label) {
                             case 0:
-                                return r = [nu({}, e)], y = {}, [4, Yl(e.body, t)];
+                                return r = [Gs({}, e)], y = {}, [4, Cl(e.body, t)];
                             case 1:
-                                switch (n = nu.apply(void 0, r.concat([(y.body = m.sent(), y)])), i = "UnknownError", i = Ql(e, n.body), i) {
+                                switch (n = Gs.apply(void 0, r.concat([(y.body = m.sent(), y)])), i = "UnknownError", i = El(e, n.body), i) {
                                     case "ExternalServiceException":
                                     case "com.amazonaws.cognitoidentity#ExternalServiceException":
                                         return [3, 2];
                                     case "InternalErrorException":
                                     case "com.amazonaws.cognitoidentity#InternalErrorException":
                                         return [3, 4];
                                     case "InvalidIdentityPoolConfigurationException":
@@ -60475,91 +57923,91 @@
                                         return [3, 14];
                                     case "TooManyRequestsException":
                                     case "com.amazonaws.cognitoidentity#TooManyRequestsException":
                                         return [3, 16]
                                 }
                                 return [3, 18];
                             case 2:
-                                return a = [{}], [4, gl(n, t)];
+                                return a = [{}], [4, rl(n, t)];
                             case 3:
-                                return o = nu.apply(void 0, [nu.apply(void 0, a.concat([m.sent()])), {
+                                return o = Gs.apply(void 0, [Gs.apply(void 0, a.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }]), [3, 19];
                             case 4:
-                                return s = [{}], [4, yl(n, t)];
+                                return s = [{}], [4, ol(n, t)];
                             case 5:
-                                return o = nu.apply(void 0, [nu.apply(void 0, s.concat([m.sent()])), {
+                                return o = Gs.apply(void 0, [Gs.apply(void 0, s.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }]), [3, 19];
                             case 6:
-                                return u = [{}], [4, ml(n, t)];
+                                return u = [{}], [4, il(n, t)];
                             case 7:
-                                return o = nu.apply(void 0, [nu.apply(void 0, u.concat([m.sent()])), {
+                                return o = Gs.apply(void 0, [Gs.apply(void 0, u.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }]), [3, 19];
                             case 8:
-                                return l = [{}], [4, vl(n, t)];
+                                return l = [{}], [4, al(n, t)];
                             case 9:
-                                return o = nu.apply(void 0, [nu.apply(void 0, l.concat([m.sent()])), {
+                                return o = Gs.apply(void 0, [Gs.apply(void 0, l.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }]), [3, 19];
                             case 10:
-                                return c = [{}], [4, bl(n, t)];
+                                return c = [{}], [4, ul(n, t)];
                             case 11:
-                                return o = nu.apply(void 0, [nu.apply(void 0, c.concat([m.sent()])), {
+                                return o = Gs.apply(void 0, [Gs.apply(void 0, c.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }]), [3, 19];
                             case 12:
-                                return d = [{}], [4, wl(n, t)];
+                                return d = [{}], [4, ll(n, t)];
                             case 13:
-                                return o = nu.apply(void 0, [nu.apply(void 0, d.concat([m.sent()])), {
+                                return o = Gs.apply(void 0, [Gs.apply(void 0, d.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }]), [3, 19];
                             case 14:
-                                return f = [{}], [4, jl(n, t)];
+                                return f = [{}], [4, cl(n, t)];
                             case 15:
-                                return o = nu.apply(void 0, [nu.apply(void 0, f.concat([m.sent()])), {
+                                return o = Gs.apply(void 0, [Gs.apply(void 0, f.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }]), [3, 19];
                             case 16:
-                                return p = [{}], [4, xl(n, t)];
+                                return p = [{}], [4, dl(n, t)];
                             case 17:
-                                return o = nu.apply(void 0, [nu.apply(void 0, p.concat([m.sent()])), {
+                                return o = Gs.apply(void 0, [Gs.apply(void 0, p.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }]), [3, 19];
                             case 18:
-                                h = n.body, i = h.code || h.Code || i, o = nu(nu({}, h), {
+                                h = n.body, i = h.code || h.Code || i, o = Gs(Gs({}, h), {
                                     name: "" + i,
                                     message: h.message || h.Message || i,
                                     $fault: "client",
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }), m.label = 19;
                             case 19:
                                 return g = o.message || o.Message || i, o.message = g, delete o.Message, [2, Promise.reject(Object.assign(new Error(g), o))]
                         }
                     }))
                 }))
             },
-            hl = function(e, t) {
-                return ru(void 0, void 0, void 0, (function() {
+            nl = function(e, t) {
+                return Ws(void 0, void 0, void 0, (function() {
                     var n, r, o, i, a, s, u, l, c, d, f, p, h, g, y;
-                    return ou(this, (function(m) {
+                    return Hs(this, (function(m) {
                         switch (m.label) {
                             case 0:
-                                return r = [nu({}, e)], y = {}, [4, Yl(e.body, t)];
+                                return r = [Gs({}, e)], y = {}, [4, Cl(e.body, t)];
                             case 1:
-                                switch (n = nu.apply(void 0, r.concat([(y.body = m.sent(), y)])), i = "UnknownError", i = Ql(e, n.body), i) {
+                                switch (n = Gs.apply(void 0, r.concat([(y.body = m.sent(), y)])), i = "UnknownError", i = El(e, n.body), i) {
                                     case "ExternalServiceException":
                                     case "com.amazonaws.cognitoidentity#ExternalServiceException":
                                         return [3, 2];
                                     case "InternalErrorException":
                                     case "com.amazonaws.cognitoidentity#InternalErrorException":
                                         return [3, 4];
                                     case "InvalidParameterException":
@@ -60579,340 +58027,340 @@
                                         return [3, 14];
                                     case "TooManyRequestsException":
                                     case "com.amazonaws.cognitoidentity#TooManyRequestsException":
                                         return [3, 16]
                                 }
                                 return [3, 18];
                             case 2:
-                                return a = [{}], [4, gl(n, t)];
+                                return a = [{}], [4, rl(n, t)];
                             case 3:
-                                return o = nu.apply(void 0, [nu.apply(void 0, a.concat([m.sent()])), {
+                                return o = Gs.apply(void 0, [Gs.apply(void 0, a.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }]), [3, 19];
                             case 4:
-                                return s = [{}], [4, yl(n, t)];
+                                return s = [{}], [4, ol(n, t)];
                             case 5:
-                                return o = nu.apply(void 0, [nu.apply(void 0, s.concat([m.sent()])), {
+                                return o = Gs.apply(void 0, [Gs.apply(void 0, s.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }]), [3, 19];
                             case 6:
-                                return u = [{}], [4, vl(n, t)];
+                                return u = [{}], [4, al(n, t)];
                             case 7:
-                                return o = nu.apply(void 0, [nu.apply(void 0, u.concat([m.sent()])), {
+                                return o = Gs.apply(void 0, [Gs.apply(void 0, u.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }]), [3, 19];
                             case 8:
-                                return l = [{}], [4, Ml(n, t)];
+                                return l = [{}], [4, sl(n, t)];
                             case 9:
-                                return o = nu.apply(void 0, [nu.apply(void 0, l.concat([m.sent()])), {
+                                return o = Gs.apply(void 0, [Gs.apply(void 0, l.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }]), [3, 19];
                             case 10:
-                                return c = [{}], [4, bl(n, t)];
+                                return c = [{}], [4, ul(n, t)];
                             case 11:
-                                return o = nu.apply(void 0, [nu.apply(void 0, c.concat([m.sent()])), {
+                                return o = Gs.apply(void 0, [Gs.apply(void 0, c.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }]), [3, 19];
                             case 12:
-                                return d = [{}], [4, wl(n, t)];
+                                return d = [{}], [4, ll(n, t)];
                             case 13:
-                                return o = nu.apply(void 0, [nu.apply(void 0, d.concat([m.sent()])), {
+                                return o = Gs.apply(void 0, [Gs.apply(void 0, d.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }]), [3, 19];
                             case 14:
-                                return f = [{}], [4, jl(n, t)];
+                                return f = [{}], [4, cl(n, t)];
                             case 15:
-                                return o = nu.apply(void 0, [nu.apply(void 0, f.concat([m.sent()])), {
+                                return o = Gs.apply(void 0, [Gs.apply(void 0, f.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }]), [3, 19];
                             case 16:
-                                return p = [{}], [4, xl(n, t)];
+                                return p = [{}], [4, dl(n, t)];
                             case 17:
-                                return o = nu.apply(void 0, [nu.apply(void 0, p.concat([m.sent()])), {
+                                return o = Gs.apply(void 0, [Gs.apply(void 0, p.concat([m.sent()])), {
                                     name: i,
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }]), [3, 19];
                             case 18:
-                                h = n.body, i = h.code || h.Code || i, o = nu(nu({}, h), {
+                                h = n.body, i = h.code || h.Code || i, o = Gs(Gs({}, h), {
                                     name: "" + i,
                                     message: h.message || h.Message || i,
                                     $fault: "client",
-                                    $metadata: Rl(e)
+                                    $metadata: Sl(e)
                                 }), m.label = 19;
                             case 19:
                                 return g = o.message || o.Message || i, o.message = g, delete o.Message, [2, Promise.reject(Object.assign(new Error(g), o))]
                         }
                     }))
                 }))
             },
-            gl = function(e, t) {
-                return ru(void 0, void 0, void 0, (function() {
+            rl = function(e, t) {
+                return Ws(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ou(this, (function(o) {
-                        return n = e.body, r = Ll(n, t), [2, nu({
+                    return Hs(this, (function(o) {
+                        return n = e.body, r = yl(n, t), [2, Gs({
                             name: "ExternalServiceException",
                             $fault: "client",
-                            $metadata: Rl(e)
+                            $metadata: Sl(e)
                         }, r)]
                     }))
                 }))
             },
-            yl = function(e, t) {
-                return ru(void 0, void 0, void 0, (function() {
+            ol = function(e, t) {
+                return Ws(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ou(this, (function(o) {
-                        return n = e.body, r = El(n, t), [2, nu({
+                    return Hs(this, (function(o) {
+                        return n = e.body, r = Ml(n, t), [2, Gs({
                             name: "InternalErrorException",
                             $fault: "server",
-                            $metadata: Rl(e)
+                            $metadata: Sl(e)
                         }, r)]
                     }))
                 }))
             },
-            ml = function(e, t) {
-                return ru(void 0, void 0, void 0, (function() {
+            il = function(e, t) {
+                return Ws(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ou(this, (function(o) {
-                        return n = e.body, r = _l(n, t), [2, nu({
+                    return Hs(this, (function(o) {
+                        return n = e.body, r = bl(n, t), [2, Gs({
                             name: "InvalidIdentityPoolConfigurationException",
                             $fault: "client",
-                            $metadata: Rl(e)
+                            $metadata: Sl(e)
                         }, r)]
                     }))
                 }))
             },
-            vl = function(e, t) {
-                return ru(void 0, void 0, void 0, (function() {
+            al = function(e, t) {
+                return Ws(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ou(this, (function(o) {
-                        return n = e.body, r = Tl(n, t), [2, nu({
+                    return Hs(this, (function(o) {
+                        return n = e.body, r = wl(n, t), [2, Gs({
                             name: "InvalidParameterException",
                             $fault: "client",
-                            $metadata: Rl(e)
+                            $metadata: Sl(e)
                         }, r)]
                     }))
                 }))
             },
-            Ml = function(e, t) {
-                return ru(void 0, void 0, void 0, (function() {
+            sl = function(e, t) {
+                return Ws(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ou(this, (function(o) {
-                        return n = e.body, r = Al(n, t), [2, nu({
+                    return Hs(this, (function(o) {
+                        return n = e.body, r = jl(n, t), [2, Gs({
                             name: "LimitExceededException",
                             $fault: "client",
-                            $metadata: Rl(e)
+                            $metadata: Sl(e)
                         }, r)]
                     }))
                 }))
             },
-            bl = function(e, t) {
-                return ru(void 0, void 0, void 0, (function() {
+            ul = function(e, t) {
+                return Ws(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ou(this, (function(o) {
-                        return n = e.body, r = Ol(n, t), [2, nu({
+                    return Hs(this, (function(o) {
+                        return n = e.body, r = xl(n, t), [2, Gs({
                             name: "NotAuthorizedException",
                             $fault: "client",
-                            $metadata: Rl(e)
+                            $metadata: Sl(e)
                         }, r)]
                     }))
                 }))
             },
-            wl = function(e, t) {
-                return ru(void 0, void 0, void 0, (function() {
+            ll = function(e, t) {
+                return Ws(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ou(this, (function(o) {
-                        return n = e.body, r = zl(n, t), [2, nu({
+                    return Hs(this, (function(o) {
+                        return n = e.body, r = Nl(n, t), [2, Gs({
                             name: "ResourceConflictException",
                             $fault: "client",
-                            $metadata: Rl(e)
+                            $metadata: Sl(e)
                         }, r)]
                     }))
                 }))
             },
-            jl = function(e, t) {
-                return ru(void 0, void 0, void 0, (function() {
+            cl = function(e, t) {
+                return Ws(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ou(this, (function(o) {
-                        return n = e.body, r = Ul(n, t), [2, nu({
+                    return Hs(this, (function(o) {
+                        return n = e.body, r = Il(n, t), [2, Gs({
                             name: "ResourceNotFoundException",
                             $fault: "client",
-                            $metadata: Rl(e)
+                            $metadata: Sl(e)
                         }, r)]
                     }))
                 }))
             },
-            xl = function(e, t) {
-                return ru(void 0, void 0, void 0, (function() {
+            dl = function(e, t) {
+                return Ws(void 0, void 0, void 0, (function() {
                     var n, r;
-                    return ou(this, (function(o) {
-                        return n = e.body, r = Pl(n, t), [2, nu({
+                    return Hs(this, (function(o) {
+                        return n = e.body, r = Dl(n, t), [2, Gs({
                             name: "TooManyRequestsException",
                             $fault: "client",
-                            $metadata: Rl(e)
+                            $metadata: Sl(e)
                         }, r)]
                     }))
                 }))
             },
-            Nl = function(e, t) {
-                return nu(nu(nu({}, void 0 !== e.CustomRoleArn && null !== e.CustomRoleArn && {
+            fl = function(e, t) {
+                return Gs(Gs(Gs({}, void 0 !== e.CustomRoleArn && null !== e.CustomRoleArn && {
                     CustomRoleArn: e.CustomRoleArn
                 }), void 0 !== e.IdentityId && null !== e.IdentityId && {
                     IdentityId: e.IdentityId
                 }), void 0 !== e.Logins && null !== e.Logins && {
-                    Logins: Dl(e.Logins, t)
+                    Logins: hl(e.Logins, t)
                 })
             },
-            Il = function(e, t) {
-                return nu(nu(nu({}, void 0 !== e.AccountId && null !== e.AccountId && {
+            pl = function(e, t) {
+                return Gs(Gs(Gs({}, void 0 !== e.AccountId && null !== e.AccountId && {
                     AccountId: e.AccountId
                 }), void 0 !== e.IdentityPoolId && null !== e.IdentityPoolId && {
                     IdentityPoolId: e.IdentityPoolId
                 }), void 0 !== e.Logins && null !== e.Logins && {
-                    Logins: Dl(e.Logins, t)
+                    Logins: hl(e.Logins, t)
                 })
             },
-            Dl = function(e, t) {
+            hl = function(e, t) {
                 return Object.entries(e).reduce((function(e, t) {
-                    var n, r = iu(t, 2),
+                    var n, r = Zs(t, 2),
                         o = r[0],
                         i = r[1];
-                    return null === i ? e : nu(nu({}, e), ((n = {})[o] = i, n))
+                    return null === i ? e : Gs(Gs({}, e), ((n = {})[o] = i, n))
                 }), {})
             },
-            Sl = function(e, t) {
+            gl = function(e, t) {
                 return {
                     AccessKeyId: void 0 !== e.AccessKeyId && null !== e.AccessKeyId ? e.AccessKeyId : void 0,
                     Expiration: void 0 !== e.Expiration && null !== e.Expiration ? new Date(Math.round(1e3 * e.Expiration)) : void 0,
                     SecretKey: void 0 !== e.SecretKey && null !== e.SecretKey ? e.SecretKey : void 0,
                     SessionToken: void 0 !== e.SessionToken && null !== e.SessionToken ? e.SessionToken : void 0
                 }
             },
-            Ll = function(e, t) {
+            yl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            kl = function(e, t) {
+            ml = function(e, t) {
                 return {
-                    Credentials: void 0 !== e.Credentials && null !== e.Credentials ? Sl(e.Credentials) : void 0,
+                    Credentials: void 0 !== e.Credentials && null !== e.Credentials ? gl(e.Credentials) : void 0,
                     IdentityId: void 0 !== e.IdentityId && null !== e.IdentityId ? e.IdentityId : void 0
                 }
             },
-            Cl = function(e, t) {
+            vl = function(e, t) {
                 return {
                     IdentityId: void 0 !== e.IdentityId && null !== e.IdentityId ? e.IdentityId : void 0
                 }
             },
-            El = function(e, t) {
+            Ml = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            _l = function(e, t) {
+            bl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Tl = function(e, t) {
+            wl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Al = function(e, t) {
+            jl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Ol = function(e, t) {
+            xl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            zl = function(e, t) {
+            Nl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Ul = function(e, t) {
+            Il = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Pl = function(e, t) {
+            Dl = function(e, t) {
                 return {
                     message: void 0 !== e.message && null !== e.message ? e.message : void 0
                 }
             },
-            Rl = function(e) {
+            Sl = function(e) {
                 var t;
                 return {
                     httpStatusCode: e.statusCode,
                     requestId: null !== (t = e.headers["x-amzn-requestid"]) && void 0 !== t ? t : e.headers["x-amzn-request-id"],
                     extendedRequestId: e.headers["x-amz-id-2"],
                     cfId: e.headers["x-amz-cf-id"]
                 }
             },
-            Bl = function(e, t) {
+            Ll = function(e, t) {
                 return void 0 === e && (e = new Uint8Array), e instanceof Uint8Array ? Promise.resolve(e) : t.streamCollector(e) || Promise.resolve(new Uint8Array)
             },
-            Fl = function(e, t, n, r, o) {
-                return ru(void 0, void 0, void 0, (function() {
+            kl = function(e, t, n, r, o) {
+                return Ws(void 0, void 0, void 0, (function() {
                     var i, a, s, u, l, c;
-                    return ou(this, (function(d) {
+                    return Hs(this, (function(d) {
                         switch (d.label) {
                             case 0:
                                 return [4, e.endpoint()];
                             case 1:
                                 return i = d.sent(), a = i.hostname, s = i.protocol, u = void 0 === s ? "https" : s, l = i.port, c = {
                                     protocol: u,
                                     hostname: a,
                                     port: l,
                                     method: "POST",
                                     path: n,
                                     headers: t
-                                }, void 0 !== r && (c.hostname = r), void 0 !== o && (c.body = o), [2, new fl(c)]
+                                }, void 0 !== r && (c.hostname = r), void 0 !== o && (c.body = o), [2, new el(c)]
                         }
                     }))
                 }))
             },
-            Yl = function(e, t) {
+            Cl = function(e, t) {
                 return function(e, t) {
-                    return Bl(e, t).then((function(e) {
+                    return Ll(e, t).then((function(e) {
                         return t.utf8Encoder(e)
                     }))
                 }(e, t).then((function(e) {
                     return e.length ? JSON.parse(e) : {}
                 }))
             },
-            Ql = function(e, t) {
+            El = function(e, t) {
                 var n, r, o = function(e) {
                         var t = e;
                         return t.indexOf(":") >= 0 && (t = t.split(":")[0]), t.indexOf("#") >= 0 && (t = t.split("#")[1]), t
                     },
                     i = (n = e.headers, r = "x-amzn-errortype", Object.keys(n).find((function(e) {
                         return e.toLowerCase() === r.toLowerCase()
                     })));
                 return void 0 !== i ? o(e.headers[i]) : void 0 !== t.code ? o(t.code) : void 0 !== t.__type ? o(t.__type) : ""
             };
-        var Gl = function() {
-            return Gl = Object.assign || function(e) {
+        var _l = function() {
+            return _l = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Gl.apply(this, arguments)
+            }, _l.apply(this, arguments)
         };
 
-        function Wl(e, t, n, r) {
+        function Tl(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -60932,15 +58380,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Hl(e, t) {
+        function Al(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -61007,36 +58455,36 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var Zl = {
+        var Ol = {
                 name: "deserializerMiddleware",
                 step: "deserialize",
                 tags: ["DESERIALIZER"],
                 override: !0
             },
-            Vl = {
+            zl = {
                 name: "serializerMiddleware",
                 step: "serialize",
                 tags: ["SERIALIZER"],
                 override: !0
             };
 
-        function ql(e, t, n) {
+        function Ul(e, t, n) {
             return {
                 applyToStack: function(r) {
                     r.add(function(e, t) {
                         return function(n, r) {
                             return function(r) {
-                                return Wl(void 0, void 0, void 0, (function() {
+                                return Tl(void 0, void 0, void 0, (function() {
                                     var o, i;
-                                    return Hl(this, (function(a) {
+                                    return Al(this, (function(a) {
                                         switch (a.label) {
                                             case 0:
                                                 return [4, n(r)];
                                             case 1:
                                                 return o = a.sent().response, [4, t(o, e)];
                                             case 2:
                                                 return i = a.sent(), [2, {
@@ -61044,45 +58492,45 @@
                                                     output: i
                                                 }]
                                         }
                                     }))
                                 }))
                             }
                         }
-                    }(e, n), Zl), r.add(function(e, t) {
+                    }(e, n), Ol), r.add(function(e, t) {
                         return function(n, r) {
                             return function(r) {
-                                return Wl(void 0, void 0, void 0, (function() {
+                                return Tl(void 0, void 0, void 0, (function() {
                                     var o;
-                                    return Hl(this, (function(i) {
+                                    return Al(this, (function(i) {
                                         switch (i.label) {
                                             case 0:
                                                 return [4, t(r.input, e)];
                                             case 1:
-                                                return o = i.sent(), [2, n(Gl(Gl({}, r), {
+                                                return o = i.sent(), [2, n(_l(_l({}, r), {
                                                     request: o
                                                 }))]
                                         }
                                     }))
                                 }))
                             }
                         }
-                    }(e, t), Vl)
+                    }(e, t), zl)
                 }
             }
         }
-        var Jl = function() {
-            return Jl = Object.assign || function(e) {
+        var Pl = function() {
+            return Pl = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Jl.apply(this, arguments)
+            }, Pl.apply(this, arguments)
         };
 
-        function Kl(e) {
+        function Rl(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -61090,15 +58538,15 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function Xl(e, t) {
+        function Bl(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -61112,75 +58560,75 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function $l() {
-            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Xl(arguments[t]));
+        function Fl() {
+            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Bl(arguments[t]));
             return e
         }
-        var ec = function e() {
+        var Yl = function e() {
                 var t = [],
                     n = [],
                     r = new Set,
                     o = function(e) {
                         return t.forEach((function(t) {
-                            e.add(t.middleware, Jl({}, t))
+                            e.add(t.middleware, Pl({}, t))
                         })), n.forEach((function(t) {
-                            e.addRelativeTo(t.middleware, Jl({}, t))
+                            e.addRelativeTo(t.middleware, Pl({}, t))
                         })), e
                     },
                     i = function e(t) {
                         var n = [];
                         return t.before.forEach((function(t) {
-                            0 === t.before.length && 0 === t.after.length ? n.push(t) : n.push.apply(n, $l(e(t)))
+                            0 === t.before.length && 0 === t.after.length ? n.push(t) : n.push.apply(n, Fl(e(t)))
                         })), n.push(t), t.after.reverse().forEach((function(t) {
-                            0 === t.before.length && 0 === t.after.length ? n.push(t) : n.push.apply(n, $l(e(t)))
+                            0 === t.before.length && 0 === t.after.length ? n.push(t) : n.push.apply(n, Fl(e(t)))
                         })), n
                     },
                     a = function() {
                         var e = [],
                             r = [],
                             o = {};
                         t.forEach((function(t) {
-                            var n = Jl(Jl({}, t), {
+                            var n = Pl(Pl({}, t), {
                                 before: [],
                                 after: []
                             });
                             n.name && (o[n.name] = n), e.push(n)
                         })), n.forEach((function(e) {
-                            var t = Jl(Jl({}, e), {
+                            var t = Pl(Pl({}, e), {
                                 before: [],
                                 after: []
                             });
                             t.name && (o[t.name] = t), r.push(t)
                         })), r.forEach((function(e) {
                             if (e.toMiddleware) {
                                 var t = o[e.toMiddleware];
                                 if (void 0 === t) throw new Error(e.toMiddleware + " is not found when adding " + (e.name || "anonymous") + " middleware " + e.relation + " " + e.toMiddleware);
                                 "after" === e.relation && t.after.push(e), "before" === e.relation && t.before.push(e)
                             }
                         }));
                         var a, s = (a = e, a.sort((function(e, t) {
-                            return tc[t.step] - tc[e.step] || nc[t.priority || "normal"] - nc[e.priority || "normal"]
+                            return Ql[t.step] - Ql[e.step] || Gl[t.priority || "normal"] - Gl[e.priority || "normal"]
                         }))).map(i).reduce((function(e, t) {
-                            return e.push.apply(e, $l(t)), e
+                            return e.push.apply(e, Fl(t)), e
                         }), []);
                         return s.map((function(e) {
                             return e.middleware
                         }))
                     },
                     s = {
                         add: function(e, n) {
                             void 0 === n && (n = {});
                             var o = n.name,
                                 i = n.override,
-                                a = Jl({
+                                a = Pl({
                                     step: "initialize",
                                     priority: "normal",
                                     middleware: e
                                 }, n);
                             if (o) {
                                 if (r.has(o)) {
                                     if (!i) throw new Error("Duplicate middleware name '" + o + "'");
@@ -61194,15 +58642,15 @@
                                 r.add(o)
                             }
                             t.push(a)
                         },
                         addRelativeTo: function(e, t) {
                             var o = t.name,
                                 i = t.override,
-                                a = Jl({
+                                a = Pl({
                                     middleware: e
                                 }, t);
                             if (o) {
                                 if (r.has(o)) {
                                     if (!i) throw new Error("Duplicate middleware name '" + o + "'");
                                     var s = n.findIndex((function(e) {
                                             return e.name === o
@@ -61249,15 +58697,15 @@
                             var n = o(e());
                             return n.use(t), n
                         },
                         applyToStack: o,
                         resolve: function(e, t) {
                             var n, r;
                             try {
-                                for (var o = Kl(a().reverse()), i = o.next(); !i.done; i = o.next()) {
+                                for (var o = Rl(a().reverse()), i = o.next(); !i.done; i = o.next()) {
                                     e = (0, i.value)(e, t)
                                 }
                             } catch (s) {
                                 n = {
                                     error: s
                                 }
                             } finally {
@@ -61268,29 +58716,29 @@
                                 }
                             }
                             return e
                         }
                     };
                 return s
             },
-            tc = {
+            Ql = {
                 initialize: 5,
                 serialize: 4,
                 build: 3,
                 finalizeRequest: 2,
                 deserialize: 1
             },
-            nc = {
+            Gl = {
                 high: 3,
                 normal: 2,
                 low: 1
             },
-            rc = function() {
+            Wl = function() {
                 function e(e) {
-                    this.middlewareStack = ec(), this.config = e
+                    this.middlewareStack = Yl(), this.config = e
                 }
                 return e.prototype.send = function(e, t, n) {
                     var r = "function" !== typeof t ? t : void 0,
                         o = "function" === typeof t ? t : n,
                         i = e.resolveMiddleware(this.middlewareStack, this.config, r);
                     if (!o) return i(e).then((function(e) {
                         return e.output
@@ -61300,29 +58748,29 @@
                     }), (function(e) {
                         return o(e)
                     })).catch((function() {}))
                 }, e.prototype.destroy = function() {
                     this.config.requestHandler.destroy && this.config.requestHandler.destroy()
                 }, e
             }(),
-            oc = function() {
-                this.middlewareStack = ec()
+            Hl = function() {
+                this.middlewareStack = Yl()
             },
-            ic = function(e, t) {
-                return ic = Object.setPrototypeOf || {
+            Zl = function(e, t) {
+                return Zl = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
                     for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n])
-                }, ic(e, t)
+                }, Zl(e, t)
             };
 
-        function ac(e, t) {
+        function Vl(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -61336,225 +58784,225 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function sc() {
-            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(ac(arguments[t]));
+        function ql() {
+            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Vl(arguments[t]));
             return e
         }
-        var uc = function() {
+        var Jl = function() {
             var e = Object.getPrototypeOf(this).constructor,
-                t = Function.bind.apply(String, sc([null], arguments)),
+                t = Function.bind.apply(String, ql([null], arguments)),
                 n = new t;
             return Object.setPrototypeOf(n, e.prototype), n
         };
-        uc.prototype = Object.create(String.prototype, {
+        Jl.prototype = Object.create(String.prototype, {
             constructor: {
-                value: uc,
+                value: Jl,
                 enumerable: !1,
                 writable: !0,
                 configurable: !0
             }
-        }), Object.setPrototypeOf(uc, String);
+        }), Object.setPrototypeOf(Jl, String);
         ! function(e) {
             function t() {
                 return null !== e && e.apply(this, arguments) || this
             }(function(e, t) {
                 function n() {
                     this.constructor = e
                 }
-                ic(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+                Zl(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
             })(t, e), t.prototype.deserializeJSON = function() {
                 return JSON.parse(e.prototype.toString.call(this))
             }, t.prototype.toJSON = function() {
                 return e.prototype.toString.call(this)
             }, t.fromObject = function(e) {
                 return e instanceof t ? e : new t(e instanceof String || "string" === typeof e ? e : JSON.stringify(e))
             }
-        }(uc);
-        var lc = function(e) {
+        }(Jl);
+        var Kl = function(e) {
                 function t(t) {
                     var n = e.call(this) || this;
                     return n.input = t, n
                 }
-                return tu(t, e), t.prototype.resolveMiddleware = function(e, t, n) {
-                    this.middlewareStack.use(ql(t, this.serialize, this.deserialize));
+                return Qs(t, e), t.prototype.resolveMiddleware = function(e, t, n) {
+                    this.middlewareStack.use(Ul(t, this.serialize, this.deserialize));
                     var r = e.concat(this.middlewareStack),
                         o = {
                             logger: t.logger,
                             clientName: "CognitoIdentityClient",
                             commandName: "GetCredentialsForIdentityCommand",
-                            inputFilterSensitiveLog: Du.filterSensitiveLog,
-                            outputFilterSensitiveLog: Lu.filterSensitiveLog
+                            inputFilterSensitiveLog: hu.filterSensitiveLog,
+                            outputFilterSensitiveLog: yu.filterSensitiveLog
                         },
                         i = t.requestHandler;
                     return r.resolve((function(e) {
                         return i.handle(e.request, n || {})
                     }), o)
                 }, t.prototype.serialize = function(e, t) {
                     return function(e, t) {
-                        return ru(void 0, void 0, void 0, (function() {
+                        return Ws(void 0, void 0, void 0, (function() {
                             var n, r;
-                            return ou(this, (function(o) {
+                            return Hs(this, (function(o) {
                                 return n = {
                                     "content-type": "application/x-amz-json-1.1",
                                     "x-amz-target": "AWSCognitoIdentityService.GetCredentialsForIdentity"
-                                }, r = JSON.stringify(Nl(e, t)), [2, Fl(t, n, "/", void 0, r)]
+                                }, r = JSON.stringify(fl(e, t)), [2, kl(t, n, "/", void 0, r)]
                             }))
                         }))
                     }(e, t)
                 }, t.prototype.deserialize = function(e, t) {
                     return function(e, t) {
-                        return ru(void 0, void 0, void 0, (function() {
+                        return Ws(void 0, void 0, void 0, (function() {
                             var n, r, o;
-                            return ou(this, (function(i) {
+                            return Hs(this, (function(i) {
                                 switch (i.label) {
                                     case 0:
-                                        return e.statusCode >= 300 ? [2, pl(e, t)] : [4, Yl(e.body, t)];
+                                        return e.statusCode >= 300 ? [2, tl(e, t)] : [4, Cl(e.body, t)];
                                     case 1:
-                                        return n = i.sent(), r = kl(n, t), o = nu({
-                                            $metadata: Rl(e)
+                                        return n = i.sent(), r = ml(n, t), o = Gs({
+                                            $metadata: Sl(e)
                                         }, r), [2, Promise.resolve(o)]
                                 }
                             }))
                         }))
                     }(e, t)
                 }, t
-            }(oc),
-            cc = function(e, t) {
-                return cc = Object.setPrototypeOf || {
+            }(Hl),
+            Xl = function(e, t) {
+                return Xl = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
                     for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n])
-                }, cc(e, t)
+                }, Xl(e, t)
             };
-        var dc = function(e) {
+        var $l = function(e) {
             function t(t, n) {
                 void 0 === n && (n = !0);
                 var r = e.call(this, t) || this;
                 return r.tryNextLink = n, r
             }
             return function(e, t) {
                 function n() {
                     this.constructor = e
                 }
-                cc(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+                Xl(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
             }(t, e), t
         }(Error);
 
-        function fc(e) {
+        function ec(e) {
             return Promise.all(Object.keys(e).reduce((function(t, n) {
                 var r = e[n];
                 return "string" === typeof r ? t.push([n, r]) : t.push(r().then((function(e) {
                     return [n, e]
                 }))), t
             }), [])).then((function(e) {
                 return e.reduce((function(e, t) {
-                    var n = $s(t, 2),
+                    var n = Fs(t, 2),
                         r = n[0],
                         o = n[1];
                     return e[r] = o, e
                 }), {})
             }))
         }
 
-        function pc(e) {
+        function tc(e) {
             var t = this;
             return function() {
-                return Ks(t, void 0, void 0, (function() {
+                return Rs(t, void 0, void 0, (function() {
                     var t, n, r, o, i, a, s, u, l, c, d, f, p;
-                    return Xs(this, (function(h) {
+                    return Bs(this, (function(h) {
                         switch (h.label) {
                             case 0:
-                                return c = (l = e.client).send, d = lc.bind, p = {
+                                return c = (l = e.client).send, d = Kl.bind, p = {
                                     CustomRoleArn: e.customRoleArn,
                                     IdentityId: e.identityId
-                                }, e.logins ? [4, fc(e.logins)] : [3, 2];
+                                }, e.logins ? [4, ec(e.logins)] : [3, 2];
                             case 1:
                                 return f = h.sent(), [3, 3];
                             case 2:
                                 f = void 0, h.label = 3;
                             case 3:
-                                return [4, c.apply(l, [new(d.apply(lc, [void 0, (p.Logins = f, p)]))])];
+                                return [4, c.apply(l, [new(d.apply(Kl, [void 0, (p.Logins = f, p)]))])];
                             case 4:
                                 return t = h.sent().Credentials, n = void 0 === t ? function() {
-                                    throw new dc("Response from Amazon Cognito contained no credentials")
+                                    throw new $l("Response from Amazon Cognito contained no credentials")
                                 }() : t, r = n.AccessKeyId, o = void 0 === r ? function() {
-                                    throw new dc("Response from Amazon Cognito contained no access key ID")
+                                    throw new $l("Response from Amazon Cognito contained no access key ID")
                                 }() : r, i = n.Expiration, a = n.SecretKey, s = void 0 === a ? function() {
-                                    throw new dc("Response from Amazon Cognito contained no secret key")
+                                    throw new $l("Response from Amazon Cognito contained no secret key")
                                 }() : a, u = n.SessionToken, [2, {
                                     identityId: e.identityId,
                                     accessKeyId: o,
                                     secretAccessKey: s,
                                     sessionToken: u,
                                     expiration: i
                                 }]
                         }
                     }))
                 }))
             }
         }
-        var hc = function(e) {
+        var nc = function(e) {
                 function t(t) {
                     var n = e.call(this) || this;
                     return n.input = t, n
                 }
-                return tu(t, e), t.prototype.resolveMiddleware = function(e, t, n) {
-                    this.middlewareStack.use(ql(t, this.serialize, this.deserialize));
+                return Qs(t, e), t.prototype.resolveMiddleware = function(e, t, n) {
+                    this.middlewareStack.use(Ul(t, this.serialize, this.deserialize));
                     var r = e.concat(this.middlewareStack),
                         o = {
                             logger: t.logger,
                             clientName: "CognitoIdentityClient",
                             commandName: "GetIdCommand",
-                            inputFilterSensitiveLog: Cu.filterSensitiveLog,
-                            outputFilterSensitiveLog: Eu.filterSensitiveLog
+                            inputFilterSensitiveLog: vu.filterSensitiveLog,
+                            outputFilterSensitiveLog: Mu.filterSensitiveLog
                         },
                         i = t.requestHandler;
                     return r.resolve((function(e) {
                         return i.handle(e.request, n || {})
                     }), o)
                 }, t.prototype.serialize = function(e, t) {
                     return function(e, t) {
-                        return ru(void 0, void 0, void 0, (function() {
+                        return Ws(void 0, void 0, void 0, (function() {
                             var n, r;
-                            return ou(this, (function(o) {
+                            return Hs(this, (function(o) {
                                 return n = {
                                     "content-type": "application/x-amz-json-1.1",
                                     "x-amz-target": "AWSCognitoIdentityService.GetId"
-                                }, r = JSON.stringify(Il(e, t)), [2, Fl(t, n, "/", void 0, r)]
+                                }, r = JSON.stringify(pl(e, t)), [2, kl(t, n, "/", void 0, r)]
                             }))
                         }))
                     }(e, t)
                 }, t.prototype.deserialize = function(e, t) {
                     return function(e, t) {
-                        return ru(void 0, void 0, void 0, (function() {
+                        return Ws(void 0, void 0, void 0, (function() {
                             var n, r, o;
-                            return ou(this, (function(i) {
+                            return Hs(this, (function(i) {
                                 switch (i.label) {
                                     case 0:
-                                        return e.statusCode >= 300 ? [2, hl(e, t)] : [4, Yl(e.body, t)];
+                                        return e.statusCode >= 300 ? [2, nl(e, t)] : [4, Cl(e.body, t)];
                                     case 1:
-                                        return n = i.sent(), r = Cl(n, t), o = nu({
-                                            $metadata: Rl(e)
+                                        return n = i.sent(), r = vl(n, t), o = Gs({
+                                            $metadata: Sl(e)
                                         }, r), [2, Promise.resolve(o)]
                                 }
                             }))
                         }))
                     }(e, t)
                 }, t
-            }(oc),
-            gc = "IdentityIds",
-            yc = function() {
+            }(Hl),
+            rc = "IdentityIds",
+            oc = function() {
                 function e(e) {
                     void 0 === e && (e = "aws:cognito-identity-ids"), this.dbName = e
                 }
                 return e.prototype.getItem = function(e) {
                     return this.withObjectStore("readonly", (function(t) {
                         var n = t.get(e);
                         return new Promise((function(e) {
@@ -61601,106 +59049,106 @@
                             n(e.error)
                         }, e.onblocked = function() {
                             n(new Error("Unable to access DB"))
                         }, e.onupgradeneeded = function() {
                             var t = e.result;
                             t.onerror = function() {
                                 n(new Error("Failed to create object store"))
-                            }, t.createObjectStore(gc, {
+                            }, t.createObjectStore(rc, {
                                 keyPath: "id"
                             })
                         }
                     }))
                 }, e.prototype.withObjectStore = function(e, t) {
                     return this.getDb().then((function(n) {
-                        var r = n.transaction(gc, e);
+                        var r = n.transaction(rc, e);
                         return r.oncomplete = function() {
                             return n.close()
                         }, new Promise((function(e, n) {
                             r.onerror = function() {
                                 return n(r.error)
-                            }, e(t(r.objectStore(gc)))
+                            }, e(t(r.objectStore(rc)))
                         })).catch((function(e) {
                             throw n.close(), e
                         }))
                     }))
                 }, e
             }(),
-            mc = new(function() {
+            ic = new(function() {
                 function e(e) {
                     void 0 === e && (e = {}), this.store = e
                 }
                 return e.prototype.getItem = function(e) {
                     return e in this.store ? this.store[e] : null
                 }, e.prototype.removeItem = function(e) {
                     delete this.store[e]
                 }, e.prototype.setItem = function(e, t) {
                     this.store[e] = t
                 }, e
             }());
 
-        function vc(e) {
+        function ac(e) {
             var t = this,
                 n = e.accountId,
                 r = e.cache,
-                o = void 0 === r ? "object" === typeof self && self.indexedDB ? new yc : "object" === typeof window && window.localStorage ? window.localStorage : mc : r,
+                o = void 0 === r ? "object" === typeof self && self.indexedDB ? new oc : "object" === typeof window && window.localStorage ? window.localStorage : ic : r,
                 i = e.client,
                 a = e.customRoleArn,
                 s = e.identityPoolId,
                 u = e.logins,
                 l = e.userIdentifier,
                 c = void 0 === l ? u && 0 !== Object.keys(u).length ? void 0 : "ANONYMOUS" : l,
                 d = c ? "aws:cognito-identity-credentials:" + s + ":" + c : void 0,
                 f = function() {
-                    return Ks(t, void 0, void 0, (function() {
+                    return Rs(t, void 0, void 0, (function() {
                         var e, t, r, l, c, p, h, g, y;
-                        return Xs(this, (function(m) {
+                        return Bs(this, (function(m) {
                             switch (m.label) {
                                 case 0:
                                     return (t = d) ? [4, o.getItem(d)] : [3, 2];
                                 case 1:
                                     t = m.sent(), m.label = 2;
                                 case 2:
-                                    return (e = t) ? [3, 7] : (p = (c = i).send, h = hc.bind, y = {
+                                    return (e = t) ? [3, 7] : (p = (c = i).send, h = nc.bind, y = {
                                         AccountId: n,
                                         IdentityPoolId: s
-                                    }, u ? [4, fc(u)] : [3, 4]);
+                                    }, u ? [4, ec(u)] : [3, 4]);
                                 case 3:
                                     return g = m.sent(), [3, 5];
                                 case 4:
                                     g = void 0, m.label = 5;
                                 case 5:
-                                    return [4, p.apply(c, [new(h.apply(hc, [void 0, (y.Logins = g, y)]))])];
+                                    return [4, p.apply(c, [new(h.apply(nc, [void 0, (y.Logins = g, y)]))])];
                                 case 6:
                                     r = m.sent().IdentityId, l = void 0 === r ? function() {
-                                        throw new dc("Response from Amazon Cognito contained no identity ID")
+                                        throw new $l("Response from Amazon Cognito contained no identity ID")
                                     }() : r, e = l, d && Promise.resolve(o.setItem(d, e)).catch((function() {})), m.label = 7;
                                 case 7:
-                                    return [2, (f = pc({
+                                    return [2, (f = tc({
                                         client: i,
                                         customRoleArn: a,
                                         logins: u,
                                         identityId: e
                                     }))()]
                             }
                         }))
                     }))
                 };
             return function() {
                 return f().catch((function(e) {
-                    return Ks(t, void 0, void 0, (function() {
-                        return Xs(this, (function(t) {
+                    return Rs(t, void 0, void 0, (function() {
+                        return Bs(this, (function(t) {
                             throw d && Promise.resolve(o.removeItem(d)).catch((function() {})), e
                         }))
                     }))
                 }))
             }
         }
-        var Mc = new Ls("Parser"),
-            bc = function(e) {
+        var sc = new ys("Parser"),
+            uc = function(e) {
                 var t, n = {};
                 if (e.aws_mobile_analytics_app_id) {
                     var r = {
                         AWSPinpoint: {
                             appId: e.aws_mobile_analytics_app_id,
                             region: e.aws_mobile_analytics_app_region
                         }
@@ -61717,23 +59165,23 @@
                     signUpVerificationMethod: e.aws_cognito_sign_up_verification_method || "code"
                 }), t = e.aws_user_files_s3_bucket ? {
                     AWSS3: {
                         bucket: e.aws_user_files_s3_bucket,
                         region: e.aws_user_files_s3_bucket_region,
                         dangerouslyConnectToHttpEndpointForTesting: e.aws_user_files_s3_dangerously_connect_to_http_endpoint_for_testing
                     }
-                } : e ? e.Storage || e : {}, e.Logging && (n.Logging = bs(bs({}, e.Logging), {
+                } : e ? e.Storage || e : {}, e.Logging && (n.Logging = us(us({}, e.Logging), {
                     region: e.aws_project_region
                 })), e.geo && (n.Geo = Object.assign({}, e.geo), e.geo.amazon_location_service && (n.Geo = {
                     AmazonLocationService: e.geo.amazon_location_service
-                })), n.Analytics = Object.assign({}, n.Analytics, e.Analytics), n.Auth = Object.assign({}, n.Auth, e.Auth), n.Storage = Object.assign({}, t), n.Logging = Object.assign({}, n.Logging, e.Logging), Mc.debug("parse config", e, "to amplifyconfig", n), n
+                })), n.Analytics = Object.assign({}, n.Analytics, e.Analytics), n.Auth = Object.assign({}, n.Auth, e.Auth), n.Storage = Object.assign({}, t), n.Logging = Object.assign({}, n.Logging, e.Logging), sc.debug("parse config", e, "to amplifyconfig", n), n
             },
-            wc = __webpack_require__(3219);
+            lc = __webpack_require__(3219);
 
-        function jc(e, t, n, r) {
+        function cc(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -61753,15 +59201,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function xc(e, t) {
+        function dc(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -61829,15 +59277,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function Nc(e) {
+        function fc(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -61845,36 +59293,36 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function Ic(e) {
+        function pc(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
                         value: e && e[r++],
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
-        var Dc = function(e) {
-                return encodeURIComponent(e).replace(/[!'()*]/g, Sc)
+        var hc = function(e) {
+                return encodeURIComponent(e).replace(/[!'()*]/g, gc)
             },
-            Sc = function(e) {
+            gc = function(e) {
                 return "%" + e.charCodeAt(0).toString(16).toUpperCase()
             };
-        for (var Lc = function() {
+        for (var yc = function() {
                 function e(e) {
                     var t = (void 0 === e ? {} : e).requestTimeout;
                     this.requestTimeout = t
                 }
                 return e.prototype.destroy = function() {}, e.prototype.handle = function(e, t) {
                     var n = (void 0 === t ? {} : t).abortSignal,
                         r = this.requestTimeout;
@@ -61883,22 +59331,22 @@
                         return o.name = "AbortError", Promise.reject(o)
                     }
                     var i = e.path;
                     if (e.query) {
                         var a = function(e) {
                             var t, n, r = [];
                             try {
-                                for (var o = Ic(Object.keys(e).sort()), i = o.next(); !i.done; i = o.next()) {
+                                for (var o = pc(Object.keys(e).sort()), i = o.next(); !i.done; i = o.next()) {
                                     var a = i.value,
                                         s = e[a];
-                                    if (a = Dc(a), Array.isArray(s))
-                                        for (var u = 0, l = s.length; u < l; u++) r.push(a + "=" + Dc(s[u]));
+                                    if (a = hc(a), Array.isArray(s))
+                                        for (var u = 0, l = s.length; u < l; u++) r.push(a + "=" + hc(s[u]));
                                     else {
                                         var c = a;
-                                        (s || "string" === typeof s) && (c += "=" + Dc(s)), r.push(c)
+                                        (s || "string" === typeof s) && (c += "=" + hc(s)), r.push(c)
                                     }
                                 }
                             } catch (d) {
                                 t = {
                                     error: d
                                 }
                             } finally {
@@ -61922,15 +59370,15 @@
                         };
                     "undefined" !== typeof AbortController && (c.signal = n);
                     var d, f = new Request(l, c),
                         p = [fetch(f).then((function(e) {
                             var t, n, r = e.headers,
                                 o = {};
                             try {
-                                for (var i = Nc(r.entries()), a = i.next(); !a.done; a = i.next()) {
+                                for (var i = fc(r.entries()), a = i.next(); !a.done; a = i.next()) {
                                     var s = a.value;
                                     o[s[0]] = s[1]
                                 }
                             } catch (u) {
                                 t = {
                                     error: u
                                 }
@@ -61938,22 +59386,22 @@
                                 try {
                                     a && !a.done && (n = i.return) && n.call(i)
                                 } finally {
                                     if (t) throw t.error
                                 }
                             }
                             return void 0 !== e.body ? {
-                                response: new ll({
+                                response: new Ku({
                                     headers: o,
                                     statusCode: e.status,
                                     body: e.body
                                 })
                             } : e.blob().then((function(t) {
                                 return {
-                                    response: new ll({
+                                    response: new Ku({
                                         headers: o,
                                         statusCode: e.status,
                                         body: t
                                     })
                                 }
                             }))
                         })), (d = r, void 0 === d && (d = 0), new Promise((function(e, t) {
@@ -61965,46 +59413,46 @@
                     return n && p.push(new Promise((function(e, t) {
                         n.onabort = function() {
                             var e = new Error("Request aborted");
                             e.name = "AbortError", t(e)
                         }
                     }))), Promise.race(p)
                 }, e
-            }(), kc = {}, Cc = new Array(64), Ec = 0, _c = "A".charCodeAt(0), Tc = "Z".charCodeAt(0); Ec + _c <= Tc; Ec++) {
-            var Ac = String.fromCharCode(Ec + _c);
-            kc[Ac] = Ec, Cc[Ec] = Ac
-        }
-        for (Ec = 0, _c = "a".charCodeAt(0), Tc = "z".charCodeAt(0); Ec + _c <= Tc; Ec++) {
-            Ac = String.fromCharCode(Ec + _c);
-            var Oc = Ec + 26;
-            kc[Ac] = Oc, Cc[Oc] = Ac
-        }
-        for (Ec = 0; Ec < 10; Ec++) {
-            kc[Ec.toString(10)] = Ec + 52;
-            Ac = Ec.toString(10), Oc = Ec + 52;
-            kc[Ac] = Oc, Cc[Oc] = Ac
+            }(), mc = {}, vc = new Array(64), Mc = 0, bc = "A".charCodeAt(0), wc = "Z".charCodeAt(0); Mc + bc <= wc; Mc++) {
+            var jc = String.fromCharCode(Mc + bc);
+            mc[jc] = Mc, vc[Mc] = jc
+        }
+        for (Mc = 0, bc = "a".charCodeAt(0), wc = "z".charCodeAt(0); Mc + bc <= wc; Mc++) {
+            jc = String.fromCharCode(Mc + bc);
+            var xc = Mc + 26;
+            mc[jc] = xc, vc[xc] = jc
+        }
+        for (Mc = 0; Mc < 10; Mc++) {
+            mc[Mc.toString(10)] = Mc + 52;
+            jc = Mc.toString(10), xc = Mc + 52;
+            mc[jc] = xc, vc[xc] = jc
         }
-        kc["+"] = 62, Cc[62] = "+", kc["/"] = 63, Cc[63] = "/";
+        mc["+"] = 62, vc[62] = "+", mc["/"] = 63, vc[63] = "/";
 
-        function zc(e) {
+        function Nc(e) {
             var t = e.length / 4 * 3;
             "==" === e.substr(-2) ? t -= 2 : "=" === e.substr(-1) && t--;
             for (var n = new ArrayBuffer(t), r = new DataView(n), o = 0; o < e.length; o += 4) {
-                for (var i = 0, a = 0, s = o, u = o + 3; s <= u; s++) "=" !== e[s] ? (i |= kc[e[s]] << 6 * (u - s), a += 6) : i >>= 6;
+                for (var i = 0, a = 0, s = o, u = o + 3; s <= u; s++) "=" !== e[s] ? (i |= mc[e[s]] << 6 * (u - s), a += 6) : i >>= 6;
                 var l = o / 4 * 3;
                 i >>= a % 8;
                 for (var c = Math.floor(a / 8), d = 0; d < c; d++) {
                     var f = 8 * (c - d - 1);
                     r.setUint8(l + d, (i & 255 << f) >> f)
                 }
             }
             return new Uint8Array(n)
         }
 
-        function Uc(e) {
+        function Ic(e) {
             return new Promise((function(t, n) {
                 var r = new FileReader;
                 r.onloadend = function() {
                     var e;
                     if (2 !== r.readyState) return n(new Error("Reader aborted too early"));
                     var o = null !== (e = r.result) && void 0 !== e ? e : "",
                         i = o.indexOf(","),
@@ -62013,23 +59461,23 @@
                 }, r.onabort = function() {
                     return n(new Error("Read aborted"))
                 }, r.onerror = function() {
                     return n(r.error)
                 }, r.readAsDataURL(e)
             }))
         }
-        var Pc = function() {
-            return Pc = Object.assign || function(e) {
+        var Dc = function() {
+            return Dc = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Pc.apply(this, arguments)
+            }, Dc.apply(this, arguments)
         };
 
-        function Rc(e, t, n, r) {
+        function Sc(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -62049,15 +59497,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Bc(e, t) {
+        function Lc(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -62125,15 +59573,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function Fc(e, t) {
+        function kc(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -62146,65 +59594,65 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var Yc = function(e) {
+        var Cc = function(e) {
                 return function(t, n) {
                     return function(r) {
-                        return Rc(void 0, void 0, void 0, (function() {
+                        return Sc(void 0, void 0, void 0, (function() {
                             var o;
-                            return Bc(this, (function(i) {
+                            return Lc(this, (function(i) {
                                 return (null === (o = null === e || void 0 === e ? void 0 : e.retryStrategy) || void 0 === o ? void 0 : o.mode) && (n.userAgent = function() {
-                                    for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Fc(arguments[t]));
+                                    for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(kc(arguments[t]));
                                     return e
                                 }(n.userAgent || [], [
                                     ["cfg/retry-mode", e.retryStrategy.mode]
                                 ])), [2, e.retryStrategy.retry(t, r)]
                             }))
                         }))
                     }
                 }
             },
-            Qc = {
+            Ec = {
                 name: "retryMiddleware",
                 tags: ["RETRY"],
                 step: "finalizeRequest",
                 priority: "high",
                 override: !0
             },
-            Gc = ["AuthFailure", "InvalidSignatureException", "RequestExpired", "RequestInTheFuture", "RequestTimeTooSkewed", "SignatureDoesNotMatch"],
-            Wc = ["BandwidthLimitExceeded", "EC2ThrottledException", "LimitExceededException", "PriorRequestNotComplete", "ProvisionedThroughputExceededException", "RequestLimitExceeded", "RequestThrottled", "RequestThrottledException", "SlowDown", "ThrottledException", "Throttling", "ThrottlingException", "TooManyRequestsException", "TransactionInProgressException"],
-            Hc = ["AbortError", "TimeoutError", "RequestTimeout", "RequestTimeoutException"],
-            Zc = [500, 502, 503, 504],
-            Vc = function(e) {
+            _c = ["AuthFailure", "InvalidSignatureException", "RequestExpired", "RequestInTheFuture", "RequestTimeTooSkewed", "SignatureDoesNotMatch"],
+            Tc = ["BandwidthLimitExceeded", "EC2ThrottledException", "LimitExceededException", "PriorRequestNotComplete", "ProvisionedThroughputExceededException", "RequestLimitExceeded", "RequestThrottled", "RequestThrottledException", "SlowDown", "ThrottledException", "Throttling", "ThrottlingException", "TooManyRequestsException", "TransactionInProgressException"],
+            Ac = ["AbortError", "TimeoutError", "RequestTimeout", "RequestTimeoutException"],
+            Oc = [500, 502, 503, 504],
+            zc = function(e) {
                 var t, n;
-                return 429 === (null === (t = e.$metadata) || void 0 === t ? void 0 : t.httpStatusCode) || Wc.includes(e.name) || 1 == (null === (n = e.$retryable) || void 0 === n ? void 0 : n.throttling)
+                return 429 === (null === (t = e.$metadata) || void 0 === t ? void 0 : t.httpStatusCode) || Tc.includes(e.name) || 1 == (null === (n = e.$retryable) || void 0 === n ? void 0 : n.throttling)
             },
-            qc = __webpack_require__(6231),
-            Jc = function(e, t) {
+            Uc = __webpack_require__(6231),
+            Pc = function(e, t) {
                 return Math.floor(Math.min(2e4, Math.random() * Math.pow(2, t) * e))
             },
-            Kc = function(e) {
+            Rc = function(e) {
                 return !!e && (function(e) {
                     return void 0 !== e.$retryable
                 }(e) || function(e) {
-                    return Gc.includes(e.name)
-                }(e) || Vc(e) || function(e) {
+                    return _c.includes(e.name)
+                }(e) || zc(e) || function(e) {
                     var t;
-                    return Hc.includes(e.name) || Zc.includes((null === (t = e.$metadata) || void 0 === t ? void 0 : t.httpStatusCode) || 0)
+                    return Ac.includes(e.name) || Oc.includes((null === (t = e.$metadata) || void 0 === t ? void 0 : t.httpStatusCode) || 0)
                 }(e))
             },
-            Xc = "standard",
-            $c = function() {
+            Bc = "standard",
+            Fc = function() {
                 function e(e, t) {
                     var n, r, o;
-                    this.maxAttemptsProvider = e, this.mode = Xc, this.retryDecider = null !== (n = null === t || void 0 === t ? void 0 : t.retryDecider) && void 0 !== n ? n : Kc, this.delayDecider = null !== (r = null === t || void 0 === t ? void 0 : t.delayDecider) && void 0 !== r ? r : Jc, this.retryQuota = null !== (o = null === t || void 0 === t ? void 0 : t.retryQuota) && void 0 !== o ? o : function(e) {
+                    this.maxAttemptsProvider = e, this.mode = Bc, this.retryDecider = null !== (n = null === t || void 0 === t ? void 0 : t.retryDecider) && void 0 !== n ? n : Rc, this.delayDecider = null !== (r = null === t || void 0 === t ? void 0 : t.delayDecider) && void 0 !== r ? r : Pc, this.retryQuota = null !== (o = null === t || void 0 === t ? void 0 : t.retryQuota) && void 0 !== o ? o : function(e) {
                         var t = e,
                             n = e,
                             r = function(e) {
                                 return "TimeoutError" === e.name ? 10 : 5
                             },
                             o = function(e) {
                                 return r(e) <= n
@@ -62221,52 +59669,52 @@
                             }
                         })
                     }(500)
                 }
                 return e.prototype.shouldRetry = function(e, t, n) {
                     return t < n && this.retryDecider(e) && this.retryQuota.hasRetryTokens(e)
                 }, e.prototype.getMaxAttempts = function() {
-                    return Rc(this, void 0, void 0, (function() {
+                    return Sc(this, void 0, void 0, (function() {
                         var e;
-                        return Bc(this, (function(t) {
+                        return Lc(this, (function(t) {
                             switch (t.label) {
                                 case 0:
                                     return t.trys.push([0, 2, , 3]), [4, this.maxAttemptsProvider()];
                                 case 1:
                                     return e = t.sent(), [3, 3];
                                 case 2:
                                     return t.sent(), e = 3, [3, 3];
                                 case 3:
                                     return [2, e]
                             }
                         }))
                     }))
                 }, e.prototype.retry = function(e, t) {
-                    return Rc(this, void 0, void 0, (function() {
+                    return Sc(this, void 0, void 0, (function() {
                         var n, r, o, i, a, s, u, l;
-                        return Bc(this, (function(c) {
+                        return Lc(this, (function(c) {
                             switch (c.label) {
                                 case 0:
                                     return r = 0, o = 0, [4, this.getMaxAttempts()];
                                 case 1:
-                                    i = c.sent(), a = t.request, fl.isInstance(a) && (a.headers["amz-sdk-invocation-id"] = (0, qc.v4)()), s = function() {
+                                    i = c.sent(), a = t.request, el.isInstance(a) && (a.headers["amz-sdk-invocation-id"] = (0, Uc.v4)()), s = function() {
                                         var s, l, c, d, f;
-                                        return Bc(this, (function(p) {
+                                        return Lc(this, (function(p) {
                                             switch (p.label) {
                                                 case 0:
-                                                    return p.trys.push([0, 2, , 5]), fl.isInstance(a) && (a.headers["amz-sdk-request"] = "attempt=" + (r + 1) + "; max=" + i), [4, e(t)];
+                                                    return p.trys.push([0, 2, , 5]), el.isInstance(a) && (a.headers["amz-sdk-request"] = "attempt=" + (r + 1) + "; max=" + i), [4, e(t)];
                                                 case 1:
                                                     return s = p.sent(), l = s.response, c = s.output, u.retryQuota.releaseRetryTokens(n), c.$metadata.attempts = r + 1, c.$metadata.totalRetryDelay = o, [2, {
                                                         value: {
                                                             response: l,
                                                             output: c
                                                         }
                                                     }];
                                                 case 2:
-                                                    return d = p.sent(), r++, u.shouldRetry(d, r, i) ? (n = u.retryQuota.retrieveRetryTokens(d), f = u.delayDecider(Vc(d) ? 500 : 100, r), o += f, [4, new Promise((function(e) {
+                                                    return d = p.sent(), r++, u.shouldRetry(d, r, i) ? (n = u.retryQuota.retrieveRetryTokens(d), f = u.delayDecider(zc(d) ? 500 : 100, r), o += f, [4, new Promise((function(e) {
                                                         return setTimeout(e, f)
                                                     }))]) : [3, 4];
                                                 case 3:
                                                     return p.sent(), [2, "continue"];
                                                 case 4:
                                                     throw d.$metadata || (d.$metadata = {}), d.$metadata.attempts = r, d.$metadata.totalRetryDelay = o, d;
                                                 case 5:
@@ -62281,25 +59729,25 @@
                                 case 4:
                                     return [2]
                             }
                         }))
                     }))
                 }, e
             }(),
-            ed = function(e) {
+            Yc = function(e) {
                 if (void 0 === e && (e = 3), "number" === typeof e) {
                     var t = Promise.resolve(e);
                     return function() {
                         return t
                     }
                 }
                 return e
             };
 
-        function td(e, t, n, r) {
+        function Qc(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -62319,15 +59767,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function nd(e, t) {
+        function Gc(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -62394,25 +59842,25 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var rd = __webpack_require__(984),
-            od = __webpack_require__.n(rd),
-            id = __webpack_require__(5863),
-            ad = "cognito-identity.{region}.amazonaws.com",
-            sd = new Set(["af-south-1", "ap-east-1", "ap-northeast-1", "ap-northeast-2", "ap-south-1", "ap-southeast-1", "ap-southeast-2", "ca-central-1", "eu-central-1", "eu-north-1", "eu-south-1", "eu-west-1", "eu-west-2", "eu-west-3", "me-south-1", "sa-east-1", "us-east-1", "us-east-2", "us-west-1", "us-west-2"]),
-            ud = new Set(["cn-north-1", "cn-northwest-1"]),
-            ld = new Set(["us-iso-east-1"]),
-            cd = new Set(["us-isob-east-1"]),
-            dd = new Set(["us-gov-east-1", "us-gov-west-1"]);
+        var Wc = __webpack_require__(984),
+            Hc = __webpack_require__.n(Wc),
+            Zc = __webpack_require__(5863),
+            Vc = "cognito-identity.{region}.amazonaws.com",
+            qc = new Set(["af-south-1", "ap-east-1", "ap-northeast-1", "ap-northeast-2", "ap-south-1", "ap-southeast-1", "ap-southeast-2", "ca-central-1", "eu-central-1", "eu-north-1", "eu-south-1", "eu-west-1", "eu-west-2", "eu-west-3", "me-south-1", "sa-east-1", "us-east-1", "us-east-2", "us-west-1", "us-west-2"]),
+            Jc = new Set(["cn-north-1", "cn-northwest-1"]),
+            Kc = new Set(["us-iso-east-1"]),
+            Xc = new Set(["us-isob-east-1"]),
+            $c = new Set(["us-gov-east-1", "us-gov-west-1"]);
 
-        function fd(e) {
+        function ed(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -62420,15 +59868,15 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function pd(e, t) {
+        function td(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -62441,15 +59889,15 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var hd, gd = {
+        var nd, rd = {
                 apiVersion: "2014-06-30",
                 disableHostPrefix: !1,
                 logger: {},
                 regionInfoProvider: function(e, t) {
                     var n = void 0;
                     switch (e) {
                         case "ap-northeast-1":
@@ -62585,51 +60033,51 @@
                         case "us-west-2":
                             n = {
                                 hostname: "cognito-identity.us-west-2.amazonaws.com",
                                 partition: "aws"
                             };
                             break;
                         default:
-                            sd.has(e) && (n = {
-                                hostname: ad.replace("{region}", e),
+                            qc.has(e) && (n = {
+                                hostname: Vc.replace("{region}", e),
                                 partition: "aws"
-                            }), ud.has(e) && (n = {
+                            }), Jc.has(e) && (n = {
                                 hostname: "cognito-identity.{region}.amazonaws.com.cn".replace("{region}", e),
                                 partition: "aws-cn"
-                            }), ld.has(e) && (n = {
+                            }), Kc.has(e) && (n = {
                                 hostname: "cognito-identity.{region}.c2s.ic.gov".replace("{region}", e),
                                 partition: "aws-iso"
-                            }), cd.has(e) && (n = {
+                            }), Xc.has(e) && (n = {
                                 hostname: "cognito-identity.{region}.sc2s.sgov.gov".replace("{region}", e),
                                 partition: "aws-iso-b"
-                            }), dd.has(e) && (n = {
+                            }), $c.has(e) && (n = {
                                 hostname: "cognito-identity.{region}.amazonaws.com".replace("{region}", e),
                                 partition: "aws-us-gov"
                             }), void 0 === n && (n = {
-                                hostname: ad.replace("{region}", e),
+                                hostname: Vc.replace("{region}", e),
                                 partition: "aws"
                             })
                     }
-                    return Promise.resolve(nu({
+                    return Promise.resolve(Gs({
                         signingService: "cognito-identity"
                     }, n))
                 },
                 serviceId: "Cognito Identity",
                 urlParser: function(e) {
                     var t, n = new URL(e),
                         r = n.hostname,
                         o = n.pathname,
                         i = n.port,
                         a = n.protocol,
                         s = n.search;
                     return s && (t = function(e) {
                         var t, n, r = {};
                         if (e = e.replace(/^\?/, "")) try {
-                            for (var o = fd(e.split("&")), i = o.next(); !i.done; i = o.next()) {
-                                var a = pd(i.value.split("="), 2),
+                            for (var o = ed(e.split("&")), i = o.next(); !i.done; i = o.next()) {
+                                var a = td(i.value.split("="), 2),
                                     s = a[0],
                                     u = a[1],
                                     l = void 0 === u ? null : u;
                                 s = decodeURIComponent(s), l && (l = decodeURIComponent(l)), s in r ? Array.isArray(r[s]) ? r[s].push(l) : r[s] = [r[s], l] : r[s] = l
                             }
                         } catch (c) {
                             t = {
@@ -62648,25 +60096,25 @@
                         port: i ? parseInt(i) : void 0,
                         protocol: a,
                         path: o,
                         query: t
                     }
                 }
             },
-            yd = nu(nu({}, gd), {
+            od = Gs(Gs({}, rd), {
                 runtime: "browser",
-                base64Decoder: zc,
+                base64Decoder: Nc,
                 base64Encoder: function(e) {
                     for (var t = "", n = 0; n < e.length; n += 3) {
                         for (var r = 0, o = 0, i = n, a = Math.min(n + 3, e.length); i < a; i++) r |= e[i] << 8 * (a - i - 1), o += 8;
                         var s = Math.ceil(o / 6);
                         r <<= 6 * s - o;
                         for (var u = 1; u <= s; u++) {
                             var l = 6 * (s - u);
-                            t += Cc[(r & 63 << l) >> l]
+                            t += vc[(r & 63 << l) >> l]
                         }
                         t += "==".slice(0, 4 - s)
                     }
                     return t
                 },
                 bodyLengthChecker: function(e) {
                     if ("string" === typeof e) {
@@ -62683,79 +60131,79 @@
                         return Promise.reject(new Error("Credential is missing"))
                     }
                 },
                 defaultUserAgentProvider: function(e) {
                     var t = e.serviceId,
                         n = e.clientVersion;
                     return function() {
-                        return td(void 0, void 0, void 0, (function() {
+                        return Qc(void 0, void 0, void 0, (function() {
                             var e, r, o, i, a, s, u, l, c;
-                            return nd(this, (function(d) {
-                                return e = (null === (o = null === window || void 0 === window ? void 0 : window.navigator) || void 0 === o ? void 0 : o.userAgent) ? od().parse(window.navigator.userAgent) : void 0, r = [
+                            return Gc(this, (function(d) {
+                                return e = (null === (o = null === window || void 0 === window ? void 0 : window.navigator) || void 0 === o ? void 0 : o.userAgent) ? Hc().parse(window.navigator.userAgent) : void 0, r = [
                                     ["aws-sdk-js", n],
                                     ["os/" + ((null === (i = null === e || void 0 === e ? void 0 : e.os) || void 0 === i ? void 0 : i.name) || "other"), null === (a = null === e || void 0 === e ? void 0 : e.os) || void 0 === a ? void 0 : a.version],
                                     ["lang/js"],
                                     ["md/browser", (null !== (u = null === (s = null === e || void 0 === e ? void 0 : e.browser) || void 0 === s ? void 0 : s.name) && void 0 !== u ? u : "unknown") + "_" + (null !== (c = null === (l = null === e || void 0 === e ? void 0 : e.browser) || void 0 === l ? void 0 : l.version) && void 0 !== c ? c : "unknown")]
                                 ], t && r.push(["api/" + t, n]), [2, r]
                             }))
                         }))
                     }
                 }({
-                    serviceId: gd.serviceId,
+                    serviceId: rd.serviceId,
                     clientVersion: "3.6.1"
                 }),
                 maxAttempts: 3,
-                region: (hd = "Region is missing", function() {
-                    return Promise.reject(hd)
+                region: (nd = "Region is missing", function() {
+                    return Promise.reject(nd)
                 }),
-                requestHandler: new Lc,
-                sha256: wc.Sha256,
+                requestHandler: new yc,
+                sha256: lc.Sha256,
                 streamCollector: function(e) {
                     return "function" === typeof Blob && e instanceof Blob ? function(e) {
-                        return jc(this, void 0, void 0, (function() {
+                        return cc(this, void 0, void 0, (function() {
                             var t, n;
-                            return xc(this, (function(r) {
+                            return dc(this, (function(r) {
                                 switch (r.label) {
                                     case 0:
-                                        return [4, Uc(e)];
+                                        return [4, Ic(e)];
                                     case 1:
-                                        return t = r.sent(), n = zc(t), [2, new Uint8Array(n)]
+                                        return t = r.sent(), n = Nc(t), [2, new Uint8Array(n)]
                                 }
                             }))
                         }))
                     }(e) : function(e) {
-                        return jc(this, void 0, void 0, (function() {
+                        return cc(this, void 0, void 0, (function() {
                             var t, n, r, o, i, a, s;
-                            return xc(this, (function(u) {
+                            return dc(this, (function(u) {
                                 switch (u.label) {
                                     case 0:
                                         t = new Uint8Array(0), n = e.getReader(), r = !1, u.label = 1;
                                     case 1:
                                         return r ? [3, 3] : [4, n.read()];
                                     case 2:
                                         return o = u.sent(), i = o.done, (a = o.value) && (s = t, (t = new Uint8Array(s.length + a.length)).set(s), t.set(a, s.length)), r = i, [3, 1];
                                     case 3:
                                         return [2, t]
                                 }
                             }))
                         }))
                     }(e)
                 },
-                utf8Decoder: id.fromUtf8,
-                utf8Encoder: id.toUtf8
+                utf8Decoder: Zc.fromUtf8,
+                utf8Encoder: Zc.toUtf8
             });
-        var md = function() {
-            return md = Object.assign || function(e) {
+        var id = function() {
+            return id = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, md.apply(this, arguments)
+            }, id.apply(this, arguments)
         };
 
-        function vd(e, t, n, r) {
+        function ad(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -62775,15 +60223,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Md(e, t) {
+        function sd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -62850,15 +60298,15 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var bd = function(e) {
+        var ud = function(e) {
                 var t = e.endpoint,
                     n = e.urlParser;
                 if ("string" === typeof t) {
                     var r = Promise.resolve(n(t));
                     return function() {
                         return r
                     }
@@ -62867,49 +60315,49 @@
                     var o = Promise.resolve(t);
                     return function() {
                         return o
                     }
                 }
                 return t
             },
-            wd = function(e) {
-                return vd(void 0, void 0, void 0, (function() {
+            ld = function(e) {
+                return ad(void 0, void 0, void 0, (function() {
                     var t, n, r, o, i;
-                    return Md(this, (function(a) {
+                    return sd(this, (function(a) {
                         switch (a.label) {
                             case 0:
                                 return t = e.tls, n = void 0 === t || t, [4, e.region()];
                             case 1:
                                 if (r = a.sent(), !new RegExp(/^([a-zA-Z0-9]|[a-zA-Z0-9][a-zA-Z0-9-]{0,61}[a-zA-Z0-9])$/).test(r)) throw new Error("Invalid region in client config");
                                 return [4, e.regionInfoProvider(r)];
                             case 2:
                                 if (!(o = (null !== (i = a.sent()) && void 0 !== i ? i : {}).hostname)) throw new Error("Cannot resolve hostname from client config");
                                 return [2, e.urlParser((n ? "https:" : "http:") + "//" + o)]
                         }
                     }))
                 }))
             },
-            jd = function(e) {
+            cd = function(e) {
                 if ("string" === typeof e) {
                     var t = Promise.resolve(e);
                     return function() {
                         return t
                     }
                 }
                 return e
             };
-        var xd = function() {
-            return xd = Object.assign || function(e) {
+        var dd = function() {
+            return dd = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, xd.apply(this, arguments)
+            }, dd.apply(this, arguments)
         };
 
-        function Nd(e, t, n, r) {
+        function fd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -62929,15 +60377,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Id(e, t) {
+        function pd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63004,46 +60452,46 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var Dd = "content-length";
-        var Sd = {
+        var hd = "content-length";
+        var gd = {
                 step: "build",
                 tags: ["SET_CONTENT_LENGTH", "CONTENT_LENGTH"],
                 name: "contentLengthMiddleware",
                 override: !0
             },
-            Ld = function(e) {
+            yd = function(e) {
                 return {
                     applyToStack: function(t) {
                         t.add(function(e) {
                             var t = this;
                             return function(n) {
                                 return function(r) {
-                                    return Nd(t, void 0, void 0, (function() {
+                                    return fd(t, void 0, void 0, (function() {
                                         var t, o, i, a, s;
-                                        return Id(this, (function(u) {
-                                            return t = r.request, fl.isInstance(t) && (o = t.body, i = t.headers, o && -1 === Object.keys(i).map((function(e) {
+                                        return pd(this, (function(u) {
+                                            return t = r.request, el.isInstance(t) && (o = t.body, i = t.headers, o && -1 === Object.keys(i).map((function(e) {
                                                 return e.toLowerCase()
-                                            })).indexOf(Dd) && void 0 !== (a = e(o)) && (t.headers = xd(xd({}, t.headers), ((s = {})["content-length"] = String(a), s)))), [2, n(xd(xd({}, r), {
+                                            })).indexOf(hd) && void 0 !== (a = e(o)) && (t.headers = dd(dd({}, t.headers), ((s = {})["content-length"] = String(a), s)))), [2, n(dd(dd({}, r), {
                                                 request: t
                                             }))]
                                         }))
                                     }))
                                 }
                             }
-                        }(e.bodyLengthChecker), Sd)
+                        }(e.bodyLengthChecker), gd)
                     }
                 }
             };
 
-        function kd(e, t, n, r) {
+        function md(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63063,15 +60511,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Cd(e, t) {
+        function vd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63138,41 +60586,41 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var Ed = {
+        var Md = {
                 name: "hostHeaderMiddleware",
                 step: "build",
                 priority: "low",
                 tags: ["HOST"],
                 override: !0
             },
-            _d = function(e) {
+            bd = function(e) {
                 return {
                     applyToStack: function(t) {
                         t.add(function(e) {
                             return function(t) {
                                 return function(n) {
-                                    return kd(void 0, void 0, void 0, (function() {
+                                    return md(void 0, void 0, void 0, (function() {
                                         var r, o;
-                                        return Cd(this, (function(i) {
-                                            return fl.isInstance(n.request) ? (r = n.request, (void 0 === (o = (e.requestHandler.metadata || {}).handlerProtocol) ? "" : o).indexOf("h2") >= 0 && !r.headers[":authority"] ? (delete r.headers.host, r.headers[":authority"] = "") : r.headers.host || (r.headers.host = r.hostname), [2, t(n)]) : [2, t(n)]
+                                        return vd(this, (function(i) {
+                                            return el.isInstance(n.request) ? (r = n.request, (void 0 === (o = (e.requestHandler.metadata || {}).handlerProtocol) ? "" : o).indexOf("h2") >= 0 && !r.headers[":authority"] ? (delete r.headers.host, r.headers[":authority"] = "") : r.headers.host || (r.headers.host = r.hostname), [2, t(n)]) : [2, t(n)]
                                         }))
                                     }))
                                 }
                             }
-                        }(e), Ed)
+                        }(e), Md)
                     }
                 }
             };
 
-        function Td(e, t, n, r) {
+        function wd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63192,15 +60640,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Ad(e, t) {
+        function jd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63267,20 +60715,20 @@
                             value: i[0] ? i[1] : void 0,
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
-        var Od = function() {
+        var xd = function() {
                 return function(e, t) {
                     return function(n) {
-                        return Td(void 0, void 0, void 0, (function() {
+                        return wd(void 0, void 0, void 0, (function() {
                             var r, o, i, a, s, u, l, c, d;
-                            return Ad(this, (function(f) {
+                            return jd(this, (function(f) {
                                 switch (f.label) {
                                     case 0:
                                         return r = t.clientName, o = t.commandName, i = t.inputFilterSensitiveLog, a = t.logger, s = t.outputFilterSensitiveLog, [4, e(n)];
                                     case 1:
                                         return u = f.sent(), a ? ("function" === typeof a.info && (l = u.output, c = l.$metadata, d = function(e, t) {
                                             var n = {};
                                             for (var r in e) Object.prototype.hasOwnProperty.call(e, r) && t.indexOf(r) < 0 && (n[r] = e[r]);
@@ -63298,29 +60746,29 @@
                                         })), [2, u]) : [2, u]
                                 }
                             }))
                         }))
                     }
                 }
             },
-            zd = {
+            Nd = {
                 name: "loggerMiddleware",
                 tags: ["LOGGER"],
                 step: "initialize",
                 override: !0
             };
-        var Ud = function() {
-            return Ud = Object.assign || function(e) {
+        var Id = function() {
+            return Id = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Ud.apply(this, arguments)
+            }, Id.apply(this, arguments)
         };
 
-        function Pd(e, t, n, r) {
+        function Dd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63340,15 +60788,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Rd(e, t) {
+        function Sd(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63416,15 +60864,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function Bd(e, t) {
+        function Ld(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -63437,23 +60885,23 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        var Fd = function() {
-            return Fd = Object.assign || function(e) {
+        var kd = function() {
+            return kd = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, Fd.apply(this, arguments)
+            }, kd.apply(this, arguments)
         };
 
-        function Yd(e, t, n, r) {
+        function Cd(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -63473,15 +60921,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Qd(e, t) {
+        function Ed(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -63549,15 +60997,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function Gd(e) {
+        function _d(e) {
             var t = "function" === typeof Symbol && Symbol.iterator,
                 n = t && e[t],
                 r = 0;
             if (n) return n.call(e);
             if (e && "number" === typeof e.length) return {
                 next: function() {
                     return e && r >= e.length && (e = void 0), {
@@ -63565,15 +61013,15 @@
                         done: !e
                     }
                 }
             };
             throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
         }
 
-        function Wd(e, t) {
+        function Td(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -63586,33 +61034,33 @@
                     r && !r.done && (n = i.return) && n.call(i)
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
-        for (var Hd = {}, Zd = {}, Vd = 0; Vd < 256; Vd++) {
-            var qd = Vd.toString(16).toLowerCase();
-            1 === qd.length && (qd = "0" + qd), Hd[Vd] = qd, Zd[qd] = Vd
+        for (var Ad = {}, Od = {}, zd = 0; zd < 256; zd++) {
+            var Ud = zd.toString(16).toLowerCase();
+            1 === Ud.length && (Ud = "0" + Ud), Ad[zd] = Ud, Od[Ud] = zd
         }
 
-        function Jd(e) {
-            for (var t = "", n = 0; n < e.byteLength; n++) t += Hd[e[n]];
+        function Pd(e) {
+            for (var t = "", n = 0; n < e.byteLength; n++) t += Ad[e[n]];
             return t
         }
-        var Kd = "X-Amz-Date",
-            Xd = "X-Amz-Signature",
-            $d = "X-Amz-Security-Token",
-            ef = "authorization",
-            tf = Kd.toLowerCase(),
-            nf = [ef, tf, "date"],
-            rf = Xd.toLowerCase(),
-            of = "x-amz-content-sha256",
-            af = $d.toLowerCase(),
-            sf = {
+        var Rd = "X-Amz-Date",
+            Bd = "X-Amz-Signature",
+            Fd = "X-Amz-Security-Token",
+            Yd = "authorization",
+            Qd = Rd.toLowerCase(),
+            Gd = [Yd, Qd, "date"],
+            Wd = Bd.toLowerCase(),
+            Hd = "x-amz-content-sha256",
+            Zd = Fd.toLowerCase(),
+            Vd = {
                 authorization: !0,
                 "cache-control": !0,
                 connection: !0,
                 expect: !0,
                 from: !0,
                 "keep-alive": !0,
                 "max-forwards": !0,
@@ -63621,39 +61069,39 @@
                 te: !0,
                 trailer: !0,
                 "transfer-encoding": !0,
                 upgrade: !0,
                 "user-agent": !0,
                 "x-amzn-trace-id": !0
             },
-            uf = /^proxy-/,
-            lf = /^sec-/,
-            cf = "AWS4-HMAC-SHA256",
-            df = "AWS4-HMAC-SHA256-PAYLOAD",
-            ff = "aws4_request",
-            pf = {},
-            hf = [];
+            qd = /^proxy-/,
+            Jd = /^sec-/,
+            Kd = "AWS4-HMAC-SHA256",
+            Xd = "AWS4-HMAC-SHA256-PAYLOAD",
+            $d = "aws4_request",
+            ef = {},
+            tf = [];
 
-        function gf(e, t, n) {
-            return e + "/" + t + "/" + n + "/" + ff
+        function nf(e, t, n) {
+            return e + "/" + t + "/" + n + "/" + $d
         }
 
-        function yf(e, t, n) {
+        function rf(e, t, n) {
             var r = new e(t);
             return r.update(n), r.digest()
         }
 
-        function mf(e, t, n) {
+        function of(e, t, n) {
             var r, o, i = e.headers,
                 a = {};
             try {
-                for (var s = Gd(Object.keys(i).sort()), u = s.next(); !u.done; u = s.next()) {
+                for (var s = _d(Object.keys(i).sort()), u = s.next(); !u.done; u = s.next()) {
                     var l = u.value,
                         c = l.toLowerCase();
-                    (c in sf || (null === t || void 0 === t ? void 0 : t.has(c)) || uf.test(c) || lf.test(c)) && (!n || n && !n.has(c)) || (a[c] = i[l].trim().replace(/\s+/g, " "))
+                    (c in Vd || (null === t || void 0 === t ? void 0 : t.has(c)) || qd.test(c) || Jd.test(c)) && (!n || n && !n.has(c)) || (a[c] = i[l].trim().replace(/\s+/g, " "))
                 }
             } catch (d) {
                 r = {
                     error: d
                 }
             } finally {
                 try {
@@ -63661,84 +61109,84 @@
                 } finally {
                     if (r) throw r.error
                 }
             }
             return a
         }
 
-        function vf(e, t) {
+        function af(e, t) {
             var n = e.headers,
                 r = e.body;
-            return Yd(this, void 0, void 0, (function() {
+            return Cd(this, void 0, void 0, (function() {
                 var e, o, i, a, s, u, l;
-                return Qd(this, (function(c) {
+                return Ed(this, (function(c) {
                     switch (c.label) {
                         case 0:
                             try {
-                                for (e = Gd(Object.keys(n)), o = e.next(); !o.done; o = e.next())
-                                    if ((i = o.value).toLowerCase() === of) return [2, n[i]]
+                                for (e = _d(Object.keys(n)), o = e.next(); !o.done; o = e.next())
+                                    if ((i = o.value).toLowerCase() === Hd) return [2, n[i]]
                             } catch (f) {
                                 u = {
                                     error: f
                                 }
                             } finally {
                                 try {
                                     o && !o.done && (l = e.return) && l.call(e)
                                 } finally {
                                     if (u) throw u.error
                                 }
                             }
                             return void 0 != r ? [3, 1] : [2, "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855"];
                         case 1:
-                            return "string" === typeof r || ArrayBuffer.isView(r) || (d = r, "function" === typeof ArrayBuffer && d instanceof ArrayBuffer || "[object ArrayBuffer]" === Object.prototype.toString.call(d)) ? ((a = new t).update(r), s = Jd, [4, a.digest()]) : [3, 3];
+                            return "string" === typeof r || ArrayBuffer.isView(r) || (d = r, "function" === typeof ArrayBuffer && d instanceof ArrayBuffer || "[object ArrayBuffer]" === Object.prototype.toString.call(d)) ? ((a = new t).update(r), s = Pd, [4, a.digest()]) : [3, 3];
                         case 2:
                             return [2, s.apply(void 0, [c.sent()])];
                         case 3:
                             return [2, "UNSIGNED-PAYLOAD"]
                     }
                     var d
                 }))
             }))
         }
 
-        function Mf(e) {
+        function sf(e) {
             var t = e.headers,
                 n = e.query,
                 r = function(e, t) {
                     var n = {};
                     for (var r in e) Object.prototype.hasOwnProperty.call(e, r) && t.indexOf(r) < 0 && (n[r] = e[r]);
                     if (null != e && "function" === typeof Object.getOwnPropertySymbols) {
                         var o = 0;
                         for (r = Object.getOwnPropertySymbols(e); o < r.length; o++) t.indexOf(r[o]) < 0 && Object.prototype.propertyIsEnumerable.call(e, r[o]) && (n[r[o]] = e[r[o]])
                     }
                     return n
                 }(e, ["headers", "query"]);
-            return Fd(Fd({}, r), {
-                headers: Fd({}, t),
-                query: n ? bf(n) : void 0
+            return kd(kd({}, r), {
+                headers: kd({}, t),
+                query: n ? uf(n) : void 0
             })
         }
 
-        function bf(e) {
+        function uf(e) {
             return Object.keys(e).reduce((function(t, n) {
                 var r, o = e[n];
-                return Fd(Fd({}, t), ((r = {})[n] = Array.isArray(o) ? function() {
-                    for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Wd(arguments[t]));
+                return kd(kd({}, t), ((r = {})[n] = Array.isArray(o) ? function() {
+                    for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(Td(arguments[t]));
                     return e
                 }(o) : o, r))
             }), {})
         }
 
-        function wf(e) {
+        function lf(e) {
             var t, n;
-            e = "function" === typeof e.clone ? e.clone() : Mf(e);
+            e = "function" === typeof e.clone ? e.clone() : sf(e);
             try {
-                for (var r = Gd(Object.keys(e.headers)), o = r.next(); !o.done; o = r.next()) {
+                for (var r = _d(Object.keys(e.headers)), o = r.next(); !o.done; o = r.next()) {
                     var i = o.value;
-                    nf.indexOf(i.toLowerCase()) > -1 && delete e.headers[i]
+                    Gd.indexOf(i.toLowerCase()) > -1 && delete e.headers[i]
                 }
             } catch (a) {
                 t = {
                     error: a
                 }
             } finally {
                 try {
@@ -63746,55 +61194,55 @@
                 } finally {
                     if (t) throw t.error
                 }
             }
             return e
         }
 
-        function jf(e) {
+        function cf(e) {
             return function(e) {
                 if ("number" === typeof e) return new Date(1e3 * e);
                 if ("string" === typeof e) return Number(e) ? new Date(1e3 * Number(e)) : new Date(e);
                 return e
             }(e).toISOString().replace(/\.\d{3}Z$/, "Z")
         }
-        var xf = function() {
+        var df = function() {
                 function e(e) {
                     var t = e.applyChecksum,
                         n = e.credentials,
                         r = e.region,
                         o = e.service,
                         i = e.sha256,
                         a = e.uriEscapePath,
                         s = void 0 === a || a;
-                    this.service = o, this.sha256 = i, this.uriEscapePath = s, this.applyChecksum = "boolean" !== typeof t || t, this.regionProvider = Df(r), this.credentialProvider = Sf(n)
+                    this.service = o, this.sha256 = i, this.uriEscapePath = s, this.applyChecksum = "boolean" !== typeof t || t, this.regionProvider = hf(r), this.credentialProvider = gf(n)
                 }
                 return e.prototype.presign = function(e, t) {
-                    return void 0 === t && (t = {}), Yd(this, void 0, void 0, (function() {
+                    return void 0 === t && (t = {}), Cd(this, void 0, void 0, (function() {
                         var n, r, o, i, a, s, u, l, c, d, f, p, h, g, y, m, v, M, b, w, j, x, N, I;
-                        return Qd(this, (function(D) {
+                        return Ed(this, (function(D) {
                             switch (D.label) {
                                 case 0:
                                     return n = t.signingDate, r = void 0 === n ? new Date : n, o = t.expiresIn, i = void 0 === o ? 3600 : o, a = t.unsignableHeaders, s = t.unhoistableHeaders, u = t.signableHeaders, l = t.signingRegion, c = t.signingService, [4, this.credentialProvider()];
                                 case 1:
                                     return d = D.sent(), null === l || void 0 === l ? [3, 2] : (p = l, [3, 4]);
                                 case 2:
                                     return [4, this.regionProvider()];
                                 case 3:
                                     p = D.sent(), D.label = 4;
                                 case 4:
-                                    return f = p, h = Nf(r), g = h.longDate, y = h.shortDate, i > 604800 ? [2, Promise.reject("Signature version 4 presigned URLs must have an expiration date less than one week in the future")] : (m = gf(y, f, null !== c && void 0 !== c ? c : this.service), v = function(e, t) {
+                                    return f = p, h = ff(r), g = h.longDate, y = h.shortDate, i > 604800 ? [2, Promise.reject("Signature version 4 presigned URLs must have an expiration date less than one week in the future")] : (m = nf(y, f, null !== c && void 0 !== c ? c : this.service), v = function(e, t) {
                                         var n, r, o;
                                         void 0 === t && (t = {});
-                                        var i = "function" === typeof e.clone ? e.clone() : Mf(e),
+                                        var i = "function" === typeof e.clone ? e.clone() : sf(e),
                                             a = i.headers,
                                             s = i.query,
                                             u = void 0 === s ? {} : s;
                                         try {
-                                            for (var l = Gd(Object.keys(a)), c = l.next(); !c.done; c = l.next()) {
+                                            for (var l = _d(Object.keys(a)), c = l.next(); !c.done; c = l.next()) {
                                                 var d = c.value,
                                                     f = d.toLowerCase();
                                                 "x-amz-" !== f.substr(0, 6) || (null === (o = t.unhoistableHeaders) || void 0 === o ? void 0 : o.has(f)) || (u[d] = a[d], delete a[d])
                                             }
                                         } catch (p) {
                                             n = {
                                                 error: p
@@ -63802,159 +61250,159 @@
                                         } finally {
                                             try {
                                                 c && !c.done && (r = l.return) && r.call(l)
                                             } finally {
                                                 if (n) throw n.error
                                             }
                                         }
-                                        return Fd(Fd({}, e), {
+                                        return kd(kd({}, e), {
                                             headers: a,
                                             query: u
                                         })
-                                    }(wf(e), {
+                                    }(lf(e), {
                                         unhoistableHeaders: s
-                                    }), d.sessionToken && (v.query[$d] = d.sessionToken), v.query["X-Amz-Algorithm"] = cf, v.query["X-Amz-Credential"] = d.accessKeyId + "/" + m, v.query["X-Amz-Date"] = g, v.query["X-Amz-Expires"] = i.toString(10), M = mf(v, a, u), v.query["X-Amz-SignedHeaders"] = If(M), b = v.query, w = Xd, j = this.getSignature, x = [g, m, this.getSigningKey(d, f, y, c)], N = this.createCanonicalRequest, I = [v, M], [4, vf(e, this.sha256)]);
+                                    }), d.sessionToken && (v.query[Fd] = d.sessionToken), v.query["X-Amz-Algorithm"] = Kd, v.query["X-Amz-Credential"] = d.accessKeyId + "/" + m, v.query["X-Amz-Date"] = g, v.query["X-Amz-Expires"] = i.toString(10), M = of(v, a, u), v.query["X-Amz-SignedHeaders"] = pf(M), b = v.query, w = Bd, j = this.getSignature, x = [g, m, this.getSigningKey(d, f, y, c)], N = this.createCanonicalRequest, I = [v, M], [4, af(e, this.sha256)]);
                                 case 5:
                                     return [4, j.apply(this, x.concat([N.apply(this, I.concat([D.sent()]))]))];
                                 case 6:
                                     return b[w] = D.sent(), [2, v]
                             }
                         }))
                     }))
                 }, e.prototype.sign = function(e, t) {
-                    return Yd(this, void 0, void 0, (function() {
-                        return Qd(this, (function(n) {
+                    return Cd(this, void 0, void 0, (function() {
+                        return Ed(this, (function(n) {
                             return "string" === typeof e ? [2, this.signString(e, t)] : e.headers && e.payload ? [2, this.signEvent(e, t)] : [2, this.signRequest(e, t)]
                         }))
                     }))
                 }, e.prototype.signEvent = function(e, t) {
                     var n = e.headers,
                         r = e.payload,
                         o = t.signingDate,
                         i = void 0 === o ? new Date : o,
                         a = t.priorSignature,
                         s = t.signingRegion,
                         u = t.signingService;
-                    return Yd(this, void 0, void 0, (function() {
+                    return Cd(this, void 0, void 0, (function() {
                         var e, t, o, l, c, d, f, p, h, g, y;
-                        return Qd(this, (function(m) {
+                        return Ed(this, (function(m) {
                             switch (m.label) {
                                 case 0:
                                     return null === s || void 0 === s ? [3, 1] : (t = s, [3, 3]);
                                 case 1:
                                     return [4, this.regionProvider()];
                                 case 2:
                                     t = m.sent(), m.label = 3;
                                 case 3:
-                                    return e = t, o = Nf(i), l = o.shortDate, c = o.longDate, d = gf(l, e, null !== u && void 0 !== u ? u : this.service), [4, vf({
+                                    return e = t, o = ff(i), l = o.shortDate, c = o.longDate, d = nf(l, e, null !== u && void 0 !== u ? u : this.service), [4, af({
                                         headers: {},
                                         body: r
                                     }, this.sha256)];
                                 case 4:
-                                    return f = m.sent(), (p = new this.sha256).update(n), g = Jd, [4, p.digest()];
+                                    return f = m.sent(), (p = new this.sha256).update(n), g = Pd, [4, p.digest()];
                                 case 5:
-                                    return h = g.apply(void 0, [m.sent()]), y = [df, c, d, a, h, f].join("\n"), [2, this.signString(y, {
+                                    return h = g.apply(void 0, [m.sent()]), y = [Xd, c, d, a, h, f].join("\n"), [2, this.signString(y, {
                                         signingDate: i,
                                         signingRegion: e,
                                         signingService: u
                                     })]
                             }
                         }))
                     }))
                 }, e.prototype.signString = function(e, t) {
                     var n = void 0 === t ? {} : t,
                         r = n.signingDate,
                         o = void 0 === r ? new Date : r,
                         i = n.signingRegion,
                         a = n.signingService;
-                    return Yd(this, void 0, void 0, (function() {
+                    return Cd(this, void 0, void 0, (function() {
                         var t, n, r, s, u, l, c, d;
-                        return Qd(this, (function(f) {
+                        return Ed(this, (function(f) {
                             switch (f.label) {
                                 case 0:
                                     return [4, this.credentialProvider()];
                                 case 1:
                                     return t = f.sent(), null === i || void 0 === i ? [3, 2] : (r = i, [3, 4]);
                                 case 2:
                                     return [4, this.regionProvider()];
                                 case 3:
                                     r = f.sent(), f.label = 4;
                                 case 4:
-                                    return n = r, s = Nf(o).shortDate, c = (l = this.sha256).bind, [4, this.getSigningKey(t, n, s, a)];
+                                    return n = r, s = ff(o).shortDate, c = (l = this.sha256).bind, [4, this.getSigningKey(t, n, s, a)];
                                 case 5:
-                                    return (u = new(c.apply(l, [void 0, f.sent()]))).update(e), d = Jd, [4, u.digest()];
+                                    return (u = new(c.apply(l, [void 0, f.sent()]))).update(e), d = Pd, [4, u.digest()];
                                 case 6:
                                     return [2, d.apply(void 0, [f.sent()])]
                             }
                         }))
                     }))
                 }, e.prototype.signRequest = function(e, t) {
                     var n = void 0 === t ? {} : t,
                         r = n.signingDate,
                         o = void 0 === r ? new Date : r,
                         i = n.signableHeaders,
                         a = n.unsignableHeaders,
                         s = n.signingRegion,
                         u = n.signingService;
-                    return Yd(this, void 0, void 0, (function() {
+                    return Cd(this, void 0, void 0, (function() {
                         var t, n, r, l, c, d, f, p, h, g, y;
-                        return Qd(this, (function(m) {
+                        return Ed(this, (function(m) {
                             switch (m.label) {
                                 case 0:
                                     return [4, this.credentialProvider()];
                                 case 1:
                                     return t = m.sent(), null === s || void 0 === s ? [3, 2] : (r = s, [3, 4]);
                                 case 2:
                                     return [4, this.regionProvider()];
                                 case 3:
                                     r = m.sent(), m.label = 4;
                                 case 4:
-                                    return n = r, l = wf(e), c = Nf(o), d = c.longDate, f = c.shortDate, p = gf(f, n, null !== u && void 0 !== u ? u : this.service), l.headers[tf] = d, t.sessionToken && (l.headers[af] = t.sessionToken), [4, vf(l, this.sha256)];
+                                    return n = r, l = lf(e), c = ff(o), d = c.longDate, f = c.shortDate, p = nf(f, n, null !== u && void 0 !== u ? u : this.service), l.headers[Qd] = d, t.sessionToken && (l.headers[Zd] = t.sessionToken), [4, af(l, this.sha256)];
                                 case 5:
                                     return h = m.sent(), ! function(e, t) {
                                         var n, r;
                                         e = e.toLowerCase();
                                         try {
-                                            for (var o = Gd(Object.keys(t)), i = o.next(); !i.done; i = o.next())
+                                            for (var o = _d(Object.keys(t)), i = o.next(); !i.done; i = o.next())
                                                 if (e === i.value.toLowerCase()) return !0
                                         } catch (a) {
                                             n = {
                                                 error: a
                                             }
                                         } finally {
                                             try {
                                                 i && !i.done && (r = o.return) && r.call(o)
                                             } finally {
                                                 if (n) throw n.error
                                             }
                                         }
                                         return !1
-                                    }(of, l.headers) && this.applyChecksum && (l.headers[of] = h), g = mf(l, a, i), [4, this.getSignature(d, p, this.getSigningKey(t, n, f, u), this.createCanonicalRequest(l, g, h))];
+                                    }(Hd, l.headers) && this.applyChecksum && (l.headers[Hd] = h), g = of(l, a, i), [4, this.getSignature(d, p, this.getSigningKey(t, n, f, u), this.createCanonicalRequest(l, g, h))];
                                 case 6:
-                                    return y = m.sent(), l.headers[ef] = "AWS4-HMAC-SHA256 Credential=" + t.accessKeyId + "/" + p + ", SignedHeaders=" + If(g) + ", Signature=" + y, [2, l]
+                                    return y = m.sent(), l.headers[Yd] = "AWS4-HMAC-SHA256 Credential=" + t.accessKeyId + "/" + p + ", SignedHeaders=" + pf(g) + ", Signature=" + y, [2, l]
                             }
                         }))
                     }))
                 }, e.prototype.createCanonicalRequest = function(e, t, n) {
                     var r = Object.keys(t).sort();
                     return e.method + "\n" + this.getCanonicalPath(e) + "\n" + function(e) {
                         var t, n, r = e.query,
                             o = void 0 === r ? {} : r,
                             i = [],
                             a = {},
                             s = function(e) {
-                                if (e.toLowerCase() === rf) return "continue";
+                                if (e.toLowerCase() === Wd) return "continue";
                                 i.push(e);
                                 var t = o[e];
-                                "string" === typeof t ? a[e] = Dc(e) + "=" + Dc(t) : Array.isArray(t) && (a[e] = t.slice(0).sort().reduce((function(t, n) {
-                                    return t.concat([Dc(e) + "=" + Dc(n)])
+                                "string" === typeof t ? a[e] = hc(e) + "=" + hc(t) : Array.isArray(t) && (a[e] = t.slice(0).sort().reduce((function(t, n) {
+                                    return t.concat([hc(e) + "=" + hc(n)])
                                 }), []).join("&"))
                             };
                         try {
-                            for (var u = Gd(Object.keys(o).sort()), l = u.next(); !l.done; l = u.next()) s(l.value)
+                            for (var u = _d(Object.keys(o).sort()), l = u.next(); !l.done; l = u.next()) s(l.value)
                         } catch (c) {
                             t = {
                                 error: c
                             }
                         } finally {
                             try {
                                 l && !l.done && (n = u.return) && n.call(u)
@@ -63967,60 +61415,60 @@
                         })).filter((function(e) {
                             return e
                         })).join("&")
                     }(e) + "\n" + r.map((function(e) {
                         return e + ":" + t[e]
                     })).join("\n") + "\n\n" + r.join(";") + "\n" + n
                 }, e.prototype.createStringToSign = function(e, t, n) {
-                    return Yd(this, void 0, void 0, (function() {
+                    return Cd(this, void 0, void 0, (function() {
                         var r, o;
-                        return Qd(this, (function(i) {
+                        return Ed(this, (function(i) {
                             switch (i.label) {
                                 case 0:
                                     return (r = new this.sha256).update(n), [4, r.digest()];
                                 case 1:
-                                    return o = i.sent(), [2, "AWS4-HMAC-SHA256\n" + e + "\n" + t + "\n" + Jd(o)]
+                                    return o = i.sent(), [2, "AWS4-HMAC-SHA256\n" + e + "\n" + t + "\n" + Pd(o)]
                             }
                         }))
                     }))
                 }, e.prototype.getCanonicalPath = function(e) {
                     var t = e.path;
                     return this.uriEscapePath ? "/" + encodeURIComponent(t.replace(/^\//, "")).replace(/%2F/g, "/") : t
                 }, e.prototype.getSignature = function(e, t, n, r) {
-                    return Yd(this, void 0, void 0, (function() {
+                    return Cd(this, void 0, void 0, (function() {
                         var o, i, a, s, u;
-                        return Qd(this, (function(l) {
+                        return Ed(this, (function(l) {
                             switch (l.label) {
                                 case 0:
                                     return [4, this.createStringToSign(e, t, r)];
                                 case 1:
                                     return o = l.sent(), s = (a = this.sha256).bind, [4, n];
                                 case 2:
-                                    return (i = new(s.apply(a, [void 0, l.sent()]))).update(o), u = Jd, [4, i.digest()];
+                                    return (i = new(s.apply(a, [void 0, l.sent()]))).update(o), u = Pd, [4, i.digest()];
                                 case 3:
                                     return [2, u.apply(void 0, [l.sent()])]
                             }
                         }))
                     }))
                 }, e.prototype.getSigningKey = function(e, t, n, r) {
                     return function(e, t, n, r, o) {
-                        return Yd(void 0, void 0, void 0, (function() {
+                        return Cd(void 0, void 0, void 0, (function() {
                             var i, a, s, u, l, c, d, f, p;
-                            return Qd(this, (function(h) {
+                            return Ed(this, (function(h) {
                                 switch (h.label) {
                                     case 0:
-                                        return [4, yf(e, t.secretAccessKey, t.accessKeyId)];
+                                        return [4, rf(e, t.secretAccessKey, t.accessKeyId)];
                                     case 1:
-                                        if (i = h.sent(), (a = n + ":" + r + ":" + o + ":" + Jd(i) + ":" + t.sessionToken) in pf) return [2, pf[a]];
-                                        for (hf.push(a); hf.length > 50;) delete pf[hf.shift()];
+                                        if (i = h.sent(), (a = n + ":" + r + ":" + o + ":" + Pd(i) + ":" + t.sessionToken) in ef) return [2, ef[a]];
+                                        for (tf.push(a); tf.length > 50;) delete ef[tf.shift()];
                                         s = "AWS4" + t.secretAccessKey, h.label = 2;
                                     case 2:
-                                        h.trys.push([2, 7, 8, 9]), u = Gd([n, r, o, ff]), l = u.next(), h.label = 3;
+                                        h.trys.push([2, 7, 8, 9]), u = _d([n, r, o, $d]), l = u.next(), h.label = 3;
                                     case 3:
-                                        return l.done ? [3, 6] : (c = l.value, [4, yf(e, s, c)]);
+                                        return l.done ? [3, 6] : (c = l.value, [4, rf(e, s, c)]);
                                     case 4:
                                         s = h.sent(), h.label = 5;
                                     case 5:
                                         return l = u.next(), [3, 3];
                                     case 6:
                                         return [3, 9];
                                     case 7:
@@ -64031,68 +61479,68 @@
                                         try {
                                             l && !l.done && (p = u.return) && p.call(u)
                                         } finally {
                                             if (f) throw f.error
                                         }
                                         return [7];
                                     case 9:
-                                        return [2, pf[a] = s]
+                                        return [2, ef[a] = s]
                                 }
                             }))
                         }))
                     }(this.sha256, e, n, t, r || this.service)
                 }, e
             }(),
-            Nf = function(e) {
-                var t = jf(e).replace(/[\-:]/g, "");
+            ff = function(e) {
+                var t = cf(e).replace(/[\-:]/g, "");
                 return {
                     longDate: t,
                     shortDate: t.substr(0, 8)
                 }
             },
-            If = function(e) {
+            pf = function(e) {
                 return Object.keys(e).sort().join(";")
             },
-            Df = function(e) {
+            hf = function(e) {
                 if ("string" === typeof e) {
                     var t = Promise.resolve(e);
                     return function() {
                         return t
                     }
                 }
                 return e
             },
-            Sf = function(e) {
+            gf = function(e) {
                 if ("object" === typeof e) {
                     var t = Promise.resolve(e);
                     return function() {
                         return t
                     }
                 }
                 return e
             };
 
-        function Lf(e) {
+        function yf(e) {
             if ("object" === typeof e) {
                 var t = Promise.resolve(e);
                 return function() {
                     return t
                 }
             }
             return e
         }
-        var kf = function() {
-            return kf = Object.assign || function(e) {
+        var mf = function() {
+            return mf = Object.assign || function(e) {
                 for (var t, n = 1, r = arguments.length; n < r; n++)
                     for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                 return e
-            }, kf.apply(this, arguments)
+            }, mf.apply(this, arguments)
         };
 
-        function Cf(e, t, n, r) {
+        function vf(e, t, n, r) {
             return new(n || (n = Promise))((function(o, i) {
                 function a(e) {
                     try {
                         u(r.next(e))
                     } catch (t) {
                         i(t)
                     }
@@ -64112,15 +61560,15 @@
                         e(t)
                     }))).then(a, s)
                 }
                 u((r = r.apply(e, t || [])).next())
             }))
         }
 
-        function Ef(e, t) {
+        function Mf(e, t) {
             var n, r, o, i, a = {
                 label: 0,
                 sent: function() {
                     if (1 & o[0]) throw o[1];
                     return o[1]
                 },
                 trys: [],
@@ -64188,15 +61636,15 @@
                             done: !0
                         }
                     }([i, s])
                 }
             }
         }
 
-        function _f(e, t) {
+        function bf(e, t) {
             var n = "function" === typeof Symbol && e[Symbol.iterator];
             if (!n) return e;
             var r, o, i = n.call(e),
                 a = [];
             try {
                 for (;
                     (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -64210,213 +61658,213 @@
                 } finally {
                     if (o) throw o.error
                 }
             }
             return a
         }
 
-        function Tf() {
-            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(_f(arguments[t]));
+        function wf() {
+            for (var e = [], t = 0; t < arguments.length; t++) e = e.concat(bf(arguments[t]));
             return e
         }
-        var Af = "user-agent",
-            Of = /[^\!\#\$\%\&\'\*\+\-\.\^\_\`\|\~\d\w]/g,
-            zf = function(e) {
-                var t = _f(e, 2),
+        var jf = "user-agent",
+            xf = /[^\!\#\$\%\&\'\*\+\-\.\^\_\`\|\~\d\w]/g,
+            Nf = function(e) {
+                var t = bf(e, 2),
                     n = t[0],
                     r = t[1],
                     o = n.indexOf("/"),
                     i = n.substring(0, o),
                     a = n.substring(o + 1);
                 return "api" === i && (a = a.toLowerCase()), [i, a, r].filter((function(e) {
                     return e && e.length > 0
                 })).map((function(e) {
-                    return null === e || void 0 === e ? void 0 : e.replace(Of, "_")
+                    return null === e || void 0 === e ? void 0 : e.replace(xf, "_")
                 })).join("/")
             },
-            Uf = {
+            If = {
                 name: "getUserAgentMiddleware",
                 step: "build",
                 priority: "low",
                 tags: ["SET_USER_AGENT", "USER_AGENT"],
                 override: !0
             },
-            Pf = function(e) {
+            Df = function(e) {
                 return {
                     applyToStack: function(t) {
                         var n;
                         t.add((n = e, function(e, t) {
                             return function(r) {
-                                return Cf(void 0, void 0, void 0, (function() {
+                                return vf(void 0, void 0, void 0, (function() {
                                     var o, i, a, s, u, l, c, d;
-                                    return Ef(this, (function(f) {
+                                    return Mf(this, (function(f) {
                                         switch (f.label) {
                                             case 0:
-                                                return o = r.request, fl.isInstance(o) ? (i = o.headers, a = (null === (c = null === t || void 0 === t ? void 0 : t.userAgent) || void 0 === c ? void 0 : c.map(zf)) || [], [4, n.defaultUserAgentProvider()]) : [2, e(r)];
+                                                return o = r.request, el.isInstance(o) ? (i = o.headers, a = (null === (c = null === t || void 0 === t ? void 0 : t.userAgent) || void 0 === c ? void 0 : c.map(Nf)) || [], [4, n.defaultUserAgentProvider()]) : [2, e(r)];
                                             case 1:
-                                                return s = f.sent().map(zf), u = (null === (d = null === n || void 0 === n ? void 0 : n.customUserAgent) || void 0 === d ? void 0 : d.map(zf)) || [], i["x-amz-user-agent"] = Tf(s, a, u).join(" "), l = Tf(s.filter((function(e) {
+                                                return s = f.sent().map(Nf), u = (null === (d = null === n || void 0 === n ? void 0 : n.customUserAgent) || void 0 === d ? void 0 : d.map(Nf)) || [], i["x-amz-user-agent"] = wf(s, a, u).join(" "), l = wf(s.filter((function(e) {
                                                     return e.startsWith("aws-sdk-")
-                                                })), u).join(" "), "browser" !== n.runtime && l && (i[Af] = i[Af] ? i[Af] + " " + l : l), [2, e(kf(kf({}, r), {
+                                                })), u).join(" "), "browser" !== n.runtime && l && (i[jf] = i[jf] ? i[jf] + " " + l : l), [2, e(mf(mf({}, r), {
                                                     request: o
                                                 }))]
                                         }
                                     }))
                                 }))
                             }
-                        }), Uf)
+                        }), If)
                     }
                 }
             },
-            Rf = function(e) {
+            Sf = function(e) {
                 function t(t) {
                     var n, r, o = this,
                         i = function(e) {
                             if (!e.region) throw new Error("Region is missing");
-                            return md(md({}, e), {
-                                region: jd(e.region)
+                            return id(id({}, e), {
+                                region: cd(e.region)
                             })
-                        }(nu(nu({}, yd), t)),
+                        }(Gs(Gs({}, od), t)),
                         a = function(e) {
                             var t;
-                            return md(md({}, e), {
+                            return id(id({}, e), {
                                 tls: null === (t = e.tls) || void 0 === t || t,
-                                endpoint: e.endpoint ? bd(e) : function() {
-                                    return wd(e)
+                                endpoint: e.endpoint ? ud(e) : function() {
+                                    return ld(e)
                                 },
                                 isCustomEndpoint: !!e.endpoint
                             })
                         }(i),
                         s = function(e) {
                             var t, n = this,
-                                r = Lf(e.credentials || e.credentialDefaultProvider(e)),
+                                r = yf(e.credentials || e.credentialDefaultProvider(e)),
                                 o = e.signingEscapePath,
                                 i = void 0 === o || o,
                                 a = e.systemClockOffset,
                                 s = void 0 === a ? e.systemClockOffset || 0 : a,
                                 u = e.sha256;
-                            return t = e.signer ? Lf(e.signer) : function() {
-                                return Lf(e.region)().then((function(t) {
-                                    return Pd(n, void 0, void 0, (function() {
-                                        return Rd(this, (function(n) {
+                            return t = e.signer ? yf(e.signer) : function() {
+                                return yf(e.region)().then((function(t) {
+                                    return Dd(n, void 0, void 0, (function() {
+                                        return Sd(this, (function(n) {
                                             switch (n.label) {
                                                 case 0:
                                                     return [4, e.regionInfoProvider(t)];
                                                 case 1:
                                                     return [2, [n.sent() || {}, t]]
                                             }
                                         }))
                                     }))
                                 })).then((function(t) {
-                                    var n = Bd(t, 2),
+                                    var n = Ld(t, 2),
                                         o = n[0],
                                         a = n[1],
                                         s = o.signingRegion,
                                         l = o.signingService;
-                                    return e.signingRegion = e.signingRegion || s || a, e.signingName = e.signingName || l || e.serviceId, new xf({
+                                    return e.signingRegion = e.signingRegion || s || a, e.signingName = e.signingName || l || e.serviceId, new df({
                                         credentials: r,
                                         region: e.signingRegion,
                                         service: e.signingName,
                                         sha256: u,
                                         uriEscapePath: i
                                     })
                                 }))
-                            }, Ud(Ud({}, e), {
+                            }, Id(Id({}, e), {
                                 systemClockOffset: s,
                                 signingEscapePath: i,
                                 credentials: r,
                                 signer: t
                             })
                         }(a),
                         u = function(e) {
-                            var t = ed(e.maxAttempts);
-                            return Pc(Pc({}, e), {
+                            var t = Yc(e.maxAttempts);
+                            return Dc(Dc({}, e), {
                                 maxAttempts: t,
-                                retryStrategy: e.retryStrategy || new $c(t)
+                                retryStrategy: e.retryStrategy || new Fc(t)
                             })
                         }(s),
-                        l = kf(kf({}, n = u), {
+                        l = mf(mf({}, n = u), {
                             customUserAgent: "string" === typeof n.customUserAgent ? [
                                 [n.customUserAgent]
                             ] : n.customUserAgent
                         });
                     return (o = e.call(this, l) || this).config = l, o.middlewareStack.use((r = o.config, {
                         applyToStack: function(e) {
-                            e.add(Yc(r), Qc)
+                            e.add(Cc(r), Ec)
                         }
-                    })), o.middlewareStack.use(Ld(o.config)), o.middlewareStack.use(_d(o.config)), o.middlewareStack.use((o.config, {
+                    })), o.middlewareStack.use(yd(o.config)), o.middlewareStack.use(bd(o.config)), o.middlewareStack.use((o.config, {
                         applyToStack: function(e) {
-                            e.add(Od(), zd)
+                            e.add(xd(), Nd)
                         }
-                    })), o.middlewareStack.use(Pf(o.config)), o
+                    })), o.middlewareStack.use(Df(o.config)), o
                 }
-                return tu(t, e), t.prototype.destroy = function() {
+                return Qs(t, e), t.prototype.destroy = function() {
                     e.prototype.destroy.call(this)
                 }, t
-            }(rc),
-            Bf = "aws-amplify/5.0.10",
-            Ff = {
-                userAgent: Bf + " js",
+            }(Wl),
+            Lf = "aws-amplify/5.0.10",
+            kf = {
+                userAgent: Lf + " js",
                 product: "",
                 navigator: null,
                 isReactNative: !1
             };
         if ("undefined" !== typeof navigator && navigator.product)
-            if (Ff.product = navigator.product || "", Ff.navigator = navigator || null, "ReactNative" === navigator.product) Ff.userAgent = Bf + " react-native", Ff.isReactNative = !0;
-            else Ff.userAgent = Bf + " js", Ff.isReactNative = !1;
+            if (kf.product = navigator.product || "", kf.navigator = navigator || null, "ReactNative" === navigator.product) kf.userAgent = Lf + " react-native", kf.isReactNative = !0;
+            else kf.userAgent = Lf + " js", kf.isReactNative = !1;
 
-        function Yf(e) {
-            var t, n = new Rf({
+        function Cf(e) {
+            var t, n = new Sf({
                 region: e.region,
-                customUserAgent: "" + Ff.userAgent + (t || "")
+                customUserAgent: "" + kf.userAgent + (t || "")
             });
             return n.middlewareStack.add((function(e, t) {
                 return function(t) {
                     return e(function(e) {
-                        return bs(bs({}, e), {
-                            request: bs(bs({}, e.request), {
-                                headers: bs(bs({}, e.request.headers), {
+                        return us(us({}, e), {
+                            request: us(us({}, e.request), {
+                                headers: us(us({}, e.request.headers), {
                                     "cache-control": "no-store"
                                 })
                             })
                         })
                     }(t))
                 }
             }), {
                 step: "build",
                 name: "cacheControlMiddleWare"
             }), n
         }
-        var Qf = new Ls("Credentials"),
-            Gf = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
-            Wf = function() {
+        var Ef = new ys("Credentials"),
+            _f = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
+            Tf = function() {
                 function e(e) {
-                    this._gettingCredPromise = null, this._refreshHandlers = {}, this.Auth = void 0, this.configure(e), this._refreshHandlers.google = Zs.refreshGoogleToken, this._refreshHandlers.facebook = Vs.refreshFacebookToken
+                    this._gettingCredPromise = null, this._refreshHandlers = {}, this.Auth = void 0, this.configure(e), this._refreshHandlers.google = Os.refreshGoogleToken, this._refreshHandlers.facebook = zs.refreshFacebookToken
                 }
                 return e.prototype.getModuleName = function() {
                     return "Credentials"
                 }, e.prototype.getCredSource = function() {
                     return this._credentials_source
                 }, e.prototype.configure = function(e) {
                     if (!e) return this._config || {};
                     this._config = Object.assign({}, this._config, e);
                     var t = this._config.refreshHandlers;
-                    return t && (this._refreshHandlers = bs(bs({}, this._refreshHandlers), t)), this._storage = this._config.storage, this._storage || (this._storage = (new Os).getStorage()), this._storageSync = Promise.resolve(), "function" === typeof this._storage.sync && (this._storageSync = this._storage.sync()),
+                    return t && (this._refreshHandlers = us(us({}, this._refreshHandlers), t)), this._storage = this._config.storage, this._storage || (this._storage = (new xs).getStorage()), this._storageSync = Promise.resolve(), "function" === typeof this._storage.sync && (this._storageSync = this._storage.sync()),
                         function(e, t, n) {
-                            _s.dispatch("core", {
+                            bs.dispatch("core", {
                                 event: e,
                                 data: t,
                                 message: n
-                            }, "Credentials", Gf)
+                            }, "Credentials", _f)
                         }("credentials_configured", null, "Credentials has been configured successfully"), this._config
                 }, e.prototype.get = function() {
-                    return Qf.debug("getting credentials"), this._pickupCredentials()
+                    return Ef.debug("getting credentials"), this._pickupCredentials()
                 }, e.prototype._getCognitoIdentityIdStorageKey = function(e) {
                     return "CognitoIdentityId-" + e
                 }, e.prototype._pickupCredentials = function() {
-                    return Qf.debug("picking up credentials"), this._gettingCredPromise && this._gettingCredPromise.isPending() ? Qf.debug("getting old cred promise") : (Qf.debug("getting new cred promise"), this._gettingCredPromise = function(e) {
+                    return Ef.debug("picking up credentials"), this._gettingCredPromise && this._gettingCredPromise.isPending() ? Ef.debug("getting old cred promise") : (Ef.debug("getting new cred promise"), this._gettingCredPromise = function(e) {
                         if (e.isResolved) return e;
                         var t = !0,
                             n = !1,
                             r = !1,
                             o = e.then((function(e) {
                                 return r = !0, t = !1, e
                             }), (function(e) {
@@ -64427,152 +61875,152 @@
                         }, o.isPending = function() {
                             return t
                         }, o.isRejected = function() {
                             return n
                         }, o
                     }(this._keepAlive())), this._gettingCredPromise
                 }, e.prototype._keepAlive = function() {
-                    return ws(this, void 0, void 0, (function() {
+                    return ls(this, void 0, void 0, (function() {
                         var e, t, n, r, o, i, a;
-                        return js(this, (function(s) {
+                        return cs(this, (function(s) {
                             switch (s.label) {
                                 case 0:
-                                    if (Qf.debug("checking if credentials exists and not expired"), (e = this._credentials) && !this._isExpired(e) && !this._isPastTTL()) return Qf.debug("credentials not changed and not expired, directly return"), [2, Promise.resolve(e)];
-                                    if (Qf.debug("need to get a new credential or refresh the existing one"), t = this.Auth, !(n = void 0 === t ? Js.Auth : t) || "function" !== typeof n.currentUserCredentials) return [2, this._setCredentialsForGuest()];
+                                    if (Ef.debug("checking if credentials exists and not expired"), (e = this._credentials) && !this._isExpired(e) && !this._isPastTTL()) return Ef.debug("credentials not changed and not expired, directly return"), [2, Promise.resolve(e)];
+                                    if (Ef.debug("need to get a new credential or refresh the existing one"), t = this.Auth, !(n = void 0 === t ? Ps.Auth : t) || "function" !== typeof n.currentUserCredentials) return [2, this._setCredentialsForGuest()];
                                     if (this._isExpired(e) || !this._isPastTTL()) return [3, 6];
-                                    Qf.debug("ttl has passed but token is not yet expired"), s.label = 1;
+                                    Ef.debug("ttl has passed but token is not yet expired"), s.label = 1;
                                 case 1:
                                     return s.trys.push([1, 5, , 6]), [4, n.currentUserPoolUser()];
                                 case 2:
                                     return r = s.sent(), [4, n.currentSession()];
                                 case 3:
                                     return o = s.sent(), i = o.refreshToken, [4, new Promise((function(e, t) {
                                         r.refreshSession(i, (function(n, r) {
                                             return n ? t(n) : e(r)
                                         }))
                                     }))];
                                 case 4:
                                     return s.sent(), [3, 6];
                                 case 5:
-                                    return a = s.sent(), Qf.debug("Error attempting to refreshing the session", a), [3, 6];
+                                    return a = s.sent(), Ef.debug("Error attempting to refreshing the session", a), [3, 6];
                                 case 6:
                                     return [2, n.currentUserCredentials()]
                             }
                         }))
                     }))
                 }, e.prototype.refreshFederatedToken = function(e) {
-                    Qf.debug("Getting federated credentials");
+                    Ef.debug("Getting federated credentials");
                     var t = e.provider,
                         n = e.user,
                         r = e.token,
                         o = e.identity_id,
                         i = e.expires_at;
                     i = 1970 === new Date(i).getFullYear() ? 1e3 * i : i;
                     var a = this;
-                    return Qf.debug("checking if federated jwt token expired"), i > (new Date).getTime() ? (Qf.debug("token not expired"), this._setCredentialsFromFederation({
+                    return Ef.debug("checking if federated jwt token expired"), i > (new Date).getTime() ? (Ef.debug("token not expired"), this._setCredentialsFromFederation({
                         provider: t,
                         token: r,
                         user: n,
                         identity_id: o,
                         expires_at: i
-                    })) : a._refreshHandlers[t] && "function" === typeof a._refreshHandlers[t] ? (Qf.debug("getting refreshed jwt token from federation provider"), this._providerRefreshWithRetry({
+                    })) : a._refreshHandlers[t] && "function" === typeof a._refreshHandlers[t] ? (Ef.debug("getting refreshed jwt token from federation provider"), this._providerRefreshWithRetry({
                         refreshHandler: a._refreshHandlers[t],
                         provider: t,
                         user: n
-                    })) : (Qf.debug("no refresh handler for provider:", t), this.clear(), Promise.reject("no refresh handler for provider"))
+                    })) : (Ef.debug("no refresh handler for provider:", t), this.clear(), Promise.reject("no refresh handler for provider"))
                 }, e.prototype._providerRefreshWithRetry = function(e) {
                     var t = this,
                         n = e.refreshHandler,
                         r = e.provider,
                         o = e.user;
-                    return Bs(n, [], 1e4).then((function(e) {
-                        return Qf.debug("refresh federated token sucessfully", e), t._setCredentialsFromFederation({
+                    return Ls(n, [], 1e4).then((function(e) {
+                        return Ef.debug("refresh federated token sucessfully", e), t._setCredentialsFromFederation({
                             provider: r,
                             token: e.token,
                             user: o,
                             identity_id: e.identity_id,
                             expires_at: e.expires_at
                         })
                     })).catch((function(e) {
-                        return "string" === typeof e && 0 === e.toLowerCase().lastIndexOf("network error", e.length) || t.clear(), Qf.debug("refresh federated token failed", e), Promise.reject("refreshing federation token failed: " + e)
+                        return "string" === typeof e && 0 === e.toLowerCase().lastIndexOf("network error", e.length) || t.clear(), Ef.debug("refresh federated token failed", e), Promise.reject("refreshing federation token failed: " + e)
                     }))
                 }, e.prototype._isExpired = function(e) {
-                    if (!e) return Qf.debug("no credentials for expiration check"), !0;
-                    Qf.debug("are these credentials expired?", e);
+                    if (!e) return Ef.debug("no credentials for expiration check"), !0;
+                    Ef.debug("are these credentials expired?", e);
                     var t = Date.now();
                     return e.expiration.getTime() <= t
                 }, e.prototype._isPastTTL = function() {
                     return this._nextCredentialsRefresh <= Date.now()
                 }, e.prototype._setCredentialsForGuest = function() {
                     var e;
-                    return ws(this, void 0, void 0, (function() {
+                    return ls(this, void 0, void 0, (function() {
                         var t, n, r, o, i, a, s, u, l, c, d = this;
-                        return js(this, (function(f) {
+                        return cs(this, (function(f) {
                             switch (f.label) {
                                 case 0:
-                                    return Qf.debug("setting credentials for guest"), (null === (e = this._config) || void 0 === e ? void 0 : e.identityPoolId) || (this._config = Object.assign({}, this._config, bc(this._config || {}).Auth)), t = this._config, n = t.identityPoolId, r = t.region, o = t.mandatorySignIn, i = t.identityPoolRegion, o ? [2, Promise.reject("cannot get guest credentials when mandatory signin enabled")] : n ? i || r ? (s = this, [4, this._getGuestIdentityId()]) : (Qf.debug("region is not configured for getting the credentials"), [2, Promise.reject("region is not configured for getting the credentials")]) : (Qf.debug("No Cognito Identity pool provided for unauthenticated access"), [2, Promise.reject("No Cognito Identity pool provided for unauthenticated access")]);
+                                    return Ef.debug("setting credentials for guest"), (null === (e = this._config) || void 0 === e ? void 0 : e.identityPoolId) || (this._config = Object.assign({}, this._config, uc(this._config || {}).Auth)), t = this._config, n = t.identityPoolId, r = t.region, o = t.mandatorySignIn, i = t.identityPoolRegion, o ? [2, Promise.reject("cannot get guest credentials when mandatory signin enabled")] : n ? i || r ? (s = this, [4, this._getGuestIdentityId()]) : (Ef.debug("region is not configured for getting the credentials"), [2, Promise.reject("region is not configured for getting the credentials")]) : (Ef.debug("No Cognito Identity pool provided for unauthenticated access"), [2, Promise.reject("No Cognito Identity pool provided for unauthenticated access")]);
                                 case 1:
-                                    return a = s._identityId = f.sent(), u = Yf({
+                                    return a = s._identityId = f.sent(), u = Cf({
                                         region: i || r
-                                    }), l = void 0, a ? l = pc({
+                                    }), l = void 0, a ? l = tc({
                                         identityId: a,
                                         client: u
                                     })() : (c = function() {
-                                        return ws(d, void 0, void 0, (function() {
+                                        return ls(d, void 0, void 0, (function() {
                                             var e;
-                                            return js(this, (function(t) {
+                                            return cs(this, (function(t) {
                                                 switch (t.label) {
                                                     case 0:
-                                                        return [4, u.send(new hc({
+                                                        return [4, u.send(new nc({
                                                             IdentityPoolId: n
                                                         }))];
                                                     case 1:
-                                                        return e = t.sent().IdentityId, this._identityId = e, [2, pc({
+                                                        return e = t.sent().IdentityId, this._identityId = e, [2, tc({
                                                             client: u,
                                                             identityId: e
                                                         })()]
                                                 }
                                             }))
                                         }))
                                     }, l = c().catch((function(e) {
-                                        return ws(d, void 0, void 0, (function() {
-                                            return js(this, (function(t) {
+                                        return ls(d, void 0, void 0, (function() {
+                                            return cs(this, (function(t) {
                                                 throw e
                                             }))
                                         }))
                                     }))), [2, this._loadCredentials(l, "guest", !1, null).then((function(e) {
                                         return e
                                     })).catch((function(e) {
-                                        return ws(d, void 0, void 0, (function() {
+                                        return ls(d, void 0, void 0, (function() {
                                             var t, r = this;
-                                            return js(this, (function(o) {
+                                            return cs(this, (function(o) {
                                                 switch (o.label) {
                                                     case 0:
-                                                        return "ResourceNotFoundException" !== e.name || e.message !== "Identity '" + a + "' not found." ? [3, 2] : (Qf.debug("Failed to load guest credentials"), [4, this._removeGuestIdentityId()]);
+                                                        return "ResourceNotFoundException" !== e.name || e.message !== "Identity '" + a + "' not found." ? [3, 2] : (Ef.debug("Failed to load guest credentials"), [4, this._removeGuestIdentityId()]);
                                                     case 1:
                                                         return o.sent(), t = function() {
-                                                            return ws(r, void 0, void 0, (function() {
+                                                            return ls(r, void 0, void 0, (function() {
                                                                 var e;
-                                                                return js(this, (function(t) {
+                                                                return cs(this, (function(t) {
                                                                     switch (t.label) {
                                                                         case 0:
-                                                                            return [4, u.send(new hc({
+                                                                            return [4, u.send(new nc({
                                                                                 IdentityPoolId: n
                                                                             }))];
                                                                         case 1:
-                                                                            return e = t.sent().IdentityId, this._identityId = e, [2, pc({
+                                                                            return e = t.sent().IdentityId, this._identityId = e, [2, tc({
                                                                                 client: u,
                                                                                 identityId: e
                                                                             })()]
                                                                     }
                                                                 }))
                                                             }))
                                                         }, l = t().catch((function(e) {
-                                                            return ws(r, void 0, void 0, (function() {
-                                                                return js(this, (function(t) {
+                                                            return ls(r, void 0, void 0, (function() {
+                                                                return cs(this, (function(t) {
                                                                     throw e
                                                                 }))
                                                             }))
                                                         })), [2, this._loadCredentials(l, "guest", !1, null)];
                                                     case 2:
                                                         return [2, e]
                                                 }
@@ -64595,191 +62043,191 @@
                     if (!o) return Promise.reject("You must specify a federated provider");
                     var i = {};
                     i[o] = n;
                     var a = this._config,
                         s = a.identityPoolId,
                         u = a.region,
                         l = a.identityPoolRegion;
-                    if (!s) return Qf.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
-                    if (!l && !u) return Qf.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
-                    var c = Yf({
+                    if (!s) return Ef.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
+                    if (!l && !u) return Ef.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
+                    var c = Cf({
                             region: l || u
                         }),
                         d = void 0;
-                    r ? d = pc({
+                    r ? d = tc({
                         identityId: r,
                         logins: i,
                         client: c
-                    })() : d = vc({
+                    })() : d = ac({
                         logins: i,
                         identityPoolId: s,
                         client: c
                     })();
                     return this._loadCredentials(d, "federated", !0, e)
                 }, e.prototype._setCredentialsFromSession = function(e) {
                     var t = this;
-                    Qf.debug("set credentials from session");
+                    Ef.debug("set credentials from session");
                     var n = e.getIdToken().getJwtToken(),
                         r = this._config,
                         o = r.region,
                         i = r.userPoolId,
                         a = r.identityPoolId,
                         s = r.identityPoolRegion;
-                    if (!a) return Qf.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
-                    if (!s && !o) return Qf.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
+                    if (!a) return Ef.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
+                    if (!s && !o) return Ef.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
                     var u = {};
                     u["cognito-idp." + o + ".amazonaws.com/" + i] = n;
-                    var l = Yf({
+                    var l = Cf({
                             region: s || o
                         }),
-                        c = ws(t, void 0, void 0, (function() {
+                        c = ls(t, void 0, void 0, (function() {
                             var e, t, n, r, o, i, s, c, d, f;
-                            return js(this, (function(p) {
+                            return cs(this, (function(p) {
                                 switch (p.label) {
                                     case 0:
                                         return [4, this._getGuestIdentityId()];
                                     case 1:
-                                        return (e = p.sent()) ? [3, 3] : [4, l.send(new hc({
+                                        return (e = p.sent()) ? [3, 3] : [4, l.send(new nc({
                                             IdentityPoolId: a,
                                             Logins: u
                                         }))];
                                     case 2:
                                         n = p.sent().IdentityId, t = n, p.label = 3;
                                     case 3:
-                                        return [4, l.send(new lc({
+                                        return [4, l.send(new Kl({
                                             IdentityId: e || t,
                                             Logins: u
                                         }))];
                                     case 4:
-                                        return r = p.sent(), o = r.Credentials, i = o.AccessKeyId, s = o.Expiration, c = o.SecretKey, d = o.SessionToken, f = r.IdentityId, this._identityId = f, e ? (Qf.debug("The guest identity " + e + " has been successfully linked to the logins"), e === f && Qf.debug("The guest identity " + e + " has become the primary identity"), [4, this._removeGuestIdentityId()]) : [3, 6];
+                                        return r = p.sent(), o = r.Credentials, i = o.AccessKeyId, s = o.Expiration, c = o.SecretKey, d = o.SessionToken, f = r.IdentityId, this._identityId = f, e ? (Ef.debug("The guest identity " + e + " has been successfully linked to the logins"), e === f && Ef.debug("The guest identity " + e + " has become the primary identity"), [4, this._removeGuestIdentityId()]) : [3, 6];
                                     case 5:
                                         p.sent(), p.label = 6;
                                     case 6:
                                         return [2, {
                                             accessKeyId: i,
                                             secretAccessKey: c,
                                             sessionToken: d,
                                             expiration: s,
                                             identityId: f
                                         }]
                                 }
                             }))
                         })).catch((function(e) {
-                            return ws(t, void 0, void 0, (function() {
-                                return js(this, (function(t) {
+                            return ls(t, void 0, void 0, (function() {
+                                return cs(this, (function(t) {
                                     throw e
                                 }))
                             }))
                         }));
                     return this._loadCredentials(c, "userPool", !0, null)
                 }, e.prototype._loadCredentials = function(e, t, n, r) {
                     var o = this,
                         i = this;
                     return new Promise((function(a, s) {
                         e.then((function(e) {
-                            return ws(o, void 0, void 0, (function() {
+                            return ls(o, void 0, void 0, (function() {
                                 var o, s, u, l, c;
-                                return js(this, (function(d) {
+                                return cs(this, (function(d) {
                                     switch (d.label) {
                                         case 0:
-                                            if (Qf.debug("Load credentials successfully", e), this._identityId && !e.identityId && (e.identityId = this._identityId), i._credentials = e, i._credentials.authenticated = n, i._credentials_source = t, i._nextCredentialsRefresh = (new Date).getTime() + 3e6, "federated" === t) {
+                                            if (Ef.debug("Load credentials successfully", e), this._identityId && !e.identityId && (e.identityId = this._identityId), i._credentials = e, i._credentials.authenticated = n, i._credentials_source = t, i._nextCredentialsRefresh = (new Date).getTime() + 3e6, "federated" === t) {
                                                 o = Object.assign({
                                                     id: this._credentials.identityId
                                                 }, r.user), s = r.provider, u = r.token, l = r.expires_at, c = r.identity_id;
                                                 try {
                                                     this._storage.setItem("aws-amplify-federatedInfo", JSON.stringify({
                                                         provider: s,
                                                         token: u,
                                                         user: o,
                                                         expires_at: l,
                                                         identity_id: c
                                                     }))
                                                 } catch (f) {
-                                                    Qf.debug("Failed to put federated info into auth storage", f)
+                                                    Ef.debug("Failed to put federated info into auth storage", f)
                                                 }
                                             }
                                             return "guest" !== t ? [3, 2] : [4, this._setGuestIdentityId(e.identityId)];
                                         case 1:
                                             d.sent(), d.label = 2;
                                         case 2:
                                             return a(i._credentials), [2]
                                     }
                                 }))
                             }))
                         })).catch((function(t) {
-                            if (t) return Qf.debug("Failed to load credentials", e), Qf.debug("Error loading credentials", t), void s(t)
+                            if (t) return Ef.debug("Failed to load credentials", e), Ef.debug("Error loading credentials", t), void s(t)
                         }))
                     }))
                 }, e.prototype.set = function(e, t) {
-                    return "session" === t ? this._setCredentialsFromSession(e) : "federation" === t ? this._setCredentialsFromFederation(e) : "guest" === t ? this._setCredentialsForGuest() : (Qf.debug("no source specified for setting credentials"), Promise.reject("invalid source"))
+                    return "session" === t ? this._setCredentialsFromSession(e) : "federation" === t ? this._setCredentialsFromFederation(e) : "guest" === t ? this._setCredentialsForGuest() : (Ef.debug("no source specified for setting credentials"), Promise.reject("invalid source"))
                 }, e.prototype.clear = function() {
-                    return ws(this, void 0, void 0, (function() {
-                        return js(this, (function(e) {
-                            return this._credentials = null, this._credentials_source = null, Qf.debug("removing aws-amplify-federatedInfo from storage"), this._storage.removeItem("aws-amplify-federatedInfo"), [2]
+                    return ls(this, void 0, void 0, (function() {
+                        return cs(this, (function(e) {
+                            return this._credentials = null, this._credentials_source = null, Ef.debug("removing aws-amplify-federatedInfo from storage"), this._storage.removeItem("aws-amplify-federatedInfo"), [2]
                         }))
                     }))
                 }, e.prototype._getGuestIdentityId = function() {
-                    return ws(this, void 0, void 0, (function() {
+                    return ls(this, void 0, void 0, (function() {
                         var e, t;
-                        return js(this, (function(n) {
+                        return cs(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     e = this._config.identityPoolId, n.label = 1;
                                 case 1:
                                     return n.trys.push([1, 3, , 4]), [4, this._storageSync];
                                 case 2:
                                     return n.sent(), [2, this._storage.getItem(this._getCognitoIdentityIdStorageKey(e))];
                                 case 3:
-                                    return t = n.sent(), Qf.debug("Failed to get the cached guest identityId", t), [3, 4];
+                                    return t = n.sent(), Ef.debug("Failed to get the cached guest identityId", t), [3, 4];
                                 case 4:
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype._setGuestIdentityId = function(e) {
-                    return ws(this, void 0, void 0, (function() {
+                    return ls(this, void 0, void 0, (function() {
                         var t, n;
-                        return js(this, (function(r) {
+                        return cs(this, (function(r) {
                             switch (r.label) {
                                 case 0:
                                     t = this._config.identityPoolId, r.label = 1;
                                 case 1:
                                     return r.trys.push([1, 3, , 4]), [4, this._storageSync];
                                 case 2:
                                     return r.sent(), this._storage.setItem(this._getCognitoIdentityIdStorageKey(t), e), [3, 4];
                                 case 3:
-                                    return n = r.sent(), Qf.debug("Failed to cache guest identityId", n), [3, 4];
+                                    return n = r.sent(), Ef.debug("Failed to cache guest identityId", n), [3, 4];
                                 case 4:
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype._removeGuestIdentityId = function() {
-                    return ws(this, void 0, void 0, (function() {
+                    return ls(this, void 0, void 0, (function() {
                         var e;
-                        return js(this, (function(t) {
-                            return e = this._config.identityPoolId, Qf.debug("removing " + this._getCognitoIdentityIdStorageKey(e) + " from storage"), this._storage.removeItem(this._getCognitoIdentityIdStorageKey(e)), [2]
+                        return cs(this, (function(t) {
+                            return e = this._config.identityPoolId, Ef.debug("removing " + this._getCognitoIdentityIdStorageKey(e) + " from storage"), this._storage.removeItem(this._getCognitoIdentityIdStorageKey(e)), [2]
                         }))
                     }))
                 }, e.prototype.shear = function(e) {
                     return {
                         accessKeyId: e.accessKeyId,
                         sessionToken: e.sessionToken,
                         secretAccessKey: e.secretAccessKey,
                         identityId: e.identityId,
                         authenticated: e.authenticated
                     }
                 }, e
             }(),
-            Hf = new Wf(null);
-        Js.register(Hf);
-        var Zf = zs().isBrowser,
-            Vf = function() {
+            Af = new Tf(null);
+        Ps.register(Af);
+        var Of = Ns().isBrowser,
+            zf = function() {
                 function e(e) {
-                    void 0 === e && (e = {}), this.cookies = new tt, this.store = Zf ? window.localStorage : Object.create(null), this.cookies = e.req ? new tt(e.req.headers.cookie) : new tt, Object.assign(this.store, this.cookies.getAll())
+                    void 0 === e && (e = {}), this.cookies = new tt, this.store = Of ? window.localStorage : Object.create(null), this.cookies = e.req ? new tt(e.req.headers.cookie) : new tt, Object.assign(this.store, this.cookies.getAll())
                 }
                 return Object.defineProperty(e.prototype, "length", {
                     get: function() {
                         return Object.entries(this.store).length
                     },
                     enumerable: !0,
                     configurable: !0
@@ -64811,22 +62259,22 @@
                     var n = e.split(".").pop();
                     ["LastAuthUser", "accessToken", "refreshToken", "idToken"].includes(null !== n && void 0 !== n ? n : "") && this.setUniversalItem(e, t, {
                         expires: new Date(Date.now() + 31536e6)
                     })
                 }, e.prototype.setLocalItem = function(e, t) {
                     this.store[e] = t
                 }, e.prototype.setUniversalItem = function(e, t, n) {
-                    void 0 === n && (n = {}), this.cookies.set(e, t, bs(bs({}, n), {
+                    void 0 === n && (n = {}), this.cookies.set(e, t, us(us({}, n), {
                         path: "/",
                         sameSite: !0,
-                        secure: !Zf || "localhost" !== window.location.hostname
+                        secure: !Of || "localhost" !== window.location.hostname
                     }))
                 }, e
             }();
-        var qf, Jf = function() {
+        var Uf, Pf = function() {
                 function e(e) {
                     var t = e || {},
                         n = t.ValidationData,
                         r = t.Username,
                         o = t.Password,
                         i = t.AuthParameters,
                         a = t.ClientMetadata;
@@ -64841,253 +62289,253 @@
                     return this.validationData
                 }, t.getAuthParameters = function() {
                     return this.authParameters
                 }, t.getClientMetadata = function() {
                     return this.clientMetadata
                 }, e
             }(),
-            Kf = __webpack_require__(2890);
+            Rf = __webpack_require__(2890);
 
-        function Xf() {
-            if (qf) {
-                if ("function" === typeof qf.getRandomValues) try {
-                    return qf.getRandomValues(new Uint32Array(1))[0]
+        function Bf() {
+            if (Uf) {
+                if ("function" === typeof Uf.getRandomValues) try {
+                    return Uf.getRandomValues(new Uint32Array(1))[0]
                 } catch (e) {}
-                if ("function" === typeof qf.randomBytes) try {
-                    return qf.randomBytes(4).readInt32LE()
+                if ("function" === typeof Uf.randomBytes) try {
+                    return Uf.randomBytes(4).readInt32LE()
                 } catch (e) {}
             }
             throw new Error("Native crypto module could not be used to get secure random number.")
         }
-        "undefined" !== typeof window && window.crypto && (qf = window.crypto), !qf && "undefined" !== typeof window && window.msCrypto && (qf = window.msCrypto);
-        var $f, ep = function() {
+        "undefined" !== typeof window && window.crypto && (Uf = window.crypto), !Uf && "undefined" !== typeof window && window.msCrypto && (Uf = window.msCrypto);
+        var Ff, Yf = function() {
                 function e(e, t) {
                     e = this.words = e || [], this.sigBytes = void 0 != t ? t : 4 * e.length
                 }
                 var t = e.prototype;
                 return t.random = function(t) {
-                    for (var n = [], r = 0; r < t; r += 4) n.push(Xf());
+                    for (var n = [], r = 0; r < t; r += 4) n.push(Bf());
                     return new e(n, t)
                 }, t.toString = function() {
                     return function(e) {
                         for (var t = e.words, n = e.sigBytes, r = [], o = 0; o < n; o++) {
                             var i = t[o >>> 2] >>> 24 - o % 4 * 8 & 255;
                             r.push((i >>> 4).toString(16)), r.push((15 & i).toString(16))
                         }
                         return r.join("")
                     }(this)
                 }, e
             }(),
-            tp = __webpack_require__(6915),
-            np = rp;
+            Qf = __webpack_require__(6915),
+            Gf = Wf;
 
-        function rp(e, t) {
+        function Wf(e, t) {
             null != e && this.fromString(e, t)
         }
 
-        function op() {
-            return new rp(null)
+        function Hf() {
+            return new Wf(null)
         }
-        var ip = "undefined" !== typeof navigator;
-        ip && "Microsoft Internet Explorer" == navigator.appName ? (rp.prototype.am = function(e, t, n, r, o, i) {
+        var Zf = "undefined" !== typeof navigator;
+        Zf && "Microsoft Internet Explorer" == navigator.appName ? (Wf.prototype.am = function(e, t, n, r, o, i) {
             for (var a = 32767 & t, s = t >> 15; --i >= 0;) {
                 var u = 32767 & this[e],
                     l = this[e++] >> 15,
                     c = s * u + l * a;
                 o = ((u = a * u + ((32767 & c) << 15) + n[r] + (1073741823 & o)) >>> 30) + (c >>> 15) + s * l + (o >>> 30), n[r++] = 1073741823 & u
             }
             return o
-        }, $f = 30) : ip && "Netscape" != navigator.appName ? (rp.prototype.am = function(e, t, n, r, o, i) {
+        }, Ff = 30) : Zf && "Netscape" != navigator.appName ? (Wf.prototype.am = function(e, t, n, r, o, i) {
             for (; --i >= 0;) {
                 var a = t * this[e++] + n[r] + o;
                 o = Math.floor(a / 67108864), n[r++] = 67108863 & a
             }
             return o
-        }, $f = 26) : (rp.prototype.am = function(e, t, n, r, o, i) {
+        }, Ff = 26) : (Wf.prototype.am = function(e, t, n, r, o, i) {
             for (var a = 16383 & t, s = t >> 14; --i >= 0;) {
                 var u = 16383 & this[e],
                     l = this[e++] >> 14,
                     c = s * u + l * a;
                 o = ((u = a * u + ((16383 & c) << 14) + n[r] + o) >> 28) + (c >> 14) + s * l, n[r++] = 268435455 & u
             }
             return o
-        }, $f = 28), rp.prototype.DB = $f, rp.prototype.DM = (1 << $f) - 1, rp.prototype.DV = 1 << $f;
-        rp.prototype.FV = Math.pow(2, 52), rp.prototype.F1 = 52 - $f, rp.prototype.F2 = 2 * $f - 52;
-        var ap, sp, up = new Array;
-        for (ap = "0".charCodeAt(0), sp = 0; sp <= 9; ++sp) up[ap++] = sp;
-        for (ap = "a".charCodeAt(0), sp = 10; sp < 36; ++sp) up[ap++] = sp;
-        for (ap = "A".charCodeAt(0), sp = 10; sp < 36; ++sp) up[ap++] = sp;
+        }, Ff = 28), Wf.prototype.DB = Ff, Wf.prototype.DM = (1 << Ff) - 1, Wf.prototype.DV = 1 << Ff;
+        Wf.prototype.FV = Math.pow(2, 52), Wf.prototype.F1 = 52 - Ff, Wf.prototype.F2 = 2 * Ff - 52;
+        var Vf, qf, Jf = new Array;
+        for (Vf = "0".charCodeAt(0), qf = 0; qf <= 9; ++qf) Jf[Vf++] = qf;
+        for (Vf = "a".charCodeAt(0), qf = 10; qf < 36; ++qf) Jf[Vf++] = qf;
+        for (Vf = "A".charCodeAt(0), qf = 10; qf < 36; ++qf) Jf[Vf++] = qf;
 
-        function lp(e) {
+        function Kf(e) {
             return "0123456789abcdefghijklmnopqrstuvwxyz".charAt(e)
         }
 
-        function cp(e, t) {
-            var n = up[e.charCodeAt(t)];
+        function Xf(e, t) {
+            var n = Jf[e.charCodeAt(t)];
             return null == n ? -1 : n
         }
 
-        function dp(e) {
-            var t = op();
+        function $f(e) {
+            var t = Hf();
             return t.fromInt(e), t
         }
 
-        function fp(e) {
+        function ep(e) {
             var t, n = 1;
             return 0 != (t = e >>> 16) && (e = t, n += 16), 0 != (t = e >> 8) && (e = t, n += 8), 0 != (t = e >> 4) && (e = t, n += 4), 0 != (t = e >> 2) && (e = t, n += 2), 0 != (t = e >> 1) && (e = t, n += 1), n
         }
 
-        function pp(e) {
+        function tp(e) {
             this.m = e, this.mp = e.invDigit(), this.mpl = 32767 & this.mp, this.mph = this.mp >> 15, this.um = (1 << e.DB - 15) - 1, this.mt2 = 2 * e.t
         }
 
-        function hp(e) {
-            return Kf.lW.from((new ep).random(e).toString(), "hex")
+        function np(e) {
+            return Rf.lW.from((new Yf).random(e).toString(), "hex")
         }
-        pp.prototype.convert = function(e) {
-            var t = op();
-            return e.abs().dlShiftTo(this.m.t, t), t.divRemTo(this.m, null, t), e.s < 0 && t.compareTo(rp.ZERO) > 0 && this.m.subTo(t, t), t
-        }, pp.prototype.revert = function(e) {
-            var t = op();
+        tp.prototype.convert = function(e) {
+            var t = Hf();
+            return e.abs().dlShiftTo(this.m.t, t), t.divRemTo(this.m, null, t), e.s < 0 && t.compareTo(Wf.ZERO) > 0 && this.m.subTo(t, t), t
+        }, tp.prototype.revert = function(e) {
+            var t = Hf();
             return e.copyTo(t), this.reduce(t), t
-        }, pp.prototype.reduce = function(e) {
+        }, tp.prototype.reduce = function(e) {
             for (; e.t <= this.mt2;) e[e.t++] = 0;
             for (var t = 0; t < this.m.t; ++t) {
                 var n = 32767 & e[t],
                     r = n * this.mpl + ((n * this.mph + (e[t] >> 15) * this.mpl & this.um) << 15) & e.DM;
                 for (e[n = t + this.m.t] += this.m.am(0, r, e, t, 0, this.m.t); e[n] >= e.DV;) e[n] -= e.DV, e[++n]++
             }
             e.clamp(), e.drShiftTo(this.m.t, e), e.compareTo(this.m) >= 0 && e.subTo(this.m, e)
-        }, pp.prototype.mulTo = function(e, t, n) {
+        }, tp.prototype.mulTo = function(e, t, n) {
             e.multiplyTo(t, n), this.reduce(n)
-        }, pp.prototype.sqrTo = function(e, t) {
+        }, tp.prototype.sqrTo = function(e, t) {
             e.squareTo(t), this.reduce(t)
-        }, rp.prototype.copyTo = function(e) {
+        }, Wf.prototype.copyTo = function(e) {
             for (var t = this.t - 1; t >= 0; --t) e[t] = this[t];
             e.t = this.t, e.s = this.s
-        }, rp.prototype.fromInt = function(e) {
+        }, Wf.prototype.fromInt = function(e) {
             this.t = 1, this.s = e < 0 ? -1 : 0, e > 0 ? this[0] = e : e < -1 ? this[0] = e + this.DV : this.t = 0
-        }, rp.prototype.fromString = function(e, t) {
+        }, Wf.prototype.fromString = function(e, t) {
             var n;
             if (16 == t) n = 4;
             else if (8 == t) n = 3;
             else if (2 == t) n = 1;
             else if (32 == t) n = 5;
             else {
                 if (4 != t) throw new Error("Only radix 2, 4, 8, 16, 32 are supported");
                 n = 2
             }
             this.t = 0, this.s = 0;
             for (var r = e.length, o = !1, i = 0; --r >= 0;) {
-                var a = cp(e, r);
+                var a = Xf(e, r);
                 a < 0 ? "-" == e.charAt(r) && (o = !0) : (o = !1, 0 == i ? this[this.t++] = a : i + n > this.DB ? (this[this.t - 1] |= (a & (1 << this.DB - i) - 1) << i, this[this.t++] = a >> this.DB - i) : this[this.t - 1] |= a << i, (i += n) >= this.DB && (i -= this.DB))
             }
-            this.clamp(), o && rp.ZERO.subTo(this, this)
-        }, rp.prototype.clamp = function() {
+            this.clamp(), o && Wf.ZERO.subTo(this, this)
+        }, Wf.prototype.clamp = function() {
             for (var e = this.s & this.DM; this.t > 0 && this[this.t - 1] == e;) --this.t
-        }, rp.prototype.dlShiftTo = function(e, t) {
+        }, Wf.prototype.dlShiftTo = function(e, t) {
             var n;
             for (n = this.t - 1; n >= 0; --n) t[n + e] = this[n];
             for (n = e - 1; n >= 0; --n) t[n] = 0;
             t.t = this.t + e, t.s = this.s
-        }, rp.prototype.drShiftTo = function(e, t) {
+        }, Wf.prototype.drShiftTo = function(e, t) {
             for (var n = e; n < this.t; ++n) t[n - e] = this[n];
             t.t = Math.max(this.t - e, 0), t.s = this.s
-        }, rp.prototype.lShiftTo = function(e, t) {
+        }, Wf.prototype.lShiftTo = function(e, t) {
             var n, r = e % this.DB,
                 o = this.DB - r,
                 i = (1 << o) - 1,
                 a = Math.floor(e / this.DB),
                 s = this.s << r & this.DM;
             for (n = this.t - 1; n >= 0; --n) t[n + a + 1] = this[n] >> o | s, s = (this[n] & i) << r;
             for (n = a - 1; n >= 0; --n) t[n] = 0;
             t[a] = s, t.t = this.t + a + 1, t.s = this.s, t.clamp()
-        }, rp.prototype.rShiftTo = function(e, t) {
+        }, Wf.prototype.rShiftTo = function(e, t) {
             t.s = this.s;
             var n = Math.floor(e / this.DB);
             if (n >= this.t) t.t = 0;
             else {
                 var r = e % this.DB,
                     o = this.DB - r,
                     i = (1 << r) - 1;
                 t[0] = this[n] >> r;
                 for (var a = n + 1; a < this.t; ++a) t[a - n - 1] |= (this[a] & i) << o, t[a - n] = this[a] >> r;
                 r > 0 && (t[this.t - n - 1] |= (this.s & i) << o), t.t = this.t - n, t.clamp()
             }
-        }, rp.prototype.subTo = function(e, t) {
+        }, Wf.prototype.subTo = function(e, t) {
             for (var n = 0, r = 0, o = Math.min(e.t, this.t); n < o;) r += this[n] - e[n], t[n++] = r & this.DM, r >>= this.DB;
             if (e.t < this.t) {
                 for (r -= e.s; n < this.t;) r += this[n], t[n++] = r & this.DM, r >>= this.DB;
                 r += this.s
             } else {
                 for (r += this.s; n < e.t;) r -= e[n], t[n++] = r & this.DM, r >>= this.DB;
                 r -= e.s
             }
             t.s = r < 0 ? -1 : 0, r < -1 ? t[n++] = this.DV + r : r > 0 && (t[n++] = r), t.t = n, t.clamp()
-        }, rp.prototype.multiplyTo = function(e, t) {
+        }, Wf.prototype.multiplyTo = function(e, t) {
             var n = this.abs(),
                 r = e.abs(),
                 o = n.t;
             for (t.t = o + r.t; --o >= 0;) t[o] = 0;
             for (o = 0; o < r.t; ++o) t[o + n.t] = n.am(0, r[o], t, o, 0, n.t);
-            t.s = 0, t.clamp(), this.s != e.s && rp.ZERO.subTo(t, t)
-        }, rp.prototype.squareTo = function(e) {
+            t.s = 0, t.clamp(), this.s != e.s && Wf.ZERO.subTo(t, t)
+        }, Wf.prototype.squareTo = function(e) {
             for (var t = this.abs(), n = e.t = 2 * t.t; --n >= 0;) e[n] = 0;
             for (n = 0; n < t.t - 1; ++n) {
                 var r = t.am(n, t[n], e, 2 * n, 0, 1);
                 (e[n + t.t] += t.am(n + 1, 2 * t[n], e, 2 * n + 1, r, t.t - n - 1)) >= t.DV && (e[n + t.t] -= t.DV, e[n + t.t + 1] = 1)
             }
             e.t > 0 && (e[e.t - 1] += t.am(n, t[n], e, 2 * n, 0, 1)), e.s = 0, e.clamp()
-        }, rp.prototype.divRemTo = function(e, t, n) {
+        }, Wf.prototype.divRemTo = function(e, t, n) {
             var r = e.abs();
             if (!(r.t <= 0)) {
                 var o = this.abs();
                 if (o.t < r.t) return null != t && t.fromInt(0), void(null != n && this.copyTo(n));
-                null == n && (n = op());
-                var i = op(),
+                null == n && (n = Hf());
+                var i = Hf(),
                     a = this.s,
                     s = e.s,
-                    u = this.DB - fp(r[r.t - 1]);
+                    u = this.DB - ep(r[r.t - 1]);
                 u > 0 ? (r.lShiftTo(u, i), o.lShiftTo(u, n)) : (r.copyTo(i), o.copyTo(n));
                 var l = i.t,
                     c = i[l - 1];
                 if (0 != c) {
                     var d = c * (1 << this.F1) + (l > 1 ? i[l - 2] >> this.F2 : 0),
                         f = this.FV / d,
                         p = (1 << this.F1) / d,
                         h = 1 << this.F2,
                         g = n.t,
                         y = g - l,
-                        m = null == t ? op() : t;
-                    for (i.dlShiftTo(y, m), n.compareTo(m) >= 0 && (n[n.t++] = 1, n.subTo(m, n)), rp.ONE.dlShiftTo(l, m), m.subTo(i, i); i.t < l;) i[i.t++] = 0;
+                        m = null == t ? Hf() : t;
+                    for (i.dlShiftTo(y, m), n.compareTo(m) >= 0 && (n[n.t++] = 1, n.subTo(m, n)), Wf.ONE.dlShiftTo(l, m), m.subTo(i, i); i.t < l;) i[i.t++] = 0;
                     for (; --y >= 0;) {
                         var v = n[--g] == c ? this.DM : Math.floor(n[g] * f + (n[g - 1] + h) * p);
                         if ((n[g] += i.am(0, v, n, y, 0, l)) < v)
                             for (i.dlShiftTo(y, m), n.subTo(m, n); n[g] < --v;) n.subTo(m, n)
                     }
-                    null != t && (n.drShiftTo(l, t), a != s && rp.ZERO.subTo(t, t)), n.t = l, n.clamp(), u > 0 && n.rShiftTo(u, n), a < 0 && rp.ZERO.subTo(n, n)
+                    null != t && (n.drShiftTo(l, t), a != s && Wf.ZERO.subTo(t, t)), n.t = l, n.clamp(), u > 0 && n.rShiftTo(u, n), a < 0 && Wf.ZERO.subTo(n, n)
                 }
             }
-        }, rp.prototype.invDigit = function() {
+        }, Wf.prototype.invDigit = function() {
             if (this.t < 1) return 0;
             var e = this[0];
             if (0 == (1 & e)) return 0;
             var t = 3 & e;
             return (t = (t = (t = (t = t * (2 - (15 & e) * t) & 15) * (2 - (255 & e) * t) & 255) * (2 - ((65535 & e) * t & 65535)) & 65535) * (2 - e * t % this.DV) % this.DV) > 0 ? this.DV - t : -t
-        }, rp.prototype.addTo = function(e, t) {
+        }, Wf.prototype.addTo = function(e, t) {
             for (var n = 0, r = 0, o = Math.min(e.t, this.t); n < o;) r += this[n] + e[n], t[n++] = r & this.DM, r >>= this.DB;
             if (e.t < this.t) {
                 for (r += e.s; n < this.t;) r += this[n], t[n++] = r & this.DM, r >>= this.DB;
                 r += this.s
             } else {
                 for (r += this.s; n < e.t;) r += e[n], t[n++] = r & this.DM, r >>= this.DB;
                 r += e.s
             }
             t.s = r < 0 ? -1 : 0, r > 0 ? t[n++] = r : r < -1 && (t[n++] = this.DV + r), t.t = n, t.clamp()
-        }, rp.prototype.toString = function(e) {
+        }, Wf.prototype.toString = function(e) {
             if (this.s < 0) return "-" + this.negate().toString(e);
             var t;
             if (16 == e) t = 4;
             else if (8 == e) t = 3;
             else if (2 == e) t = 1;
             else if (32 == e) t = 5;
             else {
@@ -65096,236 +62544,236 @@
             }
             var n, r = (1 << t) - 1,
                 o = !1,
                 i = "",
                 a = this.t,
                 s = this.DB - a * this.DB % t;
             if (a-- > 0)
-                for (s < this.DB && (n = this[a] >> s) > 0 && (o = !0, i = lp(n)); a >= 0;) s < t ? (n = (this[a] & (1 << s) - 1) << t - s, n |= this[--a] >> (s += this.DB - t)) : (n = this[a] >> (s -= t) & r, s <= 0 && (s += this.DB, --a)), n > 0 && (o = !0), o && (i += lp(n));
+                for (s < this.DB && (n = this[a] >> s) > 0 && (o = !0, i = Kf(n)); a >= 0;) s < t ? (n = (this[a] & (1 << s) - 1) << t - s, n |= this[--a] >> (s += this.DB - t)) : (n = this[a] >> (s -= t) & r, s <= 0 && (s += this.DB, --a)), n > 0 && (o = !0), o && (i += Kf(n));
             return o ? i : "0"
-        }, rp.prototype.negate = function() {
-            var e = op();
-            return rp.ZERO.subTo(this, e), e
-        }, rp.prototype.abs = function() {
+        }, Wf.prototype.negate = function() {
+            var e = Hf();
+            return Wf.ZERO.subTo(this, e), e
+        }, Wf.prototype.abs = function() {
             return this.s < 0 ? this.negate() : this
-        }, rp.prototype.compareTo = function(e) {
+        }, Wf.prototype.compareTo = function(e) {
             var t = this.s - e.s;
             if (0 != t) return t;
             var n = this.t;
             if (0 != (t = n - e.t)) return this.s < 0 ? -t : t;
             for (; --n >= 0;)
                 if (0 != (t = this[n] - e[n])) return t;
             return 0
-        }, rp.prototype.bitLength = function() {
-            return this.t <= 0 ? 0 : this.DB * (this.t - 1) + fp(this[this.t - 1] ^ this.s & this.DM)
-        }, rp.prototype.mod = function(e) {
-            var t = op();
-            return this.abs().divRemTo(e, null, t), this.s < 0 && t.compareTo(rp.ZERO) > 0 && e.subTo(t, t), t
-        }, rp.prototype.equals = function(e) {
+        }, Wf.prototype.bitLength = function() {
+            return this.t <= 0 ? 0 : this.DB * (this.t - 1) + ep(this[this.t - 1] ^ this.s & this.DM)
+        }, Wf.prototype.mod = function(e) {
+            var t = Hf();
+            return this.abs().divRemTo(e, null, t), this.s < 0 && t.compareTo(Wf.ZERO) > 0 && e.subTo(t, t), t
+        }, Wf.prototype.equals = function(e) {
             return 0 == this.compareTo(e)
-        }, rp.prototype.add = function(e) {
-            var t = op();
+        }, Wf.prototype.add = function(e) {
+            var t = Hf();
             return this.addTo(e, t), t
-        }, rp.prototype.subtract = function(e) {
-            var t = op();
+        }, Wf.prototype.subtract = function(e) {
+            var t = Hf();
             return this.subTo(e, t), t
-        }, rp.prototype.multiply = function(e) {
-            var t = op();
+        }, Wf.prototype.multiply = function(e) {
+            var t = Hf();
             return this.multiplyTo(e, t), t
-        }, rp.prototype.divide = function(e) {
-            var t = op();
+        }, Wf.prototype.divide = function(e) {
+            var t = Hf();
             return this.divRemTo(e, t, null), t
-        }, rp.prototype.modPow = function(e, t, n) {
+        }, Wf.prototype.modPow = function(e, t, n) {
             var r, o = e.bitLength(),
-                i = dp(1),
-                a = new pp(t);
+                i = $f(1),
+                a = new tp(t);
             if (o <= 0) return i;
             r = o < 18 ? 1 : o < 48 ? 3 : o < 144 ? 4 : o < 768 ? 5 : 6;
             var s = new Array,
                 u = 3,
                 l = r - 1,
                 c = (1 << r) - 1;
             if (s[1] = a.convert(this), r > 1) {
-                var d = op();
-                for (a.sqrTo(s[1], d); u <= c;) s[u] = op(), a.mulTo(d, s[u - 2], s[u]), u += 2
+                var d = Hf();
+                for (a.sqrTo(s[1], d); u <= c;) s[u] = Hf(), a.mulTo(d, s[u - 2], s[u]), u += 2
             }
             var f, p, h = e.t - 1,
                 g = !0,
-                y = op();
-            for (o = fp(e[h]) - 1; h >= 0;) {
+                y = Hf();
+            for (o = ep(e[h]) - 1; h >= 0;) {
                 for (o >= l ? f = e[h] >> o - l & c : (f = (e[h] & (1 << o + 1) - 1) << l - o, h > 0 && (f |= e[h - 1] >> this.DB + o - l)), u = r; 0 == (1 & f);) f >>= 1, --u;
                 if ((o -= u) < 0 && (o += this.DB, --h), g) s[f].copyTo(i), g = !1;
                 else {
                     for (; u > 1;) a.sqrTo(i, y), a.sqrTo(y, i), u -= 2;
                     u > 0 ? a.sqrTo(i, y) : (p = i, i = y, y = p), a.mulTo(y, s[f], i)
                 }
                 for (; h >= 0 && 0 == (e[h] & 1 << o);) a.sqrTo(i, y), p = i, i = y, y = p, --o < 0 && (o = this.DB - 1, --h)
             }
             var m = a.revert(i);
             return n(null, m), m
-        }, rp.ZERO = dp(0), rp.ONE = dp(1);
-        var gp = /^[89a-f]/i,
-            yp = function() {
+        }, Wf.ZERO = $f(0), Wf.ONE = $f(1);
+        var rp = /^[89a-f]/i,
+            op = function() {
                 function e(e) {
-                    this.N = new np("FFFFFFFFFFFFFFFFC90FDAA22168C234C4C6628B80DC1CD129024E088A67CC74020BBEA63B139B22514A08798E3404DDEF9519B3CD3A431B302B0A6DF25F14374FE1356D6D51C245E485B576625E7EC6F44C42E9A637ED6B0BFF5CB6F406B7EDEE386BFB5A899FA5AE9F24117C4B1FE649286651ECE45B3DC2007CB8A163BF0598DA48361C55D39A69163FA8FD24CF5F83655D23DCA3AD961C62F356208552BB9ED529077096966D670C354E4ABC9804F1746C08CA18217C32905E462E36CE3BE39E772C180E86039B2783A2EC07A28FB5C55DF06F4C52C9DE2BCBF6955817183995497CEA956AE515D2261898FA051015728E5A8AAAC42DAD33170D04507A33A85521ABDF1CBA64ECFB850458DBEF0A8AEA71575D060C7DB3970F85A6E1E4C7ABF5AE8CDB0933D71E8C94E04A25619DCEE3D2261AD2EE6BF12FFA06D98A0864D87602733EC86A64521F2B18177B200CBBE117577A615D6C770988C0BAD946E208E24FA074E5AB3143DB5BFCE0FD108E4B82D120A93AD2CAFFFFFFFFFFFFFFFF", 16), this.g = new np("2", 16), this.k = new np(this.hexHash("" + this.padHex(this.N) + this.padHex(this.g)), 16), this.smallAValue = this.generateRandomSmallA(), this.getLargeAValue((function() {})), this.infoBits = Kf.lW.from("Caldera Derived Key", "utf8"), this.poolName = e
+                    this.N = new Gf("FFFFFFFFFFFFFFFFC90FDAA22168C234C4C6628B80DC1CD129024E088A67CC74020BBEA63B139B22514A08798E3404DDEF9519B3CD3A431B302B0A6DF25F14374FE1356D6D51C245E485B576625E7EC6F44C42E9A637ED6B0BFF5CB6F406B7EDEE386BFB5A899FA5AE9F24117C4B1FE649286651ECE45B3DC2007CB8A163BF0598DA48361C55D39A69163FA8FD24CF5F83655D23DCA3AD961C62F356208552BB9ED529077096966D670C354E4ABC9804F1746C08CA18217C32905E462E36CE3BE39E772C180E86039B2783A2EC07A28FB5C55DF06F4C52C9DE2BCBF6955817183995497CEA956AE515D2261898FA051015728E5A8AAAC42DAD33170D04507A33A85521ABDF1CBA64ECFB850458DBEF0A8AEA71575D060C7DB3970F85A6E1E4C7ABF5AE8CDB0933D71E8C94E04A25619DCEE3D2261AD2EE6BF12FFA06D98A0864D87602733EC86A64521F2B18177B200CBBE117577A615D6C770988C0BAD946E208E24FA074E5AB3143DB5BFCE0FD108E4B82D120A93AD2CAFFFFFFFFFFFFFFFF", 16), this.g = new Gf("2", 16), this.k = new Gf(this.hexHash("" + this.padHex(this.N) + this.padHex(this.g)), 16), this.smallAValue = this.generateRandomSmallA(), this.getLargeAValue((function() {})), this.infoBits = Rf.lW.from("Caldera Derived Key", "utf8"), this.poolName = e
                 }
                 var t = e.prototype;
                 return t.getSmallAValue = function() {
                     return this.smallAValue
                 }, t.getLargeAValue = function(e) {
                     var t = this;
                     this.largeAValue ? e(null, this.largeAValue) : this.calculateA(this.smallAValue, (function(n, r) {
                         n && e(n, null), t.largeAValue = r, e(null, t.largeAValue)
                     }))
                 }, t.generateRandomSmallA = function() {
-                    var e = hp(128).toString("hex");
-                    return new np(e, 16)
+                    var e = np(128).toString("hex");
+                    return new Gf(e, 16)
                 }, t.generateRandomString = function() {
-                    return hp(40).toString("base64")
+                    return np(40).toString("base64")
                 }, t.getRandomPassword = function() {
                     return this.randomPassword
                 }, t.getSaltDevices = function() {
                     return this.SaltToHashDevices
                 }, t.getVerifierDevices = function() {
                     return this.verifierDevices
                 }, t.generateHashDevice = function(e, t, n) {
                     var r = this;
                     this.randomPassword = this.generateRandomString();
                     var o = "" + e + t + ":" + this.randomPassword,
                         i = this.hash(o),
-                        a = hp(16).toString("hex");
-                    this.SaltToHashDevices = this.padHex(new np(a, 16)), this.g.modPow(new np(this.hexHash(this.SaltToHashDevices + i), 16), this.N, (function(e, t) {
+                        a = np(16).toString("hex");
+                    this.SaltToHashDevices = this.padHex(new Gf(a, 16)), this.g.modPow(new Gf(this.hexHash(this.SaltToHashDevices + i), 16), this.N, (function(e, t) {
                         e && n(e, null), r.verifierDevices = r.padHex(t), n(null, null)
                     }))
                 }, t.calculateA = function(e, t) {
                     var n = this;
                     this.g.modPow(e, this.N, (function(e, r) {
-                        e && t(e, null), r.mod(n.N).equals(np.ZERO) && t(new Error("Illegal paramater. A mod N cannot be 0."), null), t(null, r)
+                        e && t(e, null), r.mod(n.N).equals(Gf.ZERO) && t(new Error("Illegal paramater. A mod N cannot be 0."), null), t(null, r)
                     }))
                 }, t.calculateU = function(e, t) {
-                    return this.UHexHash = this.hexHash(this.padHex(e) + this.padHex(t)), new np(this.UHexHash, 16)
+                    return this.UHexHash = this.hexHash(this.padHex(e) + this.padHex(t)), new Gf(this.UHexHash, 16)
                 }, t.hash = function(e) {
-                    var t = new tp.Sha256;
+                    var t = new Qf.Sha256;
                     t.update(e);
                     var n = t.digestSync(),
-                        r = Kf.lW.from(n).toString("hex");
+                        r = Rf.lW.from(n).toString("hex");
                     return new Array(64 - r.length).join("0") + r
                 }, t.hexHash = function(e) {
-                    return this.hash(Kf.lW.from(e, "hex"))
+                    return this.hash(Rf.lW.from(e, "hex"))
                 }, t.computehkdf = function(e, t) {
-                    var n = Kf.lW.concat([this.infoBits, Kf.lW.from(String.fromCharCode(1), "utf8")]),
-                        r = new tp.Sha256(t);
+                    var n = Rf.lW.concat([this.infoBits, Rf.lW.from(String.fromCharCode(1), "utf8")]),
+                        r = new Qf.Sha256(t);
                     r.update(e);
                     var o = r.digestSync(),
-                        i = new tp.Sha256(o);
+                        i = new Qf.Sha256(o);
                     return i.update(n), i.digestSync().slice(0, 16)
                 }, t.getPasswordAuthenticationKey = function(e, t, n, r, o) {
                     var i = this;
-                    if (n.mod(this.N).equals(np.ZERO)) throw new Error("B cannot be zero.");
-                    if (this.UValue = this.calculateU(this.largeAValue, n), this.UValue.equals(np.ZERO)) throw new Error("U cannot be zero.");
+                    if (n.mod(this.N).equals(Gf.ZERO)) throw new Error("B cannot be zero.");
+                    if (this.UValue = this.calculateU(this.largeAValue, n), this.UValue.equals(Gf.ZERO)) throw new Error("U cannot be zero.");
                     var a = "" + this.poolName + e + ":" + t,
                         s = this.hash(a),
-                        u = new np(this.hexHash(this.padHex(r) + s), 16);
+                        u = new Gf(this.hexHash(this.padHex(r) + s), 16);
                     this.calculateS(u, n, (function(e, t) {
                         e && o(e, null);
-                        var n = i.computehkdf(Kf.lW.from(i.padHex(t), "hex"), Kf.lW.from(i.padHex(i.UValue), "hex"));
+                        var n = i.computehkdf(Rf.lW.from(i.padHex(t), "hex"), Rf.lW.from(i.padHex(i.UValue), "hex"));
                         o(null, n)
                     }))
                 }, t.calculateS = function(e, t, n) {
                     var r = this;
                     this.g.modPow(e, this.N, (function(o, i) {
                         o && n(o, null), t.subtract(r.k.multiply(i)).modPow(r.smallAValue.add(r.UValue.multiply(e)), r.N, (function(e, t) {
                             e && n(e, null), n(null, t.mod(r.N))
                         }))
                     }))
                 }, t.getNewPasswordRequiredChallengeUserAttributePrefix = function() {
                     return "userAttributes."
                 }, t.padHex = function(e) {
-                    if (!(e instanceof np)) throw new Error("Not a BigInteger");
-                    var t = e.compareTo(np.ZERO) < 0,
+                    if (!(e instanceof Gf)) throw new Error("Not a BigInteger");
+                    var t = e.compareTo(Gf.ZERO) < 0,
                         n = e.abs().toString(16);
-                    if (n = n.length % 2 !== 0 ? "0" + n : n, n = gp.test(n) ? "00" + n : n, t) {
+                    if (n = n.length % 2 !== 0 ? "0" + n : n, n = rp.test(n) ? "00" + n : n, t) {
                         var r = n.split("").map((function(e) {
                             var t = 15 & ~parseInt(e, 16);
                             return "0123456789ABCDEF".charAt(t)
                         })).join("");
-                        (n = new np(r, 16).add(np.ONE).toString(16)).toUpperCase().startsWith("FF8") && (n = n.substring(2))
+                        (n = new Gf(r, 16).add(Gf.ONE).toString(16)).toUpperCase().startsWith("FF8") && (n = n.substring(2))
                     }
                     return n
                 }, e
             }(),
-            mp = function() {
+            ip = function() {
                 function e(e) {
                     this.jwtToken = e || "", this.payload = this.decodePayload()
                 }
                 var t = e.prototype;
                 return t.getJwtToken = function() {
                     return this.jwtToken
                 }, t.getExpiration = function() {
                     return this.payload.exp
                 }, t.getIssuedAt = function() {
                     return this.payload.iat
                 }, t.decodePayload = function() {
                     var e = this.jwtToken.split(".")[1];
                     try {
-                        return JSON.parse(Kf.lW.from(e, "base64").toString("utf8"))
+                        return JSON.parse(Rf.lW.from(e, "base64").toString("utf8"))
                     } catch (t) {
                         return {}
                     }
                 }, e
             }();
 
-        function vp(e, t) {
-            return vp = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+        function ap(e, t) {
+            return ap = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                 return e.__proto__ = t, e
-            }, vp(e, t)
+            }, ap(e, t)
         }
-        var Mp = function(e) {
+        var sp = function(e) {
             var t, n;
 
             function r(t) {
                 var n = (void 0 === t ? {} : t).AccessToken;
                 return e.call(this, n || "") || this
             }
-            return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, vp(t, n), r
-        }(mp);
+            return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, ap(t, n), r
+        }(ip);
 
-        function bp(e, t) {
-            return bp = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+        function up(e, t) {
+            return up = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                 return e.__proto__ = t, e
-            }, bp(e, t)
+            }, up(e, t)
         }
-        var wp = function(e) {
+        var lp = function(e) {
                 var t, n;
 
                 function r(t) {
                     var n = (void 0 === t ? {} : t).IdToken;
                     return e.call(this, n || "") || this
                 }
-                return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, bp(t, n), r
-            }(mp),
-            jp = function() {
+                return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, up(t, n), r
+            }(ip),
+            cp = function() {
                 function e(e) {
                     var t = (void 0 === e ? {} : e).RefreshToken;
                     this.token = t || ""
                 }
                 return e.prototype.getToken = function() {
                     return this.token
                 }, e
             }(),
-            xp = {
+            dp = {
                 userAgent: "aws-amplify/5.0.4 js",
                 product: "",
                 navigator: null,
                 isReactNative: !1
             };
         if ("undefined" !== typeof navigator && navigator.product)
-            if (xp.product = navigator.product || "", xp.navigator = navigator || null, "ReactNative" === navigator.product) xp.userAgent = "aws-amplify/5.0.4 react-native", xp.isReactNative = !0;
-            else xp.userAgent = "aws-amplify/5.0.4 js", xp.isReactNative = !1;
-        var Np = function() {
+            if (dp.product = navigator.product || "", dp.navigator = navigator || null, "ReactNative" === navigator.product) dp.userAgent = "aws-amplify/5.0.4 react-native", dp.isReactNative = !0;
+            else dp.userAgent = "aws-amplify/5.0.4 js", dp.isReactNative = !1;
+        var fp = function() {
                 function e(e) {
                     var t = void 0 === e ? {} : e,
                         n = t.IdToken,
                         r = t.RefreshToken,
                         o = t.AccessToken,
                         i = t.ClockDrift;
                     if (null == o || null == n) throw new Error("Id token and Access Token must be present.");
@@ -65343,32 +62791,32 @@
                 }, t.calculateClockDrift = function() {
                     return Math.floor(new Date / 1e3) - Math.min(this.accessToken.getIssuedAt(), this.idToken.getIssuedAt())
                 }, t.isValid = function() {
                     var e = Math.floor(new Date / 1e3) - this.clockDrift;
                     return e < this.accessToken.getExpiration() && e < this.idToken.getExpiration()
                 }, e
             }(),
-            Ip = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
-            Dp = ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"],
-            Sp = function() {
+            pp = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
+            hp = ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"],
+            gp = function() {
                 function e() {}
                 return e.prototype.getNowString = function() {
                     var e = new Date,
-                        t = Dp[e.getUTCDay()],
-                        n = Ip[e.getUTCMonth()],
+                        t = hp[e.getUTCDay()],
+                        n = pp[e.getUTCMonth()],
                         r = e.getUTCDate(),
                         o = e.getUTCHours();
                     o < 10 && (o = "0" + o);
                     var i = e.getUTCMinutes();
                     i < 10 && (i = "0" + i);
                     var a = e.getUTCSeconds();
                     return a < 10 && (a = "0" + a), t + " " + n + " " + r + " " + o + ":" + i + ":" + a + " UTC " + e.getUTCFullYear()
                 }, e
             }(),
-            Lp = function() {
+            yp = function() {
                 function e(e) {
                     var t = void 0 === e ? {} : e,
                         n = t.Name,
                         r = t.Value;
                     this.Name = n || "", this.Value = r || ""
                 }
                 var t = e.prototype;
@@ -65385,44 +62833,44 @@
                 }, t.toJSON = function() {
                     return {
                         Name: this.Name,
                         Value: this.Value
                     }
                 }, e
             }(),
-            kp = {},
-            Cp = function() {
+            mp = {},
+            vp = function() {
                 function e() {}
                 return e.setItem = function(e, t) {
-                    return kp[e] = t, kp[e]
+                    return mp[e] = t, mp[e]
                 }, e.getItem = function(e) {
-                    return Object.prototype.hasOwnProperty.call(kp, e) ? kp[e] : void 0
+                    return Object.prototype.hasOwnProperty.call(mp, e) ? mp[e] : void 0
                 }, e.removeItem = function(e) {
-                    return delete kp[e]
+                    return delete mp[e]
                 }, e.clear = function() {
-                    return kp = {}
+                    return mp = {}
                 }, e
             }(),
-            Ep = function() {
+            Mp = function() {
                 function e() {
                     try {
                         this.storageWindow = window.localStorage, this.storageWindow.setItem("aws.cognito.test-ls", 1), this.storageWindow.removeItem("aws.cognito.test-ls")
                     } catch (e) {
-                        this.storageWindow = Cp
+                        this.storageWindow = vp
                     }
                 }
                 return e.prototype.getStorage = function() {
                     return this.storageWindow
                 }, e
             }(),
-            _p = "undefined" !== typeof navigator ? xp.isReactNative ? "react-native" : navigator.userAgent : "nodejs",
-            Tp = function() {
+            bp = "undefined" !== typeof navigator ? dp.isReactNative ? "react-native" : navigator.userAgent : "nodejs",
+            wp = function() {
                 function e(e) {
                     if (null == e || null == e.Username || null == e.Pool) throw new Error("Username and Pool information are required.");
-                    this.username = e.Username || "", this.pool = e.Pool, this.Session = null, this.client = e.Pool.client, this.signInUserSession = null, this.authenticationFlowType = "USER_SRP_AUTH", this.storage = e.Storage || (new Ep).getStorage(), this.keyPrefix = "CognitoIdentityServiceProvider." + this.pool.getClientId(), this.userDataKey = this.keyPrefix + "." + this.username + ".userData"
+                    this.username = e.Username || "", this.pool = e.Pool, this.Session = null, this.client = e.Pool.client, this.signInUserSession = null, this.authenticationFlowType = "USER_SRP_AUTH", this.storage = e.Storage || (new Mp).getStorage(), this.keyPrefix = "CognitoIdentityServiceProvider." + this.pool.getClientId(), this.userDataKey = this.keyPrefix + "." + this.username + ".userData"
                 }
                 var t = e.prototype;
                 return t.setSignInUserSession = function(e) {
                     this.clearCachedUserData(), this.signInUserSession = e, this.cacheTokens()
                 }, t.getSignInUserSession = function() {
                     return this.signInUserSession
                 }, t.getUsername = function() {
@@ -65448,37 +62896,37 @@
                             i = r.ChallengeParameters;
                         return "CUSTOM_CHALLENGE" === o ? (n.Session = r.Session, t.customChallenge(i)) : (n.signInUserSession = n.getCognitoUserSession(r.AuthenticationResult), n.cacheTokens(), t.onSuccess(n.signInUserSession))
                     }))
                 }, t.authenticateUser = function(e, t) {
                     return "USER_PASSWORD_AUTH" === this.authenticationFlowType ? this.authenticateUserPlainUsernamePassword(e, t) : "USER_SRP_AUTH" === this.authenticationFlowType || "CUSTOM_AUTH" === this.authenticationFlowType ? this.authenticateUserDefaultAuth(e, t) : t.onFailure(new Error("Authentication flow type is invalid."))
                 }, t.authenticateUserDefaultAuth = function(e, t) {
                     var n, r, o = this,
-                        i = new yp(this.pool.getUserPoolName()),
-                        a = new Sp,
+                        i = new op(this.pool.getUserPoolName()),
+                        a = new gp,
                         s = {};
                     null != this.deviceKey && (s.DEVICE_KEY = this.deviceKey), s.USERNAME = this.username, i.getLargeAValue((function(u, l) {
                         u && t.onFailure(u), s.SRP_A = l.toString(16), "CUSTOM_AUTH" === o.authenticationFlowType && (s.CHALLENGE_NAME = "SRP_A");
                         var c = 0 !== Object.keys(e.getValidationData()).length ? e.getValidationData() : e.getClientMetadata(),
                             d = {
                                 AuthFlow: o.authenticationFlowType,
                                 ClientId: o.pool.getClientId(),
                                 AuthParameters: s,
                                 ClientMetadata: c
                             };
                         o.getUserContextData(o.username) && (d.UserContextData = o.getUserContextData(o.username)), o.client.request("InitiateAuth", d, (function(s, u) {
                             if (s) return t.onFailure(s);
                             var l = u.ChallengeParameters;
-                            o.username = l.USER_ID_FOR_SRP, o.userDataKey = o.keyPrefix + "." + o.username + ".userData", n = new np(l.SRP_B, 16), r = new np(l.SALT, 16), o.getCachedDeviceKeyAndPassword(), i.getPasswordAuthenticationKey(o.username, e.getPassword(), n, r, (function(e, n) {
+                            o.username = l.USER_ID_FOR_SRP, o.userDataKey = o.keyPrefix + "." + o.username + ".userData", n = new Gf(l.SRP_B, 16), r = new Gf(l.SALT, 16), o.getCachedDeviceKeyAndPassword(), i.getPasswordAuthenticationKey(o.username, e.getPassword(), n, r, (function(e, n) {
                                 e && t.onFailure(e);
                                 var r = a.getNowString(),
-                                    s = Kf.lW.concat([Kf.lW.from(o.pool.getUserPoolName(), "utf8"), Kf.lW.from(o.username, "utf8"), Kf.lW.from(l.SECRET_BLOCK, "base64"), Kf.lW.from(r, "utf8")]),
-                                    d = new tp.Sha256(n);
+                                    s = Rf.lW.concat([Rf.lW.from(o.pool.getUserPoolName(), "utf8"), Rf.lW.from(o.username, "utf8"), Rf.lW.from(l.SECRET_BLOCK, "base64"), Rf.lW.from(r, "utf8")]),
+                                    d = new Qf.Sha256(n);
                                 d.update(s);
                                 var f = d.digestSync(),
-                                    p = Kf.lW.from(f).toString("base64"),
+                                    p = Rf.lW.from(f).toString("base64"),
                                     h = {};
                                 h.USERNAME = o.username, h.PASSWORD_CLAIM_SECRET_BLOCK = l.SECRET_BLOCK, h.TIMESTAMP = r, h.PASSWORD_CLAIM_SIGNATURE = p, null != o.deviceKey && (h.DEVICE_KEY = o.deviceKey);
                                 var g = {
                                     ChallengeName: "PASSWORD_VERIFIER",
                                     ClientId: o.pool.getClientId(),
                                     ChallengeResponses: h,
                                     Session: u.Session,
@@ -65495,15 +62943,15 @@
                             }))
                         }))
                     }))
                 }, t.authenticateUserPlainUsernamePassword = function(e, t) {
                     var n = this,
                         r = {};
                     if (r.USERNAME = this.username, r.PASSWORD = e.getPassword(), r.PASSWORD) {
-                        var o = new yp(this.pool.getUserPoolName());
+                        var o = new op(this.pool.getUserPoolName());
                         this.getCachedDeviceKeyAndPassword(), null != this.deviceKey && (r.DEVICE_KEY = this.deviceKey);
                         var i = 0 !== Object.keys(e.getValidationData()).length ? e.getValidationData() : e.getClientMetadata(),
                             a = {
                                 AuthFlow: "USER_PASSWORD_AUTH",
                                 ClientId: this.pool.getClientId(),
                                 AuthParameters: r,
                                 ClientMetadata: i
@@ -65534,30 +62982,30 @@
                     if ("DEVICE_SRP_AUTH" === o) return this.Session = e.Session, void this.getDeviceResponse(n);
                     this.signInUserSession = this.getCognitoUserSession(e.AuthenticationResult), this.challengeName = o, this.cacheTokens();
                     var d = e.AuthenticationResult.NewDeviceMetadata;
                     if (null == d) return n.onSuccess(this.signInUserSession);
                     t.generateHashDevice(e.AuthenticationResult.NewDeviceMetadata.DeviceGroupKey, e.AuthenticationResult.NewDeviceMetadata.DeviceKey, (function(o) {
                         if (o) return n.onFailure(o);
                         var i = {
-                            Salt: Kf.lW.from(t.getSaltDevices(), "hex").toString("base64"),
-                            PasswordVerifier: Kf.lW.from(t.getVerifierDevices(), "hex").toString("base64")
+                            Salt: Rf.lW.from(t.getSaltDevices(), "hex").toString("base64"),
+                            PasswordVerifier: Rf.lW.from(t.getVerifierDevices(), "hex").toString("base64")
                         };
                         r.verifierDevices = i.PasswordVerifier, r.deviceGroupKey = d.DeviceGroupKey, r.randomPassword = t.getRandomPassword(), r.client.request("ConfirmDevice", {
                             DeviceKey: d.DeviceKey,
                             AccessToken: r.signInUserSession.getAccessToken().getJwtToken(),
                             DeviceSecretVerifierConfig: i,
-                            DeviceName: _p
+                            DeviceName: bp
                         }, (function(t, o) {
                             return t ? n.onFailure(t) : (r.deviceKey = e.AuthenticationResult.NewDeviceMetadata.DeviceKey, r.cacheDeviceKeyAndPassword(), !0 === o.UserConfirmationNecessary ? n.onSuccess(r.signInUserSession, o.UserConfirmationNecessary) : n.onSuccess(r.signInUserSession))
                         }))
                     }))
                 }, t.completeNewPasswordChallenge = function(e, t, n, r) {
                     var o = this;
                     if (!e) return n.onFailure(new Error("New password is required."));
-                    var i = new yp(this.pool.getUserPoolName()),
+                    var i = new op(this.pool.getUserPoolName()),
                         a = i.getNewPasswordRequiredChallengeUserAttributePrefix(),
                         s = {};
                     t && Object.keys(t).forEach((function(e) {
                         s[a + e] = t[e]
                     })), s.NEW_PASSWORD = e, s.USERNAME = this.username;
                     var u = {
                         ChallengeName: "NEW_PASSWORD_REQUIRED",
@@ -65567,39 +63015,39 @@
                         ClientMetadata: r
                     };
                     this.getUserContextData() && (u.UserContextData = this.getUserContextData()), this.client.request("RespondToAuthChallenge", u, (function(e, t) {
                         return e ? n.onFailure(e) : o.authenticateUserInternal(t, i, n)
                     }))
                 }, t.getDeviceResponse = function(e, t) {
                     var n = this,
-                        r = new yp(this.deviceGroupKey),
-                        o = new Sp,
+                        r = new op(this.deviceGroupKey),
+                        o = new gp,
                         i = {};
                     i.USERNAME = this.username, i.DEVICE_KEY = this.deviceKey, r.getLargeAValue((function(a, s) {
                         a && e.onFailure(a), i.SRP_A = s.toString(16);
                         var u = {
                             ChallengeName: "DEVICE_SRP_AUTH",
                             ClientId: n.pool.getClientId(),
                             ChallengeResponses: i,
                             ClientMetadata: t,
                             Session: n.Session
                         };
                         n.getUserContextData() && (u.UserContextData = n.getUserContextData()), n.client.request("RespondToAuthChallenge", u, (function(t, i) {
                             if (t) return e.onFailure(t);
                             var a = i.ChallengeParameters,
-                                s = new np(a.SRP_B, 16),
-                                u = new np(a.SALT, 16);
+                                s = new Gf(a.SRP_B, 16),
+                                u = new Gf(a.SALT, 16);
                             r.getPasswordAuthenticationKey(n.deviceKey, n.randomPassword, s, u, (function(t, r) {
                                 if (t) return e.onFailure(t);
                                 var s = o.getNowString(),
-                                    u = Kf.lW.concat([Kf.lW.from(n.deviceGroupKey, "utf8"), Kf.lW.from(n.deviceKey, "utf8"), Kf.lW.from(a.SECRET_BLOCK, "base64"), Kf.lW.from(s, "utf8")]),
-                                    l = new tp.Sha256(r);
+                                    u = Rf.lW.concat([Rf.lW.from(n.deviceGroupKey, "utf8"), Rf.lW.from(n.deviceKey, "utf8"), Rf.lW.from(a.SECRET_BLOCK, "base64"), Rf.lW.from(s, "utf8")]),
+                                    l = new Qf.Sha256(r);
                                 l.update(u);
                                 var c = l.digestSync(),
-                                    d = Kf.lW.from(c).toString("base64"),
+                                    d = Rf.lW.from(c).toString("base64"),
                                     f = {};
                                 f.USERNAME = n.username, f.PASSWORD_CLAIM_SECRET_BLOCK = a.SECRET_BLOCK, f.TIMESTAMP = s, f.PASSWORD_CLAIM_SIGNATURE = d, f.DEVICE_KEY = n.deviceKey;
                                 var p = {
                                     ChallengeName: "DEVICE_PASSWORD_VERIFIER",
                                     ClientId: n.pool.getClientId(),
                                     ChallengeResponses: f,
                                     Session: i.Session
@@ -65621,15 +63069,15 @@
                     this.getUserContextData() && (o.UserContextData = this.getUserContextData()), this.client.request("ConfirmSignUp", o, (function(e) {
                         return e ? n(e, null) : n(null, "SUCCESS")
                     }))
                 }, t.sendCustomChallengeAnswer = function(e, t, n) {
                     var r = this,
                         o = {};
                     o.USERNAME = this.username, o.ANSWER = e;
-                    var i = new yp(this.pool.getUserPoolName());
+                    var i = new op(this.pool.getUserPoolName());
                     this.getCachedDeviceKeyAndPassword(), null != this.deviceKey && (o.DEVICE_KEY = this.deviceKey);
                     var a = {
                         ChallengeName: "CUSTOM_CHALLENGE",
                         ChallengeResponses: o,
                         ClientId: this.pool.getClientId(),
                         Session: this.Session,
                         ClientMetadata: n
@@ -65650,26 +63098,26 @@
                         Session: this.Session,
                         ClientMetadata: r
                     };
                     this.getUserContextData() && (s.UserContextData = this.getUserContextData()), this.client.request("RespondToAuthChallenge", s, (function(e, n) {
                         if (e) return t.onFailure(e);
                         if ("DEVICE_SRP_AUTH" !== n.ChallengeName) {
                             if (o.signInUserSession = o.getCognitoUserSession(n.AuthenticationResult), o.cacheTokens(), null == n.AuthenticationResult.NewDeviceMetadata) return t.onSuccess(o.signInUserSession);
-                            var r = new yp(o.pool.getUserPoolName());
+                            var r = new op(o.pool.getUserPoolName());
                             r.generateHashDevice(n.AuthenticationResult.NewDeviceMetadata.DeviceGroupKey, n.AuthenticationResult.NewDeviceMetadata.DeviceKey, (function(e) {
                                 if (e) return t.onFailure(e);
                                 var i = {
-                                    Salt: Kf.lW.from(r.getSaltDevices(), "hex").toString("base64"),
-                                    PasswordVerifier: Kf.lW.from(r.getVerifierDevices(), "hex").toString("base64")
+                                    Salt: Rf.lW.from(r.getSaltDevices(), "hex").toString("base64"),
+                                    PasswordVerifier: Rf.lW.from(r.getVerifierDevices(), "hex").toString("base64")
                                 };
                                 o.verifierDevices = i.PasswordVerifier, o.deviceGroupKey = n.AuthenticationResult.NewDeviceMetadata.DeviceGroupKey, o.randomPassword = r.getRandomPassword(), o.client.request("ConfirmDevice", {
                                     DeviceKey: n.AuthenticationResult.NewDeviceMetadata.DeviceKey,
                                     AccessToken: o.signInUserSession.getAccessToken().getJwtToken(),
                                     DeviceSecretVerifierConfig: i,
-                                    DeviceName: _p
+                                    DeviceName: bp
                                 }, (function(e, r) {
                                     return e ? t.onFailure(e) : (o.deviceKey = n.AuthenticationResult.NewDeviceMetadata.DeviceKey, o.cacheDeviceKeyAndPassword(), !0 === r.UserConfirmationNecessary ? t.onSuccess(o.signInUserSession, r.UserConfirmationNecessary) : t.onSuccess(o.signInUserSession))
                                 }))
                             }))
                         } else o.getDeviceResponse(t)
                     }))
                 }, t.changePassword = function(e, t, n, r) {
@@ -65741,15 +63189,15 @@
                     }, (function(t, n) {
                         if (t) return e(t, null);
                         for (var r = [], o = 0; o < n.UserAttributes.length; o++) {
                             var i = {
                                     Name: n.UserAttributes[o].Name,
                                     Value: n.UserAttributes[o].Value
                                 },
-                                a = new Lp(i);
+                                a = new yp(i);
                             r.push(a)
                         }
                         return e(null, r)
                     }))
                 }, t.getMFAOptions = function(e) {
                     if (null == this.signInUserSession || !this.signInUserSession.isValid()) return e(new Error("User is not authenticated"), null);
                     this.client.request("GetUser", {
@@ -65823,25 +63271,25 @@
                     if (null != this.signInUserSession && this.signInUserSession.isValid()) return e(null, this.signInUserSession);
                     var n = "CognitoIdentityServiceProvider." + this.pool.getClientId() + "." + this.username,
                         r = n + ".idToken",
                         o = n + ".accessToken",
                         i = n + ".refreshToken",
                         a = n + ".clockDrift";
                     if (this.storage.getItem(r)) {
-                        var s = new wp({
+                        var s = new lp({
                                 IdToken: this.storage.getItem(r)
                             }),
-                            u = new Mp({
+                            u = new sp({
                                 AccessToken: this.storage.getItem(o)
                             }),
-                            l = new jp({
+                            l = new cp({
                                 RefreshToken: this.storage.getItem(i)
                             }),
                             c = parseInt(this.storage.getItem(a), 0) || 0,
-                            d = new Np({
+                            d = new fp({
                                 IdToken: s,
                                 AccessToken: u,
                                 RefreshToken: l,
                                 ClockDrift: c
                             });
                         if (d.isValid()) return this.signInUserSession = d, e(null, this.signInUserSession);
                         if (!l.getToken()) return e(new Error("Cannot retrieve a new session. Please authenticate."), null);
@@ -65909,18 +63357,18 @@
                         t = e + "." + this.username + ".idToken",
                         n = e + "." + this.username + ".accessToken",
                         r = e + "." + this.username + ".refreshToken",
                         o = e + ".LastAuthUser",
                         i = e + "." + this.username + ".clockDrift";
                     this.storage.removeItem(t), this.storage.removeItem(n), this.storage.removeItem(r), this.storage.removeItem(o), this.storage.removeItem(i)
                 }, t.getCognitoUserSession = function(e) {
-                    var t = new wp(e),
-                        n = new Mp(e),
-                        r = new jp(e);
-                    return new Np({
+                    var t = new lp(e),
+                        n = new sp(e),
+                        r = new cp(e);
+                    return new fp({
                         IdToken: t,
                         AccessToken: n,
                         RefreshToken: r
                     })
                 }, t.forgotPassword = function(e, t) {
                     var n = {
                         ClientId: this.pool.getClientId(),
@@ -66107,106 +63555,106 @@
                             return e ? n.onFailure(e) : (r.signInUserSession = r.getCognitoUserSession(t.AuthenticationResult), r.cacheTokens(), n.onSuccess(r.signInUserSession))
                         }))
                     }))
                 }, e
             }();
         __webpack_require__(8117);
 
-        function Ap() {}
-        Ap.prototype.userAgent = xp.userAgent;
-        var Op = Ap;
+        function jp() {}
+        jp.prototype.userAgent = dp.userAgent;
+        var xp = jp;
 
-        function zp(e, t) {
-            e.prototype = Object.create(t.prototype), e.prototype.constructor = e, Bp(e, t)
+        function Np(e, t) {
+            e.prototype = Object.create(t.prototype), e.prototype.constructor = e, Lp(e, t)
         }
 
-        function Up(e) {
+        function Ip(e) {
             var t = "function" === typeof Map ? new Map : void 0;
-            return Up = function(e) {
+            return Ip = function(e) {
                 if (null === e || (n = e, -1 === Function.toString.call(n).indexOf("[native code]"))) return e;
                 var n;
                 if ("function" !== typeof e) throw new TypeError("Super expression must either be null or a function");
                 if ("undefined" !== typeof t) {
                     if (t.has(e)) return t.get(e);
                     t.set(e, r)
                 }
 
                 function r() {
-                    return Pp(e, arguments, Fp(this).constructor)
+                    return Dp(e, arguments, kp(this).constructor)
                 }
                 return r.prototype = Object.create(e.prototype, {
                     constructor: {
                         value: r,
                         enumerable: !1,
                         writable: !0,
                         configurable: !0
                     }
-                }), Bp(r, e)
-            }, Up(e)
+                }), Lp(r, e)
+            }, Ip(e)
         }
 
-        function Pp(e, t, n) {
-            return Pp = Rp() ? Reflect.construct.bind() : function(e, t, n) {
+        function Dp(e, t, n) {
+            return Dp = Sp() ? Reflect.construct.bind() : function(e, t, n) {
                 var r = [null];
                 r.push.apply(r, t);
                 var o = new(Function.bind.apply(e, r));
-                return n && Bp(o, n.prototype), o
-            }, Pp.apply(null, arguments)
+                return n && Lp(o, n.prototype), o
+            }, Dp.apply(null, arguments)
         }
 
-        function Rp() {
+        function Sp() {
             if ("undefined" === typeof Reflect || !Reflect.construct) return !1;
             if (Reflect.construct.sham) return !1;
             if ("function" === typeof Proxy) return !0;
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
                 return !1
             }
         }
 
-        function Bp(e, t) {
-            return Bp = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+        function Lp(e, t) {
+            return Lp = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                 return e.__proto__ = t, e
-            }, Bp(e, t)
+            }, Lp(e, t)
         }
 
-        function Fp(e) {
-            return Fp = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
+        function kp(e) {
+            return kp = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
                 return e.__proto__ || Object.getPrototypeOf(e)
-            }, Fp(e)
+            }, kp(e)
         }
-        var Yp = function(e) {
+        var Cp = function(e) {
                 function t(t, n, r, o) {
                     var i;
                     return (i = e.call(this, t) || this).code = n, i.name = r, i.statusCode = o, i
                 }
-                return zp(t, e), t
-            }(Up(Error)),
-            Qp = function() {
+                return Np(t, e), t
+            }(Ip(Error)),
+            Ep = function() {
                 function e(e, t, n) {
                     this.endpoint = t || "https://cognito-idp." + e + ".amazonaws.com/";
                     var r = (n || {}).credentials;
                     this.fetchOptions = r ? {
                         credentials: r
                     } : {}
                 }
                 var t = e.prototype;
                 return t.promisifyRequest = function(e, t) {
                     var n = this;
                     return new Promise((function(r, o) {
                         n.request(e, t, (function(e, t) {
-                            e ? o(new Yp(e.message, e.code, e.name, e.statusCode)) : r(t)
+                            e ? o(new Cp(e.message, e.code, e.name, e.statusCode)) : r(t)
                         }))
                     }))
                 }, t.requestWithRetry = function(e, t, n) {
                     var r = this;
                     (function(e, t, n) {
-                        void 0 === n && (n = Hp);
-                        return Wp(e, t, function(e) {
+                        void 0 === n && (n = Ap);
+                        return Tp(e, t, function(e) {
                             var t = 100,
                                 n = 100;
                             return function(r) {
                                 var o = Math.pow(2, r) * t + n * Math.random();
                                 return !(o > e) && o
                             }
                         }(n))
@@ -66221,15 +63669,15 @@
                     })).catch((function(e) {
                         return n(e)
                     }))
                 }, t.request = function(e, t, n) {
                     var r, o = {
                             "Content-Type": "application/x-amz-json-1.1",
                             "X-Amz-Target": "AWSCognitoIdentityProviderService." + e,
-                            "X-Amz-User-Agent": Op.prototype.userAgent,
+                            "X-Amz-User-Agent": xp.prototype.userAgent,
                             "Cache-Control": "no-store"
                         },
                         i = Object.assign({}, this.fetchOptions, {
                             headers: o,
                             method: "POST",
                             mode: "cors",
                             body: JSON.stringify(t)
@@ -66257,43 +63705,43 @@
                         } catch (i) {
                             return n(e)
                         } else e instanceof Error && "Network error" === e.message && (e.code = "NetworkError");
                         return n(e)
                     }))
                 }, e
             }(),
-            Gp = function() {};
+            _p = function() {};
         Error;
 
-        function Wp(e, t, n, r) {
+        function Tp(e, t, n, r) {
             if (void 0 === r && (r = 1), "function" !== typeof e) throw Error("functionToRetry must be a function");
-            return Gp(e.name + " attempt #" + r + " with args: " + JSON.stringify(t)), e.apply(void 0, t).catch((function(o) {
-                if (Gp("error on " + e.name, o), (i = o) && i.nonRetryable) throw Gp(e.name + " non retryable error", o), o;
+            return _p(e.name + " attempt #" + r + " with args: " + JSON.stringify(t)), e.apply(void 0, t).catch((function(o) {
+                if (_p("error on " + e.name, o), (i = o) && i.nonRetryable) throw _p(e.name + " non retryable error", o), o;
                 var i, a = n(r, t, o);
-                if (Gp(e.name + " retrying in " + a + " ms"), !1 !== a) return new Promise((function(e) {
+                if (_p(e.name + " retrying in " + a + " ms"), !1 !== a) return new Promise((function(e) {
                     return setTimeout(e, a)
                 })).then((function() {
-                    return Wp(e, t, n, r + 1)
+                    return Tp(e, t, n, r + 1)
                 }));
                 throw o
             }))
         }
-        var Hp = 3e5;
-        var Zp, Vp = function() {
+        var Ap = 3e5;
+        var Op, zp = function() {
                 function e(e, t) {
                     var n = e || {},
                         r = n.UserPoolId,
                         o = n.ClientId,
                         i = n.endpoint,
                         a = n.fetchOptions,
                         s = n.AdvancedSecurityDataCollectionFlag;
                     if (!r || !o) throw new Error("Both UserPoolId and ClientId are required.");
                     if (r.length > 55 || !/^[\w-]+_[0-9a-zA-Z]+$/.test(r)) throw new Error("Invalid UserPoolId format.");
                     var u = r.split("_")[0];
-                    this.userPoolId = r, this.clientId = o, this.client = new Qp(u, i, a), this.advancedSecurityDataCollectionFlag = !1 !== s, this.storage = e.Storage || (new Ep).getStorage(), t && (this.wrapRefreshSessionCallback = t)
+                    this.userPoolId = r, this.clientId = o, this.client = new Ep(u, i, a), this.advancedSecurityDataCollectionFlag = !1 !== s, this.storage = e.Storage || (new Mp).getStorage(), t && (this.wrapRefreshSessionCallback = t)
                 }
                 var t = e.prototype;
                 return t.getUserPoolId = function() {
                     return this.userPoolId
                 }, t.getUserPoolName = function() {
                     return this.getUserPoolId().split("_")[1]
                 }, t.getClientId = function() {
@@ -66312,15 +63760,15 @@
                         if (t) return o(t, null);
                         var r = {
                                 Username: e,
                                 Pool: a,
                                 Storage: a.storage
                             },
                             i = {
-                                user: new Tp(r),
+                                user: new wp(r),
                                 userConfirmed: n.UserConfirmed,
                                 userSub: n.UserSub,
                                 codeDeliveryDetails: n.CodeDeliveryDetails
                             };
                         return o(null, i)
                     }))
                 }, t.getCurrentUser = function() {
@@ -66328,15 +63776,15 @@
                         t = this.storage.getItem(e);
                     if (t) {
                         var n = {
                             Username: t,
                             Pool: this,
                             Storage: this.storage
                         };
-                        return new Tp(n)
+                        return new wp(n)
                     }
                     return null
                 }, t.getUserContextData = function(e) {
                     if ("undefined" !== typeof AmazonCognitoAdvancedSecurityData) {
                         var t = AmazonCognitoAdvancedSecurityData;
                         if (this.advancedSecurityDataCollectionFlag) {
                             var n = t.getData(e, this.userPoolId, this.clientId);
@@ -66344,16 +63792,16 @@
                                 EncodedData: n
                             }
                         }
                         return {}
                     }
                 }, e
             }(),
-            qp = __webpack_require__(5943),
-            Jp = function() {
+            Up = __webpack_require__(5943),
+            Pp = function() {
                 function e(e) {
                     if (!e.domain) throw new Error("The domain of cookieStorage can not be undefined.");
                     if (this.domain = e.domain, e.path ? this.path = e.path : this.path = "/", Object.prototype.hasOwnProperty.call(e, "expires") ? this.expires = e.expires : this.expires = 365, Object.prototype.hasOwnProperty.call(e, "secure") ? this.secure = e.secure : this.secure = !0, Object.prototype.hasOwnProperty.call(e, "sameSite")) {
                         if (!["strict", "lax", "none"].includes(e.sameSite)) throw new Error('The sameSite value of cookieStorage must be "lax", "strict" or "none".');
                         if ("none" === e.sameSite && !this.secure) throw new Error("sameSite = None requires the Secure attribute in latest browser versions.");
                         this.sameSite = e.sameSite
                     } else this.sameSite = null
@@ -66362,116 +63810,116 @@
                 return t.setItem = function(e, t) {
                     var n = {
                         path: this.path,
                         expires: this.expires,
                         domain: this.domain,
                         secure: this.secure
                     };
-                    return this.sameSite && (n.sameSite = this.sameSite), qp.set(e, t, n), qp.get(e)
+                    return this.sameSite && (n.sameSite = this.sameSite), Up.set(e, t, n), Up.get(e)
                 }, t.getItem = function(e) {
-                    return qp.get(e)
+                    return Up.get(e)
                 }, t.removeItem = function(e) {
                     var t = {
                         path: this.path,
                         expires: this.expires,
                         domain: this.domain,
                         secure: this.secure
                     };
-                    return this.sameSite && (t.sameSite = this.sameSite), qp.remove(e, t)
+                    return this.sameSite && (t.sameSite = this.sameSite), Up.remove(e, t)
                 }, t.clear = function() {
-                    for (var e = qp.get(), t = Object.keys(e).length, n = 0; n < t; ++n) this.removeItem(Object.keys(e)[n]);
+                    for (var e = Up.get(), t = Object.keys(e).length, n = 0; n < t; ++n) this.removeItem(Object.keys(e)[n]);
                     return {}
                 }, e
             }(),
-            Kp = __webpack_require__(2770),
-            Xp = function(e) {
+            Rp = __webpack_require__(2770),
+            Bp = function(e) {
                 var t = window.open(e, "_self");
                 return t ? Promise.resolve(t) : Promise.reject()
             },
-            $p = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
-            eh = function(e, t, n) {
-                _s.dispatch("auth", {
+            Fp = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
+            Yp = function(e, t, n) {
+                bs.dispatch("auth", {
                     event: e,
                     data: t,
                     message: n
-                }, "Auth", $p)
+                }, "Auth", Fp)
             },
-            th = new Ls("OAuth"),
-            nh = function() {
+            Qp = new ys("OAuth"),
+            Gp = function() {
                 function e(e) {
                     var t = e.config,
                         n = e.cognitoClientId,
                         r = e.scopes,
                         o = void 0 === r ? [] : r;
-                    if (this._urlOpener = t.urlOpener || Xp, this._config = t, this._cognitoClientId = n, !this.isValidScopes(o)) throw Error("scopes must be a String Array");
+                    if (this._urlOpener = t.urlOpener || Bp, this._config = t, this._cognitoClientId = n, !this.isValidScopes(o)) throw Error("scopes must be a String Array");
                     this._scopes = o
                 }
                 return e.prototype.isValidScopes = function(e) {
                     return Array.isArray(e) && e.every((function(e) {
                         return "string" === typeof e
                     }))
                 }, e.prototype.oauthSignIn = function(e, t, n, r, o, i) {
-                    void 0 === e && (e = "code"), void 0 === o && (o = cs.Cognito);
+                    void 0 === e && (e = "code"), void 0 === o && (o = Xa.Cognito);
                     var a = this._generateState(32),
                         s = i ? a + "-" + i.split("").map((function(e) {
                             return e.charCodeAt(0).toString(16).padStart(2, "0")
                         })).join("") : a;
                     ! function(e) {
                         window.sessionStorage.setItem("oauth_state", e)
                     }(s);
                     var u, l = this._generateRandom(128);
                     u = l, window.sessionStorage.setItem("ouath_pkce_key", u);
                     var c = this._generateChallenge(l),
                         d = this._scopes.join(" "),
-                        f = Object.entries(ps(ps({
+                        f = Object.entries(ts(ts({
                             redirect_uri: n,
                             response_type: e,
                             client_id: r,
                             identity_provider: o,
                             scope: d,
                             state: s
                         }, "code" === e ? {
                             code_challenge: c
                         } : {}), "code" === e ? {
                             code_challenge_method: "S256"
                         } : {})).map((function(e) {
-                            var t = ys(e, 2),
+                            var t = os(e, 2),
                                 n = t[0],
                                 r = t[1];
                             return encodeURIComponent(n) + "=" + encodeURIComponent(r)
                         })).join("&"),
                         p = "https://" + t + "/oauth2/authorize?" + f;
-                    th.debug("Redirecting to " + p), this._urlOpener(p, n)
+                    Qp.debug("Redirecting to " + p), this._urlOpener(p, n)
                 }, e.prototype._handleCodeFlow = function(e) {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var t, n, r, o, i, a, s, u, l, c, d, f, p, h;
-                        return gs(this, (function(g) {
+                        return rs(this, (function(g) {
                             switch (g.label) {
                                 case 0:
-                                    return t = ((0, Kp.Qc)(e).query || "").split("&").map((function(e) {
+                                    return t = ((0, Rp.Qc)(e).query || "").split("&").map((function(e) {
                                         return e.split("=")
                                     })).reduce((function(e, t) {
-                                        var n, r = ys(t, 2),
+                                        var n, r = os(t, 2),
                                             o = r[0],
                                             i = r[1];
-                                        return ps(ps({}, e), ((n = {})[o] = i, n))
+                                        return ts(ts({}, e), ((n = {})[o] = i, n))
                                     }), {
                                         code: void 0
-                                    }).code, n = (0, Kp.Qc)(e).pathname || "/", r = (0, Kp.Qc)(this._config.redirectSignIn).pathname || "/", t && n === r ? (o = "https://" + this._config.domain + "/oauth2/token", eh("codeFlow", {}, "Retrieving tokens from " + o), i = vs(this._config) ? this._cognitoClientId : this._config.clientID, a = vs(this._config) ? this._config.redirectSignIn : this._config.redirectUri, s = function() {
+                                    }).code, n = (0, Rp.Qc)(e).pathname || "/", r = (0, Rp.Qc)(this._config.redirectSignIn).pathname || "/", t && n === r ? (o = "https://" + this._config.domain + "/oauth2/token", Yp("codeFlow", {}, "Retrieving tokens from " + o), i = as(this._config) ? this._cognitoClientId : this._config.clientID, a = as(this._config) ? this._config.redirectSignIn : this._config.redirectUri, s = function() {
                                         var e = window.sessionStorage.getItem("ouath_pkce_key");
                                         return window.sessionStorage.removeItem("ouath_pkce_key"), e
-                                    }(), u = ps({
+                                    }(), u = ts({
                                         grant_type: "authorization_code",
                                         code: t,
                                         client_id: i,
                                         redirect_uri: a
                                     }, s ? {
                                         code_verifier: s
-                                    } : {}), th.debug("Calling token endpoint: " + o + " with", u), l = Object.entries(u).map((function(e) {
-                                        var t = ys(e, 2),
+                                    } : {}), Qp.debug("Calling token endpoint: " + o + " with", u), l = Object.entries(u).map((function(e) {
+                                        var t = os(e, 2),
                                             n = t[0],
                                             r = t[1];
                                         return encodeURIComponent(n) + "=" + encodeURIComponent(r)
                                     })).join("&"), [4, fetch(o, {
                                         method: "POST",
                                         headers: {
                                             "Content-Type": "application/x-www-form-urlencoded"
@@ -66487,70 +63935,70 @@
                                         refreshToken: f,
                                         idToken: p
                                     }]
                             }
                         }))
                     }))
                 }, e.prototype._handleImplicitFlow = function(e) {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var t, n, r;
-                        return gs(this, (function(o) {
-                            return t = ((0, Kp.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
+                        return rs(this, (function(o) {
+                            return t = ((0, Rp.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
                                 return e.split("=")
                             })).reduce((function(e, t) {
-                                var n, r = ys(t, 2),
+                                var n, r = os(t, 2),
                                     o = r[0],
                                     i = r[1];
-                                return ps(ps({}, e), ((n = {})[o] = i, n))
+                                return ts(ts({}, e), ((n = {})[o] = i, n))
                             }), {
                                 id_token: void 0,
                                 access_token: void 0
-                            }), n = t.id_token, r = t.access_token, eh("implicitFlow", {}, "Got tokens from " + e), th.debug("Retrieving implicit tokens from " + e + " with"), [2, {
+                            }), n = t.id_token, r = t.access_token, Yp("implicitFlow", {}, "Got tokens from " + e), Qp.debug("Retrieving implicit tokens from " + e + " with"), [2, {
                                 accessToken: r,
                                 idToken: n,
                                 refreshToken: null
                             }]
                         }))
                     }))
                 }, e.prototype.handleAuthResponse = function(e) {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var t, n, r, o, i, a, s;
-                        return gs(this, (function(u) {
+                        return rs(this, (function(u) {
                             switch (u.label) {
                                 case 0:
-                                    if (u.trys.push([0, 5, , 6]), t = e ? ps(ps({}, ((0, Kp.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
+                                    if (u.trys.push([0, 5, , 6]), t = e ? ts(ts({}, ((0, Rp.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
                                             return e.split("=")
                                         })).reduce((function(e, t) {
-                                            var n = ys(t, 2),
+                                            var n = os(t, 2),
                                                 r = n[0],
                                                 o = n[1];
                                             return e[r] = o, e
-                                        }), {})), ((0, Kp.Qc)(e).query || "").split("&").map((function(e) {
+                                        }), {})), ((0, Rp.Qc)(e).query || "").split("&").map((function(e) {
                                             return e.split("=")
                                         })).reduce((function(e, t) {
-                                            var n = ys(t, 2),
+                                            var n = os(t, 2),
                                                 r = n[0],
                                                 o = n[1];
                                             return e[r] = o, e
                                         }), {})) : {}, n = t.error, r = t.error_description, n) throw new Error(r);
-                                    return o = this._validateState(t), th.debug("Starting " + this._config.responseType + " flow with " + e), "code" !== this._config.responseType ? [3, 2] : (i = [{}], [4, this._handleCodeFlow(e)]);
+                                    return o = this._validateState(t), Qp.debug("Starting " + this._config.responseType + " flow with " + e), "code" !== this._config.responseType ? [3, 2] : (i = [{}], [4, this._handleCodeFlow(e)]);
                                 case 1:
-                                    return [2, ps.apply(void 0, [ps.apply(void 0, i.concat([u.sent()])), {
+                                    return [2, ts.apply(void 0, [ts.apply(void 0, i.concat([u.sent()])), {
                                         state: o
                                     }])];
                                 case 2:
                                     return a = [{}], [4, this._handleImplicitFlow(e)];
                                 case 3:
-                                    return [2, ps.apply(void 0, [ps.apply(void 0, a.concat([u.sent()])), {
+                                    return [2, ts.apply(void 0, [ts.apply(void 0, a.concat([u.sent()])), {
                                         state: o
                                     }])];
                                 case 4:
                                     return [3, 6];
                                 case 5:
-                                    throw s = u.sent(), th.error("Error handling auth response.", s), s;
+                                    throw s = u.sent(), Qp.error("Error handling auth response.", s), s;
                                 case 6:
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype._validateState = function(e) {
                     if (e) {
@@ -66559,33 +64007,33 @@
                                 return window.sessionStorage.removeItem("oauth_state"), e
                             }(),
                             n = e.state;
                         if (t && t !== n) throw new Error("Invalid state in OAuth flow");
                         return n
                     }
                 }, e.prototype.signOut = function() {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var e, t, n;
-                        return gs(this, (function(r) {
-                            return e = "https://" + this._config.domain + "/logout?", t = vs(this._config) ? this._cognitoClientId : this._config.oauth.clientID, n = vs(this._config) ? this._config.redirectSignOut : this._config.returnTo, e += Object.entries({
+                        return rs(this, (function(r) {
+                            return e = "https://" + this._config.domain + "/logout?", t = as(this._config) ? this._cognitoClientId : this._config.oauth.clientID, n = as(this._config) ? this._config.redirectSignOut : this._config.returnTo, e += Object.entries({
                                 client_id: t,
                                 logout_uri: encodeURIComponent(n)
                             }).map((function(e) {
-                                var t = ys(e, 2);
+                                var t = os(e, 2);
                                 return t[0] + "=" + t[1]
-                            })).join("&"), eh("oAuthSignOut", {
+                            })).join("&"), Yp("oAuthSignOut", {
                                 oAuth: "signOut"
-                            }, "Signing out from " + e), th.debug("Signing out from " + e), [2, this._urlOpener(e, n)]
+                            }, "Signing out from " + e), Qp.debug("Signing out from " + e), [2, this._urlOpener(e, n)]
                         }))
                     }))
                 }, e.prototype._generateState = function(e) {
                     for (var t = "", n = e, r = "0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ"; n > 0; --n) t += r[Math.round(Math.random() * (r.length - 1))];
                     return t
                 }, e.prototype._generateChallenge = function(e) {
-                    var t = new tp.Sha256;
+                    var t = new Qf.Sha256;
                     t.update(e);
                     var n = t.digestSync(),
                         r = nt.lW.from(n).toString("base64");
                     return this._base64URL(r)
                 }, e.prototype._base64URL = function(e) {
                     return e.replace(/=/g, "").replace(/\+/g, "-").replace(/\//g, "_")
                 }, e.prototype._generateRandom = function(e) {
@@ -66598,104 +64046,104 @@
                     for (var t = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789", n = [], r = 0; r < e.byteLength; r += 1) {
                         var o = e[r] % t.length;
                         n.push(t[o])
                     }
                     return n.join("")
                 }, e
             }(),
-            rh = nh;
+            Wp = Gp;
         ! function(e) {
             e.DEFAULT_MSG = "Authentication Error", e.EMPTY_EMAIL = "Email cannot be empty", e.EMPTY_PHONE = "Phone number cannot be empty", e.EMPTY_USERNAME = "Username cannot be empty", e.INVALID_USERNAME = "The username should either be a string or one of the sign in types", e.EMPTY_PASSWORD = "Password cannot be empty", e.EMPTY_CODE = "Confirmation code cannot be empty", e.SIGN_UP_ERROR = "Error creating account", e.NO_MFA = "No valid MFA method provided", e.INVALID_MFA = "Invalid MFA type", e.EMPTY_CHALLENGE = "Challenge response cannot be empty", e.NO_USER_SESSION = "Failed to get the session because the user is empty", e.NETWORK_ERROR = "Network Error", e.DEVICE_CONFIG = "Device tracking has not been configured in this User Pool", e.AUTOSIGNIN_ERROR = "Please use your credentials to sign in"
-        }(Zp || (Zp = {}));
-        var oh = new Ls("AuthError"),
-            ih = function(e) {
+        }(Op || (Op = {}));
+        var Hp = new ys("AuthError"),
+            Zp = function(e) {
                 function t(n) {
                     var r = this,
-                        o = sh[n],
+                        o = qp[n],
                         i = o.message,
                         a = o.log;
-                    return (r = e.call(this, i) || this).constructor = t, Object.setPrototypeOf(r, t.prototype), r.name = "AuthError", r.log = a || i, oh.error(r.log), r
+                    return (r = e.call(this, i) || this).constructor = t, Object.setPrototypeOf(r, t.prototype), r.name = "AuthError", r.log = a || i, Hp.error(r.log), r
                 }
-                return ls(t, e), t
+                return Ka(t, e), t
             }(Error),
-            ah = function(e) {
+            Vp = function(e) {
                 function t(n) {
                     var r = e.call(this, n) || this;
                     return r.constructor = t, Object.setPrototypeOf(r, t.prototype), r.name = "NoUserPoolError", r
                 }
-                return ls(t, e), t
-            }(ih),
-            sh = {
+                return Ka(t, e), t
+            }(Zp),
+            qp = {
                 noConfig: {
-                    message: Zp.DEFAULT_MSG,
+                    message: Op.DEFAULT_MSG,
                     log: "\n            Error: Amplify has not been configured correctly.\n            This error is typically caused by one of the following scenarios:\n\n            1. Make sure you're passing the awsconfig object to Amplify.configure() in your app's entry point\n                See https://aws-amplify.github.io/docs/js/authentication#configure-your-app for more information\n            \n            2. There might be multiple conflicting versions of amplify packages in your node_modules.\n\t\t\t\tRefer to our docs site for help upgrading Amplify packages (https://docs.amplify.aws/lib/troubleshooting/upgrading/q/platform/js)\n        "
                 },
                 missingAuthConfig: {
-                    message: Zp.DEFAULT_MSG,
+                    message: Op.DEFAULT_MSG,
                     log: "\n            Error: Amplify has not been configured correctly. \n            The configuration object is missing required auth properties.\n            This error is typically caused by one of the following scenarios:\n\n            1. Did you run `amplify push` after adding auth via `amplify add auth`?\n                See https://aws-amplify.github.io/docs/js/authentication#amplify-project-setup for more information\n\n            2. This could also be caused by multiple conflicting versions of amplify packages, see (https://docs.amplify.aws/lib/troubleshooting/upgrading/q/platform/js) for help upgrading Amplify packages.\n        "
                 },
                 emptyUsername: {
-                    message: Zp.EMPTY_USERNAME
+                    message: Op.EMPTY_USERNAME
                 },
                 invalidUsername: {
-                    message: Zp.INVALID_USERNAME
+                    message: Op.INVALID_USERNAME
                 },
                 emptyPassword: {
-                    message: Zp.EMPTY_PASSWORD
+                    message: Op.EMPTY_PASSWORD
                 },
                 emptyCode: {
-                    message: Zp.EMPTY_CODE
+                    message: Op.EMPTY_CODE
                 },
                 signUpError: {
-                    message: Zp.SIGN_UP_ERROR,
+                    message: Op.SIGN_UP_ERROR,
                     log: "The first parameter should either be non-null string or object"
                 },
                 noMFA: {
-                    message: Zp.NO_MFA
+                    message: Op.NO_MFA
                 },
                 invalidMFA: {
-                    message: Zp.INVALID_MFA
+                    message: Op.INVALID_MFA
                 },
                 emptyChallengeResponse: {
-                    message: Zp.EMPTY_CHALLENGE
+                    message: Op.EMPTY_CHALLENGE
                 },
                 noUserSession: {
-                    message: Zp.NO_USER_SESSION
+                    message: Op.NO_USER_SESSION
                 },
                 deviceConfig: {
-                    message: Zp.DEVICE_CONFIG
+                    message: Op.DEVICE_CONFIG
                 },
                 networkError: {
-                    message: Zp.NETWORK_ERROR
+                    message: Op.NETWORK_ERROR
                 },
                 autoSignInError: {
-                    message: Zp.AUTOSIGNIN_ERROR
+                    message: Op.AUTOSIGNIN_ERROR
                 },
                 default: {
-                    message: Zp.DEFAULT_MSG
+                    message: Op.DEFAULT_MSG
                 }
             },
-            uh = new Ls("AuthClass"),
-            lh = "aws.cognito.signin.user.admin",
-            ch = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
-            dh = function(e, t, n) {
-                _s.dispatch("auth", {
+            Jp = new ys("AuthClass"),
+            Kp = "aws.cognito.signin.user.admin",
+            Xp = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
+            $p = function(e, t, n) {
+                bs.dispatch("auth", {
                     event: e,
                     data: t,
                     message: n
-                }, "Auth", ch)
+                }, "Auth", Xp)
             },
-            fh = function() {
+            eh = function() {
                 function e(e) {
                     var t = this;
-                    this.userPool = null, this.user = null, this.oAuthFlowInProgress = !1, this.autoSignInInitiated = !1, this.inflightSessionPromise = null, this.inflightSessionPromiseCounter = 0, this.Credentials = Hf, this.wrapRefreshSessionCallback = function(e) {
+                    this.userPool = null, this.user = null, this.oAuthFlowInProgress = !1, this.autoSignInInitiated = !1, this.inflightSessionPromise = null, this.inflightSessionPromiseCounter = 0, this.Credentials = Af, this.wrapRefreshSessionCallback = function(e) {
                         return function(t, n) {
-                            return n ? dh("tokenRefresh", void 0, "New token retrieved") : dh("tokenRefresh_failure", t, "Failed to retrieve new token"), e(t, n)
+                            return n ? $p("tokenRefresh", void 0, "New token retrieved") : $p("tokenRefresh_failure", t, "Failed to retrieve new token"), e(t, n)
                         }
-                    }, this.configure(e), this.currentCredentials = this.currentCredentials.bind(this), this.currentUserCredentials = this.currentUserCredentials.bind(this), _s.listen("auth", (function(e) {
+                    }, this.configure(e), this.currentCredentials = this.currentCredentials.bind(this), this.currentUserCredentials = this.currentUserCredentials.bind(this), bs.listen("auth", (function(e) {
                         switch (e.payload.event) {
                             case "verify":
                             case "signIn":
                                 t._storage.setItem("amplify-signin-with-hostedUI", "false");
                                 break;
                             case "signOut":
                                 t._storage.removeItem("amplify-signin-with-hostedUI");
@@ -66706,80 +64154,80 @@
                     }))
                 }
                 return e.prototype.getModuleName = function() {
                     return "Auth"
                 }, e.prototype.configure = function(e) {
                     var t = this;
                     if (!e) return this._config || {};
-                    uh.debug("configure Auth");
-                    var n = Object.assign({}, this._config, bc(e).Auth, e);
+                    Jp.debug("configure Auth");
+                    var n = Object.assign({}, this._config, uc(e).Auth, e);
                     this._config = n;
                     var r = this._config,
                         o = r.userPoolId,
                         i = r.userPoolWebClientId,
                         a = r.cookieStorage,
                         s = r.oauth,
                         u = r.region,
                         l = r.identityPoolId,
                         c = r.mandatorySignIn,
                         d = r.refreshHandlers,
                         f = r.identityPoolRegion,
                         p = r.clientMetadata,
                         h = r.endpoint;
                     if (this._config.storage) {
-                        if (!this._isValidAuthStorage(this._config.storage)) throw uh.error("The storage in the Auth config is not valid!"), new Error("Empty storage object");
+                        if (!this._isValidAuthStorage(this._config.storage)) throw Jp.error("The storage in the Auth config is not valid!"), new Error("Empty storage object");
                         this._storage = this._config.storage
-                    } else this._storage = a ? new Jp(a) : e.ssr ? new Vf : (new Os).getStorage();
+                    } else this._storage = a ? new Pp(a) : e.ssr ? new zf : (new xs).getStorage();
                     if (this._storageSync = Promise.resolve(), "function" === typeof this._storage.sync && (this._storageSync = this._storage.sync()), o) {
                         var g = {
                             UserPoolId: o,
                             ClientId: i,
                             endpoint: h
                         };
-                        g.Storage = this._storage, this.userPool = new Vp(g, this.wrapRefreshSessionCallback)
+                        g.Storage = this._storage, this.userPool = new zp(g, this.wrapRefreshSessionCallback)
                     }
                     this.Credentials.configure({
                         mandatorySignIn: c,
                         region: u,
                         userPoolId: o,
                         identityPoolId: l,
                         refreshHandlers: d,
                         storage: this._storage,
                         identityPoolRegion: f
                     });
-                    var y = s ? vs(this._config.oauth) ? s : s.awsCognito : void 0;
+                    var y = s ? as(this._config.oauth) ? s : s.awsCognito : void 0;
                     if (y) {
                         var m = Object.assign({
                             cognitoClientId: i,
                             UserPoolId: o,
                             domain: y.domain,
                             scopes: y.scope,
                             redirectSignIn: y.redirectSignIn,
                             redirectSignOut: y.redirectSignOut,
                             responseType: y.responseType,
                             Storage: this._storage,
                             urlOpener: y.urlOpener,
                             clientMetadata: p
                         }, y.options);
-                        this._oAuthHandler = new rh({
+                        this._oAuthHandler = new Wp({
                             scopes: m.scopes,
                             config: m,
                             cognitoClientId: m.cognitoClientId
                         });
                         var v = {};
                         ! function(e) {
-                            if (zs().isBrowser && window.location) e({
+                            if (Ns().isBrowser && window.location) e({
                                 url: window.location.href
                             });
-                            else if (!zs().isNode) throw new Error("Not supported")
+                            else if (!Ns().isNode) throw new Error("Not supported")
                         }((function(e) {
                             var n = e.url;
                             v[n] || (v[n] = !0, t._handleAuthResponse(n))
                         }))
-                    }(dh("configured", null, "The Auth category has been configured successfully"), this.autoSignInInitiated || "function" !== typeof this._storage.getItem) || (this.isTrueStorageValue("amplify-polling-started") && (dh("autoSignIn_failure", null, ds.AutoSignInError), this._storage.removeItem("amplify-auto-sign-in")), this._storage.removeItem("amplify-polling-started"));
+                    }($p("configured", null, "The Auth category has been configured successfully"), this.autoSignInInitiated || "function" !== typeof this._storage.getItem) || (this.isTrueStorageValue("amplify-polling-started") && ($p("autoSignIn_failure", null, $a.AutoSignInError), this._storage.removeItem("amplify-auto-sign-in")), this._storage.removeItem("amplify-polling-started"));
                     return this._config
                 }, e.prototype.signUp = function(e) {
                     for (var t, n, r, o = this, i = [], a = 1; a < arguments.length; a++) i[a - 1] = arguments[a];
                     if (!this.userPool) return this.rejectNoUserPool();
                     var s, u = null,
                         l = null,
                         c = [],
@@ -66789,187 +64237,187 @@
                         },
                         p = {},
                         h = {};
                     if (e && "string" === typeof e) {
                         u = e, l = i ? i[0] : null;
                         var g = i ? i[1] : null,
                             y = i ? i[2] : null;
-                        g && c.push(new Lp({
+                        g && c.push(new yp({
                             Name: "email",
                             Value: g
-                        })), y && c.push(new Lp({
+                        })), y && c.push(new yp({
                             Name: "phone_number",
                             Value: y
                         }))
                     } else {
-                        if (!e || "object" !== typeof e) return this.rejectAuthError(ds.SignUpError);
+                        if (!e || "object" !== typeof e) return this.rejectAuthError($a.SignUpError);
                         u = e.username, l = e.password, e && e.clientMetadata ? s = e.clientMetadata : this._config.clientMetadata && (s = this._config.clientMetadata);
                         var m = e.attributes;
                         m && Object.keys(m).map((function(e) {
-                            c.push(new Lp({
+                            c.push(new yp({
                                 Name: e,
                                 Value: m[e]
                             }))
                         }));
                         var v = e.validationData;
                         v && (d = [], Object.keys(v).map((function(e) {
-                            d.push(new Lp({
+                            d.push(new yp({
                                 Name: e,
                                 Value: v[e]
                             }))
                         }))), (f = null !== (t = e.autoSignIn) && void 0 !== t ? t : {
                             enabled: !1
                         }).enabled && (this._storage.setItem("amplify-auto-sign-in", "true"), p = null !== (n = f.validationData) && void 0 !== n ? n : {}, h = null !== (r = f.clientMetaData) && void 0 !== r ? r : {})
                     }
-                    return u ? l ? (uh.debug("signUp attrs:", c), uh.debug("signUp validation data:", d), new Promise((function(e, t) {
+                    return u ? l ? (Jp.debug("signUp attrs:", c), Jp.debug("signUp validation data:", d), new Promise((function(e, t) {
                         o.userPool.signUp(u, l, c, d, (function(n, r) {
-                            n ? (dh("signUp_failure", n, u + " failed to signup"), t(n)) : (dh("signUp", r, u + " has signed up successfully"), f.enabled && o.handleAutoSignIn(u, l, p, h, r), e(r))
+                            n ? ($p("signUp_failure", n, u + " failed to signup"), t(n)) : ($p("signUp", r, u + " has signed up successfully"), f.enabled && o.handleAutoSignIn(u, l, p, h, r), e(r))
                         }), s)
-                    }))) : this.rejectAuthError(ds.EmptyPassword) : this.rejectAuthError(ds.EmptyUsername)
+                    }))) : this.rejectAuthError($a.EmptyPassword) : this.rejectAuthError($a.EmptyUsername)
                 }, e.prototype.handleAutoSignIn = function(e, t, n, r, o) {
                     this.autoSignInInitiated = !0;
-                    var i = new Jf({
+                    var i = new Pf({
                         Username: e,
                         Password: t,
                         ValidationData: n,
                         ClientMetadata: r
                     });
                     o.userConfirmed ? this.signInAfterUserConfirmed(i) : "link" === this._config.signUpVerificationMethod ? this.handleLinkAutoSignIn(i) : this.handleCodeAutoSignIn(i)
                 }, e.prototype.handleCodeAutoSignIn = function(e) {
                     var t = this;
-                    _s.listen("auth", (function n(r) {
+                    bs.listen("auth", (function n(r) {
                         "confirmSignUp" === r.payload.event && t.signInAfterUserConfirmed(e, n)
                     }))
                 }, e.prototype.handleLinkAutoSignIn = function(e) {
                     var t = this;
                     this._storage.setItem("amplify-polling-started", "true");
                     var n = Date.now(),
                         r = setInterval((function() {
-                            Date.now() - n > 18e4 ? (clearInterval(r), dh("autoSignIn_failure", null, "Please confirm your account and use your credentials to sign in."), t._storage.removeItem("amplify-auto-sign-in")) : t.signInAfterUserConfirmed(e, null, r)
+                            Date.now() - n > 18e4 ? (clearInterval(r), $p("autoSignIn_failure", null, "Please confirm your account and use your credentials to sign in."), t._storage.removeItem("amplify-auto-sign-in")) : t.signInAfterUserConfirmed(e, null, r)
                         }), 5e3)
                 }, e.prototype.signInAfterUserConfirmed = function(e, t, n) {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var r, o, i = this;
-                        return gs(this, (function(a) {
+                        return rs(this, (function(a) {
                             switch (a.label) {
                                 case 0:
                                     r = this.createCognitoUser(e.getUsername()), a.label = 1;
                                 case 1:
                                     return a.trys.push([1, 3, , 4]), [4, r.authenticateUser(e, this.authCallbacks(r, (function(r) {
-                                        dh("autoSignIn", r, e.getUsername() + " has signed in successfully"), t && _s.remove("auth", t), n && (clearInterval(n), i._storage.removeItem("amplify-polling-started")), i._storage.removeItem("amplify-auto-sign-in")
+                                        $p("autoSignIn", r, e.getUsername() + " has signed in successfully"), t && bs.remove("auth", t), n && (clearInterval(n), i._storage.removeItem("amplify-polling-started")), i._storage.removeItem("amplify-auto-sign-in")
                                     }), (function(e) {
-                                        uh.error(e), i._storage.removeItem("amplify-auto-sign-in")
+                                        Jp.error(e), i._storage.removeItem("amplify-auto-sign-in")
                                     })))];
                                 case 2:
                                     return a.sent(), [3, 4];
                                 case 3:
-                                    return o = a.sent(), uh.error(o), [3, 4];
+                                    return o = a.sent(), Jp.error(o), [3, 4];
                                 case 4:
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype.confirmSignUp = function(e, t, n) {
                     var r = this;
                     if (!this.userPool) return this.rejectNoUserPool();
-                    if (!e) return this.rejectAuthError(ds.EmptyUsername);
-                    if (!t) return this.rejectAuthError(ds.EmptyCode);
+                    if (!e) return this.rejectAuthError($a.EmptyUsername);
+                    if (!t) return this.rejectAuthError($a.EmptyCode);
                     var o, i = this.createCognitoUser(e),
                         a = !n || "boolean" !== typeof n.forceAliasCreation || n.forceAliasCreation;
                     return n && n.clientMetadata ? o = n.clientMetadata : this._config.clientMetadata && (o = this._config.clientMetadata), new Promise((function(n, s) {
                         i.confirmRegistration(t, a, (function(t, o) {
-                            t ? s(t) : (dh("confirmSignUp", o, e + " has been confirmed successfully"), r.isTrueStorageValue("amplify-auto-sign-in") && !r.autoSignInInitiated && (dh("autoSignIn_failure", null, ds.AutoSignInError), r._storage.removeItem("amplify-auto-sign-in")), n(o))
+                            t ? s(t) : ($p("confirmSignUp", o, e + " has been confirmed successfully"), r.isTrueStorageValue("amplify-auto-sign-in") && !r.autoSignInInitiated && ($p("autoSignIn_failure", null, $a.AutoSignInError), r._storage.removeItem("amplify-auto-sign-in")), n(o))
                         }), o)
                     }))
                 }, e.prototype.isTrueStorageValue = function(e) {
                     var t = this._storage.getItem(e);
                     return !!t && "true" === t
                 }, e.prototype.resendSignUp = function(e, t) {
                     if (void 0 === t && (t = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                    if (!e) return this.rejectAuthError(ds.EmptyUsername);
+                    if (!e) return this.rejectAuthError($a.EmptyUsername);
                     var n = this.createCognitoUser(e);
                     return new Promise((function(e, r) {
                         n.resendConfirmationCode((function(t, n) {
                             t ? r(t) : e(n)
                         }), t)
                     }))
                 }, e.prototype.signIn = function(e, t, n) {
                     if (void 0 === n && (n = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
                     var r = null,
                         o = null,
                         i = {};
                     if ("string" === typeof e) r = e, o = t;
                     else {
-                        if (!e.username) return this.rejectAuthError(ds.InvalidUsername);
-                        "undefined" !== typeof t && uh.warn("The password should be defined under the first parameter object!"), r = e.username, o = e.password, i = e.validationData
+                        if (!e.username) return this.rejectAuthError($a.InvalidUsername);
+                        "undefined" !== typeof t && Jp.warn("The password should be defined under the first parameter object!"), r = e.username, o = e.password, i = e.validationData
                     }
-                    if (!r) return this.rejectAuthError(ds.EmptyUsername);
-                    var a = new Jf({
+                    if (!r) return this.rejectAuthError($a.EmptyUsername);
+                    var a = new Pf({
                         Username: r,
                         Password: o,
                         ValidationData: i,
                         ClientMetadata: n
                     });
                     return o ? this.signInWithPassword(a) : this.signInWithoutPassword(a)
                 }, e.prototype.authCallbacks = function(e, t, n) {
                     var r = this,
                         o = this;
                     return {
                         onSuccess: function(i) {
-                            return hs(r, void 0, void 0, (function() {
+                            return ns(r, void 0, void 0, (function() {
                                 var r, a, s, u;
-                                return gs(this, (function(l) {
+                                return rs(this, (function(l) {
                                     switch (l.label) {
                                         case 0:
-                                            uh.debug(i), delete e.challengeName, delete e.challengeParam, l.label = 1;
+                                            Jp.debug(i), delete e.challengeName, delete e.challengeParam, l.label = 1;
                                         case 1:
                                             return l.trys.push([1, 4, 5, 9]), [4, this.Credentials.clear()];
                                         case 2:
                                             return l.sent(), [4, this.Credentials.set(i, "session")];
                                         case 3:
-                                            return r = l.sent(), uh.debug("succeed to get cognito credentials", r), [3, 9];
+                                            return r = l.sent(), Jp.debug("succeed to get cognito credentials", r), [3, 9];
                                         case 4:
-                                            return a = l.sent(), uh.debug("cannot get cognito credentials", a), [3, 9];
+                                            return a = l.sent(), Jp.debug("cannot get cognito credentials", a), [3, 9];
                                         case 5:
                                             return l.trys.push([5, 7, , 8]), [4, this.currentUserPoolUser()];
                                         case 6:
-                                            return s = l.sent(), o.user = s, dh("signIn", s, "A user " + e.getUsername() + " has been signed in"), t(s), [3, 8];
+                                            return s = l.sent(), o.user = s, $p("signIn", s, "A user " + e.getUsername() + " has been signed in"), t(s), [3, 8];
                                         case 7:
-                                            return u = l.sent(), uh.error("Failed to get the signed in user", u), n(u), [3, 8];
+                                            return u = l.sent(), Jp.error("Failed to get the signed in user", u), n(u), [3, 8];
                                         case 8:
                                             return [7];
                                         case 9:
                                             return [2]
                                     }
                                 }))
                             }))
                         },
                         onFailure: function(t) {
-                            uh.debug("signIn failure", t), dh("signIn_failure", t, e.getUsername() + " failed to signin"), n(t)
+                            Jp.debug("signIn failure", t), $p("signIn_failure", t, e.getUsername() + " failed to signin"), n(t)
                         },
                         customChallenge: function(n) {
-                            uh.debug("signIn custom challenge answer required"), e.challengeName = "CUSTOM_CHALLENGE", e.challengeParam = n, t(e)
+                            Jp.debug("signIn custom challenge answer required"), e.challengeName = "CUSTOM_CHALLENGE", e.challengeParam = n, t(e)
                         },
                         mfaRequired: function(n, r) {
-                            uh.debug("signIn MFA required"), e.challengeName = n, e.challengeParam = r, t(e)
+                            Jp.debug("signIn MFA required"), e.challengeName = n, e.challengeParam = r, t(e)
                         },
                         mfaSetup: function(n, r) {
-                            uh.debug("signIn mfa setup", n), e.challengeName = n, e.challengeParam = r, t(e)
+                            Jp.debug("signIn mfa setup", n), e.challengeName = n, e.challengeParam = r, t(e)
                         },
                         newPasswordRequired: function(n, r) {
-                            uh.debug("signIn new password"), e.challengeName = "NEW_PASSWORD_REQUIRED", e.challengeParam = {
+                            Jp.debug("signIn new password"), e.challengeName = "NEW_PASSWORD_REQUIRED", e.challengeParam = {
                                 userAttributes: n,
                                 requiredAttributes: r
                             }, t(e)
                         },
                         totpRequired: function(n, r) {
-                            uh.debug("signIn totpRequired"), e.challengeName = n, e.challengeParam = r, t(e)
+                            Jp.debug("signIn totpRequired"), e.challengeName = n, e.challengeParam = r, t(e)
                         },
                         selectMFAType: function(n, r) {
-                            uh.debug("signIn selectMFAType", n), e.challengeName = n, e.challengeParam = r, t(e)
+                            Jp.debug("signIn selectMFAType", n), e.challengeName = n, e.challengeParam = r, t(e)
                         }
                     }
                 }, e.prototype.signInWithPassword = function(e) {
                     var t = this;
                     if (this.pendingSignIn) throw new Error("Pending sign-in attempt already in progress");
                     var n = this.createCognitoUser(e.getUsername());
                     return this.pendingSignIn = new Promise((function(r, o) {
@@ -66984,32 +64432,32 @@
                         n = this.createCognitoUser(e.getUsername());
                     return n.setAuthenticationFlowType("CUSTOM_AUTH"), new Promise((function(r, o) {
                         n.initiateAuth(e, t.authCallbacks(n, r, o))
                     }))
                 }, e.prototype.getMFAOptions = function(e) {
                     return new Promise((function(t, n) {
                         e.getMFAOptions((function(e, r) {
-                            if (e) return uh.debug("get MFA Options failed", e), void n(e);
-                            uh.debug("get MFA options success", r), t(r)
+                            if (e) return Jp.debug("get MFA Options failed", e), void n(e);
+                            Jp.debug("get MFA options success", r), t(r)
                         }))
                     }))
                 }, e.prototype.getPreferredMFA = function(e, t) {
                     var n = this,
                         r = this;
                     return new Promise((function(o, i) {
                         var a = n._config.clientMetadata,
                             s = !!t && t.bypassCache;
                         e.getUserData((function(t, a) {
-                            return hs(n, void 0, void 0, (function() {
+                            return ns(n, void 0, void 0, (function() {
                                 var n, s;
-                                return gs(this, (function(u) {
+                                return rs(this, (function(u) {
                                     switch (u.label) {
                                         case 0:
                                             if (!t) return [3, 5];
-                                            if (uh.debug("getting preferred mfa failed", t), !this.isSessionInvalid(t)) return [3, 4];
+                                            if (Jp.debug("getting preferred mfa failed", t), !this.isSessionInvalid(t)) return [3, 4];
                                             u.label = 1;
                                         case 1:
                                             return u.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                         case 2:
                                             return u.sent(), [3, 4];
                                         case 3:
                                             return n = u.sent(), i(new Error("Session is invalid due to: " + t.message + " and failed to clean up invalid session: " + n.message)), [2];
@@ -67027,29 +64475,29 @@
                     }))
                 }, e.prototype._getMfaTypeFromUserData = function(e) {
                     var t = null,
                         n = e.PreferredMfaSetting;
                     if (n) t = n;
                     else {
                         var r = e.UserMFASettingList;
-                        if (r) 0 === r.length ? t = "NOMFA" : uh.debug("invalid case for getPreferredMFA", e);
+                        if (r) 0 === r.length ? t = "NOMFA" : Jp.debug("invalid case for getPreferredMFA", e);
                         else t = e.MFAOptions ? "SMS_MFA" : "NOMFA"
                     }
                     return t
                 }, e.prototype._getUserData = function(e, t) {
                     var n = this;
                     return new Promise((function(r, o) {
                         e.getUserData((function(t, i) {
-                            return hs(n, void 0, void 0, (function() {
+                            return ns(n, void 0, void 0, (function() {
                                 var n;
-                                return gs(this, (function(a) {
+                                return rs(this, (function(a) {
                                     switch (a.label) {
                                         case 0:
                                             if (!t) return [3, 5];
-                                            if (uh.debug("getting user data failed", t), !this.isSessionInvalid(t)) return [3, 4];
+                                            if (Jp.debug("getting user data failed", t), !this.isSessionInvalid(t)) return [3, 4];
                                             a.label = 1;
                                         case 1:
                                             return a.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                         case 2:
                                             return a.sent(), [3, 4];
                                         case 3:
                                             return n = a.sent(), o(new Error("Session is invalid due to: " + t.message + " and failed to clean up invalid session: " + n.message)), [2];
@@ -67061,17 +64509,17 @@
                                             return [2]
                                     }
                                 }))
                             }))
                         }), t)
                     }))
                 }, e.prototype.setPreferredMFA = function(e, t) {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var n, r, o, i, a, s, u = this;
-                        return gs(this, (function(l) {
+                        return rs(this, (function(l) {
                             switch (l.label) {
                                 case 0:
                                     return n = this._config.clientMetadata, [4, this._getUserData(e, {
                                         bypassCache: !0,
                                         clientMetadata: n
                                     })];
                                 case 1:
@@ -67101,15 +64549,15 @@
                                 case 5:
                                     if ("NOMFA" === (s = l.sent())) return [2, Promise.resolve("No change for mfa type")];
                                     if ("SMS_MFA" === s) o = {
                                         PreferredMfa: !1,
                                         Enabled: !1
                                     };
                                     else {
-                                        if ("SOFTWARE_TOKEN_MFA" !== s) return [2, this.rejectAuthError(ds.InvalidMFA)];
+                                        if ("SOFTWARE_TOKEN_MFA" !== s) return [2, this.rejectAuthError($a.InvalidMFA)];
                                         i = {
                                             PreferredMfa: !1,
                                             Enabled: !1
                                         }
                                     }
                                     return a && 0 !== a.length && a.forEach((function(e) {
                                         "SMS_MFA" === e ? o = {
@@ -67117,27 +64565,27 @@
                                             Enabled: !1
                                         } : "SOFTWARE_TOKEN_MFA" === e && (i = {
                                             PreferredMfa: !1,
                                             Enabled: !1
                                         })
                                     })), [3, 7];
                                 case 6:
-                                    return uh.debug("no validmfa method provided"), [2, this.rejectAuthError(ds.NoMFA)];
+                                    return Jp.debug("no validmfa method provided"), [2, this.rejectAuthError($a.NoMFA)];
                                 case 7:
                                     return this, [2, new Promise((function(t, r) {
                                         e.setUserMfaPreference(o, i, (function(o, i) {
-                                            if (o) return uh.debug("Set user mfa preference error", o), r(o);
-                                            uh.debug("Set user mfa success", i), uh.debug("Caching the latest user data into local"), e.getUserData((function(n, o) {
-                                                return hs(u, void 0, void 0, (function() {
+                                            if (o) return Jp.debug("Set user mfa preference error", o), r(o);
+                                            Jp.debug("Set user mfa success", i), Jp.debug("Caching the latest user data into local"), e.getUserData((function(n, o) {
+                                                return ns(u, void 0, void 0, (function() {
                                                     var o;
-                                                    return gs(this, (function(a) {
+                                                    return rs(this, (function(a) {
                                                         switch (a.label) {
                                                             case 0:
                                                                 if (!n) return [3, 5];
-                                                                if (uh.debug("getting user data failed", n), !this.isSessionInvalid(n)) return [3, 4];
+                                                                if (Jp.debug("getting user data failed", n), !this.isSessionInvalid(n)) return [3, 4];
                                                                 a.label = 1;
                                                             case 1:
                                                                 return a.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                                             case 2:
                                                                 return a.sent(), [3, 4];
                                                             case 3:
                                                                 return o = a.sent(), r(new Error("Session is invalid due to: " + n.message + " and failed to clean up invalid session: " + o.message)), [2];
@@ -67156,195 +64604,195 @@
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.disableSMS = function(e) {
                     return new Promise((function(t, n) {
                         e.disableMFA((function(e, r) {
-                            if (e) return uh.debug("disable mfa failed", e), void n(e);
-                            uh.debug("disable mfa succeed", r), t(r)
+                            if (e) return Jp.debug("disable mfa failed", e), void n(e);
+                            Jp.debug("disable mfa succeed", r), t(r)
                         }))
                     }))
                 }, e.prototype.enableSMS = function(e) {
                     return new Promise((function(t, n) {
                         e.enableMFA((function(e, r) {
-                            if (e) return uh.debug("enable mfa failed", e), void n(e);
-                            uh.debug("enable mfa succeed", r), t(r)
+                            if (e) return Jp.debug("enable mfa failed", e), void n(e);
+                            Jp.debug("enable mfa succeed", r), t(r)
                         }))
                     }))
                 }, e.prototype.setupTOTP = function(e) {
                     return new Promise((function(t, n) {
                         e.associateSoftwareToken({
                             onFailure: function(e) {
-                                uh.debug("associateSoftwareToken failed", e), n(e)
+                                Jp.debug("associateSoftwareToken failed", e), n(e)
                             },
                             associateSecretCode: function(e) {
-                                uh.debug("associateSoftwareToken sucess", e), t(e)
+                                Jp.debug("associateSoftwareToken sucess", e), t(e)
                             }
                         })
                     }))
                 }, e.prototype.verifyTotpToken = function(e, t) {
-                    return uh.debug("verification totp token", e, t), new Promise((function(n, r) {
+                    return Jp.debug("verification totp token", e, t), new Promise((function(n, r) {
                         e.verifySoftwareToken(t, "My TOTP device", {
                             onFailure: function(e) {
-                                uh.debug("verifyTotpToken failed", e), r(e)
+                                Jp.debug("verifyTotpToken failed", e), r(e)
                             },
                             onSuccess: function(t) {
-                                dh("signIn", e, "A user " + e.getUsername() + " has been signed in"), dh("verify", e, "A user " + e.getUsername() + " has been verified"), uh.debug("verifyTotpToken success", t), n(t)
+                                $p("signIn", e, "A user " + e.getUsername() + " has been signed in"), $p("verify", e, "A user " + e.getUsername() + " has been verified"), Jp.debug("verifyTotpToken success", t), n(t)
                             }
                         })
                     }))
                 }, e.prototype.confirmSignIn = function(e, t, n, r) {
                     var o = this;
-                    if (void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(ds.EmptyCode);
+                    if (void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError($a.EmptyCode);
                     var i = this;
                     return new Promise((function(a, s) {
                         e.sendMFACode(t, {
                             onSuccess: function(t) {
-                                return hs(o, void 0, void 0, (function() {
+                                return ns(o, void 0, void 0, (function() {
                                     var n, r;
-                                    return gs(this, (function(o) {
+                                    return rs(this, (function(o) {
                                         switch (o.label) {
                                             case 0:
-                                                uh.debug(t), o.label = 1;
+                                                Jp.debug(t), o.label = 1;
                                             case 1:
                                                 return o.trys.push([1, 4, 5, 6]), [4, this.Credentials.clear()];
                                             case 2:
                                                 return o.sent(), [4, this.Credentials.set(t, "session")];
                                             case 3:
-                                                return n = o.sent(), uh.debug("succeed to get cognito credentials", n), [3, 6];
+                                                return n = o.sent(), Jp.debug("succeed to get cognito credentials", n), [3, 6];
                                             case 4:
-                                                return r = o.sent(), uh.debug("cannot get cognito credentials", r), [3, 6];
+                                                return r = o.sent(), Jp.debug("cannot get cognito credentials", r), [3, 6];
                                             case 5:
-                                                return i.user = e, dh("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
+                                                return i.user = e, $p("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
                                             case 6:
                                                 return [2]
                                         }
                                     }))
                                 }))
                             },
                             onFailure: function(e) {
-                                uh.debug("confirm signIn failure", e), s(e)
+                                Jp.debug("confirm signIn failure", e), s(e)
                             }
                         }, n, r)
                     }))
                 }, e.prototype.completeNewPassword = function(e, t, n, r) {
                     var o = this;
-                    if (void 0 === n && (n = {}), void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(ds.EmptyPassword);
+                    if (void 0 === n && (n = {}), void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError($a.EmptyPassword);
                     var i = this;
                     return new Promise((function(a, s) {
                         e.completeNewPasswordChallenge(t, n, {
                             onSuccess: function(t) {
-                                return hs(o, void 0, void 0, (function() {
+                                return ns(o, void 0, void 0, (function() {
                                     var n, r;
-                                    return gs(this, (function(o) {
+                                    return rs(this, (function(o) {
                                         switch (o.label) {
                                             case 0:
-                                                uh.debug(t), o.label = 1;
+                                                Jp.debug(t), o.label = 1;
                                             case 1:
                                                 return o.trys.push([1, 4, 5, 6]), [4, this.Credentials.clear()];
                                             case 2:
                                                 return o.sent(), [4, this.Credentials.set(t, "session")];
                                             case 3:
-                                                return n = o.sent(), uh.debug("succeed to get cognito credentials", n), [3, 6];
+                                                return n = o.sent(), Jp.debug("succeed to get cognito credentials", n), [3, 6];
                                             case 4:
-                                                return r = o.sent(), uh.debug("cannot get cognito credentials", r), [3, 6];
+                                                return r = o.sent(), Jp.debug("cannot get cognito credentials", r), [3, 6];
                                             case 5:
-                                                return i.user = e, dh("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
+                                                return i.user = e, $p("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
                                             case 6:
                                                 return [2]
                                         }
                                     }))
                                 }))
                             },
                             onFailure: function(e) {
-                                uh.debug("completeNewPassword failure", e), dh("completeNewPassword_failure", e, o.user + " failed to complete the new password flow"), s(e)
+                                Jp.debug("completeNewPassword failure", e), $p("completeNewPassword_failure", e, o.user + " failed to complete the new password flow"), s(e)
                             },
                             mfaRequired: function(t, n) {
-                                uh.debug("signIn MFA required"), e.challengeName = t, e.challengeParam = n, a(e)
+                                Jp.debug("signIn MFA required"), e.challengeName = t, e.challengeParam = n, a(e)
                             },
                             mfaSetup: function(t, n) {
-                                uh.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
+                                Jp.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
                             },
                             totpRequired: function(t, n) {
-                                uh.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
+                                Jp.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
                             }
                         }, r)
                     }))
                 }, e.prototype.sendCustomChallengeAnswer = function(e, t, n) {
                     var r = this;
                     if (void 0 === n && (n = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                    if (!t) return this.rejectAuthError(ds.EmptyChallengeResponse);
+                    if (!t) return this.rejectAuthError($a.EmptyChallengeResponse);
                     return new Promise((function(o, i) {
                         e.sendCustomChallengeAnswer(t, r.authCallbacks(e, o, i), n)
                     }))
                 }, e.prototype.deleteUserAttributes = function(e, t) {
                     var n = this;
                     return new Promise((function(r, o) {
                         n.userSession(e).then((function(n) {
                             e.deleteAttributes(t, (function(e, t) {
                                 return e ? o(e) : r(t)
                             }))
                         }))
                     }))
                 }, e.prototype.deleteUser = function() {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var e, t, n = this;
-                        return gs(this, (function(r) {
+                        return rs(this, (function(r) {
                             switch (r.label) {
                                 case 0:
                                     return r.trys.push([0, 2, , 3]), [4, this._storageSync];
                                 case 1:
                                     return r.sent(), [3, 3];
                                 case 2:
-                                    throw e = r.sent(), uh.debug("Failed to sync cache info into memory", e), new Error(e);
+                                    throw e = r.sent(), Jp.debug("Failed to sync cache info into memory", e), new Error(e);
                                 case 3:
                                     return t = this._oAuthHandler && "true" === this._storage.getItem("amplify-signin-with-hostedUI"), [2, new Promise((function(e, r) {
-                                        return hs(n, void 0, void 0, (function() {
+                                        return ns(n, void 0, void 0, (function() {
                                             var n, o = this;
-                                            return gs(this, (function(i) {
+                                            return rs(this, (function(i) {
                                                 if (this.userPool) {
-                                                    if (!(n = this.userPool.getCurrentUser())) return uh.debug("Failed to get user from user pool"), [2, r(new Error("No current user."))];
+                                                    if (!(n = this.userPool.getCurrentUser())) return Jp.debug("Failed to get user from user pool"), [2, r(new Error("No current user."))];
                                                     n.getSession((function(i, a) {
-                                                        return hs(o, void 0, void 0, (function() {
+                                                        return ns(o, void 0, void 0, (function() {
                                                             var o, a = this;
-                                                            return gs(this, (function(s) {
+                                                            return rs(this, (function(s) {
                                                                 switch (s.label) {
                                                                     case 0:
                                                                         if (!i) return [3, 5];
-                                                                        if (uh.debug("Failed to get the user session", i), !this.isSessionInvalid(i)) return [3, 4];
+                                                                        if (Jp.debug("Failed to get the user session", i), !this.isSessionInvalid(i)) return [3, 4];
                                                                         s.label = 1;
                                                                     case 1:
                                                                         return s.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(n)];
                                                                     case 2:
                                                                         return s.sent(), [3, 4];
                                                                     case 3:
                                                                         return o = s.sent(), r(new Error("Session is invalid due to: " + i.message + " and failed to clean up invalid session: " + o.message)), [2];
                                                                     case 4:
                                                                         return [2, r(i)];
                                                                     case 5:
                                                                         n.deleteUser((function(o, i) {
                                                                             if (o) r(o);
                                                                             else {
-                                                                                dh("userDeleted", i, "The authenticated user has been deleted."), n.signOut(), a.user = null;
+                                                                                $p("userDeleted", i, "The authenticated user has been deleted."), n.signOut(), a.user = null;
                                                                                 try {
                                                                                     a.cleanCachedItems()
                                                                                 } catch (s) {
-                                                                                    uh.debug("failed to clear cached items")
+                                                                                    Jp.debug("failed to clear cached items")
                                                                                 }
-                                                                                t ? a.oAuthSignOutRedirect(e, r) : (dh("signOut", a.user, "A user has been signed out"), e(i))
+                                                                                t ? a.oAuthSignOutRedirect(e, r) : ($p("signOut", a.user, "A user has been signed out"), e(i))
                                                                             }
                                                                         })), s.label = 6;
                                                                     case 6:
                                                                         return [2]
                                                                 }
                                                             }))
                                                         }))
                                                     }))
-                                                } else uh.debug("no Congito User pool"), r(new Error("Cognito User pool does not exist"));
+                                                } else Jp.debug("no Congito User pool"), r(new Error("Cognito User pool does not exist"));
                                                 return [2]
                                             }))
                                         }))
                                     }))]
                             }
                         }))
                     }))
@@ -67359,17 +64807,17 @@
                                 if ("sub" !== u && u.indexOf("_verified") < 0) {
                                     var l = {
                                         Name: u,
                                         Value: t[u]
                                     };
                                     o.push(l)
                                 } e.updateAttributes(o, (function(e, n, o) {
-                                if (e) return dh("updateUserAttributes_failure", e, "Failed to update attributes"), s(e);
+                                if (e) return $p("updateUserAttributes_failure", e, "Failed to update attributes"), s(e);
                                 var i = r.createUpdateAttributesResultList(t, null === o || void 0 === o ? void 0 : o.CodeDeliveryDetailsList);
-                                return dh("updateUserAttributes", i, "Attributes successfully updated"), a(n)
+                                return $p("updateUserAttributes", i, "Attributes successfully updated"), a(n)
                             }), n)
                         }))
                     }))
                 }, e.prototype.createUpdateAttributesResultList = function(e, t) {
                     var n = {};
                     return Object.keys(e).forEach((function(e) {
                         n[e] = {
@@ -67413,73 +64861,73 @@
                 }, e.prototype.isRefreshTokenExpiredError = function(e) {
                     return this.isErrorWithMessage(e) && "Refresh Token has expired" === e.message
                 }, e.prototype.isSignedInHostedUI = function() {
                     return this._oAuthHandler && "true" === this._storage.getItem("amplify-signin-with-hostedUI")
                 }, e.prototype.isSessionInvalid = function(e) {
                     return this.isUserDisabledError(e) || this.isUserDoesNotExistError(e) || this.isTokenRevokedError(e) || this.isRefreshTokenRevokedError(e) || this.isRefreshTokenExpiredError(e)
                 }, e.prototype.cleanUpInvalidSession = function(e) {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var t = this;
-                        return gs(this, (function(n) {
+                        return rs(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     e.signOut(), this.user = null, n.label = 1;
                                 case 1:
                                     return n.trys.push([1, 3, , 4]), [4, this.cleanCachedItems()];
                                 case 2:
                                     return n.sent(), [3, 4];
                                 case 3:
-                                    return n.sent(), uh.debug("failed to clear cached items"), [3, 4];
+                                    return n.sent(), Jp.debug("failed to clear cached items"), [3, 4];
                                 case 4:
                                     return this.isSignedInHostedUI() ? [2, new Promise((function(e, n) {
                                         t.oAuthSignOutRedirect(e, n)
-                                    }))] : (dh("signOut", this.user, "A user has been signed out"), [2])
+                                    }))] : ($p("signOut", this.user, "A user has been signed out"), [2])
                             }
                         }))
                     }))
                 }, e.prototype.currentUserPoolUser = function(e) {
                     var t = this;
                     return this.userPool ? new Promise((function(n, r) {
                         t._storageSync.then((function() {
-                            return hs(t, void 0, void 0, (function() {
+                            return ns(t, void 0, void 0, (function() {
                                 var t, o, i, a, s, u, l = this;
-                                return gs(this, (function(c) {
+                                return rs(this, (function(c) {
                                     switch (c.label) {
                                         case 0:
-                                            return this.isOAuthInProgress() ? (uh.debug("OAuth signIn in progress, waiting for resolution..."), [4, new Promise((function(e) {
+                                            return this.isOAuthInProgress() ? (Jp.debug("OAuth signIn in progress, waiting for resolution..."), [4, new Promise((function(e) {
                                                 var t = setTimeout((function() {
-                                                    uh.debug("OAuth signIn in progress timeout"), _s.remove("auth", n), e()
+                                                    Jp.debug("OAuth signIn in progress timeout"), bs.remove("auth", n), e()
                                                 }), 1e4);
 
                                                 function n(r) {
                                                     var o = r.payload.event;
-                                                    "cognitoHostedUI" !== o && "cognitoHostedUI_failure" !== o || (uh.debug("OAuth signIn resolved: " + o), clearTimeout(t), _s.remove("auth", n), e())
+                                                    "cognitoHostedUI" !== o && "cognitoHostedUI_failure" !== o || (Jp.debug("OAuth signIn resolved: " + o), clearTimeout(t), bs.remove("auth", n), e())
                                                 }
-                                                _s.listen("auth", n)
+                                                bs.listen("auth", n)
                                             }))]) : [3, 2];
                                         case 1:
                                             c.sent(), c.label = 2;
                                         case 2:
-                                            if (!(t = this.userPool.getCurrentUser())) return uh.debug("Failed to get user from user pool"), r("No current user"), [2];
+                                            if (!(t = this.userPool.getCurrentUser())) return Jp.debug("Failed to get user from user pool"), r("No current user"), [2];
                                             c.label = 3;
                                         case 3:
                                             return c.trys.push([3, 7, , 8]), [4, this._userSession(t)];
                                         case 4:
                                             return o = c.sent(), (i = !!e && e.bypassCache) ? [4, this.Credentials.clear()] : [3, 6];
                                         case 5:
                                             c.sent(), c.label = 6;
                                         case 6:
-                                            return a = this._config.clientMetadata, s = o.getAccessToken().decodePayload().scope, (void 0 === s ? "" : s).split(" ").includes(lh) ? (t.getUserData((function(e, o) {
-                                                return hs(l, void 0, void 0, (function() {
+                                            return a = this._config.clientMetadata, s = o.getAccessToken().decodePayload().scope, (void 0 === s ? "" : s).split(" ").includes(Kp) ? (t.getUserData((function(e, o) {
+                                                return ns(l, void 0, void 0, (function() {
                                                     var i, a, s, u, l, c, d;
-                                                    return gs(this, (function(f) {
+                                                    return rs(this, (function(f) {
                                                         switch (f.label) {
                                                             case 0:
                                                                 if (!e) return [3, 7];
-                                                                if (uh.debug("getting user data failed", e), !this.isSessionInvalid(e)) return [3, 5];
+                                                                if (Jp.debug("getting user data failed", e), !this.isSessionInvalid(e)) return [3, 5];
                                                                 f.label = 1;
                                                             case 1:
                                                                 return f.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(t)];
                                                             case 2:
                                                                 return f.sent(), [3, 4];
                                                             case 3:
                                                                 return i = f.sent(), r(new Error("Session is invalid due to: " + e.message + " and failed to clean up invalid session: " + i.message)), [2];
@@ -67489,114 +64937,114 @@
                                                                 n(t), f.label = 6;
                                                             case 6:
                                                                 return [2];
                                                             case 7:
                                                                 for (a = o.PreferredMfaSetting || "NOMFA", s = [], u = 0; u < o.UserAttributes.length; u++) l = {
                                                                     Name: o.UserAttributes[u].Name,
                                                                     Value: o.UserAttributes[u].Value
-                                                                }, c = new Lp(l), s.push(c);
+                                                                }, c = new yp(l), s.push(c);
                                                                 return d = this.attributesToObject(s), Object.assign(t, {
                                                                     attributes: d,
                                                                     preferredMFA: a
                                                                 }), [2, n(t)]
                                                         }
                                                     }))
                                                 }))
                                             }), {
                                                 bypassCache: i,
                                                 clientMetadata: a
-                                            }), [3, 8]) : (uh.debug("Unable to get the user data because the " + lh + " is not in the scopes of the access token"), [2, n(t)]);
+                                            }), [3, 8]) : (Jp.debug("Unable to get the user data because the " + Kp + " is not in the scopes of the access token"), [2, n(t)]);
                                         case 7:
                                             return u = c.sent(), r(u), [3, 8];
                                         case 8:
                                             return [2]
                                     }
                                 }))
                             }))
                         })).catch((function(e) {
-                            return uh.debug("Failed to sync cache info into memory", e), r(e)
+                            return Jp.debug("Failed to sync cache info into memory", e), r(e)
                         }))
                     })) : this.rejectNoUserPool()
                 }, e.prototype.isOAuthInProgress = function() {
                     return this.oAuthFlowInProgress
                 }, e.prototype.currentAuthenticatedUser = function(e) {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var t, n, r, o, i;
-                        return gs(this, (function(a) {
+                        return rs(this, (function(a) {
                             switch (a.label) {
                                 case 0:
-                                    uh.debug("getting current authenticated user"), t = null, a.label = 1;
+                                    Jp.debug("getting current authenticated user"), t = null, a.label = 1;
                                 case 1:
                                     return a.trys.push([1, 3, , 4]), [4, this._storageSync];
                                 case 2:
                                     return a.sent(), [3, 4];
                                 case 3:
-                                    throw n = a.sent(), uh.debug("Failed to sync cache info into memory", n), n;
+                                    throw n = a.sent(), Jp.debug("Failed to sync cache info into memory", n), n;
                                 case 4:
                                     try {
-                                        (r = JSON.parse(this._storage.getItem("aws-amplify-federatedInfo"))) && (t = ps(ps({}, r.user), {
+                                        (r = JSON.parse(this._storage.getItem("aws-amplify-federatedInfo"))) && (t = ts(ts({}, r.user), {
                                             token: r.token
                                         }))
                                     } catch (s) {
-                                        uh.debug("cannot load federated user from auth storage")
+                                        Jp.debug("cannot load federated user from auth storage")
                                     }
-                                    return t ? (this.user = t, uh.debug("get current authenticated federated user", this.user), [2, this.user]) : [3, 5];
+                                    return t ? (this.user = t, Jp.debug("get current authenticated federated user", this.user), [2, this.user]) : [3, 5];
                                 case 5:
-                                    uh.debug("get current authenticated userpool user"), o = null, a.label = 6;
+                                    Jp.debug("get current authenticated userpool user"), o = null, a.label = 6;
                                 case 6:
                                     return a.trys.push([6, 8, , 9]), [4, this.currentUserPoolUser(e)];
                                 case 7:
                                     return o = a.sent(), [3, 9];
                                 case 8:
-                                    return "No userPool" === (i = a.sent()) && uh.error("Cannot get the current user because the user pool is missing. Please make sure the Auth module is configured with a valid Cognito User Pool ID"), uh.debug("The user is not authenticated by the error", i), [2, Promise.reject("The user is not authenticated")];
+                                    return "No userPool" === (i = a.sent()) && Jp.error("Cannot get the current user because the user pool is missing. Please make sure the Auth module is configured with a valid Cognito User Pool ID"), Jp.debug("The user is not authenticated by the error", i), [2, Promise.reject("The user is not authenticated")];
                                 case 9:
                                     return this.user = o, [2, this.user]
                             }
                         }))
                     }))
                 }, e.prototype.currentSession = function() {
                     var e = this;
-                    return uh.debug("Getting current session"), this.userPool ? new Promise((function(t, n) {
+                    return Jp.debug("Getting current session"), this.userPool ? new Promise((function(t, n) {
                         e.currentUserPoolUser().then((function(r) {
                             e.userSession(r).then((function(e) {
                                 t(e)
                             })).catch((function(e) {
-                                uh.debug("Failed to get the current session", e), n(e)
+                                Jp.debug("Failed to get the current session", e), n(e)
                             }))
                         })).catch((function(e) {
-                            uh.debug("Failed to get the current user", e), n(e)
+                            Jp.debug("Failed to get the current user", e), n(e)
                         }))
                     })) : Promise.reject(new Error("No User Pool in the configuration."))
                 }, e.prototype._userSession = function(e) {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var t, n, r = this;
-                        return gs(this, (function(o) {
+                        return rs(this, (function(o) {
                             switch (o.label) {
                                 case 0:
-                                    if (!e) return uh.debug("the user is null"), [2, this.rejectAuthError(ds.NoUserSession)];
+                                    if (!e) return Jp.debug("the user is null"), [2, this.rejectAuthError($a.NoUserSession)];
                                     t = this._config.clientMetadata, 0 === this.inflightSessionPromiseCounter && (this.inflightSessionPromise = new Promise((function(n, o) {
                                         e.getSession((function(t, i) {
-                                            return hs(r, void 0, void 0, (function() {
+                                            return ns(r, void 0, void 0, (function() {
                                                 var r;
-                                                return gs(this, (function(a) {
+                                                return rs(this, (function(a) {
                                                     switch (a.label) {
                                                         case 0:
                                                             if (!t) return [3, 5];
-                                                            if (uh.debug("Failed to get the session from user", e), !this.isSessionInvalid(t)) return [3, 4];
+                                                            if (Jp.debug("Failed to get the session from user", e), !this.isSessionInvalid(t)) return [3, 4];
                                                             a.label = 1;
                                                         case 1:
                                                             return a.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                                         case 2:
                                                             return a.sent(), [3, 4];
                                                         case 3:
                                                             return r = a.sent(), o(new Error("Session is invalid due to: " + t.message + " and failed to clean up invalid session: " + r.message)), [2];
                                                         case 4:
                                                             return o(t), [2];
                                                         case 5:
-                                                            return uh.debug("Succeed to get the user session", i), n(i), [2]
+                                                            return Jp.debug("Succeed to get the user session", i), n(i), [2]
                                                     }
                                                 }))
                                             }))
                                         }), {
                                             clientMetadata: t
                                         })
                                     }))), this.inflightSessionPromiseCounter++, o.label = 1;
@@ -67610,43 +65058,43 @@
                                     return [2]
                             }
                         }))
                     }))
                 }, e.prototype.userSession = function(e) {
                     return this._userSession(e)
                 }, e.prototype.currentUserCredentials = function() {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var e, t, n = this;
-                        return gs(this, (function(r) {
+                        return rs(this, (function(r) {
                             switch (r.label) {
                                 case 0:
-                                    uh.debug("Getting current user credentials"), r.label = 1;
+                                    Jp.debug("Getting current user credentials"), r.label = 1;
                                 case 1:
                                     return r.trys.push([1, 3, , 4]), [4, this._storageSync];
                                 case 2:
                                     return r.sent(), [3, 4];
                                 case 3:
-                                    throw e = r.sent(), uh.debug("Failed to sync cache info into memory", e), e;
+                                    throw e = r.sent(), Jp.debug("Failed to sync cache info into memory", e), e;
                                 case 4:
                                     t = null;
                                     try {
                                         t = JSON.parse(this._storage.getItem("aws-amplify-federatedInfo"))
                                     } catch (o) {
-                                        uh.debug("failed to get or parse item aws-amplify-federatedInfo", o)
+                                        Jp.debug("failed to get or parse item aws-amplify-federatedInfo", o)
                                     }
                                     return t ? [2, this.Credentials.refreshFederatedToken(t)] : [2, this.currentSession().then((function(e) {
-                                        return uh.debug("getting session success", e), n.Credentials.set(e, "session")
+                                        return Jp.debug("getting session success", e), n.Credentials.set(e, "session")
                                     })).catch((function() {
-                                        return uh.debug("getting guest credentials"), n.Credentials.set(null, "guest")
+                                        return Jp.debug("getting guest credentials"), n.Credentials.set(null, "guest")
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.currentCredentials = function() {
-                    return uh.debug("getting current credentials"), this.Credentials.get()
+                    return Jp.debug("getting current credentials"), this.Credentials.get()
                 }, e.prototype.verifyUserAttribute = function(e, t, n) {
                     return void 0 === n && (n = this._config.clientMetadata), new Promise((function(r, o) {
                         e.getAttributeVerificationCode(t, {
                             onSuccess: function(e) {
                                 return r(e)
                             },
                             onFailure: function(e) {
@@ -67660,289 +65108,289 @@
                             onSuccess: function(e) {
                                 r(e)
                             },
                             onFailure: function(e) {
                                 o(e)
                             }
                         })
-                    })) : this.rejectAuthError(ds.EmptyCode)
+                    })) : this.rejectAuthError($a.EmptyCode)
                 }, e.prototype.verifyCurrentUserAttribute = function(e) {
                     var t = this;
                     return t.currentUserPoolUser().then((function(n) {
                         return t.verifyUserAttribute(n, e)
                     }))
                 }, e.prototype.verifyCurrentUserAttributeSubmit = function(e, t) {
                     var n = this;
                     return n.currentUserPoolUser().then((function(r) {
                         return n.verifyUserAttributeSubmit(r, e, t)
                     }))
                 }, e.prototype.cognitoIdentitySignOut = function(e, t) {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var n, r, o = this;
-                        return gs(this, (function(i) {
+                        return rs(this, (function(i) {
                             switch (i.label) {
                                 case 0:
                                     return i.trys.push([0, 2, , 3]), [4, this._storageSync];
                                 case 1:
                                     return i.sent(), [3, 3];
                                 case 2:
-                                    throw n = i.sent(), uh.debug("Failed to sync cache info into memory", n), n;
+                                    throw n = i.sent(), Jp.debug("Failed to sync cache info into memory", n), n;
                                 case 3:
                                     return r = this._oAuthHandler && "true" === this._storage.getItem("amplify-signin-with-hostedUI"), [2, new Promise((function(n, i) {
                                         if (e && e.global) {
-                                            uh.debug("user global sign out", t);
+                                            Jp.debug("user global sign out", t);
                                             var a = o._config.clientMetadata;
                                             t.getSession((function(e, a) {
-                                                return hs(o, void 0, void 0, (function() {
+                                                return ns(o, void 0, void 0, (function() {
                                                     var o, a = this;
-                                                    return gs(this, (function(s) {
+                                                    return rs(this, (function(s) {
                                                         switch (s.label) {
                                                             case 0:
                                                                 if (!e) return [3, 5];
-                                                                if (uh.debug("failed to get the user session", e), !this.isSessionInvalid(e)) return [3, 4];
+                                                                if (Jp.debug("failed to get the user session", e), !this.isSessionInvalid(e)) return [3, 4];
                                                                 s.label = 1;
                                                             case 1:
                                                                 return s.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(t)];
                                                             case 2:
                                                                 return s.sent(), [3, 4];
                                                             case 3:
                                                                 return o = s.sent(), i(new Error("Session is invalid due to: " + e.message + " and failed to clean up invalid session: " + o.message)), [2];
                                                             case 4:
                                                                 return [2, i(e)];
                                                             case 5:
                                                                 return t.globalSignOut({
                                                                     onSuccess: function(e) {
-                                                                        if (uh.debug("global sign out success"), !r) return n();
+                                                                        if (Jp.debug("global sign out success"), !r) return n();
                                                                         a.oAuthSignOutRedirect(n, i)
                                                                     },
                                                                     onFailure: function(e) {
-                                                                        return uh.debug("global sign out failed", e), i(e)
+                                                                        return Jp.debug("global sign out failed", e), i(e)
                                                                     }
                                                                 }), [2]
                                                         }
                                                     }))
                                                 }))
                                             }), {
                                                 clientMetadata: a
                                             })
-                                        } else uh.debug("user sign out", t), t.signOut((function() {
+                                        } else Jp.debug("user sign out", t), t.signOut((function() {
                                             if (!r) return n();
                                             o.oAuthSignOutRedirect(n, i)
                                         }))
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.oAuthSignOutRedirect = function(e, t) {
-                    zs().isBrowser ? this.oAuthSignOutRedirectOrReject(t) : this.oAuthSignOutAndResolve(e)
+                    Ns().isBrowser ? this.oAuthSignOutRedirectOrReject(t) : this.oAuthSignOutAndResolve(e)
                 }, e.prototype.oAuthSignOutAndResolve = function(e) {
                     this._oAuthHandler.signOut(), e()
                 }, e.prototype.oAuthSignOutRedirectOrReject = function(e) {
                     this._oAuthHandler.signOut(), setTimeout((function() {
                         return e(Error("Signout timeout fail"))
                     }), 3e3)
                 }, e.prototype.signOut = function(e) {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var t;
-                        return gs(this, (function(n) {
+                        return rs(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return n.trys.push([0, 2, , 3]), [4, this.cleanCachedItems()];
                                 case 1:
                                     return n.sent(), [3, 3];
                                 case 2:
-                                    return n.sent(), uh.debug("failed to clear cached items"), [3, 3];
+                                    return n.sent(), Jp.debug("failed to clear cached items"), [3, 3];
                                 case 3:
                                     return this.userPool ? (t = this.userPool.getCurrentUser()) ? [4, this.cognitoIdentitySignOut(e, t)] : [3, 5] : [3, 7];
                                 case 4:
                                     return n.sent(), [3, 6];
                                 case 5:
-                                    uh.debug("no current Cognito user"), n.label = 6;
+                                    Jp.debug("no current Cognito user"), n.label = 6;
                                 case 6:
                                     return [3, 8];
                                 case 7:
-                                    uh.debug("no Cognito User pool"), n.label = 8;
+                                    Jp.debug("no Cognito User pool"), n.label = 8;
                                 case 8:
-                                    return dh("signOut", this.user, "A user has been signed out"), this.user = null, [2]
+                                    return $p("signOut", this.user, "A user has been signed out"), this.user = null, [2]
                             }
                         }))
                     }))
                 }, e.prototype.cleanCachedItems = function() {
-                    return hs(this, void 0, void 0, (function() {
-                        return gs(this, (function(e) {
+                    return ns(this, void 0, void 0, (function() {
+                        return rs(this, (function(e) {
                             switch (e.label) {
                                 case 0:
                                     return [4, this.Credentials.clear()];
                                 case 1:
                                     return e.sent(), [2]
                             }
                         }))
                     }))
                 }, e.prototype.changePassword = function(e, t, n, r) {
                     var o = this;
                     return void 0 === r && (r = this._config.clientMetadata), new Promise((function(i, a) {
                         o.userSession(e).then((function(o) {
                             e.changePassword(t, n, (function(e, t) {
-                                return e ? (uh.debug("change password failure", e), a(e)) : i(t)
+                                return e ? (Jp.debug("change password failure", e), a(e)) : i(t)
                             }), r)
                         }))
                     }))
                 }, e.prototype.forgotPassword = function(e, t) {
                     if (void 0 === t && (t = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                    if (!e) return this.rejectAuthError(ds.EmptyUsername);
+                    if (!e) return this.rejectAuthError($a.EmptyUsername);
                     var n = this.createCognitoUser(e);
                     return new Promise((function(r, o) {
                         n.forgotPassword({
                             onSuccess: function() {
                                 r()
                             },
                             onFailure: function(t) {
-                                uh.debug("forgot password failure", t), dh("forgotPassword_failure", t, e + " forgotPassword failed"), o(t)
+                                Jp.debug("forgot password failure", t), $p("forgotPassword_failure", t, e + " forgotPassword failed"), o(t)
                             },
                             inputVerificationCode: function(t) {
-                                dh("forgotPassword", n, e + " has initiated forgot password flow"), r(t)
+                                $p("forgotPassword", n, e + " has initiated forgot password flow"), r(t)
                             }
                         }, t)
                     }))
                 }, e.prototype.forgotPasswordSubmit = function(e, t, n, r) {
                     if (void 0 === r && (r = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                    if (!e) return this.rejectAuthError(ds.EmptyUsername);
-                    if (!t) return this.rejectAuthError(ds.EmptyCode);
-                    if (!n) return this.rejectAuthError(ds.EmptyPassword);
+                    if (!e) return this.rejectAuthError($a.EmptyUsername);
+                    if (!t) return this.rejectAuthError($a.EmptyCode);
+                    if (!n) return this.rejectAuthError($a.EmptyPassword);
                     var o = this.createCognitoUser(e);
                     return new Promise((function(i, a) {
                         o.confirmPassword(t, n, {
                             onSuccess: function(t) {
-                                dh("forgotPasswordSubmit", o, e + " forgotPasswordSubmit successful"), i(t)
+                                $p("forgotPasswordSubmit", o, e + " forgotPasswordSubmit successful"), i(t)
                             },
                             onFailure: function(t) {
-                                dh("forgotPasswordSubmit_failure", t, e + " forgotPasswordSubmit failed"), a(t)
+                                $p("forgotPasswordSubmit_failure", t, e + " forgotPasswordSubmit failed"), a(t)
                             }
                         }, r)
                     }))
                 }, e.prototype.currentUserInfo = function() {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var e, t, n, r, o, i, a;
-                        return gs(this, (function(s) {
+                        return rs(this, (function(s) {
                             switch (s.label) {
                                 case 0:
                                     return (e = this.Credentials.getCredSource()) && "aws" !== e && "userPool" !== e ? [3, 9] : [4, this.currentUserPoolUser().catch((function(e) {
-                                        return uh.error(e)
+                                        return Jp.error(e)
                                     }))];
                                 case 1:
                                     if (!(a = s.sent())) return [2, null];
                                     s.label = 2;
                                 case 2:
                                     return s.trys.push([2, 8, , 9]), [4, this.userAttributes(a)];
                                 case 3:
                                     t = s.sent(), n = this.attributesToObject(t), r = null, s.label = 4;
                                 case 4:
                                     return s.trys.push([4, 6, , 7]), [4, this.currentCredentials()];
                                 case 5:
                                     return r = s.sent(), [3, 7];
                                 case 6:
-                                    return o = s.sent(), uh.debug("Failed to retrieve credentials while getting current user info", o), [3, 7];
+                                    return o = s.sent(), Jp.debug("Failed to retrieve credentials while getting current user info", o), [3, 7];
                                 case 7:
                                     return [2, {
                                         id: r ? r.identityId : void 0,
                                         username: a.getUsername(),
                                         attributes: n
                                     }];
                                 case 8:
-                                    return i = s.sent(), uh.error("currentUserInfo error", i), [2, {}];
+                                    return i = s.sent(), Jp.error("currentUserInfo error", i), [2, {}];
                                 case 9:
                                     return "federated" === e ? [2, (a = this.user) || {}] : [2]
                             }
                         }))
                     }))
                 }, e.prototype.federatedSignIn = function(e, t, n) {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var r, o, i, a, s, u, l, c, d, f, p;
-                        return gs(this, (function(h) {
+                        return rs(this, (function(h) {
                             switch (h.label) {
                                 case 0:
                                     if (!this._config.identityPoolId && !this._config.userPoolId) throw new Error("Federation requires either a User Pool or Identity Pool in config");
                                     if ("undefined" === typeof e && this._config.identityPoolId && !this._config.userPoolId) throw new Error("Federation with Identity Pools requires tokens passed as arguments");
-                                    return ms(e) || (g = e) && ["customProvider"].find((function(e) {
+                                    return is(e) || (g = e) && ["customProvider"].find((function(e) {
                                         return g.hasOwnProperty(e)
                                     })) || function(e) {
                                         return e && !!["customState"].find((function(t) {
                                             return e.hasOwnProperty(t)
                                         }))
                                     }(e) || "undefined" === typeof e ? (r = e || {
-                                        provider: cs.Cognito
-                                    }, s = ms(r) ? r.provider : r.customProvider, ms(r), o = r.customState, this._config.userPoolId && (i = vs(this._config.oauth) ? this._config.userPoolWebClientId : this._config.oauth.clientID, a = vs(this._config.oauth) ? this._config.oauth.redirectSignIn : this._config.oauth.redirectUri, this._oAuthHandler.oauthSignIn(this._config.oauth.responseType, this._config.oauth.domain, a, i, s, o)), [3, 4]) : [3, 1];
+                                        provider: Xa.Cognito
+                                    }, s = is(r) ? r.provider : r.customProvider, is(r), o = r.customState, this._config.userPoolId && (i = as(this._config.oauth) ? this._config.userPoolWebClientId : this._config.oauth.clientID, a = as(this._config.oauth) ? this._config.oauth.redirectSignIn : this._config.oauth.redirectUri, this._oAuthHandler.oauthSignIn(this._config.oauth.responseType, this._config.oauth.domain, a, i, s, o)), [3, 4]) : [3, 1];
                                 case 1:
                                     s = e;
                                     try {
-                                        (u = JSON.stringify(JSON.parse(this._storage.getItem("aws-amplify-federatedInfo")).user)) && uh.warn("There is already a signed in user: " + u + " in your app.\n\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\tYou should not call Auth.federatedSignIn method again as it may cause unexpected behavior.")
+                                        (u = JSON.stringify(JSON.parse(this._storage.getItem("aws-amplify-federatedInfo")).user)) && Jp.warn("There is already a signed in user: " + u + " in your app.\n\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\tYou should not call Auth.federatedSignIn method again as it may cause unexpected behavior.")
                                     } catch (y) {}
                                     return l = t.token, c = t.identity_id, d = t.expires_at, [4, this.Credentials.set({
                                         provider: s,
                                         token: l,
                                         identity_id: c,
                                         user: n,
                                         expires_at: d
                                     }, "federation")];
                                 case 2:
                                     return f = h.sent(), [4, this.currentAuthenticatedUser()];
                                 case 3:
-                                    return p = h.sent(), dh("signIn", p, "A user " + p.username + " has been signed in"), uh.debug("federated sign in credentials", f), [2, f];
+                                    return p = h.sent(), $p("signIn", p, "A user " + p.username + " has been signed in"), Jp.debug("federated sign in credentials", f), [2, f];
                                 case 4:
                                     return [2]
                             }
                             var g
                         }))
                     }))
                 }, e.prototype._handleAuthResponse = function(e) {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var t, n, r, o, i, a, s, u, l, c, d, f, p, h;
-                        return gs(this, (function(g) {
+                        return rs(this, (function(g) {
                             switch (g.label) {
                                 case 0:
-                                    if (this.oAuthFlowInProgress) return uh.debug("Skipping URL " + e + " current flow in progress"), [2];
+                                    if (this.oAuthFlowInProgress) return Jp.debug("Skipping URL " + e + " current flow in progress"), [2];
                                     g.label = 1;
                                 case 1:
                                     if (g.trys.push([1, , 8, 9]), this.oAuthFlowInProgress = !0, !this._config.userPoolId) throw new Error("OAuth responses require a User Pool defined in config");
-                                    if (dh("parsingCallbackUrl", {
+                                    if ($p("parsingCallbackUrl", {
                                             url: e
-                                        }, "The callback url is being parsed"), t = e || (zs().isBrowser ? window.location.href : ""), n = !!((0, Kp.Qc)(t).query || "").split("&").map((function(e) {
+                                        }, "The callback url is being parsed"), t = e || (Ns().isBrowser ? window.location.href : ""), n = !!((0, Rp.Qc)(t).query || "").split("&").map((function(e) {
                                             return e.split("=")
                                         })).find((function(e) {
-                                            var t = ys(e, 1)[0];
+                                            var t = os(e, 1)[0];
                                             return "code" === t || "error" === t
-                                        })), r = !!((0, Kp.Qc)(t).hash || "#").substr(1).split("&").map((function(e) {
+                                        })), r = !!((0, Rp.Qc)(t).hash || "#").substr(1).split("&").map((function(e) {
                                             return e.split("=")
                                         })).find((function(e) {
-                                            var t = ys(e, 1)[0];
+                                            var t = os(e, 1)[0];
                                             return "access_token" === t || "error" === t
                                         })), !n && !r) return [3, 7];
                                     this._storage.setItem("amplify-redirected-from-hosted-ui", "true"), g.label = 2;
                                 case 2:
                                     return g.trys.push([2, 6, , 7]), [4, this._oAuthHandler.handleAuthResponse(t)];
                                 case 3:
-                                    return o = g.sent(), i = o.accessToken, a = o.idToken, s = o.refreshToken, u = o.state, l = new Np({
-                                        IdToken: new wp({
+                                    return o = g.sent(), i = o.accessToken, a = o.idToken, s = o.refreshToken, u = o.state, l = new fp({
+                                        IdToken: new lp({
                                             IdToken: a
                                         }),
-                                        RefreshToken: new jp({
+                                        RefreshToken: new cp({
                                             RefreshToken: s
                                         }),
-                                        AccessToken: new Mp({
+                                        AccessToken: new sp({
                                             AccessToken: i
                                         })
                                     }), c = void 0, this._config.identityPoolId ? [4, this.Credentials.set(l, "session")] : [3, 5];
                                 case 4:
-                                    c = g.sent(), uh.debug("AWS credentials", c), g.label = 5;
+                                    c = g.sent(), Jp.debug("AWS credentials", c), g.label = 5;
                                 case 5:
-                                    return d = /-/.test(u), (f = this.createCognitoUser(l.getIdToken().decodePayload()["cognito:username"])).setSignInUserSession(l), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), dh("signIn", f, "A user " + f.getUsername() + " has been signed in"), dh("cognitoHostedUI", f, "A user " + f.getUsername() + " has been signed in via Cognito Hosted UI"), d && (p = u.split("-").splice(1).join("-"), dh("customOAuthState", p.match(/.{2}/g).map((function(e) {
+                                    return d = /-/.test(u), (f = this.createCognitoUser(l.getIdToken().decodePayload()["cognito:username"])).setSignInUserSession(l), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), $p("signIn", f, "A user " + f.getUsername() + " has been signed in"), $p("cognitoHostedUI", f, "A user " + f.getUsername() + " has been signed in via Cognito Hosted UI"), d && (p = u.split("-").splice(1).join("-"), $p("customOAuthState", p.match(/.{2}/g).map((function(e) {
                                         return String.fromCharCode(parseInt(e, 16))
                                     })).join(""), "State for user " + f.getUsername())), [2, c];
                                 case 6:
-                                    return h = g.sent(), uh.debug("Error in cognito hosted auth response", h), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), dh("signIn_failure", h, "The OAuth response flow failed"), dh("cognitoHostedUI_failure", h, "A failure occurred when returning to the Cognito Hosted UI"), dh("customState_failure", h, "A failure occurred when returning state"), [3, 7];
+                                    return h = g.sent(), Jp.debug("Error in cognito hosted auth response", h), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), $p("signIn_failure", h, "The OAuth response flow failed"), $p("cognitoHostedUI_failure", h, "A failure occurred when returning to the Cognito Hosted UI"), $p("customState_failure", h, "A failure occurred when returning state"), [3, 7];
                                 case 7:
                                     return [3, 9];
                                 case 8:
                                     return this.oAuthFlowInProgress = !1, [7];
                                 case 9:
                                     return [2]
                             }
@@ -67967,86 +65415,86 @@
                 }, e.prototype.createCognitoUser = function(e) {
                     var t = {
                         Username: e,
                         Pool: this.userPool
                     };
                     t.Storage = this._storage;
                     var n = this._config.authenticationFlowType,
-                        r = new Tp(t);
+                        r = new wp(t);
                     return n && r.setAuthenticationFlowType(n), r
                 }, e.prototype._isValidAuthStorage = function(e) {
                     return !!e && "function" === typeof e.getItem && "function" === typeof e.setItem && "function" === typeof e.removeItem && "function" === typeof e.clear
                 }, e.prototype.noUserPoolErrorHandler = function(e) {
-                    return !e || e.userPoolId && e.identityPoolId ? ds.NoConfig : ds.MissingAuthConfig
+                    return !e || e.userPoolId && e.identityPoolId ? $a.NoConfig : $a.MissingAuthConfig
                 }, e.prototype.rejectAuthError = function(e) {
-                    return Promise.reject(new ih(e))
+                    return Promise.reject(new Zp(e))
                 }, e.prototype.rejectNoUserPool = function() {
                     var e = this.noUserPoolErrorHandler(this._config);
-                    return Promise.reject(new ah(e))
+                    return Promise.reject(new Vp(e))
                 }, e.prototype.rememberDevice = function() {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var e, t;
-                        return gs(this, (function(n) {
+                        return rs(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return n.trys.push([0, 2, , 3]), [4, this.currentUserPoolUser()];
                                 case 1:
                                     return e = n.sent(), [3, 3];
                                 case 2:
-                                    return t = n.sent(), uh.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
+                                    return t = n.sent(), Jp.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
                                 case 3:
                                     return e.getCachedDeviceKeyAndPassword(), [2, new Promise((function(t, n) {
                                         e.setDeviceStatusRemembered({
                                             onSuccess: function(e) {
                                                 t(e)
                                             },
                                             onFailure: function(e) {
-                                                "InvalidParameterException" === e.code ? n(new ih(ds.DeviceConfig)) : "NetworkError" === e.code ? n(new ih(ds.NetworkError)) : n(e)
+                                                "InvalidParameterException" === e.code ? n(new Zp($a.DeviceConfig)) : "NetworkError" === e.code ? n(new Zp($a.NetworkError)) : n(e)
                                             }
                                         })
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.forgetDevice = function() {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var e, t;
-                        return gs(this, (function(n) {
+                        return rs(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return n.trys.push([0, 2, , 3]), [4, this.currentUserPoolUser()];
                                 case 1:
                                     return e = n.sent(), [3, 3];
                                 case 2:
-                                    return t = n.sent(), uh.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
+                                    return t = n.sent(), Jp.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
                                 case 3:
                                     return e.getCachedDeviceKeyAndPassword(), [2, new Promise((function(t, n) {
                                         e.forgetDevice({
                                             onSuccess: function(e) {
                                                 t(e)
                                             },
                                             onFailure: function(e) {
-                                                "InvalidParameterException" === e.code ? n(new ih(ds.DeviceConfig)) : "NetworkError" === e.code ? n(new ih(ds.NetworkError)) : n(e)
+                                                "InvalidParameterException" === e.code ? n(new Zp($a.DeviceConfig)) : "NetworkError" === e.code ? n(new Zp($a.NetworkError)) : n(e)
                                             }
                                         })
                                     }))]
                             }
                         }))
                     }))
                 }, e.prototype.fetchDevices = function() {
-                    return hs(this, void 0, void 0, (function() {
+                    return ns(this, void 0, void 0, (function() {
                         var e, t;
-                        return gs(this, (function(n) {
+                        return rs(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     return n.trys.push([0, 2, , 3]), [4, this.currentUserPoolUser()];
                                 case 1:
                                     return e = n.sent(), [3, 3];
                                 case 2:
-                                    throw t = n.sent(), uh.debug("The user is not authenticated by the error", t), new Error("The user is not authenticated");
+                                    throw t = n.sent(), Jp.debug("The user is not authenticated by the error", t), new Error("The user is not authenticated");
                                 case 3:
                                     return e.getCachedDeviceKeyAndPassword(), [2, new Promise((function(t, n) {
                                         var r = {
                                             onSuccess: function(e) {
                                                 var n = e.Devices.map((function(e) {
                                                     var t = e.DeviceAttributes.find((function(e) {
                                                         return "device_name" === e.Name
@@ -68055,28 +65503,28 @@
                                                         id: e.DeviceKey,
                                                         name: t.Value
                                                     }
                                                 }));
                                                 t(n)
                                             },
                                             onFailure: function(e) {
-                                                "InvalidParameterException" === e.code ? n(new ih(ds.DeviceConfig)) : "NetworkError" === e.code ? n(new ih(ds.NetworkError)) : n(e)
+                                                "InvalidParameterException" === e.code ? n(new Zp($a.DeviceConfig)) : "NetworkError" === e.code ? n(new Zp($a.NetworkError)) : n(e)
                                             }
                                         };
                                         e.listDevices(60, null, r)
                                     }))]
                             }
                         }))
                     }))
                 }, e
             }(),
-            ph = new fh(null);
-        Js.register(ph);
-        var hh = "#FEFEFE",
-            gh = function(e) {
+            th = new eh(null);
+        Ps.register(th);
+        var nh = "#FEFEFE",
+            rh = function(e) {
                 var t = e.hide,
                     n = pe().environ,
                     r = co(),
                     o = so(zt.Url("/cognito_config", !1), {
                         cache: !0,
                         onData: function(e) {
                             var t = {
@@ -68088,15 +65536,15 @@
                                     domain: e.domain,
                                     scope: e.scope,
                                     prompt: "select_account",
                                     redirectSignIn: e.callback,
                                     responseType: "code"
                                 }
                             };
-                            ph.configure(t)
+                            th.configure(t)
                         }
                     });
                 var i = (0, Fr.jsx)("div", {
                     children: (0, Fr.jsxs)("div", {
                         className: "title-font",
                         style: {
                             marginTop: "4pt",
@@ -68124,52 +65572,52 @@
                 });
                 return (0, Fr.jsx)("div", {
                     style: {
                         transform: "scale(1.1)",
                         marginTop: "10pt",
                         marginBottom: "40pt"
                     },
-                    children: (0, Fr.jsx)(yh, {
+                    children: (0, Fr.jsx)(oh, {
                         links: i,
                         children: o.loading ? (0, Fr.jsx)(Fr.Fragment, {
                             children: (0, Fr.jsx)(No, {
                                 condition: !0,
                                 color: Ft.GetForegroundColor(),
                                 bold: !1,
                                 size: "140px",
                                 label: "Loading configuration "
                             })
                         }) : (0, Fr.jsxs)(Fr.Fragment, {
                             children: [(0, Fr.jsx)("div", {
                                 style: {
                                     paddingTop: "0pt"
                                 }
-                            }), (0, Fr.jsx)(mh, {
+                            }), (0, Fr.jsx)(ih, {
                                 signin: function() {
-                                    bt.Set("env", At.PreferredName(n, r)), bt.Set("signinvia", "Google"), ph.federatedSignIn({
+                                    bt.Set("env", At.PreferredName(n, r)), bt.Set("signinvia", "Google"), th.federatedSignIn({
                                         provider: "Google",
                                         prompt: "select_account"
                                     }, {
                                         prompt: "select_account"
                                     })
                                 }
                             }), (0, Fr.jsx)("div", {
                                 style: {
                                     paddingTop: "6pt"
                                 }
-                            }), (0, Fr.jsx)(vh, {
+                            }), (0, Fr.jsx)(ah, {
                                 signin: function() {
                                     window.alert("Sign in with GitHub via Cognito not supported.")
                                 }
                             })]
                         })
                     })
                 })
             },
-            yh = function(e) {
+            oh = function(e) {
                 var t = e.links,
                     n = e.children;
                 return (0, Fr.jsx)("div", {
                     className: "container",
                     style: {
                         width: "265pt",
                         marginTop: "30pt"
@@ -68180,15 +65628,15 @@
                                 border: "2px solid var(--box-fg)",
                                 padding: "2px 2px 2px 2px",
                                 borderRadius: "6px",
                                 overflow: "hidden"
                             },
                             children: (0, Fr.jsxs)("div", {
                                 style: {
-                                    background: hh,
+                                    background: nh,
                                     border: "1px solid var(--box-fg)",
                                     borderRadius: "6px",
                                     overflow: "hidden"
                                 },
                                 children: [(0, Fr.jsx)("div", {
                                     style: {
                                         background: "var(--box-fg)",
@@ -68213,17 +65661,17 @@
                             })
                         }), t && (0, Fr.jsx)(Fr.Fragment, {
                             children: t
                         })]
                     })
                 })
             },
-            mh = function(e) {
+            ih = function(e) {
                 var t = e.signin;
-                return (0, Fr.jsxs)(Mh, {
+                return (0, Fr.jsxs)(sh, {
                     signin: t,
                     children: [(0, Fr.jsx)("img", {
                         alt: "google",
                         src: Ut.GoogleLoginLogo(),
                         style: {
                             position: "relative",
                             marginTop: "-2px"
@@ -68235,17 +65683,17 @@
                             fontSize: "12pt",
                             marginLeft: "10pt"
                         },
                         children: "Sign in with Google"
                     })]
                 })
             },
-            vh = function(e) {
+            ah = function(e) {
                 var t = e.signin;
-                return (0, Fr.jsxs)(Mh, {
+                return (0, Fr.jsxs)(sh, {
                     signin: t,
                     children: [(0, Fr.jsx)("img", {
                         alt: "github",
                         src: Ut.GitHubLoginLogo(),
                         style: {
                             position: "relative",
                             marginTop: "-2px",
@@ -68258,30 +65706,2829 @@
                             fontSize: "12pt",
                             marginLeft: "7pt"
                         },
                         children: "Sign in with GitHub"
                     })]
                 })
             },
-            Mh = function(e) {
+            sh = function(e) {
                 var t = e.signin,
                     n = e.children;
                 return (0, Fr.jsx)("div", {
                     style: {
-                        background: hh,
+                        background: nh,
                         padding: "0 10pt 0 10pt"
                     },
                     children: (0, Fr.jsx)("button", {
                         className: "signin-as-button",
                         onClick: t,
                         children: n
                     })
                 })
             },
+            uh = function(e) {
+                var t;
+                return null === e || void 0 === e || null === (t = e.portal) || void 0 === t ? void 0 : t.ssl_certificate_error
+            },
+            lh = function(e) {
+                return uh(e.header) ? (0, Fr.jsx)(Fr.Fragment, {
+                    children: (0, Fr.jsx)(ch, {
+                        header: e.header
+                    })
+                }) : (0, Fr.jsx)(Fr.Fragment, {})
+            };
+        lh.IsFatalError = uh;
+        var ch = function(e) {
+                var n = e.header,
+                    r = {
+                        fontSize: "11pt",
+                        color: "darkred",
+                        verticalAlign: "top",
+                        paddingBottom: "3pt",
+                        paddingRight: "10pt"
+                    },
+                    o = a((0, t.useState)(!1), 2),
+                    i = o[0],
+                    s = o[1];
+                return (0, Fr.jsx)(Fr.Fragment, {
+                    children: (0, Fr.jsx)("div", {
+                        className: "container",
+                        style: {
+                            width: "800pt"
+                        },
+                        children: (0, Fr.jsxs)("div", {
+                            className: "box error thickborder",
+                            children: [(0, Fr.jsx)("img", {
+                                src: "https://cdn0.iconfinder.com/data/icons/reject-filled-color/64/reject_cross_cancel_remove_accept_diploma_certificate0-1024.png",
+                                height: "35"
+                            }), (0, Fr.jsx)("b", {
+                                style: {
+                                    fontSize: "16pt",
+                                    marginLeft: "10pt"
+                                },
+                                children: "SSL Certificate Error"
+                            }), (0, Fr.jsx)("br", {}), (0, Fr.jsx)(Ji, {
+                                top: "6pt",
+                                bottom: "6pt",
+                                color: "darkred"
+                            }), "There is a problem with the SSL certificate for the ", (0, Fr.jsx)("b", {
+                                children: "Portal"
+                            }), " associated with this Foursight instance: \xa0", (0, Fr.jsx)("b", {
+                                children: (0, Fr.jsx)("small", {
+                                    children: (0, Fr.jsx)("a", {
+                                        href: n.portal.url,
+                                        style: {
+                                            color: "darkred"
+                                        },
+                                        target: "_blank",
+                                        children: n.portal.url
+                                    })
+                                })
+                            }), " ", (0, Fr.jsx)("br", {}), (0, Fr.jsx)(Ji, {
+                                top: "6pt",
+                                bottom: "6pt",
+                                color: "darkred"
+                            }), (0, Fr.jsxs)("b", {
+                                children: [Do.RightArrow, " ", (0, Fr.jsxs)("small", {
+                                    children: [(0, Fr.jsxs)("i", {
+                                        children: ["You ", (0, Fr.jsx)("u", {
+                                            children: "must"
+                                        }), " contact your system adminstrator to resolve this issue"]
+                                    }), "\xa0\xa0:-("]
+                                })]
+                            }), (0, Fr.jsx)(Ji, {
+                                top: "6pt",
+                                bottom: "6pt",
+                                color: "darkred"
+                            }), (0, Fr.jsx)("table", {
+                                children: (0, Fr.jsxs)("tbody", {
+                                    children: [(0, Fr.jsxs)("tr", {
+                                        children: [(0, Fr.jsx)("td", {
+                                            style: r,
+                                            children: "Hostname:"
+                                        }), (0, Fr.jsx)("td", {
+                                            style: r,
+                                            children: (0, Fr.jsx)("b", {
+                                                children: n.portal.ssl_certificate.hostname
+                                            })
+                                        })]
+                                    }), (0, Fr.jsxs)("tr", {
+                                        children: [(0, Fr.jsx)("td", {
+                                            style: r,
+                                            children: "Owner:"
+                                        }), (0, Fr.jsxs)("td", {
+                                            style: r,
+                                            children: [n.portal.ssl_certificate.owner, n.portal.ssl_certificate.owner_entity && (0, Fr.jsxs)(Fr.Fragment, {
+                                                children: ["\xa0(", n.portal.ssl_certificate.owner_entity, ")"]
+                                            })]
+                                        })]
+                                    }), (0, Fr.jsxs)("tr", {
+                                        children: [(0, Fr.jsx)("td", {
+                                            style: r,
+                                            children: "Issuer:"
+                                        }), (0, Fr.jsxs)("td", {
+                                            style: r,
+                                            children: [n.portal.ssl_certificate.issuer, n.portal.ssl_certificate.issuer_entity && (0, Fr.jsxs)(Fr.Fragment, {
+                                                children: ["\xa0(", n.portal.ssl_certificate.issuer_entity, ")"]
+                                            })]
+                                        })]
+                                    }), (0, Fr.jsxs)("tr", {
+                                        children: [(0, Fr.jsx)("td", {
+                                            style: r,
+                                            children: "Activation Date:"
+                                        }), (0, Fr.jsxs)("td", {
+                                            style: r,
+                                            children: [n.portal.ssl_certificate.active_at, n.portal.ssl_certificate.inactive && (0, Fr.jsxs)("b", {
+                                                style: {
+                                                    color: "darkred"
+                                                },
+                                                children: ["\xa0\xa0", Do.RightArrow, "\xa0\xa0", (0, Fr.jsx)("b", {
+                                                    children: (0, Fr.jsx)("u", {
+                                                        children: "Inactive"
+                                                    })
+                                                }), "\xa0\xa0", Do.LeftArrow]
+                                            })]
+                                        })]
+                                    }), (0, Fr.jsxs)("tr", {
+                                        children: [(0, Fr.jsx)("td", {
+                                            style: r,
+                                            children: "Expiration Date:"
+                                        }), (0, Fr.jsxs)("td", {
+                                            style: r,
+                                            children: [n.portal.ssl_certificate.expires_at, n.portal.ssl_certificate.expired && (0, Fr.jsxs)(Fr.Fragment, {
+                                                children: ["\xa0\xa0", Do.RightArrow, "\xa0\xa0", (0, Fr.jsx)("b", {
+                                                    children: (0, Fr.jsx)("u", {
+                                                        children: "Expired"
+                                                    })
+                                                }), "\xa0\xa0", Do.LeftArrow, "\xa0\xa0", (0, Fr.jsx)("small", {
+                                                    children: Pr.Ago(n.portal.ssl_certificate.expires_at)
+                                                })]
+                                            })]
+                                        })]
+                                    }), (0, Fr.jsxs)("tr", {
+                                        children: [(0, Fr.jsx)("td", {
+                                            style: r,
+                                            children: "Details:"
+                                        }), (0, Fr.jsx)("td", {
+                                            style: r,
+                                            children: i ? (0, Fr.jsx)(Fr.Fragment, {
+                                                children: (0, Fr.jsxs)("span", {
+                                                    onClick: function() {
+                                                        return s(!1)
+                                                    },
+                                                    style: {
+                                                        cursor: "pointer"
+                                                    },
+                                                    children: ["Hide ", Do.DownArrow]
+                                                })
+                                            }) : (0, Fr.jsx)(Fr.Fragment, {
+                                                children: (0, Fr.jsxs)("span", {
+                                                    onClick: function() {
+                                                        return s(!0)
+                                                    },
+                                                    style: {
+                                                        cursor: "pointer"
+                                                    },
+                                                    children: ["Show ", Do.UpArrow]
+                                                })
+                                            })
+                                        })]
+                                    }), i && (0, Fr.jsxs)(Fr.Fragment, {
+                                        children: [(0, Fr.jsxs)("tr", {
+                                            children: [(0, Fr.jsx)("td", {
+                                                style: r,
+                                                children: "Serial Number:"
+                                            }), (0, Fr.jsx)("td", {
+                                                style: r,
+                                                children: n.portal.ssl_certificate.serial_number
+                                            })]
+                                        }), (0, Fr.jsxs)("tr", {
+                                            children: [(0, Fr.jsx)("td", {
+                                                style: r,
+                                                children: "PEM:"
+                                            }), (0, Fr.jsx)("td", {
+                                                style: r,
+                                                children: (0, Fr.jsx)("pre", {
+                                                    style: {
+                                                        background: "inherit",
+                                                        color: "inherit",
+                                                        marginTop: "2pt"
+                                                    },
+                                                    children: n.portal.ssl_certificate.pem
+                                                })
+                                            })]
+                                        })]
+                                    })]
+                                })
+                            })]
+                        })
+                    })
+                })
+            },
+            dh = lh,
+            fh = function(e) {
+                var t, n, r = co(),
+                    o = Va(),
+                    i = so(Br.IsLoggedIn() ? zt.Url("/info") : null);
+                Hr.NoteLastUrl(r);
+                var a = fe();
+
+                function s() {
+                    return At.IsKnown(At.Current(), r)
+                }
+
+                function u(e) {
+                    return At.Equals(At.Current(), e)
+                }
+
+                function l(e) {
+                    return At.IsDefault(e, r)
+                }
+
+                function c() {
+                    return At.PreferredName(At.Default(r), r)
+                }
+
+                function d(e, t) {
+                    var n;
+                    if (!st.IsNonEmptyObject(t)) return "Fetching ...";
+                    var r = null === (n = t.known_envs) || void 0 === n ? void 0 : n.filter((function(t) {
+                        return At.Equals(t, e)
+                    }));
+                    return st.IsNonEmptyArray(r) && r[0].gac_name || "GAC name unknown"
+                }
+
+                function f(e, t) {
+                    var n;
+                    if (!st.IsNonEmptyObject(t)) return !1;
+                    var r = null === (n = t.known_envs) || void 0 === n ? void 0 : n.filter((function(t) {
+                        return At.Equals(t, e)
+                    }));
+                    return st.IsNonEmptyArray(r) && r[0].gac_name
+                }
+                var p = s() && At.IsAllowed(At.Current(), r) ? "box" : "box warning";
+
+                function h(e) {
+                    return {
+                        fontWeight: e === At.Current() ? "bold" : "inherit"
+                    }
+                }
+                return dh.IsFatalError(r) ? (0, Fr.jsx)(dh, {
+                    header: r
+                }) : r.error ? (0, Fr.jsx)(Xi, {
+                    error: r.error,
+                    message: "Error loading users from Foursight API"
+                }) : r.loading ? (0, Fr.jsx)(Fr.Fragment, {
+                    children: "Loading ..."
+                }) : (0, Fr.jsx)("div", {
+                    children: (0, Fr.jsxs)("div", {
+                        className: "container",
+                        children: [!Br.IsLoggedIn(r) && s() ? (0, Fr.jsxs)("div", {
+                            className: "box warning",
+                            style: {
+                                margin: "0pt",
+                                padding: "10pt",
+                                marginBottom: "8pt"
+                            },
+                            children: [(0, Fr.jsx)("span", {
+                                className: "pointer",
+                                onClick: function() {
+                                    return a(kr.Path("/login?auth=1"))
+                                },
+                                style: {
+                                    fontSize: "large",
+                                    color: "inherit"
+                                },
+                                children: (0, Fr.jsxs)("b", {
+                                    children: [Do.Warning, "\xa0\xa0Not Logged In"]
+                                })
+                            }), " ", (0, Fr.jsx)("br", {}), (0, Fr.jsx)(Ji, {
+                                top: "6pt",
+                                bottom: "6pt"
+                            }), (0, Fr.jsxs)("small", {
+                                children: ["Click ", (0, Fr.jsx)(Oe, {
+                                    to: kr.Path("/login", !!s() || r, r),
+                                    style: {
+                                        cursor: "pointer",
+                                        color: "inherit"
+                                    },
+                                    children: (0, Fr.jsx)("b", {
+                                        children: (0, Fr.jsx)("u", {
+                                            children: "here"
+                                        })
+                                    })
+                                }), " to go to the ", (0, Fr.jsx)(Oe, {
+                                    to: kr.Path("/login", !!s() || r, r),
+                                    style: {
+                                        cursor: "pointer",
+                                        color: "inherit"
+                                    },
+                                    children: (0, Fr.jsx)("b", {
+                                        children: "login"
+                                    })
+                                }), " page."]
+                            })]
+                        }) : (0, Fr.jsx)("span", {}), (0, Fr.jsx)("b", {
+                            children: "Environment"
+                        }), s() ? (0, Fr.jsx)(Fr.Fragment, {
+                            children: (0, Fr.jsxs)("div", {
+                                className: p,
+                                style: {
+                                    marginBottom: "8pt",
+                                    padding: "10pt"
+                                },
+                                children: ["Current environment: ", (0, Fr.jsx)("b", {
+                                    children: At.PreferredName(At.Current(), r)
+                                }), Br.IsLoggedIn(r) && !At.IsAllowed(At.Current(), r) && (0, Fr.jsxs)("span", {
+                                    style: {
+                                        color: "red"
+                                    },
+                                    children: ["\xa0", (0, Fr.jsx)("b", {
+                                        children: Do.RightArrow
+                                    }), " You do not have permission for this environment ", (0, Fr.jsx)("b", {
+                                        children: Do.Warning
+                                    })]
+                                })]
+                            })
+                        }) : (0, Fr.jsx)(Fr.Fragment, {
+                            children: (0, Fr.jsxs)("div", {
+                                className: "box warning",
+                                style: {
+                                    marginBottom: "8pt",
+                                    padding: "10pt"
+                                },
+                                children: [At.Current() && "env" !== At.Current() ? (0, Fr.jsxs)(Fr.Fragment, {
+                                    children: ["Unknown environment: ", (0, Fr.jsx)("b", {
+                                        style: {
+                                            color: "darkred"
+                                        },
+                                        children: At.Current()
+                                    })]
+                                }) : (0, Fr.jsx)(Fr.Fragment, {
+                                    children: "No environment specified in URL!"
+                                }), (0, Fr.jsx)("br", {}), (0, Fr.jsxs)("small", {
+                                    children: ["Click ", (0, Fr.jsx)(Oe, {
+                                        to: kr.Path("/env", c()),
+                                        onClick: function() {
+                                            return o(c())
+                                        },
+                                        style: {
+                                            fontWeight: "bold",
+                                            color: "darkred"
+                                        },
+                                        children: "here"
+                                    }), " to use this default environment: \xa0", (0, Fr.jsx)(Oe, {
+                                        to: kr.Path("/env", c()),
+                                        onClick: function() {
+                                            return o(c())
+                                        },
+                                        style: {
+                                            fontWeight: "bold",
+                                            color: "darkred"
+                                        },
+                                        children: c()
+                                    })]
+                                })]
+                            })
+                        }), (0, Fr.jsx)("b", {
+                            children: "Available Environments"
+                        }), " ", (null === (t = r.auth) || void 0 === t ? void 0 : t.known_envs_actual_count) > (null === (n = At.KnownEnvs(r)) || void 0 === n ? void 0 : n.length) && (0, Fr.jsxs)("small", {
+                            children: ["\xa0(", r.auth.known_envs_actual_count, ")"]
+                        }), (0, Fr.jsx)("div", {
+                            className: p,
+                            style: {
+                                margin: "0pt",
+                                padding: "10pt"
+                            },
+                            children: (0, Fr.jsxs)("table", {
+                                style: {
+                                    color: "inherit"
+                                },
+                                children: [(0, Fr.jsx)("thead", {}), (0, Fr.jsx)("tbody", {
+                                    children: At.KnownEnvs(r).map((function(e, t) {
+                                        return (0, Fr.jsxs)("tr", {
+                                            children: [(0, Fr.jsxs)("td", {
+                                                style: {
+                                                    fontWeight: u(e) ? "bold" : "normal",
+                                                    color: s(e.public_name) ? u(e) ? "black" : "inherit" : "red",
+                                                    verticalAlign: "top"
+                                                },
+                                                children: [u(e) ? (0, Fr.jsx)(Fr.Fragment, {
+                                                    children: (0, Fr.jsxs)("span", {
+                                                        id: "tooltip-env-current-check",
+                                                        style: {
+                                                            color: Br.IsLoggedIn(r) && !At.IsAllowed(e, r) ? "red" : "inherit"
+                                                        },
+                                                        children: [Do.Check, "\xa0\xa0"]
+                                                    })
+                                                }) : (0, Fr.jsx)(Fr.Fragment, {
+                                                    children: (0, Fr.jsxs)("span", {
+                                                        style: {
+                                                            color: At.IsAllowed(e, r) ? "inherit" : "red"
+                                                        },
+                                                        children: [Do.Dot, "\xa0\xa0"]
+                                                    })
+                                                }), (0, Fr.jsx)(Yi, {
+                                                    id: "tooltip-env-current-check",
+                                                    position: "bottom",
+                                                    text: "This is your current environment."
+                                                })]
+                                            }), (0, Fr.jsxs)("td", {
+                                                children: [Br.IsLoggedIn(r) && !At.IsAllowed(e, r) ? (0, Fr.jsx)(Fr.Fragment, {
+                                                    children: (0, Fr.jsxs)("span", {
+                                                        style: {
+                                                            color: "red"
+                                                        },
+                                                        children: [(0, Fr.jsx)(Oe, {
+                                                            id: "tooltip-env-nopermission",
+                                                            to: kr.Path("/env", At.PreferredName(e, r)),
+                                                            onClick: function() {
+                                                                return o(At.PreferredName(e, r))
+                                                            },
+                                                            style: {
+                                                                color: "inherit",
+                                                                textDecoration: u(e) ? "underline" : "normal"
+                                                            },
+                                                            children: (0, Fr.jsx)("b", {
+                                                                children: At.PreferredName(e, r)
+                                                            })
+                                                        }), l(e) && (0, Fr.jsxs)("span", {
+                                                            style: {
+                                                                color: "black"
+                                                            },
+                                                            children: ["\xa0", (0, Fr.jsx)("b", {
+                                                                children: Do.RightArrow
+                                                            }), "This is the default environment ", Do.Star]
+                                                        }), "\xa0", (0, Fr.jsx)("b", {
+                                                            children: Do.RightArrow
+                                                        }), " You do not have permission for this environment ", (0, Fr.jsx)("b", {
+                                                            children: Do.Warning
+                                                        }), (0, Fr.jsx)(Yi, {
+                                                            id: "tooltip-env-nopermission",
+                                                            position: "bottom",
+                                                            text: "You do not have permission for this environment."
+                                                        })]
+                                                    })
+                                                }) : (0, Fr.jsx)(Fr.Fragment, {
+                                                    children: u(e) ? (0, Fr.jsxs)(Fr.Fragment, {
+                                                        children: [(0, Fr.jsxs)("span", {
+                                                            style: {
+                                                                color: "black"
+                                                            },
+                                                            children: [(0, Fr.jsx)(Oe, {
+                                                                id: u(e) ? "tooltip-env-current" : "",
+                                                                to: kr.Path("/env", At.PreferredName(e, r)),
+                                                                onClick: function() {
+                                                                    return o(At.PreferredName(e, r))
+                                                                },
+                                                                style: {
+                                                                    color: "inherit"
+                                                                },
+                                                                children: (0, Fr.jsx)("b", {
+                                                                    children: (0, Fr.jsx)("u", {
+                                                                        children: At.PreferredName(e, r)
+                                                                    })
+                                                                })
+                                                            }), l(e) && (0, Fr.jsxs)("span", {
+                                                                children: ["\xa0", (0, Fr.jsx)("b", {
+                                                                    children: Do.RightArrow
+                                                                }), " This is the default environment ", Do.Star]
+                                                            })]
+                                                        }), (0, Fr.jsx)(Yi, {
+                                                            id: "tooltip-env-current",
+                                                            position: "bottom",
+                                                            text: "This is your current environment."
+                                                        })]
+                                                    }) : (0, Fr.jsx)(Fr.Fragment, {
+                                                        children: (0, Fr.jsxs)("span", {
+                                                            children: [(0, Fr.jsx)(Oe, {
+                                                                id: "tooltip-env-default-".concat(e.full_name),
+                                                                to: kr.Path("/env", At.PreferredName(e, r)),
+                                                                onClick: function() {
+                                                                    return o(At.PreferredName(e, r))
+                                                                },
+                                                                style: {
+                                                                    color: "inherit"
+                                                                },
+                                                                children: (0, Fr.jsx)("b", {
+                                                                    children: At.PreferredName(e, r)
+                                                                })
+                                                            }), l(e) && (0, Fr.jsxs)("span", {
+                                                                style: {
+                                                                    color: "black"
+                                                                },
+                                                                children: ["\xa0", (0, Fr.jsx)("b", {
+                                                                    children: Do.RightArrow
+                                                                }), " This is the default environment ", Do.Star]
+                                                            }), (0, Fr.jsx)(Yi, {
+                                                                id: "tooltip-env-default-".concat(e.full_name),
+                                                                position: "top",
+                                                                text: "This is the default environment."
+                                                            })]
+                                                        })
+                                                    })
+                                                }), (0, Fr.jsx)("br", {}), "Full Name: ", (0, Fr.jsx)("span", {
+                                                    style: h(e.full_name),
+                                                    children: e.full_name
+                                                }), " ", (0, Fr.jsx)("br", {}), "Short Name: ", (0, Fr.jsx)("span", {
+                                                    style: h(e.short_name),
+                                                    children: e.short_name
+                                                }), " ", (0, Fr.jsx)("br", {}), "Public Name: ", (0, Fr.jsx)("span", {
+                                                    style: h(e.public_name),
+                                                    children: e.public_name
+                                                }), " ", (0, Fr.jsx)("br", {}), Br.IsLoggedIn() && (0, Fr.jsxs)(Fr.Fragment, {
+                                                    children: ["GAC Name: ", d(e, i.data), " ", (0, Fr.jsx)("br", {}), s() && f(e, i.data) && (0, Fr.jsxs)(Fr.Fragment, {
+                                                        children: [(0, Fr.jsxs)("select", {
+                                                            style: {
+                                                                border: "0",
+                                                                background: "transparent",
+                                                                WebkitAppearance: "none"
+                                                            },
+                                                            onChange: function(t) {
+                                                                return function(e, t) {
+                                                                    var n = e.target.value;
+                                                                    a(kr.Path("/gac/" + n, t))
+                                                                }(t, At.PreferredName(e, r))
+                                                            },
+                                                            children: [(0, Fr.jsxs)("option", {
+                                                                children: ["GAC Compare ", Do.DownArrow]
+                                                            }), At.KnownEnvs(r).map((function(e) {
+                                                                return (0, Fr.jsx)("option", {
+                                                                    children: At.PreferredName(e, r)
+                                                                }, Dr()())
+                                                            }))]
+                                                        }), (0, Fr.jsx)("br", {})]
+                                                    }), t < At.KnownEnvs(r).length - 1 && (0, Fr.jsx)("br", {})]
+                                                })]
+                                            })]
+                                        }, Dr()())
+                                    }))
+                                })]
+                            })
+                        }), Br.IsLoggedIn(r) && (0, Fr.jsx)("div", {
+                            style: {
+                                marginTop: "8pt"
+                            }
+                        })]
+                    })
+                })
+            },
+            ph = function(e) {
+                var t = co();
+                return t.loading ? null : (0, Fr.jsxs)(Fr.Fragment, {
+                    children: [(0, Fr.jsx)("br", {}), (0, Fr.jsx)("table", {
+                        width: "100%",
+                        children: (0, Fr.jsxs)("tbody", {
+                            children: [(0, Fr.jsx)("tr", {
+                                style: {
+                                    backgroundColor: "darkred",
+                                    height: "1px"
+                                },
+                                children: (0, Fr.jsx)("td", {})
+                            }), (0, Fr.jsx)("tr", {
+                                children: (0, Fr.jsx)("td", {
+                                    align: "center",
+                                    style: {
+                                        paddingTop: "2px",
+                                        paddingBottom: "6px"
+                                    },
+                                    children: (0, Fr.jsx)("a", {
+                                        href: kr.PortalLink(t),
+                                        target: "_blank",
+                                        rel: "noreferrer",
+                                        children: (0, Fr.jsx)("img", {
+                                            alt: "harvard",
+                                            src: Ut.Harvard(),
+                                            height: "46"
+                                        })
+                                    })
+                                })
+                            }), (0, Fr.jsx)("tr", {
+                                style: {
+                                    backgroundColor: "darkred",
+                                    height: "1px"
+                                },
+                                children: (0, Fr.jsx)("td", {})
+                            })]
+                        })
+                    })]
+                })
+            },
+            hh = function(e) {
+                var t = co();
+                return (0, Fr.jsx)(Fr.Fragment, {
+                    children: (0, Fr.jsx)("div", {
+                        className: "container",
+                        id: "login_container",
+                        children: (0, Fr.jsxs)("div", {
+                            className: "boxstyle check-error",
+                            style: {
+                                margin: "20pt",
+                                padding: "10pt"
+                            },
+                            children: [(0, Fr.jsx)("b", {
+                                children: "Forbidden response from server."
+                            }), ".  ", (0, Fr.jsx)("br", {}), "You seem to be logged in but the server does not seem to think so. ", (0, Fr.jsx)("br", {}), "Try ", (0, Fr.jsx)("span", {
+                                onClick: function() {
+                                    return Zr()
+                                },
+                                style: {
+                                    cursor: "pointer"
+                                },
+                                children: (0, Fr.jsx)("u", {
+                                    children: "logging out"
+                                })
+                            }), " and logging in again.", (0, Fr.jsx)("br", {}), (0, Fr.jsxs)("small", {
+                                children: ["Click ", (0, Fr.jsx)(Oe, {
+                                    to: kr.Path("/login", At.Current(t)),
+                                    style: {
+                                        color: "darkred"
+                                    },
+                                    children: (0, Fr.jsx)("b", {
+                                        children: "here"
+                                    })
+                                }), " to go to the ", (0, Fr.jsx)(Oe, {
+                                    to: kr.Path("/login", At.Current(t)),
+                                    children: (0, Fr.jsx)("b", {
+                                        style: {
+                                            color: "darkred"
+                                        },
+                                        children: "login"
+                                    })
+                                }), " page."]
+                            })]
+                        })
+                    })
+                })
+            },
+            gh = function() {
+                var e = a(ra(), 2),
+                    t = e[0],
+                    n = e[1];
+                return (0, Fr.jsxs)(Fr.Fragment, {
+                    children: [(0, Fr.jsx)("img", {
+                        id: "tooltip-readonly",
+                        alt: "lock",
+                        src: t ? Ut.Lock() : Ut.Unlock(),
+                        style: {
+                            height: "35",
+                            cursor: "pointer"
+                        },
+                        onClick: function() {
+                            return n(!t)
+                        }
+                    }), (0, Fr.jsx)(Yi, {
+                        id: "tooltip-readonly",
+                        position: "bottom",
+                        text: "You are in ".concat(t ? "readonly" : "read/write", " mode. Click to enter ").concat(t ? "read/write" : "readonly", " mode.")
+                    })]
+                })
+            },
+            yh = function(e) {
+                e.header;
+                var t, n, r, o, i = a(Re(), 1)[0].get("soon"),
+                    s = so("/certificates?soon=".concat(i));
+                return s.loading ? (0, Fr.jsx)(Fr.Fragment, {}) : null !== s && void 0 !== s && null !== (t = s.data) && void 0 !== t && null !== (n = t.portal_ssl_certificate) && void 0 !== n && n.expires_soon ? (0, Fr.jsxs)(Fr.Fragment, {
+                    children: [(0, Fr.jsx)("tr", {
+                        children: (0, Fr.jsx)("td", {
+                            style: {
+                                background: "black",
+                                height: "2px"
+                            },
+                            colSpan: "3"
+                        })
+                    }), (0, Fr.jsx)("tr", {
+                        children: (0, Fr.jsxs)("td", {
+                            style: {
+                                background: "darkred",
+                                color: "#FFF4F3",
+                                padding: "3pt",
+                                fontSize: "9pt"
+                            },
+                            colSpan: "3",
+                            children: [(0, Fr.jsx)("b", {
+                                children: "Warning: SSL certificate for associated Portal will expire soon"
+                            }), "\xa0", Do.RightArrow, "\xa0", null === (r = s.data.portal_ssl_certificate) || void 0 === r ? void 0 : r.expires_at, "\xa0", Do.RightArrow, "\xa0", Pr.FromNow(null === (o = s.data.portal_ssl_certificate) || void 0 === o ? void 0 : o.expires_at)]
+                        })
+                    }), (0, Fr.jsx)("tr", {
+                        children: (0, Fr.jsx)("td", {
+                            style: {
+                                background: "black",
+                                height: "1px"
+                            },
+                            colSpan: "3"
+                        })
+                    })]
+                }) : (0, Fr.jsx)(Fr.Fragment, {})
+            },
+            mh = function(e) {
+                var t = e.header,
+                    n = Ft.LightenDarkenColor(Ft.GetBackgroundColor(), -10),
+                    r = function(e) {
+                        var t = e.path,
+                            n = e.label;
+                        return (0, Fr.jsx)(Fr.Fragment, {
+                            children: kr.CurrentLogicalPath() === t ? (0, Fr.jsxs)("span", {
+                                style: {
+                                    fontWeight: "bold"
+                                },
+                                children: [n, "\xa0", Do.Check]
+                            }) : (0, Fr.jsx)(Oe, {
+                                to: kr.Path(t),
+                                children: n
+                            }, t)
+                        })
+                    },
+                    o = function() {
+                        return (0, Fr.jsx)("div", {
+                            style: {
+                                height: "1px",
+                                marginTop: "1pt",
+                                marginBottom: "1pt",
+                                marginLeft: "6pt",
+                                marginRight: "6pt",
+                                background: "var(--box-fg)"
+                            }
+                        })
+                    };
+                return (0, Fr.jsx)(Fr.Fragment, {
+                    children: (0, Fr.jsxs)("span", {
+                        className: "dropdown",
+                        children: [(0, Fr.jsx)("span", {
+                            className: "dropdown-button",
+                            children: (0, Fr.jsx)("img", {
+                                alt: "menu",
+                                style: {
+                                    marginLeft: "-4px",
+                                    marginTop: "-1px"
+                                },
+                                src: Ut.MenuIcon(),
+                                height: "20"
+                            })
+                        }), (0, Fr.jsxs)("div", {
+                            className: "dropdown-content",
+                            id: "dropdown-content-id",
+                            style: {
+                                background: n
+                            },
+                            children: [(0, Fr.jsx)(r, {
+                                path: "/home",
+                                label: "Home"
+                            }), (0, Fr.jsx)(r, {
+                                path: "/info",
+                                label: "General Info"
+                            }), (0, Fr.jsx)(r, {
+                                path: "/checks",
+                                label: "Checks"
+                            }), (0, Fr.jsx)(o, {}), (0, Fr.jsx)(r, {
+                                path: "/aws/infrastructure",
+                                label: "Infrastructure"
+                            }), (0, Fr.jsx)(r, {
+                                path: "/aws/s3",
+                                label: "S3"
+                            }), (0, Fr.jsx)(r, {
+                                path: "/users",
+                                label: "Users"
+                            }), (0, Fr.jsx)(o, {}), (0, Fr.jsx)(r, {
+                                path: "/env",
+                                label: "Environments"
+                            }), (0, Fr.jsx)(r, {
+                                path: "/accounts",
+                                label: "Accounts"
+                            }), (0, Fr.jsx)(r, {
+                                path: "/login",
+                                label: Br.IsLoggedIn(t) ? "Session" : "Login"
+                            })]
+                        })]
+                    })
+                })
+            },
+            vh = function(e) {
+                var t, n, r, o, i = e.header;
+
+                function a(e) {
+                    return e ? {
+                        textDecoration: "none",
+                        color: "black",
+                        fontWeight: "bold"
+                    } : {
+                        textDecoration: "none",
+                        color: Ft.GetForegroundColor(),
+                        fontWeight: "normal"
+                    }
+                }
+                return (0, Fr.jsxs)(Fr.Fragment, {
+                    children: [(0, Fr.jsx)(ze, {
+                        to: kr.Path("/home"),
+                        style: function(e) {
+                            return a(e.isActive)
+                        },
+                        children: "HOME"
+                    }), "\xa0|\xa0", (0, Fr.jsx)(ze, {
+                        to: kr.Path("/info"),
+                        style: function(e) {
+                            return a(e.isActive)
+                        },
+                        children: "INFO"
+                    }), "\xa0|\xa0", (0, Fr.jsx)(ze, {
+                        to: kr.Path("/checks"),
+                        style: function(e) {
+                            return a(e.isActive)
+                        },
+                        children: "CHECKS"
+                    }), "\xa0|\xa0", (0, Fr.jsx)(ze, {
+                        to: kr.Path("/env"),
+                        style: function(e) {
+                            return a(e.isActive)
+                        },
+                        children: "ENV"
+                    }), "\xa0|\xa0", (0, Fr.jsxs)("a", {
+                        target: "_blank",
+                        rel: "noreferrer",
+                        id: "tooltip-header-portal",
+                        style: {
+                            textDecoration: "none",
+                            color: "darkgreen"
+                        },
+                        href: kr.PortalLink(i),
+                        children: ["PORTAL ", (0, Fr.jsx)("span", {
+                            className: "fa fa-external-link",
+                            style: {
+                                position: "relative",
+                                bottom: "-1px",
+                                fontSize: "14px"
+                            }
+                        })]
+                    }), "\xa0|\xa0", (0, Fr.jsxs)("a", {
+                        target: "_blank",
+                        rel: "noreferrer",
+                        id: "tooltip-header-aws",
+                        style: {
+                            textDecoration: "none",
+                            color: "darkgreen"
+                        },
+                        href: "https://" + (null === (t = i.app) || void 0 === t ? void 0 : t.credentials.aws_account_number) + ".signin.aws.amazon.com/console/",
+                        children: ["AWS ", (0, Fr.jsx)("span", {
+                            className: "fa fa-external-link",
+                            style: {
+                                position: "relative",
+                                bottom: "-1px",
+                                fontSize: "14px"
+                            }
+                        })]
+                    }), (0, Fr.jsx)(Yi, {
+                        id: "tooltip-header-portal",
+                        position: "bottom",
+                        text: "Open portal (in new tab)."
+                    }), (0, Fr.jsx)(Yi, {
+                        id: "tooltip-header-aws",
+                        position: "bottom",
+                        text: "Open AWS console for (".concat(null !== (n = i.app) && void 0 !== n && n.credentials.aws_account_name ? (null === (r = i.app) || void 0 === r ? void 0 : r.credentials.aws_account_name) + "/" : "").concat(null === (o = i.app) || void 0 === o ? void 0 : o.credentials.aws_account_number, ") account (in new tab).")
+                    })]
+                })
+            },
+            Mh = function(e) {
+                var t = e.header;
+                return (0, Fr.jsxs)("span", {
+                    children: [(0, Fr.jsx)(mh, {
+                        header: t
+                    }), (0, Fr.jsx)(Fr.Fragment, {
+                        children: "\xa0|\xa0"
+                    }), (0, Fr.jsx)(vh, {
+                        header: t
+                    })]
+                })
+            },
             bh = function(e) {
+                var n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, w, j, x, N, I, D, S, L, k = co(),
+                    C = Va(),
+                    E = fe(),
+                    _ = a(So(), 1)[0],
+                    T = At.IsFoursightFourfront(k) ? "#14533C" : "#143C53",
+                    A = Ft.LightenDarkenColor(Ft.GetBackgroundColor(), -10);
+                return (0, Fr.jsx)(Fr.Fragment, {
+                    children: k.loading ? (0, Fr.jsxs)("div", {
+                        style: {
+                            width: "100%"
+                        },
+                        children: [(0, Fr.jsx)("table", {
+                            style: {
+                                width: "100%",
+                                height: "42px",
+                                background: Br.IsLoggedIn(k) ? T : "#444444"
+                            },
+                            children: (0, Fr.jsx)("tbody", {
+                                children: (0, Fr.jsxs)("tr", {
+                                    children: [(0, Fr.jsx)("td", {
+                                        width: "1%",
+                                        style: {
+                                            height: "42px",
+                                            paddingLeft: "2pt",
+                                            whiteSpace: "nowrap"
+                                        },
+                                        children: (0, Fr.jsx)("div", {
+                                            style: {
+                                                width: "200px"
+                                            }
+                                        })
+                                    }), (0, Fr.jsx)("td", {
+                                        width: "98%",
+                                        align: "center",
+                                        style: {
+                                            fontSize: "16pt",
+                                            color: "white",
+                                            nowrap: "1"
+                                        },
+                                        children: k.error ? (0, Fr.jsx)("span", {
+                                            children: (0, Fr.jsx)("b", {
+                                                style: {
+                                                    color: "red"
+                                                },
+                                                children: "Foursight Load Error"
+                                            })
+                                        }) : (0, Fr.jsx)("span", {
+                                            children: (0, Fr.jsx)("i", {
+                                                style: {
+                                                    color: "yellow"
+                                                },
+                                                children: "Foursight Loading ..."
+                                            })
+                                        })
+                                    }), (0, Fr.jsx)("td", {
+                                        width: "1%",
+                                        align: "right",
+                                        children: (0, Fr.jsxs)("span", {
+                                            style: {
+                                                position: "relative",
+                                                bottom: "5pt"
+                                            },
+                                            children: ["\xa0", (0, Fr.jsx)(wo, {
+                                                loading: k.loading && !k.error,
+                                                color: "yellow",
+                                                size: 150,
+                                                style: {
+                                                    marginRight: "20px"
+                                                }
+                                            })]
+                                        })
+                                    })]
+                                })
+                            })
+                        }), (0, Fr.jsx)("table", {
+                            style: {
+                                width: "100%",
+                                height: "22px",
+                                background: "lightgray"
+                            },
+                            children: (0, Fr.jsxs)("tbody", {
+                                children: [(0, Fr.jsx)("tr", {
+                                    children: (0, Fr.jsx)("td", {
+                                        style: {
+                                            height: "27px",
+                                            paddingLeft: "2pt",
+                                            whiteSpace: "nowrap",
+                                            background: "lightgray"
+                                        }
+                                    })
+                                }), (0, Fr.jsx)("tr", {
+                                    children: (0, Fr.jsx)("td", {
+                                        style: {
+                                            height: "20px",
+                                            paddingLeft: "2pt",
+                                            whiteSpace: "nowrap",
+                                            background: "lightyellow"
+                                        }
+                                    })
+                                })]
+                            })
+                        })]
+                    }) : (0, Fr.jsxs)(t.Fragment, {
+                        children: [(0, Fr.jsxs)("div", {
+                            style: {
+                                width: "100%",
+                                background: T
+                            },
+                            children: [(0, Fr.jsx)("table", {
+                                width: "100%",
+                                cellPadding: "0",
+                                cellSpacing: "0",
+                                children: (0, Fr.jsx)("tbody", {
+                                    children: (0, Fr.jsxs)("tr", {
+                                        children: [(0, Fr.jsx)("td", {
+                                            width: "38%",
+                                            style: {
+                                                paddingLeft: "2pt",
+                                                whiteSpace: "nowrap"
+                                            },
+                                            children: (0, Fr.jsx)("a", {
+                                                href: kr.PortalLink(k),
+                                                target: "_blank",
+                                                rel: "noreferrer",
+                                                children: At.IsFoursightFourfront(k) ? (0, Fr.jsx)("span", {
+                                                    children: (0, Fr.jsx)("img", {
+                                                        alt: "foursight",
+                                                        style: {
+                                                            marginLeft: "14px",
+                                                            marginTop: "5px",
+                                                            marginBottom: "5px"
+                                                        },
+                                                        src: Ut.FoursightFourfrontLogo(),
+                                                        height: "32",
+                                                        width: "44"
+                                                    })
+                                                }) : (0, Fr.jsx)("span", {
+                                                    children: (0, Fr.jsx)("img", {
+                                                        alt: "foursight",
+                                                        src: Ut.FoursightCgapLogo(),
+                                                        width: "130"
+                                                    })
+                                                })
+                                            })
+                                        }), (0, Fr.jsx)("td", {
+                                            width: "24%",
+                                            align: "center",
+                                            style: {
+                                                whiteSpace: "nowrap"
+                                            },
+                                            children: (0, Fr.jsx)("div", {
+                                                style: {
+                                                    fontSize: "20pt",
+                                                    color: "white",
+                                                    cursor: "pointer"
+                                                },
+                                                onClick: function() {
+                                                    return E(kr.Path("/home"))
+                                                },
+                                                children: "dev" === (null === (n = k.app) || void 0 === n ? void 0 : n.stage) ? (0, Fr.jsx)(Fr.Fragment, {
+                                                    children: null !== (r = k.app) && void 0 !== r && r.local ? (0, Fr.jsxs)(Fr.Fragment, {
+                                                        children: [(0, Fr.jsx)("span", {
+                                                            title: "Running locally.",
+                                                            style: {
+                                                                position: "relative",
+                                                                bottom: "3pt",
+                                                                color: "yellow",
+                                                                fontSize: "17pt"
+                                                            },
+                                                            children: Do.DoNotEnter
+                                                        }), "\xa0", (0, Fr.jsx)("span", {
+                                                            title: "Stage is DEV. Running locally",
+                                                            style: {
+                                                                position: "relative",
+                                                                bottom: "1pt",
+                                                                color: "yellow",
+                                                                fontSize: "26pt"
+                                                            },
+                                                            children: Do.Atom
+                                                        }), "\xa0\xa0", (0, Fr.jsx)("span", {
+                                                            className: "title-font",
+                                                            style: {
+                                                                position: "relative",
+                                                                bottom: "3pt",
+                                                                color: "white",
+                                                                fontWeight: "bold"
+                                                            },
+                                                            children: null === (o = k.app) || void 0 === o ? void 0 : o.title.toUpperCase()
+                                                        }), "\xa0\xa0", (0, Fr.jsx)("span", {
+                                                            title: "Stage is DEV. Running locally",
+                                                            style: {
+                                                                position: "relative",
+                                                                bottom: "1pt",
+                                                                color: "yellow",
+                                                                fontSize: "24pt"
+                                                            },
+                                                            children: Do.Atom
+                                                        }), "\xa0", (0, Fr.jsx)("span", {
+                                                            title: "Running locally.",
+                                                            style: {
+                                                                position: "relative",
+                                                                bottom: "3pt",
+                                                                color: "yellow",
+                                                                fontSize: "17pt"
+                                                            },
+                                                            children: Do.DoNotEnter
+                                                        }), "\xa0\xa0"]
+                                                    }) : (0, Fr.jsxs)(Fr.Fragment, {
+                                                        children: [(0, Fr.jsx)("span", {
+                                                            title: "Stage is DEV.",
+                                                            style: {
+                                                                position: "relative",
+                                                                bottom: "1pt",
+                                                                color: "yellow",
+                                                                fontSize: "24pt"
+                                                            },
+                                                            children: Do.Atom
+                                                        }), "\xa0\xa0", (0, Fr.jsx)("span", {
+                                                            className: "title-font",
+                                                            style: {
+                                                                position: "relative",
+                                                                bottom: "2pt",
+                                                                color: "white",
+                                                                fontWeight: "bold"
+                                                            },
+                                                            children: null === (i = k.app) || void 0 === i ? void 0 : i.title.toUpperCase()
+                                                        }), "\xa0\xa0", (0, Fr.jsx)("span", {
+                                                            title: "Stage is DEV.",
+                                                            style: {
+                                                                position: "relative",
+                                                                bottom: "1pt",
+                                                                color: "yellow",
+                                                                fontSize: "24pt"
+                                                            },
+                                                            children: Do.Atom
+                                                        }), "\xa0"]
+                                                    })
+                                                }) : (0, Fr.jsx)(Fr.Fragment, {
+                                                    children: null !== (s = k.app) && void 0 !== s && s.local ? (0, Fr.jsxs)(Fr.Fragment, {
+                                                        children: [(0, Fr.jsx)("span", {
+                                                            title: "Running locally.",
+                                                            style: {
+                                                                position: "relative",
+                                                                bottom: "2pt",
+                                                                color: "yellow",
+                                                                fontSize: "17pt"
+                                                            },
+                                                            children: Do.DoNotEnter
+                                                        }), "\xa0\xa0", (0, Fr.jsx)("span", {
+                                                            className: "title-font",
+                                                            style: {
+                                                                position: "relative",
+                                                                bottom: "1pt",
+                                                                color: "white",
+                                                                fontWeight: "bold"
+                                                            },
+                                                            children: null === (u = k.app) || void 0 === u ? void 0 : u.title.toUpperCase()
+                                                        }), "\xa0\xa0", (0, Fr.jsx)("span", {
+                                                            title: "Running locally.",
+                                                            style: {
+                                                                position: "relative",
+                                                                bottom: "2pt",
+                                                                color: "yellow",
+                                                                fontSize: "17pt"
+                                                            },
+                                                            children: Do.DoNotEnter
+                                                        }), "\xa0\xa0"]
+                                                    }) : (0, Fr.jsxs)(Fr.Fragment, {
+                                                        children: [(0, Fr.jsx)("span", {
+                                                            className: "title-font",
+                                                            style: {
+                                                                position: "relative",
+                                                                bottom: "1pt",
+                                                                color: "white",
+                                                                fontWeight: "bold"
+                                                            },
+                                                            children: null === (l = k.app) || void 0 === l ? void 0 : l.title.toUpperCase()
+                                                        }), "\xa0\xa0"]
+                                                    })
+                                                })
+                                            })
+                                        }), (0, Fr.jsxs)("td", {
+                                            width: "38%",
+                                            style: {
+                                                paddingRight: "10pt",
+                                                whiteSpace: "nowrap",
+                                                color: "#D6EAF8"
+                                            },
+                                            align: "right",
+                                            children: [(0, Fr.jsx)("small", {
+                                                children: (0, Fr.jsx)(aa.FormatDateTime, {
+                                                    verbose: !0,
+                                                    timezone: !1
+                                                })
+                                            }), (null === (c = k.app) || void 0 === c || null === (d = c.credentials) || void 0 === d ? void 0 : d.aws_account_name) && (0, Fr.jsxs)(Fr.Fragment, {
+                                                children: ["\xa0|\xa0", (0, Fr.jsx)(Oe, {
+                                                    id: "tooltip-header-account",
+                                                    to: kr.Path("/login"),
+                                                    style: {
+                                                        textDecoration: "none",
+                                                        color: "inherit"
+                                                    },
+                                                    children: (0, Fr.jsx)("b", {
+                                                        children: null === (f = k.app) || void 0 === f || null === (p = f.credentials) || void 0 === p || null === (h = p.aws_account_name) || void 0 === h ? void 0 : h.replace(/^cgap-/, "")
+                                                    })
+                                                }), (0, Fr.jsx)(Yi, {
+                                                    id: "tooltip-header-account",
+                                                    position: "bottom",
+                                                    text: "AWS account number: ".concat(null === (g = k.app) || void 0 === g || null === (y = g.credentials) || void 0 === y ? void 0 : y.aws_account_number)
+                                                })]
+                                            }), Br.IsLoggedIn(k) ? (0, Fr.jsxs)("span", {
+                                                children: ["\xa0|\xa0", (0, Fr.jsx)("span", {
+                                                    style: {
+                                                        cursor: "pointer",
+                                                        color: "#D6EAF8"
+                                                    },
+                                                    onClick: function() {
+                                                        return Zr()
+                                                    },
+                                                    children: "LOGOUT"
+                                                })]
+                                            }) : (0, Fr.jsxs)("span", {
+                                                children: ["\xa0|\xa0", (0, Fr.jsx)(Oe, {
+                                                    to: kr.Path("/login?auth", At.Current(k)),
+                                                    style: {
+                                                        cursor: "pointer",
+                                                        color: "#D6EAF8"
+                                                    },
+                                                    id: "tooltip-header-nologin",
+                                                    children: "LOGIN"
+                                                }), (0, Fr.jsx)(Yi, {
+                                                    id: "tooltip-header-nologin",
+                                                    position: "bottom",
+                                                    text: "Not logged in. Click to login."
+                                                })]
+                                            })]
+                                        })]
+                                    })
+                                })
+                            }), (0, Fr.jsx)("table", {
+                                width: "100%",
+                                cellPadding: "0",
+                                cellSpacing: "0",
+                                children: (0, Fr.jsxs)("tbody", {
+                                    children: [(0, Fr.jsxs)("tr", {
+                                        style: {
+                                            background: A
+                                        },
+                                        children: [(0, Fr.jsx)("td", {
+                                            width: "49%",
+                                            style: {
+                                                paddingLeft: "10pt",
+                                                paddingTop: "3pt",
+                                                paddingBottom: "3pt",
+                                                whiteSpace: "nowrap"
+                                            },
+                                            children: (0, Fr.jsx)(Mh, {
+                                                header: k
+                                            })
+                                        }), (0, Fr.jsx)("td", {
+                                            width: "2%",
+                                            align: "center",
+                                            style: {
+                                                whiteSpace: "nowrap",
+                                                margin: "0 auto"
+                                            },
+                                            children: (0, Fr.jsxs)("a", {
+                                                target: "_blank",
+                                                rel: "noreferrer",
+                                                href: "https://pypi.org/project/" + (At.IsFoursightFourfront(k) ? "foursight" : "foursight-cgap") + "/" + (null === (m = k.app) || void 0 === m ? void 0 : m.version) + "/",
+                                                children: [(0, Fr.jsx)("b", {
+                                                    style: {
+                                                        textDecoration: "none",
+                                                        color: "#263A48",
+                                                        paddingRight: "8pt"
+                                                    },
+                                                    id: "tooltip-header-version",
+                                                    children: null === (v = k.app) || void 0 === v ? void 0 : v.version
+                                                }), (0, Fr.jsx)(Yi, {
+                                                    id: "tooltip-header-version",
+                                                    position: "bottom",
+                                                    text: (null !== (M = k.app) && void 0 !== M && M.deployed ? "Deployed: ".concat(null === (b = k.app) || void 0 === b ? void 0 : b.deployed, ". ") : "") + "Launched: " + (null === (w = k.app) || void 0 === w ? void 0 : w.launched),
+                                                    size: "x-small"
+                                                })]
+                                            })
+                                        }), (0, Fr.jsxs)("td", {
+                                            width: "49%",
+                                            style: {
+                                                paddingRight: "10pt",
+                                                paddingTop: "2pt",
+                                                paddingBottom: "1pt",
+                                                whiteSpace: "nowrap"
+                                            },
+                                            align: "right",
+                                            nowrap: "1",
+                                            children: ["cognito" !== At.Current() && At.KnownEnvs(k).length > 0 ? (0, Fr.jsxs)(Fr.Fragment, {
+                                                children: [(0, Fr.jsxs)("span", {
+                                                    className: "dropdown",
+                                                    children: [(0, Fr.jsx)(Yi, {
+                                                        id: "tooltip-header-env",
+                                                        position: "left",
+                                                        size: "small",
+                                                        text: "Environments",
+                                                        shape: "squared",
+                                                        nopad: !0
+                                                    }), (0, Fr.jsx)("b", {
+                                                        id: "tooltip-header-env",
+                                                        className: "dropdown-button",
+                                                        style: {
+                                                            color: !At.IsKnown(At.Current(), k) || Br.IsLoggedIn(k) && !At.IsAllowed(At.Current(), k) ? "red" : "#143c53"
+                                                        },
+                                                        children: At.Current() || "unknown-env"
+                                                    }), (0, Fr.jsxs)("div", {
+                                                        className: "dropdown-content",
+                                                        id: "dropdown-content-id",
+                                                        style: {
+                                                            background: A
+                                                        },
+                                                        children: [At.KnownEnvs(k).map((function(e) {
+                                                            return At.Equals(e, At.Current()) ? (0, Fr.jsxs)("span", {
+                                                                children: [At.PreferredName(e, k), "\xa0\xa0", Do.Check, !At.IsAllowed(e, k) && Br.IsLoggedIn(k) && (0, Fr.jsxs)(Fr.Fragment, {
+                                                                    children: ["\xa0\xa0", Do.Warning]
+                                                                })]
+                                                            }, e.full_name) : At.IsAllowed(e, k) ? (0, Fr.jsx)(Oe, {
+                                                                onClick: function() {
+                                                                    return C(At.PreferredName(e))
+                                                                },
+                                                                to: {
+                                                                    pathname: "/redirect"
+                                                                },
+                                                                state: {
+                                                                    url: At.IsKnown(At.Current(), k) ? kr.Path(null, At.PreferredName(e, k)) : kr.Path("/env", At.PreferredName(At.Default(k), k))
+                                                                },
+                                                                children: At.PreferredName(e, k)
+                                                            }, e.full_name) : (0, Fr.jsxs)(Oe, {
+                                                                to: kr.Path("/env", At.PreferredName(e, k)),
+                                                                children: [At.PreferredName(e, k), !At.IsAllowed(e, k) && Br.IsLoggedIn(k) && (0, Fr.jsxs)(Fr.Fragment, {
+                                                                    children: ["\xa0\xa0", Do.Warning]
+                                                                })]
+                                                            }, e.public_name)
+                                                        })), (0, Fr.jsx)("div", {
+                                                            height: "1",
+                                                            style: {
+                                                                marginTop: "2px",
+                                                                height: "1px",
+                                                                background: "darkblue"
+                                                            }
+                                                        }), (0, Fr.jsx)(Oe, {
+                                                            id: "__envinfo__",
+                                                            to: kr.Path("/env"),
+                                                            onClick: function() {
+                                                                document.getElementById("__envinfo__").style.fontWeight = "normal"
+                                                            },
+                                                            children: "Environments"
+                                                        })]
+                                                    })]
+                                                }), "\xa0|\xa0"]
+                                            }) : (0, Fr.jsx)(Fr.Fragment, {
+                                                children: "cognito" !== At.Current() ? (0, Fr.jsxs)(Fr.Fragment, {
+                                                    children: [(0, Fr.jsx)("b", {
+                                                        style: {
+                                                            color: T
+                                                        },
+                                                        children: At.Current()
+                                                    }), "\xa0|\xa0"]
+                                                }) : (0, Fr.jsx)(Fr.Fragment, {
+                                                    children: (0, Fr.jsx)("b", {
+                                                        style: {
+                                                            color: T
+                                                        },
+                                                        children: At.PreferredName(At.Default(k))
+                                                    })
+                                                })
+                                            }), "prod" === (null === (j = k.app) || void 0 === j ? void 0 : j.stage) ? (0, Fr.jsxs)(Fr.Fragment, {
+                                                children: [(0, Fr.jsx)("b", {
+                                                    id: "tooltip-header-stage-prod",
+                                                    style: {
+                                                        color: "darkred"
+                                                    },
+                                                    children: null === (x = k.app) || void 0 === x ? void 0 : x.stage
+                                                }), " \xa0|\xa0", (0, Fr.jsx)(Yi, {
+                                                    id: "tooltip-header-stage-prod",
+                                                    position: "bottom",
+                                                    text: "Deployment stage: PROD"
+                                                })]
+                                            }) : (0, Fr.jsx)(Fr.Fragment, {}), "dev" === (null === (N = k.app) || void 0 === N ? void 0 : N.stage) ? (0, Fr.jsxs)(Fr.Fragment, {
+                                                children: [(0, Fr.jsx)("b", {
+                                                    id: "tooltip-header-stage-dev",
+                                                    style: {
+                                                        color: "darkgreen"
+                                                    },
+                                                    children: null === (I = k.app) || void 0 === I ? void 0 : I.stage
+                                                }), " \xa0|\xa0", (0, Fr.jsx)(Yi, {
+                                                    id: "tooltip-header-stage-dev",
+                                                    position: "bottom",
+                                                    text: "Deployment stage: DEV"
+                                                })]
+                                            }) : (0, Fr.jsx)(Fr.Fragment, {}), "prod" !== (null === (D = k.app) || void 0 === D ? void 0 : D.stage) && "dev" !== (null === (S = k.app) || void 0 === S ? void 0 : S.stage) ? (0, Fr.jsxs)(Fr.Fragment, {
+                                                children: [(0, Fr.jsxs)("b", {
+                                                    id: "tooltip-header-stage",
+                                                    children: [null === (L = k.app) || void 0 === L ? void 0 : L.stage, "}"]
+                                                }), " \xa0|\xa0", (0, Fr.jsx)(Yi, {
+                                                    id: "tooltip-header-stage",
+                                                    position: "bottom",
+                                                    text: "Deployment stage: {header.app?.stage}"
+                                                })]
+                                            }) : (0, Fr.jsx)(Fr.Fragment, {}), Br.IsLoggedIn(k) ? (0, Fr.jsx)(Fr.Fragment, {
+                                                children: Br.LoggedInUser(k) ? (0, Fr.jsxs)(Fr.Fragment, {
+                                                    children: [(0, Fr.jsx)(Oe, {
+                                                        to: kr.Path("/login"),
+                                                        id: "tooltip-header-logged-in",
+                                                        style: {
+                                                            textDecoration: "none"
+                                                        },
+                                                        children: (0, Fr.jsx)("b", {
+                                                            style: {
+                                                                color: "darkblue"
+                                                            },
+                                                            children: Br.LoggedInUser(k)
+                                                        })
+                                                    }), (0, Fr.jsx)(Yi, {
+                                                        id: "tooltip-header-logged-in",
+                                                        position: "bottom",
+                                                        text: "Logged in ".concat(Pr.Ago(Br.LoggedInAt()))
+                                                    }), Br.LoggedInViaGoogle(k) ? (0, Fr.jsx)(Fr.Fragment, {
+                                                        children: (0, Fr.jsxs)("span", {
+                                                            children: [(0, Fr.jsx)("img", {
+                                                                id: "tooltip-header-login-google",
+                                                                alt: "google",
+                                                                style: {
+                                                                    marginLeft: "9px",
+                                                                    marginRight: "0",
+                                                                    marginBottom: "2px"
+                                                                },
+                                                                src: Ut.GoogleLoginLogo(),
+                                                                height: "15"
+                                                            }), (0, Fr.jsx)(Yi, {
+                                                                id: "tooltip-header-login-google",
+                                                                position: "bottom",
+                                                                text: "Logged in via Google authentication."
+                                                            })]
+                                                        })
+                                                    }) : (0, Fr.jsx)(Fr.Fragment, {
+                                                        children: Br.LoggedInViaGitHub(k) && (0, Fr.jsxs)(Fr.Fragment, {
+                                                            children: [(0, Fr.jsx)("span", {
+                                                                id: "tooltip-header-login-github",
+                                                                children: (0, Fr.jsx)("img", {
+                                                                    alt: "github",
+                                                                    style: {
+                                                                        marginLeft: "5px",
+                                                                        marginRight: "-4px",
+                                                                        marginBottom: "2px"
+                                                                    },
+                                                                    src: Ut.GitHubLoginLogo(),
+                                                                    height: "19"
+                                                                })
+                                                            }), (0, Fr.jsx)(Yi, {
+                                                                id: "tooltip-header-login-github",
+                                                                position: "bottom",
+                                                                text: "Logged in via GitHub authentication."
+                                                            })]
+                                                        })
+                                                    })]
+                                                }) : (0, Fr.jsx)(Fr.Fragment, {
+                                                    children: (0, Fr.jsx)("b", {
+                                                        style: {
+                                                            color: "darkred"
+                                                        },
+                                                        children: "UNKNOWN USER"
+                                                    })
+                                                })
+                                            }) : (0, Fr.jsxs)(Fr.Fragment, {
+                                                children: [(0, Fr.jsx)(Oe, {
+                                                    to: kr.Path("/login", At.Current(k)),
+                                                    style: {
+                                                        textDecoration: "none"
+                                                    },
+                                                    children: (0, Fr.jsx)("b", {
+                                                        style: {
+                                                            color: "darkblue"
+                                                        },
+                                                        id: "tooltip-header-nologin-2",
+                                                        children: "NOT LOGGED IN"
+                                                    })
+                                                }), (0, Fr.jsx)(Yi, {
+                                                    id: "tooltip-header-nologin-2",
+                                                    position: "bottom",
+                                                    text: "Not logged in. Click to login."
+                                                })]
+                                            })]
+                                        })]
+                                    }), (0, Fr.jsxs)("tr", {
+                                        children: [(0, Fr.jsx)("td", {
+                                            style: {
+                                                background: "lightyellow",
+                                                color: "darkred",
+                                                padding: "3pt"
+                                            },
+                                            colSpan: "1",
+                                            children: (0, Fr.jsxs)("i", {
+                                                style: {
+                                                    fontSize: "small"
+                                                },
+                                                children: ["This is the ", (0, Fr.jsx)("b", {
+                                                    children: "new"
+                                                }), " Foursight ", (0, Fr.jsx)("b", {
+                                                    children: "React"
+                                                }), ". For the ", (0, Fr.jsx)("b", {
+                                                    children: "legacy"
+                                                }), " Foursight click ", (0, Fr.jsx)("a", {
+                                                    href: At.LegacyFoursightLink(k),
+                                                    style: {
+                                                        color: "inherit"
+                                                    },
+                                                    children: (0, Fr.jsx)("b", {
+                                                        children: (0, Fr.jsx)("u", {
+                                                            children: "here"
+                                                        })
+                                                    })
+                                                }), "."]
+                                            })
+                                        }), (0, Fr.jsx)("td", {
+                                            style: {
+                                                background: "lightyellow"
+                                            }
+                                        }), (0, Fr.jsx)("td", {
+                                            style: {
+                                                background: "lightyellow",
+                                                color: "darkred",
+                                                fontSize: "small"
+                                            },
+                                            children: (0, Fr.jsx)("table", {
+                                                width: "100%",
+                                                children: (0, Fr.jsx)("tbody", {
+                                                    children: (0, Fr.jsxs)("tr", {
+                                                        children: [(0, Fr.jsx)("td", {
+                                                            style: {
+                                                                float: "right",
+                                                                width: "98%",
+                                                                whiteSpace: "nowrap",
+                                                                align: "right"
+                                                            },
+                                                            align: "right",
+                                                            children: _.length > 0 && (0, Fr.jsx)(Fr.Fragment, {
+                                                                children: (0, Fr.jsx)("span", {
+                                                                    children: (0, Fr.jsx)(No, {
+                                                                        loading: _.length > 0,
+                                                                        color: "darkred",
+                                                                        label: "",
+                                                                        size: 150,
+                                                                        style: {
+                                                                            marginRight: "20px"
+                                                                        }
+                                                                    })
+                                                                })
+                                                            })
+                                                        }), (0, Fr.jsx)("td", {
+                                                            style: {
+                                                                width: "1%",
+                                                                color: "darkred"
+                                                            },
+                                                            children: _.length > 0 && (0, Fr.jsxs)("small", {
+                                                                children: ["\xa0\xa0[", _.length, "]"]
+                                                            })
+                                                        }), (0, Fr.jsx)("td", {
+                                                            style: {
+                                                                color: "darkred",
+                                                                textAlign: "right",
+                                                                paddingRight: "10pt",
+                                                                width: "1%",
+                                                                fontSize: "small",
+                                                                fontStyle: "italic",
+                                                                whiteSpace: "nowrap"
+                                                            },
+                                                            children: kr.IsLocal() && (0, Fr.jsxs)(Fr.Fragment, {
+                                                                children: ["\xa0\xa0", Je.IsLocalCrossOrigin() ? (0, Fr.jsx)(Fr.Fragment, {
+                                                                    children: "Running locally cross-origin"
+                                                                }) : (0, Fr.jsx)(Fr.Fragment, {
+                                                                    children: "Running locally"
+                                                                })]
+                                                            })
+                                                        })]
+                                                    })
+                                                })
+                                            })
+                                        })]
+                                    }), (0, Fr.jsx)(yh, {
+                                        header: k
+                                    }), (0, Fr.jsx)("tr", {
+                                        children: (0, Fr.jsx)("td", {
+                                            style: {
+                                                height: "1px",
+                                                background: "darkblue"
+                                            }
+                                        })
+                                    })]
+                                })
+                            })]
+                        }), (0, Fr.jsxs)("div", {
+                            style: {
+                                float: "right",
+                                marginRight: "7pt",
+                                marginTop: "6pt"
+                            },
+                            children: [!1, (0, Fr.jsx)("div", {
+                                children: (0, Fr.jsx)("table", {
+                                    children: (0, Fr.jsx)("tbody", {
+                                        children: (0, Fr.jsx)("tr", {
+                                            children: (0, Fr.jsx)("td", {
+                                                style: {
+                                                    paddingLeft: "10pt"
+                                                },
+                                                children: (0, Fr.jsx)(gh, {})
+                                            })
+                                        })
+                                    })
+                                })
+                            })]
+                        })]
+                    })
+                })
+            },
+            wh = function(e) {
+                var n = e.children,
+                    r = a((0, t.useState)({
+                        loading: !0
+                    }), 2),
+                    o = r[0],
+                    i = r[1];
+                return so("/header", {
+                    onData: function(e) {
+                        e.loading = !1, i(e), At.IsFoursightFourfront(e) ? Ft.SetFoursightFourfront() : Ft.SetFoursightCgap()
+                    },
+                    onError: function(e) {
+                        i((function(e) {
+                            return Ye(Ye({}, e), {
+                                error: !0
+                            })
+                        }))
+                    },
+                    cache: !0
+                }), (0, Fr.jsx)(lo.Provider, {
+                    value: [o, i],
+                    children: n
+                })
+            },
+            jh = function(e) {
+                var n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, w, j = co(),
+                    x = (At.IsFoursightFourfront(j) ? "foursight" : "foursight-cgap") + ": " + (null === j || void 0 === j || null === (n = j.versions) || void 0 === n ? void 0 : n.foursight_core) + " | foursight-core: " + (null === j || void 0 === j || null === (r = j.versions) || void 0 === r ? void 0 : r.foursight) + " | dcicutils: " + (null === j || void 0 === j || null === (o = j.versions) || void 0 === o ? void 0 : o.dcicutils),
+                    N = {
+                        id: "".concat(null === (i = j.app) || void 0 === i || null === (s = i.credentials) || void 0 === s ? void 0 : s.aws_account_name, ":").concat(null === j || void 0 === j || null === (u = j.app) || void 0 === u ? void 0 : u.stage),
+                        name: null === (l = j.app) || void 0 === l || null === (c = l.credentials) || void 0 === c ? void 0 : c.aws_account_name,
+                        stage: null === (d = j.app) || void 0 === d ? void 0 : d.stage
+                    },
+                    I = a((0, t.useState)(!1), 2),
+                    D = I[0],
+                    S = I[1];
+                return (0, Fr.jsx)(Fr.Fragment, {
+                    children: (0, Fr.jsxs)("div", {
+                        className: "container",
+                        style: {
+                            marginTop: "-16pt"
+                        },
+                        children: [(0, Fr.jsxs)("div", {
+                            className: "box lighten",
+                            style: {
+                                margin: "20pt",
+                                padding: "10pt"
+                            },
+                            children: [(0, Fr.jsxs)("b", {
+                                style: {
+                                    fontSize: "x-large"
+                                },
+                                children: ["Welcome to Foursight \xa0", (0, Fr.jsxs)("span", {
+                                    style: {
+                                        fontWeight: "normal"
+                                    },
+                                    children: ["(", At.IsFoursightFourfront(j) ? "Fourfront" : "CGAP", ")"]
+                                })]
+                            }), (0, Fr.jsxs)("div", {
+                                style: {
+                                    float: "right",
+                                    fontSize: "x-small",
+                                    textAlign: "right",
+                                    marginTop: "-3pt",
+                                    marginRight: "2pt"
+                                },
+                                children: [(0, Fr.jsxs)("span", {
+                                    id: "tooltip-home-versions",
+                                    children: ["Foursight Version: ", (0, Fr.jsx)("b", {
+                                        children: null === j || void 0 === j || null === (f = j.versions) || void 0 === f ? void 0 : f.foursight
+                                    })]
+                                }), " ", (0, Fr.jsx)("br", {}), (0, Fr.jsx)(Yi, {
+                                    id: "tooltip-home-versions",
+                                    position: "top",
+                                    size: "small",
+                                    text: x
+                                }), null !== j && void 0 !== j && null !== (p = j.app) && void 0 !== p && null !== (h = p.credentials) && void 0 !== h && h.aws_account_name ? (0, Fr.jsxs)(Fr.Fragment, {
+                                    children: [(0, Fr.jsxs)("span", {
+                                        id: "tooltip-home-aws-account",
+                                        children: ["AWS Account: ", (0, Fr.jsx)("b", {
+                                            children: null === j || void 0 === j || null === (g = j.app) || void 0 === g || null === (y = g.credentials) || void 0 === y ? void 0 : y.aws_account_name
+                                        })]
+                                    }), " ", (0, Fr.jsx)("br", {}), (0, Fr.jsx)(Yi, {
+                                        id: "tooltip-home-aws-account",
+                                        position: "top",
+                                        size: "small",
+                                        text: "AWS Account Number: " + (null === j || void 0 === j || null === (m = j.app) || void 0 === m || null === (v = m.credentials) || void 0 === v ? void 0 : v.aws_account_number)
+                                    })]
+                                }) : (0, Fr.jsxs)(Fr.Fragment, {
+                                    children: [(0, Fr.jsxs)("span", {
+                                        children: ["AWS Account: ", (0, Fr.jsx)("b", {
+                                            children: null === j || void 0 === j || null === (M = j.app) || void 0 === M || null === (b = M.credentials) || void 0 === b ? void 0 : b.aws_account_number
+                                        })]
+                                    }), " ", (0, Fr.jsx)("br", {})]
+                                }), "Foursight Stage: ", (0, Fr.jsx)("b", {
+                                    children: null === j || void 0 === j || null === (w = j.app) || void 0 === w ? void 0 : w.stage
+                                }), " ", (0, Fr.jsx)("br", {})]
+                            }), (0, Fr.jsx)(Ji, {
+                                top: "10pt",
+                                bottom: "4pt"
+                            }), "This is the ", (0, Fr.jsx)("b", {
+                                children: "new"
+                            }), " React version of Foursight. To use the previous version click ", (0, Fr.jsx)("b", {
+                                children: (0, Fr.jsx)("a", {
+                                    href: At.LegacyFoursightLink(j),
+                                    style: {
+                                        color: "inherit"
+                                    },
+                                    children: (0, Fr.jsx)("u", {
+                                        children: "here"
+                                    })
+                                })
+                            }), ".", (0, Fr.jsx)("span", {
+                                id: "tooltip-account-summary",
+                                style: {
+                                    float: "right",
+                                    marginTop: "-3pt"
+                                },
+                                className: "pointer",
+                                onClick: function() {
+                                    return S(!D)
+                                },
+                                children: (0, Fr.jsx)("img", {
+                                    alt: "settings",
+                                    src: Ut.SettingsRedIcon(),
+                                    height: "28"
+                                })
+                            }), (0, Fr.jsx)(Yi, {
+                                id: "tooltip-account-summary",
+                                position: "top",
+                                size: "small",
+                                text: "Click to " + (D ? "hide" : "show") + " account summary."
+                            }), (0, Fr.jsx)(Ji, {
+                                top: "4pt",
+                                bottom: "10pt"
+                            }), D && (0, Fr.jsx)(Fr.Fragment, {
+                                children: (0, Fr.jsx)("div", {
+                                    style: {
+                                        marginBottom: "12pt"
+                                    },
+                                    children: (0, Fr.jsx)(Wi, {
+                                        account: N,
+                                        header: j,
+                                        decrementAccountCount: function() {},
+                                        all: !0,
+                                        brighten: !0
+                                    })
+                                })
+                            }), (0, Fr.jsx)("p", {}), (0, Fr.jsxs)("ul", {
+                                children: [(0, Fr.jsxs)("li", {
+                                    children: [" To view Foursight ", (0, Fr.jsx)("b", {
+                                        children: (0, Fr.jsx)(qi, {
+                                            to: "/checks",
+                                            children: "checks"
+                                        })
+                                    }), " click ", (0, Fr.jsx)("b", {
+                                        children: (0, Fr.jsx)(qi, {
+                                            to: "/checks",
+                                            children: (0, Fr.jsx)("u", {
+                                                children: "here"
+                                            })
+                                        })
+                                    }), ".  "]
+                                }), (0, Fr.jsxs)("li", {
+                                    children: [" To view Foursight ", (0, Fr.jsx)("b", {
+                                        children: (0, Fr.jsx)(qi, {
+                                            to: "/info",
+                                            children: "general"
+                                        })
+                                    }), " info click ", (0, Fr.jsx)("b", {
+                                        children: (0, Fr.jsx)(qi, {
+                                            to: "/info",
+                                            children: (0, Fr.jsx)("u", {
+                                                children: "here"
+                                            })
+                                        })
+                                    }), ".  "]
+                                }), (0, Fr.jsxs)("li", {
+                                    children: [" To view Foursight ", (0, Fr.jsx)("b", {
+                                        children: (0, Fr.jsx)(qi, {
+                                            to: "/env",
+                                            children: "environments"
+                                        })
+                                    }), " info click ", (0, Fr.jsx)("b", {
+                                        children: (0, Fr.jsx)(qi, {
+                                            to: "/env",
+                                            children: (0, Fr.jsx)("u", {
+                                                children: "here"
+                                            })
+                                        })
+                                    }), ". "]
+                                }), (0, Fr.jsxs)("li", {
+                                    children: [" To view Foursight ", (0, Fr.jsx)("b", {
+                                        children: (0, Fr.jsx)(qi, {
+                                            to: "/users",
+                                            children: "users"
+                                        })
+                                    }), " click ", (0, Fr.jsx)("b", {
+                                        children: (0, Fr.jsx)(qi, {
+                                            to: "/users",
+                                            children: (0, Fr.jsx)("u", {
+                                                children: "here"
+                                            })
+                                        })
+                                    }), ".  "]
+                                }), (0, Fr.jsxs)("li", {
+                                    children: [" To view ", (0, Fr.jsx)("b", {
+                                        children: (0, Fr.jsx)(qi, {
+                                            to: "/aws/s3",
+                                            children: "AWS S3"
+                                        })
+                                    }), " info click ", (0, Fr.jsx)("b", {
+                                        children: (0, Fr.jsx)(qi, {
+                                            to: "/aws/s3",
+                                            children: (0, Fr.jsx)("u", {
+                                                children: "here"
+                                            })
+                                        })
+                                    }), ".  "]
+                                }), (0, Fr.jsxs)("li", {
+                                    children: [" To view ", (0, Fr.jsx)("b", {
+                                        children: (0, Fr.jsx)(qi, {
+                                            to: "/aws/infrastructure",
+                                            children: "AWS infrastructure"
+                                        })
+                                    }), " info click ", (0, Fr.jsx)("b", {
+                                        children: (0, Fr.jsx)(qi, {
+                                            to: "/aws/infrastructure",
+                                            children: (0, Fr.jsx)("u", {
+                                                children: "here"
+                                            })
+                                        })
+                                    }), ".  "]
+                                })]
+                            })]
+                        }), (0, Fr.jsxs)("div", {
+                            className: "box thickborder",
+                            style: {
+                                margin: "20pt",
+                                padding: "10pt",
+                                marginTop: "-10pt"
+                            },
+                            children: ["You are logged in as: ", (0, Fr.jsx)(Ki, {}), (0, Fr.jsx)("br", {}), "To view your ", (0, Fr.jsx)("b", {
+                                children: (0, Fr.jsx)(qi, {
+                                    to: "/login",
+                                    children: "session"
+                                })
+                            }), " info click ", (0, Fr.jsx)("b", {
+                                children: (0, Fr.jsx)(qi, {
+                                    to: "/login",
+                                    children: (0, Fr.jsx)("u", {
+                                        children: "here"
+                                    })
+                                })
+                            }), ". ", (0, Fr.jsx)("br", {}), "To ", (0, Fr.jsx)("b", {
+                                onClick: Zr,
+                                children: (0, Fr.jsx)(qi, {
+                                    children: "logout"
+                                })
+                            }), " click ", (0, Fr.jsx)("b", {
+                                onClick: Zr,
+                                children: (0, Fr.jsx)(qi, {
+                                    children: (0, Fr.jsx)("u", {
+                                        children: "here"
+                                    })
+                                })
+                            }), "."]
+                        }), (0, Fr.jsx)(Fr.Fragment, {
+                            children: (0, Fr.jsxs)("div", {
+                                className: "box lighten",
+                                style: {
+                                    fontSize: "small",
+                                    margin: "20pt",
+                                    padding: "5pt 10pt 5pt 10pt",
+                                    marginTop: "-10pt"
+                                },
+                                children: ["Click ", (0, Fr.jsx)("a", {
+                                    href: kr.Path("/accounts?all=true"),
+                                    rel: "noreferrer",
+                                    target: "_blank",
+                                    style: {
+                                        color: "var(--box-fg)"
+                                    },
+                                    children: (0, Fr.jsx)("b", {
+                                        children: "here"
+                                    })
+                                }), " to view all ", (0, Fr.jsx)("a", {
+                                    href: kr.Path("/accounts?all=true"),
+                                    style: {
+                                        color: "var(--box-fg)"
+                                    },
+                                    rel: "noreferrer",
+                                    target: "_blank",
+                                    children: (0, Fr.jsx)("b", {
+                                        children: "known accounts"
+                                    })
+                                }), ".", (0, Fr.jsx)($i, {
+                                    href: kr.Path("/accounts?all=true"),
+                                    bold: !0,
+                                    style: {
+                                        marginLeft: "6pt"
+                                    }
+                                })]
+                            })
+                        })]
+                    })
+                })
+            },
+            xh = function(e) {
+                var n = e.title,
+                    r = e.show,
+                    o = void 0 === r || r,
+                    i = e.info,
+                    s = e.children,
+                    u = a((0, t.useState)(o), 2),
+                    l = u[0],
+                    c = u[1];
+                return (0, Fr.jsx)(Fr.Fragment, {
+                    children: (0, Fr.jsx)("div", {
+                        className: "container",
+                        children: l ? (0, Fr.jsxs)(Fr.Fragment, {
+                            children: [(0, Fr.jsx)("b", {
+                                onClick: function() {
+                                    return c(!1)
+                                },
+                                style: {
+                                    cursor: "pointer"
+                                },
+                                children: n
+                            }), " \xa0", (0, Fr.jsx)("span", {
+                                onClick: function() {
+                                    return c(!1)
+                                },
+                                style: {
+                                    cursor: "pointer"
+                                },
+                                children: Do.DownArrow
+                            }), "Versions" === n && (0, Fr.jsxs)("b", {
+                                id: "tooltip-info-refresh",
+                                style: {
+                                    float: "right",
+                                    cursor: "pointer"
+                                },
+                                onClick: i.refresh,
+                                children: [Do.Refresh, "\xa0"]
+                            }), (0, Fr.jsx)(Yi, {
+                                id: "tooltip-info-refresh",
+                                position: "bottom",
+                                size: "small",
+                                text: "Click to refresh."
+                            }), (0, Fr.jsx)("ul", {
+                                className: "top-level-list",
+                                children: (0, Fr.jsx)("div", {
+                                    className: "box",
+                                    style: {
+                                        paddingLeft: "8pt",
+                                        paddingTop: "6pt",
+                                        paddingBottom: "8pt"
+                                    },
+                                    children: s
+                                })
+                            })]
+                        }) : (0, Fr.jsxs)(Fr.Fragment, {
+                            children: [(0, Fr.jsx)("b", {
+                                onClick: function() {
+                                    return c(!0)
+                                },
+                                style: {
+                                    cursor: "pointer"
+                                },
+                                children: n
+                            }), " \xa0", (0, Fr.jsx)("span", {
+                                onClick: function() {
+                                    return c(!0)
+                                },
+                                style: {
+                                    cursor: "pointer"
+                                },
+                                children: Do.UpArrow
+                            }), (0, Fr.jsxs)("div", {
+                                className: "box",
+                                children: ["Click ", (0, Fr.jsx)("span", {
+                                    onClick: function() {
+                                        return c(!0)
+                                    },
+                                    style: {
+                                        cursor: "pointer"
+                                    },
+                                    children: (0, Fr.jsx)("b", {
+                                        children: "here"
+                                    })
+                                }), " to ", (0, Fr.jsx)("span", {
+                                    onClick: function() {
+                                        return c(!0)
+                                    },
+                                    style: {
+                                        cursor: "pointer"
+                                    },
+                                    children: "show"
+                                }), "."]
+                            })]
+                        })
+                    })
+                })
+            },
+            Nh = function(e) {
+                var t = e.name,
+                    n = e.value,
+                    r = e.monospace,
+                    o = void 0 !== r && r,
+                    i = e.copy,
+                    a = void 0 === i || i,
+                    s = e.size,
+                    u = void 0 === s ? "4" : s,
+                    l = e.pypi,
+                    c = void 0 === l ? null : l,
+                    d = e.github,
+                    f = void 0 === d ? null : d,
+                    p = e.elasticsearch,
+                    h = void 0 !== p && p,
+                    g = e.python,
+                    y = void 0 !== g && g,
+                    m = (e.chalice, e.check),
+                    v = void 0 !== m && m,
+                    M = e.link,
+                    b = void 0 === M ? null : M,
+                    w = e.optional,
+                    j = void 0 !== w && w;
+                var x = {
+                        fontSize: "11pt",
+                        fontFamily: o ? "monospace" : "inherit",
+                        fontWeight: "bold",
+                        wordWrap: "break-word",
+                        cursor: a ? "copy" : "inherit",
+                        align: "left"
+                    },
+                    N = a ? {
+                        onClick: function() {
+                            return Vi.Copy(t)
+                        }
+                    } : {},
+                    I = v ? (0, Fr.jsxs)("span", {
+                        children: ["\xa0", (0, Fr.jsx)("b", {
+                            style: {
+                                fontSize: "13pt",
+                                color: "green"
+                            },
+                            children: Do.Check
+                        })]
+                    }) : (0, Fr.jsx)("span", {}),
+                    D = c ? (0, Fr.jsxs)("span", {
+                        children: [(0, Fr.jsx)("a", {
+                            target: "_blank",
+                            rel: "noreferrer",
+                            href: "https://pypi.org/project/" + t + "/" + n + "/",
+                            children: (0, Fr.jsx)("img", {
+                                alt: "pypi",
+                                src: Ut.PyPi(),
+                                height: "21"
+                            })
+                        }), "\xa0"]
+                    }) : (0, Fr.jsx)("span", {}),
+                    S = f ? (0, Fr.jsxs)("span", {
+                        children: [(0, Fr.jsx)("a", {
+                            target: "_blank",
+                            rel: "noreferrer",
+                            href: "https://github.com/" + f + "/" + ("dcicutils" === t ? "utils" : t) + "/releases/tag/" + ("chalice" !== t ? "v" : "") + n,
+                            children: (0, Fr.jsx)("img", {
+                                alt: "github",
+                                src: Ut.GitHub(),
+                                height: "15"
+                            })
+                        }), "\xa0"]
+                    }) : (0, Fr.jsx)("span", {}),
+                    L = h ? (0, Fr.jsxs)("span", {
+                        children: [(0, Fr.jsx)("a", {
+                            target: "_blank",
+                            rel: "noreferrer",
+                            href: "https://www.elastic.co/guide/en/elasticsearch/reference/".concat(function(e) {
+                                var t = null === e || void 0 === e ? void 0 : e.split(".");
+                                return (null === t || void 0 === t ? void 0 : t.length) >= 2 ? t[0] + "." + t[1] : e
+                            }(n), "/release-notes-").concat(n, ".html"),
+                            style: {
+                                marginLeft: "-2px"
+                            },
+                            children: (0, Fr.jsx)("img", {
+                                alt: "github",
+                                src: Ut.ElasticsearchLogo(),
+                                height: "18"
+                            })
+                        }), "\xa0"]
+                    }) : (0, Fr.jsx)("span", {}),
+                    k = y ? (0, Fr.jsxs)("span", {
+                        children: [(0, Fr.jsx)("a", {
+                            target: "_blank",
+                            rel: "noreferrer",
+                            href: "https://docs.python.org/release/" + n + "/",
+                            children: (0, Fr.jsx)("img", {
+                                alt: "python",
+                                src: Ut.Python(),
+                                height: "19"
+                            })
+                        }), "\xa0"]
+                    }) : (0, Fr.jsx)("span", {}),
+                    C = (0, Fr.jsx)("span", {});
+                return (0, Fr.jsx)(Fr.Fragment, {
+                    children: (0, Fr.jsx)("div", {
+                        style: {
+                            marginTop: "1px"
+                        },
+                        children: !j || n ? (0, Fr.jsxs)("div", {
+                            className: "row",
+                            children: [(0, Fr.jsx)("div", {
+                                className: "col-sm-" + u,
+                                children: (0, Fr.jsxs)("div", {
+                                    style: {
+                                        fontSize: "11pt",
+                                        fontFamily: "inherit",
+                                        fontWeight: "normal",
+                                        padding: "0px",
+                                        align: "left"
+                                    },
+                                    children: [t, ":"]
+                                })
+                            }), (0, Fr.jsxs)("div", Ye(Ye({
+                                id: t,
+                                className: "col-sm-8",
+                                style: x,
+                                align: "left"
+                            }, N), {}, {
+                                children: [D, S, L, k, C, b && n ? (0, Fr.jsx)("span", {
+                                    children: (0, Fr.jsx)(Oe, {
+                                        to: b,
+                                        children: n
+                                    })
+                                }) : (0, Fr.jsx)("span", {
+                                    children: st.IsNonEmptyObject(n) ? (0, Fr.jsx)(Fr.Fragment, {
+                                        children: n
+                                    }) : (0, Fr.jsx)(Fr.Fragment, {
+                                        children: n || (0, Fr.jsx)("span", {
+                                            children: Do.EmptySet
+                                        })
+                                    })
+                                }), I]
+                            }))]
+                        }) : (0, Fr.jsx)("span", {})
+                    })
+                })
+            },
+            Ih = function() {
+                var e, n, r, o, i, s, u, l, c, d, f, p, h, g, y, m, v, M, b, w, j, x, N, I, D, S, L, k, C, E, _, T, A, O, z, U, P, R = co(),
+                    B = so("/info"),
+                    F = a((0, t.useState)(!1), 2),
+                    Y = F[0],
+                    Q = F[1],
+                    G = a((0, t.useState)(!1), 2),
+                    W = G[0],
+                    H = G[1],
+                    Z = a((0, t.useState)(!1), 2),
+                    V = Z[0],
+                    q = Z[1],
+                    J = oa();
+                return B.error ? (0, Fr.jsx)(Xi, {
+                    error: B.error,
+                    message: "Error loading info from Foursight API"
+                }) : (0, Fr.jsxs)("div", {
+                    className: "container",
+                    children: [(0, Fr.jsxs)(xh, {
+                        info: B,
+                        title: "Versions",
+                        children: [(0, Fr.jsx)(Nh, {
+                            name: null === (e = R.app) || void 0 === e ? void 0 : e.package,
+                            value: null === (n = R.versions) || void 0 === n ? void 0 : n.foursight,
+                            monospace: !0,
+                            copy: !0,
+                            pypi: !0,
+                            github: At.IsFoursightFourfront(R) ? "4dn-dcic" : "dbmi-bgm",
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "foursight-core",
+                            value: null === (r = R.versions) || void 0 === r ? void 0 : r.foursight_core,
+                            monospace: !0,
+                            copy: !0,
+                            pypi: !0,
+                            github: "4dn-dcic",
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "dcicutils",
+                            value: null === (o = R.versions) || void 0 === o ? void 0 : o.dcicutils,
+                            monospace: !0,
+                            copy: !0,
+                            pypi: !0,
+                            github: "4dn-dcic",
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "tibanna",
+                            value: null === (i = R.versions) || void 0 === i ? void 0 : i.tibanna,
+                            monospace: !0,
+                            copy: !0,
+                            size: "2",
+                            pypi: !0
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "tibanna-ff",
+                            value: null === (s = R.versions) || void 0 === s ? void 0 : s.tibanna_ff,
+                            monospace: !0,
+                            copy: !0,
+                            size: "2",
+                            pypi: !0
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "chalice",
+                            value: null === (u = R.versions) || void 0 === u ? void 0 : u.chalice,
+                            monospace: !0,
+                            copy: !0,
+                            chalice: !0,
+                            size: "2",
+                            pypi: !0,
+                            github: "aws"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "python",
+                            value: null === (l = R.versions) || void 0 === l ? void 0 : l.python,
+                            monospace: !0,
+                            copy: !0,
+                            python: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "elasticsearch-server",
+                            value: (null === (c = R.versions) || void 0 === c ? void 0 : c.elasticsearch_server) || (null === (d = B.data) || void 0 === d || null === (f = d.versions) || void 0 === f ? void 0 : f.elasticsearch_server),
+                            monospace: !0,
+                            copy: !0,
+                            size: "2",
+                            elasticsearch: !0
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "elasticsearch",
+                            value: null === (p = R.versions) || void 0 === p ? void 0 : p.elasticsearch,
+                            monospace: !0,
+                            copy: !0,
+                            size: "2",
+                            pypi: !0
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "elasticsearch-dsl",
+                            value: null === (h = R.versions) || void 0 === h ? void 0 : h.elasticsearch_dsl,
+                            monospace: !0,
+                            copy: !0,
+                            size: "2",
+                            pypi: !0
+                        })]
+                    }), (0, Fr.jsxs)(xh, {
+                        info: B,
+                        title: "Credentials Info",
+                        children: [(0, Fr.jsx)(Nh, {
+                            name: "AWS Account Number",
+                            value: B.get("app.credentials.aws_account_number"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "AWS User ARN",
+                            value: B.get("app.credentials.aws_user_arn"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "AWS Access Key ID",
+                            value: B.get("app.credentials.aws_access_key_id"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "AWS Region Name",
+                            value: B.get("app.credentials.aws_region"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Auth0 Client ID",
+                            value: B.get("app.credentials.auth0_client_id"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "2"
+                        })]
+                    }), (0, Fr.jsxs)(xh, {
+                        info: B,
+                        title: "Resources",
+                        children: [(0, Fr.jsx)(Nh, {
+                            name: "Foursight Server",
+                            value: B.get("server.foursight"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Portal Server",
+                            value: B.get("server.portal"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "ElasticSearch Server",
+                            value: B.get("server.es"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "RDS Server",
+                            value: B.get("server.rds"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "SQS Server",
+                            value: B.get("server.sqs"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "2"
+                        })]
+                    }), (0, Fr.jsxs)(xh, {
+                        info: B,
+                        title: "Environment Names",
+                        children: [(0, Fr.jsx)(Nh, {
+                            name: "Environment Name",
+                            value: At.RegularName(At.Current(), R),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Environment Name (Full)",
+                            value: At.FullName(At.Current(), R),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Environment Name (Short)",
+                            value: At.ShortName(At.Current(), R),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Environment Name (Public)",
+                            value: At.PublicName(At.Current(), R),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Environment Name (Foursight)",
+                            value: At.FoursightName(At.Current(), R),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Environment Name (Preferred)",
+                            value: At.PreferredName(At.Current(R), R),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        })]
+                    }), (0, Fr.jsxs)(xh, {
+                        info: B,
+                        title: "Bucket Names",
+                        children: [(0, Fr.jsx)(Nh, {
+                            name: "Global Environment Bucket",
+                            value: B.get("buckets.env"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Foursight Bucket Name",
+                            value: B.get("buckets.foursight"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Foursight Bucket Prefix",
+                            value: B.get("buckets.foursight_prefix"),
+                            monospace: !0,
+                            copy: !0,
+                            size: "3"
+                        })]
+                    }), (0, Fr.jsx)(xh, {
+                        info: B,
+                        title: "Environment & Bucket Names",
+                        children: (0, Fr.jsx)("pre", {
+                            className: "box",
+                            style: {
+                                border: "0",
+                                margin: "0",
+                                padding: "8",
+                                paddingBottom: "8",
+                                marginTop: "0"
+                            },
+                            children: (0, Fr.jsxs)("span", {
+                                children: [qr.Format(B.get("buckets.info")), (null === (g = B.get("buckets.info")) || void 0 === g ? void 0 : g.length) > 1 ? (0, Fr.jsx)("div", {
+                                    style: {
+                                        height: "1px",
+                                        marginTop: "6px",
+                                        marginBottom: "6px",
+                                        background: "black"
+                                    }
+                                }) : (0, Fr.jsx)("span", {})]
+                            }, Dr()())
+                        })
+                    }), (0, Fr.jsx)(xh, {
+                        info: B,
+                        title: "Ecosystem",
+                        show: !1,
+                        children: (0, Fr.jsx)("pre", {
+                            className: "box",
+                            style: {
+                                border: "0",
+                                margin: "0",
+                                paddingTop: "8",
+                                paddingBottom: "8",
+                                marginTop: "0"
+                            },
+                            children: qr.Format(B.get("buckets.ecosystem"))
+                        })
+                    }), (0, Fr.jsxs)(xh, {
+                        info: B,
+                        title: "Authentication/Authorization Info",
+                        show: !1,
+                        children: [(0, Fr.jsx)(Nh, {
+                            name: "Email",
+                            value: null === (y = Br.Token()) || void 0 === y ? void 0 : y.user,
+                            monospace: !0,
+                            copy: !0,
+                            check: null === (m = Br.Token()) || void 0 === m ? void 0 : m.user_verified,
+                            link: kr.Path("/users/" + Br.LoggedInUser(R), !0),
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "First Name",
+                            value: null === (v = Br.Token()) || void 0 === v ? void 0 : v.first_name,
+                            monospace: !0,
+                            copy: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Last Name",
+                            value: null === (M = Br.Token()) || void 0 === M ? void 0 : M.last_name,
+                            monospace: !0,
+                            copy: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Environments",
+                            value: null === (b = Br.Token()) || void 0 === b ? void 0 : b.allowed_envs.join(", "),
+                            monospace: !0,
+                            copy: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Audience",
+                            value: null === (w = Br.Token()) || void 0 === w ? void 0 : w.aud,
+                            monospace: !0,
+                            copy: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Issued At",
+                            monospace: !0,
+                            copy: !0,
+                            size: "2",
+                            value: (0, Fr.jsx)(aa.FormatDuration, {
+                                start: null === (j = Br.Token()) || void 0 === j ? void 0 : j.authenticated_at,
+                                verbose: !0,
+                                fallback: "just now",
+                                suffix: "ago",
+                                tooltip: !0,
+                                prefix: "datetime"
+                            })
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Expires At",
+                            monospace: !0,
+                            copy: !0,
+                            size: "2",
+                            value: (0, Fr.jsx)(aa.FormatDuration, {
+                                end: null === (x = Br.Token()) || void 0 === x ? void 0 : x.authenticated_until,
+                                verbose: !0,
+                                fallback: "now",
+                                suffix: "from now",
+                                tooltip: !0,
+                                prefix: "datetime"
+                            })
+                        }), (0, Fr.jsx)("hr", {
+                            style: {
+                                borderTop: "1px solid darkblue",
+                                marginTop: "8",
+                                marginBottom: "8"
+                            }
+                        }), Y ? (0, Fr.jsxs)(Fr.Fragment, {
+                            children: [(0, Fr.jsx)("small", {
+                                onClick: function() {
+                                    return Q(!1)
+                                },
+                                style: {
+                                    cursor: "pointer",
+                                    color: "inherit"
+                                },
+                                children: (0, Fr.jsxs)("b", {
+                                    children: [(0, Fr.jsx)("u", {
+                                        children: "AuthToken"
+                                    }), "\xa0", Do.DownArrow]
+                                })
+                            }), (0, Fr.jsxs)("pre", {
+                                style: {
+                                    filter: "brightness(1.05)",
+                                    background: "inherit",
+                                    color: "inherit",
+                                    fontWeight: "bold",
+                                    marginTop: "6pt"
+                                },
+                                children: [(0, Fr.jsx)("span", {
+                                    style: {
+                                        fontSize: "0",
+                                        opacity: "0"
+                                    },
+                                    id: "authtoken",
+                                    children: Tr.Str(Br.Token())
+                                }), (0, Fr.jsx)("img", {
+                                    src: Ut.Clipboard(),
+                                    alt: "copy",
+                                    onClick: function() {
+                                        return Vi.Copy("authtoken")
+                                    },
+                                    style: {
+                                        float: "right",
+                                        height: "20px",
+                                        cursor: "copy"
+                                    }
+                                }), qr.Format(Br.Token())]
+                            })]
+                        }) : (0, Fr.jsxs)(Fr.Fragment, {
+                            children: [(0, Fr.jsx)("small", {
+                                onClick: function() {
+                                    return Q(!0)
+                                },
+                                style: {
+                                    cursor: "pointer",
+                                    color: "darkblue"
+                                },
+                                children: (0, Fr.jsxs)("b", {
+                                    children: [(0, Fr.jsx)("u", {
+                                        children: "AuthToken"
+                                    }), "\xa0", Do.UpArrow]
+                                })
+                            }), (0, Fr.jsx)("br", {})]
+                        })]
+                    }), B.get("environ.AWS_LAMBDA_LOG_GROUP_NAME") && B.get("environ.AWS_LAMBDA_LOG_STREAM_NAME") && (0, Fr.jsx)(Fr.Fragment, {
+                        children: (0, Fr.jsxs)(xh, {
+                            info: B,
+                            title: "Logs",
+                            children: [(0, Fr.jsx)(Nh, {
+                                name: "Log Group",
+                                value: B.get("environ.AWS_LAMBDA_LOG_GROUP_NAME"),
+                                monospace: !0,
+                                size: "2"
+                            }), (0, Fr.jsx)(Nh, {
+                                name: "Log Stream",
+                                value: B.get("environ.AWS_LAMBDA_LOG_STREAM_NAME"),
+                                monospace: !0,
+                                size: "2"
+                            })]
+                        })
+                    }), B.get("app.lambda") && (0, Fr.jsxs)(xh, {
+                        info: B,
+                        title: "Lambda",
+                        show: !1,
+                        children: [(0, Fr.jsx)(Nh, {
+                            name: "Name",
+                            value: B.get("app.lambda.lambda_name"),
+                            monospace: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Function",
+                            value: B.get("app.lambda.lambda_function_name"),
+                            monospace: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "ARN",
+                            value: B.get("app.lambda.lambda_function_arn"),
+                            monospace: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "S3 Location",
+                            value: B.get("app.lambda.lambda_code_s3_bucket") + "/" + B.get("app.lambda.lambda_code_s3_bucket_key"),
+                            monospace: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Size",
+                            value: B.get("app.lambda.lambda_code_size"),
+                            monospace: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Modified",
+                            value: Pr.FormatDateTime(B.get("app.lambda.lambda_modified")),
+                            monospace: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Role",
+                            value: B.get("app.lambda.lambda_role"),
+                            monospace: !0,
+                            size: "2"
+                        })]
+                    }), (0, Fr.jsxs)(xh, {
+                        info: B,
+                        title: "Miscellany",
+                        children: [V ? (0, Fr.jsxs)(Fr.Fragment, {
+                            children: [(0, Fr.jsx)("div", {
+                                id: "tooltip-info-reloading",
+                                style: {
+                                    float: "right"
+                                },
+                                children: (0, Fr.jsx)(No, {
+                                    condition: V,
+                                    label: "",
+                                    color: "darkblue"
+                                })
+                            }), (0, Fr.jsx)(Yi, {
+                                id: "tooltip-info-reloading",
+                                position: "bottom",
+                                size: "small",
+                                text: "Reloading the Foursight app."
+                            })]
+                        }) : (0, Fr.jsxs)(Fr.Fragment, {
+                            children: [(0, Fr.jsx)("b", {
+                                onClick: function() {
+                                    return q(!0), void J("/__reloadlambda__", {
+                                        onDone: function() {
+                                            return q(!1)
+                                        }
+                                    })
+                                },
+                                id: "tooltip-info-reload",
+                                style: {
+                                    float: "right",
+                                    cursor: "pointer"
+                                },
+                                children: Do.Refresh
+                            }), (0, Fr.jsx)(Yi, {
+                                id: "tooltip-info-reload",
+                                position: "bottom",
+                                size: "small",
+                                text: "Click here to reload the Foursight app."
+                            })]
+                        }), (0, Fr.jsxs)("div", {
+                            id: "tooltip-info-clear",
+                            style: {
+                                float: "right",
+                                marginTop: "-1px",
+                                marginRight: "4pt",
+                                cursor: "pointer"
+                            },
+                            children: ["\xa0\xa0", (0, Fr.jsx)("img", {
+                                alt: "Clear Cache",
+                                src: Ut.ClearCache(),
+                                height: "19",
+                                onClick: function() {
+                                    J(zt.Url("/__clearcache__", !1))
+                                }
+                            })]
+                        }), (0, Fr.jsx)(Yi, {
+                            id: "tooltip-info-clear",
+                            position: "bottom",
+                            size: "small",
+                            text: "Click to clear any server-side caches."
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "App Deployed At",
+                            value: zt.IsLocal() ? "running locally" + (Je.IsLocalCrossOrigin() ? " (cross-origin)" : "") : (null === (N = R.app) || void 0 === N ? void 0 : N.deployed) + Pr.FormatDuration(null === (I = R.app) || void 0 === I ? void 0 : I.deployed, new Date, !0, "just now", "|", "ago"),
+                            monospace: !0,
+                            copy: !0,
+                            optional: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "App Launched At",
+                            value: (null === (D = R.app) || void 0 === D ? void 0 : D.launched) + Pr.FormatDuration(null === (S = R.app) || void 0 === S ? void 0 : S.launched, new Date, !0, "just now", "|", "ago"),
+                            monospace: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Page Loaded At",
+                            value: B.get("page.loaded") + Pr.FormatDuration(B.get("page.loaded"), new Date, !0, "just now", "|", "ago"),
+                            monospace: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Package",
+                            value: null === (L = R.app) || void 0 === L ? void 0 : L.package,
+                            monospace: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Stage",
+                            value: null === (k = R.app) || void 0 === k ? void 0 : k.stage,
+                            monospace: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Environment",
+                            value: At.Current(),
+                            monospace: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Domain",
+                            value: null === (C = R.app) || void 0 === C ? void 0 : C.domain,
+                            monospace: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Context",
+                            value: null === (E = R.app) || void 0 === E ? void 0 : E.context,
+                            monospace: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Path",
+                            value: B.get("page.path"),
+                            monospace: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Endpoint",
+                            value: B.get("page.endpoint"),
+                            monospace: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Client (React UI)",
+                            value: kr.BaseUrl(),
+                            monospace: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Server (React API)",
+                            value: zt.BaseUrl(),
+                            monospace: !0,
+                            size: "2"
+                        }), (0, Fr.jsx)(Nh, {
+                            name: "Checks File",
+                            value: null === (_ = B.data) || void 0 === _ || null === (T = _.checks) || void 0 === T ? void 0 : T.file,
+                            monospace: !0,
+                            size: "2"
+                        }), (null === (A = R.app) || void 0 === A ? void 0 : A.accounts_file) && (0, Fr.jsx)(Nh, {
+                            name: "Accounts File",
+                            value: null === (O = R.app) || void 0 === O ? void 0 : O.accounts_file,
+                            monospace: !0,
+                            size: "2"
+                        }), (null === (z = R.app) || void 0 === z ? void 0 : z.accounts_file_from_s3) && (0, Fr.jsx)(Nh, {
+                            name: "Accounts File (S3)",
+                            value: null === (U = R.app) || void 0 === U ? void 0 : U.accounts_file_from_s3,
+                            monospace: !0,
+                            size: "2"
+                        })]
+                    }), (0, Fr.jsx)(xh, {
+                        info: B,
+                        title: "GAC: ".concat(B.get("gac.name")),
+                        show: !1,
+                        children: B.get("gac.values") ? (0, Fr.jsx)("span", {
+                            children: Object.keys(B.get("gac.values")).map((function(e) {
+                                return (0, Fr.jsx)(Nh, {
+                                    name: e,
+                                    value: B.get("gac.values")[e],
+                                    monospace: !0,
+                                    copy: !0
+                                }, e)
+                            }))
+                        }) : (0, Fr.jsx)("span", {})
+                    }), (0, Fr.jsx)(xh, {
+                        info: B,
+                        title: "Environment Variables",
+                        show: !1,
+                        children: B.get("environ") ? (0, Fr.jsx)("span", {
+                            children: Object.keys(B.get("environ")).map((function(e) {
+                                return (0, Fr.jsx)(Nh, {
+                                    name: e,
+                                    value: B.get("environ")[e],
+                                    monospace: !0,
+                                    copy: !0
+                                }, e)
+                            }))
+                        }) : (0, Fr.jsx)("span", {})
+                    }), (null === (P = R.app) || void 0 === P ? void 0 : P.accounts) && (0, Fr.jsx)("div", {
+                        className: "container",
+                        style: {
+                            marginTop: "4pt"
+                        },
+                        children: W ? (0, Fr.jsx)(Fr.Fragment, {
+                            children: (0, Fr.jsx)(Hi, {})
+                        }) : (0, Fr.jsxs)(Fr.Fragment, {
+                            children: [(0, Fr.jsx)("b", {
+                                onClick: function() {
+                                    return H(!0)
+                                },
+                                style: {
+                                    cursor: "pointer"
+                                },
+                                children: "Show Accounts"
+                            }), (0, Fr.jsxs)("div", {
+                                className: "box",
+                                children: ["Click ", (0, Fr.jsx)("b", {
+                                    onClick: function() {
+                                        return H(!0)
+                                    },
+                                    style: {
+                                        cursor: "pointer"
+                                    },
+                                    children: "here"
+                                }), " to ", (0, Fr.jsx)("span", {
+                                    onClick: function() {
+                                        return H(!0)
+                                    },
+                                    style: {
+                                        cursor: "pointer"
+                                    },
+                                    children: "show"
+                                }), "."]
+                            })]
+                        })
+                    })]
+                })
+            },
+            Dh = function(e) {
                 var t = a(Re(), 1)[0],
                     n = t.get("code"),
                     r = t.get("state"),
                     o = sessionStorage.getItem("oauth_state"),
                     i = sessionStorage.getItem("ouath_pkce_key"),
                     s = fe(),
                     u = "".concat(zt.Url("/cognito/callback", !1), "?code=").concat(n, "&code_verifier=").concat(i, "&state=").concat(r, "&state_verifier=").concat(o),
@@ -68304,28 +68551,27 @@
                     var c = bt.Get("signinvia");
                     return (0, Fr.jsx)("div", {
                         style: {
                             transform: "scale(1.1)",
                             marginTop: "10pt",
                             marginBottom: "40pt"
                         },
-                        children: (0, Fr.jsx)(yh, {
+                        children: (0, Fr.jsx)(oh, {
                             children: (0, Fr.jsx)(No, {
                                 condition: l.loading,
                                 color: Ft.GetForegroundColor(),
                                 bold: !1,
                                 size: 140,
                                 label: "Signing in via ".concat(c)
                             })
                         })
                     })
                 }
             },
-            wh = __webpack_require__(9712),
-            jh = function(e) {
+            Sh = function(e) {
                 var n, r, o, i, s, u, l, c, d, f, p, h, g = co(),
                     y = a((0, t.useState)(!1), 2),
                     m = y[0],
                     v = y[1],
                     M = a((0, t.useState)(!1), 2),
                     b = M[0],
                     w = M[1],
@@ -68371,15 +68617,15 @@
                                 theme: {
                                     primaryColor: "blue",
                                     backgroundColor: "blue",
                                     logo: ""
                                 },
                                 allowedConnections: null === x || void 0 === x || null === (o = x.data) || void 0 === o ? void 0 : o.connections
                             };
-                            return new wh.default(null === x || void 0 === x || null === (i = x.data) || void 0 === i ? void 0 : i.client, null === x || void 0 === x || null === (a = x.data) || void 0 === a ? void 0 : a.domain, s)
+                            return new qa.default(null === x || void 0 === x || null === (i = x.data) || void 0 === i ? void 0 : i.client, null === x || void 0 === x || null === (a = x.data) || void 0 === a ? void 0 : a.domain, s)
                         }().show(), navigator.userAgent.toLowerCase().indexOf("firefox") > -1 && (document.getElementById("login_auth_container").style.height = "200", document.getElementById("login_auth_container").style.background = "white", document.getElementById("login_auth_container").style.borderStyle = "none"), document.getElementById("login_auth_container").firstChild.firstChild.style.paddingLeft = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.paddingRight = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.paddingTop = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.paddingBottom = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.fontWeight = "bold", document.getElementById("login_auth_container").firstChild.firstChild.style.fontWeight = "bold", v(!0)
                 }
                 if ((g.loading || x.loading) && !g.error) return (0, Fr.jsx)(Fr.Fragment, {
                     children: "Loading ..."
                 });
                 if (g.error) return (0, Fr.jsx)(Xi, {
                     error: g.error,
@@ -68423,15 +68669,17 @@
                                     position: "bottom",
                                     text: "AWS Account Alias: ".concat(null === g || void 0 === g || null === (c = g.app) || void 0 === c || null === (d = c.credentials) || void 0 === d ? void 0 : d.aws_account_name)
                                 })]
                             }), (0, Fr.jsx)("br", {})]
                         })]
                     })
                 };
-                return I ? (0, Fr.jsx)(gh, {
+                return dh.IsFatalError(g) ? (0, Fr.jsx)(dh, {
+                    header: g
+                }) : I ? (0, Fr.jsx)(rh, {
                     hide: function() {
                         return D(!1)
                     }
                 }) : (0, Fr.jsx)(Fr.Fragment, {
                     children: Br.IsLoggedIn(g) ? (0, Fr.jsx)(t.Fragment, {
                         children: (0, Fr.jsxs)("div", {
                             className: "container",
@@ -68560,15 +68808,15 @@
                                         padding: "9pt",
                                         color: "darkred"
                                     },
                                     children: ["Note that though you are logged in, you do not have permission to access the currently selected environment: ", (0, Fr.jsx)("b", {
                                         style: {
                                             color: "red"
                                         },
-                                        children: At.Current()
+                                        children: At.PreferredName(At.Current(), g)
                                     }), " ", (0, Fr.jsx)("br", {}), (0, Fr.jsxs)("small", {
                                         children: ["Click ", (0, Fr.jsx)(qi, {
                                             to: "/env",
                                             children: (0, Fr.jsx)("u", {
                                                 children: "here"
                                             })
                                         }), " to go the the ", (0, Fr.jsx)(qi, {
@@ -69050,15 +69298,15 @@
                                     j && !m && T()
                                 }), 10), "")]
                             })]
                         })]
                     })
                 })
             },
-            xh = function(e) {
+            Lh = function(e) {
                 var n = co(),
                     r = pe().environCompare,
                     o = a((0, t.useState)(!1), 2),
                     i = o[0],
                     s = o[1],
                     u = a((0, t.useState)("all"), 2),
                     l = u[0],
@@ -69404,15 +69652,15 @@
                                 display: "none"
                             },
                             children: d.yaml()
                         })]
                     })
                 })
             },
-            Nh = function(e) {
+            kh = function(e) {
                 return {
                     __get: function(t, n, r, o) {
                         var i = e.findIndex((function(e) {
                             return e.type === t
                         }));
                         if (i >= 0) {
                             var a = n ? "".concat(t, ".").concat(n) : t;
@@ -69425,16 +69673,16 @@
                                 }
                             }
                         }
                         return null
                     }
                 }
             },
-            Ih = function(e) {
-                e = Nh(e);
+            Ch = function(e) {
+                e = kh(e);
                 var n = a((0, t.useState)([]), 2),
                     r = n[0],
                     o = n[1];
                 return (0, t.useState)({
                     count: function() {
                         return r.length
                     },
@@ -69479,23 +69727,23 @@
                     __unselect: function(e) {
                         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null,
                             n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : null;
                         null == n && (n = this.__lookup(e, t)), n >= 0 && (r.splice(n, 1), o(u(r)))
                     }
                 })[0]
             },
-            Dh = function(e) {
+            Eh = function(e) {
                 var t;
                 return "function" == typeof e && (e = e()), (null === (t = e) || void 0 === t ? void 0 : t.constructor) === Object ? e : {}
             },
-            Sh = function(e, t) {
+            _h = function(e, t) {
                 return "function" == typeof e && (e = e()), void 0 !== e ? e : {}
             };
 
-        function Lh(e) {
+        function Th(e) {
             var t, n, r = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : void 0,
                 o = !(arguments.length > 2 && void 0 !== arguments[2]) || arguments[2];
             if (Object.is(e, r))
                 if ((null === (n = e) || void 0 === n ? void 0 : n.constructor) === Object) e = Ye({}, e);
                 else if (Array.isArray(e)) {
                 var i = function(e) {
                     var t = u(e),
@@ -69510,24 +69758,24 @@
                     return t
                 };
                 e = i(e)
             } else "function" === typeof e && (e = e(r));
             else(null === (t = e) || void 0 === t ? void 0 : t.constructor) === Object && (null === r || void 0 === r ? void 0 : r.constructor) === Object && o && (e = Ye(Ye({}, r), e));
             return e
         }
-        var kh = function(e, n) {
+        var Ah = function(e, n) {
                 var r = !0 === (null === e || void 0 === e ? void 0 : e.__keyedState) ? !0 === e.__keyedStateUsage ? e : e.keyed("default") : null,
-                    o = r ? r.__state() ? r.__state() : Sh(n) : Dh(e),
+                    o = r ? r.__state() ? r.__state() : _h(n) : Eh(e),
                     i = a((0, t.useState)(o), 2),
                     s = i[0],
                     u = i[1];
                 return (0, t.useEffect)((function() {
-                    o && r && !r.__state() && r.__updateState(Lh(o, s, !0))
+                    o && r && !r.__state() && r.__updateState(Th(o, s, !0))
                 }), []), r ? [s, function(e) {
-                    e = Lh(e, s, !0), u(e), r.__updateState(e)
+                    e = Th(e, s, !0), u(e), r.__updateState(e)
                 }] : {
                     __keyedState: !0,
                     key: null,
                     keyed: function(e) {
                         var t;
                         if (!0 === this.__keyedState) {
                             (null === (t = e) || void 0 === t ? void 0 : t.constructor) === String && 0 !== e.length || (e = "default");
@@ -69551,27 +69799,27 @@
                                     return s[e]
                                 }
                             }
                         }
                     }
                 }
             },
-            Ch = {
+            Oh = {
                 color: "var(--box-fg)",
                 fontWeight: "bold",
                 paddingTop: "1pt",
                 verticalAlign: "top",
                 width: "5%",
                 paddingRight: "8pt",
                 whiteSpace: "nowrap"
             },
-            Eh = {
+            zh = {
                 verticalAlign: "top"
             },
-            _h = function(e) {
+            Uh = function(e) {
                 var t = e.showVpcs,
                     n = e.toggleVpcs,
                     r = e.showSecurityGroups,
                     o = e.toggleSecurityGroups,
                     i = e.showSubnetsPublic,
                     a = e.toggleSubnetsPublic,
                     s = e.showSubnetsPrivate,
@@ -69624,15 +69872,15 @@
                             },
                             onClick: o,
                             children: "Security Groups"
                         })]
                     })]
                 })
             },
-            Th = function(e) {
+            Ph = function(e) {
                 var t = e.showGac,
                     n = e.toggleGac,
                     r = e.showEcosystem,
                     o = e.toggleEcosystem;
                 return (0, Fr.jsx)(Fr.Fragment, {
                     children: (0, Fr.jsxs)("div", {
                         className: "box margin thickborder",
@@ -69657,15 +69905,15 @@
                             },
                             onClick: o,
                             children: "Ecosystem Definition"
                         })]
                     })
                 })
             },
-            Ah = function(e) {
+            Rh = function(e) {
                 var t, n, r = e.keyedState,
                     o = e.hide,
                     i = "true" === (null === (t = Re()[0]) || void 0 === t || null === (n = t.get("all")) || void 0 === n ? void 0 : n.toLowerCase()),
                     a = so("/aws/vpcs".concat(i ? "/all" : ""), {
                         cache: !0
                     });
                 return (0, Fr.jsxs)("div", {
@@ -69704,27 +69952,27 @@
                                 marginTop: "2pt"
                             },
                             children: (0, Fr.jsx)(No, {
                                 label: "Loading VPCs"
                             })
                         }), a.map((function(e) {
                             return (0, Fr.jsx)("div", {
-                                children: (0, Fr.jsx)(Oh, {
+                                children: (0, Fr.jsx)(Bh, {
                                     vpc: e,
                                     keyedState: null === r || void 0 === r ? void 0 : r.keyed(e.id)
                                 })
                             }, e.id)
                         }))]
                     })]
                 })
             },
-            Oh = function(e) {
+            Bh = function(e) {
                 var t = e.vpc,
                     n = e.keyedState,
-                    r = a(kh(n), 2),
+                    r = a(Ah(n), 2),
                     o = r[0],
                     i = r[1],
                     s = function(e) {
                         return o[e]
                     },
                     u = function(e) {
                         return i(Be({}, e, !o[e]))
@@ -69770,42 +70018,42 @@
                                 }
                             })]
                         }), (0, Fr.jsx)("table", {
                             width: "100%",
                             children: (0, Fr.jsxs)("tbody", {
                                 children: [(0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "ID:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: t.id
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.stack) && (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Stack:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: null === t || void 0 === t ? void 0 : t.stack
                                     })]
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "CIDR:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: null === t || void 0 === t ? void 0 : t.cidr
                                     })]
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Status:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: null === t || void 0 === t ? void 0 : t.status
                                     })]
                                 }), (0, Fr.jsx)("tr", {
                                     children: (0, Fr.jsx)("td", {
                                         style: {
                                             height: "2pt"
                                         },
@@ -69828,15 +70076,15 @@
                                     })
                                 }), (0, Fr.jsxs)("tr", {
                                     onClick: function() {
                                         return t.id, u("showSubnetsPublic")
                                     },
                                     className: "pointer",
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Public Subnets:"
                                     }), (0, Fr.jsx)("td", {
                                         children: l() ? (0, Fr.jsx)(Fr.Fragment, {
                                             children: (0, Fr.jsx)("small", {
                                                 children: (0, Fr.jsxs)("u", {
                                                     children: ["Hide\xa0", Do.DownArrowHollow]
                                                 })
@@ -69852,29 +70100,29 @@
                                 }), l() && (0, Fr.jsx)(Fr.Fragment, {
                                     children: (0, Fr.jsx)("tr", {
                                         children: (0, Fr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Fr.jsx)(zh, {
+                                            children: (0, Fr.jsx)(Fh, {
                                                 type: "public",
                                                 vpcId: null === t || void 0 === t ? void 0 : t.id,
                                                 notitle: !0,
                                                 keyedState: null === n || void 0 === n ? void 0 : n.keyed("subnets-public")
                                             })
                                         })
                                     })
                                 }), (0, Fr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showSubnetsPrivate")
                                     },
                                     className: "pointer",
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Private Subnets:"
                                     }), (0, Fr.jsx)("td", {
                                         children: c() ? (0, Fr.jsx)(Fr.Fragment, {
                                             children: (0, Fr.jsx)("small", {
                                                 children: (0, Fr.jsxs)("u", {
                                                     children: ["Hide\xa0", Do.DownArrowHollow]
                                                 })
@@ -69890,29 +70138,29 @@
                                 }), c() && (0, Fr.jsx)(Fr.Fragment, {
                                     children: (0, Fr.jsx)("tr", {
                                         children: (0, Fr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Fr.jsx)(zh, {
+                                            children: (0, Fr.jsx)(Fh, {
                                                 type: "private",
                                                 vpcId: null === t || void 0 === t ? void 0 : t.id,
                                                 notitle: !0,
                                                 keyedState: null === n || void 0 === n ? void 0 : n.keyed("subnets-private")
                                             })
                                         })
                                     })
                                 }), (0, Fr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showSecurityGroups")
                                     },
                                     className: "pointer",
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Security Groups:"
                                     }), (0, Fr.jsx)("td", {
                                         children: d() ? (0, Fr.jsx)(Fr.Fragment, {
                                             children: (0, Fr.jsx)("small", {
                                                 children: (0, Fr.jsxs)("u", {
                                                     children: ["Hide\xa0", Do.DownArrowHollow]
                                                 })
@@ -69928,28 +70176,28 @@
                                 }), d() && (0, Fr.jsx)(Fr.Fragment, {
                                     children: (0, Fr.jsx)("tr", {
                                         children: (0, Fr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Fr.jsx)(Ph, {
+                                            children: (0, Fr.jsx)(Qh, {
                                                 vpcId: null === t || void 0 === t ? void 0 : t.id,
                                                 notitle: !0,
                                                 keyedState: null === n || void 0 === n ? void 0 : n.keyed("security-groups")
                                             })
                                         })
                                     })
                                 }), (0, Fr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showTags")
                                     },
                                     className: "pointer",
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Tags:"
                                     }), (0, Fr.jsx)("td", {
                                         children: f() ? (0, Fr.jsx)(Fr.Fragment, {
                                             children: (0, Fr.jsx)("small", {
                                                 children: (0, Fr.jsxs)("u", {
                                                     children: ["Hide\xa0", Do.DownArrowHollow]
                                                 })
@@ -69965,26 +70213,26 @@
                                 }), f() && (0, Fr.jsx)(Fr.Fragment, {
                                     children: (0, Fr.jsx)("tr", {
                                         children: (0, Fr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Fr.jsx)(Yh, {
+                                            children: (0, Fr.jsx)(Zh, {
                                                 tags: null === t || void 0 === t ? void 0 : t.tags
                                             })
                                         })
                                     })
                                 })]
                             })
                         })]
                     })
                 })
             },
-            zh = function(e) {
+            Fh = function(e) {
                 var t, n, r = e.vpcId,
                     o = e.type,
                     i = e.hide,
                     a = e.notitle,
                     s = e.keyedState,
                     u = "true" === (null === (t = Re()[0].get("all")) || void 0 === t ? void 0 : t.toLowerCase()),
                     l = r ? "?vpc=".concat(r) : "",
@@ -70023,31 +70271,31 @@
                             children: (0, Fr.jsx)(No, {
                                 label: "Loading Subnets"
                             })
                         }), null === (n = c.filter((function(e) {
                             return !o || e.type === o
                         }))) || void 0 === n ? void 0 : n.map((function(e) {
                             return (0, Fr.jsxs)("div", {
-                                children: [(0, Fr.jsx)(Uh, {
+                                children: [(0, Fr.jsx)(Yh, {
                                     subnet: e,
                                     keyedState: null === s || void 0 === s ? void 0 : s.keyed(e.id)
                                 }), (0, Fr.jsx)("div", {
                                     style: {
                                         height: "4pt"
                                     }
                                 })]
                             }, e.id)
                         }))]
                     })]
                 })
             },
-            Uh = function(e) {
+            Yh = function(e) {
                 var t = e.subnet,
                     n = e.keyedState,
-                    r = a(kh(n), 2),
+                    r = a(Ah(n), 2),
                     o = r[0],
                     i = r[1],
                     s = function() {
                         return o["showTags"]
                     };
                 return (0, Fr.jsx)(Fr.Fragment, {
                     children: (0, Fr.jsxs)("div", {
@@ -70095,60 +70343,60 @@
                                 })
                             })]
                         }), (0, Fr.jsx)("table", {
                             width: "100%",
                             children: (0, Fr.jsxs)("tbody", {
                                 children: [(0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "ID:"
                                     }), (0, Fr.jsxs)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: [null === t || void 0 === t ? void 0 : t.id, (0, Fr.jsx)("br", {}), (0, Fr.jsx)("small", {
                                             children: null === t || void 0 === t ? void 0 : t.subnet_arn
                                         })]
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.stack) && (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Stack:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: null === t || void 0 === t ? void 0 : t.stack
                                     })]
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "CIDR:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: null === t || void 0 === t ? void 0 : t.cidr
                                     })]
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Zone:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: null === t || void 0 === t ? void 0 : t.zone
                                     })]
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "VPC:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: null === t || void 0 === t ? void 0 : t.vpc
                                     })]
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Status:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: null === t || void 0 === t ? void 0 : t.status
                                     })]
                                 }), (0, Fr.jsx)("tr", {
                                     children: (0, Fr.jsx)("td", {
                                         style: {
                                             height: "4pt"
                                         },
@@ -70172,15 +70420,15 @@
                                 }), (0, Fr.jsxs)("tr", {
                                     onClick: function() {
                                         return i(Be({}, e = "showTags", !o[e]));
                                         var e
                                     },
                                     className: "pointer",
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Tags:"
                                     }), (0, Fr.jsx)("td", {
                                         children: s() ? (0, Fr.jsx)(Fr.Fragment, {
                                             children: (0, Fr.jsx)("small", {
                                                 children: (0, Fr.jsxs)("u", {
                                                     children: ["Hide\xa0", Do.DownArrowHollow]
                                                 })
@@ -70196,26 +70444,26 @@
                                 }), s() && (0, Fr.jsx)(Fr.Fragment, {
                                     children: (0, Fr.jsx)("tr", {
                                         children: (0, Fr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Fr.jsx)(Yh, {
+                                            children: (0, Fr.jsx)(Zh, {
                                                 tags: null === t || void 0 === t ? void 0 : t.tags
                                             })
                                         })
                                     })
                                 })]
                             })
                         })]
                     })
                 })
             },
-            Ph = function(e) {
+            Qh = function(e) {
                 var t, n = e.vpcId,
                     r = e.notitle,
                     o = e.keyedState,
                     i = e.hide,
                     a = "true" === (null === (t = Re()[0].get("all")) || void 0 === t ? void 0 : t.toLowerCase()),
                     s = n ? "?vpc=".concat(n) : "",
                     u = so("/aws/security_groups".concat(a ? "/all" : "").concat(s), {
@@ -70251,31 +70499,31 @@
                                 marginTop: "2pt"
                             },
                             children: (0, Fr.jsx)(No, {
                                 label: "Loading security groups"
                             })
                         }), u.map((function(e) {
                             return (0, Fr.jsxs)("div", {
-                                children: [(0, Fr.jsx)(Rh, {
+                                children: [(0, Fr.jsx)(Gh, {
                                     securityGroup: e,
                                     keyedState: null === o || void 0 === o ? void 0 : o.keyed(e.id)
                                 }), (0, Fr.jsx)("div", {
                                     style: {
                                         height: "4pt"
                                     }
                                 })]
                             }, e.id)
                         }))]
                     })]
                 })
             },
-            Rh = function(e) {
+            Gh = function(e) {
                 var t = e.securityGroup,
                     n = e.keyedState,
-                    r = a(kh(n), 2),
+                    r = a(Ah(n), 2),
                     o = r[0],
                     i = r[1],
                     s = function(e) {
                         return o[e]
                     },
                     u = function(e) {
                         return i(Be({}, e, !o[e]))
@@ -70317,47 +70565,47 @@
                                 }
                             })]
                         }), (0, Fr.jsx)("table", {
                             width: "100%",
                             children: (0, Fr.jsxs)("tbody", {
                                 children: [(0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "ID:"
                                     }), (0, Fr.jsxs)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: [null === t || void 0 === t ? void 0 : t.id, (0, Fr.jsx)("br", {}), (0, Fr.jsx)("small", {
                                             children: null === t || void 0 === t ? void 0 : t.securityGroup
                                         })]
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.stack) && (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Stack:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: null === t || void 0 === t ? void 0 : t.stack
                                     })]
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Description:"
                                     }), (0, Fr.jsx)("td", {
                                         style: {
                                             whiteSpace: "break-spaces",
                                             wordBreak: "break-all"
                                         },
                                         children: null === t || void 0 === t ? void 0 : t.description
                                     })]
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "VPC:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: null === t || void 0 === t ? void 0 : t.vpc
                                     })]
                                 }), (0, Fr.jsx)("tr", {
                                     children: (0, Fr.jsx)("td", {
                                         style: {
                                             height: "4pt"
                                         },
@@ -70380,15 +70628,15 @@
                                     })
                                 }), (0, Fr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showInboundRules")
                                     },
                                     className: "pointer",
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Inbound Rules:"
                                     }), (0, Fr.jsx)("td", {
                                         children: l() ? (0, Fr.jsx)(Fr.Fragment, {
                                             children: (0, Fr.jsxs)("small", {
                                                 children: [(0, Fr.jsx)("u", {
                                                     children: "Hide"
                                                 }), "\xa0", Do.DownArrowHollow]
@@ -70404,27 +70652,27 @@
                                 }), l() && (0, Fr.jsx)(Fr.Fragment, {
                                     children: (0, Fr.jsx)("tr", {
                                         children: (0, Fr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Fr.jsx)(Bh, {
+                                            children: (0, Fr.jsx)(Wh, {
                                                 securityGroupId: null === t || void 0 === t ? void 0 : t.id,
                                                 direction: "inbound"
                                             })
                                         })
                                     })
                                 }), (0, Fr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showOutboundRules")
                                     },
                                     className: "pointer",
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Outbound Rules:"
                                     }), (0, Fr.jsx)("td", {
                                         children: c() ? (0, Fr.jsx)(Fr.Fragment, {
                                             children: (0, Fr.jsx)("small", {
                                                 children: (0, Fr.jsxs)("u", {
                                                     children: ["Hide\xa0", Do.DownArrowHollow]
                                                 })
@@ -70440,27 +70688,27 @@
                                 }), c() && (0, Fr.jsx)(Fr.Fragment, {
                                     children: (0, Fr.jsx)("tr", {
                                         children: (0, Fr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Fr.jsx)(Bh, {
+                                            children: (0, Fr.jsx)(Wh, {
                                                 securityGroupId: null === t || void 0 === t ? void 0 : t.id,
                                                 direction: "outbound"
                                             })
                                         })
                                     })
                                 }), (0, Fr.jsxs)("tr", {
                                     onClick: function() {
                                         return u("showTags")
                                     },
                                     className: "pointer",
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Tags:"
                                     }), (0, Fr.jsx)("td", {
                                         children: d() ? (0, Fr.jsx)(Fr.Fragment, {
                                             children: (0, Fr.jsx)("small", {
                                                 children: (0, Fr.jsxs)("u", {
                                                     children: ["Hide\xa0", Do.DownArrowHollow]
                                                 })
@@ -70476,26 +70724,26 @@
                                 }), d() && (0, Fr.jsx)(Fr.Fragment, {
                                     children: (0, Fr.jsx)("tr", {
                                         children: (0, Fr.jsx)("td", {
                                             style: {
                                                 paddingTop: "2pt"
                                             },
                                             colSpan: "2",
-                                            children: (0, Fr.jsx)(Yh, {
+                                            children: (0, Fr.jsx)(Zh, {
                                                 tags: null === t || void 0 === t ? void 0 : t.tags
                                             })
                                         })
                                     })
                                 })]
                             })
                         })]
                     })
                 })
             },
-            Bh = function(e) {
+            Wh = function(e) {
                 var t = e.securityGroupId,
                     n = e.direction,
                     r = "inbound" === n ? "?direction=inbound" : "outbound" === n ? "?direction=outbound" : "",
                     o = so("/aws/security_group_rules/".concat(t).concat(r), {
                         cache: !0
                     });
                 return (0, Fr.jsxs)(Fr.Fragment, {
@@ -70505,26 +70753,26 @@
                             paddingBottom: "10pt"
                         },
                         children: (0, Fr.jsx)(No, {
                             label: "Loading security group rules"
                         })
                     }), null === o || void 0 === o ? void 0 : o.map((function(e) {
                         return (0, Fr.jsxs)("div", {
-                            children: [(0, Fr.jsx)(Fh, {
+                            children: [(0, Fr.jsx)(Hh, {
                                 securityGroupRule: e
                             }), (0, Fr.jsx)("div", {
                                 style: {
                                     height: "4pt"
                                 }
                             })]
                         }, e.id)
                     }))]
                 })
             },
-            Fh = function(e) {
+            Hh = function(e) {
                 var t = e.securityGroupRule;
 
                 function n(e) {
                     var t, n;
                     if ("TCP" === (null === e || void 0 === e || null === (t = e.protocol) || void 0 === t ? void 0 : t.toUpperCase())) {
                         if (22 === (null === e || void 0 === e ? void 0 : e.port_from) && 22 === (null === e || void 0 === e ? void 0 : e.port_thru)) return "SSH";
                         if (443 === (null === e || void 0 === e ? void 0 : e.port_from) && 443 === (null === e || void 0 === e ? void 0 : e.port_thru)) return "HTTPS";
@@ -70579,78 +70827,78 @@
                                 }
                             })]
                         }), (0, Fr.jsx)("table", {
                             width: "100%",
                             children: (0, Fr.jsxs)("tbody", {
                                 children: [(0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Direction:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: null !== t && void 0 !== t && t.egress ? "Outbound" : "Inbound"
                                     })]
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Protocol:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: r(t)
                                     })]
                                 }), n(t) !== r(t) && (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Type:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: n(t)
                                     })]
                                 }), o(t) && (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Port:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: o(t)
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.cidr) && (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "CIDR:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: null === t || void 0 === t ? void 0 : t.cidr
                                     })]
                                 }), (null === t || void 0 === t ? void 0 : t.description) && (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Description:"
                                     }), (0, Fr.jsx)("td", {
                                         style: {
                                             whiteSpace: "break-spaces",
                                             wordBreak: "break-all"
                                         },
                                         children: null === t || void 0 === t ? void 0 : t.description
                                     })]
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Security Group:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: null === t || void 0 === t ? void 0 : t.security_group
                                     })]
                                 })]
                             })
                         })]
                     })
                 })
             },
-            Yh = function(e) {
+            Zh = function(e) {
                 var t;
                 return (0, Fr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
                     children: (0, Fr.jsx)("div", {
                         className: "box lighten",
@@ -70685,15 +70933,15 @@
                             children: (0, Fr.jsx)("li", {
                                 children: "No tags."
                             })
                         })
                     })
                 })
             },
-            Qh = function(e) {
+            Vh = function(e) {
                 var t = so("/aws/stacks", {
                         cache: !0
                     }),
                     n = {
                         cursor: "pointer"
                     },
                     r = Ye(Ye({}, n), {}, {
@@ -70724,19 +70972,19 @@
                                 },
                                 children: o.name
                             }, o.name)
                         }))]
                     })]
                 })
             },
-            Gh = function(e) {
+            qh = function(e) {
                 var t, n, r, o, i, s, u, l, c, d, f, p, h = e.stackName,
                     g = e.keyedState,
                     y = e.hide,
-                    m = a(kh(g), 2),
+                    m = a(Ah(g), 2),
                     v = m[0],
                     M = m[1],
                     b = so("/aws/stacks/".concat(h), {
                         cache: !0
                     }),
                     w = function(e) {
                         return v[e]
@@ -70788,56 +71036,56 @@
                         children: b.loading ? (0, Fr.jsx)(No, {
                             label: "Loading stack info"
                         }) : (0, Fr.jsx)("table", {
                             width: "100%",
                             children: (0, Fr.jsxs)("tbody", {
                                 children: [(0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Name:"
                                     }), (0, Fr.jsxs)("td", {
-                                        style: Ye(Ye({}, Eh), {}, {
+                                        style: Ye(Ye({}, zh), {}, {
                                             wordBreak: "break-all"
                                         }),
                                         children: [(0, Fr.jsx)("b", {
                                             style: {
                                                 float: "right",
                                                 cursor: "pointer",
                                                 marginTop: "-2pt"
                                             },
                                             onClick: y,
                                             children: Do.X
                                         }), h]
                                     })]
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "ID:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Ye(Ye({}, Eh), {}, {
+                                        style: Ye(Ye({}, zh), {}, {
                                             wordBreak: "break-all"
                                         }),
                                         children: (0, Fr.jsx)("small", {
                                             children: null === (n = b.data) || void 0 === n ? void 0 : n.id
                                         })
                                     })]
                                 }), (null === (r = b.data) || void 0 === r ? void 0 : r.role_arn) && (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Role:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: (null === (o = b.data) || void 0 === o ? void 0 : o.role_arn) || Do.EmptySet
                                     })]
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Description:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: null === (i = b.data) || void 0 === i ? void 0 : i.description
                                     })]
                                 }), (0, Fr.jsx)("tr", {
                                     children: (0, Fr.jsx)("td", {
                                         style: {
                                             height: "2pt"
                                         },
@@ -70856,34 +71104,34 @@
                                         style: {
                                             height: "2pt"
                                         },
                                         colSpan: "2"
                                     })
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Status:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: null === (s = b.data) || void 0 === s ? void 0 : s.status
                                     })]
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Created:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: null === (u = b.data) || void 0 === u ? void 0 : u.created
                                     })]
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Updated:"
                                     }), (0, Fr.jsx)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: null === (l = b.data) || void 0 === l ? void 0 : l.updated
                                     })]
                                 }), (0, Fr.jsx)("tr", {
                                     children: (0, Fr.jsx)("td", {
                                         style: {
                                             height: "2pt"
                                         },
@@ -70902,18 +71150,18 @@
                                         style: {
                                             height: "2pt"
                                         },
                                         colSpan: "2"
                                     })
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Outputs:"
                                     }), (0, Fr.jsxs)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: [x() ? (0, Fr.jsx)(Fr.Fragment, {
                                             children: (0, Fr.jsx)("small", {
                                                 className: "pointer",
                                                 onClick: N,
                                                 children: (0, Fr.jsxs)("u", {
                                                     children: ["Hide\xa0", Do.DownArrowHollow]
                                                 })
@@ -70938,25 +71186,25 @@
                                 }), x() && (0, Fr.jsx)(Fr.Fragment, {
                                     children: (0, Fr.jsx)("tr", {
                                         children: (0, Fr.jsx)("td", {
                                             colSpan: "2",
                                             style: {
                                                 paddingTop: "2pt"
                                             },
-                                            children: (0, Fr.jsx)(Wh, {
+                                            children: (0, Fr.jsx)(Jh, {
                                                 stackName: h
                                             })
                                         })
                                     })
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Parameters:"
                                     }), (0, Fr.jsxs)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: [I() ? (0, Fr.jsx)(Fr.Fragment, {
                                             children: (0, Fr.jsx)("small", {
                                                 className: "pointer",
                                                 onClick: D,
                                                 children: (0, Fr.jsxs)("u", {
                                                     children: ["Hide\xa0", Do.DownArrowHollow]
                                                 })
@@ -70981,25 +71229,25 @@
                                 }), I() && (0, Fr.jsx)(Fr.Fragment, {
                                     children: (0, Fr.jsx)("tr", {
                                         children: (0, Fr.jsx)("td", {
                                             colSpan: "2",
                                             style: {
                                                 paddingTop: "2pt"
                                             },
-                                            children: (0, Fr.jsx)(Hh, {
+                                            children: (0, Fr.jsx)(Kh, {
                                                 stackName: h
                                             })
                                         })
                                     })
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Resources:"
                                     }), (0, Fr.jsxs)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: [S() ? (0, Fr.jsx)(Fr.Fragment, {
                                             children: (0, Fr.jsx)("small", {
                                                 className: "pointer",
                                                 onClick: L,
                                                 children: (0, Fr.jsxs)("u", {
                                                     children: ["Hide\xa0", Do.DownArrowHollow]
                                                 })
@@ -71024,25 +71272,25 @@
                                 }), S() && (0, Fr.jsx)(Fr.Fragment, {
                                     children: (0, Fr.jsx)("tr", {
                                         children: (0, Fr.jsx)("td", {
                                             colSpan: "2",
                                             style: {
                                                 paddingTop: "2pt"
                                             },
-                                            children: (0, Fr.jsx)(Zh, {
+                                            children: (0, Fr.jsx)(Xh, {
                                                 stackName: h
                                             })
                                         })
                                     })
                                 }), (0, Fr.jsxs)("tr", {
                                     children: [(0, Fr.jsx)("td", {
-                                        style: Ch,
+                                        style: Oh,
                                         children: "Template:"
                                     }), (0, Fr.jsxs)("td", {
-                                        style: Eh,
+                                        style: zh,
                                         children: [k() ? (0, Fr.jsx)(Fr.Fragment, {
                                             children: (0, Fr.jsx)("small", {
                                                 className: "pointer",
                                                 onClick: C,
                                                 children: (0, Fr.jsxs)("u", {
                                                     children: ["Hide\xa0", Do.DownArrowHollow]
                                                 })
@@ -71067,26 +71315,26 @@
                                 }), k() && (0, Fr.jsx)(Fr.Fragment, {
                                     children: (0, Fr.jsx)("tr", {
                                         children: (0, Fr.jsx)("td", {
                                             colSpan: "2",
                                             style: {
                                                 paddingTop: "2pt"
                                             },
-                                            children: (0, Fr.jsx)(Vh, {
+                                            children: (0, Fr.jsx)($h, {
                                                 stackName: h
                                             })
                                         })
                                     })
                                 })]
                             })
                         })
                     })]
                 })
             },
-            Wh = function(e) {
+            Jh = function(e) {
                 var t, n = so("/aws/stacks/".concat(e.stackName, "/outputs"), {
                     cache: !0
                 });
                 return (0, Fr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
@@ -71129,15 +71377,15 @@
                                     }, e)
                                 })))
                             })
                         })
                     })
                 })
             },
-            Hh = function(e) {
+            Kh = function(e) {
                 var t, n = so("/aws/stacks/".concat(e.stackName, "/parameters"), {
                     cache: !0
                 });
                 return (0, Fr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
@@ -71180,15 +71428,15 @@
                                     }, e)
                                 })))
                             })
                         })
                     })
                 })
             },
-            Zh = function(e) {
+            Xh = function(e) {
                 var t, n = so("/aws/stacks/".concat(e.stackName, "/resources"), {
                     cache: !0
                 });
                 return (0, Fr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
@@ -71234,15 +71482,15 @@
                                     }, e)
                                 })))
                             })
                         })
                     })
                 })
             },
-            Vh = function(e) {
+            $h = function(e) {
                 var t = so("/aws/stacks/".concat(e.stackName, "/template"), {
                     cache: !0
                 });
                 return (0, Fr.jsx)("div", {
                     style: {
                         maxWidth: "480pt"
                     },
@@ -71269,15 +71517,15 @@
                                 },
                                 children: st.IsObject(t.data) ? qr.Format(t.data) : t.data
                             })
                         })
                     })
                 })
             },
-            qh = function(e) {
+            eg = function(e) {
                 var t, n, r, o, i, a, s = e.hide,
                     u = so("/info", {
                         cache: !0
                     });
                 return (0, Fr.jsxs)("div", {
                     style: {
                         maxWidth: "500pt",
@@ -71328,15 +71576,15 @@
                                     }) : u.data.gac.values[e]]
                                 }, e)
                             })))
                         })]
                     })]
                 })
             },
-            Jh = function(e) {
+            tg = function(e) {
                 var t, n, r, o, i = e.hide,
                     a = so("/info", {
                         cache: !0
                     });
                 return (0, Fr.jsxs)("div", {
                     style: {
                         maxWidth: "500pt",
@@ -71362,81 +71610,81 @@
                         className: "box margin",
                         children: [a.loading && (0, Fr.jsx)(No, {
                             label: "Loading Ecosystem"
                         }), !a.loading && qr.Format(null === (r = a.data) || void 0 === r || null === (o = r.buckets) || void 0 === o ? void 0 : o.ecosystem)]
                     })]
                 })
             },
-            Kh = function() {
-                var e = kh(),
+            ng = function() {
+                var e = Ah(),
                     n = [{
                         type: "stack",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Fr.jsx)(Gh, {
+                            return (0, Fr.jsx)(qh, {
                                 stackName: e,
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "vpcs",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Fr.jsx)(Ah, {
+                            return (0, Fr.jsx)(Rh, {
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "subnets-public",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Fr.jsx)(zh, {
+                            return (0, Fr.jsx)(Fh, {
                                 type: "public",
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "subnets-private",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Fr.jsx)(zh, {
+                            return (0, Fr.jsx)(Fh, {
                                 type: "private",
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "security-groups",
                         create: function(e, t, n, r) {
                             var o = r.keyedState;
-                            return (0, Fr.jsx)(Ph, {
+                            return (0, Fr.jsx)(Qh, {
                                 keyedState: o.keyed(t),
                                 hide: n
                             })
                         }
                     }, {
                         type: "gac",
                         create: function(e, t, n, r) {
-                            return (0, Fr.jsx)(qh, {
+                            return (0, Fr.jsx)(eg, {
                                 hide: n
                             })
                         }
                     }, {
                         type: "ecosystem",
                         create: function(e, t, n, r) {
-                            return (0, Fr.jsx)(Jh, {
+                            return (0, Fr.jsx)(tg, {
                                 hide: n
                             })
                         }
                     }],
-                    r = Ih(n),
-                    o = Ih(n);
+                    r = Ch(n),
+                    o = Ch(n);
                 var i = function() {
                         return r.toggle("vpcs")
                     },
                     a = function() {
                         return r.toggle("ecosystem")
                     };
                 return (0, t.useEffect)((function() {
@@ -71445,15 +71693,15 @@
                     children: (0, Fr.jsx)("tbody", {
                         children: (0, Fr.jsxs)("tr", {
                             children: [(0, Fr.jsxs)("td", {
                                 style: {
                                     verticalAlign: "top",
                                     paddingRight: "8pt"
                                 },
-                                children: [(0, Fr.jsx)(_h, {
+                                children: [(0, Fr.jsx)(Uh, {
                                     keyedState: e,
                                     showVpcs: function() {
                                         return r.selected("vpcs")
                                     },
                                     toggleVpcs: i,
                                     showSubnetsPublic: function() {
                                         return o.selected("subnets-public")
@@ -71469,26 +71717,26 @@
                                     },
                                     showSecurityGroups: function() {
                                         return o.selected("security-groups")
                                     },
                                     toggleSecurityGroups: function() {
                                         return o.toggle("security-groups")
                                     }
-                                }), (0, Fr.jsx)(Th, {
+                                }), (0, Fr.jsx)(Ph, {
                                     showGac: function() {
                                         return r.selected("gac")
                                     },
                                     toggleGac: function() {
                                         return r.toggle("gac")
                                     },
                                     showEcosystem: function() {
                                         return r.selected("ecosystem")
                                     },
                                     toggleEcosystem: a
-                                }), (0, Fr.jsx)(Qh, {
+                                }), (0, Fr.jsx)(Vh, {
                                     toggleStack: function(e) {
                                         return r.toggle("stack", e)
                                     },
                                     selectedStack: function(e) {
                                         return r.selected("stack", e)
                                     }
                                 })]
@@ -71517,15 +71765,15 @@
                                     }, t.key)
                                 }))
                             })]
                         })
                     })
                 })
             },
-            Xh = function(e) {
+            rg = function(e) {
                 var t = co();
                 return (0, Fr.jsx)(Fr.Fragment, {
                     children: (0, Fr.jsx)("div", {
                         className: "container",
                         id: "login_container",
                         children: (0, Fr.jsxs)("div", {
                             className: "boxstyle check-warn",
@@ -71554,22 +71802,22 @@
                                     })
                                 }), " page."]
                             })]
                         })
                     })
                 })
             },
-            $h = function() {
+            og = function() {
                 var e = ce().state.url;
                 return e.startsWith(window.location.origin) && (e = e.substring(window.location.origin.length)), (0, Fr.jsx)(xe, {
                     to: e,
                     replace: !0
                 })
             },
-            eg = function() {
+            ig = function() {
                 var e = so("/users/projects", {
                         cache: !0
                     }),
                     t = so("/users/roles", {
                         cache: !0
                     }),
                     n = so("/users/institutions", {
@@ -71627,15 +71875,15 @@
                             return (null === e || void 0 === e ? void 0 : e.map((function(e) {
                                 return o.title(e)
                             })).join(", ")) || ""
                         }
                     };
                 return o
             },
-            tg = [{
+            ag = [{
                 name: "email",
                 label: "Email Address",
                 type: "email",
                 focus: !0,
                 required: !0
             }, {
                 name: "first_name",
@@ -71680,38 +71928,38 @@
                 label: "Updated",
                 readonly: !0
             }, {
                 name: "uuid",
                 label: "UUID",
                 readonly: !0
             }],
-            ng = {
+            sg = {
                 PrincipalInvestigatorLine: function(e) {
                     var t, n, r = e.institution,
-                        o = eg();
+                        o = ig();
                     return (0, Fr.jsx)("div", {
                         style: e.style,
                         children: o.principleInvestigator(r) && (0, Fr.jsxs)("small", {
                             children: [(0, Fr.jsxs)("b", {
                                 children: ["Principle Investigator ", Do.RightArrow]
                             }), " ", null === (t = o.principleInvestigator(r)) || void 0 === t ? void 0 : t.name, "\xa0", (0, Fr.jsx)($i, {
                                 href: kr.Path("/users/".concat(null === (n = o.principleInvestigator(r)) || void 0 === n ? void 0 : n.uuid))
                             })]
                         })
                     })
                 },
                 useUserInputs: function() {
                     var e = co(),
-                        n = At.IsFoursightFourfront(e) ? tg.filter((function(e) {
+                        n = At.IsFoursightFourfront(e) ? ag.filter((function(e) {
                             return "project" !== e.name && "role" !== e.name && "institution" !== e.name
-                        })) : tg;
+                        })) : ag;
                     return (0, t.useState)(Tr.Clone(Tr.Clone(n)))
                 }
             },
-            rg = function(e) {
+            ug = function(e) {
                 var t = so("/users/".concat(e.email, "?raw=true"));
                 return (0, Fr.jsxs)("pre", {
                     className: "box",
                     children: [(0, Fr.jsx)("span", {
                         style: {
                             float: "right",
                             marginTop: "-6pt",
@@ -71725,15 +71973,15 @@
                     }), t.loading ? (0, Fr.jsx)(Fr.Fragment, {
                         children: (0, Fr.jsx)(No, {})
                     }) : (0, Fr.jsx)(Fr.Fragment, {
                         children: qr.Format(t.data)
                     })]
                 })
             },
-            og = function(e) {
+            lg = function(e) {
                 var n = {
                         color: "var(--box-fg)",
                         fontWeight: "bold",
                         fontSize: "small",
                         paddingTop: "1pt",
                         verticalAlign: "top",
                         width: "5%",
@@ -71842,16 +72090,16 @@
                                     })]
                                 }, o.name)
                             }))
                         })
                     })
                 })
             },
-            ig = function(e) {
-                var t = eg(),
+            cg = function(e) {
+                var t = ig(),
                     n = [{
                         label: "Email",
                         name: "email"
                     }, {
                         label: "First Name",
                         name: "first_name"
                     }, {
@@ -71874,26 +72122,26 @@
                         name: "role",
                         map: function(n) {
                             return t.userRoleTitle(e.user, e.user.project)
                         }
                     }, {
                         label: "Roles",
                         name: "roles",
-                        ui: (0, Fr.jsx)(ag, {
+                        ui: (0, Fr.jsx)(dg, {
                             user: e.user
                         }),
                         toggle: !0
                     }, {
                         label: "Institution",
                         name: "institution",
                         map: function(e) {
                             return t.institutionTitle(e)
                         },
                         subComponent: function(e) {
-                            return (0, Fr.jsx)(ng.PrincipalInvestigatorLine, {
+                            return (0, Fr.jsx)(sg.PrincipalInvestigatorLine, {
                                 institution: e
                             })
                         }
                     }, {
                         label: "Status",
                         name: "status",
                         map: function(e) {
@@ -71913,22 +72161,22 @@
                         }
                     }, {
                         label: "UUID",
                         name: "uuid"
                     }];
                 return At.IsFoursightFourfront(co()) && (n = n.filter((function(e) {
                     return "institution" !== e.name && "project" !== e.name && "roles" !== e.name && "role" !== e.name
-                }))), (0, Fr.jsx)(og, {
+                }))), (0, Fr.jsx)(lg, {
                     keys: n,
                     value: e.user,
                     separators: !0
                 })
             },
-            ag = function(e) {
-                var t = eg();
+            dg = function(e) {
+                var t = ig();
                 return (0, Fr.jsx)("div", {
                     className: "box lighten",
                     style: {
                         marginTop: "2pt",
                         marginBottom: "2pt"
                     },
                     children: (0, Fr.jsx)("table", {
@@ -71991,15 +72239,15 @@
                                     })]
                                 }, e.project)
                             }))]
                         })
                     })
                 })
             },
-            sg = function(e) {
+            fg = function(e) {
                 var n, r, o, i = pe().email,
                     s = a((0, t.useState)(!1), 2),
                     u = s[0],
                     l = s[1],
                     c = fe();
                 var d = so({
                     url: "/users/".concat(i),
@@ -72115,25 +72363,25 @@
                                             float: "right",
                                             fontSize: "small",
                                             marginTop: "-1pt",
                                             marginRight: "2pt"
                                         },
                                         children: "Edit"
                                     })]
-                                }), u ? (0, Fr.jsx)(rg, {
+                                }), u ? (0, Fr.jsx)(ug, {
                                     email: e.email
-                                }) : (0, Fr.jsx)(ig, {
+                                }) : (0, Fr.jsx)(cg, {
                                     user: e
                                 })]
                             }, e.uuid)
                         }))]
                     })
                 })
             },
-            ug = function(e) {
+            pg = function(e) {
                 var n = so(e.url, {
                         nofetch: !0,
                         cache: !0
                     }),
                     r = a((0, t.useState)(e.selected), 2),
                     o = r[0],
                     i = r[1];
@@ -72166,15 +72414,15 @@
                             }, e.id) : null
                         }))]
                     }), e.subComponent && (0, Fr.jsx)(Fr.Fragment, {
                         children: e.subComponent(o)
                     })]
                 })
             },
-            lg = function(e) {
+            hg = function(e) {
                 var n = e.inputs,
                     r = (e.setInputs, e.title, e.loading),
                     o = e.onCreate,
                     i = e.onUpdate,
                     u = e.onDelete,
                     l = e.onCancel,
                     c = e.onRefresh,
@@ -72426,15 +72674,15 @@
                                                         }), (0, Fr.jsx)("option", {
                                                             value: !0,
                                                             children: "True"
                                                         })]
                                                     })
                                                 }) : (0, Fr.jsx)(Fr.Fragment, {
                                                     children: "select" === e.type ? (0, Fr.jsx)(Fr.Fragment, {
-                                                        children: (0, Fr.jsx)(ug, {
+                                                        children: (0, Fr.jsx)(pg, {
                                                             id: e.name,
                                                             url: e.url,
                                                             required: e.required,
                                                             selected: z(e),
                                                             onChange: T,
                                                             disabled: F() || e.readonly,
                                                             setLoadingCount: S,
@@ -72610,28 +72858,28 @@
                                     })]
                                 })
                             })
                         })
                     })
                 })
             },
-            cg = function() {
+            gg = function() {
                 var e = so(zt.Url("/users"), {
                         method: "POST",
                         nofetch: !0
                     }),
-                    n = a(ng.useUserInputs(), 2),
+                    n = a(sg.useUserInputs(), 2),
                     r = n[0],
                     o = (n[1], fe());
                 return (0, t.useEffect)((function() {
                     var e = r.find((function(e) {
                         return "institution" === e.name
                     }));
                     e && (e.subComponent = function(e) {
-                        return (0, Fr.jsx)(ng.PrincipalInvestigatorLine, {
+                        return (0, Fr.jsx)(sg.PrincipalInvestigatorLine, {
                             institution: e
                         })
                     })
                 }), []), (0, Fr.jsx)("center", {
                     children: (0, Fr.jsx)("table", {
                         children: (0, Fr.jsxs)("tbody", {
                             children: [(0, Fr.jsx)("tr", {
@@ -72658,15 +72906,15 @@
                                                 children: "List"
                                             })
                                         })
                                     })]
                                 })
                             }), (0, Fr.jsx)("tr", {
                                 children: (0, Fr.jsx)("td", {
-                                    children: (0, Fr.jsx)(lg, {
+                                    children: (0, Fr.jsx)(hg, {
                                         title: "Edit User",
                                         inputs: r,
                                         onCreate: function(t) {
                                             t.admin ? (delete t.admin, t = Ye(Ye({}, t), {}, {
                                                 groups: ["admin"]
                                             })) : (delete t.admin, t = Ye(Ye({}, t), {}, {
                                                 groups: []
@@ -72686,17 +72934,17 @@
                                     })
                                 })
                             })]
                         })
                     })
                 })
             },
-            dg = function() {
+            yg = function() {
                 var e = pe().uuid,
-                    n = a(ng.useUserInputs(), 2),
+                    n = a(sg.useUserInputs(), 2),
                     r = n[0],
                     o = n[1],
                     i = a((0, t.useState)(!1), 2),
                     l = i[0],
                     c = i[1],
                     d = a(ra(), 1)[0],
                     f = so({
@@ -72720,27 +72968,27 @@
                                 return u(t)
                             }))
                         },
                         onError: function(e) {
                             404 === e.status && c(!0)
                         }
                     }),
-                    p = eg(),
+                    p = ig(),
                     h = fe();
 
                 function g() {
                     h(kr.Path("/users/".concat(e)))
                 }
                 return (0, t.useEffect)((function() {
                     f.fetch();
                     var e = r.find((function(e) {
                         return "institution" === e.name
                     }));
                     e && (e.subComponent = function(e) {
-                        return (0, Fr.jsx)(ng.PrincipalInvestigatorLine, {
+                        return (0, Fr.jsx)(sg.PrincipalInvestigatorLine, {
                             institution: e
                         })
                     })
                 }), [e]), (0, Fr.jsx)("center", {
                     children: (0, Fr.jsx)("table", {
                         children: (0, Fr.jsxs)("tbody", {
                             children: [(0, Fr.jsx)("tr", {
@@ -72781,15 +73029,15 @@
                                             children: ["The specified user was not found: ", e, " ", (0, Fr.jsx)("p", {}), (0, Fr.jsx)("button", {
                                                 className: "button cancel",
                                                 onClick: g,
                                                 children: "Cancel"
                                             })]
                                         })
                                     }) : (0, Fr.jsx)(Fr.Fragment, {
-                                        children: (0, Fr.jsx)(lg, {
+                                        children: (0, Fr.jsx)(hg, {
                                             title: "Edit User",
                                             inputs: r,
                                             setInputs: o,
                                             onUpdate: function(t) {
                                                 var n, r = (null === (n = f.get("groups")) || void 0 === n ? void 0 : n.filter((function(e) {
                                                     return "admin" !== e
                                                 }))) || [];
@@ -72824,15 +73072,15 @@
                                     })
                                 })
                             })]
                         })
                     })
                 })
             },
-            fg = function(e) {
+            mg = function(e) {
                 var n, r = e.columns,
                     o = e.data,
                     i = e.update,
                     s = e.initialSort,
                     u = e.children,
                     l = a(Re(), 2),
                     c = l[0],
@@ -73012,27 +73260,27 @@
                             }), (0, Fr.jsx)("tbody", {
                                 children: u
                             })]
                         })
                     })]
                 })
             },
-            pg = function() {
+            vg = function() {
                 var e = pe().environ,
                     n = a(Re(), 2),
                     r = n[0],
                     o = n[1],
                     i = so(),
                     s = a((0, t.useState)(r.get("search") || ""), 2),
                     u = s[0],
                     l = s[1],
                     c = a((0, t.useState)(it.HasValue(u)), 2),
                     d = c[0],
                     f = c[1],
-                    p = eg();
+                    p = ig();
 
                 function h(t) {
                     var n = t.limit,
                         o = t.offset,
                         a = t.sort,
                         s = t.search,
                         u = t.onDone;
@@ -73159,15 +73407,15 @@
                                 style: {
                                     height: "1px",
                                     background: Ft.GetForegroundColor(),
                                     marginTop: "2pt",
                                     marginBottom: "4pt"
                                 }
                             })]
-                        }), (0, Fr.jsx)(fg, {
+                        }), (0, Fr.jsx)(mg, {
                             columns: [{
                                 label: ""
                             }, {
                                 label: "User",
                                 key: "email"
                             }, {
                                 label: "Groups",
@@ -73296,30 +73544,30 @@
                                     })]
                                 }, e.uuid)
                             }))
                         })]
                     })
                 })
             },
-            hg = function() {
+            Mg = function() {
                 var e = co();
 
                 function t() {
                     return "/api/react/".concat(At.PreferredName(At.Default(e)), "/login")
                 }
                 return (0, Fr.jsx)(Ae, {
-                    children: (0, Fr.jsxs)(rs, {
-                        children: [(0, Fr.jsx)(ns, {}), (0, Fr.jsx)("div", {
+                    children: (0, Fr.jsxs)(wh, {
+                        children: [(0, Fr.jsx)(bh, {}), (0, Fr.jsx)("div", {
                             style: {
                                 margin: "14pt"
                             },
                             children: (0, Fr.jsxs)(De, {
                                 children: [(0, Fr.jsx)(Ne, {
                                     path: "/api/react/cognito/callback",
-                                    element: (0, Fr.jsx)(bh, {})
+                                    element: (0, Fr.jsx)(Dh, {})
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/",
                                     element: (0, Fr.jsx)(xe, {
                                         to: t()
                                     })
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/api",
@@ -73340,110 +73588,110 @@
                                     path: "/api/react/:environ/accounts",
                                     element: (0, Fr.jsx)(Hr.AuthorizationRequired, {
                                         children: (0, Fr.jsx)(Zi, {})
                                     })
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/api/react/:environ/env",
                                     element: (0, Fr.jsx)(Hr.KnownEnvRequired, {
-                                        children: (0, Fr.jsx)(qa, {})
+                                        children: (0, Fr.jsx)(fh, {})
                                     })
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/api/react/env",
                                     element: (0, Fr.jsx)(Hr.KnownEnvRequired, {
-                                        children: (0, Fr.jsx)(qa, {})
+                                        children: (0, Fr.jsx)(fh, {})
                                     })
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/api/react/:environ/login",
                                     element: (0, Fr.jsx)(Hr.KnownEnvRequired, {
-                                        children: (0, Fr.jsx)(jh, {})
+                                        children: (0, Fr.jsx)(Sh, {})
                                     })
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/api/react/:environ/checks",
                                     element: (0, Fr.jsx)(Hr.AuthorizationRequired, {
                                         children: (0, Fr.jsx)(Ra, {})
                                     })
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/api/react/:environ/checks/:check/history",
                                     element: (0, Fr.jsx)(Hr.AuthorizationRequired, {
                                         children: (0, Fr.jsx)(Za, {})
                                     })
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/api/react/:environ/home",
                                     element: (0, Fr.jsx)(Hr.AuthorizationRequired, {
-                                        children: (0, Fr.jsx)(os, {})
+                                        children: (0, Fr.jsx)(jh, {})
                                     })
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/api/react/:environ/info",
                                     element: (0, Fr.jsx)(Hr.AuthorizationRequired, {
-                                        children: (0, Fr.jsx)(ss, {})
+                                        children: (0, Fr.jsx)(Ih, {})
                                     })
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/api/react/:environ/users",
                                     element: (0, Fr.jsx)(Hr.AuthorizationRequired, {
-                                        children: (0, Fr.jsx)(pg, {})
+                                        children: (0, Fr.jsx)(vg, {})
                                     })
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/api/react/:environ/users/:email",
                                     element: (0, Fr.jsx)(Hr.AuthorizationRequired, {
-                                        children: (0, Fr.jsx)(sg, {})
+                                        children: (0, Fr.jsx)(fg, {})
                                     })
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/api/react/:environ/users/edit/:uuid",
                                     element: (0, Fr.jsx)(Hr.AuthorizationRequired, {
-                                        children: (0, Fr.jsx)(dg, {})
+                                        children: (0, Fr.jsx)(yg, {})
                                     })
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/api/react/:environ/users/create",
                                     element: (0, Fr.jsx)(Hr.AuthorizationRequired, {
-                                        children: (0, Fr.jsx)(cg, {})
+                                        children: (0, Fr.jsx)(gg, {})
                                     })
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/api/react/:environ/gac/:environCompare",
                                     element: (0, Fr.jsx)(Hr.AuthorizationRequired, {
-                                        children: (0, Fr.jsx)(xh, {})
+                                        children: (0, Fr.jsx)(Lh, {})
                                     })
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/api/react/:environ/aws/s3",
                                     element: (0, Fr.jsx)(Hr.AuthorizationRequired, {
                                         children: (0, Fr.jsx)(ta, {})
                                     })
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/api/react/:environ/aws/infrastructure",
                                     element: (0, Fr.jsx)(Hr.AuthorizationRequired, {
-                                        children: (0, Fr.jsx)(Kh, {})
+                                        children: (0, Fr.jsx)(ng, {})
                                     })
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/api/react/:environ/forbidden",
-                                    element: (0, Fr.jsx)(Ka, {})
+                                    element: (0, Fr.jsx)(hh, {})
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "/redirect",
-                                    element: (0, Fr.jsx)($h, {})
+                                    element: (0, Fr.jsx)(og, {})
                                 }), (0, Fr.jsx)(Ne, {
                                     path: "*",
                                     element: (0, Fr.jsx)(Hr.AuthorizationRequired, {
-                                        children: (0, Fr.jsx)(Xh, {})
+                                        children: (0, Fr.jsx)(rg, {})
                                     })
                                 })]
                             })
-                        }), (0, Fr.jsx)(Ja, {})]
+                        }), (0, Fr.jsx)(ph, {})]
                     })
                 })
             },
-            gg = r.createRoot(document.getElementById("root"));
-        "1" === bt.Get("test_mode_strict_mode") ? gg.render((0, Fr.jsx)(t.StrictMode, {
-            children: (0, Fr.jsx)(hg, {})
-        })) : gg.render((0, Fr.jsx)("table", {
+            bg = r.createRoot(document.getElementById("root"));
+        "1" === bt.Get("test_mode_strict_mode") ? bg.render((0, Fr.jsx)(t.StrictMode, {
+            children: (0, Fr.jsx)(Mg, {})
+        })) : bg.render((0, Fr.jsx)("table", {
             style: {
                 width: "100%"
             },
             cellPadding: "0",
             cellSpacing: "0",
             children: (0, Fr.jsx)("tbody", {
                 children: (0, Fr.jsx)("tr", {
                     children: (0, Fr.jsx)("td", {
-                        children: (0, Fr.jsx)(hg, {})
+                        children: (0, Fr.jsx)(Mg, {})
                     })
                 })
             })
         }))
     }()
 })();
```

### Comparing `foursight_core-3.3.2.2b1/foursight_core/route_prefixes.py` & `foursight_core-4.1.0.1b0/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/routes.py` & `foursight_core-4.1.0.1b0/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/run_result.py` & `foursight_core-4.1.0.1b0/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/s3_connection.py` & `foursight_core-4.1.0.1b0/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/schedule_decorator.py` & `foursight_core-4.1.0.1b0/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/scripts/decrypt_accounts_file.py` & `foursight_core-4.1.0.1b0/foursight_core/scripts/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/scripts/encrypt_accounts_file.py` & `foursight_core-4.1.0.1b0/foursight_core/scripts/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/sqs_utils.py` & `foursight_core-4.1.0.1b0/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/stage.py` & `foursight_core-4.1.0.1b0/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/templates/base.html` & `foursight_core-4.1.0.1b0/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/templates/header.html` & `foursight_core-4.1.0.1b0/foursight_core/templates/header.html`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
                             <span class="dropdown-content">
                                 {% for environment in environments %}
                                     {% if environment["name"].upper() == env.upper() or environment["public_name"].upper() == env.upper() or environment["full_name"].upper() == env.upper() or environment["short_name"].upper() == env.upper() or environment["foursight_name"].upper() == env.upper() %}
                                         <span>{{environment["public_name"]}}&nbsp;&nbsp;&#x2713;</span>
                                     {% else %}
                                         <a href="{{request.context.path.replace('/' + env, '/' + environment['public_name'])}}" onclick="this.style.color = 'yellow'; this.style.backgroundColor = '#143c53'; this.style.fontWeight = 'bold';">{{environment["public_name"]}}</a>
                                     {% endif %}
-                                {% endfor %}     
+                                {% endfor %}
                             </span>
                          </span>
                     {% else %}
                         <b style="color:#143c53" title="Environment: {{env}}">{{env}}</b>
                     {% endif %}
                     &nbsp;|&nbsp;
                     {% if stage == 'prod' %}
@@ -404,15 +404,15 @@
         r.selectNode(document.getElementById(id));
         window.getSelection().removeAllRanges();
         window.getSelection().addRange(r);
         document.execCommand('copy');
         window.getSelection().removeAllRanges();
     }
     function delete_login_cookies() {
-        document.cookie = "jwtToken=; expires=Thu, 01 Jan 1970 00:00:00 UTC; path=/; domain=" + location.hostname + ";";
+        document.cookie = "c4_st=; expires=Thu, 01 Jan 1970 00:00:00 UTC; path=/; domain=" + location.hostname + ";";
     }
 </script>
 {% block script %}{% endblock %}
 </body>
 <br /><p /><br />
 <center>
 <table width="100%">
```

### Comparing `foursight_core-3.3.2.2b1/foursight_core/templates/history.html` & `foursight_core-4.1.0.1b0/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/templates/info.html` & `foursight_core-4.1.0.1b0/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/templates/unused.html` & `foursight_core-4.1.0.1b0/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/templates/user.html` & `foursight_core-4.1.0.1b0/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/templates/users.html` & `foursight_core-4.1.0.1b0/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/templates/view_checks.html` & `foursight_core-4.1.0.1b0/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/foursight_core/templates/view_groups.html` & `foursight_core-4.1.0.1b0/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-3.3.2.2b1/PKG-INFO` & `foursight_core-4.1.0.1b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 3.3.2.2b1
+Version: 4.1.0.1b0
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (==2.10.1)
 Requires-Dist: MarkupSafe (==1.1.1)
-Requires-Dist: PyJWT (==2.5.0)
+Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: cron-descriptor (>=1.2.31,<2.0.0)
 Requires-Dist: cryptography (==39.0.0)
-Requires-Dist: dcicutils (>=6.8.0,<7.0.0)
+Requires-Dist: dcicutils (==7.2.0.1b0)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google (>=3.0.0,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.12.5,<2.0.0)
 Requires-Dist: google-auth-oauthlib (>=0.7.0,<0.8.0)
 Requires-Dist: pyDes (>=2.0.1,<3.0.0)
-Requires-Dist: pytz (>=2020.1,<2021.0)
+Requires-Dist: pytz (>=2020.1)
+Requires-Dist: redis (>=4.5.1,<5.0.0)
```

