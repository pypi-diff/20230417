# Comparing `tmp/alertify-0.7.0.tar.gz` & `tmp/alertify-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alertify-0.7.0.tar", last modified: Mon Feb 20 17:15:44 2023, max compression
+gzip compressed data, was "alertify-0.8.0.tar", last modified: Sun Apr 16 23:35:43 2023, max compression
```

## Comparing `alertify-0.7.0.tar` & `alertify-0.8.0.tar`

### file list

```diff
@@ -1,70 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.951399 alertify-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.931399 alertify-0.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-20 17:15:19.000000 alertify-0.7.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-20 17:15:19.000000 alertify-0.7.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.935399 alertify-0.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-20 17:15:19.000000 alertify-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-02-20 17:15:19.000000 alertify-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-02-20 17:15:19.000000 alertify-0.7.0/.github/boring-cyborg.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.935399 alertify-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-02-20 17:15:19.000000 alertify-0.7.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-02-20 17:15:19.000000 alertify-0.7.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-02-20 17:15:19.000000 alertify-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-02-20 17:15:19.000000 alertify-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-20 17:15:19.000000 alertify-0.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-20 17:15:19.000000 alertify-0.7.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-02-20 17:15:19.000000 alertify-0.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-02-20 17:15:19.000000 alertify-0.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-20 17:15:19.000000 alertify-0.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-02-20 17:15:19.000000 alertify-0.7.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-02-20 17:15:44.951399 alertify-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-20 17:15:19.000000 alertify-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.935399 alertify-0.7.0/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-20 17:15:19.000000 alertify-0.7.0/cache/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.935399 alertify-0.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-20 17:15:19.000000 alertify-0.7.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-02-20 17:15:19.000000 alertify-0.7.0/examples/opsgenie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-02-20 17:15:19.000000 alertify-0.7.0/examples/pagerduty.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-20 17:15:19.000000 alertify-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-20 17:15:19.000000 alertify-0.7.0/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-02-20 17:15:44.951399 alertify-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-02-20 17:15:19.000000 alertify-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.935399 alertify-0.7.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 17:15:19.000000 alertify-0.7.0/src/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.935399 alertify-0.7.0/src/alertify/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-02-20 17:15:19.000000 alertify-0.7.0/src/alertify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.947399 alertify-0.7.0/src/alertify/exception/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-02-20 17:15:19.000000 alertify-0.7.0/src/alertify/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-02-20 17:15:19.000000 alertify-0.7.0/src/alertify/exception/api_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.947399 alertify-0.7.0/src/alertify/opsgenie/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-02-20 17:15:19.000000 alertify-0.7.0/src/alertify/opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-02-20 17:15:19.000000 alertify-0.7.0/src/alertify/opsgenie/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.947399 alertify-0.7.0/src/alertify/pagerduty/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-02-20 17:15:19.000000 alertify-0.7.0/src/alertify/pagerduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-02-20 17:15:19.000000 alertify-0.7.0/src/alertify/pagerduty/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.951399 alertify-0.7.0/src/alertify/sendgrid/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-02-20 17:15:19.000000 alertify-0.7.0/src/alertify/sendgrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-02-20 17:15:19.000000 alertify-0.7.0/src/alertify/sendgrid/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.951399 alertify-0.7.0/src/alertify/slack/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-02-20 17:15:19.000000 alertify-0.7.0/src/alertify/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-20 17:15:19.000000 alertify-0.7.0/src/alertify/slack/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.951399 alertify-0.7.0/src/alertify/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-20 17:15:19.000000 alertify-0.7.0/src/alertify/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-02-20 17:15:19.000000 alertify-0.7.0/src/alertify/util/file_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.951399 alertify-0.7.0/src/alertify/webhook/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-02-20 17:15:19.000000 alertify-0.7.0/src/alertify/webhook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-02-20 17:15:19.000000 alertify-0.7.0/src/alertify/webhook/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.935399 alertify-0.7.0/src/alertify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-02-20 17:15:44.000000 alertify-0.7.0/src/alertify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-02-20 17:15:44.000000 alertify-0.7.0/src/alertify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 17:15:44.000000 alertify-0.7.0/src/alertify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 17:15:44.000000 alertify-0.7.0/src/alertify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-20 17:15:44.000000 alertify-0.7.0/src/alertify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-20 17:15:44.000000 alertify-0.7.0/src/alertify.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.951399 alertify-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-20 17:15:19.000000 alertify-0.7.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:15:44.951399 alertify-0.7.0/tests/exception/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-02-20 17:15:19.000000 alertify-0.7.0/tests/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-02-20 17:15:19.000000 alertify-0.7.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-20 17:15:19.000000 alertify-0.7.0/todo.md
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-02-20 17:15:19.000000 alertify-0.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.755826 alertify-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.751826 alertify-0.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-16 23:35:21.000000 alertify-0.8.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 23:35:21.000000 alertify-0.8.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.751826 alertify-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-16 23:35:21.000000 alertify-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-16 23:35:21.000000 alertify-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-16 23:35:21.000000 alertify-0.8.0/.github/boring-cyborg.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.751826 alertify-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-16 23:35:21.000000 alertify-0.8.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-16 23:35:21.000000 alertify-0.8.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-16 23:35:21.000000 alertify-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-16 23:35:21.000000 alertify-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-16 23:35:21.000000 alertify-0.8.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-16 23:35:21.000000 alertify-0.8.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-16 23:35:21.000000 alertify-0.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-16 23:35:21.000000 alertify-0.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 23:35:21.000000 alertify-0.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-16 23:35:21.000000 alertify-0.8.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-16 23:35:43.755826 alertify-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-16 23:35:21.000000 alertify-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.751826 alertify-0.8.0/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-16 23:35:21.000000 alertify-0.8.0/cache/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.751826 alertify-0.8.0/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-04-16 23:35:21.000000 alertify-0.8.0/chart/chart.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (123)    51845 2023-04-16 23:35:21.000000 alertify-0.8.0/chart/chart.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.751826 alertify-0.8.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 23:35:21.000000 alertify-0.8.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-16 23:35:21.000000 alertify-0.8.0/examples/opsgenie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-16 23:35:21.000000 alertify-0.8.0/examples/pagerduty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-16 23:35:21.000000 alertify-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 23:35:21.000000 alertify-0.8.0/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-16 23:35:43.755826 alertify-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-16 23:35:21.000000 alertify-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.751826 alertify-0.8.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 23:35:21.000000 alertify-0.8.0/src/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.751826 alertify-0.8.0/src/alertify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-16 23:35:21.000000 alertify-0.8.0/src/alertify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.751826 alertify-0.8.0/src/alertify/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-16 23:35:21.000000 alertify-0.8.0/src/alertify/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-16 23:35:21.000000 alertify-0.8.0/src/alertify/exception/api_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.751826 alertify-0.8.0/src/alertify/opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-16 23:35:21.000000 alertify-0.8.0/src/alertify/opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-16 23:35:21.000000 alertify-0.8.0/src/alertify/opsgenie/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.751826 alertify-0.8.0/src/alertify/pagerduty/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-16 23:35:21.000000 alertify-0.8.0/src/alertify/pagerduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-16 23:35:21.000000 alertify-0.8.0/src/alertify/pagerduty/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.751826 alertify-0.8.0/src/alertify/sendgrid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-16 23:35:21.000000 alertify-0.8.0/src/alertify/sendgrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-16 23:35:21.000000 alertify-0.8.0/src/alertify/sendgrid/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.751826 alertify-0.8.0/src/alertify/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-16 23:35:21.000000 alertify-0.8.0/src/alertify/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-16 23:35:21.000000 alertify-0.8.0/src/alertify/slack/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.751826 alertify-0.8.0/src/alertify/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 23:35:21.000000 alertify-0.8.0/src/alertify/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-16 23:35:21.000000 alertify-0.8.0/src/alertify/util/file_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.755826 alertify-0.8.0/src/alertify/webhook/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-16 23:35:21.000000 alertify-0.8.0/src/alertify/webhook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-16 23:35:21.000000 alertify-0.8.0/src/alertify/webhook/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.751826 alertify-0.8.0/src/alertify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-16 23:35:43.000000 alertify-0.8.0/src/alertify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-16 23:35:43.000000 alertify-0.8.0/src/alertify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 23:35:43.000000 alertify-0.8.0/src/alertify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 23:35:43.000000 alertify-0.8.0/src/alertify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-16 23:35:43.000000 alertify-0.8.0/src/alertify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-16 23:35:43.000000 alertify-0.8.0/src/alertify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.755826 alertify-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 23:35:21.000000 alertify-0.8.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:35:43.755826 alertify-0.8.0/tests/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 23:35:21.000000 alertify-0.8.0/tests/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-16 23:35:21.000000 alertify-0.8.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-16 23:35:21.000000 alertify-0.8.0/todo.md
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-16 23:35:21.000000 alertify-0.8.0/tox.ini
```

### Comparing `alertify-0.7.0/.github/boring-cyborg.yml` & `alertify-0.8.0/.github/boring-cyborg.yml`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/.github/workflows/release.yml` & `alertify-0.8.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/.gitignore` & `alertify-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/CODE_OF_CONDUCT.md` & `alertify-0.8.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/CONTRIBUTING.rst` & `alertify-0.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/LICENSE.txt` & `alertify-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/Makefile` & `alertify-0.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/PKG-INFO` & `alertify-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertify
-Version: 0.7.0
+Version: 0.8.0
 Summary: Uptimedog Alerting Integrations.
 Home-page: https://github.com/uptimedog/alertify/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/uptimedog/alertify/
 Project-URL: Source, https://github.com/uptimedog/alertify/
@@ -23,14 +23,19 @@
     :target: https://pypi.org/project/Alertify/
 .. image:: https://github.com/Uptimedog/Alertify/actions/workflows/ci.yml/badge.svg
     :alt: Build Status
     :target: https://github.com/Uptimedog/Alertify/actions/workflows/ci.yml
 
 |
 
+.. image:: https://raw.githubusercontent.com/Uptimedog/Alertify/main/chart/chart.png
+   :width: 100%
+
+|
+
 ========
 Alertify
 ========
 
     Uptimedog Alerting Integrations
```

### Comparing `alertify-0.7.0/examples/__init__.py` & `alertify-0.8.0/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/examples/opsgenie.py` & `alertify-0.8.0/examples/opsgenie.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/examples/pagerduty.py` & `alertify-0.8.0/examples/pagerduty.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/setup.cfg` & `alertify-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/setup.py` & `alertify-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/src/alertify/__init__.py` & `alertify-0.8.0/src/alertify/__init__.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/src/alertify/exception/__init__.py` & `alertify-0.8.0/src/alertify/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/src/alertify/exception/api_error.py` & `alertify-0.8.0/src/alertify/exception/api_error.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/src/alertify/opsgenie/__init__.py` & `alertify-0.8.0/src/alertify/opsgenie/__init__.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/src/alertify/opsgenie/client.py` & `alertify-0.8.0/src/alertify/opsgenie/client.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/src/alertify/pagerduty/__init__.py` & `alertify-0.8.0/src/alertify/pagerduty/__init__.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/src/alertify/pagerduty/client.py` & `alertify-0.8.0/src/alertify/pagerduty/client.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/src/alertify/sendgrid/__init__.py` & `alertify-0.8.0/src/alertify/sendgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/src/alertify/sendgrid/client.py` & `alertify-0.8.0/src/alertify/sendgrid/client.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/src/alertify/slack/__init__.py` & `alertify-0.8.0/src/alertify/slack/__init__.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/src/alertify/slack/client.py` & `alertify-0.8.0/src/alertify/slack/client.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/src/alertify/util/__init__.py` & `alertify-0.8.0/src/alertify/util/__init__.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/src/alertify/util/file_system.py` & `alertify-0.8.0/src/alertify/util/file_system.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/src/alertify/webhook/__init__.py` & `alertify-0.8.0/src/alertify/webhook/__init__.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/src/alertify/webhook/client.py` & `alertify-0.8.0/src/alertify/webhook/client.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/src/alertify.egg-info/PKG-INFO` & `alertify-0.8.0/src/alertify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alertify
-Version: 0.7.0
+Version: 0.8.0
 Summary: Uptimedog Alerting Integrations.
 Home-page: https://github.com/uptimedog/alertify/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/uptimedog/alertify/
 Project-URL: Source, https://github.com/uptimedog/alertify/
@@ -23,14 +23,19 @@
     :target: https://pypi.org/project/Alertify/
 .. image:: https://github.com/Uptimedog/Alertify/actions/workflows/ci.yml/badge.svg
     :alt: Build Status
     :target: https://github.com/Uptimedog/Alertify/actions/workflows/ci.yml
 
 |
 
+.. image:: https://raw.githubusercontent.com/Uptimedog/Alertify/main/chart/chart.png
+   :width: 100%
+
+|
+
 ========
 Alertify
 ========
 
     Uptimedog Alerting Integrations
```

### Comparing `alertify-0.7.0/src/alertify.egg-info/SOURCES.txt` & `alertify-0.8.0/src/alertify.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 .github/FUNDING.yml
 .github/boring-cyborg.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/ci.yml
 .github/workflows/release.yml
 cache/.gitignore
+chart/chart.excalidraw
+chart/chart.png
 examples/__init__.py
 examples/opsgenie.py
 examples/pagerduty.py
 src/.gitkeep
 src/alertify/__init__.py
 src/alertify.egg-info/PKG-INFO
 src/alertify.egg-info/SOURCES.txt
```

### Comparing `alertify-0.7.0/tests/__init__.py` & `alertify-0.8.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/tests/exception/__init__.py` & `alertify-0.8.0/tests/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/tests/test_client.py` & `alertify-0.8.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `alertify-0.7.0/tox.ini` & `alertify-0.8.0/tox.ini`

 * *Files identical despite different names*

