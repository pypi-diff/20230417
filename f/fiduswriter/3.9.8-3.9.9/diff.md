# Comparing `tmp/fiduswriter-3.9.8.tar.gz` & `tmp/fiduswriter-3.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fiduswriter-3.9.8.tar", last modified: Tue Jan  5 13:17:44 2021, max compression
+gzip compressed data, was "dist/fiduswriter-3.9.9.tar", last modified: Tue Jan  5 14:54:58 2021, max compression
```

## Comparing `fiduswriter-3.9.8.tar` & `fiduswriter-3.9.9.tar`

### file list

```diff
@@ -1,897 +1,897 @@
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.246680 fiduswriter-3.9.8/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      785 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/MANIFEST.in
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2759 2021-01-05 13:17:44.246680 fiduswriter-3.9.8/PKG-INFO
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)     1408 2019-11-03 23:58:06.000000 fiduswriter-3.9.8/README.md
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.158680 fiduswriter-3.9.8/fiduswriter/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      159 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/.babelrc
--rw-r--r--   0 johannes  (1000) johannes  (1000)       82 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/.eslintignore
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    10135 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/.eslintrc.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.158680 fiduswriter-3.9.8/fiduswriter/base/
--rwxrwxr-x   0 johannes  (1000) johannes  (1000)      683 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      326 2020-02-12 14:24:52.000000 fiduswriter-3.9.8/fiduswriter/base/apps.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      495 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/decorators.py
--rwxrwxr-x   0 johannes  (1000) johannes  (1000)    10773 2021-01-05 13:17:05.000000 fiduswriter-3.9.8/fiduswriter/base/default_settings.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      797 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/django_handler_mixin.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.158680 fiduswriter-3.9.8/fiduswriter/base/fixtures/
--rw-r--r--   0 johannes  (1000) johannes  (1000)    34753 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/fixtures/initial_terms.json
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.158680 fiduswriter-3.9.8/fiduswriter/base/handlers/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2824 2020-10-23 20:16:08.000000 fiduswriter-3.9.8/fiduswriter/base/handlers/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      191 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/html_email.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.158680 fiduswriter-3.9.8/fiduswriter/base/management/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      199 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/management/__init__.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.162680 fiduswriter-3.9.8/fiduswriter/base/management/commands/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/management/commands/__init__.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4027 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/management/commands/bundle_mathlive.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      357 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/management/commands/collectstatic.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      476 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/management/commands/compilemessages.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1381 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/management/commands/initadmin.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1082 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/management/commands/jest.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      302 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/management/commands/lint.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1292 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/management/commands/lint_css.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1697 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/management/commands/lint_js.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      581 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/management/commands/lint_py.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2878 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/management/commands/makemessages.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4420 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/management/commands/runserver.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2944 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/management/commands/setup.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1224 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/management/commands/startproject.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2931 2020-12-31 17:57:32.000000 fiduswriter-3.9.8/fiduswriter/base/package.json
--rwxrwxr-x   0 johannes  (1000) johannes  (1000)     2445 2021-01-05 13:17:05.000000 fiduswriter-3.9.8/fiduswriter/base/root_urls.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.162680 fiduswriter-3.9.8/fiduswriter/base/servers/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/servers/__init__.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1942 2020-10-28 16:28:23.000000 fiduswriter-3.9.8/fiduswriter/base/servers/tornado_django_hybrid.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.162680 fiduswriter-3.9.8/fiduswriter/base/setup_page/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      924 2020-01-13 20:06:18.000000 fiduswriter-3.9.8/fiduswriter/base/setup_page/index.html
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.142679 fiduswriter-3.9.8/fiduswriter/base/static/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.162680 fiduswriter-3.9.8/fiduswriter/base/static/css/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      402 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/add_remove_dialog.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)      433 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/admin.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1594 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/alerts.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7761 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/buttons.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)     5561 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/colors.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3265 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/common.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1732 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/content_menu.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2969 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/data_table.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2269 2020-12-01 12:42:15.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/dialog.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1324 2020-03-10 12:31:45.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/dialog_table.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      167 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/faq_dialog.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1629 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/figure.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)      659 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/flatpage.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     8968 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/fonts.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     9648 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/forms.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1756 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/header_menu.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1470 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/inline_tools.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      681 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/loader.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1966 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/overview_menu.css
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)     2416 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/prelogin.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1946 2020-12-31 17:57:32.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/pulldown.css
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)     1867 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/reset.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)      636 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/text.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1890 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/ui_dialogs.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)      747 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/static/css/ui_tabs.css
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.138679 fiduswriter-3.9.8/fiduswriter/base/static/fonts/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.166680 fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/
--rw-r--r--   0 johannes  (1000) johannes  (1000)    23208 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-300.woff2
--rw-r--r--   0 johannes  (1000) johannes  (1000)    23316 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-400.woff2
--rw-r--r--   0 johannes  (1000) johannes  (1000)    22820 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-700.woff2
--rw-r--r--   0 johannes  (1000) johannes  (1000)    22352 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-900.woff2
--rw-r--r--   0 johannes  (1000) johannes  (1000)     5468 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-ext-300.woff2
--rw-r--r--   0 johannes  (1000) johannes  (1000)     5296 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-ext-400.woff2
--rw-r--r--   0 johannes  (1000) johannes  (1000)     5192 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-ext-700.woff2
--rw-r--r--   0 johannes  (1000) johannes  (1000)     5192 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-ext-900.woff2
--rw-r--r--   0 johannes  (1000) johannes  (1000)     5304 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-ext-italic-400.woff2
--rw-r--r--   0 johannes  (1000) johannes  (1000)    24192 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-italic-400.woff2
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.166680 fiduswriter-3.9.8/fiduswriter/base/static/fonts/roboto/
--rw-r--r--   0 johannes  (1000) johannes  (1000)    15440 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/fonts/roboto/roboto-300.woff2
--rw-r--r--   0 johannes  (1000) johannes  (1000)    15436 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/fonts/roboto/roboto-700.woff2
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.166680 fiduswriter-3.9.8/fiduswriter/base/static/img/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    16430 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/img/accept-change.png
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2186 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/img/default_avatar.png
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)      934 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/img/dots.png
--rw-r--r--   0 johannes  (1000) johannes  (1000)    11322 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/img/error.png
--rw-r--r--   0 johannes  (1000) johannes  (1000)     6917 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/img/favicon.png
--rw-r--r--   0 johannes  (1000) johannes  (1000)     4477 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/img/fidus_face.png
--rw-r--r--   0 johannes  (1000) johannes  (1000)     4966 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/img/free_star.png
--rw-r--r--   0 johannes  (1000) johannes  (1000)     7656 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/img/icon_192.png
--rw-r--r--   0 johannes  (1000) johannes  (1000)    21686 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/img/icon_512.png
--rw-r--r--   0 johannes  (1000) johannes  (1000)    45452 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/img/wait.gif
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.170680 fiduswriter-3.9.8/fiduswriter/base/static/js/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      163 2020-06-29 09:52:39.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/admin_console.mjs
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      159 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/app.mjs
--rw-r--r--   0 johannes  (1000) johannes  (1000)      140 2020-05-13 11:21:08.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/error_hook.mjs
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.138679 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.170680 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/404/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      423 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/404/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.170680 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/admin_console/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2200 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/admin_console/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.170680 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/app/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    12184 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/app/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.170680 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    10377 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/basic.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6107 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/content_menu.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3255 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/datatable_bulk.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    10574 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/dialog.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2145 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/faq_dialog.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      864 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4361 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/network.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     8581 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/overview_menu.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1689 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/templates.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      474 2020-02-22 23:38:55.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/user.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      586 2020-02-22 19:43:36.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/user_util.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      470 2020-02-22 19:53:57.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/worker.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     9144 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/ws.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.170680 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/copyright_dialog/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5073 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/copyright_dialog/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4485 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/copyright_dialog/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.170680 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/error_hook/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2998 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/error_hook/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.170680 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/flatpage/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1233 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/flatpage/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.170680 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/indexed_db/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6114 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/indexed_db/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.170680 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/offline/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1057 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/offline/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.170680 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/prelogin/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     3184 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/prelogin/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2271 2020-12-27 21:39:09.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/prelogin/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.170680 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/prosemirror/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1715 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/prosemirror/inline_tools.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.170680 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/setup/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      933 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/modules/setup/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.142679 fiduswriter-3.9.8/fiduswriter/base/static/js/plugins/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.170680 fiduswriter-3.9.8/fiduswriter/base/static/js/plugins/app/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       31 2020-08-19 20:40:04.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/plugins/app/init.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.170680 fiduswriter-3.9.8/fiduswriter/base/static/js/plugins/prelogin/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       33 2020-08-19 20:39:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/plugins/prelogin/init.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1262 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/static/js/sw-template.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.170680 fiduswriter-3.9.8/fiduswriter/base/static/svg/
--rw-r--r--   0 johannes  (1000) johannes  (1000)    16277 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/static/svg/icon.svg
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.174680 fiduswriter-3.9.8/fiduswriter/base/templates/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      285 2020-05-13 11:21:08.000000 fiduswriter-3.9.8/fiduswriter/base/templates/500.html
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.174680 fiduswriter-3.9.8/fiduswriter/base/templates/admin/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1674 2020-05-13 11:21:08.000000 fiduswriter-3.9.8/fiduswriter/base/templates/admin/console.html
--rw-r--r--   0 johannes  (1000) johannes  (1000)      689 2020-03-15 09:48:05.000000 fiduswriter-3.9.8/fiduswriter/base/templates/admin/overview.html
--rw-r--r--   0 johannes  (1000) johannes  (1000)      237 2020-05-13 11:21:08.000000 fiduswriter-3.9.8/fiduswriter/base/templates/api_404.html
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3216 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/templates/app.html
--rw-r--r--   0 johannes  (1000) johannes  (1000)      793 2020-05-13 11:21:08.000000 fiduswriter-3.9.8/fiduswriter/base/templates/base.html
--rw-r--r--   0 johannes  (1000) johannes  (1000)       87 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/templates/email.html
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2186 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/templates/email_base.html
--rw-r--r--   0 johannes  (1000) johannes  (1000)      442 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/base/templates/manifest.json
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.174680 fiduswriter-3.9.8/fiduswriter/base/templates/socialaccount/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      121 2020-05-13 11:21:08.000000 fiduswriter-3.9.8/fiduswriter/base/templates/socialaccount/connections.html
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      108 2020-12-27 21:39:09.000000 fiduswriter-3.9.8/fiduswriter/base/templates/socialaccount/login_cancelled.html
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.174680 fiduswriter-3.9.8/fiduswriter/base/tests/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/tests/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2740 2020-03-10 12:31:45.000000 fiduswriter-3.9.8/fiduswriter/base/tests/test_admin.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2331 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/base/tests/test_manage.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2855 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/tests/test_prelogin.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      202 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/base/urls.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3669 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/views.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3871 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/base/webpack.config.template.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6531 2020-10-28 16:28:12.000000 fiduswriter-3.9.8/fiduswriter/base/ws_handler.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2294 2020-09-16 17:56:23.000000 fiduswriter-3.9.8/fiduswriter/base/ws_views.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.174680 fiduswriter-3.9.8/fiduswriter/bibliography/
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)       62 2020-02-01 14:06:35.000000 fiduswriter-3.9.8/fiduswriter/bibliography/__init__.py
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)      298 2020-02-01 14:06:35.000000 fiduswriter-3.9.8/fiduswriter/bibliography/admin.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.174680 fiduswriter-3.9.8/fiduswriter/bibliography/migrations/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2326 2020-02-01 14:06:35.000000 fiduswriter-3.9.8/fiduswriter/bibliography/migrations/0001_squashed_0011_auto_20170101_1647.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1473 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/migrations/0002_move_json_data.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2020-02-01 14:06:35.000000 fiduswriter-3.9.8/fiduswriter/bibliography/migrations/__init__.py
--rwxrwxr-x   0 johannes  (1000) johannes  (1000)      935 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/models.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      135 2020-08-27 07:41:05.000000 fiduswriter-3.9.8/fiduswriter/bibliography/package.json
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.142679 fiduswriter-3.9.8/fiduswriter/bibliography/static/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.174680 fiduswriter-3.9.8/fiduswriter/bibliography/static/css/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2899 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/css/bibliography.css
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.174680 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      309 2020-02-01 14:06:35.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/biblatex_import_worker.mjs
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.142679 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.174680 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.174680 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/database/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6869 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/database/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1997 2020-12-11 16:49:15.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/database/server_connector.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.174680 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/export/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      829 2020-02-01 14:06:35.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/export/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.178680 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      839 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/cats.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.178680 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      922 2020-03-10 04:36:41.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/date.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4159 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/key.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2401 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/key_list.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3910 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/literal.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2328 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/literal_list.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2852 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/literal_long.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5270 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/name.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2316 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/name_list.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3689 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/range.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2350 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/range_list.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      859 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/tag_list.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2924 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/title.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1550 2020-02-01 14:06:35.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/uri.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      624 2020-02-01 14:06:35.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/verbatim.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     9812 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/index.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     9969 2020-02-23 02:16:13.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/strings.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2312 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.178680 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/import/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2595 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/import/biblatex.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2869 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/import/dialog.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)       94 2020-02-01 14:06:35.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/import/index.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      471 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/import/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.178680 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/overview/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    13466 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/overview/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3051 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/overview/menu.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1100 2020-02-01 14:06:35.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/overview/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.178680 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/schema/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1547 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/schema/common.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2336 2020-02-01 14:06:35.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/schema/csl_bib.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      480 2020-02-01 14:06:35.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/schema/literal.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      725 2020-02-01 14:06:35.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/schema/literal_long.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      619 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/schema/title.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      914 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/tools.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.142679 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/plugins/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.178680 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/plugins/bibliography_overview/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       40 2020-02-01 14:06:35.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/plugins/bibliography_overview/init.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.142679 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/workers/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.178680 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/workers/importer/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2750 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/static/js/workers/importer/biblatex.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.178680 fiduswriter-3.9.8/fiduswriter/bibliography/tests/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2020-02-01 14:06:35.000000 fiduswriter-3.9.8/fiduswriter/bibliography/tests/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)    11769 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/bibliography/tests/test_overview.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.178680 fiduswriter-3.9.8/fiduswriter/bibliography/tests/uploads/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      192 2020-02-01 14:06:35.000000 fiduswriter-3.9.8/fiduswriter/bibliography/tests/uploads/bibliography.bib
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)      498 2020-02-01 14:06:35.000000 fiduswriter-3.9.8/fiduswriter/bibliography/urls.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5508 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/bibliography/views.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.178680 fiduswriter-3.9.8/fiduswriter/browser_check/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/browser_check/__init__.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      481 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/browser_check/package.json
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.142679 fiduswriter-3.9.8/fiduswriter/browser_check/templates/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.178680 fiduswriter-3.9.8/fiduswriter/browser_check/templates/browser_check/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1179 2020-01-02 09:57:49.000000 fiduswriter-3.9.8/fiduswriter/browser_check/templates/browser_check/browser_not_supported.html
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.178680 fiduswriter-3.9.8/fiduswriter/browser_check/tests/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/browser_check/tests/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2065 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/browser_check/tests/test_access.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      114 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/browser_check/urls.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      175 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/browser_check/views.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3963 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/configuration.py-default
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       64 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/dev-requirements.txt
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.182680 fiduswriter-3.9.8/fiduswriter/document/
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)      190 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/__init__.py
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)     2081 2020-04-02 15:01:45.000000 fiduswriter-3.9.8/fiduswriter/document/admin.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      364 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/apps.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.182680 fiduswriter-3.9.8/fiduswriter/document/fixtures/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2777 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/fixtures/initial_documenttemplates.json
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.182680 fiduswriter-3.9.8/fiduswriter/document/helpers/
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/helpers/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1716 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/helpers/serializers.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1959 2020-03-10 12:31:45.000000 fiduswriter-3.9.8/fiduswriter/document/helpers/session_user_info.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.182680 fiduswriter-3.9.8/fiduswriter/document/management/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/management/__init__.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.182680 fiduswriter-3.9.8/fiduswriter/document/management/commands/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1379 2020-12-26 13:18:19.000000 fiduswriter-3.9.8/fiduswriter/document/management/commands/export_schema.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.182680 fiduswriter-3.9.8/fiduswriter/document/migrations/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     5726 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/migrations/0001_squashed_20200219.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3318 2020-12-28 09:33:35.000000 fiduswriter-3.9.8/fiduswriter/document/migrations/0002_fidus_3_2.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7353 2020-12-28 09:33:35.000000 fiduswriter-3.9.8/fiduswriter/document/migrations/0003_fidus_3_3.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3807 2021-01-05 11:35:13.000000 fiduswriter-3.9.8/fiduswriter/document/migrations/0004_move_json_data.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      570 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/migrations/0005_auto_20201109_0255.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      399 2020-12-27 21:39:09.000000 fiduswriter-3.9.8/fiduswriter/document/migrations/0006_auto_20201209_1610.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6783 2020-12-28 09:33:35.000000 fiduswriter-3.9.8/fiduswriter/document/migrations/0007_fix_fidus_3_3.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/migrations/__init__.py
--rwxrwxr-x   0 johannes  (1000) johannes  (1000)    11461 2020-12-27 21:39:09.000000 fiduswriter-3.9.8/fiduswriter/document/models.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1079 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/package.json
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2091 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/prosemirror.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      444 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/signals.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.150679 fiduswriter-3.9.8/fiduswriter/document/static/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.186680 fiduswriter-3.9.8/fiduswriter/document/static/css/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      127 2020-01-28 23:50:30.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/access_rights_dialog.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)      290 2020-01-28 23:50:30.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/carets.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1320 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/chat.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)      748 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/citation_dialog.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)      309 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/contributors.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3982 2020-12-31 17:57:32.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/document.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)      134 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/document_overview.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)     3598 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/document_template_designer.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)      557 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/document_template_designer_admin.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      722 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/dot_menu.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    22087 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/editor.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1820 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/footnotes.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    10046 2020-12-31 17:57:32.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/margin_boxes.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3379 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/merge.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)      105 2020-01-28 23:50:30.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/review.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)      164 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/table.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)      574 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/tags.css
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1039 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/css/tracking.css
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.142679 fiduswriter-3.9.8/fiduswriter/document/static/fonts/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.190680 fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/
--rw-r--r--   0 johannes  (1000) johannes  (1000)   191484 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/Cardo-Bold.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)   153060 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/Cardo-Italic.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)   223616 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/Cardo-Regular.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    44512 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/CrimsonText-Bold.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    39280 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/CrimsonText-BoldItalic.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    55548 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/CrimsonText-Italic.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    95500 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/CrimsonText-Roman.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    26424 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/Lobster-1.4.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    41084 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/NoticiaText-Bold.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    37520 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/NoticiaText-BoldItalic.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    37404 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/NoticiaText-Italic.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    41604 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/NoticiaText-Regular.woff
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)    91484 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/OpenSans-Bold.woff
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)    94044 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/OpenSans-Regular.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    63256 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/SourceSansPro-Bold.woff
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.190680 fiduswriter-3.9.8/fiduswriter/document/static/js/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      365 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/adjust_doc_to_template_worker.mjs
--rw-r--r--   0 johannes  (1000) johannes  (1000)      221 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/document_template_admin.mjs
--rw-r--r--   0 johannes  (1000) johannes  (1000)      157 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/maintenance.mjs
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.150679 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.194680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/citations/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1308 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/citations/citeproc_sys.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5923 2020-06-11 04:48:02.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/citations/format.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1720 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/citations/render.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.194680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4921 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/admin.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    23684 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/designer.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    10889 2020-10-23 10:37:35.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/document_style_dialog.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    12813 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/export_template_dialog.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1670 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/extract_template.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     8636 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/fix_doc.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      246 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6503 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/schema.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    31344 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/templates.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1931 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/tools.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.194680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.194680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/access_rights/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    12207 2020-12-27 21:39:09.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/access_rights/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3982 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/access_rights/templates.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      954 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/invite.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.194680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/overview/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    14382 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/overview/actions.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    13271 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/overview/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5531 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/overview/menu.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      533 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/overview/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.194680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/revisions/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5647 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/revisions/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1902 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/revisions/templates.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1743 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/tools.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.194680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.194680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/citations/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     8476 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/citations/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.146679 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.194680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/copy/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       76 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/copy/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      959 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/copy/schema.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6007 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/copy/serializers.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.198680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/paste/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1915 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/paste/fidus_writer.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2378 2020-06-11 08:33:17.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/paste/general.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      892 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/paste/google_docs.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2239 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/paste/html.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)       66 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/paste/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1083 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/paste/libreoffice_writer.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3075 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/paste/microsoft_word.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2774 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/paste/text.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.198680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4742 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/chat.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2002 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/colors.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    18284 2020-12-28 01:14:38.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/doc.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2911 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.198680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2653 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/changeset.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    35635 2020-12-27 21:39:09.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/editor.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4923 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/footnotes.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    10823 2020-12-27 21:39:09.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    10424 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/recreate_transform.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3491 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/schema.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.198680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/state_plugins/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6136 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/state_plugins/action.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1673 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/state_plugins/clipboard.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    22790 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/state_plugins/diff.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       90 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/state_plugins/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7210 2020-12-27 21:39:09.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/tools.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      473 2019-11-23 15:40:08.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.198680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/comments/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      950 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/comments/comment.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.198680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/comments/editors/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1366 2020-08-24 18:06:36.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/comments/editors/answer.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7798 2020-12-31 17:58:21.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/comments/editors/comment.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      146 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/comments/editors/index.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      448 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/comments/editors/notify.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1336 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/comments/editors/schema.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      295 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/comments/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    12782 2020-12-31 17:57:32.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/comments/interactions.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    12682 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/comments/store.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.198680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/databases/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5295 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/databases/bibliography.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7253 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/databases/images.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2508 2020-12-27 21:39:09.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/databases/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.202680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    12360 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/citation.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     3686 2019-10-17 15:05:38.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/contributor.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    13470 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/figure.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      396 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/index.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1675 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/language.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    11386 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/link.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3866 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/math.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2081 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/ordered_list.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1018 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/revision.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7717 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/table.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    15936 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.202680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/document_template/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    11414 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/document_template/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.202680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/footnotes/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7174 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/footnotes/editor.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      363 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/footnotes/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7518 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/footnotes/layout.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.202680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/footnotes/state_plugins/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      925 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/footnotes/state_plugins/access_rights.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       61 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/footnotes/state_plugins/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    21613 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2614 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/keymap.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.202680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/marginboxes/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    27512 2020-12-31 17:57:32.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/marginboxes/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    21089 2020-12-31 17:57:32.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/marginboxes/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.202680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.202680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/figure/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       40 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/figure/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1224 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/figure/model.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.202680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/headerbar/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       76 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/headerbar/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    24167 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/headerbar/model.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    13091 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/headerbar/view.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.202680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/image/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       38 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/image/index.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1089 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/image/model.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      396 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.202680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/navigator/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       44 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/navigator/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      565 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/navigator/model.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.202680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/ordered_list/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       45 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/ordered_list/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      511 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/ordered_list/model.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.202680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/selection/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       84 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/selection/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4392 2020-11-26 19:52:06.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/selection/model.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5314 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/selection/view.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.202680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/table/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       38 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/table/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    13680 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/table/model.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.202680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/toolbar/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       72 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/toolbar/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    26842 2020-11-26 19:52:06.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/toolbar/model.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    11700 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/toolbar/view.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.202680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/navigator/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7932 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/navigator/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.206680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1277 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/access_rights.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3499 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/citation_render.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2177 2019-11-02 10:42:57.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/clipboard.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4556 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/collab_carets.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     8234 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/comments.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5067 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/contributor_input.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     9328 2020-11-26 19:52:06.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/document_template.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3513 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/figure.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7596 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/footnote_markers.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      321 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/headerbar.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1952 2020-11-26 19:52:06.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2054 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/jump_hidden_nodes.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    19870 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/links.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      395 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/marginboxes.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2584 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/ordered_list_menu.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4274 2020-11-26 19:52:06.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/placeholders.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7371 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/search.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      334 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/selection_menu.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7176 2020-11-26 19:06:33.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/settings.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3819 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/table.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     8460 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/tag_input.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5624 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/toc_render.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      316 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/toolbar.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.206680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/track/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3562 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/track/find_selected_changes.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2822 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/track/helpers.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      152 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/track/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4085 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/track/plugin.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.206680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/tools/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      146 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/tools/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.206680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/tools/key_bindings/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      604 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/tools/key_bindings/index.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2815 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/tools/key_bindings/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.206680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/tools/search_replace/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    10353 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/tools/search_replace/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      523 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/tools/search_replace/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.206680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/tools/word_count/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2388 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/tools/word_count/index.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1211 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/tools/word_count/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.206680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2868 2020-08-24 18:06:36.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/accept.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2979 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/accept_all.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2080 2020-11-18 16:58:19.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/accept_all_no_insertions.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    17917 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/amend_transaction.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2880 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/delete.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      269 2020-01-02 09:57:49.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2849 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/mod.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3453 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/reject.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3655 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/reject_all.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.146679 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.210680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6803 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/citations.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7940 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/footnotes.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2696 2020-12-11 17:39:01.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/images.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3164 2020-12-11 16:35:33.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    11586 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/lists.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3149 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/math.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4634 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/metadata.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4136 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/rels.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     9428 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/render.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    30036 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/richtext.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     3745 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/tables.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.210680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/epub/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7009 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/epub/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7134 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/epub/templates.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5042 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/epub/tools.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.210680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/html/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2972 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/html/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1297 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/html/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.210680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/jats/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     5078 2019-11-05 22:04:35.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/jats/citations.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    29148 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/jats/convert.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2259 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/jats/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1208 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/jats/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.210680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/latex/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    31491 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/latex/convert.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      834 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/latex/escape_latex.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2077 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/latex/index.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      618 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/latex/readme.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.210680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/native/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1237 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/native/copy.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      792 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/native/file.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      111 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/native/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2145 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/native/revision.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3023 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/native/shrink.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1040 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/native/zip.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.210680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4053 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/citations.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4957 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/footnotes.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3188 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/images.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2745 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2469 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/math.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5036 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/metadata.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6530 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/render.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    19150 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/richtext.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    16047 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/styles.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.210680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/print/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4965 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/print/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.214680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/tools/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3771 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/tools/doc_content.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     8587 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/tools/dom_export.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      228 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/tools/file.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1029 2020-12-11 16:30:25.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/tools/html.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2245 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/tools/json.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3055 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/tools/xml_zip.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3014 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/tools/zip.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.214680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/importer/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     8181 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/importer/file.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2184 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/importer/get_images.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5481 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/importer/native.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      777 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/importer/update.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.214680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/maintenance/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     9971 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/maintenance/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.214680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.214680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1780 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/annotate.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1777 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/base.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1343 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/citation.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      710 2020-12-26 13:17:58.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/equation.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4740 2020-12-27 21:39:09.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/figure.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1028 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/heading.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      715 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1955 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/list.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1937 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/reference.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2531 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/table.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4315 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/track.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2387 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/const.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    29380 2020-12-27 21:39:09.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/convert.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.214680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/document/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3136 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/document/content.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1981 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/document/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     8027 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/document/structure.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      846 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/export.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2539 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/footnotes.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      997 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/footnotes_convert.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5152 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/i18n.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      208 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/index.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1902 2019-09-29 23:49:15.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/mini_json.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.214680 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/test_caret/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      492 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/modules/test_caret/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.150679 fiduswriter-3.9.8/fiduswriter/document/static/js/plugins/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.214680 fiduswriter-3.9.8/fiduswriter/document/static/js/plugins/citation_dialog/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       43 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/plugins/citation_dialog/init.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.214680 fiduswriter-3.9.8/fiduswriter/document/static/js/plugins/documents_overview/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       45 2020-05-13 11:21:08.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/plugins/documents_overview/init.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.214680 fiduswriter-3.9.8/fiduswriter/document/static/js/plugins/editor/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       34 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/plugins/editor/init.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.214680 fiduswriter-3.9.8/fiduswriter/document/static/js/plugins/schema_export/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       41 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/plugins/schema_export/init.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      206 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/schema_export.mjs
--rw-r--r--   0 johannes  (1000) johannes  (1000)      114 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/test_caret.mjs
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.150679 fiduswriter-3.9.8/fiduswriter/document/static/js/workers/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.214680 fiduswriter-3.9.8/fiduswriter/document/static/js/workers/document_template/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1198 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/document/static/js/workers/document_template/adjust_doc.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.214680 fiduswriter-3.9.8/fiduswriter/document/static/ogg/
--rw-r--r--   0 johannes  (1000) johannes  (1000)    18048 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/static/ogg/chat_notification.ogg
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.150679 fiduswriter-3.9.8/fiduswriter/document/templates/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.150679 fiduswriter-3.9.8/fiduswriter/document/templates/admin/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.214680 fiduswriter-3.9.8/fiduswriter/document/templates/admin/document/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.218680 fiduswriter-3.9.8/fiduswriter/document/templates/admin/document/document/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      475 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/templates/admin/document/document/change_list_object_tools.html
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.218680 fiduswriter-3.9.8/fiduswriter/document/templates/admin/document/documenttemplate/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      635 2020-05-13 11:21:08.000000 fiduswriter-3.9.8/fiduswriter/document/templates/admin/document/documenttemplate/change_form.html
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1286 2020-05-13 11:21:08.000000 fiduswriter-3.9.8/fiduswriter/document/templates/admin/document/maintenance.html
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.218680 fiduswriter-3.9.8/fiduswriter/document/tests/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/tests/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2915 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/document/tests/editor_helper.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    17904 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/tests/test_admin.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    43519 2020-12-31 17:57:32.000000 fiduswriter-3.9.8/fiduswriter/document/tests/test_collaboration.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    41137 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/tests/test_editor.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    24540 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/tests/test_export.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6016 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/tests/test_message_exchange.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    30249 2020-12-01 12:42:15.000000 fiduswriter-3.9.8/fiduswriter/document/tests/test_offline.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.218680 fiduswriter-3.9.8/fiduswriter/document/tests/uploads/
--rw-r--r--   0 johannes  (1000) johannes  (1000)    45965 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/tests/uploads/image.png
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)     2542 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/document/urls.py
--rwxrwxr-x   0 johannes  (1000) johannes  (1000)    38974 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/views.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    28963 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/document/ws_views.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.218680 fiduswriter-3.9.8/fiduswriter/feedback/
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)       50 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/feedback/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      168 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/feedback/admin.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.218680 fiduswriter-3.9.8/fiduswriter/feedback/migrations/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      713 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/feedback/migrations/0001_initial.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/feedback/migrations/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1043 2020-03-16 20:47:16.000000 fiduswriter-3.9.8/fiduswriter/feedback/models.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.150679 fiduswriter-3.9.8/fiduswriter/feedback/static/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.150679 fiduswriter-3.9.8/fiduswriter/feedback/static/css/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.218680 fiduswriter-3.9.8/fiduswriter/feedback/static/css/feedback/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2323 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/feedback/static/css/feedback/feedback.css
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.150679 fiduswriter-3.9.8/fiduswriter/feedback/static/js/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.150679 fiduswriter-3.9.8/fiduswriter/feedback/static/js/modules/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.218680 fiduswriter-3.9.8/fiduswriter/feedback/static/js/modules/feedback/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3733 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/feedback/static/js/modules/feedback/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.218680 fiduswriter-3.9.8/fiduswriter/feedback/tests/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-11-05 22:04:35.000000 fiduswriter-3.9.8/fiduswriter/feedback/tests/__init__.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3191 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/feedback/tests/test_feedback.py
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)      129 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/feedback/urls.py
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)      557 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/feedback/views.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.218680 fiduswriter-3.9.8/fiduswriter/fixturemedia/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       51 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/fixturemedia/__init__.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.218680 fiduswriter-3.9.8/fiduswriter/fixturemedia/management/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/fixturemedia/management/__init__.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.218680 fiduswriter-3.9.8/fiduswriter/fixturemedia/management/commands/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/fixturemedia/management/commands/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     3142 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/fixturemedia/management/commands/dumpdata.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3183 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/fixturemedia/management/commands/loaddata.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.218680 fiduswriter-3.9.8/fiduswriter/locale/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.150679 fiduswriter-3.9.8/fiduswriter/locale/bg/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.222680 fiduswriter-3.9.8/fiduswriter/locale/bg/LC_MESSAGES/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     7727 2021-01-05 13:17:40.000000 fiduswriter-3.9.8/fiduswriter/locale/bg/LC_MESSAGES/django.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    12634 2020-12-31 18:00:45.000000 fiduswriter-3.9.8/fiduswriter/locale/bg/LC_MESSAGES/django.po
--rw-r--r--   0 johannes  (1000) johannes  (1000)   104753 2021-01-05 13:17:40.000000 fiduswriter-3.9.8/fiduswriter/locale/bg/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)   197856 2020-12-31 18:21:32.000000 fiduswriter-3.9.8/fiduswriter/locale/bg/LC_MESSAGES/djangojs.po
--rw-r--r--   0 johannes  (1000) johannes  (1000)      609 2020-01-02 09:57:49.000000 fiduswriter-3.9.8/fiduswriter/locale/copyright.txt
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.150679 fiduswriter-3.9.8/fiduswriter/locale/de/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.222680 fiduswriter-3.9.8/fiduswriter/locale/de/LC_MESSAGES/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     6213 2021-01-05 13:17:40.000000 fiduswriter-3.9.8/fiduswriter/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    10881 2020-12-31 18:00:45.000000 fiduswriter-3.9.8/fiduswriter/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 johannes  (1000) johannes  (1000)    83975 2021-01-05 13:17:40.000000 fiduswriter-3.9.8/fiduswriter/locale/de/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)   174813 2020-12-31 18:21:32.000000 fiduswriter-3.9.8/fiduswriter/locale/de/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.150679 fiduswriter-3.9.8/fiduswriter/locale/es/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.222680 fiduswriter-3.9.8/fiduswriter/locale/es/LC_MESSAGES/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     6035 2021-01-05 13:17:40.000000 fiduswriter-3.9.8/fiduswriter/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    10596 2020-12-31 18:00:45.000000 fiduswriter-3.9.8/fiduswriter/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0 johannes  (1000) johannes  (1000)    83451 2021-01-05 13:17:40.000000 fiduswriter-3.9.8/fiduswriter/locale/es/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)   174281 2020-12-31 18:21:32.000000 fiduswriter-3.9.8/fiduswriter/locale/es/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.150679 fiduswriter-3.9.8/fiduswriter/locale/fr/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.222680 fiduswriter-3.9.8/fiduswriter/locale/fr/LC_MESSAGES/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     7632 2021-01-05 13:17:40.000000 fiduswriter-3.9.8/fiduswriter/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    11173 2021-01-05 11:36:58.000000 fiduswriter-3.9.8/fiduswriter/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 johannes  (1000) johannes  (1000)    83496 2021-01-05 13:17:40.000000 fiduswriter-3.9.8/fiduswriter/locale/fr/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)   176456 2021-01-05 11:36:58.000000 fiduswriter-3.9.8/fiduswriter/locale/fr/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.150679 fiduswriter-3.9.8/fiduswriter/locale/it/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.222680 fiduswriter-3.9.8/fiduswriter/locale/it/LC_MESSAGES/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     6125 2021-01-05 13:17:40.000000 fiduswriter-3.9.8/fiduswriter/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    10730 2020-12-31 18:00:45.000000 fiduswriter-3.9.8/fiduswriter/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0 johannes  (1000) johannes  (1000)    81067 2021-01-05 13:17:40.000000 fiduswriter-3.9.8/fiduswriter/locale/it/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)   173513 2020-12-31 18:21:32.000000 fiduswriter-3.9.8/fiduswriter/locale/it/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.150679 fiduswriter-3.9.8/fiduswriter/locale/pt_BR/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.222680 fiduswriter-3.9.8/fiduswriter/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     5940 2021-01-05 13:17:40.000000 fiduswriter-3.9.8/fiduswriter/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    10434 2020-12-31 18:00:45.000000 fiduswriter-3.9.8/fiduswriter/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0 johannes  (1000) johannes  (1000)    82052 2021-01-05 13:17:40.000000 fiduswriter-3.9.8/fiduswriter/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 johannes  (1000) johannes  (1000)   173060 2020-12-31 18:21:32.000000 fiduswriter-3.9.8/fiduswriter/locale/pt_BR/LC_MESSAGES/djangojs.po
--rwxrwxr-x   0 johannes  (1000) johannes  (1000)     3085 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/manage.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.222680 fiduswriter-3.9.8/fiduswriter/menu/
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)       58 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/menu/__init__.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/menu/static/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/menu/static/js/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/menu/static/js/modules/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.222680 fiduswriter-3.9.8/fiduswriter/menu/static/js/modules/menu/
--rwxrwxr-x   0 johannes  (1000) johannes  (1000)     2822 2021-01-05 12:13:06.000000 fiduswriter-3.9.8/fiduswriter/menu/static/js/modules/menu/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      472 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/menu/static/js/modules/menu/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/menu/static/js/plugins/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.226680 fiduswriter-3.9.8/fiduswriter/menu/static/js/plugins/menu/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       37 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/menu/static/js/plugins/menu/init.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)       19 2020-01-02 09:57:49.000000 fiduswriter-3.9.8/fiduswriter/mysql-requirements.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)       16 2019-10-30 06:04:12.000000 fiduswriter-3.9.8/fiduswriter/postgresql-requirements.txt
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      299 2021-01-05 13:17:05.000000 fiduswriter-3.9.8/fiduswriter/requirements.txt
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.226680 fiduswriter-3.9.8/fiduswriter/style/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       73 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      565 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/admin.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.226680 fiduswriter-3.9.8/fiduswriter/style/fixtures/
--rw-r--r--   0 johannes  (1000) johannes  (1000)    35063 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/initial_styles.json
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.226680 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/export-template-files/
--rw-r--r--   0 johannes  (1000) johannes  (1000)    10707 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/export-template-files/Classic.docx
--rw-r--r--   0 johannes  (1000) johannes  (1000)     9852 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/export-template-files/Free.odt
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.234680 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/
--rw-r--r--   0 johannes  (1000) johannes  (1000)   191484 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/Cardo-Bold.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)   153060 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/Cardo-Italic.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)   223616 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/Cardo-Regular.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    44512 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/CrimsonText-Bold.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    39280 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/CrimsonText-BoldItalic.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    55548 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/CrimsonText-Italic.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    95500 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/CrimsonText-Roman.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    26424 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/Lobster-1.4.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    37520 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-BoldItalic.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    37520 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-BoldItalic_KMSnKTE.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    37520 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-BoldItalic_Xg38HXg.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    41084 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Bold_2.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    41084 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Bold_2_77vhC50.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    41084 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Bold_2_qiGg4Ow.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    37404 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Italic.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    37404 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Italic_3AoQkPt.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    37404 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Italic_ai8IvB3.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    41604 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Regular.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    41604 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Regular_eNSdC3U.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    41604 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Regular_zGx3t7x.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    91484 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/OpenSans-Bold.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    94044 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/OpenSans-Regular.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    63256 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/SourceSansPro-Bold.woff
--rw-r--r--   0 johannes  (1000) johannes  (1000)    63256 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/SourceSansPro-Bold_ySHS5jh.woff
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.234680 fiduswriter-3.9.8/fiduswriter/style/migrations/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     3043 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/style/migrations/0001_squashed_20200219.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/migrations/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2523 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/models.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      571 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/style/urls.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     4875 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/style/views.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      697 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/stylelint.config.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)       38 2019-10-30 15:40:18.000000 fiduswriter-3.9.8/fiduswriter/test-requirements.txt
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.234680 fiduswriter-3.9.8/fiduswriter/testing/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       38 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/testing/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1857 2020-05-13 11:21:08.000000 fiduswriter-3.9.8/fiduswriter/testing/eslint_import_resolver.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3524 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/testing/selenium_helper.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6671 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/testing/testcases.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.238680 fiduswriter-3.9.8/fiduswriter/user/
--rwxr-xr-x   0 johannes  (1000) johannes  (1000)       97 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/user/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1190 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/user/adapter.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      287 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/user/admin.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      118 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/user/apps.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      506 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/user/forms.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.238680 fiduswriter-3.9.8/fiduswriter/user/migrations/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1605 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/user/migrations/0001_squashed_0003_auto_20151226_1110.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      661 2021-01-05 13:17:05.000000 fiduswriter-3.9.8/fiduswriter/user/migrations/0002_loginas.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/user/migrations/__init__.py
--rwxrwxr-x   0 johannes  (1000) johannes  (1000)     1691 2021-01-05 13:17:05.000000 fiduswriter-3.9.8/fiduswriter/user/models.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3202 2020-12-27 21:39:09.000000 fiduswriter-3.9.8/fiduswriter/user/signals.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/user/static/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.238680 fiduswriter-3.9.8/fiduswriter/user/static/css/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      973 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/user/static/css/show_profile.css
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/user/static/js/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.238680 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/contacts/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4153 2020-12-27 21:39:09.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/contacts/add_dialog.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1427 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/contacts/delete_dialog.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3780 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/contacts/index.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1261 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/contacts/menu.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1226 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/contacts/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.238680 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/email_confirm/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4355 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/email_confirm/index.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2458 2019-11-16 17:50:16.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/email_confirm/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.238680 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/login/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7144 2020-12-27 21:39:09.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/login/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.238680 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/password_reset/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5163 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/password_reset/change_password.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      115 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/password_reset/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4061 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/password_reset/request_email.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.238680 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/profile/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1990 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/profile/delete_user.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    12498 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/profile/dialogs.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4182 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/profile/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    10161 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/profile/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.238680 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/signup/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     8280 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/modules/signup/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/user/static/js/plugins/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.238680 fiduswriter-3.9.8/fiduswriter/user/static/js/plugins/confirm_account/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       43 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/plugins/confirm_account/init.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.238680 fiduswriter-3.9.8/fiduswriter/user/static/js/plugins/login/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       33 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/user/static/js/plugins/login/init.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/user/templates/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/user/templates/account/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.238680 fiduswriter-3.9.8/fiduswriter/user/templates/account/email/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      719 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/user/templates/account/email/email_confirmation_message.html
--rw-r--r--   0 johannes  (1000) johannes  (1000)       62 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/user/templates/account/email/email_confirmation_signup_message.html
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      875 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/user/templates/account/email/password_reset_key_message.html
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.238680 fiduswriter-3.9.8/fiduswriter/user/tests/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/user/tests/__init__.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5074 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/user/tests/test_contacts.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)    13106 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/user/tests/test_profile.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1652 2020-05-13 11:21:08.000000 fiduswriter-3.9.8/fiduswriter/user/urls.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1969 2020-03-10 12:31:45.000000 fiduswriter-3.9.8/fiduswriter/user/util.py
--rwxrwxr-x   0 johannes  (1000) johannes  (1000)    12900 2020-12-27 21:39:09.000000 fiduswriter-3.9.8/fiduswriter/user/views.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.242680 fiduswriter-3.9.8/fiduswriter/user_template_manager/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      118 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/user_template_manager/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      357 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/user_template_manager/apps.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/user_template_manager/static/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.242680 fiduswriter-3.9.8/fiduswriter/user_template_manager/static/css/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      234 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/user_template_manager/static/css/errorlist.css
--rw-r--r--   0 johannes  (1000) johannes  (1000)      308 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/user_template_manager/static/css/user_template_manager.css
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/modules/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.242680 fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/modules/user_template_manager/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2797 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/modules/user_template_manager/actions.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4244 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/modules/user_template_manager/editor.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)       92 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/modules/user_template_manager/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1706 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/modules/user_template_manager/menu.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7307 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/modules/user_template_manager/overview.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/plugins/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.242680 fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/plugins/app/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      875 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/plugins/app/user_template_manager.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.242680 fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/plugins/menu/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      407 2020-01-02 09:57:49.000000 fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/plugins/menu/user_template_manager.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)      391 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/user_template_manager/urls.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     4321 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/user_template_manager/views.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.242680 fiduswriter-3.9.8/fiduswriter/usermedia/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       86 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/usermedia/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      521 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/usermedia/admin.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.242680 fiduswriter-3.9.8/fiduswriter/usermedia/migrations/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     4369 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/usermedia/migrations/0001_squashed_0009_auto_20170908_0953.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      584 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/usermedia/migrations/0002_auto_20200205_2140.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)      669 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/usermedia/migrations/0003_auto_20200205_2230.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      706 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/usermedia/migrations/0004_auto_20200205_2347.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3264 2021-01-05 11:35:13.000000 fiduswriter-3.9.8/fiduswriter/usermedia/migrations/0005_move_json_data.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      633 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/usermedia/migrations/0006_auto_20200820_0510.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/usermedia/migrations/__init__.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     7272 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/usermedia/models.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)      289 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/usermedia/package.json
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/usermedia/static/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.242680 fiduswriter-3.9.8/fiduswriter/usermedia/static/css/
--rw-r--r--   0 johannes  (1000) johannes  (1000)      195 2020-03-03 14:35:50.000000 fiduswriter-3.9.8/fiduswriter/usermedia/static/css/dialog_usermedia.css
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.242680 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1899 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/database.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.242680 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/edit_dialog/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6333 2020-12-24 00:27:12.000000 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/edit_dialog/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5431 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/edit_dialog/model.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     1925 2020-06-11 02:38:24.000000 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/edit_dialog/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.246680 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/overview/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     3467 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/overview/categories.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     9680 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/overview/index.js
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     2154 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/overview/menu.js
--rw-r--r--   0 johannes  (1000) johannes  (1000)     1057 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/overview/templates.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.246680 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/selection_dialog/
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6145 2020-11-26 14:54:59.000000 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/selection_dialog/index.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.154679 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/plugins/
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.246680 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/plugins/images_overview/
--rw-r--r--   0 johannes  (1000) johannes  (1000)       33 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/usermedia/static/js/plugins/images_overview/init.js
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.246680 fiduswriter-3.9.8/fiduswriter/usermedia/tests/
--rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/usermedia/tests/__init__.py
--rw-r--r--   0 johannes  (1000) johannes  (1000)     7396 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/usermedia/tests/test_overview.py
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.246680 fiduswriter-3.9.8/fiduswriter/usermedia/tests/uploads/
--rw-r--r--   0 johannes  (1000) johannes  (1000)    45965 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/usermedia/tests/uploads/image.png
--rw-r--r--   0 johannes  (1000) johannes  (1000)      361 2019-09-23 11:40:46.000000 fiduswriter-3.9.8/fiduswriter/usermedia/urls.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     5869 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/fiduswriter/usermedia/views.py
--rw-rw-r--   0 johannes  (1000) johannes  (1000)        6 2021-01-05 13:17:05.000000 fiduswriter-3.9.8/fiduswriter/version.txt
-drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 13:17:44.158680 fiduswriter-3.9.8/fiduswriter.egg-info/
--rw-r--r--   0 johannes  (1000) johannes  (1000)     2759 2021-01-05 13:17:40.000000 fiduswriter-3.9.8/fiduswriter.egg-info/PKG-INFO
--rw-r--r--   0 johannes  (1000) johannes  (1000)    37827 2021-01-05 13:17:44.000000 fiduswriter-3.9.8/fiduswriter.egg-info/SOURCES.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)        1 2021-01-05 13:17:40.000000 fiduswriter-3.9.8/fiduswriter.egg-info/dependency_links.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)       58 2021-01-05 13:17:40.000000 fiduswriter-3.9.8/fiduswriter.egg-info/entry_points.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)      573 2021-01-05 13:17:40.000000 fiduswriter-3.9.8/fiduswriter.egg-info/requires.txt
--rw-r--r--   0 johannes  (1000) johannes  (1000)       12 2021-01-05 13:17:40.000000 fiduswriter-3.9.8/fiduswriter.egg-info/top_level.txt
--rw-rw-r--   0 johannes  (1000) johannes  (1000)       38 2021-01-05 13:17:44.246680 fiduswriter-3.9.8/setup.cfg
--rw-rw-r--   0 johannes  (1000) johannes  (1000)     6911 2020-12-28 00:54:47.000000 fiduswriter-3.9.8/setup.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.216592 fiduswriter-3.9.9/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      785 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/MANIFEST.in
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2759 2021-01-05 14:54:58.216592 fiduswriter-3.9.9/PKG-INFO
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)     1408 2019-11-03 23:58:06.000000 fiduswriter-3.9.9/README.md
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.136592 fiduswriter-3.9.9/fiduswriter/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      159 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/.babelrc
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       82 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/.eslintignore
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    10135 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/.eslintrc.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.140592 fiduswriter-3.9.9/fiduswriter/base/
+-rwxrwxr-x   0 johannes  (1000) johannes  (1000)      683 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      326 2020-02-12 14:24:52.000000 fiduswriter-3.9.9/fiduswriter/base/apps.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      495 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/decorators.py
+-rwxrwxr-x   0 johannes  (1000) johannes  (1000)    10773 2021-01-05 13:17:05.000000 fiduswriter-3.9.9/fiduswriter/base/default_settings.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      797 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/django_handler_mixin.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.140592 fiduswriter-3.9.9/fiduswriter/base/fixtures/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    34753 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/fixtures/initial_terms.json
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.140592 fiduswriter-3.9.9/fiduswriter/base/handlers/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2824 2020-10-23 20:16:08.000000 fiduswriter-3.9.9/fiduswriter/base/handlers/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      191 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/html_email.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.140592 fiduswriter-3.9.9/fiduswriter/base/management/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      199 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/management/__init__.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.140592 fiduswriter-3.9.9/fiduswriter/base/management/commands/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/management/commands/__init__.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4027 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/management/commands/bundle_mathlive.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      357 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/management/commands/collectstatic.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      476 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/management/commands/compilemessages.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1381 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/management/commands/initadmin.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1082 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/management/commands/jest.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      302 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/management/commands/lint.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1292 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/management/commands/lint_css.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1697 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/management/commands/lint_js.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      581 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/management/commands/lint_py.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2878 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/management/commands/makemessages.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4420 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/management/commands/runserver.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2944 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/management/commands/setup.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1224 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/management/commands/startproject.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2931 2020-12-31 17:57:32.000000 fiduswriter-3.9.9/fiduswriter/base/package.json
+-rwxrwxr-x   0 johannes  (1000) johannes  (1000)     2445 2021-01-05 13:17:05.000000 fiduswriter-3.9.9/fiduswriter/base/root_urls.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.140592 fiduswriter-3.9.9/fiduswriter/base/servers/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/servers/__init__.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1942 2020-10-28 16:28:23.000000 fiduswriter-3.9.9/fiduswriter/base/servers/tornado_django_hybrid.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.140592 fiduswriter-3.9.9/fiduswriter/base/setup_page/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      924 2020-01-13 20:06:18.000000 fiduswriter-3.9.9/fiduswriter/base/setup_page/index.html
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.124592 fiduswriter-3.9.9/fiduswriter/base/static/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.144592 fiduswriter-3.9.9/fiduswriter/base/static/css/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      402 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/add_remove_dialog.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      433 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/admin.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1594 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/alerts.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7761 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/buttons.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     5561 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/colors.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3265 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/common.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1732 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/content_menu.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2969 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/data_table.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2269 2020-12-01 12:42:15.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/dialog.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1324 2020-03-10 12:31:45.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/dialog_table.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      167 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/faq_dialog.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1629 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/figure.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      659 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/flatpage.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     8968 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/fonts.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     9648 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/forms.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1756 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/header_menu.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1470 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/inline_tools.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      681 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/loader.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1966 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/overview_menu.css
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)     2416 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/prelogin.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2027 2021-01-05 14:54:45.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/pulldown.css
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)     1867 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/reset.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      636 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/text.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1890 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/ui_dialogs.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      747 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/static/css/ui_tabs.css
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.120591 fiduswriter-3.9.9/fiduswriter/base/static/fonts/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.144592 fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    23208 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-300.woff2
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    23316 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-400.woff2
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    22820 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-700.woff2
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    22352 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-900.woff2
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     5468 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-ext-300.woff2
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     5296 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-ext-400.woff2
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     5192 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-ext-700.woff2
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     5192 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-ext-900.woff2
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     5304 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-ext-italic-400.woff2
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    24192 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-italic-400.woff2
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.144592 fiduswriter-3.9.9/fiduswriter/base/static/fonts/roboto/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    15440 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/fonts/roboto/roboto-300.woff2
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    15436 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/fonts/roboto/roboto-700.woff2
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.148592 fiduswriter-3.9.9/fiduswriter/base/static/img/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    16430 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/img/accept-change.png
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2186 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/img/default_avatar.png
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)      934 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/img/dots.png
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    11322 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/img/error.png
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     6917 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/img/favicon.png
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     4477 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/img/fidus_face.png
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     4966 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/img/free_star.png
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     7656 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/img/icon_192.png
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    21686 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/img/icon_512.png
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    45452 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/img/wait.gif
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.148592 fiduswriter-3.9.9/fiduswriter/base/static/js/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      163 2020-06-29 09:52:39.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/admin_console.mjs
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      159 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/app.mjs
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      140 2020-05-13 11:21:08.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/error_hook.mjs
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.124592 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.148592 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/404/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      423 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/404/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.148592 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/admin_console/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2200 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/admin_console/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.148592 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/app/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    12184 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/app/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.148592 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    10377 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/basic.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6107 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/content_menu.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3255 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/datatable_bulk.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    10574 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/dialog.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2145 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/faq_dialog.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      864 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4361 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/network.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     8581 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/overview_menu.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1689 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/templates.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      474 2020-02-22 23:38:55.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/user.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      586 2020-02-22 19:43:36.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/user_util.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      470 2020-02-22 19:53:57.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/worker.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     9144 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/ws.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.148592 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/copyright_dialog/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5073 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/copyright_dialog/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4485 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/copyright_dialog/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.148592 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/error_hook/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2998 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/error_hook/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.148592 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/flatpage/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1233 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/flatpage/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.148592 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/indexed_db/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6114 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/indexed_db/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.148592 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/offline/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1057 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/offline/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.152592 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/prelogin/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     3184 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/prelogin/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2271 2020-12-27 21:39:09.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/prelogin/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.152592 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/prosemirror/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1715 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/prosemirror/inline_tools.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.152592 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/setup/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      933 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/modules/setup/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.124592 fiduswriter-3.9.9/fiduswriter/base/static/js/plugins/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.152592 fiduswriter-3.9.9/fiduswriter/base/static/js/plugins/app/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       31 2020-08-19 20:40:04.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/plugins/app/init.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.152592 fiduswriter-3.9.9/fiduswriter/base/static/js/plugins/prelogin/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       33 2020-08-19 20:39:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/plugins/prelogin/init.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1262 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/static/js/sw-template.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.152592 fiduswriter-3.9.9/fiduswriter/base/static/svg/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    16277 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/static/svg/icon.svg
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.152592 fiduswriter-3.9.9/fiduswriter/base/templates/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      285 2020-05-13 11:21:08.000000 fiduswriter-3.9.9/fiduswriter/base/templates/500.html
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.152592 fiduswriter-3.9.9/fiduswriter/base/templates/admin/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1674 2020-05-13 11:21:08.000000 fiduswriter-3.9.9/fiduswriter/base/templates/admin/console.html
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      689 2020-03-15 09:48:05.000000 fiduswriter-3.9.9/fiduswriter/base/templates/admin/overview.html
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      237 2020-05-13 11:21:08.000000 fiduswriter-3.9.9/fiduswriter/base/templates/api_404.html
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3216 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/templates/app.html
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      793 2020-05-13 11:21:08.000000 fiduswriter-3.9.9/fiduswriter/base/templates/base.html
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       87 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/templates/email.html
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2186 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/templates/email_base.html
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      442 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/base/templates/manifest.json
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.152592 fiduswriter-3.9.9/fiduswriter/base/templates/socialaccount/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      121 2020-05-13 11:21:08.000000 fiduswriter-3.9.9/fiduswriter/base/templates/socialaccount/connections.html
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      108 2020-12-27 21:39:09.000000 fiduswriter-3.9.9/fiduswriter/base/templates/socialaccount/login_cancelled.html
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.152592 fiduswriter-3.9.9/fiduswriter/base/tests/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/tests/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2740 2020-03-10 12:31:45.000000 fiduswriter-3.9.9/fiduswriter/base/tests/test_admin.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2331 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/base/tests/test_manage.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2855 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/tests/test_prelogin.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      202 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/base/urls.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3669 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/views.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3871 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/base/webpack.config.template.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6531 2020-10-28 16:28:12.000000 fiduswriter-3.9.9/fiduswriter/base/ws_handler.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2294 2020-09-16 17:56:23.000000 fiduswriter-3.9.9/fiduswriter/base/ws_views.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.152592 fiduswriter-3.9.9/fiduswriter/bibliography/
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)       62 2020-02-01 14:06:35.000000 fiduswriter-3.9.9/fiduswriter/bibliography/__init__.py
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)      298 2020-02-01 14:06:35.000000 fiduswriter-3.9.9/fiduswriter/bibliography/admin.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.152592 fiduswriter-3.9.9/fiduswriter/bibliography/migrations/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2326 2020-02-01 14:06:35.000000 fiduswriter-3.9.9/fiduswriter/bibliography/migrations/0001_squashed_0011_auto_20170101_1647.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1473 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/migrations/0002_move_json_data.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2020-02-01 14:06:35.000000 fiduswriter-3.9.9/fiduswriter/bibliography/migrations/__init__.py
+-rwxrwxr-x   0 johannes  (1000) johannes  (1000)      935 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/models.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      135 2020-08-27 07:41:05.000000 fiduswriter-3.9.9/fiduswriter/bibliography/package.json
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.124592 fiduswriter-3.9.9/fiduswriter/bibliography/static/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.152592 fiduswriter-3.9.9/fiduswriter/bibliography/static/css/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2899 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/css/bibliography.css
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.152592 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      309 2020-02-01 14:06:35.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/biblatex_import_worker.mjs
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.124592 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.152592 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.156592 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/database/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6869 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/database/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1997 2020-12-11 16:49:15.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/database/server_connector.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.156592 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/export/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      829 2020-02-01 14:06:35.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/export/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.156592 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      839 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/cats.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.156592 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      922 2020-03-10 04:36:41.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/date.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4159 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/key.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2401 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/key_list.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3910 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/literal.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2328 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/literal_list.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2852 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/literal_long.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5270 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/name.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2316 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/name_list.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3689 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/range.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2350 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/range_list.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      859 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/tag_list.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2924 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/title.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1550 2020-02-01 14:06:35.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/uri.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      624 2020-02-01 14:06:35.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/verbatim.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     9812 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/index.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     9969 2020-02-23 02:16:13.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/strings.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2312 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.156592 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/import/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2595 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/import/biblatex.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2869 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/import/dialog.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       94 2020-02-01 14:06:35.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/import/index.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      471 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/import/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.156592 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/overview/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    13466 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/overview/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3051 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/overview/menu.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1100 2020-02-01 14:06:35.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/overview/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.156592 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/schema/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1547 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/schema/common.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2336 2020-02-01 14:06:35.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/schema/csl_bib.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      480 2020-02-01 14:06:35.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/schema/literal.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      725 2020-02-01 14:06:35.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/schema/literal_long.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      619 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/schema/title.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      914 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/tools.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.124592 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/plugins/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.156592 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/plugins/bibliography_overview/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       40 2020-02-01 14:06:35.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/plugins/bibliography_overview/init.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.124592 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/workers/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.156592 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/workers/importer/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2750 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/static/js/workers/importer/biblatex.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.160592 fiduswriter-3.9.9/fiduswriter/bibliography/tests/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2020-02-01 14:06:35.000000 fiduswriter-3.9.9/fiduswriter/bibliography/tests/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    11769 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/bibliography/tests/test_overview.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.160592 fiduswriter-3.9.9/fiduswriter/bibliography/tests/uploads/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      192 2020-02-01 14:06:35.000000 fiduswriter-3.9.9/fiduswriter/bibliography/tests/uploads/bibliography.bib
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)      498 2020-02-01 14:06:35.000000 fiduswriter-3.9.9/fiduswriter/bibliography/urls.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5508 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/bibliography/views.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.160592 fiduswriter-3.9.9/fiduswriter/browser_check/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/browser_check/__init__.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      481 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/browser_check/package.json
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.124592 fiduswriter-3.9.9/fiduswriter/browser_check/templates/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.160592 fiduswriter-3.9.9/fiduswriter/browser_check/templates/browser_check/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1179 2020-01-02 09:57:49.000000 fiduswriter-3.9.9/fiduswriter/browser_check/templates/browser_check/browser_not_supported.html
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.160592 fiduswriter-3.9.9/fiduswriter/browser_check/tests/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/browser_check/tests/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2065 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/browser_check/tests/test_access.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      114 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/browser_check/urls.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      175 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/browser_check/views.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3963 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/configuration.py-default
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       64 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/dev-requirements.txt
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.160592 fiduswriter-3.9.9/fiduswriter/document/
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)      190 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/__init__.py
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)     2081 2020-04-02 15:01:45.000000 fiduswriter-3.9.9/fiduswriter/document/admin.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      364 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/apps.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.160592 fiduswriter-3.9.9/fiduswriter/document/fixtures/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2777 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/fixtures/initial_documenttemplates.json
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.160592 fiduswriter-3.9.9/fiduswriter/document/helpers/
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/helpers/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1716 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/helpers/serializers.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1959 2020-03-10 12:31:45.000000 fiduswriter-3.9.9/fiduswriter/document/helpers/session_user_info.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.160592 fiduswriter-3.9.9/fiduswriter/document/management/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)        0 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/management/__init__.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.160592 fiduswriter-3.9.9/fiduswriter/document/management/commands/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1379 2020-12-26 13:18:19.000000 fiduswriter-3.9.9/fiduswriter/document/management/commands/export_schema.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.160592 fiduswriter-3.9.9/fiduswriter/document/migrations/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     5726 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/migrations/0001_squashed_20200219.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3318 2020-12-28 09:33:35.000000 fiduswriter-3.9.9/fiduswriter/document/migrations/0002_fidus_3_2.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7353 2020-12-28 09:33:35.000000 fiduswriter-3.9.9/fiduswriter/document/migrations/0003_fidus_3_3.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3807 2021-01-05 11:35:13.000000 fiduswriter-3.9.9/fiduswriter/document/migrations/0004_move_json_data.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      570 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/migrations/0005_auto_20201109_0255.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      399 2020-12-27 21:39:09.000000 fiduswriter-3.9.9/fiduswriter/document/migrations/0006_auto_20201209_1610.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6783 2020-12-28 09:33:35.000000 fiduswriter-3.9.9/fiduswriter/document/migrations/0007_fix_fidus_3_3.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/migrations/__init__.py
+-rwxrwxr-x   0 johannes  (1000) johannes  (1000)    11461 2020-12-27 21:39:09.000000 fiduswriter-3.9.9/fiduswriter/document/models.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1079 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/package.json
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2091 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/prosemirror.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      444 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/signals.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.128592 fiduswriter-3.9.9/fiduswriter/document/static/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.164592 fiduswriter-3.9.9/fiduswriter/document/static/css/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      127 2020-01-28 23:50:30.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/access_rights_dialog.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      290 2020-01-28 23:50:30.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/carets.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1320 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/chat.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      748 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/citation_dialog.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      309 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/contributors.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3982 2020-12-31 17:57:32.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/document.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      134 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/document_overview.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     3598 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/document_template_designer.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      557 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/document_template_designer_admin.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      722 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/dot_menu.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    22087 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/editor.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1820 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/footnotes.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    10046 2020-12-31 17:57:32.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/margin_boxes.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3379 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/merge.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      105 2020-01-28 23:50:30.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/review.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      164 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/table.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      574 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/tags.css
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1039 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/css/tracking.css
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.124592 fiduswriter-3.9.9/fiduswriter/document/static/fonts/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.168592 fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)   191484 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/Cardo-Bold.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)   153060 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/Cardo-Italic.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)   223616 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/Cardo-Regular.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    44512 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/CrimsonText-Bold.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    39280 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/CrimsonText-BoldItalic.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    55548 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/CrimsonText-Italic.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    95500 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/CrimsonText-Roman.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    26424 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/Lobster-1.4.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    41084 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/NoticiaText-Bold.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    37520 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/NoticiaText-BoldItalic.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    37404 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/NoticiaText-Italic.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    41604 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/NoticiaText-Regular.woff
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)    91484 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/OpenSans-Bold.woff
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)    94044 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/OpenSans-Regular.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    63256 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/SourceSansPro-Bold.woff
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.168592 fiduswriter-3.9.9/fiduswriter/document/static/js/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      365 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/adjust_doc_to_template_worker.mjs
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      221 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/document_template_admin.mjs
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      157 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/maintenance.mjs
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.128592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.168592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/citations/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1308 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/citations/citeproc_sys.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5923 2020-06-11 04:48:02.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/citations/format.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1720 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/citations/render.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.168592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4921 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/admin.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    23684 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/designer.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    10889 2020-10-23 10:37:35.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/document_style_dialog.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    12813 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/export_template_dialog.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1670 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/extract_template.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     8636 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/fix_doc.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      246 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6503 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/schema.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    31344 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/templates.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1931 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/tools.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.168592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.168592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/access_rights/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    12207 2020-12-27 21:39:09.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/access_rights/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3982 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/access_rights/templates.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      954 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/invite.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.168592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/overview/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    14382 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/overview/actions.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    13271 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/overview/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5531 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/overview/menu.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      533 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/overview/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.168592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/revisions/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5647 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/revisions/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1902 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/revisions/templates.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1743 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/tools.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.168592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.168592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/citations/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     8476 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/citations/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.124592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.172592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/copy/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       76 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/copy/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      959 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/copy/schema.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6007 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/copy/serializers.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.172592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/paste/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1915 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/paste/fidus_writer.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2378 2020-06-11 08:33:17.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/paste/general.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      892 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/paste/google_docs.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2239 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/paste/html.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       66 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/paste/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1083 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/paste/libreoffice_writer.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3075 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/paste/microsoft_word.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2774 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/paste/text.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.172592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4742 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/chat.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2002 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/colors.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    18284 2020-12-28 01:14:38.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/doc.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2911 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.172592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2653 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/changeset.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    35635 2020-12-27 21:39:09.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/editor.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4923 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/footnotes.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    10823 2020-12-27 21:39:09.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    10424 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/recreate_transform.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3491 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/schema.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.172592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/state_plugins/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6136 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/state_plugins/action.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1673 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/state_plugins/clipboard.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    22790 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/state_plugins/diff.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       90 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/state_plugins/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7210 2020-12-27 21:39:09.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/tools.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      473 2019-11-23 15:40:08.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.172592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/comments/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      950 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/comments/comment.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.176592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/comments/editors/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1366 2020-08-24 18:06:36.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/comments/editors/answer.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7798 2020-12-31 17:58:21.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/comments/editors/comment.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      146 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/comments/editors/index.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      448 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/comments/editors/notify.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1336 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/comments/editors/schema.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      295 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/comments/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    12782 2020-12-31 17:57:32.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/comments/interactions.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    12682 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/comments/store.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.176592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/databases/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5295 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/databases/bibliography.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7253 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/databases/images.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2508 2020-12-27 21:39:09.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/databases/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.176592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    12360 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/citation.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     3686 2019-10-17 15:05:38.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/contributor.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    13470 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/figure.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      396 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/index.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1675 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/language.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    11386 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/link.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3866 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/math.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2081 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/ordered_list.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1018 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/revision.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7717 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/table.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    15936 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.176592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/document_template/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    11414 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/document_template/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.176592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/footnotes/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7174 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/footnotes/editor.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      363 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/footnotes/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7518 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/footnotes/layout.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.176592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/footnotes/state_plugins/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      925 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/footnotes/state_plugins/access_rights.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       61 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/footnotes/state_plugins/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    21613 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2614 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/keymap.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.176592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/marginboxes/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    27512 2020-12-31 17:57:32.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/marginboxes/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    21089 2020-12-31 17:57:32.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/marginboxes/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.176592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.176592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/figure/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       40 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/figure/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1224 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/figure/model.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.176592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/headerbar/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       76 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/headerbar/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    24167 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/headerbar/model.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    13091 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/headerbar/view.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.176592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/image/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       38 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/image/index.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1089 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/image/model.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      396 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.176592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/navigator/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       44 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/navigator/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      565 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/navigator/model.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.180592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/ordered_list/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       45 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/ordered_list/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      511 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/ordered_list/model.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.180592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/selection/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       84 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/selection/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4392 2020-11-26 19:52:06.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/selection/model.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5314 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/selection/view.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.180592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/table/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       38 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/table/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    13680 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/table/model.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.180592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/toolbar/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       72 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/toolbar/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    26842 2020-11-26 19:52:06.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/toolbar/model.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    11700 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/toolbar/view.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.180592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/navigator/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7932 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/navigator/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.184592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1277 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/access_rights.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3499 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/citation_render.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2177 2019-11-02 10:42:57.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/clipboard.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4556 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/collab_carets.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     8234 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/comments.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5067 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/contributor_input.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     9328 2020-11-26 19:52:06.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/document_template.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3513 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/figure.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7596 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/footnote_markers.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      321 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/headerbar.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1952 2020-11-26 19:52:06.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2054 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/jump_hidden_nodes.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    19870 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/links.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      395 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/marginboxes.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2584 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/ordered_list_menu.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4274 2020-11-26 19:52:06.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/placeholders.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7371 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/search.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      334 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/selection_menu.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7176 2020-11-26 19:06:33.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/settings.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3819 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/table.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     8460 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/tag_input.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5624 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/toc_render.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      316 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/toolbar.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.184592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/track/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3562 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/track/find_selected_changes.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2822 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/track/helpers.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      152 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/track/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4085 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/track/plugin.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.184592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/tools/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      146 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/tools/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.184592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/tools/key_bindings/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      604 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/tools/key_bindings/index.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2815 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/tools/key_bindings/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.184592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/tools/search_replace/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    10353 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/tools/search_replace/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      523 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/tools/search_replace/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.184592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/tools/word_count/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2388 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/tools/word_count/index.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1211 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/tools/word_count/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.184592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2868 2020-08-24 18:06:36.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/accept.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2979 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/accept_all.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2080 2020-11-18 16:58:19.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/accept_all_no_insertions.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    17917 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/amend_transaction.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2880 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/delete.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      269 2020-01-02 09:57:49.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2849 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/mod.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3453 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/reject.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3655 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/reject_all.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.128592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.184592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6803 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/citations.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7940 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/footnotes.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2696 2020-12-11 17:39:01.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/images.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3164 2020-12-11 16:35:33.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    11586 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/lists.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3149 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/math.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4634 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/metadata.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4136 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/rels.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     9428 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/render.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    30036 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/richtext.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     3745 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/tables.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.188592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/epub/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7009 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/epub/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7134 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/epub/templates.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5042 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/epub/tools.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.188592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/html/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2972 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/html/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1297 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/html/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.188592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/jats/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     5078 2019-11-05 22:04:35.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/jats/citations.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    29148 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/jats/convert.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2259 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/jats/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1208 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/jats/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.188592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/latex/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    31491 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/latex/convert.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      834 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/latex/escape_latex.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2077 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/latex/index.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      618 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/latex/readme.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.188592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/native/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1237 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/native/copy.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      792 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/native/file.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      111 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/native/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2145 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/native/revision.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3023 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/native/shrink.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1040 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/native/zip.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.188592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4001 2021-01-05 14:54:45.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/citations.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4957 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/footnotes.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3188 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/images.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2745 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2469 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/math.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5036 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/metadata.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6530 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/render.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    19151 2021-01-05 14:54:45.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/richtext.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    16047 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/styles.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.188592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/print/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4965 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/print/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.192592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/tools/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3771 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/tools/doc_content.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     8587 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/tools/dom_export.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      228 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/tools/file.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1029 2020-12-11 16:30:25.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/tools/html.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2245 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/tools/json.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3055 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/tools/xml_zip.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3014 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/tools/zip.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.192592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/importer/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     8181 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/importer/file.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2184 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/importer/get_images.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5481 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/importer/native.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      777 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/importer/update.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.192592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/maintenance/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     9971 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/maintenance/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.192592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.192592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1780 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/annotate.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1777 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/base.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1343 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/citation.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      710 2020-12-26 13:17:58.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/equation.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4740 2020-12-27 21:39:09.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/figure.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1028 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/heading.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      715 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1955 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/list.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1937 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/reference.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2531 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/table.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4315 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/track.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2387 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/const.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    29380 2020-12-27 21:39:09.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/convert.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.192592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/document/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3136 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/document/content.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1981 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/document/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     8027 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/document/structure.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      846 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/export.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2539 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/footnotes.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      997 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/footnotes_convert.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5152 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/i18n.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      208 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/index.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1902 2019-09-29 23:49:15.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/mini_json.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.192592 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/test_caret/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      492 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/modules/test_caret/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.128592 fiduswriter-3.9.9/fiduswriter/document/static/js/plugins/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.192592 fiduswriter-3.9.9/fiduswriter/document/static/js/plugins/citation_dialog/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       43 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/plugins/citation_dialog/init.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.192592 fiduswriter-3.9.9/fiduswriter/document/static/js/plugins/documents_overview/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       45 2020-05-13 11:21:08.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/plugins/documents_overview/init.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.192592 fiduswriter-3.9.9/fiduswriter/document/static/js/plugins/editor/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       34 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/plugins/editor/init.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.192592 fiduswriter-3.9.9/fiduswriter/document/static/js/plugins/schema_export/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       41 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/plugins/schema_export/init.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      206 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/schema_export.mjs
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      114 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/test_caret.mjs
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.128592 fiduswriter-3.9.9/fiduswriter/document/static/js/workers/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.196592 fiduswriter-3.9.9/fiduswriter/document/static/js/workers/document_template/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1198 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/document/static/js/workers/document_template/adjust_doc.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.196592 fiduswriter-3.9.9/fiduswriter/document/static/ogg/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    18048 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/static/ogg/chat_notification.ogg
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.128592 fiduswriter-3.9.9/fiduswriter/document/templates/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.128592 fiduswriter-3.9.9/fiduswriter/document/templates/admin/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.196592 fiduswriter-3.9.9/fiduswriter/document/templates/admin/document/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.196592 fiduswriter-3.9.9/fiduswriter/document/templates/admin/document/document/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      475 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/templates/admin/document/document/change_list_object_tools.html
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.196592 fiduswriter-3.9.9/fiduswriter/document/templates/admin/document/documenttemplate/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      635 2020-05-13 11:21:08.000000 fiduswriter-3.9.9/fiduswriter/document/templates/admin/document/documenttemplate/change_form.html
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1286 2020-05-13 11:21:08.000000 fiduswriter-3.9.9/fiduswriter/document/templates/admin/document/maintenance.html
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.196592 fiduswriter-3.9.9/fiduswriter/document/tests/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/tests/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2915 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/document/tests/editor_helper.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    17904 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/tests/test_admin.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    43519 2020-12-31 17:57:32.000000 fiduswriter-3.9.9/fiduswriter/document/tests/test_collaboration.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    41137 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/tests/test_editor.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    24540 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/tests/test_export.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6016 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/tests/test_message_exchange.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    30249 2020-12-01 12:42:15.000000 fiduswriter-3.9.9/fiduswriter/document/tests/test_offline.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.196592 fiduswriter-3.9.9/fiduswriter/document/tests/uploads/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    45965 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/tests/uploads/image.png
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)     2542 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/document/urls.py
+-rwxrwxr-x   0 johannes  (1000) johannes  (1000)    38974 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/views.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    28963 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/document/ws_views.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.196592 fiduswriter-3.9.9/fiduswriter/feedback/
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)       50 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/feedback/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      168 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/feedback/admin.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.196592 fiduswriter-3.9.9/fiduswriter/feedback/migrations/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      713 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/feedback/migrations/0001_initial.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/feedback/migrations/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1043 2020-03-16 20:47:16.000000 fiduswriter-3.9.9/fiduswriter/feedback/models.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.128592 fiduswriter-3.9.9/fiduswriter/feedback/static/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.128592 fiduswriter-3.9.9/fiduswriter/feedback/static/css/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.196592 fiduswriter-3.9.9/fiduswriter/feedback/static/css/feedback/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2323 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/feedback/static/css/feedback/feedback.css
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.128592 fiduswriter-3.9.9/fiduswriter/feedback/static/js/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.128592 fiduswriter-3.9.9/fiduswriter/feedback/static/js/modules/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.196592 fiduswriter-3.9.9/fiduswriter/feedback/static/js/modules/feedback/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3733 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/feedback/static/js/modules/feedback/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.196592 fiduswriter-3.9.9/fiduswriter/feedback/tests/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-11-05 22:04:35.000000 fiduswriter-3.9.9/fiduswriter/feedback/tests/__init__.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3191 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/feedback/tests/test_feedback.py
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)      129 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/feedback/urls.py
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)      557 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/feedback/views.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.196592 fiduswriter-3.9.9/fiduswriter/fixturemedia/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       51 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/fixturemedia/__init__.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.196592 fiduswriter-3.9.9/fiduswriter/fixturemedia/management/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/fixturemedia/management/__init__.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.196592 fiduswriter-3.9.9/fiduswriter/fixturemedia/management/commands/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/fixturemedia/management/commands/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     3142 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/fixturemedia/management/commands/dumpdata.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3183 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/fixturemedia/management/commands/loaddata.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.196592 fiduswriter-3.9.9/fiduswriter/locale/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/locale/bg/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.196592 fiduswriter-3.9.9/fiduswriter/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     7727 2021-01-05 14:54:54.000000 fiduswriter-3.9.9/fiduswriter/locale/bg/LC_MESSAGES/django.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    12634 2020-12-31 18:00:45.000000 fiduswriter-3.9.9/fiduswriter/locale/bg/LC_MESSAGES/django.po
+-rw-r--r--   0 johannes  (1000) johannes  (1000)   104753 2021-01-05 14:54:54.000000 fiduswriter-3.9.9/fiduswriter/locale/bg/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)   197856 2020-12-31 18:21:32.000000 fiduswriter-3.9.9/fiduswriter/locale/bg/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      609 2020-01-02 09:57:49.000000 fiduswriter-3.9.9/fiduswriter/locale/copyright.txt
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/locale/de/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.200592 fiduswriter-3.9.9/fiduswriter/locale/de/LC_MESSAGES/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     6213 2021-01-05 14:54:54.000000 fiduswriter-3.9.9/fiduswriter/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    10881 2020-12-31 18:00:45.000000 fiduswriter-3.9.9/fiduswriter/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    83975 2021-01-05 14:54:54.000000 fiduswriter-3.9.9/fiduswriter/locale/de/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)   174813 2020-12-31 18:21:32.000000 fiduswriter-3.9.9/fiduswriter/locale/de/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/locale/es/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.200592 fiduswriter-3.9.9/fiduswriter/locale/es/LC_MESSAGES/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     6035 2021-01-05 14:54:54.000000 fiduswriter-3.9.9/fiduswriter/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    10596 2020-12-31 18:00:45.000000 fiduswriter-3.9.9/fiduswriter/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    83451 2021-01-05 14:54:54.000000 fiduswriter-3.9.9/fiduswriter/locale/es/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)   174281 2020-12-31 18:21:32.000000 fiduswriter-3.9.9/fiduswriter/locale/es/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/locale/fr/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.200592 fiduswriter-3.9.9/fiduswriter/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     7632 2021-01-05 14:54:54.000000 fiduswriter-3.9.9/fiduswriter/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    11173 2021-01-05 11:36:58.000000 fiduswriter-3.9.9/fiduswriter/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    83496 2021-01-05 14:54:54.000000 fiduswriter-3.9.9/fiduswriter/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)   176456 2021-01-05 11:36:58.000000 fiduswriter-3.9.9/fiduswriter/locale/fr/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/locale/it/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.200592 fiduswriter-3.9.9/fiduswriter/locale/it/LC_MESSAGES/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     6125 2021-01-05 14:54:54.000000 fiduswriter-3.9.9/fiduswriter/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    10730 2020-12-31 18:00:45.000000 fiduswriter-3.9.9/fiduswriter/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    81067 2021-01-05 14:54:54.000000 fiduswriter-3.9.9/fiduswriter/locale/it/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)   173513 2020-12-31 18:21:32.000000 fiduswriter-3.9.9/fiduswriter/locale/it/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/locale/pt_BR/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.200592 fiduswriter-3.9.9/fiduswriter/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     5940 2021-01-05 14:54:54.000000 fiduswriter-3.9.9/fiduswriter/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    10434 2020-12-31 18:00:45.000000 fiduswriter-3.9.9/fiduswriter/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    82052 2021-01-05 14:54:54.000000 fiduswriter-3.9.9/fiduswriter/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)   173060 2020-12-31 18:21:32.000000 fiduswriter-3.9.9/fiduswriter/locale/pt_BR/LC_MESSAGES/djangojs.po
+-rwxrwxr-x   0 johannes  (1000) johannes  (1000)     3085 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/manage.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.200592 fiduswriter-3.9.9/fiduswriter/menu/
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)       58 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/menu/__init__.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/menu/static/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/menu/static/js/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/menu/static/js/modules/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.200592 fiduswriter-3.9.9/fiduswriter/menu/static/js/modules/menu/
+-rwxrwxr-x   0 johannes  (1000) johannes  (1000)     2822 2021-01-05 12:13:06.000000 fiduswriter-3.9.9/fiduswriter/menu/static/js/modules/menu/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      472 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/menu/static/js/modules/menu/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/menu/static/js/plugins/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.200592 fiduswriter-3.9.9/fiduswriter/menu/static/js/plugins/menu/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       37 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/menu/static/js/plugins/menu/init.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       19 2020-01-02 09:57:49.000000 fiduswriter-3.9.9/fiduswriter/mysql-requirements.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       16 2019-10-30 06:04:12.000000 fiduswriter-3.9.9/fiduswriter/postgresql-requirements.txt
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      299 2021-01-05 13:17:05.000000 fiduswriter-3.9.9/fiduswriter/requirements.txt
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.204592 fiduswriter-3.9.9/fiduswriter/style/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       73 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      565 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/admin.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.204592 fiduswriter-3.9.9/fiduswriter/style/fixtures/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    35063 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/initial_styles.json
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.204592 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/export-template-files/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    10707 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/export-template-files/Classic.docx
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     9852 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/export-template-files/Free.odt
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.208593 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)   191484 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/Cardo-Bold.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)   153060 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/Cardo-Italic.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)   223616 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/Cardo-Regular.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    44512 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/CrimsonText-Bold.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    39280 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/CrimsonText-BoldItalic.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    55548 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/CrimsonText-Italic.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    95500 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/CrimsonText-Roman.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    26424 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/Lobster-1.4.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    37520 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-BoldItalic.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    37520 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-BoldItalic_KMSnKTE.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    37520 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-BoldItalic_Xg38HXg.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    41084 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Bold_2.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    41084 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Bold_2_77vhC50.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    41084 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Bold_2_qiGg4Ow.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    37404 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Italic.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    37404 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Italic_3AoQkPt.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    37404 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Italic_ai8IvB3.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    41604 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Regular.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    41604 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Regular_eNSdC3U.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    41604 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Regular_zGx3t7x.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    91484 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/OpenSans-Bold.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    94044 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/OpenSans-Regular.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    63256 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/SourceSansPro-Bold.woff
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    63256 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/SourceSansPro-Bold_ySHS5jh.woff
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.208593 fiduswriter-3.9.9/fiduswriter/style/migrations/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     3043 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/style/migrations/0001_squashed_20200219.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/migrations/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2523 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/models.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      571 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/style/urls.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     4875 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/style/views.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      697 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/stylelint.config.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       38 2019-10-30 15:40:18.000000 fiduswriter-3.9.9/fiduswriter/test-requirements.txt
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.208593 fiduswriter-3.9.9/fiduswriter/testing/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       38 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/testing/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1857 2020-05-13 11:21:08.000000 fiduswriter-3.9.9/fiduswriter/testing/eslint_import_resolver.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3524 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/testing/selenium_helper.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6671 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/testing/testcases.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.208593 fiduswriter-3.9.9/fiduswriter/user/
+-rwxr-xr-x   0 johannes  (1000) johannes  (1000)       97 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/user/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1190 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/user/adapter.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      287 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/user/admin.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      118 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/user/apps.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      506 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/user/forms.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.208593 fiduswriter-3.9.9/fiduswriter/user/migrations/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1605 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/user/migrations/0001_squashed_0003_auto_20151226_1110.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      661 2021-01-05 13:17:05.000000 fiduswriter-3.9.9/fiduswriter/user/migrations/0002_loginas.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/user/migrations/__init__.py
+-rwxrwxr-x   0 johannes  (1000) johannes  (1000)     1691 2021-01-05 13:17:05.000000 fiduswriter-3.9.9/fiduswriter/user/models.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3202 2020-12-27 21:39:09.000000 fiduswriter-3.9.9/fiduswriter/user/signals.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/user/static/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.208593 fiduswriter-3.9.9/fiduswriter/user/static/css/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      973 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/user/static/css/show_profile.css
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/user/static/js/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.208593 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/contacts/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4153 2020-12-27 21:39:09.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/contacts/add_dialog.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1427 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/contacts/delete_dialog.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3780 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/contacts/index.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1261 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/contacts/menu.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1226 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/contacts/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.208593 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/email_confirm/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4355 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/email_confirm/index.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2458 2019-11-16 17:50:16.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/email_confirm/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.208593 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/login/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7144 2020-12-27 21:39:09.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/login/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.212592 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/password_reset/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5163 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/password_reset/change_password.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      115 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/password_reset/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4061 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/password_reset/request_email.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.212592 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/profile/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1990 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/profile/delete_user.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    12498 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/profile/dialogs.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4182 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/profile/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    10161 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/profile/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.212592 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/signup/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     8280 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/modules/signup/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/user/static/js/plugins/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.212592 fiduswriter-3.9.9/fiduswriter/user/static/js/plugins/confirm_account/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       43 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/plugins/confirm_account/init.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.212592 fiduswriter-3.9.9/fiduswriter/user/static/js/plugins/login/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       33 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/user/static/js/plugins/login/init.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/user/templates/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/user/templates/account/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.212592 fiduswriter-3.9.9/fiduswriter/user/templates/account/email/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      719 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/user/templates/account/email/email_confirmation_message.html
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       62 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/user/templates/account/email/email_confirmation_signup_message.html
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      875 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/user/templates/account/email/password_reset_key_message.html
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.212592 fiduswriter-3.9.9/fiduswriter/user/tests/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/user/tests/__init__.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5074 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/user/tests/test_contacts.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)    13106 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/user/tests/test_profile.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1652 2020-05-13 11:21:08.000000 fiduswriter-3.9.9/fiduswriter/user/urls.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1969 2020-03-10 12:31:45.000000 fiduswriter-3.9.9/fiduswriter/user/util.py
+-rwxrwxr-x   0 johannes  (1000) johannes  (1000)    12900 2020-12-27 21:39:09.000000 fiduswriter-3.9.9/fiduswriter/user/views.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.212592 fiduswriter-3.9.9/fiduswriter/user_template_manager/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      118 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/user_template_manager/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      357 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/user_template_manager/apps.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/user_template_manager/static/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.212592 fiduswriter-3.9.9/fiduswriter/user_template_manager/static/css/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      234 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/user_template_manager/static/css/errorlist.css
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      308 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/user_template_manager/static/css/user_template_manager.css
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/modules/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.212592 fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/modules/user_template_manager/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2797 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/modules/user_template_manager/actions.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4244 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/modules/user_template_manager/editor.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       92 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/modules/user_template_manager/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1706 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/modules/user_template_manager/menu.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7307 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/modules/user_template_manager/overview.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.132592 fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/plugins/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.212592 fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/plugins/app/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      875 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/plugins/app/user_template_manager.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.212592 fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/plugins/menu/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      407 2020-01-02 09:57:49.000000 fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/plugins/menu/user_template_manager.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      391 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/user_template_manager/urls.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     4321 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/user_template_manager/views.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.216592 fiduswriter-3.9.9/fiduswriter/usermedia/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       86 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/usermedia/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      521 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/usermedia/admin.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.216592 fiduswriter-3.9.9/fiduswriter/usermedia/migrations/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     4369 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/usermedia/migrations/0001_squashed_0009_auto_20170908_0953.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      584 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/usermedia/migrations/0002_auto_20200205_2140.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      669 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/usermedia/migrations/0003_auto_20200205_2230.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      706 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/usermedia/migrations/0004_auto_20200205_2347.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3264 2021-01-05 11:35:13.000000 fiduswriter-3.9.9/fiduswriter/usermedia/migrations/0005_move_json_data.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      633 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/usermedia/migrations/0006_auto_20200820_0510.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/usermedia/migrations/__init__.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     7272 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/usermedia/models.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)      289 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/usermedia/package.json
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.136592 fiduswriter-3.9.9/fiduswriter/usermedia/static/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.216592 fiduswriter-3.9.9/fiduswriter/usermedia/static/css/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      195 2020-03-03 14:35:50.000000 fiduswriter-3.9.9/fiduswriter/usermedia/static/css/dialog_usermedia.css
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.136592 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.136592 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.216592 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1899 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/database.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.216592 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/edit_dialog/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6333 2020-12-24 00:27:12.000000 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/edit_dialog/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5431 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/edit_dialog/model.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     1925 2020-06-11 02:38:24.000000 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/edit_dialog/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.216592 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/overview/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     3467 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/overview/categories.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     9680 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/overview/index.js
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     2154 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/overview/menu.js
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     1057 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/overview/templates.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.216592 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/selection_dialog/
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6145 2020-11-26 14:54:59.000000 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/selection_dialog/index.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.136592 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/plugins/
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.216592 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/plugins/images_overview/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       33 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/usermedia/static/js/plugins/images_overview/init.js
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.216592 fiduswriter-3.9.9/fiduswriter/usermedia/tests/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        0 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/usermedia/tests/__init__.py
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     7396 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/usermedia/tests/test_overview.py
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.216592 fiduswriter-3.9.9/fiduswriter/usermedia/tests/uploads/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    45965 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/usermedia/tests/uploads/image.png
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      361 2019-09-23 11:40:46.000000 fiduswriter-3.9.9/fiduswriter/usermedia/urls.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     5869 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/fiduswriter/usermedia/views.py
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)        6 2021-01-05 14:54:45.000000 fiduswriter-3.9.9/fiduswriter/version.txt
+drwxrwxr-x   0 johannes  (1000) johannes  (1000)        0 2021-01-05 14:54:58.136592 fiduswriter-3.9.9/fiduswriter.egg-info/
+-rw-r--r--   0 johannes  (1000) johannes  (1000)     2759 2021-01-05 14:54:54.000000 fiduswriter-3.9.9/fiduswriter.egg-info/PKG-INFO
+-rw-r--r--   0 johannes  (1000) johannes  (1000)    37827 2021-01-05 14:54:58.000000 fiduswriter-3.9.9/fiduswriter.egg-info/SOURCES.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)        1 2021-01-05 14:54:54.000000 fiduswriter-3.9.9/fiduswriter.egg-info/dependency_links.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       58 2021-01-05 14:54:54.000000 fiduswriter-3.9.9/fiduswriter.egg-info/entry_points.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)      573 2021-01-05 14:54:54.000000 fiduswriter-3.9.9/fiduswriter.egg-info/requires.txt
+-rw-r--r--   0 johannes  (1000) johannes  (1000)       12 2021-01-05 14:54:54.000000 fiduswriter-3.9.9/fiduswriter.egg-info/top_level.txt
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)       38 2021-01-05 14:54:58.216592 fiduswriter-3.9.9/setup.cfg
+-rw-rw-r--   0 johannes  (1000) johannes  (1000)     6911 2020-12-28 00:54:47.000000 fiduswriter-3.9.9/setup.py
```

### Comparing `fiduswriter-3.9.8/MANIFEST.in` & `fiduswriter-3.9.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/PKG-INFO` & `fiduswriter-3.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiduswriter
-Version: 3.9.8
+Version: 3.9.9
 Summary: A semantic wordprocessor for academic purposes
 Home-page: https://www.fiduswriter.org
 Author: Lund Info AB
 Author-email: mail@lundinfo.com
 License: AGPL
 Description: Fidus Writer
         ============
```

### Comparing `fiduswriter-3.9.8/README.md` & `fiduswriter-3.9.9/README.md`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/.eslintrc.js` & `fiduswriter-3.9.9/fiduswriter/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/__init__.py` & `fiduswriter-3.9.9/fiduswriter/base/__init__.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/default_settings.py` & `fiduswriter-3.9.9/fiduswriter/base/default_settings.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/django_handler_mixin.py` & `fiduswriter-3.9.9/fiduswriter/base/django_handler_mixin.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/fixtures/initial_terms.json` & `fiduswriter-3.9.9/fiduswriter/base/fixtures/initial_terms.json`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/handlers/__init__.py` & `fiduswriter-3.9.9/fiduswriter/base/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/management/commands/bundle_mathlive.py` & `fiduswriter-3.9.9/fiduswriter/base/management/commands/bundle_mathlive.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/management/commands/initadmin.py` & `fiduswriter-3.9.9/fiduswriter/base/management/commands/initadmin.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/management/commands/jest.py` & `fiduswriter-3.9.9/fiduswriter/base/management/commands/jest.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/management/commands/lint_css.py` & `fiduswriter-3.9.9/fiduswriter/base/management/commands/lint_css.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/management/commands/lint_js.py` & `fiduswriter-3.9.9/fiduswriter/base/management/commands/lint_js.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/management/commands/lint_py.py` & `fiduswriter-3.9.9/fiduswriter/base/management/commands/lint_py.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/management/commands/makemessages.py` & `fiduswriter-3.9.9/fiduswriter/base/management/commands/makemessages.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/management/commands/runserver.py` & `fiduswriter-3.9.9/fiduswriter/base/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/management/commands/setup.py` & `fiduswriter-3.9.9/fiduswriter/base/management/commands/setup.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/management/commands/startproject.py` & `fiduswriter-3.9.9/fiduswriter/base/management/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/package.json` & `fiduswriter-3.9.9/fiduswriter/base/package.json`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/root_urls.py` & `fiduswriter-3.9.9/fiduswriter/base/root_urls.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/servers/tornado_django_hybrid.py` & `fiduswriter-3.9.9/fiduswriter/base/servers/tornado_django_hybrid.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/setup_page/index.html` & `fiduswriter-3.9.9/fiduswriter/base/setup_page/index.html`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/alerts.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/alerts.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/buttons.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/buttons.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/colors.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/colors.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/common.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/common.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/content_menu.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/content_menu.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/data_table.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/data_table.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/dialog.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/dialog.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/dialog_table.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/dialog_table.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/figure.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/figure.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/flatpage.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/flatpage.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/fonts.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/fonts.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/forms.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/forms.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/header_menu.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/header_menu.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/inline_tools.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/inline_tools.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/loader.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/loader.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/overview_menu.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/overview_menu.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/prelogin.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/prelogin.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/pulldown.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/pulldown.css`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,23 @@
 .fw-pulldown.fw-right {
     right: 0;
 }
 
 /* sub menu */
 .fw-pulldown .fw-pulldown {
     top: 0;
-    right: 100%;
+    left: 100%;
     margin-top: 0;
 }
 
+.marginbox-options.fw-pulldown .fw-pulldown {
+    right: 100%;
+    left: auto;
+}
+
 .fw-pulldown.fw-right .fw-pulldown {
     left: auto;
     right: 100%;
 }
 
 .fw-pulldown > ul {
     position: relative;
```

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/reset.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/reset.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/text.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/text.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/ui_dialogs.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/ui_dialogs.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/css/ui_tabs.css` & `fiduswriter-3.9.9/fiduswriter/base/static/css/ui_tabs.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-300.woff2` & `fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-300.woff2`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-400.woff2` & `fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-400.woff2`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-700.woff2` & `fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-700.woff2`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-900.woff2` & `fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-900.woff2`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-ext-300.woff2` & `fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-ext-300.woff2`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-ext-400.woff2` & `fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-ext-400.woff2`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-ext-700.woff2` & `fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-ext-700.woff2`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-ext-900.woff2` & `fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-ext-900.woff2`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-ext-italic-400.woff2` & `fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-ext-italic-400.woff2`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/fonts/lato/lato-italic-400.woff2` & `fiduswriter-3.9.9/fiduswriter/base/static/fonts/lato/lato-italic-400.woff2`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/fonts/roboto/roboto-300.woff2` & `fiduswriter-3.9.9/fiduswriter/base/static/fonts/roboto/roboto-300.woff2`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/fonts/roboto/roboto-700.woff2` & `fiduswriter-3.9.9/fiduswriter/base/static/fonts/roboto/roboto-700.woff2`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/img/accept-change.png` & `fiduswriter-3.9.9/fiduswriter/base/static/img/accept-change.png`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/img/default_avatar.png` & `fiduswriter-3.9.9/fiduswriter/base/static/img/default_avatar.png`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/img/dots.png` & `fiduswriter-3.9.9/fiduswriter/base/static/img/dots.png`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/img/error.png` & `fiduswriter-3.9.9/fiduswriter/base/static/img/error.png`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/img/favicon.png` & `fiduswriter-3.9.9/fiduswriter/base/static/img/favicon.png`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/img/fidus_face.png` & `fiduswriter-3.9.9/fiduswriter/base/static/img/fidus_face.png`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/img/free_star.png` & `fiduswriter-3.9.9/fiduswriter/base/static/img/free_star.png`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/img/icon_192.png` & `fiduswriter-3.9.9/fiduswriter/base/static/img/icon_192.png`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/img/icon_512.png` & `fiduswriter-3.9.9/fiduswriter/base/static/img/icon_512.png`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/img/wait.gif` & `fiduswriter-3.9.9/fiduswriter/base/static/img/wait.gif`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/admin_console/index.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/admin_console/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/app/index.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/app/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/basic.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/basic.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/content_menu.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/content_menu.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/datatable_bulk.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/datatable_bulk.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/dialog.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/dialog.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/faq_dialog.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/faq_dialog.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/index.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/network.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/network.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/overview_menu.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/overview_menu.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/templates.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/user_util.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/user_util.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/common/ws.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/common/ws.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/copyright_dialog/index.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/copyright_dialog/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/copyright_dialog/templates.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/copyright_dialog/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/error_hook/index.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/error_hook/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/flatpage/index.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/flatpage/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/indexed_db/index.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/indexed_db/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/offline/index.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/offline/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/prelogin/index.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/prelogin/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/prelogin/templates.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/prelogin/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/prosemirror/inline_tools.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/prosemirror/inline_tools.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/modules/setup/index.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/modules/setup/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/js/sw-template.js` & `fiduswriter-3.9.9/fiduswriter/base/static/js/sw-template.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/static/svg/icon.svg` & `fiduswriter-3.9.9/fiduswriter/base/static/svg/icon.svg`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/templates/admin/console.html` & `fiduswriter-3.9.9/fiduswriter/base/templates/admin/console.html`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/templates/admin/overview.html` & `fiduswriter-3.9.9/fiduswriter/base/templates/admin/overview.html`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/templates/app.html` & `fiduswriter-3.9.9/fiduswriter/base/templates/app.html`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/templates/base.html` & `fiduswriter-3.9.9/fiduswriter/base/templates/base.html`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/templates/email_base.html` & `fiduswriter-3.9.9/fiduswriter/base/templates/email_base.html`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/tests/test_admin.py` & `fiduswriter-3.9.9/fiduswriter/base/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/tests/test_manage.py` & `fiduswriter-3.9.9/fiduswriter/base/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/tests/test_prelogin.py` & `fiduswriter-3.9.9/fiduswriter/base/tests/test_prelogin.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/views.py` & `fiduswriter-3.9.9/fiduswriter/base/views.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/webpack.config.template.js` & `fiduswriter-3.9.9/fiduswriter/base/webpack.config.template.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/ws_handler.py` & `fiduswriter-3.9.9/fiduswriter/base/ws_handler.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/base/ws_views.py` & `fiduswriter-3.9.9/fiduswriter/base/ws_views.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/migrations/0001_squashed_0011_auto_20170101_1647.py` & `fiduswriter-3.9.9/fiduswriter/bibliography/migrations/0001_squashed_0011_auto_20170101_1647.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/migrations/0002_move_json_data.py` & `fiduswriter-3.9.9/fiduswriter/bibliography/migrations/0002_move_json_data.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/models.py` & `fiduswriter-3.9.9/fiduswriter/bibliography/models.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/css/bibliography.css` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/css/bibliography.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/database/index.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/database/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/database/server_connector.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/database/server_connector.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/export/index.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/export/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/cats.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/cats.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/date.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/date.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/key.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/key.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/key_list.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/key_list.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/literal.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/literal.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/literal_list.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/literal_list.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/literal_long.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/literal_long.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/name.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/name.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/name_list.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/name_list.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/range.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/range.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/range_list.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/range_list.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/tag_list.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/tag_list.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/title.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/title.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/uri.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/uri.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/verbatim.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/fields/verbatim.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/index.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/strings.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/strings.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/form/templates.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/form/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/import/biblatex.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/import/biblatex.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/import/dialog.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/import/dialog.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/overview/index.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/overview/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/overview/menu.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/overview/menu.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/overview/templates.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/overview/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/schema/common.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/schema/common.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/schema/csl_bib.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/schema/csl_bib.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/schema/literal_long.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/schema/literal_long.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/schema/title.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/schema/title.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/modules/bibliography/tools.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/modules/bibliography/tools.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/static/js/workers/importer/biblatex.js` & `fiduswriter-3.9.9/fiduswriter/bibliography/static/js/workers/importer/biblatex.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/tests/test_overview.py` & `fiduswriter-3.9.9/fiduswriter/bibliography/tests/test_overview.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/bibliography/views.py` & `fiduswriter-3.9.9/fiduswriter/bibliography/views.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/browser_check/templates/browser_check/browser_not_supported.html` & `fiduswriter-3.9.9/fiduswriter/browser_check/templates/browser_check/browser_not_supported.html`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/browser_check/tests/test_access.py` & `fiduswriter-3.9.9/fiduswriter/browser_check/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/configuration.py-default` & `fiduswriter-3.9.9/fiduswriter/configuration.py-default`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/admin.py` & `fiduswriter-3.9.9/fiduswriter/document/admin.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/fixtures/initial_documenttemplates.json` & `fiduswriter-3.9.9/fiduswriter/document/fixtures/initial_documenttemplates.json`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/helpers/serializers.py` & `fiduswriter-3.9.9/fiduswriter/document/helpers/serializers.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/helpers/session_user_info.py` & `fiduswriter-3.9.9/fiduswriter/document/helpers/session_user_info.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/management/commands/export_schema.py` & `fiduswriter-3.9.9/fiduswriter/document/management/commands/export_schema.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/migrations/0001_squashed_20200219.py` & `fiduswriter-3.9.9/fiduswriter/document/migrations/0001_squashed_20200219.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/migrations/0002_fidus_3_2.py` & `fiduswriter-3.9.9/fiduswriter/document/migrations/0002_fidus_3_2.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/migrations/0003_fidus_3_3.py` & `fiduswriter-3.9.9/fiduswriter/document/migrations/0003_fidus_3_3.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/migrations/0004_move_json_data.py` & `fiduswriter-3.9.9/fiduswriter/document/migrations/0004_move_json_data.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/migrations/0005_auto_20201109_0255.py` & `fiduswriter-3.9.9/fiduswriter/document/migrations/0005_auto_20201109_0255.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/migrations/0007_fix_fidus_3_3.py` & `fiduswriter-3.9.9/fiduswriter/document/migrations/0007_fix_fidus_3_3.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/models.py` & `fiduswriter-3.9.9/fiduswriter/document/models.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/package.json` & `fiduswriter-3.9.9/fiduswriter/document/package.json`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/prosemirror.py` & `fiduswriter-3.9.9/fiduswriter/document/prosemirror.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/css/chat.css` & `fiduswriter-3.9.9/fiduswriter/document/static/css/chat.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/css/citation_dialog.css` & `fiduswriter-3.9.9/fiduswriter/document/static/css/citation_dialog.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/css/document.css` & `fiduswriter-3.9.9/fiduswriter/document/static/css/document.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/css/document_template_designer.css` & `fiduswriter-3.9.9/fiduswriter/document/static/css/document_template_designer.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/css/document_template_designer_admin.css` & `fiduswriter-3.9.9/fiduswriter/document/static/css/document_template_designer_admin.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/css/dot_menu.css` & `fiduswriter-3.9.9/fiduswriter/document/static/css/dot_menu.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/css/editor.css` & `fiduswriter-3.9.9/fiduswriter/document/static/css/editor.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/css/footnotes.css` & `fiduswriter-3.9.9/fiduswriter/document/static/css/footnotes.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/css/margin_boxes.css` & `fiduswriter-3.9.9/fiduswriter/document/static/css/margin_boxes.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/css/merge.css` & `fiduswriter-3.9.9/fiduswriter/document/static/css/merge.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/css/tags.css` & `fiduswriter-3.9.9/fiduswriter/document/static/css/tags.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/css/tracking.css` & `fiduswriter-3.9.9/fiduswriter/document/static/css/tracking.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/Cardo-Bold.woff` & `fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/Cardo-Bold.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/Cardo-Italic.woff` & `fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/Cardo-Italic.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/Cardo-Regular.woff` & `fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/Cardo-Regular.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/CrimsonText-Bold.woff` & `fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/CrimsonText-Bold.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/CrimsonText-BoldItalic.woff` & `fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/CrimsonText-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/CrimsonText-Italic.woff` & `fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/CrimsonText-Italic.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/CrimsonText-Roman.woff` & `fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/CrimsonText-Roman.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/Lobster-1.4.woff` & `fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/Lobster-1.4.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/NoticiaText-Bold.woff` & `fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/NoticiaText-Bold.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/NoticiaText-BoldItalic.woff` & `fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/NoticiaText-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/NoticiaText-Italic.woff` & `fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/NoticiaText-Italic.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/NoticiaText-Regular.woff` & `fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/NoticiaText-Regular.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/OpenSans-Bold.woff` & `fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/OpenSans-Bold.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/OpenSans-Regular.woff` & `fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/OpenSans-Regular.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/fonts/document/SourceSansPro-Bold.woff` & `fiduswriter-3.9.9/fiduswriter/document/static/fonts/document/SourceSansPro-Bold.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/citations/citeproc_sys.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/citations/citeproc_sys.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/citations/format.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/citations/format.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/citations/render.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/citations/render.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/admin.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/admin.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/designer.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/designer.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/document_style_dialog.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/document_style_dialog.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/export_template_dialog.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/export_template_dialog.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/extract_template.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/extract_template.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/fix_doc.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/fix_doc.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/schema.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/schema.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/templates.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/document_template/tools.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/document_template/tools.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/access_rights/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/access_rights/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/access_rights/templates.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/access_rights/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/invite.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/invite.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/overview/actions.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/overview/actions.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/overview/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/overview/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/overview/menu.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/overview/menu.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/overview/templates.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/overview/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/revisions/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/revisions/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/revisions/templates.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/revisions/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/documents/tools.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/documents/tools.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/citations/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/citations/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/copy/schema.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/copy/schema.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/copy/serializers.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/copy/serializers.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/paste/fidus_writer.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/paste/fidus_writer.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/paste/general.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/paste/general.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/paste/google_docs.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/paste/google_docs.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/paste/html.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/paste/html.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/paste/libreoffice_writer.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/paste/libreoffice_writer.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/paste/microsoft_word.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/paste/microsoft_word.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/clipboard/paste/text.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/clipboard/paste/text.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/chat.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/chat.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/colors.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/colors.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/doc.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/doc.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/changeset.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/changeset.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/editor.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/editor.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/footnotes.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/footnotes.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/recreate_transform.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/recreate_transform.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/schema.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/schema.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/state_plugins/action.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/state_plugins/action.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/state_plugins/clipboard.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/state_plugins/clipboard.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/state_plugins/diff.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/state_plugins/diff.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/collab/merge/tools.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/collab/merge/tools.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/comments/comment.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/comments/comment.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/comments/editors/answer.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/comments/editors/answer.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/comments/editors/comment.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/comments/editors/comment.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/comments/editors/schema.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/comments/editors/schema.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/comments/interactions.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/comments/interactions.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/comments/store.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/comments/store.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/databases/bibliography.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/databases/bibliography.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/databases/images.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/databases/images.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/databases/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/databases/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/citation.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/citation.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/contributor.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/contributor.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/figure.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/figure.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/language.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/language.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/link.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/link.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/math.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/math.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/ordered_list.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/ordered_list.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/revision.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/revision.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/table.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/table.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/dialogs/templates.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/dialogs/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/document_template/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/document_template/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/footnotes/editor.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/footnotes/editor.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/footnotes/layout.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/footnotes/layout.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/footnotes/state_plugins/access_rights.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/footnotes/state_plugins/access_rights.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/keymap.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/keymap.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/marginboxes/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/marginboxes/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/marginboxes/templates.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/marginboxes/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/figure/model.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/figure/model.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/headerbar/model.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/headerbar/model.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/headerbar/view.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/headerbar/view.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/image/model.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/image/model.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/navigator/model.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/navigator/model.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/selection/model.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/selection/model.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/selection/view.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/selection/view.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/table/model.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/table/model.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/toolbar/model.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/toolbar/model.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/menus/toolbar/view.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/menus/toolbar/view.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/navigator/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/navigator/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/access_rights.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/access_rights.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/citation_render.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/citation_render.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/clipboard.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/clipboard.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/collab_carets.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/collab_carets.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/comments.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/comments.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/contributor_input.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/contributor_input.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/document_template.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/document_template.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/figure.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/figure.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/footnote_markers.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/footnote_markers.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/jump_hidden_nodes.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/jump_hidden_nodes.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/links.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/links.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/ordered_list_menu.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/ordered_list_menu.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/placeholders.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/placeholders.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/search.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/search.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/settings.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/settings.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/table.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/table.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/tag_input.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/tag_input.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/toc_render.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/toc_render.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/track/find_selected_changes.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/track/find_selected_changes.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/track/helpers.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/track/helpers.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/state_plugins/track/plugin.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/state_plugins/track/plugin.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/tools/key_bindings/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/tools/key_bindings/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/tools/key_bindings/templates.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/tools/key_bindings/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/tools/search_replace/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/tools/search_replace/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/tools/search_replace/templates.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/tools/search_replace/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/tools/word_count/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/tools/word_count/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/tools/word_count/templates.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/tools/word_count/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/accept.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/accept.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/accept_all.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/accept_all.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/accept_all_no_insertions.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/accept_all_no_insertions.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/amend_transaction.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/amend_transaction.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/delete.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/delete.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/mod.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/mod.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/reject.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/reject.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/editor/track/reject_all.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/editor/track/reject_all.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/citations.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/citations.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/footnotes.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/footnotes.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/images.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/images.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/lists.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/lists.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/math.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/math.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/metadata.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/metadata.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/rels.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/rels.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/render.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/render.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/richtext.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/richtext.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/docx/tables.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/docx/tables.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/epub/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/epub/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/epub/templates.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/epub/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/epub/tools.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/epub/tools.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/html/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/html/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/html/templates.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/html/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/jats/citations.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/jats/citations.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/jats/convert.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/jats/convert.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/jats/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/jats/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/jats/templates.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/jats/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/latex/convert.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/latex/convert.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/latex/escape_latex.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/latex/escape_latex.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/latex/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/latex/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/latex/readme.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/latex/readme.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/native/copy.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/native/copy.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/native/file.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/native/file.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/native/revision.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/native/revision.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/native/shrink.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/native/shrink.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/native/zip.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/native/zip.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/citations.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/citations.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -13,20 +13,19 @@
     cslBibSchema
 } from "../../bibliography/schema/csl_bib"
 import {
     descendantNodes
 } from "../tools/doc_content"
 
 export class OdtExporterCitations {
-    constructor(exporter, bibDB, csl, docContent, docTemplate, origCitInfos = []) {
+    constructor(exporter, bibDB, csl, docContent, origCitInfos = []) {
         this.exporter = exporter
         this.bibDB = bibDB
         this.csl = csl
         this.docContent = docContent
-        this.docTemplate = docTemplate
         // If citInfos were found in a previous run, they are stored here
         // (for example: first citations in main document, then in footnotes)
         this.origCitInfos = origCitInfos
         this.citInfos = []
         this.citationTexts = []
         this.pmCits = []
         this.citFm = false
```

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/footnotes.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/footnotes.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/images.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/images.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/math.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/math.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/metadata.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/metadata.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/render.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/render.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/richtext.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/richtext.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -209,15 +209,15 @@
                 start += '<text:p text:style-name="Standard">'
                 end = '</text:p>' + end
 
                 if (node.attrs.aligned === 'center') {
                     // Needed to prevent subsequent image from overlapping
                     end = end + '<text:p text:style-name="Standard"></text:p>'
                 }
-                let caption = node.attrs.caption ? node.content.find(node => node.type === 'figure_caption')?.content.map(node => this.transformRichtext(node)).join('') || '' : ''
+                let caption = node.attrs.caption ? node.content.find(node => node.type === 'figure_caption')?.content?.map(node => this.transformRichtext(node)).join('') || '' : ''
                 // The figure category should not be in the
                 // user's language but rather the document language
                 const category = node.attrs.category
                 if (category !== 'none') {
                     const categoryCounter = options.inFootnote ? this.fnCategoryCounter : this.categoryCounter
                     if (!categoryCounter[category]) {
                         categoryCounter[category] = 1
```

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/odt/styles.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/odt/styles.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/print/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/print/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/tools/doc_content.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/tools/doc_content.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/tools/dom_export.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/tools/dom_export.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/tools/html.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/tools/html.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/tools/json.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/tools/json.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/tools/xml_zip.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/tools/xml_zip.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/exporter/tools/zip.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/exporter/tools/zip.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/importer/file.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/importer/file.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/importer/get_images.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/importer/get_images.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/importer/native.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/importer/native.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/importer/update.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/importer/update.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/maintenance/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/maintenance/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/annotate.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/annotate.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/base.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/base.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/citation.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/citation.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/equation.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/equation.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/figure.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/figure.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/heading.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/heading.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/list.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/list.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/reference.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/reference.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/table.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/table.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/common/track.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/common/track.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/const.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/const.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/convert.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/convert.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/document/content.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/document/content.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/document/index.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/document/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/document/structure.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/document/structure.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/export.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/export.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/footnotes.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/footnotes.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/footnotes_convert.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/footnotes_convert.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/i18n.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/i18n.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/modules/schema/mini_json.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/modules/schema/mini_json.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/js/workers/document_template/adjust_doc.js` & `fiduswriter-3.9.9/fiduswriter/document/static/js/workers/document_template/adjust_doc.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/static/ogg/chat_notification.ogg` & `fiduswriter-3.9.9/fiduswriter/document/static/ogg/chat_notification.ogg`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/templates/admin/document/documenttemplate/change_form.html` & `fiduswriter-3.9.9/fiduswriter/document/templates/admin/document/documenttemplate/change_form.html`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/templates/admin/document/maintenance.html` & `fiduswriter-3.9.9/fiduswriter/document/templates/admin/document/maintenance.html`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/tests/editor_helper.py` & `fiduswriter-3.9.9/fiduswriter/document/tests/editor_helper.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/tests/test_admin.py` & `fiduswriter-3.9.9/fiduswriter/document/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/tests/test_collaboration.py` & `fiduswriter-3.9.9/fiduswriter/document/tests/test_collaboration.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/tests/test_editor.py` & `fiduswriter-3.9.9/fiduswriter/document/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/tests/test_export.py` & `fiduswriter-3.9.9/fiduswriter/document/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/tests/test_message_exchange.py` & `fiduswriter-3.9.9/fiduswriter/document/tests/test_message_exchange.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/tests/test_offline.py` & `fiduswriter-3.9.9/fiduswriter/document/tests/test_offline.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/tests/uploads/image.png` & `fiduswriter-3.9.9/fiduswriter/document/tests/uploads/image.png`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/urls.py` & `fiduswriter-3.9.9/fiduswriter/document/urls.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/views.py` & `fiduswriter-3.9.9/fiduswriter/document/views.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/document/ws_views.py` & `fiduswriter-3.9.9/fiduswriter/document/ws_views.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/feedback/migrations/0001_initial.py` & `fiduswriter-3.9.9/fiduswriter/feedback/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/feedback/models.py` & `fiduswriter-3.9.9/fiduswriter/feedback/models.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/feedback/static/css/feedback/feedback.css` & `fiduswriter-3.9.9/fiduswriter/feedback/static/css/feedback/feedback.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/feedback/static/js/modules/feedback/index.js` & `fiduswriter-3.9.9/fiduswriter/feedback/static/js/modules/feedback/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/feedback/tests/test_feedback.py` & `fiduswriter-3.9.9/fiduswriter/feedback/tests/test_feedback.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/feedback/views.py` & `fiduswriter-3.9.9/fiduswriter/feedback/views.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/fixturemedia/management/commands/dumpdata.py` & `fiduswriter-3.9.9/fiduswriter/fixturemedia/management/commands/dumpdata.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/fixturemedia/management/commands/loaddata.py` & `fiduswriter-3.9.9/fiduswriter/fixturemedia/management/commands/loaddata.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/bg/LC_MESSAGES/django.mo` & `fiduswriter-3.9.9/fiduswriter/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/bg/LC_MESSAGES/django.po` & `fiduswriter-3.9.9/fiduswriter/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/bg/LC_MESSAGES/djangojs.mo` & `fiduswriter-3.9.9/fiduswriter/locale/bg/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/bg/LC_MESSAGES/djangojs.po` & `fiduswriter-3.9.9/fiduswriter/locale/bg/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/copyright.txt` & `fiduswriter-3.9.9/fiduswriter/locale/copyright.txt`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/de/LC_MESSAGES/django.mo` & `fiduswriter-3.9.9/fiduswriter/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/de/LC_MESSAGES/django.po` & `fiduswriter-3.9.9/fiduswriter/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/de/LC_MESSAGES/djangojs.mo` & `fiduswriter-3.9.9/fiduswriter/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/de/LC_MESSAGES/djangojs.po` & `fiduswriter-3.9.9/fiduswriter/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/es/LC_MESSAGES/django.mo` & `fiduswriter-3.9.9/fiduswriter/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/es/LC_MESSAGES/django.po` & `fiduswriter-3.9.9/fiduswriter/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/es/LC_MESSAGES/djangojs.mo` & `fiduswriter-3.9.9/fiduswriter/locale/es/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/es/LC_MESSAGES/djangojs.po` & `fiduswriter-3.9.9/fiduswriter/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/fr/LC_MESSAGES/django.mo` & `fiduswriter-3.9.9/fiduswriter/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/fr/LC_MESSAGES/django.po` & `fiduswriter-3.9.9/fiduswriter/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/fr/LC_MESSAGES/djangojs.mo` & `fiduswriter-3.9.9/fiduswriter/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/fr/LC_MESSAGES/djangojs.po` & `fiduswriter-3.9.9/fiduswriter/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/it/LC_MESSAGES/django.mo` & `fiduswriter-3.9.9/fiduswriter/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/it/LC_MESSAGES/django.po` & `fiduswriter-3.9.9/fiduswriter/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/it/LC_MESSAGES/djangojs.mo` & `fiduswriter-3.9.9/fiduswriter/locale/it/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/it/LC_MESSAGES/djangojs.po` & `fiduswriter-3.9.9/fiduswriter/locale/it/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/pt_BR/LC_MESSAGES/django.mo` & `fiduswriter-3.9.9/fiduswriter/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/pt_BR/LC_MESSAGES/django.po` & `fiduswriter-3.9.9/fiduswriter/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `fiduswriter-3.9.9/fiduswriter/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/locale/pt_BR/LC_MESSAGES/djangojs.po` & `fiduswriter-3.9.9/fiduswriter/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/manage.py` & `fiduswriter-3.9.9/fiduswriter/manage.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/menu/static/js/modules/menu/index.js` & `fiduswriter-3.9.9/fiduswriter/menu/static/js/modules/menu/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/admin.py` & `fiduswriter-3.9.9/fiduswriter/style/admin.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/initial_styles.json` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/initial_styles.json`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/export-template-files/Classic.docx` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/export-template-files/Classic.docx`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/export-template-files/Free.odt` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/export-template-files/Free.odt`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/Cardo-Bold.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/Cardo-Bold.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/Cardo-Italic.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/Cardo-Italic.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/Cardo-Regular.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/Cardo-Regular.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/CrimsonText-Bold.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/CrimsonText-Bold.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/CrimsonText-BoldItalic.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/CrimsonText-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/CrimsonText-Italic.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/CrimsonText-Italic.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/CrimsonText-Roman.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/CrimsonText-Roman.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/Lobster-1.4.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/Lobster-1.4.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-BoldItalic.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-BoldItalic_KMSnKTE.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-BoldItalic_KMSnKTE.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-BoldItalic_Xg38HXg.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-BoldItalic_Xg38HXg.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Bold_2.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Bold_2.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Bold_2_77vhC50.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Bold_2_77vhC50.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Bold_2_qiGg4Ow.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Bold_2_qiGg4Ow.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Italic.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Italic.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Italic_3AoQkPt.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Italic_3AoQkPt.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Italic_ai8IvB3.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Italic_ai8IvB3.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Regular.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Regular.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Regular_eNSdC3U.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Regular_eNSdC3U.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/NoticiaText-Regular_zGx3t7x.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/NoticiaText-Regular_zGx3t7x.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/OpenSans-Bold.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/OpenSans-Bold.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/OpenSans-Regular.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/OpenSans-Regular.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/SourceSansPro-Bold.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/SourceSansPro-Bold.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/fixtures/media/style-files/SourceSansPro-Bold_ySHS5jh.woff` & `fiduswriter-3.9.9/fiduswriter/style/fixtures/media/style-files/SourceSansPro-Bold_ySHS5jh.woff`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/migrations/0001_squashed_20200219.py` & `fiduswriter-3.9.9/fiduswriter/style/migrations/0001_squashed_20200219.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/models.py` & `fiduswriter-3.9.9/fiduswriter/style/models.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/urls.py` & `fiduswriter-3.9.9/fiduswriter/style/urls.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/style/views.py` & `fiduswriter-3.9.9/fiduswriter/style/views.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/stylelint.config.js` & `fiduswriter-3.9.9/fiduswriter/stylelint.config.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/testing/eslint_import_resolver.js` & `fiduswriter-3.9.9/fiduswriter/testing/eslint_import_resolver.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/testing/selenium_helper.py` & `fiduswriter-3.9.9/fiduswriter/testing/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/testing/testcases.py` & `fiduswriter-3.9.9/fiduswriter/testing/testcases.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/adapter.py` & `fiduswriter-3.9.9/fiduswriter/user/adapter.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/migrations/0001_squashed_0003_auto_20151226_1110.py` & `fiduswriter-3.9.9/fiduswriter/user/migrations/0001_squashed_0003_auto_20151226_1110.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/migrations/0002_loginas.py` & `fiduswriter-3.9.9/fiduswriter/user/migrations/0002_loginas.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/models.py` & `fiduswriter-3.9.9/fiduswriter/user/models.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/signals.py` & `fiduswriter-3.9.9/fiduswriter/user/signals.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/static/css/show_profile.css` & `fiduswriter-3.9.9/fiduswriter/user/static/css/show_profile.css`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/static/js/modules/contacts/add_dialog.js` & `fiduswriter-3.9.9/fiduswriter/user/static/js/modules/contacts/add_dialog.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/static/js/modules/contacts/delete_dialog.js` & `fiduswriter-3.9.9/fiduswriter/user/static/js/modules/contacts/delete_dialog.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/static/js/modules/contacts/index.js` & `fiduswriter-3.9.9/fiduswriter/user/static/js/modules/contacts/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/static/js/modules/contacts/menu.js` & `fiduswriter-3.9.9/fiduswriter/user/static/js/modules/contacts/menu.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/static/js/modules/contacts/templates.js` & `fiduswriter-3.9.9/fiduswriter/user/static/js/modules/contacts/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/static/js/modules/email_confirm/index.js` & `fiduswriter-3.9.9/fiduswriter/user/static/js/modules/email_confirm/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/static/js/modules/email_confirm/templates.js` & `fiduswriter-3.9.9/fiduswriter/user/static/js/modules/email_confirm/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/static/js/modules/login/index.js` & `fiduswriter-3.9.9/fiduswriter/user/static/js/modules/login/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/static/js/modules/password_reset/change_password.js` & `fiduswriter-3.9.9/fiduswriter/user/static/js/modules/password_reset/change_password.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/static/js/modules/password_reset/request_email.js` & `fiduswriter-3.9.9/fiduswriter/user/static/js/modules/password_reset/request_email.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/static/js/modules/profile/delete_user.js` & `fiduswriter-3.9.9/fiduswriter/user/static/js/modules/profile/delete_user.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/static/js/modules/profile/dialogs.js` & `fiduswriter-3.9.9/fiduswriter/user/static/js/modules/profile/dialogs.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/static/js/modules/profile/index.js` & `fiduswriter-3.9.9/fiduswriter/user/static/js/modules/profile/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/static/js/modules/profile/templates.js` & `fiduswriter-3.9.9/fiduswriter/user/static/js/modules/profile/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/static/js/modules/signup/index.js` & `fiduswriter-3.9.9/fiduswriter/user/static/js/modules/signup/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/templates/account/email/email_confirmation_message.html` & `fiduswriter-3.9.9/fiduswriter/user/templates/account/email/email_confirmation_message.html`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/templates/account/email/password_reset_key_message.html` & `fiduswriter-3.9.9/fiduswriter/user/templates/account/email/password_reset_key_message.html`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/tests/test_contacts.py` & `fiduswriter-3.9.9/fiduswriter/user/tests/test_contacts.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/tests/test_profile.py` & `fiduswriter-3.9.9/fiduswriter/user/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/urls.py` & `fiduswriter-3.9.9/fiduswriter/user/urls.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/util.py` & `fiduswriter-3.9.9/fiduswriter/user/util.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user/views.py` & `fiduswriter-3.9.9/fiduswriter/user/views.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/modules/user_template_manager/actions.js` & `fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/modules/user_template_manager/actions.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/modules/user_template_manager/editor.js` & `fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/modules/user_template_manager/editor.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/modules/user_template_manager/menu.js` & `fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/modules/user_template_manager/menu.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/modules/user_template_manager/overview.js` & `fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/modules/user_template_manager/overview.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user_template_manager/static/js/plugins/app/user_template_manager.js` & `fiduswriter-3.9.9/fiduswriter/user_template_manager/static/js/plugins/app/user_template_manager.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/user_template_manager/views.py` & `fiduswriter-3.9.9/fiduswriter/user_template_manager/views.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/admin.py` & `fiduswriter-3.9.9/fiduswriter/usermedia/admin.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/migrations/0001_squashed_0009_auto_20170908_0953.py` & `fiduswriter-3.9.9/fiduswriter/usermedia/migrations/0001_squashed_0009_auto_20170908_0953.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/migrations/0002_auto_20200205_2140.py` & `fiduswriter-3.9.9/fiduswriter/usermedia/migrations/0002_auto_20200205_2140.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/migrations/0003_auto_20200205_2230.py` & `fiduswriter-3.9.9/fiduswriter/usermedia/migrations/0003_auto_20200205_2230.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/migrations/0004_auto_20200205_2347.py` & `fiduswriter-3.9.9/fiduswriter/usermedia/migrations/0004_auto_20200205_2347.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/migrations/0005_move_json_data.py` & `fiduswriter-3.9.9/fiduswriter/usermedia/migrations/0005_move_json_data.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/migrations/0006_auto_20200820_0510.py` & `fiduswriter-3.9.9/fiduswriter/usermedia/migrations/0006_auto_20200820_0510.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/models.py` & `fiduswriter-3.9.9/fiduswriter/usermedia/models.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/database.js` & `fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/database.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/edit_dialog/index.js` & `fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/edit_dialog/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/edit_dialog/model.js` & `fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/edit_dialog/model.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/edit_dialog/templates.js` & `fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/edit_dialog/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/overview/categories.js` & `fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/overview/categories.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/overview/index.js` & `fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/overview/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/overview/menu.js` & `fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/overview/menu.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/overview/templates.js` & `fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/overview/templates.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/static/js/modules/images/selection_dialog/index.js` & `fiduswriter-3.9.9/fiduswriter/usermedia/static/js/modules/images/selection_dialog/index.js`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/tests/test_overview.py` & `fiduswriter-3.9.9/fiduswriter/usermedia/tests/test_overview.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/tests/uploads/image.png` & `fiduswriter-3.9.9/fiduswriter/usermedia/tests/uploads/image.png`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter/usermedia/views.py` & `fiduswriter-3.9.9/fiduswriter/usermedia/views.py`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter.egg-info/PKG-INFO` & `fiduswriter-3.9.9/fiduswriter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiduswriter
-Version: 3.9.8
+Version: 3.9.9
 Summary: A semantic wordprocessor for academic purposes
 Home-page: https://www.fiduswriter.org
 Author: Lund Info AB
 Author-email: mail@lundinfo.com
 License: AGPL
 Description: Fidus Writer
         ============
```

### Comparing `fiduswriter-3.9.8/fiduswriter.egg-info/SOURCES.txt` & `fiduswriter-3.9.9/fiduswriter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/fiduswriter.egg-info/requires.txt` & `fiduswriter-3.9.9/fiduswriter.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fiduswriter-3.9.8/setup.py` & `fiduswriter-3.9.9/setup.py`

 * *Files identical despite different names*

