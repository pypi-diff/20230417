# Comparing `tmp/hdn-research-environment-1.5.2.tar.gz` & `tmp/hdn-research-environment-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hdn-research-environment-1.5.2.tar", last modified: Thu Apr 13 13:51:39 2023, max compression
+gzip compressed data, was "dist/hdn-research-environment-1.5.3.tar", last modified: Mon Apr 17 10:46:27 2023, max compression
```

## Comparing `hdn-research-environment-1.5.2.tar` & `hdn-research-environment-1.5.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-1.5.2/LICENSE
--rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-1.5.2/MANIFEST.in
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-1.5.2/README.md
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/__init__.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/environment/api/
--rw-r--r--   0 karolszuster   (501) staff       (20)     2906 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.2/environment/api/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      749 2023-02-11 18:26:19.000000 hdn-research-environment-1.5.2/environment/api/auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      663 2023-02-11 18:26:19.000000 hdn-research-environment-1.5.2/environment/api/decorators.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/environment/api/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/api/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1392 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.2/environment/api/tests/test_auth.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1543 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.2/environment/api/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/apps.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3042 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.2/environment/constants.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1298 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1619 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/deserializers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2904 2023-04-12 08:30:41.000000 hdn-research-environment-1.5.2/environment/entities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      547 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/exceptions.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2182 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.2/environment/forms.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/managers.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/environment/migrations/
--rw-r--r--   0 karolszuster   (501) staff       (20)     1444 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/migrations/0001_initial.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1580 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/migrations/0002_billingsetup.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      404 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/migrations/0003_cloudidentity_is_workspace_done.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      421 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/migrations/0004_auto_20220309_0330.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2184 2022-03-29 15:52:24.000000 hdn-research-environment-1.5.2/environment/migrations/0005_workflow.py
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/migrations/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1821 2023-01-20 14:18:52.000000 hdn-research-environment-1.5.2/environment/models.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    14537 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.2/environment/services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     2556 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.2/environment/signals.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/environment/static/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/environment/static/environment/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/environment/static/environment/css/
--rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-1.5.2/environment/static/environment/css/create_research_environment.css
--rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/static/environment/css/environment-base.css
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/environment/static/environment/js/
--rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-1.5.2/environment/static/environment/js/cookie.js
--rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-04-13 13:50:19.000000 hdn-research-environment-1.5.2/environment/static/environment/js/gpu_disabling.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     3058 2023-04-12 08:30:41.000000 hdn-research-environment-1.5.2/environment/static/environment/js/pricing_change.js
--rw-r--r--   0 karolszuster   (501) staff       (20)     1658 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.2/environment/tasks.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/environment/templates/
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/environment/templates/environment/
--rw-r--r--   0 karolszuster   (501) staff       (20)     4511 2023-01-20 14:18:52.000000 hdn-research-environment-1.5.2/environment/templates/environment/_available_environments_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/templates/environment/_available_projects_list.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      400 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/templates/environment/_cloud_identity_info.html
--rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-1.5.2/environment/templates/environment/base_environment_home.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     2193 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/templates/environment/billing_setup.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-04-13 13:50:19.000000 hdn-research-environment-1.5.2/environment/templates/environment/create_research_environment.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/environment/templates/environment/email/
--rw-r--r--   0 karolszuster   (501) staff       (20)      416 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/templates/environment/email/environment_access_expired.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1416 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.2/environment/templates/environment/identity_provisioning.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     3866 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/templates/environment/research_environments.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/templates/environment/workspace_being_provisioned.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/environment/templates/tag/
--rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/templates/tag/environment_action_button.html
--rw-r--r--   0 karolszuster   (501) staff       (20)     1422 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/templates/tag/environment_modal_button.html
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/environment/templatetags/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/templatetags/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3460 2023-02-22 22:00:03.000000 hdn-research-environment-1.5.2/environment/templatetags/action_buttons.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/environment/tests/
--rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/tests/__init__.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      974 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/tests/helpers.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    12256 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/tests/mocks.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3977 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.2/environment/tests/test_decorators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    11233 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.2/environment/tests/test_services.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     6444 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.2/environment/tests/test_signals.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     3847 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.2/environment/tests/test_utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      629 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.2/environment/tests/test_validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     7755 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.2/environment/tests/test_views.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1474 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/urls.py
--rw-r--r--   0 karolszuster   (501) staff       (20)     1305 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.2/environment/utilities.py
--rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.2/environment/validators.py
--rw-r--r--   0 karolszuster   (501) staff       (20)    10182 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.2/environment/views.py
-drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/hdn_research_environment.egg-info/
--rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/hdn_research_environment.egg-info/PKG-INFO
--rw-r--r--   0 karolszuster   (501) staff       (20)     2560 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/hdn_research_environment.egg-info/SOURCES.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/hdn_research_environment.egg-info/dependency_links.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/hdn_research_environment.egg-info/requires.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/hdn_research_environment.egg-info/top_level.txt
--rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-1.5.2/pyproject.toml
--rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-04-13 13:51:39.000000 hdn-research-environment-1.5.2/setup.cfg
--rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-1.5.2/setup.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1551 2022-03-29 08:15:30.000000 hdn-research-environment-1.5.3/LICENSE
+-rw-r--r--   0 karolszuster   (501) staff       (20)      115 2022-03-29 08:32:41.000000 hdn-research-environment-1.5.3/MANIFEST.in
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)       90 2022-03-29 07:59:09.000000 hdn-research-environment-1.5.3/README.md
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/__init__.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/api/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2906 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/api/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      749 2023-02-11 18:26:19.000000 hdn-research-environment-1.5.3/environment/api/auth.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      663 2023-02-11 18:26:19.000000 hdn-research-environment-1.5.3/environment/api/decorators.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/api/tests/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/api/tests/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1392 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/api/tests/test_auth.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1543 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/api/tests/test_decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      154 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/apps.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3042 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/constants.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1298 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1619 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/deserializers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2904 2023-04-12 08:30:41.000000 hdn-research-environment-1.5.3/environment/entities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      547 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/exceptions.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2182 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/forms.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      155 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/managers.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/migrations/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1444 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/migrations/0001_initial.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1580 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/migrations/0002_billingsetup.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      404 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/migrations/0003_cloudidentity_is_workspace_done.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      421 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/migrations/0004_auto_20220309_0330.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2184 2022-03-29 15:52:24.000000 hdn-research-environment-1.5.3/environment/migrations/0005_workflow.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/migrations/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1821 2023-01-20 14:18:52.000000 hdn-research-environment-1.5.3/environment/models.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    14537 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2556 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/signals.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/static/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/static/environment/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/static/environment/css/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      342 2023-02-22 22:00:03.000000 hdn-research-environment-1.5.3/environment/static/environment/css/create_research_environment.css
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6583 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/static/environment/css/environment-base.css
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/static/environment/js/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      564 2022-03-30 12:50:58.000000 hdn-research-environment-1.5.3/environment/static/environment/js/cookie.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)      516 2023-04-13 13:50:19.000000 hdn-research-environment-1.5.3/environment/static/environment/js/gpu_disabling.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3058 2023-04-12 08:30:41.000000 hdn-research-environment-1.5.3/environment/static/environment/js/pricing_change.js
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1658 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/tasks.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/templates/
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/templates/environment/
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4511 2023-01-20 14:18:52.000000 hdn-research-environment-1.5.3/environment/templates/environment/_available_environments_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1423 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templates/environment/_available_projects_list.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      400 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templates/environment/_cloud_identity_info.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)      801 2022-03-30 12:51:12.000000 hdn-research-environment-1.5.3/environment/templates/environment/base_environment_home.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2193 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templates/environment/billing_setup.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     4327 2023-04-13 13:50:19.000000 hdn-research-environment-1.5.3/environment/templates/environment/create_research_environment.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/templates/environment/email/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      416 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templates/environment/email/environment_access_expired.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1416 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/templates/environment/identity_provisioning.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3866 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templates/environment/research_environments.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1018 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templates/environment/workspace_being_provisioned.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/templates/tag/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      241 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templates/tag/environment_action_button.html
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1422 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templates/tag/environment_modal_button.html
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/templatetags/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/templatetags/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3460 2023-02-22 22:00:03.000000 hdn-research-environment-1.5.3/environment/templatetags/action_buttons.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/environment/tests/
+-rw-r--r--   0 karolszuster   (501) staff       (20)        0 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/tests/__init__.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      974 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/tests/helpers.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    12256 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/tests/mocks.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3977 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/tests/test_decorators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    11233 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/tests/test_services.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     6444 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/tests/test_signals.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     3847 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/tests/test_utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      629 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/tests/test_validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     7755 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/tests/test_views.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1474 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/urls.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1305 2023-04-13 13:50:11.000000 hdn-research-environment-1.5.3/environment/utilities.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)      236 2022-03-29 08:08:24.000000 hdn-research-environment-1.5.3/environment/validators.py
+-rw-r--r--   0 karolszuster   (501) staff       (20)    10168 2023-04-17 10:45:42.000000 hdn-research-environment-1.5.3/environment/views.py
+drwxr-xr-x   0 karolszuster   (501) staff       (20)        0 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/hdn_research_environment.egg-info/
+-rw-r--r--   0 karolszuster   (501) staff       (20)      995 2023-04-17 10:46:26.000000 hdn-research-environment-1.5.3/hdn_research_environment.egg-info/PKG-INFO
+-rw-r--r--   0 karolszuster   (501) staff       (20)     2560 2023-04-17 10:46:26.000000 hdn-research-environment-1.5.3/hdn_research_environment.egg-info/SOURCES.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)        1 2023-04-17 10:46:26.000000 hdn-research-environment-1.5.3/hdn_research_environment.egg-info/dependency_links.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       84 2023-04-17 10:46:26.000000 hdn-research-environment-1.5.3/hdn_research_environment.egg-info/requires.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)       12 2023-04-17 10:46:26.000000 hdn-research-environment-1.5.3/hdn_research_environment.egg-info/top_level.txt
+-rw-r--r--   0 karolszuster   (501) staff       (20)      109 2022-03-29 08:03:11.000000 hdn-research-environment-1.5.3/pyproject.toml
+-rw-r--r--   0 karolszuster   (501) staff       (20)     1056 2023-04-17 10:46:27.000000 hdn-research-environment-1.5.3/setup.cfg
+-rw-r--r--   0 karolszuster   (501) staff       (20)       38 2022-03-29 08:03:11.000000 hdn-research-environment-1.5.3/setup.py
```

### Comparing `hdn-research-environment-1.5.2/LICENSE` & `hdn-research-environment-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/PKG-INFO` & `hdn-research-environment-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 1.5.2
+Version: 1.5.3
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-1.5.2/environment/api/__init__.py` & `hdn-research-environment-1.5.3/environment/api/__init__.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/api/auth.py` & `hdn-research-environment-1.5.3/environment/api/auth.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/api/decorators.py` & `hdn-research-environment-1.5.3/environment/api/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/api/tests/test_auth.py` & `hdn-research-environment-1.5.3/environment/api/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/api/tests/test_decorators.py` & `hdn-research-environment-1.5.3/environment/api/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/constants.py` & `hdn-research-environment-1.5.3/environment/constants.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/decorators.py` & `hdn-research-environment-1.5.3/environment/decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/deserializers.py` & `hdn-research-environment-1.5.3/environment/deserializers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/entities.py` & `hdn-research-environment-1.5.3/environment/entities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/exceptions.py` & `hdn-research-environment-1.5.3/environment/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/forms.py` & `hdn-research-environment-1.5.3/environment/forms.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/migrations/0001_initial.py` & `hdn-research-environment-1.5.3/environment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/migrations/0002_billingsetup.py` & `hdn-research-environment-1.5.3/environment/migrations/0002_billingsetup.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/migrations/0005_workflow.py` & `hdn-research-environment-1.5.3/environment/migrations/0005_workflow.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/models.py` & `hdn-research-environment-1.5.3/environment/models.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/services.py` & `hdn-research-environment-1.5.3/environment/services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/signals.py` & `hdn-research-environment-1.5.3/environment/signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/static/environment/css/environment-base.css` & `hdn-research-environment-1.5.3/environment/static/environment/css/environment-base.css`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/static/environment/js/cookie.js` & `hdn-research-environment-1.5.3/environment/static/environment/js/cookie.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/static/environment/js/gpu_disabling.js` & `hdn-research-environment-1.5.3/environment/static/environment/js/gpu_disabling.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/static/environment/js/pricing_change.js` & `hdn-research-environment-1.5.3/environment/static/environment/js/pricing_change.js`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/tasks.py` & `hdn-research-environment-1.5.3/environment/tasks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/templates/environment/_available_environments_list.html` & `hdn-research-environment-1.5.3/environment/templates/environment/_available_environments_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/templates/environment/_available_projects_list.html` & `hdn-research-environment-1.5.3/environment/templates/environment/_available_projects_list.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/templates/environment/base_environment_home.html` & `hdn-research-environment-1.5.3/environment/templates/environment/base_environment_home.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/templates/environment/billing_setup.html` & `hdn-research-environment-1.5.3/environment/templates/environment/billing_setup.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/templates/environment/create_research_environment.html` & `hdn-research-environment-1.5.3/environment/templates/environment/create_research_environment.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/templates/environment/identity_provisioning.html` & `hdn-research-environment-1.5.3/environment/templates/environment/identity_provisioning.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/templates/environment/research_environments.html` & `hdn-research-environment-1.5.3/environment/templates/environment/research_environments.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/templates/environment/workspace_being_provisioned.html` & `hdn-research-environment-1.5.3/environment/templates/environment/workspace_being_provisioned.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/templates/tag/environment_modal_button.html` & `hdn-research-environment-1.5.3/environment/templates/tag/environment_modal_button.html`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/templatetags/action_buttons.py` & `hdn-research-environment-1.5.3/environment/templatetags/action_buttons.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/tests/helpers.py` & `hdn-research-environment-1.5.3/environment/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/tests/mocks.py` & `hdn-research-environment-1.5.3/environment/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/tests/test_decorators.py` & `hdn-research-environment-1.5.3/environment/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/tests/test_services.py` & `hdn-research-environment-1.5.3/environment/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/tests/test_signals.py` & `hdn-research-environment-1.5.3/environment/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/tests/test_utilities.py` & `hdn-research-environment-1.5.3/environment/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/tests/test_validators.py` & `hdn-research-environment-1.5.3/environment/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/tests/test_views.py` & `hdn-research-environment-1.5.3/environment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/urls.py` & `hdn-research-environment-1.5.3/environment/urls.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/utilities.py` & `hdn-research-environment-1.5.3/environment/utilities.py`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/environment/views.py` & `hdn-research-environment-1.5.3/environment/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             except BillingVerificationFailed as err:
                 form.add_error("billing_account_id", err)
     else:
         form = BillingAccountIdForm()
 
     cloud_identity = request.user.cloud_identity
     session_otp = request.session.get("cloud_identity_otp")
-    one_time_password = session_otp or services.get_user_info(cloud_identity.gcp_user_id).get("one-time-password")
+    one_time_password = session_otp or services.get_user_info(request.user).get("one-time-password")
     context = {
         "email": cloud_identity.email,
         "otp": one_time_password,
         "form": form,
     }
     return render(request, "environment/billing_setup.html", context)
```

### Comparing `hdn-research-environment-1.5.2/hdn_research_environment.egg-info/PKG-INFO` & `hdn-research-environment-1.5.3/hdn_research_environment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: hdn-research-environment
-Version: 1.5.2
+Version: 1.5.3
 Summary: A Django app for supporting cloud-native research environments
 Home-page: https://www.healthdatanexus.ai/
 Author: Your Name
 Author-email: yourname@example.com
 License: BSD-3-Clause  # Example license
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `hdn-research-environment-1.5.2/hdn_research_environment.egg-info/SOURCES.txt` & `hdn-research-environment-1.5.3/hdn_research_environment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdn-research-environment-1.5.2/setup.cfg` & `hdn-research-environment-1.5.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hdn-research-environment
-version = 1.5.2
+version = 1.5.3
 description = A Django app for supporting cloud-native research environments
 long_description = file: README.rst
 url = https://www.healthdatanexus.ai/
 author = Your Name
 author_email = yourname@example.com
 license = BSD-3-Clause  # Example license
 classifiers =
```

