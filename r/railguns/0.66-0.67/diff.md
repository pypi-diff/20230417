# Comparing `tmp/railguns-0.66.tar.gz` & `tmp/railguns-0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "railguns-0.66.tar", last modified: Sat Feb 25 15:15:24 2023, max compression
+gzip compressed data, was "railguns-0.67.tar", last modified: Mon Apr 17 06:54:42 2023, max compression
```

## Comparing `railguns-0.66.tar` & `railguns-0.67.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.342535 railguns-0.66/
--rw-r--r--   0 ny         (501) staff       (20)     1089 2022-06-18 13:16:59.000000 railguns-0.66/LICENSE
--rw-r--r--   0 ny         (501) staff       (20)      109 2022-06-18 13:16:59.000000 railguns-0.66/MANIFEST.in
--rw-r--r--   0 ny         (501) staff       (20)     3954 2023-02-25 15:15:24.342415 railguns-0.66/PKG-INFO
--rw-r--r--   0 ny         (501) staff       (20)     1648 2022-06-18 13:16:59.000000 railguns-0.66/README.md
--rw-r--r--   0 ny         (501) staff       (20)     1687 2023-02-25 15:14:15.000000 railguns-0.66/pyproject.toml
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.337248 railguns-0.66/railguns/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.66/railguns/__init__.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.338258 railguns-0.66/railguns/cloudfile/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.66/railguns/cloudfile/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)      470 2022-06-18 13:16:59.000000 railguns-0.66/railguns/cloudfile/fields.py
--rw-r--r--   0 ny         (501) staff       (20)     1137 2022-06-18 13:16:59.000000 railguns-0.66/railguns/cloudfile/widgets.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.338443 railguns-0.66/railguns/django/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.66/railguns/django/__init__.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.338629 railguns-0.66/railguns/django/contrib/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.66/railguns/django/contrib/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)     2321 2022-06-18 13:16:59.000000 railguns-0.66/railguns/django/contrib/admin.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.338818 railguns-0.66/railguns/django/contrib/auth/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.66/railguns/django/contrib/auth/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)      855 2022-06-18 13:16:59.000000 railguns-0.66/railguns/django/contrib/auth/backends.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.339130 railguns-0.66/railguns/django/db/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.66/railguns/django/db/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)     3140 2022-06-18 13:16:59.000000 railguns-0.66/railguns/django/db/models.py
--rw-r--r--   0 ny         (501) staff       (20)     2190 2022-06-18 13:16:59.000000 railguns-0.66/railguns/django/db/utils.py
--rw-r--r--   0 ny         (501) staff       (20)     1776 2022-06-18 13:16:59.000000 railguns-0.66/railguns/django/generics.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.339424 railguns-0.66/railguns/django/utils/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.66/railguns/django/utils/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)      459 2022-06-18 13:16:59.000000 railguns-0.66/railguns/django/utils/html.py
--rw-r--r--   0 ny         (501) staff       (20)      777 2022-06-18 13:16:59.000000 railguns-0.66/railguns/django/utils/translation.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.340275 railguns-0.66/railguns/rest_framework/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.66/railguns/rest_framework/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)     1614 2022-06-18 13:16:59.000000 railguns-0.66/railguns/rest_framework/generics.py
--rw-r--r--   0 ny         (501) staff       (20)     2762 2022-06-18 13:16:59.000000 railguns-0.66/railguns/rest_framework/mixins.py
--rw-r--r--   0 ny         (501) staff       (20)      306 2022-06-18 13:16:59.000000 railguns-0.66/railguns/rest_framework/pagination.py
--rw-r--r--   0 ny         (501) staff       (20)     1750 2022-06-18 13:16:59.000000 railguns-0.66/railguns/rest_framework/permissions.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.340490 railguns-0.66/railguns/rest_framework/schemas/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.66/railguns/rest_framework/schemas/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)      948 2022-06-18 13:16:59.000000 railguns-0.66/railguns/rest_framework/schemas/openapi.py
--rw-r--r--   0 ny         (501) staff       (20)      746 2022-06-18 13:16:59.000000 railguns-0.66/railguns/rest_framework/serializers.py
--rw-r--r--   0 ny         (501) staff       (20)      128 2022-06-18 13:16:59.000000 railguns-0.66/railguns/rest_framework/utils.py
--rw-r--r--   0 ny         (501) staff       (20)     6642 2022-06-18 13:16:59.000000 railguns-0.66/railguns/rest_framework/views.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.335830 railguns-0.66/railguns/static/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.335772 railguns-0.66/railguns/static/cloudfile/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.340596 railguns-0.66/railguns/static/cloudfile/js/
--rw-r--r--   0 ny         (501) staff       (20)     5251 2022-06-18 13:16:59.000000 railguns-0.66/railguns/static/cloudfile/js/scripts.js
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.336039 railguns-0.66/railguns/static/railguns/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.340828 railguns-0.66/railguns/static/railguns/es2015/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.340937 railguns-0.66/railguns/static/railguns/es2015/components/
--rw-r--r--   0 ny         (501) staff       (20)    16351 2022-06-18 13:16:59.000000 railguns-0.66/railguns/static/railguns/es2015/components/weui-components.js
--rw-r--r--   0 ny         (501) staff       (20)     1691 2022-06-18 13:16:59.000000 railguns-0.66/railguns/static/railguns/es2015/mixins.js
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.341048 railguns-0.66/railguns/static/railguns/es2015/util/
--rw-r--r--   0 ny         (501) staff       (20)     2000 2022-06-18 13:16:59.000000 railguns-0.66/railguns/static/railguns/es2015/util/http-utils.js
--rw-r--r--   0 ny         (501) staff       (20)      555 2022-06-18 13:16:59.000000 railguns-0.66/railguns/static/railguns/es2015/vendor.js
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.341282 railguns-0.66/railguns/static/railguns/js/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.341400 railguns-0.66/railguns/static/railguns/js/components/
--rw-r--r--   0 ny         (501) staff       (20)    13372 2022-06-18 13:16:59.000000 railguns-0.66/railguns/static/railguns/js/components/weui-components.js
--rw-r--r--   0 ny         (501) staff       (20)     1160 2022-06-18 13:16:59.000000 railguns-0.66/railguns/static/railguns/js/mixins.js
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.341510 railguns-0.66/railguns/static/railguns/js/util/
--rw-r--r--   0 ny         (501) staff       (20)      948 2022-06-18 13:16:59.000000 railguns-0.66/railguns/static/railguns/js/util/http-utils.js
--rw-r--r--   0 ny         (501) staff       (20)      346 2022-06-18 13:16:59.000000 railguns-0.66/railguns/static/railguns/js/vendor.js
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.336249 railguns-0.66/railguns/templates/
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.341722 railguns-0.66/railguns/templates/railguns/
--rw-r--r--   0 ny         (501) staff       (20)      583 2022-06-18 13:16:59.000000 railguns-0.66/railguns/templates/railguns/base.html
--rw-r--r--   0 ny         (501) staff       (20)     1738 2022-06-18 13:16:59.000000 railguns-0.66/railguns/templates/railguns/base_quick.html
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.342069 railguns-0.66/railguns/templates/railguns/ui/
--rw-r--r--   0 ny         (501) staff       (20)     1325 2022-06-18 13:16:59.000000 railguns-0.66/railguns/templates/railguns/ui/base.html
--rw-r--r--   0 ny         (501) staff       (20)      740 2022-06-18 13:16:59.000000 railguns-0.66/railguns/templates/railguns/ui/detail.html
--rw-r--r--   0 ny         (501) staff       (20)      775 2022-06-18 13:16:59.000000 railguns-0.66/railguns/templates/railguns/ui/list.html
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.342259 railguns-0.66/railguns/tools/
--rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.66/railguns/tools/__init__.py
--rw-r--r--   0 ny         (501) staff       (20)      238 2022-06-18 13:16:59.000000 railguns-0.66/railguns/tools/utils.py
--rw-r--r--   0 ny         (501) staff       (20)     1653 2022-06-18 13:16:59.000000 railguns-0.66/railguns/urls.py
-drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-02-25 15:15:24.337924 railguns-0.66/railguns.egg-info/
--rw-r--r--   0 ny         (501) staff       (20)     3954 2023-02-25 15:15:24.000000 railguns-0.66/railguns.egg-info/PKG-INFO
--rw-r--r--   0 ny         (501) staff       (20)     1787 2023-02-25 15:15:24.000000 railguns-0.66/railguns.egg-info/SOURCES.txt
--rw-r--r--   0 ny         (501) staff       (20)        1 2023-02-25 15:15:24.000000 railguns-0.66/railguns.egg-info/dependency_links.txt
--rw-r--r--   0 ny         (501) staff       (20)      285 2023-02-25 15:15:24.000000 railguns-0.66/railguns.egg-info/requires.txt
--rw-r--r--   0 ny         (501) staff       (20)        9 2023-02-25 15:15:24.000000 railguns-0.66/railguns.egg-info/top_level.txt
--rw-r--r--   0 ny         (501) staff       (20)       38 2023-02-25 15:15:24.342565 railguns-0.66/setup.cfg
--rw-r--r--   0 ny         (501) staff       (20)     1560 2023-02-25 15:12:56.000000 railguns-0.66/setup.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.966435 railguns-0.67/
+-rw-r--r--   0 ny         (501) staff       (20)     1089 2022-06-18 13:16:59.000000 railguns-0.67/LICENSE
+-rw-r--r--   0 ny         (501) staff       (20)      109 2022-06-18 13:16:59.000000 railguns-0.67/MANIFEST.in
+-rw-r--r--   0 ny         (501) staff       (20)     3954 2023-04-17 06:54:42.966301 railguns-0.67/PKG-INFO
+-rw-r--r--   0 ny         (501) staff       (20)     1648 2022-06-18 13:16:59.000000 railguns-0.67/README.md
+-rw-r--r--   0 ny         (501) staff       (20)     1685 2023-04-17 06:53:46.000000 railguns-0.67/pyproject.toml
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.958569 railguns-0.67/railguns/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.67/railguns/__init__.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.960188 railguns-0.67/railguns/cloudfile/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.67/railguns/cloudfile/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)      470 2022-06-18 13:16:59.000000 railguns-0.67/railguns/cloudfile/fields.py
+-rw-r--r--   0 ny         (501) staff       (20)     1137 2022-06-18 13:16:59.000000 railguns-0.67/railguns/cloudfile/widgets.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.960788 railguns-0.67/railguns/django/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.67/railguns/django/__init__.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.961091 railguns-0.67/railguns/django/contrib/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.67/railguns/django/contrib/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)     2321 2022-06-18 13:16:59.000000 railguns-0.67/railguns/django/contrib/admin.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.961425 railguns-0.67/railguns/django/contrib/auth/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.67/railguns/django/contrib/auth/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)      855 2022-06-18 13:16:59.000000 railguns-0.67/railguns/django/contrib/auth/backends.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.961804 railguns-0.67/railguns/django/db/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.67/railguns/django/db/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)     3140 2022-06-18 13:16:59.000000 railguns-0.67/railguns/django/db/models.py
+-rw-r--r--   0 ny         (501) staff       (20)     2190 2022-06-18 13:16:59.000000 railguns-0.67/railguns/django/db/utils.py
+-rw-r--r--   0 ny         (501) staff       (20)     1776 2022-06-18 13:16:59.000000 railguns-0.67/railguns/django/generics.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.962185 railguns-0.67/railguns/django/utils/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.67/railguns/django/utils/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)      459 2022-06-18 13:16:59.000000 railguns-0.67/railguns/django/utils/html.py
+-rw-r--r--   0 ny         (501) staff       (20)      777 2022-06-18 13:16:59.000000 railguns-0.67/railguns/django/utils/translation.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.963577 railguns-0.67/railguns/rest_framework/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.67/railguns/rest_framework/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)     1614 2022-06-18 13:16:59.000000 railguns-0.67/railguns/rest_framework/generics.py
+-rw-r--r--   0 ny         (501) staff       (20)     2762 2022-06-18 13:16:59.000000 railguns-0.67/railguns/rest_framework/mixins.py
+-rw-r--r--   0 ny         (501) staff       (20)      306 2022-06-18 13:16:59.000000 railguns-0.67/railguns/rest_framework/pagination.py
+-rw-r--r--   0 ny         (501) staff       (20)     1750 2022-06-18 13:16:59.000000 railguns-0.67/railguns/rest_framework/permissions.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.963837 railguns-0.67/railguns/rest_framework/schemas/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.67/railguns/rest_framework/schemas/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)      948 2022-06-18 13:16:59.000000 railguns-0.67/railguns/rest_framework/schemas/openapi.py
+-rw-r--r--   0 ny         (501) staff       (20)      746 2022-06-18 13:16:59.000000 railguns-0.67/railguns/rest_framework/serializers.py
+-rw-r--r--   0 ny         (501) staff       (20)      128 2022-06-18 13:16:59.000000 railguns-0.67/railguns/rest_framework/utils.py
+-rw-r--r--   0 ny         (501) staff       (20)     6642 2022-06-18 13:16:59.000000 railguns-0.67/railguns/rest_framework/views.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.957239 railguns-0.67/railguns/static/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.957182 railguns-0.67/railguns/static/cloudfile/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.963990 railguns-0.67/railguns/static/cloudfile/js/
+-rw-r--r--   0 ny         (501) staff       (20)     5251 2022-06-18 13:16:59.000000 railguns-0.67/railguns/static/cloudfile/js/scripts.js
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.957439 railguns-0.67/railguns/static/railguns/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.964271 railguns-0.67/railguns/static/railguns/es2015/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.964425 railguns-0.67/railguns/static/railguns/es2015/components/
+-rw-r--r--   0 ny         (501) staff       (20)    16351 2022-06-18 13:16:59.000000 railguns-0.67/railguns/static/railguns/es2015/components/weui-components.js
+-rw-r--r--   0 ny         (501) staff       (20)     1691 2022-06-18 13:16:59.000000 railguns-0.67/railguns/static/railguns/es2015/mixins.js
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.964573 railguns-0.67/railguns/static/railguns/es2015/util/
+-rw-r--r--   0 ny         (501) staff       (20)     2000 2022-06-18 13:16:59.000000 railguns-0.67/railguns/static/railguns/es2015/util/http-utils.js
+-rw-r--r--   0 ny         (501) staff       (20)      555 2022-06-18 13:16:59.000000 railguns-0.67/railguns/static/railguns/es2015/vendor.js
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.964862 railguns-0.67/railguns/static/railguns/js/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.965013 railguns-0.67/railguns/static/railguns/js/components/
+-rw-r--r--   0 ny         (501) staff       (20)    13372 2022-06-18 13:16:59.000000 railguns-0.67/railguns/static/railguns/js/components/weui-components.js
+-rw-r--r--   0 ny         (501) staff       (20)     1160 2022-06-18 13:16:59.000000 railguns-0.67/railguns/static/railguns/js/mixins.js
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.965169 railguns-0.67/railguns/static/railguns/js/util/
+-rw-r--r--   0 ny         (501) staff       (20)      948 2022-06-18 13:16:59.000000 railguns-0.67/railguns/static/railguns/js/util/http-utils.js
+-rw-r--r--   0 ny         (501) staff       (20)      346 2022-06-18 13:16:59.000000 railguns-0.67/railguns/static/railguns/js/vendor.js
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.957646 railguns-0.67/railguns/templates/
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.965458 railguns-0.67/railguns/templates/railguns/
+-rw-r--r--   0 ny         (501) staff       (20)      583 2022-06-18 13:16:59.000000 railguns-0.67/railguns/templates/railguns/base.html
+-rw-r--r--   0 ny         (501) staff       (20)     1738 2022-06-18 13:16:59.000000 railguns-0.67/railguns/templates/railguns/base_quick.html
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.965865 railguns-0.67/railguns/templates/railguns/ui/
+-rw-r--r--   0 ny         (501) staff       (20)     1325 2022-06-18 13:16:59.000000 railguns-0.67/railguns/templates/railguns/ui/base.html
+-rw-r--r--   0 ny         (501) staff       (20)      740 2022-06-18 13:16:59.000000 railguns-0.67/railguns/templates/railguns/ui/detail.html
+-rw-r--r--   0 ny         (501) staff       (20)      775 2022-06-18 13:16:59.000000 railguns-0.67/railguns/templates/railguns/ui/list.html
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.966096 railguns-0.67/railguns/tools/
+-rw-r--r--   0 ny         (501) staff       (20)        0 2022-06-18 13:16:59.000000 railguns-0.67/railguns/tools/__init__.py
+-rw-r--r--   0 ny         (501) staff       (20)      238 2022-06-18 13:16:59.000000 railguns-0.67/railguns/tools/utils.py
+-rw-r--r--   0 ny         (501) staff       (20)     1653 2022-06-18 13:16:59.000000 railguns-0.67/railguns/urls.py
+drwxr-xr-x   0 ny         (501) staff       (20)        0 2023-04-17 06:54:42.959737 railguns-0.67/railguns.egg-info/
+-rw-r--r--   0 ny         (501) staff       (20)     3954 2023-04-17 06:54:42.000000 railguns-0.67/railguns.egg-info/PKG-INFO
+-rw-r--r--   0 ny         (501) staff       (20)     1787 2023-04-17 06:54:42.000000 railguns-0.67/railguns.egg-info/SOURCES.txt
+-rw-r--r--   0 ny         (501) staff       (20)        1 2023-04-17 06:54:42.000000 railguns-0.67/railguns.egg-info/dependency_links.txt
+-rw-r--r--   0 ny         (501) staff       (20)      283 2023-04-17 06:54:42.000000 railguns-0.67/railguns.egg-info/requires.txt
+-rw-r--r--   0 ny         (501) staff       (20)        9 2023-04-17 06:54:42.000000 railguns-0.67/railguns.egg-info/top_level.txt
+-rw-r--r--   0 ny         (501) staff       (20)       38 2023-04-17 06:54:42.966469 railguns-0.67/setup.cfg
+-rw-r--r--   0 ny         (501) staff       (20)     1558 2023-04-17 06:51:57.000000 railguns-0.67/setup.py
```

### Comparing `railguns-0.66/LICENSE` & `railguns-0.67/LICENSE`

 * *Files identical despite different names*

### Comparing `railguns-0.66/PKG-INFO` & `railguns-0.67/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: railguns
-Version: 0.66
+Version: 0.67
 Summary: Only My Railgun
 Home-page: https://github.com/nyssance/railguns
 Author: NY
 Author-email: nyssance@icloud.com
 License: MIT License
         
         Copyright (c) 2018-present NY <nyssance@icloud.com>
```

### Comparing `railguns-0.66/README.md` & `railguns-0.67/README.md`

 * *Files identical despite different names*

### Comparing `railguns-0.66/pyproject.toml` & `railguns-0.67/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "railguns"
-version = "0.66"
+version = "0.67"
 description = "Only My Railgun"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["django", "railguns"]
 authors = [
   {email = "nyssance@icloud.com"},
@@ -25,26 +25,26 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Internet :: WWW/HTTP"
 ]
 dependencies = [
-  "django[argon2]==4.2b1",
+  "django[argon2]==4.2",
   "djangorestframework==3.14.0",
   "djangorestframework_simplejwt==5.2.2",
   "gunicorn==20.1.0",
-  "uvicorn==0.20.0",
+  "uvicorn==0.21.1",
   #
   "django-ckeditor==6.5.1",
-  "django-filter==22.1",
+  "django-filter==23.1",
   "django-htmlmin==0.11.0",
   "hiredis==2.2.1",
   "mysqlclient==2.1.1",
-  "redis==4.5.1"
+  "redis==4.5.4"
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest < 5.0.0",
   "pytest-cov[all]"
 ]
```

### Comparing `railguns-0.66/railguns/cloudfile/widgets.py` & `railguns-0.67/railguns/cloudfile/widgets.py`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/django/contrib/admin.py` & `railguns-0.67/railguns/django/contrib/admin.py`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/django/contrib/auth/backends.py` & `railguns-0.67/railguns/django/contrib/auth/backends.py`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/django/db/models.py` & `railguns-0.67/railguns/django/db/models.py`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/django/db/utils.py` & `railguns-0.67/railguns/django/db/utils.py`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/django/generics.py` & `railguns-0.67/railguns/django/generics.py`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/django/utils/translation.py` & `railguns-0.67/railguns/django/utils/translation.py`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/rest_framework/generics.py` & `railguns-0.67/railguns/rest_framework/generics.py`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/rest_framework/mixins.py` & `railguns-0.67/railguns/rest_framework/mixins.py`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/rest_framework/permissions.py` & `railguns-0.67/railguns/rest_framework/permissions.py`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/rest_framework/schemas/openapi.py` & `railguns-0.67/railguns/rest_framework/schemas/openapi.py`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/rest_framework/serializers.py` & `railguns-0.67/railguns/rest_framework/serializers.py`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/rest_framework/views.py` & `railguns-0.67/railguns/rest_framework/views.py`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/static/cloudfile/js/scripts.js` & `railguns-0.67/railguns/static/cloudfile/js/scripts.js`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/static/railguns/es2015/components/weui-components.js` & `railguns-0.67/railguns/static/railguns/es2015/components/weui-components.js`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/static/railguns/es2015/mixins.js` & `railguns-0.67/railguns/static/railguns/es2015/mixins.js`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/static/railguns/es2015/util/http-utils.js` & `railguns-0.67/railguns/static/railguns/es2015/util/http-utils.js`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/static/railguns/es2015/vendor.js` & `railguns-0.67/railguns/static/railguns/es2015/vendor.js`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/static/railguns/js/components/weui-components.js` & `railguns-0.67/railguns/static/railguns/js/components/weui-components.js`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/static/railguns/js/mixins.js` & `railguns-0.67/railguns/static/railguns/js/mixins.js`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/static/railguns/js/util/http-utils.js` & `railguns-0.67/railguns/static/railguns/js/util/http-utils.js`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/templates/railguns/base.html` & `railguns-0.67/railguns/templates/railguns/base.html`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/templates/railguns/base_quick.html` & `railguns-0.67/railguns/templates/railguns/base_quick.html`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/templates/railguns/ui/base.html` & `railguns-0.67/railguns/templates/railguns/ui/base.html`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/templates/railguns/ui/detail.html` & `railguns-0.67/railguns/templates/railguns/ui/detail.html`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/templates/railguns/ui/list.html` & `railguns-0.67/railguns/templates/railguns/ui/list.html`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns/urls.py` & `railguns-0.67/railguns/urls.py`

 * *Files identical despite different names*

### Comparing `railguns-0.66/railguns.egg-info/PKG-INFO` & `railguns-0.67/railguns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: railguns
-Version: 0.66
+Version: 0.67
 Summary: Only My Railgun
 Home-page: https://github.com/nyssance/railguns
 Author: NY
 Author-email: nyssance@icloud.com
 License: MIT License
         
         Copyright (c) 2018-present NY <nyssance@icloud.com>
```

### Comparing `railguns-0.66/railguns.egg-info/SOURCES.txt` & `railguns-0.67/railguns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `railguns-0.66/setup.py` & `railguns-0.67/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='RailgunS',
-    version='0.66',
+    version='0.67',
     author='NY',
     author_email='nyssance@icloud.com',
     description='Only My Railgun',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nyssance/railguns',
     project_urls={
@@ -30,25 +30,25 @@
     ],
     # package_dir={'': 'src'},
     packages=find_packages(exclude=['tests']),
     python_requires='>=3.10',
     # zip_safe=False,
     include_package_data=True,
     install_requires=[
-        'django[argon2]==4.2b1',
+        'django[argon2]==4.2',
         'djangorestframework==3.14.0',
         'djangorestframework_simplejwt==5.2.2',
         'gunicorn==20.1.0',
-        'uvicorn==0.20.0',
+        'uvicorn==0.21.1',
         #
         'django-ckeditor==6.5.1',
-        'django-filter==22.1',
+        'django-filter==23.1',
         'django-htmlmin==0.11.0',
         'hiredis==2.2.1',
         'mysqlclient==2.1.1',
-        'redis==4.5.1'
+        'redis==4.5.4'
     ],
     extras_require={
         'dev': [],
         'prod': []
     }
 )
```

