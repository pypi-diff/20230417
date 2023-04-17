# Comparing `tmp/fiduswriter-gitrepo-export-3.11.2.tar.gz` & `tmp/fiduswriter-gitrepo-export-3.11.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/johannes/src/fiduswriter/fiduswriter-gitrepo-export/dist/.tmp-2ikjz9wm/fiduswriter-gitrepo-export-3.11.2.tar", last modified: Wed Mar  1 06:59:14 2023, max compression
+gzip compressed data, was "/home/johannes/src/fiduswriter/fiduswriter-gitrepo-export/dist/.tmp-3hn5anu3/fiduswriter-gitrepo-export-3.11.3.tar", last modified: Mon Apr 17 10:47:49 2023, max compression
```

## Comparing `fiduswriter-gitrepo-export-3.11.2.tar` & `fiduswriter-gitrepo-export-3.11.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.947363 fiduswriter-gitrepo-export-3.11.2/
--rw-r--r--   0 johannes  (1000) johannes  (1000)    34523 2020-04-02 14:48:36.000000 fiduswriter-gitrepo-export-3.11.2/LICENSE
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      338 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/MANIFEST.in
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2726 2023-03-01 06:59:14.947363 fiduswriter-gitrepo-export-3.11.2/PKG-INFO
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1857 2023-03-01 06:56:29.000000 fiduswriter-gitrepo-export-3.11.2/README.md
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.935363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.939363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/__init__.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      280 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/admin.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      143 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/apps.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.939363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/helpers/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/helpers/__init__.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2509 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/helpers/github.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2704 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/helpers/gitlab.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.935363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.935363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/bg/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.939363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2206 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3539 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.935363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/de/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.939363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1800 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3133 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.935363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/es/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.939363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1763 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3123 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.935363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/fr/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.943363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1784 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3117 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.935363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/it/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.943363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1711 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3044 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.935363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/pt_BR/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.943363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1755 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3088 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.943363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/migrations/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2586 2023-02-26 06:56:30.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/migrations/0001_initial.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/migrations/__init__.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1057 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/models.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.935363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.935363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.935363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.943363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    11633 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/books_overview.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.943363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2482 2023-02-25 17:01:11.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/book_exporters.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5779 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/book_processor.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       53 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.947363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3076 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_file.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2149 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_tree.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3058 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_zip_contents.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      183 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      372 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/promise_chain.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.947363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2234 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/book_exporters.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5342 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/book_processor.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       53 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.947363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3303 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/commit.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       76 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1521 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/zip2blobs.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       62 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3024 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/templates.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1403 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/tools.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.935363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/plugins/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.947363 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/plugins/books_overview/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       74 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/plugins/books_overview/gitrepo_export.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      795 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/urls.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6267 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/views.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-03-01 06:59:14.947363 fiduswriter-gitrepo-export-3.11.2/fiduswriter_gitrepo_export.egg-info/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2726 2023-03-01 06:59:14.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter_gitrepo_export.egg-info/PKG-INFO
--rw-r--r--   0 johannes  (1000) johannes  (1000)     3004 2023-03-01 06:59:14.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter_gitrepo_export.egg-info/SOURCES.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)        1 2023-03-01 06:59:14.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter_gitrepo_export.egg-info/dependency_links.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)       20 2023-03-01 06:59:14.000000 fiduswriter-gitrepo-export-3.11.2/fiduswriter_gitrepo_export.egg-info/top_level.txt
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      914 2023-03-01 06:58:57.000000 fiduswriter-gitrepo-export-3.11.2/pyproject.toml
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       38 2023-03-01 06:59:14.947363 fiduswriter-gitrepo-export-3.11.2/setup.cfg
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1083 2023-03-01 06:58:00.000000 fiduswriter-gitrepo-export-3.11.2/setup.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.889304 fiduswriter-gitrepo-export-3.11.3/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    34523 2020-04-02 14:48:36.000000 fiduswriter-gitrepo-export-3.11.3/LICENSE
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      338 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/MANIFEST.in
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2726 2023-04-17 10:47:49.885304 fiduswriter-gitrepo-export-3.11.3/PKG-INFO
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1857 2023-03-01 06:56:29.000000 fiduswriter-gitrepo-export-3.11.3/README.md
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.869304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.877304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/__init__.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      280 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/admin.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      143 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/apps.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.877304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/helpers/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/helpers/__init__.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2509 2023-04-13 22:20:28.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/helpers/github.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2704 2023-04-13 22:39:13.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/helpers/gitlab.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/bg/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.877304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2206 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3539 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/de/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.881304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1800 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3133 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/es/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.881304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1763 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3123 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/fr/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.881304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1784 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3117 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/it/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.881304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1711 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3044 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/pt_BR/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.881304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1755 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3088 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.881304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/migrations/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2586 2023-02-26 06:56:30.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/migrations/0001_initial.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/migrations/__init__.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1057 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/models.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.885304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    11633 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/books_overview.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.885304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2482 2023-02-25 17:01:11.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/book_exporters.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5779 2023-04-13 22:39:18.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/book_processor.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       53 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.885304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3325 2023-04-13 22:39:54.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_file.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2149 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_tree.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3058 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_zip_contents.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      183 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      372 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/promise_chain.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.885304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2234 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/book_exporters.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5342 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/book_processor.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       53 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.885304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3303 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/commit.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       76 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1521 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/zip2blobs.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       62 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3024 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/templates.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1403 2022-10-26 17:58:37.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/tools.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.873304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/plugins/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.885304 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/plugins/books_overview/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       74 2022-05-13 19:55:44.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/plugins/books_overview/gitrepo_export.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      795 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/urls.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6267 2023-02-26 06:58:11.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/views.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2023-04-17 10:47:49.885304 fiduswriter-gitrepo-export-3.11.3/fiduswriter_gitrepo_export.egg-info/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2726 2023-04-17 10:47:49.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter_gitrepo_export.egg-info/PKG-INFO
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     3004 2023-04-17 10:47:49.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter_gitrepo_export.egg-info/SOURCES.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        1 2023-04-17 10:47:49.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter_gitrepo_export.egg-info/dependency_links.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       20 2023-04-17 10:47:49.000000 fiduswriter-gitrepo-export-3.11.3/fiduswriter_gitrepo_export.egg-info/top_level.txt
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      914 2023-04-17 10:47:34.000000 fiduswriter-gitrepo-export-3.11.3/pyproject.toml
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       38 2023-04-17 10:47:49.889304 fiduswriter-gitrepo-export-3.11.3/setup.cfg
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1083 2023-03-01 06:58:00.000000 fiduswriter-gitrepo-export-3.11.3/setup.py
```

### Comparing `fiduswriter-gitrepo-export-3.11.2/LICENSE` & `fiduswriter-gitrepo-export-3.11.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/PKG-INFO` & `fiduswriter-gitrepo-export-3.11.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiduswriter-gitrepo-export
-Version: 3.11.2
+Version: 3.11.3
 Summary: A Fidus Writer plugin to allow publishing of books to a Gitlab/Github repository.
 Author-email: Johannes Wilm <johannes@fiduswriter.org>
 License: AGPL-3.0-or-later
 Project-URL: repository, https://www.github.org/fiduswriter/fiduswriter-gitrepo-export
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
```

### Comparing `fiduswriter-gitrepo-export-3.11.2/README.md` & `fiduswriter-gitrepo-export-3.11.3/README.md`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/helpers/github.py` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/helpers/github.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/helpers/gitlab.py` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/helpers/gitlab.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/djangojs.mo` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/djangojs.po` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/bg/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/djangojs.mo` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/djangojs.po` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/djangojs.mo` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/djangojs.po` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/djangojs.mo` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/djangojs.po` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/djangojs.mo` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/djangojs.po` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/it/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/djangojs.po` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/migrations/0001_initial.py` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/models.py` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/models.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/books_overview.js` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/books_overview.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/book_exporters.js` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/book_exporters.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/book_processor.js` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/book_processor.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_file.js` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_file.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -12,14 +12,21 @@
     const getDirJsonPromise = repoDirCache[dirUrl] ?
         Promise.resolve(repoDirCache[dirUrl]) :
         getJson(dirUrl).then(
             json => {
                 repoDirCache[dirUrl] = json
                 return Promise.resolve(json)
             }
+        ).catch(
+            error => {
+                if (error.status === 302) { // Redirect - which means the directory does not exist.
+                    return Promise.resolve(false)
+                }
+                throw error
+            }
         )
     const csrfToken = getCookie("csrftoken")
     return Promise.resolve(getDirJsonPromise).then(json => {
         const fileEntry = Array.isArray(json) ? json.find(entry => entry.name === filename) : false
         const commitData = {
             encoding: "base64",
         }
```

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_tree.js` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_tree.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_zip_contents.js` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/github/tools/commit_zip_contents.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/book_exporters.js` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/book_exporters.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/book_processor.js` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/book_processor.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/commit.js` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/commit.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/zip2blobs.js` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/gitlab/tools/zip2blobs.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/templates.js` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/tools.js` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/static/js/modules/gitrepo_export/tools.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/urls.py` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/urls.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter/gitrepo_export/views.py` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter/gitrepo_export/views.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter_gitrepo_export.egg-info/PKG-INFO` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter_gitrepo_export.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiduswriter-gitrepo-export
-Version: 3.11.2
+Version: 3.11.3
 Summary: A Fidus Writer plugin to allow publishing of books to a Gitlab/Github repository.
 Author-email: Johannes Wilm <johannes@fiduswriter.org>
 License: AGPL-3.0-or-later
 Project-URL: repository, https://www.github.org/fiduswriter/fiduswriter-gitrepo-export
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
```

### Comparing `fiduswriter-gitrepo-export-3.11.2/fiduswriter_gitrepo_export.egg-info/SOURCES.txt` & `fiduswriter-gitrepo-export-3.11.3/fiduswriter_gitrepo_export.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiduswriter-gitrepo-export-3.11.2/pyproject.toml` & `fiduswriter-gitrepo-export-3.11.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=65.6.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fiduswriter-gitrepo-export"
 description = "A Fidus Writer plugin to allow publishing of books to a Gitlab/Github repository."
-version = "3.11.2"
+version = "3.11.3"
 readme = "README.md"
 license = {text = "AGPL-3.0-or-later"}
 authors = [
   {email = "johannes@fiduswriter.org", name = "Johannes Wilm"},
 ]
 classifiers=[
   "Environment :: Web Environment",
```

### Comparing `fiduswriter-gitrepo-export-3.11.2/setup.py` & `fiduswriter-gitrepo-export-3.11.3/setup.py`

 * *Files identical despite different names*

