# Comparing `tmp/otcdocstheme-0.8.1.tar.gz` & `tmp/otcdocstheme-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otcdocstheme-0.8.1.tar", last modified: Mon Jan 24 08:47:32 2022, max compression
+gzip compressed data, was "otcdocstheme-0.9.0.tar", last modified: Thu Jan 27 17:01:57 2022, max compression
```

## Comparing `otcdocstheme-0.8.1.tar` & `otcdocstheme-0.9.0.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.520211 otcdocstheme-0.8.1/
--rw-r--r--   0 root         (0) root         (0)     1070 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      777 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/.zuul.yaml
--rw-r--r--   0 root         (0) root         (0)      317 2022-01-24 08:47:32.000000 otcdocstheme-0.8.1/AUTHORS
--rw-r--r--   0 root         (0) root         (0)      109 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)     1217 2022-01-24 08:47:32.000000 otcdocstheme-0.8.1/ChangeLog
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/HACKING.rst
--rw-r--r--   0 root         (0) root         (0)    11357 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6782 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/Makefile
--rw-r--r--   0 root         (0) root         (0)     1667 2022-01-24 08:47:32.520211 otcdocstheme-0.8.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      606 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.451210 otcdocstheme-0.8.1/api-ref/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.459210 otcdocstheme-0.8.1/api-ref/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.451210 otcdocstheme-0.8.1/api-ref/source/_static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.459210 otcdocstheme-0.8.1/api-ref/source/_static/css/
--rw-r--r--   0 root         (0) root         (0)      160 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/api-ref/source/_static/css/README.md
--rw-r--r--   0 root         (0) root         (0)     3008 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/api-ref/source/conf.py
--rw-r--r--   0 root         (0) root         (0)     2384 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/api-ref/source/image.inc
--rw-r--r--   0 root         (0) root         (0)       84 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/api-ref/source/index.rst
--rw-r--r--   0 root         (0) root         (0)      655 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/api-ref/source/parameters.yaml
--rw-r--r--   0 root         (0) root         (0)     3132 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/api-ref/source/service.inc
--rw-r--r--   0 root         (0) root         (0)      370 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/api-ref/source/status.yaml
--rw-r--r--   0 root         (0) root         (0)       52 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/api-ref/source/update-server-resp.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.459210 otcdocstheme-0.8.1/bin/
--rw-r--r--   0 root         (0) root         (0)     1159 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/bin/docstheme-build-pdf
--rw-r--r--   0 root         (0) root         (0)     1167 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/bindep.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.460210 otcdocstheme-0.8.1/doc/
--rw-r--r--   0 root         (0) root         (0)      489 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/doc/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.461210 otcdocstheme-0.8.1/doc/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.451210 otcdocstheme-0.8.1/doc/source/_static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.461210 otcdocstheme-0.8.1/doc/source/_static/css/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/doc/source/_static/css/.placeholder
--rw-r--r--   0 root         (0) root         (0)     2254 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/doc/source/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.464210 otcdocstheme-0.8.1/doc/source/demo/
--rw-r--r--   0 root         (0) root         (0)     7146 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/doc/source/demo/configure_access_and_security_for_instances.rst
--rw-r--r--   0 root         (0) root         (0)     4896 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/doc/source/demo/create_and_manage_databases.rst
--rw-r--r--   0 root         (0) root         (0)     3317 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/doc/source/demo/create_and_manage_networks.rst
--rw-r--r--   0 root         (0) root         (0)     6490 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/doc/source/demo/dashboard_demo.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.467210 otcdocstheme-0.8.1/doc/source/demo/figures/
--rw-r--r--   0 root         (0) root         (0)    74714 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/doc/source/demo/figures/dashboard-project-tab.png
--rw-r--r--   0 root         (0) root         (0)    72705 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/doc/source/demo/figures/dashboard_admin_project_tab.png
--rw-r--r--   0 root         (0) root         (0)    42821 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/doc/source/demo/figures/doc-logo-fox.jpg
--rw-r--r--   0 root         (0) root         (0)     4211 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/doc/source/demo/index.rst
--rw-r--r--   0 root         (0) root         (0)     2788 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/doc/source/demo/launch-instance.rst
--rw-r--r--   0 root         (0) root         (0)     6987 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/doc/source/demo/section_dashboard_access_and_security.rst
--rw-r--r--   0 root         (0) root         (0)     3010 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/doc/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.470210 otcdocstheme-0.8.1/otcdocstheme/
--rw-r--r--   0 root         (0) root         (0)      666 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14876 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/ext.py
--rw-r--r--   0 root         (0) root         (0)     3777 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/page_context.py
--rw-r--r--   0 root         (0) root         (0)     1270 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/paths.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.452210 otcdocstheme-0.8.1/otcdocstheme/theme/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.477211 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/
--rw-r--r--   0 root         (0) root         (0)     1009 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/css.html
--rw-r--r--   0 root         (0) root         (0)      543 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/footer.html
--rw-r--r--   0 root         (0) root         (0)     2150 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/header.html
--rw-r--r--   0 root         (0) root         (0)     1939 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/layout.html
--rw-r--r--   0 root         (0) root         (0)      345 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/license_cc.html
--rw-r--r--   0 root         (0) root         (0)      346 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/localtoc.html
--rw-r--r--   0 root         (0) root         (0)     3046 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/script_footer.html
--rw-r--r--   0 root         (0) root         (0)       75 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/script_search.html
--rw-r--r--   0 root         (0) root         (0)     1203 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/search.html
--rw-r--r--   0 root         (0) root         (0)      582 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/sidebartoc.html
--rw-r--r--   0 root         (0) root         (0)      401 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/sidebartoc_menu.html
--rw-r--r--   0 root         (0) root         (0)      393 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/sidebartoc_menu_apiref.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.478211 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.485211 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/css/
--rw-r--r--   0 root         (0) root         (0)   146010 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/css/bootstrap.css
--rw-r--r--   0 root         (0) root         (0)   121200 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/css/bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)    95095 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/css/combined.css
--rw-r--r--   0 root         (0) root         (0)    37414 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/css/font-awesome.css
--rw-r--r--   0 root         (0) root         (0)    31000 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/css/font-awesome.min.css
--rw-r--r--   0 root         (0) root         (0)     6733 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/css/otcdocstheme.css
--rwxr-xr-x   0 root         (0) root         (0)     1150 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.498211 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/.gitkeep
--rw-r--r--   0 root         (0) root         (0)   124988 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/FontAwesome.otf
--rw-r--r--   0 root         (0) root         (0)    76518 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 root         (0) root         (0)   391621 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 root         (0) root         (0)   152796 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 root         (0) root         (0)    90412 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 root         (0) root         (0)    71896 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 root         (0) root         (0)    20127 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 root         (0) root         (0)   108737 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 root         (0) root         (0)    45404 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 root         (0) root         (0)    23424 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 root         (0) root         (0)    18028 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.504211 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/
--rw-r--r--   0 root         (0) root         (0)      751 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/deutsche-telekom-logo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.507211 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/docs/
--rw-r--r--   0 root         (0) root         (0)     4739 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/docs/license.png
--rw-r--r--   0 root         (0) root         (0)    18616 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/docs/superuser1.png
--rw-r--r--   0 root         (0) root         (0)    14372 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/docs/superuser2.png
--rw-r--r--   0 root         (0) root         (0)    12403 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/docs/superuser3.png
--rw-r--r--   0 root         (0) root         (0)    11727 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/docs/superuser4.png
--rw-r--r--   0 root         (0) root         (0)     1099 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/footer-facebook-hover.png
--rw-r--r--   0 root         (0) root         (0)     1097 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/footer-facebook.png
--rw-r--r--   0 root         (0) root         (0)     1119 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/footer-linkedin-hover.png
--rw-r--r--   0 root         (0) root         (0)     1144 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/footer-linkedin.png
--rw-r--r--   0 root         (0) root         (0)     1277 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/footer-twitter-hover.png
--rw-r--r--   0 root         (0) root         (0)     1280 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/footer-twitter.png
--rw-r--r--   0 root         (0) root         (0)     1045 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/footer-youtube-hover.png
--rw-r--r--   0 root         (0) root         (0)     1209 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/footer-youtube.png
--rw-r--r--   0 root         (0) root         (0)      729 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/loading.gif
--rw-r--r--   0 root         (0) root         (0)      751 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/logo-full.png
--rw-r--r--   0 root         (0) root         (0)      937 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/openstack-logo-full.png
--rw-r--r--   0 root         (0) root         (0)      658 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/openstack-logo-vert.png
--rw-r--r--   0 root         (0) root         (0)      278 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/search-icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.514211 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/js/
--rw-r--r--   0 root         (0) root         (0)    69707 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/js/bootstrap.js
--rw-r--r--   0 root         (0) root         (0)    37045 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/js/bootstrap.min.js
--rw-r--r--   0 root         (0) root         (0)     4175 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/js/docs.js
--rw-r--r--   0 root         (0) root         (0)   268039 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/js/jquery-3.2.1.js
--rw-r--r--   0 root         (0) root         (0)    86659 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/js/jquery-3.2.1.min.js
--rw-r--r--   0 root         (0) root         (0)     1887 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/js/navigation.js
--rw-r--r--   0 root         (0) root         (0)    20621 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/js/webui-popover.js
--rw-r--r--   0 root         (0) root         (0)      275 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/package.json
--rw-r--r--   0 root         (0) root         (0)      157 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/swiftype_search.html
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/swiftype_search_install.html
--rw-r--r--   0 root         (0) root         (0)      130 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/swiftype_search_mobile.html
--rw-r--r--   0 root         (0) root         (0)      293 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/theme.conf
--rw-r--r--   0 root         (0) root         (0)      900 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/titlerow.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.515211 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs_pdf/
--rw-r--r--   0 root         (0) root         (0)      766 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs_pdf/deutsche-telekom-logo.png
--rw-r--r--   0 root         (0) root         (0)     1821 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs_pdf/pdftheme.sty
--rw-r--r--   0 root         (0) root         (0)      648 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/otcdocstheme/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.470210 otcdocstheme-0.8.1/otcdocstheme.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1667 2022-01-24 08:47:32.000000 otcdocstheme-0.8.1/otcdocstheme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5612 2022-01-24 08:47:32.000000 otcdocstheme-0.8.1/otcdocstheme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-24 08:47:32.000000 otcdocstheme-0.8.1/otcdocstheme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-24 08:47:32.000000 otcdocstheme-0.8.1/otcdocstheme.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2022-01-24 08:47:32.000000 otcdocstheme-0.8.1/otcdocstheme.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       35 2022-01-24 08:47:32.000000 otcdocstheme-0.8.1/otcdocstheme.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-01-24 08:47:32.000000 otcdocstheme-0.8.1/otcdocstheme.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.452210 otcdocstheme-0.8.1/releasenotes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.519211 otcdocstheme-0.8.1/releasenotes/notes/
--rw-r--r--   0 root         (0) root         (0)       76 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/releasenotes/notes/add-project-links-ff3e9377417a5c10.yaml
--rw-r--r--   0 root         (0) root         (0)       99 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/releasenotes/notes/change-root-link-5e6eb70fb869ac12.yaml
--rw-r--r--   0 root         (0) root         (0)      102 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/releasenotes/notes/drop-google-01017fb959b908a7.yaml
--rw-r--r--   0 root         (0) root         (0)       82 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/releasenotes/notes/fix-api-ref-df2269c9ad560c6b.yaml
--rw-r--r--   0 root         (0) root         (0)       58 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/releasenotes/notes/fix-bug-tracker-260f8de5be2a849e.yaml
--rw-r--r--   0 root         (0) root         (0)      142 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/releasenotes/notes/fix-sphinx4-ee98168de2714190.yaml
--rw-r--r--   0 root         (0) root         (0)       65 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/releasenotes/notes/fix-table-09c4e5eaf38be8c0.yaml
--rw-r--r--   0 root         (0) root         (0)      227 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/releasenotes/notes/new-theme-4c62220ee9492289.yaml
--rw-r--r--   0 root         (0) root         (0)       79 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/releasenotes/notes/sync-with-openstack-87c6854f3bc4f180.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.520211 otcdocstheme-0.8.1/releasenotes/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.520211 otcdocstheme-0.8.1/releasenotes/source/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/releasenotes/source/_static/.placeholder
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 08:47:32.520211 otcdocstheme-0.8.1/releasenotes/source/_templates/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/releasenotes/source/_templates/.placeholder
--rw-r--r--   0 root         (0) root         (0)     8797 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/releasenotes/source/conf.py
--rw-r--r--   0 root         (0) root         (0)      146 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/releasenotes/source/index.rst
--rw-r--r--   0 root         (0) root         (0)      272 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      836 2022-01-24 08:47:32.521211 otcdocstheme-0.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      766 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/setup.py
--rw-r--r--   0 root         (0) root         (0)      343 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/test-requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1848 2022-01-24 08:41:38.000000 otcdocstheme-0.8.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:57.038336 otcdocstheme-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1070 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      558 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/.zuul.yaml
+-rw-r--r--   0 root         (0) root         (0)      317 2022-01-27 17:01:56.000000 otcdocstheme-0.9.0/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)      109 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)     1258 2022-01-27 17:01:56.000000 otcdocstheme-0.9.0/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/HACKING.rst
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6782 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)     1667 2022-01-27 17:01:57.038336 otcdocstheme-0.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      606 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:56.975335 otcdocstheme-0.9.0/api-ref/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:56.983335 otcdocstheme-0.9.0/api-ref/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:56.975335 otcdocstheme-0.9.0/api-ref/source/_static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:56.983335 otcdocstheme-0.9.0/api-ref/source/_static/css/
+-rw-r--r--   0 root         (0) root         (0)      160 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/api-ref/source/_static/css/README.md
+-rw-r--r--   0 root         (0) root         (0)     3008 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/api-ref/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2384 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/api-ref/source/image.inc
+-rw-r--r--   0 root         (0) root         (0)       84 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/api-ref/source/index.rst
+-rw-r--r--   0 root         (0) root         (0)      655 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/api-ref/source/parameters.yaml
+-rw-r--r--   0 root         (0) root         (0)     3132 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/api-ref/source/service.inc
+-rw-r--r--   0 root         (0) root         (0)      370 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/api-ref/source/status.yaml
+-rw-r--r--   0 root         (0) root         (0)       52 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/api-ref/source/update-server-resp.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:56.983335 otcdocstheme-0.9.0/bin/
+-rw-r--r--   0 root         (0) root         (0)     1159 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/bin/docstheme-build-pdf
+-rw-r--r--   0 root         (0) root         (0)     1167 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/bindep.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:56.984335 otcdocstheme-0.9.0/doc/
+-rw-r--r--   0 root         (0) root         (0)      489 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/doc/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:56.985335 otcdocstheme-0.9.0/doc/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:56.975335 otcdocstheme-0.9.0/doc/source/_static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:56.985335 otcdocstheme-0.9.0/doc/source/_static/css/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/doc/source/_static/css/.placeholder
+-rw-r--r--   0 root         (0) root         (0)     2273 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/doc/source/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:56.988335 otcdocstheme-0.9.0/doc/source/demo/
+-rw-r--r--   0 root         (0) root         (0)     7146 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/doc/source/demo/configure_access_and_security_for_instances.rst
+-rw-r--r--   0 root         (0) root         (0)     4896 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/doc/source/demo/create_and_manage_databases.rst
+-rw-r--r--   0 root         (0) root         (0)     3317 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/doc/source/demo/create_and_manage_networks.rst
+-rw-r--r--   0 root         (0) root         (0)     6490 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/doc/source/demo/dashboard_demo.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:56.990335 otcdocstheme-0.9.0/doc/source/demo/figures/
+-rw-r--r--   0 root         (0) root         (0)    74714 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/doc/source/demo/figures/dashboard-project-tab.png
+-rw-r--r--   0 root         (0) root         (0)    72705 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/doc/source/demo/figures/dashboard_admin_project_tab.png
+-rw-r--r--   0 root         (0) root         (0)    42821 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/doc/source/demo/figures/doc-logo-fox.jpg
+-rw-r--r--   0 root         (0) root         (0)     4211 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/doc/source/demo/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2788 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/doc/source/demo/launch-instance.rst
+-rw-r--r--   0 root         (0) root         (0)     6987 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/doc/source/demo/section_dashboard_access_and_security.rst
+-rw-r--r--   0 root         (0) root         (0)     3010 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/doc/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:56.993335 otcdocstheme-0.9.0/otcdocstheme/
+-rw-r--r--   0 root         (0) root         (0)      666 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15190 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/ext.py
+-rw-r--r--   0 root         (0) root         (0)     3777 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/page_context.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/paths.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:56.976335 otcdocstheme-0.9.0/otcdocstheme/theme/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:57.000335 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/
+-rw-r--r--   0 root         (0) root         (0)     1009 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/css.html
+-rw-r--r--   0 root         (0) root         (0)      543 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/footer.html
+-rw-r--r--   0 root         (0) root         (0)     2150 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/header.html
+-rw-r--r--   0 root         (0) root         (0)     1939 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/layout.html
+-rw-r--r--   0 root         (0) root         (0)      345 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/license_cc.html
+-rw-r--r--   0 root         (0) root         (0)      346 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/localtoc.html
+-rw-r--r--   0 root         (0) root         (0)     3046 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/script_footer.html
+-rw-r--r--   0 root         (0) root         (0)       75 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/script_search.html
+-rw-r--r--   0 root         (0) root         (0)     1203 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/search.html
+-rw-r--r--   0 root         (0) root         (0)      582 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/sidebartoc.html
+-rw-r--r--   0 root         (0) root         (0)      401 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/sidebartoc_menu.html
+-rw-r--r--   0 root         (0) root         (0)      393 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/sidebartoc_menu_apiref.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:57.001335 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:57.008335 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/css/
+-rw-r--r--   0 root         (0) root         (0)   146010 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/css/bootstrap.css
+-rw-r--r--   0 root         (0) root         (0)   121200 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/css/bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)    95095 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/css/combined.css
+-rw-r--r--   0 root         (0) root         (0)    37414 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/css/font-awesome.css
+-rw-r--r--   0 root         (0) root         (0)    31000 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/css/font-awesome.min.css
+-rw-r--r--   0 root         (0) root         (0)     6733 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/css/otcdocstheme.css
+-rwxr-xr-x   0 root         (0) root         (0)     1150 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:57.021336 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/.gitkeep
+-rw-r--r--   0 root         (0) root         (0)   124988 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/FontAwesome.otf
+-rw-r--r--   0 root         (0) root         (0)    76518 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 root         (0) root         (0)   391621 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 root         (0) root         (0)   152796 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    90412 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 root         (0) root         (0)    71896 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 root         (0) root         (0)    20127 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 root         (0) root         (0)   108737 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 root         (0) root         (0)    45404 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 root         (0) root         (0)    23424 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 root         (0) root         (0)    18028 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:57.027336 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/
+-rw-r--r--   0 root         (0) root         (0)      751 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/deutsche-telekom-logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:57.029336 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/docs/
+-rw-r--r--   0 root         (0) root         (0)     4739 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/docs/license.png
+-rw-r--r--   0 root         (0) root         (0)    18616 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/docs/superuser1.png
+-rw-r--r--   0 root         (0) root         (0)    14372 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/docs/superuser2.png
+-rw-r--r--   0 root         (0) root         (0)    12403 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/docs/superuser3.png
+-rw-r--r--   0 root         (0) root         (0)    11727 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/docs/superuser4.png
+-rw-r--r--   0 root         (0) root         (0)     1099 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/footer-facebook-hover.png
+-rw-r--r--   0 root         (0) root         (0)     1097 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/footer-facebook.png
+-rw-r--r--   0 root         (0) root         (0)     1119 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/footer-linkedin-hover.png
+-rw-r--r--   0 root         (0) root         (0)     1144 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/footer-linkedin.png
+-rw-r--r--   0 root         (0) root         (0)     1277 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/footer-twitter-hover.png
+-rw-r--r--   0 root         (0) root         (0)     1280 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/footer-twitter.png
+-rw-r--r--   0 root         (0) root         (0)     1045 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/footer-youtube-hover.png
+-rw-r--r--   0 root         (0) root         (0)     1209 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/footer-youtube.png
+-rw-r--r--   0 root         (0) root         (0)      729 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/loading.gif
+-rw-r--r--   0 root         (0) root         (0)      751 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/logo-full.png
+-rw-r--r--   0 root         (0) root         (0)      937 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/openstack-logo-full.png
+-rw-r--r--   0 root         (0) root         (0)      658 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/openstack-logo-vert.png
+-rw-r--r--   0 root         (0) root         (0)      278 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/search-icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:57.033336 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/js/
+-rw-r--r--   0 root         (0) root         (0)    69707 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/js/bootstrap.js
+-rw-r--r--   0 root         (0) root         (0)    37045 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/js/bootstrap.min.js
+-rw-r--r--   0 root         (0) root         (0)     4175 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/js/docs.js
+-rw-r--r--   0 root         (0) root         (0)   268039 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/js/jquery-3.2.1.js
+-rw-r--r--   0 root         (0) root         (0)    86659 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/js/jquery-3.2.1.min.js
+-rw-r--r--   0 root         (0) root         (0)     1887 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/js/navigation.js
+-rw-r--r--   0 root         (0) root         (0)    20621 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/js/webui-popover.js
+-rw-r--r--   0 root         (0) root         (0)      275 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/package.json
+-rw-r--r--   0 root         (0) root         (0)      157 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/swiftype_search.html
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/swiftype_search_install.html
+-rw-r--r--   0 root         (0) root         (0)      130 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/swiftype_search_mobile.html
+-rw-r--r--   0 root         (0) root         (0)      293 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/theme.conf
+-rw-r--r--   0 root         (0) root         (0)      900 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/titlerow.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:57.034336 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs_pdf/
+-rw-r--r--   0 root         (0) root         (0)      766 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs_pdf/deutsche-telekom-logo.png
+-rw-r--r--   0 root         (0) root         (0)     1253 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs_pdf/pdftheme.sty
+-rw-r--r--   0 root         (0) root         (0)      648 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/otcdocstheme/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:56.994335 otcdocstheme-0.9.0/otcdocstheme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1667 2022-01-27 17:01:56.000000 otcdocstheme-0.9.0/otcdocstheme.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5612 2022-01-27 17:01:56.000000 otcdocstheme-0.9.0/otcdocstheme.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-27 17:01:56.000000 otcdocstheme-0.9.0/otcdocstheme.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-01-27 17:01:56.000000 otcdocstheme-0.9.0/otcdocstheme.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2022-01-27 17:01:56.000000 otcdocstheme-0.9.0/otcdocstheme.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       35 2022-01-27 17:01:56.000000 otcdocstheme-0.9.0/otcdocstheme.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-01-27 17:01:56.000000 otcdocstheme-0.9.0/otcdocstheme.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:56.976335 otcdocstheme-0.9.0/releasenotes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:57.037336 otcdocstheme-0.9.0/releasenotes/notes/
+-rw-r--r--   0 root         (0) root         (0)       76 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/releasenotes/notes/add-project-links-ff3e9377417a5c10.yaml
+-rw-r--r--   0 root         (0) root         (0)       99 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/releasenotes/notes/change-root-link-5e6eb70fb869ac12.yaml
+-rw-r--r--   0 root         (0) root         (0)      102 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/releasenotes/notes/drop-google-01017fb959b908a7.yaml
+-rw-r--r--   0 root         (0) root         (0)       82 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/releasenotes/notes/fix-api-ref-df2269c9ad560c6b.yaml
+-rw-r--r--   0 root         (0) root         (0)       58 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/releasenotes/notes/fix-bug-tracker-260f8de5be2a849e.yaml
+-rw-r--r--   0 root         (0) root         (0)      142 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/releasenotes/notes/fix-sphinx4-ee98168de2714190.yaml
+-rw-r--r--   0 root         (0) root         (0)       65 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/releasenotes/notes/fix-table-09c4e5eaf38be8c0.yaml
+-rw-r--r--   0 root         (0) root         (0)      227 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/releasenotes/notes/new-theme-4c62220ee9492289.yaml
+-rw-r--r--   0 root         (0) root         (0)       79 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/releasenotes/notes/sync-with-openstack-87c6854f3bc4f180.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:57.037336 otcdocstheme-0.9.0/releasenotes/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:57.038336 otcdocstheme-0.9.0/releasenotes/source/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/releasenotes/source/_static/.placeholder
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-27 17:01:57.038336 otcdocstheme-0.9.0/releasenotes/source/_templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/releasenotes/source/_templates/.placeholder
+-rw-r--r--   0 root         (0) root         (0)     8797 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/releasenotes/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)      146 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/releasenotes/source/index.rst
+-rw-r--r--   0 root         (0) root         (0)      272 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      836 2022-01-27 17:01:57.038336 otcdocstheme-0.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      766 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      343 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/test-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1848 2022-01-27 16:56:15.000000 otcdocstheme-0.9.0/tox.ini
```

### Comparing `otcdocstheme-0.8.1/.pre-commit-config.yaml` & `otcdocstheme-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/ChangeLog` & `otcdocstheme-0.9.0/ChangeLog`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+0.9.0
+-----
+
+* Fix pdf generation (#25)
+
 0.8.1
 -----
 
 * change width of content (#23)
 
 0.8.0
 -----
```

### Comparing `otcdocstheme-0.8.1/LICENSE` & `otcdocstheme-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/Makefile` & `otcdocstheme-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/PKG-INFO` & `otcdocstheme-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: otcdocstheme
-Version: 0.8.1
+Version: 0.9.0
 Summary: OpenTelekomCloud Docs Theme
 Home-page: https://cloud.otc.com
 Author: Artem Goncharov
 Author-email: artem.goncharov@gmail.com
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `otcdocstheme-0.8.1/README.rst` & `otcdocstheme-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/api-ref/source/conf.py` & `otcdocstheme-0.9.0/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/api-ref/source/image.inc` & `otcdocstheme-0.9.0/api-ref/source/image.inc`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/api-ref/source/parameters.yaml` & `otcdocstheme-0.9.0/api-ref/source/parameters.yaml`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/api-ref/source/service.inc` & `otcdocstheme-0.9.0/api-ref/source/service.inc`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/bin/docstheme-build-pdf` & `otcdocstheme-0.9.0/bin/docstheme-build-pdf`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/bindep.txt` & `otcdocstheme-0.9.0/bindep.txt`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/doc/source/conf.py` & `otcdocstheme-0.9.0/doc/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,10 +55,10 @@
 
 # -- Options for LaTeX output ---------------------------------------------
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-  ('index', 'os-doc-demo.tex', u'os-doc-demo Documentation',
+  ('index', 'doc-otcdocstheme.tex', u'Open Telekom Cloud Theme  Documentation',
    u'OpenTelekomCloud Contributors', 'manual'),
 ]
```

### Comparing `otcdocstheme-0.8.1/doc/source/demo/configure_access_and_security_for_instances.rst` & `otcdocstheme-0.9.0/doc/source/demo/configure_access_and_security_for_instances.rst`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/doc/source/demo/create_and_manage_databases.rst` & `otcdocstheme-0.9.0/doc/source/demo/create_and_manage_databases.rst`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/doc/source/demo/create_and_manage_networks.rst` & `otcdocstheme-0.9.0/doc/source/demo/create_and_manage_networks.rst`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/doc/source/demo/dashboard_demo.rst` & `otcdocstheme-0.9.0/doc/source/demo/dashboard_demo.rst`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/doc/source/demo/figures/dashboard-project-tab.png` & `otcdocstheme-0.9.0/doc/source/demo/figures/dashboard-project-tab.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/doc/source/demo/figures/dashboard_admin_project_tab.png` & `otcdocstheme-0.9.0/doc/source/demo/figures/dashboard_admin_project_tab.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/doc/source/demo/figures/doc-logo-fox.jpg` & `otcdocstheme-0.9.0/doc/source/demo/figures/doc-logo-fox.jpg`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/doc/source/demo/index.rst` & `otcdocstheme-0.9.0/doc/source/demo/index.rst`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/doc/source/demo/launch-instance.rst` & `otcdocstheme-0.9.0/doc/source/demo/launch-instance.rst`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/doc/source/demo/section_dashboard_access_and_security.rst` & `otcdocstheme-0.9.0/doc/source/demo/section_dashboard_access_and_security.rst`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/doc/source/index.rst` & `otcdocstheme-0.9.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/__init__.py` & `otcdocstheme-0.9.0/otcdocstheme/__init__.py`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/ext.py` & `otcdocstheme-0.9.0/otcdocstheme/ext.py`

 * *Files 3% similar despite different names*

```diff
@@ -400,25 +400,31 @@
     }
 
     if app.config.latex_elements:
         latex_elements.update(app.config.latex_elements)
 
     preamble = textwrap.dedent(
         r"""
-        \usepackage{%s}
-        \\newcommand{\openstacklogo}{%s}
+        \input{%s.sty}
+        \newcommand{\otclogo}{%s}
         """
     ) % (pdf_theme_path, theme_logo)
 
     if 'preamble' in latex_elements:
         preamble += latex_elements['preamble']
 
     latex_elements['preamble'] = preamble
 
     app.config.latex_elements = latex_elements
+    app.config.latex_additional_files = [f'{pdf_theme_path}.sty']
+
+    # This hook is invoked when latex builder is already initialized. We loose
+    # preamble if we only set it to the config
+    if hasattr(app.builder, 'context') and 'preamble' in app.builder.context:
+        app.builder.context['preamble'] = preamble
 
 
 def setup(app):
     logger.info(
         '[otcdocstheme] version: %s',
         version.version_info.version_string(),
     )
```

### Comparing `otcdocstheme-0.8.1/otcdocstheme/page_context.py` & `otcdocstheme-0.9.0/otcdocstheme/page_context.py`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/paths.py` & `otcdocstheme-0.9.0/otcdocstheme/paths.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,9 +28,9 @@
     """Return the directory containing PDF theme for local builds."""
     args = ['theme', 'otcdocs_pdf', 'pdftheme']
     return os.path.join(get_pkg_path(), *args)
 
 
 def get_theme_logo_path(theme='otcdocs'):
     """Return the directory containing theme logo for local builds."""
-    args = ['theme', theme + '_pdf', 'logo-full.png']
+    args = ['theme', theme + '_pdf', 'deutsche-telekom-logo.png']
     return os.path.join(get_pkg_path(), *args)
```

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/css.html` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/css.html`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/footer.html` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/footer.html`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/header.html` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/header.html`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/layout.html` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/layout.html`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/script_footer.html` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/script_footer.html`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/search.html` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/search.html`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/sidebartoc.html` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/sidebartoc.html`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/css/bootstrap.css` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/css/bootstrap.min.css` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/css/combined.css` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/css/combined.css`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/css/font-awesome.css` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/css/font-awesome.min.css` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/css/otcdocstheme.css` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/css/otcdocstheme.css`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/favicon.ico` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/FontAwesome.otf` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.eot` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.svg` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.ttf` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.woff` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.woff2` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.eot` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.svg` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.ttf` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.woff` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.woff2` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/deutsche-telekom-logo.svg` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/deutsche-telekom-logo.svg`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/docs/license.png` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/docs/license.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/docs/superuser1.png` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/docs/superuser1.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/docs/superuser2.png` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/docs/superuser2.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/docs/superuser3.png` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/docs/superuser3.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/docs/superuser4.png` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/docs/superuser4.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/footer-facebook-hover.png` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/footer-facebook-hover.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/footer-facebook.png` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/footer-facebook.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/footer-linkedin-hover.png` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/footer-linkedin-hover.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/footer-linkedin.png` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/footer-linkedin.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/footer-twitter-hover.png` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/footer-twitter-hover.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/footer-twitter.png` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/footer-twitter.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/footer-youtube-hover.png` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/footer-youtube-hover.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/footer-youtube.png` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/footer-youtube.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/loading.gif` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/loading.gif`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/logo-full.png` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/logo-full.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/openstack-logo-full.png` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/openstack-logo-full.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/images/openstack-logo-vert.png` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/images/openstack-logo-vert.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/js/bootstrap.js` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/js/bootstrap.min.js` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/js/docs.js` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/js/docs.js`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/js/jquery-3.2.1.js` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/js/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/js/jquery-3.2.1.min.js` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/js/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/js/navigation.js` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/js/navigation.js`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/static/js/webui-popover.js` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/static/js/webui-popover.js`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs/titlerow.html` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs/titlerow.html`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs_pdf/deutsche-telekom-logo.png` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs_pdf/deutsche-telekom-logo.png`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme/theme/otcdocs_pdf/pdftheme.sty` & `otcdocstheme-0.9.0/otcdocstheme/theme/otcdocs_pdf/pdftheme.sty`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,11 @@
 \makeatletter
 
-% Do not print release information if empty
-% Note: Sphinx does support version variable in conf.py to latex yet
-\def \ifempty#1{\def\temp{#1} \ifx\temp\empty }
-\renewcommand{\release}[1]{
-   \ifempty{#1}
-     \newcommand{\osreleasetitle}{}
-     \newcommand{\osreleaseheader}{}
-   \else
-     \newcommand{\osreleasetitle}{\LARGE Release Version: #1\newline}
-     \newcommand{\osreleaseheader}{\space\small\nouppercase{(Release Version: #1)}}
-   \fi
-}
-
 \usepackage[multidot]{grffile}
+\usepackage{longtable}
 
 % Defines title page
 \renewcommand{\maketitle}{
   \begin{titlepage}
     \begin{flushleft}
        \includegraphics[width=1.6cm, height=0.8cm]{\otclogo}
     \end{flushleft}
@@ -47,23 +35,20 @@
 }
 
 % Customizes page header & footer for otc
 \fancypagestyle{normal}{
   \fancyhf{}
   \fancyfoot[LE,RO]{{\py@HeaderFamily\thepage}}
   \fancyfoot[RE,LO]{{\py@HeaderFamily\nouppercase\rightmark}}
-  \fancyhead[LE,RO]{{\py@HeaderFamily\@title\osreleaseheader}}
+  \fancyhead[LE,RO]{{\py@HeaderFamily\@title}}
   \fancyhead[RE,LO]{{\py@HeaderFamily\includegraphics[width=1.6cm, height=0.8cm]{\otclogo}}}
 }
 
 % Customizes colors
 \definecolor{VerbatimColor}{rgb}{.95,.95,.95}
 
 % Do not use chapter and section number
 \setcounter{secnumdepth}{-1}
 
 % Font selection (English)
 \usepackage{fontspec}
 \defaultfontfeatures{Scale=MatchLowercase}
-\setmainfont{Liberation Serif}
-\setsansfont{Liberation Sans}
-\setmonofont[SmallCapsFont={Liberation Mono}]{Liberation Mono}
```

### Comparing `otcdocstheme-0.8.1/otcdocstheme/version.py` & `otcdocstheme-0.9.0/otcdocstheme/version.py`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/otcdocstheme.egg-info/PKG-INFO` & `otcdocstheme-0.9.0/otcdocstheme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: otcdocstheme
-Version: 0.8.1
+Version: 0.9.0
 Summary: OpenTelekomCloud Docs Theme
 Home-page: https://cloud.otc.com
 Author: Artem Goncharov
 Author-email: artem.goncharov@gmail.com
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `otcdocstheme-0.8.1/otcdocstheme.egg-info/SOURCES.txt` & `otcdocstheme-0.9.0/otcdocstheme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/releasenotes/source/conf.py` & `otcdocstheme-0.9.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/setup.cfg` & `otcdocstheme-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/setup.py` & `otcdocstheme-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `otcdocstheme-0.8.1/tox.ini` & `otcdocstheme-0.9.0/tox.ini`

 * *Files identical despite different names*

