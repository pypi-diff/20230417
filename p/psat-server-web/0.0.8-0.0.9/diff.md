# Comparing `tmp/psat-server-web-0.0.8.tar.gz` & `tmp/psat-server-web-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/psat-server-web-0.0.8.tar", last modified: Thu May 20 22:04:35 2021, max compression
+gzip compressed data, was "dist/psat-server-web-0.0.9.tar", last modified: Thu May 20 22:55:55 2021, max compression
```

## Comparing `psat-server-web-0.0.8.tar` & `psat-server-web-0.0.9.tar`

### file list

```diff
@@ -1,397 +1,397 @@
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:35.336604 psat-server-web-0.0.8/
--rw-r--r--   0 kws        (502) staff       (20)      228 2021-05-20 00:05:16.000000 psat-server-web-0.0.8/MANIFEST.in
--rw-r--r--   0 kws        (502) staff       (20)      594 2021-05-20 22:04:35.336196 psat-server-web-0.0.8/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)       79 2021-03-09 12:47:41.000000 psat-server-web-0.0.8/README.md
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.836628 psat-server-web-0.0.8/psat_server_web/
--rw-r--r--   0 kws        (502) staff       (20)       38 2021-05-15 13:54:02.000000 psat-server-web-0.0.8/psat_server_web/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       22 2021-05-20 22:03:54.000000 psat-server-web-0.0.8/psat_server_web/__version__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.840640 psat-server-web-0.0.8/psat_server_web/atlas/
--rw-r--r--   0 kws        (502) staff       (20)        0 2021-05-15 12:47:24.000000 psat-server-web-0.0.8/psat_server_web/atlas/__init__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.850432 psat-server-web-0.0.8/psat_server_web/atlas/atlas/
--rw-r--r--   0 kws        (502) staff       (20)        0 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/atlas/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)    41196 2021-03-11 18:42:36.000000 psat-server-web-0.0.8/psat_server_web/atlas/atlas/commonqueries.py
--rw-r--r--   0 kws        (502) staff       (20)    17570 2021-05-05 20:09:40.000000 psat-server-web-0.0.8/psat_server_web/atlas/atlas/dbviews.py
--rw-r--r--   0 kws        (502) staff       (20)      379 2021-03-09 14:56:31.000000 psat-server-web-0.0.8/psat_server_web/atlas/atlas/document.sh
--rw-r--r--   0 kws        (502) staff       (20)     5959 2021-05-13 00:15:35.000000 psat-server-web-0.0.8/psat_server_web/atlas/atlas/formchoices.py
--rw-r--r--   0 kws        (502) staff       (20)    13331 2021-05-14 12:21:06.000000 psat-server-web-0.0.8/psat_server_web/atlas/atlas/helpers.py
--rw-r--r--   0 kws        (502) staff       (20)    29140 2021-03-09 14:56:37.000000 psat-server-web-0.0.8/psat_server_web/atlas/atlas/lightcurvequeries.py
--rw-r--r--   0 kws        (502) staff       (20)    43611 2021-05-05 19:59:34.000000 psat-server-web-0.0.8/psat_server_web/atlas/atlas/models.py
--rw-r--r--   0 kws        (502) staff       (20)     5162 2021-05-20 22:01:48.000000 psat-server-web-0.0.8/psat_server_web/atlas/atlas/settings.py
--rw-r--r--   0 kws        (502) staff       (20)     5390 2021-03-11 00:41:45.000000 psat-server-web-0.0.8/psat_server_web/atlas/atlas/sqlpaginator.py
--rw-r--r--   0 kws        (502) staff       (20)     4310 2021-05-07 00:15:44.000000 psat-server-web-0.0.8/psat_server_web/atlas/atlas/urls.py
--rw-r--r--   0 kws        (502) staff       (20)   163293 2021-05-20 22:00:55.000000 psat-server-web-0.0.8/psat_server_web/atlas/atlas/views.py
--rw-r--r--   0 kws        (502) staff       (20)     1165 2021-03-10 22:48:56.000000 psat-server-web-0.0.8/psat_server_web/atlas/atlas/wsgi.atlas.conf
--rw-r--r--   0 kws        (502) staff       (20)      329 2021-05-05 21:27:19.000000 psat-server-web-0.0.8/psat_server_web/atlas/atlas/wsgi.py
--rw-r--r--   0 kws        (502) staff       (20)      945 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/atlas/wsgi_apache_example.conf
--rwxr-xr-x   0 kws        (502) staff       (20)     1836 2021-05-20 15:50:55.000000 psat-server-web-0.0.8/psat_server_web/atlas/generate_mod_wsgi_apachectl.sh
--rwxr-xr-x   0 kws        (502) staff       (20)      248 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/manage.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.828338 psat-server-web-0.0.8/psat_server_web/atlas/media/
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.851030 psat-server-web-0.0.8/psat_server_web/atlas/media/images/
--rw-r--r--   0 kws        (502) staff       (20)       81 2021-05-15 10:03:26.000000 psat-server-web-0.0.8/psat_server_web/atlas/media/images/README.txt
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.829149 psat-server-web-0.0.8/psat_server_web/atlas/site_media/
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.853454 psat-server-web-0.0.8/psat_server_web/atlas/site_media/css/
--rw-r--r--   0 kws        (502) staff       (20)    15810 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/css/aladin.css
--rw-r--r--   0 kws        (502) staff       (20)     6501 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/css/celestial.css
--rw-r--r--   0 kws        (502) staff       (20)    13715 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/css/main.css
--rw-r--r--   0 kws        (502) staff       (20)     3383 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/css/main_bootstrap.css
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.855176 psat-server-web-0.0.8/psat_server_web/atlas/site_media/images/
--rw-r--r--   0 kws        (502) staff       (20)   163712 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/images/atlas_logo.png
--rw-r--r--   0 kws        (502) staff       (20)    14986 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/images/image_not_available.jpeg
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.891099 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/
--rw-r--r--   0 kws        (502) staff       (20)   455297 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/aladin.js
--rw-r--r--   0 kws        (502) staff       (20)     1620 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/bootstrap_utils.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.896592 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/
--rw-r--r--   0 kws        (502) staff       (20)   160860 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/celestial.js
--rw-r--r--   0 kws        (502) staff       (20)    90592 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/d3.geo.projection.js
--rw-r--r--   0 kws        (502) staff       (20)    46780 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/d3.geo.projection.min.js
--rw-r--r--   0 kws        (502) staff       (20)     8471 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/d3.geo.zoom.js
--rw-r--r--   0 kws        (502) staff       (20)   151732 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/d3.min.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.904936 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/
--rw-r--r--   0 kws        (502) staff       (20)        0 2021-05-14 23:13:00.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)    39824 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/constellations.bounds.json
--rw-r--r--   0 kws        (502) staff       (20)    19510 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/constellations.json
--rw-r--r--   0 kws        (502) staff       (20)    26254 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/constellations.lines.json
--rw-r--r--   0 kws        (502) staff       (20)     7398 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/dsos.bright.json
--rw-r--r--   0 kws        (502) staff       (20)    61574 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/lg.json
--rw-r--r--   0 kws        (502) staff       (20)   534254 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/mw.json
--rw-r--r--   0 kws        (502) staff       (20)     3884 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/planets.json
--rw-r--r--   0 kws        (502) staff       (20)   759360 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/stars.6.json
--rw-r--r--   0 kws        (502) staff       (20)     9941 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/colourplot.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.916744 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/
--rw-r--r--   0 kws        (502) staff       (20)    41784 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/excanvas.js
--rw-r--r--   0 kws        (502) staff       (20)   252881 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery-1.7.2.js
--rw-r--r--   0 kws        (502) staff       (20)    17407 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.axislabels.js
--rw-r--r--   0 kws        (502) staff       (20)     5191 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.crosshair.js
--rw-r--r--   0 kws        (502) staff       (20)    12389 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.errorbars.js
--rw-r--r--   0 kws        (502) staff       (20)     6771 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.fillbetween.js
--rw-r--r--   0 kws        (502) staff       (20)     7351 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.image.js
--rw-r--r--   0 kws        (502) staff       (20)   106797 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.js
--rw-r--r--   0 kws        (502) staff       (20)    13634 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.navigate.js
--rw-r--r--   0 kws        (502) staff       (20)    22589 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.pie.js
--rw-r--r--   0 kws        (502) staff       (20)     2458 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.resize.js
--rw-r--r--   0 kws        (502) staff       (20)    12018 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.selection.js
--rw-r--r--   0 kws        (502) staff       (20)     6968 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.stack.js
--rw-r--r--   0 kws        (502) staff       (20)     2441 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.symbol.js
--rw-r--r--   0 kws        (502) staff       (20)     3291 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.threshold.js
--rw-r--r--   0 kws        (502) staff       (20)     2709 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/followup_selectall.js
--rw-r--r--   0 kws        (502) staff       (20)    10907 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/lightcurve.js
--rw-r--r--   0 kws        (502) staff       (20)     8349 2021-03-09 13:34:59.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/lightcurveplotly.js
--rw-r--r--   0 kws        (502) staff       (20)     5637 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/mjdcalc.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.917204 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/plotly/
--rw-r--r--   0 kws        (502) staff       (20)  5856350 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/plotly/plotly-latest.kws.js
--rw-r--r--   0 kws        (502) staff       (20)     7661 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/recurrenceplot.js
--rw-r--r--   0 kws        (502) staff       (20)     7430 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/recurrenceplotplotly.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.928051 psat-server-web-0.0.8/psat_server_web/atlas/sql/
--rw-r--r--   0 kws        (502) staff       (20)    16485 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/sql/create_web_views.sql
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.939257 psat-server-web-0.0.8/psat_server_web/atlas/templates/
--rw-r--r--   0 kws        (502) staff       (20)      448 2021-05-20 10:54:42.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/400.html
--rw-r--r--   0 kws        (502) staff       (20)      435 2021-05-20 10:37:36.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/403.html
--rw-r--r--   0 kws        (502) staff       (20)      446 2021-05-20 08:49:19.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/404.html
--rw-r--r--   0 kws        (502) staff       (20)      465 2021-05-20 10:56:58.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/500.html
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.977972 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/
--rw-r--r--   0 kws        (502) staff       (20)     3700 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/atelfasttrackobject.txt
--rw-r--r--   0 kws        (502) staff       (20)     1276 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/atelsdiscovery.txt
--rw-r--r--   0 kws        (502) staff       (20)     5724 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/atelsfast.txt
--rw-r--r--   0 kws        (502) staff       (20)    40683 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/candidate.html
--rw-r--r--   0 kws        (502) staff       (20)    36872 2021-05-07 00:28:04.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/candidate_plotly.html
--rw-r--r--   0 kws        (502) staff       (20)     3246 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/crossmatch_external.html
--rw-r--r--   0 kws        (502) staff       (20)      462 2021-03-09 13:34:59.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/error.html
--rw-r--r--   0 kws        (502) staff       (20)     2080 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/followup.html
--rw-r--r--   0 kws        (502) staff       (20)      761 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/followup.txt
--rw-r--r--   0 kws        (502) staff       (20)     2414 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/followup2.html
--rw-r--r--   0 kws        (502) staff       (20)      657 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/followup_bs.html
--rw-r--r--   0 kws        (502) staff       (20)     3227 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/followup_bypass_django_tables.html
--rw-r--r--   0 kws        (502) staff       (20)    12788 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/followup_quickview.html
--rw-r--r--   0 kws        (502) staff       (20)     1012 2021-05-14 12:15:07.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/followup_quickview_bs.html
--rw-r--r--   0 kws        (502) staff       (20)      570 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/followup_subset.txt
--rw-r--r--   0 kws        (502) staff       (20)     2765 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/index.html
--rw-r--r--   0 kws        (502) staff       (20)     1527 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/index_bs.html
--rw-r--r--   0 kws        (502) staff       (20)     7243 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/index_bs_celestial.html
--rw-r--r--   0 kws        (502) staff       (20)      169 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/iobserve.txt
--rw-r--r--   0 kws        (502) staff       (20)      557 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/lightcurve.txt
--rw-r--r--   0 kws        (502) staff       (20)      625 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/lightcurveddc.txt
--rw-r--r--   0 kws        (502) staff       (20)      821 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/lightcurveforced.txt
--rw-r--r--   0 kws        (502) staff       (20)      445 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/pesstorecurrences.txt
--rw-r--r--   0 kws        (502) staff       (20)      294 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/pesstorecurrencesddc.txt
--rw-r--r--   0 kws        (502) staff       (20)      725 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/pesstosummary.txt
--rw-r--r--   0 kws        (502) staff       (20)     6942 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/search_results.html
--rw-r--r--   0 kws        (502) staff       (20)    21043 2021-05-14 12:38:16.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/search_results_plotly.html
--rw-r--r--   0 kws        (502) staff       (20)       19 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/sne.json
--rw-r--r--   0 kws        (502) staff       (20)      626 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/summary.csv
--rw-r--r--   0 kws        (502) staff       (20)     2058 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/userdefinedlists.html
--rw-r--r--   0 kws        (502) staff       (20)      538 2021-05-10 19:49:10.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/userdefinedlists_bs.html
--rw-r--r--   0 kws        (502) staff       (20)      176 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/visibility.txt
--rw-r--r--   0 kws        (502) staff       (20)     1006 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/base.html
--rw-r--r--   0 kws        (502) staff       (20)     7304 2021-05-19 13:31:33.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/base_bootstrap.html
--rw-r--r--   0 kws        (502) staff       (20)     2343 2021-05-19 19:17:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/base_bootstrap_login.html
--rw-r--r--   0 kws        (502) staff       (20)     6107 2021-05-14 16:01:35.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/bootstrap4_django_tables2_atlas.html
--rw-r--r--   0 kws        (502) staff       (20)      501 2021-05-19 21:12:44.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/invalid_login.html
--rw-r--r--   0 kws        (502) staff       (20)      355 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/loggedin.html
--rw-r--r--   0 kws        (502) staff       (20)      937 2021-05-19 21:36:39.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/login.html
--rw-r--r--   0 kws        (502) staff       (20)      428 2021-05-19 21:12:06.000000 psat-server-web-0.0.8/psat_server_web/atlas/templates/logout.html
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.978512 psat-server-web-0.0.8/psat_server_web/config/
--rw-r--r--   0 kws        (502) staff       (20)      770 2020-10-02 22:40:04.000000 psat-server-web-0.0.8/psat_server_web/config/wsgi.conf.template
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.980121 psat-server-web-0.0.8/psat_server_web/ps1/
--rw-r--r--   0 kws        (502) staff       (20)        0 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)     1890 2021-03-09 14:51:15.000000 psat-server-web-0.0.8/psat_server_web/ps1/createUsers.py
--rwxr-xr-x   0 kws        (502) staff       (20)      247 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/manage.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.991720 psat-server-web-0.0.8/psat_server_web/ps1/psdb/
--rw-r--r--   0 kws        (502) staff       (20)        0 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/psdb/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)      697 2021-03-09 14:54:01.000000 psat-server-web-0.0.8/psat_server_web/ps1/psdb/admin.py
--rw-r--r--   0 kws        (502) staff       (20)     7516 2021-03-09 14:54:02.000000 psat-server-web-0.0.8/psat_server_web/ps1/psdb/catalogueviews.py
--rw-r--r--   0 kws        (502) staff       (20)    42272 2021-03-09 14:54:02.000000 psat-server-web-0.0.8/psat_server_web/ps1/psdb/commonqueries.py
--rw-r--r--   0 kws        (502) staff       (20)    34040 2021-03-11 12:13:25.000000 psat-server-web-0.0.8/psat_server_web/ps1/psdb/dbviews.py
--rw-r--r--   0 kws        (502) staff       (20)     4871 2021-03-09 13:30:11.000000 psat-server-web-0.0.8/psat_server_web/ps1/psdb/formchoices.py
--rw-r--r--   0 kws        (502) staff       (20)     9899 2021-03-09 14:54:02.000000 psat-server-web-0.0.8/psat_server_web/ps1/psdb/helpers.py
--rw-r--r--   0 kws        (502) staff       (20)    15791 2021-03-09 14:35:48.000000 psat-server-web-0.0.8/psat_server_web/ps1/psdb/img_scale.py
--rw-r--r--   0 kws        (502) staff       (20)    18778 2021-03-09 14:54:03.000000 psat-server-web-0.0.8/psat_server_web/ps1/psdb/lightcurvequeries.py
--rw-r--r--   0 kws        (502) staff       (20)    43644 2021-03-11 12:13:00.000000 psat-server-web-0.0.8/psat_server_web/ps1/psdb/models.py
--rw-r--r--   0 kws        (502) staff       (20)     5837 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/psdb/settings.py.template
--rw-r--r--   0 kws        (502) staff       (20)     4007 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/psdb/urls.py
--rw-r--r--   0 kws        (502) staff       (20)    99285 2021-03-09 14:54:03.000000 psat-server-web-0.0.8/psat_server_web/ps1/psdb/views.py
--rw-r--r--   0 kws        (502) staff       (20)      280 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/psdb/wsgi.py.template
--rw-r--r--   0 kws        (502) staff       (20)      893 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/psdb/wsgi_apache_example.conf
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.832190 psat-server-web-0.0.8/psat_server_web/ps1/site_media/
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.993663 psat-server-web-0.0.8/psat_server_web/ps1/site_media/css/
--rw-r--r--   0 kws        (502) staff       (20)    15810 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/css/aladin.css
--rw-r--r--   0 kws        (502) staff       (20)     6501 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/css/celestial.css
--rw-r--r--   0 kws        (502) staff       (20)    13430 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/css/main.css
--rw-r--r--   0 kws        (502) staff       (20)     3479 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/css/main_bootstrap.css
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:35.085469 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/
--rw-r--r--   0 kws        (502) staff       (20)    35860 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/1-star-hover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    22130 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/1-star.jpg
--rw-r--r--   0 kws        (502) staff       (20)    36051 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/2-star-hover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    27068 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/2-star.jpg
--rw-r--r--   0 kws        (502) staff       (20)    36308 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/3-star-hover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    31801 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/3-star.jpg
--rw-r--r--   0 kws        (502) staff       (20)     2610 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/aladin.gif
--rw-r--r--   0 kws        (502) staff       (20)    58676 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/cfaIcon.jpg
--rw-r--r--   0 kws        (502) staff       (20)    61573 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/cfaIconHover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    21821 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/confirmed-sne-hover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    23630 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/confirmed-sne.jpg
--rw-r--r--   0 kws        (502) staff       (20)    57933 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/detection_example.jpg
--rwxr-xr-x   0 kws        (502) staff       (20)      465 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/down.jpeg
--rw-r--r--   0 kws        (502) staff       (20)     6659 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/down.jpg
--rw-r--r--   0 kws        (502) staff       (20)    14986 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/image_not_available.jpeg
--rw-r--r--   0 kws        (502) staff       (20)    36417 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/jhuIcon.jpg
--rw-r--r--   0 kws        (502) staff       (20)    38864 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/jhuIconHover.jpg
--rw-r--r--   0 kws        (502) staff       (20)     7928 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/minus.jpg
--rw-r--r--   0 kws        (502) staff       (20)    44343 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/ncuIcon.jpg
--rw-r--r--   0 kws        (502) staff       (20)    46130 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/ncuIconHover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    58496 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/non_detection_example.jpg
--rw-r--r--   0 kws        (502) staff       (20)     8506 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/others-hover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    11289 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/others.jpg
--rw-r--r--   0 kws        (502) staff       (20)    25306 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/panstarrs-logo-hover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    21877 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/panstarrs-logo.jpg
--rw-r--r--   0 kws        (502) staff       (20)    74999 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/panstarrs1_logo.jpg
--rw-r--r--   0 kws        (502) staff       (20)    85348 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/panstarrs1_o3_logo.jpg
--rw-r--r--   0 kws        (502) staff       (20)    76781 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/panstarrs2_logo.jpg
--rw-r--r--   0 kws        (502) staff       (20)    86931 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/panstarrs2_o3_logo.jpg
--rw-r--r--   0 kws        (502) staff       (20)    95536 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/panstarrs_logo.jpg
--rw-r--r--   0 kws        (502) staff       (20)    48452 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/pittsIcon.jpg
--rw-r--r--   0 kws        (502) staff       (20)    50248 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/pittsIconHover.jpg
--rw-r--r--   0 kws        (502) staff       (20)     7740 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/plus.jpg
--rw-r--r--   0 kws        (502) staff       (20)    47509 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/ps1Icon.jpg
--rw-r--r--   0 kws        (502) staff       (20)    45155 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/ps1IconHover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    12609 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/ps1sc.gif
--rw-r--r--   0 kws        (502) staff       (20)    30826 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/qub-logo-hover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    26675 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/qub-logo.jpg
--rw-r--r--   0 kws        (502) staff       (20)    37401 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/qubIcon.jpg
--rw-r--r--   0 kws        (502) staff       (20)    38167 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/qubIconHover.jpg
--rw-r--r--   0 kws        (502) staff       (20)     1493 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/sdss.gif
--rw-r--r--   0 kws        (502) staff       (20)    15197 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/table-background.jpg
--rw-r--r--   0 kws        (502) staff       (20)     1524 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/table-bottom-left.jpg
--rw-r--r--   0 kws        (502) staff       (20)     1551 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/table-bottom-right.jpg
--rw-r--r--   0 kws        (502) staff       (20)     1272 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/table-row.jpg
--rw-r--r--   0 kws        (502) staff       (20)     1442 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/table-top-left.jpg
--rw-r--r--   0 kws        (502) staff       (20)     1549 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/table-top-right.jpg
--rw-r--r--   0 kws        (502) staff       (20)    41765 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/uhifaIcon.jpg
--rw-r--r--   0 kws        (502) staff       (20)    44162 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/uhifaIconHover.jpg
--rw-r--r--   0 kws        (502) staff       (20)      473 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/up.jpeg
--rw-r--r--   0 kws        (502) staff       (20)     6445 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/up.jpg
--rw-r--r--   0 kws        (502) staff       (20)    14173 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/variable-stars-hover.jpg
--rw-r--r--   0 kws        (502) staff       (20)    16952 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/variable-stars.jpg
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:35.091642 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/
--rw-r--r--   0 kws        (502) staff       (20)   455297 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/aladin.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:35.094550 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/
--rw-r--r--   0 kws        (502) staff       (20)   160860 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/celestial.js
--rw-r--r--   0 kws        (502) staff       (20)    90592 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/d3.geo.projection.js
--rw-r--r--   0 kws        (502) staff       (20)    46780 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/d3.geo.projection.min.js
--rw-r--r--   0 kws        (502) staff       (20)     8471 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/d3.geo.zoom.js
--rw-r--r--   0 kws        (502) staff       (20)   151732 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/d3.min.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:35.099182 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/
--rw-r--r--   0 kws        (502) staff       (20)        0 2021-05-14 23:13:00.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)    39824 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/constellations.bounds.json
--rw-r--r--   0 kws        (502) staff       (20)    19510 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/constellations.json
--rw-r--r--   0 kws        (502) staff       (20)    26254 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/constellations.lines.json
--rw-r--r--   0 kws        (502) staff       (20)     7398 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/dsos.bright.json
--rw-r--r--   0 kws        (502) staff       (20)    61574 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/lg.json
--rw-r--r--   0 kws        (502) staff       (20)   534254 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/mw.json
--rw-r--r--   0 kws        (502) staff       (20)     3884 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/planets.json
--rw-r--r--   0 kws        (502) staff       (20)   759360 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/stars.6.json
--rw-r--r--   0 kws        (502) staff       (20)     9941 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/colourplot.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:35.141128 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/
--rw-r--r--   0 kws        (502) staff       (20)    41784 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/excanvas.js
--rw-r--r--   0 kws        (502) staff       (20)   252881 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery-1.7.2.js
--rw-r--r--   0 kws        (502) staff       (20)    17407 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.axislabels.js
--rw-r--r--   0 kws        (502) staff       (20)     5191 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.crosshair.js
--rw-r--r--   0 kws        (502) staff       (20)    12389 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.errorbars.js
--rw-r--r--   0 kws        (502) staff       (20)     6771 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.fillbetween.js
--rw-r--r--   0 kws        (502) staff       (20)     7351 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.image.js
--rw-r--r--   0 kws        (502) staff       (20)   106797 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.js
--rw-r--r--   0 kws        (502) staff       (20)    13634 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.navigate.js
--rw-r--r--   0 kws        (502) staff       (20)    22589 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.pie.js
--rw-r--r--   0 kws        (502) staff       (20)     2458 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.resize.js
--rw-r--r--   0 kws        (502) staff       (20)    12018 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.selection.js
--rw-r--r--   0 kws        (502) staff       (20)     6968 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.stack.js
--rw-r--r--   0 kws        (502) staff       (20)     2441 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.symbol.js
--rw-r--r--   0 kws        (502) staff       (20)     3291 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.threshold.js
--rw-r--r--   0 kws        (502) staff       (20)     1260 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/followup_selectall.js
--rw-r--r--   0 kws        (502) staff       (20)    10724 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/lightcurve.js
--rw-r--r--   0 kws        (502) staff       (20)     8308 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/lightcurveplotly.js
--rw-r--r--   0 kws        (502) staff       (20)     5859 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/mjdcalc.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:35.141605 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/plotly/
--rw-r--r--   0 kws        (502) staff       (20)  5856350 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/plotly/plotly-latest.kws.js
--rw-r--r--   0 kws        (502) staff       (20)     7661 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/recurrenceplot.js
--rw-r--r--   0 kws        (502) staff       (20)     7430 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/recurrenceplotplotly.js
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:35.153568 psat-server-web-0.0.8/psat_server_web/ps1/sql/
--rw-r--r--   0 kws        (502) staff       (20)      982 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/sql/create_web_cat_views.sql
--rw-r--r--   0 kws        (502) staff       (20)      812 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/sql/create_web_user_grants.sql
--rw-r--r--   0 kws        (502) staff       (20)    44715 2021-03-09 13:30:11.000000 psat-server-web-0.0.8/psat_server_web/ps1/sql/create_web_views.sql
--rw-r--r--   0 kws        (502) staff       (20)    13969 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/sql/create_web_views_fgss.sql
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:35.191984 psat-server-web-0.0.8/psat_server_web/ps1/templates/
--rw-r--r--   0 kws        (502) staff       (20)      193 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/404.html
--rw-r--r--   0 kws        (502) staff       (20)      368 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/500.html
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:35.192529 psat-server-web-0.0.8/psat_server_web/ps1/templates/admin/
--rw-r--r--   0 kws        (502) staff       (20)      333 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/admin/base_site.html
--rw-r--r--   0 kws        (502) staff       (20)    10344 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/base.html
--rw-r--r--   0 kws        (502) staff       (20)     7099 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/base_bootstrap.html
--rw-r--r--   0 kws        (502) staff       (20)      956 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/base_new.html
--rw-r--r--   0 kws        (502) staff       (20)      250 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/invalid_login.html
--rw-r--r--   0 kws        (502) staff       (20)      359 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/loggedin.html
--rw-r--r--   0 kws        (502) staff       (20)      771 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/login.html
--rw-r--r--   0 kws        (502) staff       (20)      197 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/logout.html
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:35.209297 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/
--rw-r--r--   0 kws        (502) staff       (20)     1173 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/atelsdiscovery.txt
--rw-r--r--   0 kws        (502) staff       (20)    18270 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/candidate.html
--rw-r--r--   0 kws        (502) staff       (20)    38886 2021-03-09 13:30:11.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/candidate_plotly.html
--rw-r--r--   0 kws        (502) staff       (20)    32828 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/candidate_quickview.html
--rw-r--r--   0 kws        (502) staff       (20)    40854 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/candidateflot.html
--rw-r--r--   0 kws        (502) staff       (20)     2215 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/candidates.html
--rw-r--r--   0 kws        (502) staff       (20)      756 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/colourdata.txt
--rw-r--r--   0 kws        (502) staff       (20)     3628 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/crossmatch_cfa_with_ipp.html
--rw-r--r--   0 kws        (502) staff       (20)     3328 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/crossmatch_external.html
--rw-r--r--   0 kws        (502) staff       (20)       17 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/dss2.html
--rw-r--r--   0 kws        (502) staff       (20)      462 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/error.html
--rw-r--r--   0 kws        (502) staff       (20)     3229 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/fasttrackastronote.txt
--rw-r--r--   0 kws        (502) staff       (20)     3731 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/followup.html
--rw-r--r--   0 kws        (502) staff       (20)      864 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/followup.txt
--rw-r--r--   0 kws        (502) staff       (20)     2873 2021-03-09 13:30:11.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/followup_bs.html
--rw-r--r--   0 kws        (502) staff       (20)    12747 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/followup_quickview.html
--rw-r--r--   0 kws        (502) staff       (20)     9846 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/followup_quickview_bs.html
--rw-r--r--   0 kws        (502) staff       (20)      702 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/gcn.txt
--rw-r--r--   0 kws        (502) staff       (20)      652 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/gcn_latex.txt
--rw-r--r--   0 kws        (502) staff       (20)     4902 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/index.html
--rw-r--r--   0 kws        (502) staff       (20)    10229 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/index_bs_celestial.html
--rw-r--r--   0 kws        (502) staff       (20)    15063 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/index_public.html
--rw-r--r--   0 kws        (502) staff       (20)      245 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/lightcurve.txt
--rw-r--r--   0 kws        (502) staff       (20)      321 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/lightcurveforced.txt
--rw-r--r--   0 kws        (502) staff       (20)     5801 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/lightcurves.html
--rw-r--r--   0 kws        (502) staff       (20)      294 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/obscat.txt
--rw-r--r--   0 kws        (502) staff       (20)     1344 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/obsmediawiki.txt
--rw-r--r--   0 kws        (502) staff       (20)     3803 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/public.html
--rw-r--r--   0 kws        (502) staff       (20)      859 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/public_textonly.txt
--rw-r--r--   0 kws        (502) staff       (20)     9225 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/reports.html
--rw-r--r--   0 kws        (502) staff       (20)     3801 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/search_results.html
--rw-r--r--   0 kws        (502) staff       (20)       19 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/sne.json
--rw-r--r--   0 kws        (502) staff       (20)     2537 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/userdefinedlists.html
--rw-r--r--   0 kws        (502) staff       (20)      875 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/userdefinedlists_bs.html
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:35.335515 psat-server-web-0.0.8/psat_server_web/schema/
--rw-r--r--   0 kws        (502) staff       (20)     2263 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/atlas_detections.sql
--rw-r--r--   0 kws        (502) staff       (20)     1731 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/atlas_detectionsddc.sql
--rw-r--r--   0 kws        (502) staff       (20)     2212 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/atlas_diff_detections.sql
--rw-r--r--   0 kws        (502) staff       (20)      652 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/atlas_diff_logs.sql
--rw-r--r--   0 kws        (502) staff       (20)     1093 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/atlas_diff_moments.sql
--rw-r--r--   0 kws        (502) staff       (20)     3319 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/atlas_diff_objects.sql
--rw-r--r--   0 kws        (502) staff       (20)      645 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/atlas_diff_subcell_logs.sql
--rw-r--r--   0 kws        (502) staff       (20)      540 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/atlas_diff_subcells.sql
--rw-r--r--   0 kws        (502) staff       (20)     1646 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/atlas_forced_photometry.sql
--rw-r--r--   0 kws        (502) staff       (20)     2928 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/atlas_metadata.sql
--rw-r--r--   0 kws        (502) staff       (20)     1400 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/atlas_metadataddc.sql
--rw-r--r--   0 kws        (502) staff       (20)     1824 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/atlas_objects.sql
--rw-r--r--   0 kws        (502) staff       (20)     1595 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/atlas_stacked_forced_photometry.sql
--rw-r--r--   0 kws        (502) staff       (20)      970 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/create_atlas_flattened_view.sql
--rw-r--r--   0 kws        (502) staff       (20)     4055 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/create_photpipe_views.sql
--rw-r--r--   0 kws        (502) staff       (20)     2641 2021-03-11 12:43:21.000000 psat-server-web-0.0.8/psat_server_web/schema/create_schema.sql
--rw-r--r--   0 kws        (502) staff       (20)     3312 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/create_user_grants.sql
--rw-r--r--   0 kws        (502) staff       (20)     1332 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/create_user_grants_generic.sql
--rw-r--r--   0 kws        (502) staff       (20)      232 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/create_user_grants_root.sql
--rw-r--r--   0 kws        (502) staff       (20)     1190 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/delete_transients.sql
--rw-r--r--   0 kws        (502) staff       (20)    60402 2021-03-10 12:07:36.000000 psat-server-web-0.0.8/psat_server_web/schema/generateATLASSchemaAndCPPClasses.py
--rw-r--r--   0 kws        (502) staff       (20)     2489 2021-03-10 12:03:01.000000 psat-server-web-0.0.8/psat_server_web/schema/get_table_columns_for_avro.py
--rw-r--r--   0 kws        (502) staff       (20)      182 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/get_table_columns_for_avro.sql
--rw-r--r--   0 kws        (502) staff       (20)      977 2021-03-10 12:32:10.000000 psat-server-web-0.0.8/psat_server_web/schema/refresh_django_views.py
--rw-r--r--   0 kws        (502) staff       (20)     4853 2021-03-10 22:44:14.000000 psat-server-web-0.0.8/psat_server_web/schema/setup_database.py
--rw-r--r--   0 kws        (502) staff       (20)    13195 2021-03-10 22:48:16.000000 psat-server-web-0.0.8/psat_server_web/schema/setup_database_utils.py
--rw-r--r--   0 kws        (502) staff       (20)      714 2021-03-09 13:30:11.000000 psat-server-web-0.0.8/psat_server_web/schema/sherlock_classifications.sql
--rw-r--r--   0 kws        (502) staff       (20)     3104 2021-03-09 13:30:11.000000 psat-server-web-0.0.8/psat_server_web/schema/sherlock_crossmatches.sql
--rw-r--r--   0 kws        (502) staff       (20)     2038 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_cat_gaia_dr1.sql
--rw-r--r--   0 kws        (502) staff       (20)     2927 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_cat_gaia_dr2.sql
--rw-r--r--   0 kws        (502) staff       (20)     2421 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_cat_gaia_dr2_cassandra.cql
--rw-r--r--   0 kws        (502) staff       (20)     1378 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_cat_kepler_k2.sql
--rw-r--r--   0 kws        (502) staff       (20)      699 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_cat_kepler_k2_pixels.sql
--rw-r--r--   0 kws        (502) staff       (20)     6105 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_cat_ps1_medium_deep_ref.sql
--rw-r--r--   0 kws        (502) staff       (20)      713 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_cat_ps1_ubercal_stars.sql
--rw-r--r--   0 kws        (502) staff       (20)      570 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_cat_satellites.sql
--rw-r--r--   0 kws        (502) staff       (20)     4598 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_catalogue_tables.sql
--rw-r--r--   0 kws        (502) staff       (20)     1501 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_cfa_detections.sql
--rw-r--r--   0 kws        (502) staff       (20)      418 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_cfa_to_ipp_lookup.sql
--rw-r--r--   0 kws        (502) staff       (20)      916 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_classification_flags.sql
--rw-r--r--   0 kws        (502) staff       (20)      389 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_classification_history.sql
--rw-r--r--   0 kws        (502) staff       (20)     5585 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_cmf_metadata.sql
--rw-r--r--   0 kws        (502) staff       (20)     1857 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_cross_matches.sql
--rw-r--r--   0 kws        (502) staff       (20)      816 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_cross_matches_external.sql
--rw-r--r--   0 kws        (502) staff       (20)      618 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_detection_lists.sql
--rw-r--r--   0 kws        (502) staff       (20)      605 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_detection_lists_atlas.sql
--rw-r--r--   0 kws        (502) staff       (20)      572 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_followup_photometry.sql
--rw-r--r--   0 kws        (502) staff       (20)      920 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_followup_telescope_instruments.sql
--rw-r--r--   0 kws        (502) staff       (20)      679 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_followup_telescopes.sql
--rw-r--r--   0 kws        (502) staff       (20)     1857 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_forced_photometry.sql
--rw-r--r--   0 kws        (502) staff       (20)     1020 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_function_lunation.sql
--rw-r--r--   0 kws        (502) staff       (20)      898 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_function_mjdlunation.sql
--rw-r--r--   0 kws        (502) staff       (20)      728 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_gravity_event_annotations.sql
--rw-r--r--   0 kws        (502) staff       (20)      451 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_gravity_events.sql
--rw-r--r--   0 kws        (502) staff       (20)     1501 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_guide_star_cat.sql
--rw-r--r--   0 kws        (502) staff       (20)      717 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_image_groups.sql
--rw-r--r--   0 kws        (502) staff       (20)      763 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_images.sql
--rw-r--r--   0 kws        (502) staff       (20)      418 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_ipp_to_cfa_lookup.sql
--rw-r--r--   0 kws        (502) staff       (20)     1499 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_latest_object_stats.sql
--rw-r--r--   0 kws        (502) staff       (20)      761 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_object_comments.sql
--rw-r--r--   0 kws        (502) staff       (20)     2464 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_object_group_definitions.sql
--rw-r--r--   0 kws        (502) staff       (20)     1746 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_object_group_definitions_atlas.sql
--rw-r--r--   0 kws        (502) staff       (20)      465 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_object_groups.sql
--rw-r--r--   0 kws        (502) staff       (20)     2771 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_parameter_definitions.sql
--rw-r--r--   0 kws        (502) staff       (20)     1189 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_photpipe_detections.sql
--rw-r--r--   0 kws        (502) staff       (20)      942 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_postage_stamp_images.sql
--rw-r--r--   0 kws        (502) staff       (20)      557 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_postage_stamp_requests.sql
--rw-r--r--   0 kws        (502) staff       (20)      933 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_postage_stamp_status_codes.sql
--rw-r--r--   0 kws        (502) staff       (20)      879 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_processing_status.sql
--rw-r--r--   0 kws        (502) staff       (20)      672 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_search_parameters.sql
--rw-r--r--   0 kws        (502) staff       (20)      522 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_tns_requests.sql
--rw-r--r--   0 kws        (502) staff       (20)     1140 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_tphot_detections.sql
--rw-r--r--   0 kws        (502) staff       (20)     7691 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_transient_objects.sql
--rw-r--r--   0 kws        (502) staff       (20)     4486 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_transient_reobservations.sql
--rw-r--r--   0 kws        (502) staff       (20)      671 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_zoo_requests.sql
--rw-r--r--   0 kws        (502) staff       (20)      545 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/tcs_zooniverse_scores.sql
--rw-r--r--   0 kws        (502) staff       (20)      537 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/types_gaia_dr2_cassandra.txt
--rw-r--r--   0 kws        (502) staff       (20)     4346 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/update_database_types_to_tns_types_atlas.sql
--rw-r--r--   0 kws        (502) staff       (20)     4521 2021-03-09 13:29:22.000000 psat-server-web-0.0.8/psat_server_web/schema/update_database_types_to_tns_types_panstarrs.sql
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:04:34.839336 psat-server-web-0.0.8/psat_server_web.egg-info/
--rw-r--r--   0 kws        (502) staff       (20)      594 2021-05-20 22:04:33.000000 psat-server-web-0.0.8/psat_server_web.egg-info/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)    18701 2021-05-20 22:04:34.000000 psat-server-web-0.0.8/psat_server_web.egg-info/SOURCES.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2021-05-20 22:04:33.000000 psat-server-web-0.0.8/psat_server_web.egg-info/dependency_links.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2021-05-20 22:04:33.000000 psat-server-web-0.0.8/psat_server_web.egg-info/not-zip-safe
--rw-r--r--   0 kws        (502) staff       (20)       82 2021-05-20 22:04:33.000000 psat-server-web-0.0.8/psat_server_web.egg-info/requires.txt
--rw-r--r--   0 kws        (502) staff       (20)       16 2021-05-20 22:04:33.000000 psat-server-web-0.0.8/psat_server_web.egg-info/top_level.txt
--rw-r--r--   0 kws        (502) staff       (20)       38 2021-05-20 22:04:35.336739 psat-server-web-0.0.8/setup.cfg
--rwxr-xr-x   0 kws        (502) staff       (20)     1091 2021-05-20 22:04:04.000000 psat-server-web-0.0.8/setup.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.544044 psat-server-web-0.0.9/
+-rw-r--r--   0 kws        (502) staff       (20)      228 2021-05-20 00:05:16.000000 psat-server-web-0.0.9/MANIFEST.in
+-rw-r--r--   0 kws        (502) staff       (20)      594 2021-05-20 22:55:55.543570 psat-server-web-0.0.9/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)       79 2021-03-09 12:47:41.000000 psat-server-web-0.0.9/README.md
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:54.925799 psat-server-web-0.0.9/psat_server_web/
+-rw-r--r--   0 kws        (502) staff       (20)       38 2021-05-15 13:54:02.000000 psat-server-web-0.0.9/psat_server_web/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       22 2021-05-20 22:44:26.000000 psat-server-web-0.0.9/psat_server_web/__version__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:54.929094 psat-server-web-0.0.9/psat_server_web/atlas/
+-rw-r--r--   0 kws        (502) staff       (20)        0 2021-05-15 12:47:24.000000 psat-server-web-0.0.9/psat_server_web/atlas/__init__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:54.941858 psat-server-web-0.0.9/psat_server_web/atlas/atlas/
+-rw-r--r--   0 kws        (502) staff       (20)        0 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/atlas/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)    41196 2021-03-11 18:42:36.000000 psat-server-web-0.0.9/psat_server_web/atlas/atlas/commonqueries.py
+-rw-r--r--   0 kws        (502) staff       (20)    17570 2021-05-05 20:09:40.000000 psat-server-web-0.0.9/psat_server_web/atlas/atlas/dbviews.py
+-rw-r--r--   0 kws        (502) staff       (20)      379 2021-03-09 14:56:31.000000 psat-server-web-0.0.9/psat_server_web/atlas/atlas/document.sh
+-rw-r--r--   0 kws        (502) staff       (20)     5959 2021-05-13 00:15:35.000000 psat-server-web-0.0.9/psat_server_web/atlas/atlas/formchoices.py
+-rw-r--r--   0 kws        (502) staff       (20)    13331 2021-05-14 12:21:06.000000 psat-server-web-0.0.9/psat_server_web/atlas/atlas/helpers.py
+-rw-r--r--   0 kws        (502) staff       (20)    29140 2021-03-09 14:56:37.000000 psat-server-web-0.0.9/psat_server_web/atlas/atlas/lightcurvequeries.py
+-rw-r--r--   0 kws        (502) staff       (20)    43611 2021-05-05 19:59:34.000000 psat-server-web-0.0.9/psat_server_web/atlas/atlas/models.py
+-rw-r--r--   0 kws        (502) staff       (20)     4730 2021-05-20 22:52:38.000000 psat-server-web-0.0.9/psat_server_web/atlas/atlas/settings.py
+-rw-r--r--   0 kws        (502) staff       (20)     5390 2021-03-11 00:41:45.000000 psat-server-web-0.0.9/psat_server_web/atlas/atlas/sqlpaginator.py
+-rw-r--r--   0 kws        (502) staff       (20)     4310 2021-05-07 00:15:44.000000 psat-server-web-0.0.9/psat_server_web/atlas/atlas/urls.py
+-rw-r--r--   0 kws        (502) staff       (20)   163293 2021-05-20 22:00:55.000000 psat-server-web-0.0.9/psat_server_web/atlas/atlas/views.py
+-rw-r--r--   0 kws        (502) staff       (20)     1165 2021-03-10 22:48:56.000000 psat-server-web-0.0.9/psat_server_web/atlas/atlas/wsgi.atlas.conf
+-rw-r--r--   0 kws        (502) staff       (20)      329 2021-05-05 21:27:19.000000 psat-server-web-0.0.9/psat_server_web/atlas/atlas/wsgi.py
+-rw-r--r--   0 kws        (502) staff       (20)      945 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/atlas/wsgi_apache_example.conf
+-rwxr-xr-x   0 kws        (502) staff       (20)     1851 2021-05-20 22:37:24.000000 psat-server-web-0.0.9/psat_server_web/atlas/generate_mod_wsgi_apachectl.sh
+-rwxr-xr-x   0 kws        (502) staff       (20)      248 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/manage.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:54.916285 psat-server-web-0.0.9/psat_server_web/atlas/media/
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:54.942484 psat-server-web-0.0.9/psat_server_web/atlas/media/images/
+-rw-r--r--   0 kws        (502) staff       (20)       81 2021-05-15 10:03:26.000000 psat-server-web-0.0.9/psat_server_web/atlas/media/images/README.txt
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:54.917439 psat-server-web-0.0.9/psat_server_web/atlas/site_media/
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:54.944858 psat-server-web-0.0.9/psat_server_web/atlas/site_media/css/
+-rw-r--r--   0 kws        (502) staff       (20)    15810 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/css/aladin.css
+-rw-r--r--   0 kws        (502) staff       (20)     6501 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/css/celestial.css
+-rw-r--r--   0 kws        (502) staff       (20)    13715 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/css/main.css
+-rw-r--r--   0 kws        (502) staff       (20)     3383 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/css/main_bootstrap.css
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:54.946601 psat-server-web-0.0.9/psat_server_web/atlas/site_media/images/
+-rw-r--r--   0 kws        (502) staff       (20)   163712 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/images/atlas_logo.png
+-rw-r--r--   0 kws        (502) staff       (20)    14986 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/images/image_not_available.jpeg
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:54.982840 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/
+-rw-r--r--   0 kws        (502) staff       (20)   455297 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/aladin.js
+-rw-r--r--   0 kws        (502) staff       (20)     1620 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/bootstrap_utils.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:54.988765 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/
+-rw-r--r--   0 kws        (502) staff       (20)   160860 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/celestial.js
+-rw-r--r--   0 kws        (502) staff       (20)    90592 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/d3.geo.projection.js
+-rw-r--r--   0 kws        (502) staff       (20)    46780 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/d3.geo.projection.min.js
+-rw-r--r--   0 kws        (502) staff       (20)     8471 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/d3.geo.zoom.js
+-rw-r--r--   0 kws        (502) staff       (20)   151732 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/d3.min.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:54.997006 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/
+-rw-r--r--   0 kws        (502) staff       (20)        0 2021-05-14 23:13:00.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)    39824 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/constellations.bounds.json
+-rw-r--r--   0 kws        (502) staff       (20)    19510 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/constellations.json
+-rw-r--r--   0 kws        (502) staff       (20)    26254 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/constellations.lines.json
+-rw-r--r--   0 kws        (502) staff       (20)     7398 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/dsos.bright.json
+-rw-r--r--   0 kws        (502) staff       (20)    61574 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/lg.json
+-rw-r--r--   0 kws        (502) staff       (20)   534254 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/mw.json
+-rw-r--r--   0 kws        (502) staff       (20)     3884 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/planets.json
+-rw-r--r--   0 kws        (502) staff       (20)   759360 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/stars.6.json
+-rw-r--r--   0 kws        (502) staff       (20)     9941 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/colourplot.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.038733 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/
+-rw-r--r--   0 kws        (502) staff       (20)    41784 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/excanvas.js
+-rw-r--r--   0 kws        (502) staff       (20)   252881 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery-1.7.2.js
+-rw-r--r--   0 kws        (502) staff       (20)    17407 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.axislabels.js
+-rw-r--r--   0 kws        (502) staff       (20)     5191 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.crosshair.js
+-rw-r--r--   0 kws        (502) staff       (20)    12389 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.errorbars.js
+-rw-r--r--   0 kws        (502) staff       (20)     6771 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.fillbetween.js
+-rw-r--r--   0 kws        (502) staff       (20)     7351 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.image.js
+-rw-r--r--   0 kws        (502) staff       (20)   106797 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.js
+-rw-r--r--   0 kws        (502) staff       (20)    13634 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.navigate.js
+-rw-r--r--   0 kws        (502) staff       (20)    22589 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.pie.js
+-rw-r--r--   0 kws        (502) staff       (20)     2458 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.resize.js
+-rw-r--r--   0 kws        (502) staff       (20)    12018 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.selection.js
+-rw-r--r--   0 kws        (502) staff       (20)     6968 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.stack.js
+-rw-r--r--   0 kws        (502) staff       (20)     2441 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.symbol.js
+-rw-r--r--   0 kws        (502) staff       (20)     3291 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.threshold.js
+-rw-r--r--   0 kws        (502) staff       (20)     2709 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/followup_selectall.js
+-rw-r--r--   0 kws        (502) staff       (20)    10907 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/lightcurve.js
+-rw-r--r--   0 kws        (502) staff       (20)     8349 2021-03-09 13:34:59.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/lightcurveplotly.js
+-rw-r--r--   0 kws        (502) staff       (20)     5637 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/mjdcalc.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.039199 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/plotly/
+-rw-r--r--   0 kws        (502) staff       (20)  5856350 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/plotly/plotly-latest.kws.js
+-rw-r--r--   0 kws        (502) staff       (20)     7661 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/recurrenceplot.js
+-rw-r--r--   0 kws        (502) staff       (20)     7430 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/recurrenceplotplotly.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.077607 psat-server-web-0.0.9/psat_server_web/atlas/sql/
+-rw-r--r--   0 kws        (502) staff       (20)    16485 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/sql/create_web_views.sql
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.088003 psat-server-web-0.0.9/psat_server_web/atlas/templates/
+-rw-r--r--   0 kws        (502) staff       (20)      448 2021-05-20 10:54:42.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/400.html
+-rw-r--r--   0 kws        (502) staff       (20)      435 2021-05-20 10:37:36.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/403.html
+-rw-r--r--   0 kws        (502) staff       (20)      446 2021-05-20 08:49:19.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/404.html
+-rw-r--r--   0 kws        (502) staff       (20)      465 2021-05-20 10:56:58.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/500.html
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.132961 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/
+-rw-r--r--   0 kws        (502) staff       (20)     3700 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/atelfasttrackobject.txt
+-rw-r--r--   0 kws        (502) staff       (20)     1276 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/atelsdiscovery.txt
+-rw-r--r--   0 kws        (502) staff       (20)     5724 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/atelsfast.txt
+-rw-r--r--   0 kws        (502) staff       (20)    40683 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/candidate.html
+-rw-r--r--   0 kws        (502) staff       (20)    36872 2021-05-07 00:28:04.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/candidate_plotly.html
+-rw-r--r--   0 kws        (502) staff       (20)     3246 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/crossmatch_external.html
+-rw-r--r--   0 kws        (502) staff       (20)      462 2021-03-09 13:34:59.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/error.html
+-rw-r--r--   0 kws        (502) staff       (20)     2080 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/followup.html
+-rw-r--r--   0 kws        (502) staff       (20)      761 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/followup.txt
+-rw-r--r--   0 kws        (502) staff       (20)     2414 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/followup2.html
+-rw-r--r--   0 kws        (502) staff       (20)      657 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/followup_bs.html
+-rw-r--r--   0 kws        (502) staff       (20)     3227 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/followup_bypass_django_tables.html
+-rw-r--r--   0 kws        (502) staff       (20)    12788 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/followup_quickview.html
+-rw-r--r--   0 kws        (502) staff       (20)     1012 2021-05-14 12:15:07.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/followup_quickview_bs.html
+-rw-r--r--   0 kws        (502) staff       (20)      570 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/followup_subset.txt
+-rw-r--r--   0 kws        (502) staff       (20)     2765 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/index.html
+-rw-r--r--   0 kws        (502) staff       (20)     1527 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/index_bs.html
+-rw-r--r--   0 kws        (502) staff       (20)     7243 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/index_bs_celestial.html
+-rw-r--r--   0 kws        (502) staff       (20)      169 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/iobserve.txt
+-rw-r--r--   0 kws        (502) staff       (20)      557 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/lightcurve.txt
+-rw-r--r--   0 kws        (502) staff       (20)      625 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/lightcurveddc.txt
+-rw-r--r--   0 kws        (502) staff       (20)      821 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/lightcurveforced.txt
+-rw-r--r--   0 kws        (502) staff       (20)      445 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/pesstorecurrences.txt
+-rw-r--r--   0 kws        (502) staff       (20)      294 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/pesstorecurrencesddc.txt
+-rw-r--r--   0 kws        (502) staff       (20)      725 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/pesstosummary.txt
+-rw-r--r--   0 kws        (502) staff       (20)     6942 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/search_results.html
+-rw-r--r--   0 kws        (502) staff       (20)    21043 2021-05-14 12:38:16.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/search_results_plotly.html
+-rw-r--r--   0 kws        (502) staff       (20)       19 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/sne.json
+-rw-r--r--   0 kws        (502) staff       (20)      626 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/summary.csv
+-rw-r--r--   0 kws        (502) staff       (20)     2058 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/userdefinedlists.html
+-rw-r--r--   0 kws        (502) staff       (20)      538 2021-05-10 19:49:10.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/userdefinedlists_bs.html
+-rw-r--r--   0 kws        (502) staff       (20)      176 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/visibility.txt
+-rw-r--r--   0 kws        (502) staff       (20)     1006 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/base.html
+-rw-r--r--   0 kws        (502) staff       (20)     7304 2021-05-19 13:31:33.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/base_bootstrap.html
+-rw-r--r--   0 kws        (502) staff       (20)     2343 2021-05-19 19:17:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/base_bootstrap_login.html
+-rw-r--r--   0 kws        (502) staff       (20)     6107 2021-05-14 16:01:35.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/bootstrap4_django_tables2_atlas.html
+-rw-r--r--   0 kws        (502) staff       (20)      501 2021-05-19 21:12:44.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/invalid_login.html
+-rw-r--r--   0 kws        (502) staff       (20)      355 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/loggedin.html
+-rw-r--r--   0 kws        (502) staff       (20)      937 2021-05-19 21:36:39.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/login.html
+-rw-r--r--   0 kws        (502) staff       (20)      428 2021-05-19 21:12:06.000000 psat-server-web-0.0.9/psat_server_web/atlas/templates/logout.html
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.133446 psat-server-web-0.0.9/psat_server_web/config/
+-rw-r--r--   0 kws        (502) staff       (20)      770 2020-10-02 22:40:04.000000 psat-server-web-0.0.9/psat_server_web/config/wsgi.conf.template
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.135076 psat-server-web-0.0.9/psat_server_web/ps1/
+-rw-r--r--   0 kws        (502) staff       (20)        0 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)     1890 2021-03-09 14:51:15.000000 psat-server-web-0.0.9/psat_server_web/ps1/createUsers.py
+-rwxr-xr-x   0 kws        (502) staff       (20)      247 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/manage.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.145357 psat-server-web-0.0.9/psat_server_web/ps1/psdb/
+-rw-r--r--   0 kws        (502) staff       (20)        0 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/psdb/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)      697 2021-03-09 14:54:01.000000 psat-server-web-0.0.9/psat_server_web/ps1/psdb/admin.py
+-rw-r--r--   0 kws        (502) staff       (20)     7516 2021-03-09 14:54:02.000000 psat-server-web-0.0.9/psat_server_web/ps1/psdb/catalogueviews.py
+-rw-r--r--   0 kws        (502) staff       (20)    42272 2021-03-09 14:54:02.000000 psat-server-web-0.0.9/psat_server_web/ps1/psdb/commonqueries.py
+-rw-r--r--   0 kws        (502) staff       (20)    34040 2021-03-11 12:13:25.000000 psat-server-web-0.0.9/psat_server_web/ps1/psdb/dbviews.py
+-rw-r--r--   0 kws        (502) staff       (20)     4871 2021-03-09 13:30:11.000000 psat-server-web-0.0.9/psat_server_web/ps1/psdb/formchoices.py
+-rw-r--r--   0 kws        (502) staff       (20)     9899 2021-03-09 14:54:02.000000 psat-server-web-0.0.9/psat_server_web/ps1/psdb/helpers.py
+-rw-r--r--   0 kws        (502) staff       (20)    15791 2021-03-09 14:35:48.000000 psat-server-web-0.0.9/psat_server_web/ps1/psdb/img_scale.py
+-rw-r--r--   0 kws        (502) staff       (20)    18778 2021-03-09 14:54:03.000000 psat-server-web-0.0.9/psat_server_web/ps1/psdb/lightcurvequeries.py
+-rw-r--r--   0 kws        (502) staff       (20)    43644 2021-03-11 12:13:00.000000 psat-server-web-0.0.9/psat_server_web/ps1/psdb/models.py
+-rw-r--r--   0 kws        (502) staff       (20)     5837 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/psdb/settings.py.template
+-rw-r--r--   0 kws        (502) staff       (20)     4007 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/psdb/urls.py
+-rw-r--r--   0 kws        (502) staff       (20)    99285 2021-03-09 14:54:03.000000 psat-server-web-0.0.9/psat_server_web/ps1/psdb/views.py
+-rw-r--r--   0 kws        (502) staff       (20)      280 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/psdb/wsgi.py.template
+-rw-r--r--   0 kws        (502) staff       (20)      893 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/psdb/wsgi_apache_example.conf
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:54.920960 psat-server-web-0.0.9/psat_server_web/ps1/site_media/
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.147242 psat-server-web-0.0.9/psat_server_web/ps1/site_media/css/
+-rw-r--r--   0 kws        (502) staff       (20)    15810 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/css/aladin.css
+-rw-r--r--   0 kws        (502) staff       (20)     6501 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/css/celestial.css
+-rw-r--r--   0 kws        (502) staff       (20)    13430 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/css/main.css
+-rw-r--r--   0 kws        (502) staff       (20)     3479 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/css/main_bootstrap.css
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.246070 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/
+-rw-r--r--   0 kws        (502) staff       (20)    35860 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/1-star-hover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    22130 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/1-star.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    36051 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/2-star-hover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    27068 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/2-star.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    36308 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/3-star-hover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    31801 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/3-star.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     2610 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/aladin.gif
+-rw-r--r--   0 kws        (502) staff       (20)    58676 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/cfaIcon.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    61573 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/cfaIconHover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    21821 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/confirmed-sne-hover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    23630 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/confirmed-sne.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    57933 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/detection_example.jpg
+-rwxr-xr-x   0 kws        (502) staff       (20)      465 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/down.jpeg
+-rw-r--r--   0 kws        (502) staff       (20)     6659 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/down.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    14986 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/image_not_available.jpeg
+-rw-r--r--   0 kws        (502) staff       (20)    36417 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/jhuIcon.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    38864 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/jhuIconHover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     7928 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/minus.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    44343 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/ncuIcon.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    46130 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/ncuIconHover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    58496 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/non_detection_example.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     8506 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/others-hover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    11289 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/others.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    25306 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/panstarrs-logo-hover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    21877 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/panstarrs-logo.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    74999 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/panstarrs1_logo.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    85348 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/panstarrs1_o3_logo.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    76781 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/panstarrs2_logo.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    86931 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/panstarrs2_o3_logo.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    95536 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/panstarrs_logo.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    48452 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/pittsIcon.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    50248 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/pittsIconHover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     7740 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/plus.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    47509 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/ps1Icon.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    45155 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/ps1IconHover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    12609 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/ps1sc.gif
+-rw-r--r--   0 kws        (502) staff       (20)    30826 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/qub-logo-hover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    26675 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/qub-logo.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    37401 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/qubIcon.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    38167 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/qubIconHover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     1493 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/sdss.gif
+-rw-r--r--   0 kws        (502) staff       (20)    15197 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/table-background.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     1524 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/table-bottom-left.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     1551 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/table-bottom-right.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     1272 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/table-row.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     1442 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/table-top-left.jpg
+-rw-r--r--   0 kws        (502) staff       (20)     1549 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/table-top-right.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    41765 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/uhifaIcon.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    44162 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/uhifaIconHover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)      473 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/up.jpeg
+-rw-r--r--   0 kws        (502) staff       (20)     6445 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/up.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    14173 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/variable-stars-hover.jpg
+-rw-r--r--   0 kws        (502) staff       (20)    16952 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/variable-stars.jpg
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.251350 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/
+-rw-r--r--   0 kws        (502) staff       (20)   455297 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/aladin.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.282204 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/
+-rw-r--r--   0 kws        (502) staff       (20)   160860 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/celestial.js
+-rw-r--r--   0 kws        (502) staff       (20)    90592 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/d3.geo.projection.js
+-rw-r--r--   0 kws        (502) staff       (20)    46780 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/d3.geo.projection.min.js
+-rw-r--r--   0 kws        (502) staff       (20)     8471 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/d3.geo.zoom.js
+-rw-r--r--   0 kws        (502) staff       (20)   151732 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/d3.min.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.288411 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/
+-rw-r--r--   0 kws        (502) staff       (20)        0 2021-05-14 23:13:00.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)    39824 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/constellations.bounds.json
+-rw-r--r--   0 kws        (502) staff       (20)    19510 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/constellations.json
+-rw-r--r--   0 kws        (502) staff       (20)    26254 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/constellations.lines.json
+-rw-r--r--   0 kws        (502) staff       (20)     7398 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/dsos.bright.json
+-rw-r--r--   0 kws        (502) staff       (20)    61574 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/lg.json
+-rw-r--r--   0 kws        (502) staff       (20)   534254 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/mw.json
+-rw-r--r--   0 kws        (502) staff       (20)     3884 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/planets.json
+-rw-r--r--   0 kws        (502) staff       (20)   759360 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/stars.6.json
+-rw-r--r--   0 kws        (502) staff       (20)     9941 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/colourplot.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.329497 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/
+-rw-r--r--   0 kws        (502) staff       (20)    41784 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/excanvas.js
+-rw-r--r--   0 kws        (502) staff       (20)   252881 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery-1.7.2.js
+-rw-r--r--   0 kws        (502) staff       (20)    17407 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.axislabels.js
+-rw-r--r--   0 kws        (502) staff       (20)     5191 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.crosshair.js
+-rw-r--r--   0 kws        (502) staff       (20)    12389 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.errorbars.js
+-rw-r--r--   0 kws        (502) staff       (20)     6771 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.fillbetween.js
+-rw-r--r--   0 kws        (502) staff       (20)     7351 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.image.js
+-rw-r--r--   0 kws        (502) staff       (20)   106797 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.js
+-rw-r--r--   0 kws        (502) staff       (20)    13634 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.navigate.js
+-rw-r--r--   0 kws        (502) staff       (20)    22589 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.pie.js
+-rw-r--r--   0 kws        (502) staff       (20)     2458 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.resize.js
+-rw-r--r--   0 kws        (502) staff       (20)    12018 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.selection.js
+-rw-r--r--   0 kws        (502) staff       (20)     6968 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.stack.js
+-rw-r--r--   0 kws        (502) staff       (20)     2441 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.symbol.js
+-rw-r--r--   0 kws        (502) staff       (20)     3291 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.threshold.js
+-rw-r--r--   0 kws        (502) staff       (20)     1260 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/followup_selectall.js
+-rw-r--r--   0 kws        (502) staff       (20)    10724 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/lightcurve.js
+-rw-r--r--   0 kws        (502) staff       (20)     8308 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/lightcurveplotly.js
+-rw-r--r--   0 kws        (502) staff       (20)     5859 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/mjdcalc.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.330205 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/plotly/
+-rw-r--r--   0 kws        (502) staff       (20)  5856350 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/plotly/plotly-latest.kws.js
+-rw-r--r--   0 kws        (502) staff       (20)     7661 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/recurrenceplot.js
+-rw-r--r--   0 kws        (502) staff       (20)     7430 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/recurrenceplotplotly.js
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.344324 psat-server-web-0.0.9/psat_server_web/ps1/sql/
+-rw-r--r--   0 kws        (502) staff       (20)      982 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/sql/create_web_cat_views.sql
+-rw-r--r--   0 kws        (502) staff       (20)      812 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/sql/create_web_user_grants.sql
+-rw-r--r--   0 kws        (502) staff       (20)    44715 2021-03-09 13:30:11.000000 psat-server-web-0.0.9/psat_server_web/ps1/sql/create_web_views.sql
+-rw-r--r--   0 kws        (502) staff       (20)    13969 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/sql/create_web_views_fgss.sql
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.349226 psat-server-web-0.0.9/psat_server_web/ps1/templates/
+-rw-r--r--   0 kws        (502) staff       (20)      193 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/404.html
+-rw-r--r--   0 kws        (502) staff       (20)      368 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/500.html
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.349758 psat-server-web-0.0.9/psat_server_web/ps1/templates/admin/
+-rw-r--r--   0 kws        (502) staff       (20)      333 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/admin/base_site.html
+-rw-r--r--   0 kws        (502) staff       (20)    10344 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/base.html
+-rw-r--r--   0 kws        (502) staff       (20)     7099 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/base_bootstrap.html
+-rw-r--r--   0 kws        (502) staff       (20)      956 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/base_new.html
+-rw-r--r--   0 kws        (502) staff       (20)      250 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/invalid_login.html
+-rw-r--r--   0 kws        (502) staff       (20)      359 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/loggedin.html
+-rw-r--r--   0 kws        (502) staff       (20)      771 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/login.html
+-rw-r--r--   0 kws        (502) staff       (20)      197 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/logout.html
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.398502 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/
+-rw-r--r--   0 kws        (502) staff       (20)     1173 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/atelsdiscovery.txt
+-rw-r--r--   0 kws        (502) staff       (20)    18270 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/candidate.html
+-rw-r--r--   0 kws        (502) staff       (20)    38886 2021-03-09 13:30:11.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/candidate_plotly.html
+-rw-r--r--   0 kws        (502) staff       (20)    32828 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/candidate_quickview.html
+-rw-r--r--   0 kws        (502) staff       (20)    40854 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/candidateflot.html
+-rw-r--r--   0 kws        (502) staff       (20)     2215 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/candidates.html
+-rw-r--r--   0 kws        (502) staff       (20)      756 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/colourdata.txt
+-rw-r--r--   0 kws        (502) staff       (20)     3628 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/crossmatch_cfa_with_ipp.html
+-rw-r--r--   0 kws        (502) staff       (20)     3328 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/crossmatch_external.html
+-rw-r--r--   0 kws        (502) staff       (20)       17 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/dss2.html
+-rw-r--r--   0 kws        (502) staff       (20)      462 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/error.html
+-rw-r--r--   0 kws        (502) staff       (20)     3229 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/fasttrackastronote.txt
+-rw-r--r--   0 kws        (502) staff       (20)     3731 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/followup.html
+-rw-r--r--   0 kws        (502) staff       (20)      864 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/followup.txt
+-rw-r--r--   0 kws        (502) staff       (20)     2873 2021-03-09 13:30:11.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/followup_bs.html
+-rw-r--r--   0 kws        (502) staff       (20)    12747 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/followup_quickview.html
+-rw-r--r--   0 kws        (502) staff       (20)     9846 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/followup_quickview_bs.html
+-rw-r--r--   0 kws        (502) staff       (20)      702 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/gcn.txt
+-rw-r--r--   0 kws        (502) staff       (20)      652 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/gcn_latex.txt
+-rw-r--r--   0 kws        (502) staff       (20)     4902 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/index.html
+-rw-r--r--   0 kws        (502) staff       (20)    10229 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/index_bs_celestial.html
+-rw-r--r--   0 kws        (502) staff       (20)    15063 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/index_public.html
+-rw-r--r--   0 kws        (502) staff       (20)      245 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/lightcurve.txt
+-rw-r--r--   0 kws        (502) staff       (20)      321 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/lightcurveforced.txt
+-rw-r--r--   0 kws        (502) staff       (20)     5801 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/lightcurves.html
+-rw-r--r--   0 kws        (502) staff       (20)      294 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/obscat.txt
+-rw-r--r--   0 kws        (502) staff       (20)     1344 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/obsmediawiki.txt
+-rw-r--r--   0 kws        (502) staff       (20)     3803 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/public.html
+-rw-r--r--   0 kws        (502) staff       (20)      859 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/public_textonly.txt
+-rw-r--r--   0 kws        (502) staff       (20)     9225 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/reports.html
+-rw-r--r--   0 kws        (502) staff       (20)     3801 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/search_results.html
+-rw-r--r--   0 kws        (502) staff       (20)       19 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/sne.json
+-rw-r--r--   0 kws        (502) staff       (20)     2537 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/userdefinedlists.html
+-rw-r--r--   0 kws        (502) staff       (20)      875 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/userdefinedlists_bs.html
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:55.542668 psat-server-web-0.0.9/psat_server_web/schema/
+-rw-r--r--   0 kws        (502) staff       (20)     2263 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/atlas_detections.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1731 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/atlas_detectionsddc.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2212 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/atlas_diff_detections.sql
+-rw-r--r--   0 kws        (502) staff       (20)      652 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/atlas_diff_logs.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1093 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/atlas_diff_moments.sql
+-rw-r--r--   0 kws        (502) staff       (20)     3319 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/atlas_diff_objects.sql
+-rw-r--r--   0 kws        (502) staff       (20)      645 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/atlas_diff_subcell_logs.sql
+-rw-r--r--   0 kws        (502) staff       (20)      540 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/atlas_diff_subcells.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1646 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/atlas_forced_photometry.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2928 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/atlas_metadata.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1400 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/atlas_metadataddc.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1824 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/atlas_objects.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1595 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/atlas_stacked_forced_photometry.sql
+-rw-r--r--   0 kws        (502) staff       (20)      970 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/create_atlas_flattened_view.sql
+-rw-r--r--   0 kws        (502) staff       (20)     4055 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/create_photpipe_views.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2641 2021-03-11 12:43:21.000000 psat-server-web-0.0.9/psat_server_web/schema/create_schema.sql
+-rw-r--r--   0 kws        (502) staff       (20)     3312 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/create_user_grants.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1332 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/create_user_grants_generic.sql
+-rw-r--r--   0 kws        (502) staff       (20)      232 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/create_user_grants_root.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1190 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/delete_transients.sql
+-rw-r--r--   0 kws        (502) staff       (20)    60402 2021-03-10 12:07:36.000000 psat-server-web-0.0.9/psat_server_web/schema/generateATLASSchemaAndCPPClasses.py
+-rw-r--r--   0 kws        (502) staff       (20)     2489 2021-03-10 12:03:01.000000 psat-server-web-0.0.9/psat_server_web/schema/get_table_columns_for_avro.py
+-rw-r--r--   0 kws        (502) staff       (20)      182 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/get_table_columns_for_avro.sql
+-rw-r--r--   0 kws        (502) staff       (20)      977 2021-03-10 12:32:10.000000 psat-server-web-0.0.9/psat_server_web/schema/refresh_django_views.py
+-rw-r--r--   0 kws        (502) staff       (20)     4853 2021-03-10 22:44:14.000000 psat-server-web-0.0.9/psat_server_web/schema/setup_database.py
+-rw-r--r--   0 kws        (502) staff       (20)    13195 2021-03-10 22:48:16.000000 psat-server-web-0.0.9/psat_server_web/schema/setup_database_utils.py
+-rw-r--r--   0 kws        (502) staff       (20)      714 2021-03-09 13:30:11.000000 psat-server-web-0.0.9/psat_server_web/schema/sherlock_classifications.sql
+-rw-r--r--   0 kws        (502) staff       (20)     3104 2021-03-09 13:30:11.000000 psat-server-web-0.0.9/psat_server_web/schema/sherlock_crossmatches.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2038 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_cat_gaia_dr1.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2927 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_cat_gaia_dr2.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2421 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_cat_gaia_dr2_cassandra.cql
+-rw-r--r--   0 kws        (502) staff       (20)     1378 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_cat_kepler_k2.sql
+-rw-r--r--   0 kws        (502) staff       (20)      699 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_cat_kepler_k2_pixels.sql
+-rw-r--r--   0 kws        (502) staff       (20)     6105 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_cat_ps1_medium_deep_ref.sql
+-rw-r--r--   0 kws        (502) staff       (20)      713 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_cat_ps1_ubercal_stars.sql
+-rw-r--r--   0 kws        (502) staff       (20)      570 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_cat_satellites.sql
+-rw-r--r--   0 kws        (502) staff       (20)     4598 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_catalogue_tables.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1501 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_cfa_detections.sql
+-rw-r--r--   0 kws        (502) staff       (20)      418 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_cfa_to_ipp_lookup.sql
+-rw-r--r--   0 kws        (502) staff       (20)      916 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_classification_flags.sql
+-rw-r--r--   0 kws        (502) staff       (20)      389 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_classification_history.sql
+-rw-r--r--   0 kws        (502) staff       (20)     5585 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_cmf_metadata.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1857 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_cross_matches.sql
+-rw-r--r--   0 kws        (502) staff       (20)      816 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_cross_matches_external.sql
+-rw-r--r--   0 kws        (502) staff       (20)      618 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_detection_lists.sql
+-rw-r--r--   0 kws        (502) staff       (20)      605 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_detection_lists_atlas.sql
+-rw-r--r--   0 kws        (502) staff       (20)      572 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_followup_photometry.sql
+-rw-r--r--   0 kws        (502) staff       (20)      920 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_followup_telescope_instruments.sql
+-rw-r--r--   0 kws        (502) staff       (20)      679 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_followup_telescopes.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1857 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_forced_photometry.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1020 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_function_lunation.sql
+-rw-r--r--   0 kws        (502) staff       (20)      898 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_function_mjdlunation.sql
+-rw-r--r--   0 kws        (502) staff       (20)      728 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_gravity_event_annotations.sql
+-rw-r--r--   0 kws        (502) staff       (20)      451 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_gravity_events.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1501 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_guide_star_cat.sql
+-rw-r--r--   0 kws        (502) staff       (20)      717 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_image_groups.sql
+-rw-r--r--   0 kws        (502) staff       (20)      763 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_images.sql
+-rw-r--r--   0 kws        (502) staff       (20)      418 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_ipp_to_cfa_lookup.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1499 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_latest_object_stats.sql
+-rw-r--r--   0 kws        (502) staff       (20)      761 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_object_comments.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2464 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_object_group_definitions.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1746 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_object_group_definitions_atlas.sql
+-rw-r--r--   0 kws        (502) staff       (20)      465 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_object_groups.sql
+-rw-r--r--   0 kws        (502) staff       (20)     2771 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_parameter_definitions.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1189 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_photpipe_detections.sql
+-rw-r--r--   0 kws        (502) staff       (20)      942 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_postage_stamp_images.sql
+-rw-r--r--   0 kws        (502) staff       (20)      557 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_postage_stamp_requests.sql
+-rw-r--r--   0 kws        (502) staff       (20)      933 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_postage_stamp_status_codes.sql
+-rw-r--r--   0 kws        (502) staff       (20)      879 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_processing_status.sql
+-rw-r--r--   0 kws        (502) staff       (20)      672 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_search_parameters.sql
+-rw-r--r--   0 kws        (502) staff       (20)      522 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_tns_requests.sql
+-rw-r--r--   0 kws        (502) staff       (20)     1140 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_tphot_detections.sql
+-rw-r--r--   0 kws        (502) staff       (20)     7691 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_transient_objects.sql
+-rw-r--r--   0 kws        (502) staff       (20)     4486 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_transient_reobservations.sql
+-rw-r--r--   0 kws        (502) staff       (20)      671 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_zoo_requests.sql
+-rw-r--r--   0 kws        (502) staff       (20)      545 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/tcs_zooniverse_scores.sql
+-rw-r--r--   0 kws        (502) staff       (20)      537 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/types_gaia_dr2_cassandra.txt
+-rw-r--r--   0 kws        (502) staff       (20)     4346 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/update_database_types_to_tns_types_atlas.sql
+-rw-r--r--   0 kws        (502) staff       (20)     4521 2021-03-09 13:29:22.000000 psat-server-web-0.0.9/psat_server_web/schema/update_database_types_to_tns_types_panstarrs.sql
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2021-05-20 22:55:54.928063 psat-server-web-0.0.9/psat_server_web.egg-info/
+-rw-r--r--   0 kws        (502) staff       (20)      594 2021-05-20 22:55:53.000000 psat-server-web-0.0.9/psat_server_web.egg-info/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)    18701 2021-05-20 22:55:54.000000 psat-server-web-0.0.9/psat_server_web.egg-info/SOURCES.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2021-05-20 22:55:53.000000 psat-server-web-0.0.9/psat_server_web.egg-info/dependency_links.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2021-05-20 22:55:53.000000 psat-server-web-0.0.9/psat_server_web.egg-info/not-zip-safe
+-rw-r--r--   0 kws        (502) staff       (20)       82 2021-05-20 22:55:53.000000 psat-server-web-0.0.9/psat_server_web.egg-info/requires.txt
+-rw-r--r--   0 kws        (502) staff       (20)       16 2021-05-20 22:55:53.000000 psat-server-web-0.0.9/psat_server_web.egg-info/top_level.txt
+-rw-r--r--   0 kws        (502) staff       (20)       38 2021-05-20 22:55:55.544209 psat-server-web-0.0.9/setup.cfg
+-rwxr-xr-x   0 kws        (502) staff       (20)     1091 2021-05-20 22:53:22.000000 psat-server-web-0.0.9/setup.py
```

### Comparing `psat-server-web-0.0.8/PKG-INFO` & `psat-server-web-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psat-server-web
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pan-STARRS and ATLAS web interface.
 Home-page: https://github.com/genghisken/psat-server-web
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Description: # psat-server-web
         Python 3 web interface for the Pan-STARRS and ATLAS surveys.
```

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/atlas/commonqueries.py` & `psat-server-web-0.0.9/psat_server_web/atlas/atlas/commonqueries.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/atlas/dbviews.py` & `psat-server-web-0.0.9/psat_server_web/atlas/atlas/dbviews.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/atlas/formchoices.py` & `psat-server-web-0.0.9/psat_server_web/atlas/atlas/formchoices.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/atlas/helpers.py` & `psat-server-web-0.0.9/psat_server_web/atlas/atlas/helpers.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/atlas/lightcurvequeries.py` & `psat-server-web-0.0.9/psat_server_web/atlas/atlas/lightcurvequeries.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/atlas/models.py` & `psat-server-web-0.0.9/psat_server_web/atlas/atlas/models.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/atlas/settings.py` & `psat-server-web-0.0.9/psat_server_web/ps1/psdb/settings.py.template`

 * *Files 14% similar despite different names*

```diff
@@ -1,139 +1,161 @@
 """
-Django settings for atlas project.
+Django settings for PS1 project.
 
 For more information on this file, see
 https://docs.djangoproject.com/en/1.7/topics/settings/
 
 For the full list of settings and their values, see
 https://docs.djangoproject.com/en/1.7/ref/settings/
 """
 
 # Build paths inside the project like this: os.path.join(BASE_DIR, ...)
 import os
-from dotenv import load_dotenv
-
-# import forcephot
-
-load_dotenv(override=True)
-
-#from pathlib import Path  # Python 3.6+ only
-
 BASE_DIR = os.path.dirname(os.path.dirname(__file__))
-#BASE_DIR = Path(__file__).resolve().parent.parent
-#PATHPREFIX = '/sne/atlas'
-PATHPREFIX = ''
 
 SITE_ID = 1
 
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/1.7/howto/deployment/checklist/
 
 # SECURITY WARNING: keep the secret key used in production secret!
-SECRET_KEY = os.environ.get('DJANGO_SECRET_KEY')
+SECRET_KEY = 'gcu3znpf+#a5iglpe1y+g*s7k^&mz8xe)=6h606rk46o*3-!!f'
 
 # SECURITY WARNING: don't run with debug turned on in production!
-DEBUG = False
+DEBUG = True
 
-TEMPLATE_DEBUG = False
+TEMPLATE_DEBUG = True
 
 ALLOWED_HOSTS = ['*']
 
-ROOT_URLCONF = 'atlas.urls'
+ROOT_URLCONF = 'psdb.urls'
 
-WSGI_APPLICATION = 'atlas.wsgi.application'
+WSGI_APPLICATION = 'psdb.wsgi.application'
 
 # 2016-11-07 KWS Fixed the authentication issues by setting cookie names
-CSRF_COOKIE_NAME = 'csrf_' + os.environ.get('DJANGO_MYSQL_DBNAME')
-SESSION_COOKIE_NAME = 'session_' + os.environ.get('DJANGO_MYSQL_DBNAME')
+CSRF_COOKIE_NAME = 'csrf_GENERIC_DATABASE'
+SESSION_COOKIE_NAME = 'session_GENERIC_DATABASE'
 
 # 2017-10-03 KWS Had to add this setting because of SSL proxy.
 CSRF_TRUSTED_ORIGINS = ['star.pst.qub.ac.uk']
 
-CSRF_FAILURE_VIEW = 'atlas.views.csrf_failure'
-
-LOGIN_REDIRECT_URL = 'home'
-LOGIN_URL = 'login'
-LOGOUT_URL = 'logout'
+CSRF_FAILURE_VIEW = 'psdb.views.csrf_failure'
+LOGIN_REDIRECT_URL = '/sne/GENERIC_DATABASE/psdb/'
+LOGIN_URL = '/sne/GENERIC_DATABASE/accounts/login/'
+LOGOUT_URL = '/sne/GENERIC_DATABASE/accounts/logout/'
 
 # Database
 # https://docs.djangoproject.com/en/1.7/ref/settings/#databases
 
 DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.mysql',
-        'NAME': os.environ.get('DJANGO_MYSQL_DBNAME'),
-        'USER': os.environ.get('DJANGO_MYSQL_DBUSER'),
-        'PASSWORD': os.environ.get('DJANGO_MYSQL_DBPASS'),
-        'HOST': os.environ.get('DJANGO_MYSQL_DBHOST'),
-        'PORT': int(os.environ.get('DJANGO_MYSQL_DBPORT')),
+        'NAME': 'GENERIC_DATABASE',
+        'USER': 'GENERIC_USER',
+        'PASSWORD': 'GENERIC_PASSWORD',
+        'HOST': 'GENERIC_HOST'
     }
 }
 
-
+# 2019-07-23 KWS Introduced daemons settings.
 DAEMONS = {
     'tns': {
-        'host': os.environ.get('DJANGO_TNS_DAEMON_SERVER'),
-        'port': int(os.environ.get('DJANGO_TNS_DAEMON_PORT')),
+        'host': GENERIC_DAEMON_HOST_TNS,
+        'port': GENERIC_DAEMON_PORT_TNS,
         'test': True
     },
     'mpc': {
-        'host': os.environ.get('DJANGO_MPC_DAEMON_SERVER'),
-        'port': int(os.environ.get('DJANGO_MPC_DAEMON_PORT')),
+        'host': GENERIC_DAEMON_HOST_MPC,
+        'port': GENERIC_DAEMON_PORT_MPC,
         'test': True
-    }
+    },
+    'psnames': {
+        'host': GENERIC_DAEMON_HOST_PS,
+        'port': GENERIC_DAEMON_PORT_PS,
+        'test': True
+    },
+}
+
+# 2019-08-23 KWS Moved SURVEY_FIELDS out of views.py into settings.py. Now we can modify
+#                without changing views.py.
+
+SURVEY_FIELDS = {
+    'RINGS': '3P',
+    'FGSS': '3F',
+    'MD01': '01',
+    'MD02': '02',
+    'MD03': '03',
+    'MD04': '04',
+    'MD05': '05',
+    'MD06': '06',
+    'MD07': '07',
+    'MD08': '08',
+    'MD09': '09',
+    'MD10': '10',
+    'M31': '31',
 }
 
+
 # Internationalization
 # https://docs.djangoproject.com/en/1.7/topics/i18n/
 
 LANGUAGE_CODE = 'en-us'
 
 TIME_ZONE = 'UTC'
 
 USE_I18N = True
 
 USE_L10N = True
 
 USE_TZ = True
 
 
+# Static files (CSS, JavaScript, Images)
+# https://docs.djangoproject.com/en/1.7/howto/static-files/
 
-# 2021-05-06 KWS New settings means that if we edit a static file we MUST rerun the collectstatic
-#                code to deploy the modified file.
-
-STATIC_URL = PATHPREFIX + '/static/'
-
-# STATICFILES_DIRS tells collectstatic where MY static files are.
-STATICFILES_DIRS = (
-  os.path.join(BASE_DIR, 'site_media'),
-)
-
-STATIC_ROOT = os.path.join(BASE_DIR, 'static')
-
-MEDIA_ROOT = os.path.join(BASE_DIR, 'media')
-MEDIA_URL = PATHPREFIX + '/media/'
+STATIC_URL = '/sne/GENERIC_DATABASE/site_media/'
+STATIC_ROOT = 'GENERIC_FILESYSTEM/code/web/ps1/site_media'
+MEDIA_ROOT = ''
+MEDIA_URL = ''
+
+
+## These settings will be deprecated in Django 1.8. You have been warned.
+#TEMPLATE_DIRS = (
+#    # Put strings here, like "/home/html/django_templates" or "C:/www/django/templates".
+#    # Always use forward slashes, even on Windows.
+#    # Don't forget to use absolute paths, not relative paths.
+#    "GENERIC_FILESYSTEM/code/web/ps1/templates",
+#)
 
 # All below copied from PS1 web app.
 
 # List of callables that know how to import templates from various sources.
 TEMPLATE_LOADERS = (
     'django.template.loaders.filesystem.Loader',
     'django.template.loaders.app_directories.Loader',
 )
 
-# 2018-06-06 KWS Added new TEMPLATES settings in place of TEMPLATE_CONTEXT_PROCESSORS
-#                and TEMPLATE_DIRS
+## 2015-11-30 KWS Added django.core.context_processors.request for django-tables2
+#TEMPLATE_CONTEXT_PROCESSORS = (
+#    "django.contrib.auth.context_processors.auth",
+#    "django.contrib.messages.context_processors.messages",
+#    "django.core.context_processors.debug",
+#    "django.core.context_processors.i18n",
+#    "django.core.context_processors.media",
+#    "django.core.context_processors.request",
+#    "django.core.context_processors.static",
+#    "django.core.context_processors.request",
+#)
+
 TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
         'DIRS': [
             # insert your TEMPLATE_DIRS here
-            os.path.join(BASE_DIR, 'templates'),
-
+            "GENERIC_FILESYSTEM/code/web/ps1/templates",
         ],
         'APP_DIRS': True,
         'OPTIONS': {
             'context_processors': [
                 # Insert your TEMPLATE_CONTEXT_PROCESSORS here or use this
                 # list if you haven't customized them:
                 "django.contrib.auth.context_processors.auth",
@@ -146,34 +168,34 @@
                 "django.template.context_processors.request",
             ],
         },
     },
 ]
 
 # KWS - Added pagination
-MIDDLEWARE = [
+MIDDLEWARE_CLASSES = (
     'django.middleware.common.CommonMiddleware',
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
-#    'django.contrib.auth.middleware.SessionAuthenticationMiddleware',
+    'django.contrib.auth.middleware.SessionAuthenticationMiddleware',
     'django.middleware.clickjacking.XFrameOptionsMiddleware',
-#    'pagination.middleware.PaginationMiddleware',
-    'django.middleware.security.SecurityMiddleware',
-]
+    'pagination.middleware.PaginationMiddleware',
+)
 
-ROOT_URLCONF = 'atlas.urls'
+ROOT_URLCONF = 'psdb.urls'
 
 # 2015-11-30 KWS Added django-tables2
-INSTALLED_APPS = [
+INSTALLED_APPS = (
     'django.contrib.admin',
     'django.contrib.auth',
-    'django.contrib.messages',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.sites',
     'django.contrib.staticfiles',
-    'atlas',
-    # 'pagination',
+    'psdb',
+    # 2016-02-09 KWS Try sqlpaginator
+    'sqlpaginator',
+    'pagination',
     'django_tables2',
-]
+)
```

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/atlas/sqlpaginator.py` & `psat-server-web-0.0.9/psat_server_web/atlas/atlas/sqlpaginator.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/atlas/urls.py` & `psat-server-web-0.0.9/psat_server_web/atlas/atlas/urls.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/atlas/views.py` & `psat-server-web-0.0.9/psat_server_web/atlas/atlas/views.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/atlas/wsgi.atlas.conf` & `psat-server-web-0.0.9/psat_server_web/atlas/atlas/wsgi.atlas.conf`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/atlas/wsgi_apache_example.conf` & `psat-server-web-0.0.9/psat_server_web/atlas/atlas/wsgi_apache_example.conf`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/generate_mod_wsgi_apachectl.sh` & `psat-server-web-0.0.9/psat_server_web/atlas/generate_mod_wsgi_apachectl.sh`

 * *Files 5% similar despite different names*

```diff
@@ -52,11 +52,12 @@
     sleep 1
     # wait a second to make sure the port is released
 else
     echo "Creating directory $APACHEPATH"
     mkdir -p APACHEPATH
 fi
 
-mod_wsgi-express setup-server --working-directory atlas --url-alias /static static --url-alias /media media --application-type module atlas.wsgi --server-root $APACHEPATH --port $PORT --mount-point $PREFIX
+mod_wsgi-express setup-server --working-directory atlas --url-alias $PREFIX/static static --url-alias $PREFIX/media media --application-type module atlas.wsgi --server-root $APACHEPATH --port $PORT --mount-point $PREFIX
+
 
 export PYTHONPATH=$(pwd)
 $APACHEPATH/apachectl start
```

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/css/aladin.css` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/css/aladin.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/css/celestial.css` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/css/celestial.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/css/main.css` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/css/main.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/css/main_bootstrap.css` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/css/main_bootstrap.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/images/atlas_logo.png` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/images/atlas_logo.png`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/images/image_not_available.jpeg` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/images/image_not_available.jpeg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/aladin.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/aladin.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/bootstrap_utils.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/bootstrap_utils.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/celestial.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/celestial.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/d3.geo.projection.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/d3.geo.projection.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/d3.geo.projection.min.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/d3.geo.projection.min.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/d3.geo.zoom.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/d3.geo.zoom.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/d3.min.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/d3.min.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/constellations.bounds.json` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/constellations.bounds.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/constellations.json` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/constellations.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/constellations.lines.json` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/constellations.lines.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/dsos.bright.json` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/dsos.bright.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/lg.json` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/lg.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/mw.json` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/mw.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/planets.json` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/planets.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/celestial/data/stars.6.json` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/celestial/data/stars.6.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/colourplot.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/colourplot.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/excanvas.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/excanvas.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery-1.7.2.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery-1.7.2.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.axislabels.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.axislabels.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.crosshair.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.crosshair.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.errorbars.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.errorbars.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.fillbetween.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.fillbetween.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.image.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.image.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.navigate.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.navigate.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.pie.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.pie.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.resize.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.resize.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.selection.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.selection.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.stack.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.stack.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.symbol.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.symbol.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/flot/jquery.flot.threshold.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/flot/jquery.flot.threshold.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/followup_selectall.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/followup_selectall.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/lightcurve.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/lightcurve.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/lightcurveplotly.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/lightcurveplotly.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/mjdcalc.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/mjdcalc.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/plotly/plotly-latest.kws.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/plotly/plotly-latest.kws.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/recurrenceplot.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/recurrenceplot.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/site_media/js/recurrenceplotplotly.js` & `psat-server-web-0.0.9/psat_server_web/atlas/site_media/js/recurrenceplotplotly.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/sql/create_web_views.sql` & `psat-server-web-0.0.9/psat_server_web/atlas/sql/create_web_views.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/atelfasttrackobject.txt` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/atelfasttrackobject.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/atelsdiscovery.txt` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/atelsdiscovery.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/atelsfast.txt` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/atelsfast.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/candidate.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/candidate.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/candidate_plotly.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/candidate_plotly.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/crossmatch_external.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/crossmatch_external.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/followup.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/followup.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/followup.txt` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/followup.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/followup2.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/followup2.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/followup_bs.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/followup_bs.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/followup_bypass_django_tables.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/followup_bypass_django_tables.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/followup_quickview.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/followup_quickview.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/followup_quickview_bs.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/followup_quickview_bs.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/followup_subset.txt` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/followup_subset.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/index.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/index.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/index_bs.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/index_bs.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/index_bs_celestial.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/index_bs_celestial.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/lightcurve.txt` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/lightcurve.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/lightcurveddc.txt` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/lightcurveddc.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/lightcurveforced.txt` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/lightcurveforced.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/pesstosummary.txt` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/pesstosummary.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/search_results.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/search_results.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/search_results_plotly.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/search_results_plotly.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/summary.csv` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/summary.csv`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/userdefinedlists.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/userdefinedlists.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/atlas/userdefinedlists_bs.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/atlas/userdefinedlists_bs.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/base.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/base.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/base_bootstrap.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/base_bootstrap.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/base_bootstrap_login.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/base_bootstrap_login.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/bootstrap4_django_tables2_atlas.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/bootstrap4_django_tables2_atlas.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/atlas/templates/login.html` & `psat-server-web-0.0.9/psat_server_web/atlas/templates/login.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/config/wsgi.conf.template` & `psat-server-web-0.0.9/psat_server_web/config/wsgi.conf.template`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/createUsers.py` & `psat-server-web-0.0.9/psat_server_web/ps1/createUsers.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/psdb/admin.py` & `psat-server-web-0.0.9/psat_server_web/ps1/psdb/admin.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/psdb/catalogueviews.py` & `psat-server-web-0.0.9/psat_server_web/ps1/psdb/catalogueviews.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/psdb/commonqueries.py` & `psat-server-web-0.0.9/psat_server_web/ps1/psdb/commonqueries.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/psdb/dbviews.py` & `psat-server-web-0.0.9/psat_server_web/ps1/psdb/dbviews.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/psdb/formchoices.py` & `psat-server-web-0.0.9/psat_server_web/ps1/psdb/formchoices.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/psdb/helpers.py` & `psat-server-web-0.0.9/psat_server_web/ps1/psdb/helpers.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/psdb/img_scale.py` & `psat-server-web-0.0.9/psat_server_web/ps1/psdb/img_scale.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/psdb/lightcurvequeries.py` & `psat-server-web-0.0.9/psat_server_web/ps1/psdb/lightcurvequeries.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/psdb/models.py` & `psat-server-web-0.0.9/psat_server_web/ps1/psdb/models.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/psdb/urls.py` & `psat-server-web-0.0.9/psat_server_web/ps1/psdb/urls.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/psdb/views.py` & `psat-server-web-0.0.9/psat_server_web/ps1/psdb/views.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/psdb/wsgi_apache_example.conf` & `psat-server-web-0.0.9/psat_server_web/ps1/psdb/wsgi_apache_example.conf`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/css/aladin.css` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/css/aladin.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/css/celestial.css` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/css/celestial.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/css/main.css` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/css/main.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/css/main_bootstrap.css` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/css/main_bootstrap.css`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/1-star-hover.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/1-star-hover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/1-star.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/1-star.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/2-star-hover.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/2-star-hover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/2-star.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/2-star.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/3-star-hover.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/3-star-hover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/3-star.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/3-star.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/aladin.gif` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/aladin.gif`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/cfaIcon.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/cfaIcon.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/cfaIconHover.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/cfaIconHover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/confirmed-sne-hover.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/confirmed-sne-hover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/confirmed-sne.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/confirmed-sne.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/detection_example.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/detection_example.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/down.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/down.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/image_not_available.jpeg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/image_not_available.jpeg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/jhuIcon.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/jhuIcon.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/jhuIconHover.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/jhuIconHover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/minus.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/minus.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/ncuIcon.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/ncuIcon.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/ncuIconHover.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/ncuIconHover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/non_detection_example.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/non_detection_example.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/others-hover.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/others-hover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/others.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/others.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/panstarrs-logo-hover.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/panstarrs-logo-hover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/panstarrs-logo.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/panstarrs-logo.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/panstarrs1_logo.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/panstarrs1_logo.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/panstarrs1_o3_logo.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/panstarrs1_o3_logo.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/panstarrs2_logo.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/panstarrs2_logo.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/panstarrs2_o3_logo.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/panstarrs2_o3_logo.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/panstarrs_logo.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/panstarrs_logo.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/pittsIcon.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/pittsIcon.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/pittsIconHover.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/pittsIconHover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/plus.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/plus.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/ps1Icon.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/ps1Icon.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/ps1IconHover.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/ps1IconHover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/ps1sc.gif` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/ps1sc.gif`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/qub-logo-hover.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/qub-logo-hover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/qub-logo.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/qub-logo.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/qubIcon.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/qubIcon.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/qubIconHover.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/qubIconHover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/sdss.gif` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/sdss.gif`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/table-background.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/table-background.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/table-bottom-left.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/table-bottom-left.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/table-bottom-right.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/table-bottom-right.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/table-row.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/table-row.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/table-top-left.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/table-top-left.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/table-top-right.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/table-top-right.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/uhifaIcon.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/uhifaIcon.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/uhifaIconHover.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/uhifaIconHover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/up.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/up.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/variable-stars-hover.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/variable-stars-hover.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/images/variable-stars.jpg` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/images/variable-stars.jpg`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/aladin.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/aladin.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/celestial.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/celestial.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/d3.geo.projection.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/d3.geo.projection.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/d3.geo.projection.min.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/d3.geo.projection.min.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/d3.geo.zoom.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/d3.geo.zoom.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/d3.min.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/d3.min.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/constellations.bounds.json` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/constellations.bounds.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/constellations.json` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/constellations.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/constellations.lines.json` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/constellations.lines.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/dsos.bright.json` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/dsos.bright.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/lg.json` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/lg.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/mw.json` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/mw.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/planets.json` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/planets.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/celestial/data/stars.6.json` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/celestial/data/stars.6.json`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/colourplot.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/colourplot.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/excanvas.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/excanvas.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery-1.7.2.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery-1.7.2.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.axislabels.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.axislabels.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.crosshair.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.crosshair.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.errorbars.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.errorbars.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.fillbetween.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.fillbetween.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.image.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.image.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.navigate.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.navigate.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.pie.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.pie.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.resize.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.resize.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.selection.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.selection.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.stack.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.stack.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.symbol.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.symbol.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/flot/jquery.flot.threshold.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/flot/jquery.flot.threshold.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/followup_selectall.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/followup_selectall.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/lightcurve.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/lightcurve.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/lightcurveplotly.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/lightcurveplotly.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/mjdcalc.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/mjdcalc.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/plotly/plotly-latest.kws.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/plotly/plotly-latest.kws.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/recurrenceplot.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/recurrenceplot.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/site_media/js/recurrenceplotplotly.js` & `psat-server-web-0.0.9/psat_server_web/ps1/site_media/js/recurrenceplotplotly.js`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/sql/create_web_cat_views.sql` & `psat-server-web-0.0.9/psat_server_web/ps1/sql/create_web_cat_views.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/sql/create_web_user_grants.sql` & `psat-server-web-0.0.9/psat_server_web/ps1/sql/create_web_user_grants.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/sql/create_web_views.sql` & `psat-server-web-0.0.9/psat_server_web/ps1/sql/create_web_views.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/sql/create_web_views_fgss.sql` & `psat-server-web-0.0.9/psat_server_web/ps1/sql/create_web_views_fgss.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/base.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/base.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/base_bootstrap.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/base_bootstrap.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/base_new.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/base_new.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/login.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/login.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/atelsdiscovery.txt` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/atelsdiscovery.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/candidate.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/candidate.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/candidate_plotly.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/candidate_plotly.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/candidate_quickview.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/candidate_quickview.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/candidateflot.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/candidateflot.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/candidates.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/candidates.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/colourdata.txt` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/colourdata.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/crossmatch_cfa_with_ipp.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/crossmatch_cfa_with_ipp.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/crossmatch_external.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/crossmatch_external.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/fasttrackastronote.txt` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/fasttrackastronote.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/followup.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/followup.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/followup.txt` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/followup.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/followup_bs.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/followup_bs.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/followup_quickview.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/followup_quickview.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/followup_quickview_bs.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/followup_quickview_bs.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/gcn.txt` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/gcn.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/gcn_latex.txt` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/gcn_latex.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/index.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/index.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/index_bs_celestial.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/index_bs_celestial.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/index_public.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/index_public.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/lightcurves.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/lightcurves.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/obsmediawiki.txt` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/obsmediawiki.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/public.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/public.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/public_textonly.txt` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/public_textonly.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/reports.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/reports.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/search_results.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/search_results.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/userdefinedlists.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/userdefinedlists.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/ps1/templates/psdb/userdefinedlists_bs.html` & `psat-server-web-0.0.9/psat_server_web/ps1/templates/psdb/userdefinedlists_bs.html`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/atlas_detections.sql` & `psat-server-web-0.0.9/psat_server_web/schema/atlas_detections.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/atlas_detectionsddc.sql` & `psat-server-web-0.0.9/psat_server_web/schema/atlas_detectionsddc.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/atlas_diff_detections.sql` & `psat-server-web-0.0.9/psat_server_web/schema/atlas_diff_detections.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/atlas_diff_logs.sql` & `psat-server-web-0.0.9/psat_server_web/schema/atlas_diff_logs.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/atlas_diff_moments.sql` & `psat-server-web-0.0.9/psat_server_web/schema/atlas_diff_moments.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/atlas_diff_objects.sql` & `psat-server-web-0.0.9/psat_server_web/schema/atlas_diff_objects.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/atlas_diff_subcell_logs.sql` & `psat-server-web-0.0.9/psat_server_web/schema/atlas_diff_subcell_logs.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/atlas_diff_subcells.sql` & `psat-server-web-0.0.9/psat_server_web/schema/atlas_diff_subcells.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/atlas_forced_photometry.sql` & `psat-server-web-0.0.9/psat_server_web/schema/atlas_forced_photometry.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/atlas_metadata.sql` & `psat-server-web-0.0.9/psat_server_web/schema/atlas_metadata.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/atlas_metadataddc.sql` & `psat-server-web-0.0.9/psat_server_web/schema/atlas_metadataddc.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/atlas_objects.sql` & `psat-server-web-0.0.9/psat_server_web/schema/atlas_objects.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/atlas_stacked_forced_photometry.sql` & `psat-server-web-0.0.9/psat_server_web/schema/atlas_stacked_forced_photometry.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/create_atlas_flattened_view.sql` & `psat-server-web-0.0.9/psat_server_web/schema/create_atlas_flattened_view.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/create_photpipe_views.sql` & `psat-server-web-0.0.9/psat_server_web/schema/create_photpipe_views.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/create_schema.sql` & `psat-server-web-0.0.9/psat_server_web/schema/create_schema.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/create_user_grants.sql` & `psat-server-web-0.0.9/psat_server_web/schema/create_user_grants.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/create_user_grants_generic.sql` & `psat-server-web-0.0.9/psat_server_web/schema/create_user_grants_generic.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/delete_transients.sql` & `psat-server-web-0.0.9/psat_server_web/schema/delete_transients.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/generateATLASSchemaAndCPPClasses.py` & `psat-server-web-0.0.9/psat_server_web/schema/generateATLASSchemaAndCPPClasses.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/get_table_columns_for_avro.py` & `psat-server-web-0.0.9/psat_server_web/schema/get_table_columns_for_avro.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/refresh_django_views.py` & `psat-server-web-0.0.9/psat_server_web/schema/refresh_django_views.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/setup_database.py` & `psat-server-web-0.0.9/psat_server_web/schema/setup_database.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/setup_database_utils.py` & `psat-server-web-0.0.9/psat_server_web/schema/setup_database_utils.py`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/sherlock_classifications.sql` & `psat-server-web-0.0.9/psat_server_web/schema/sherlock_classifications.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/sherlock_crossmatches.sql` & `psat-server-web-0.0.9/psat_server_web/schema/sherlock_crossmatches.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_cat_gaia_dr1.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_cat_gaia_dr1.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_cat_gaia_dr2.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_cat_gaia_dr2.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_cat_gaia_dr2_cassandra.cql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_cat_gaia_dr2_cassandra.cql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_cat_kepler_k2.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_cat_kepler_k2.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_cat_kepler_k2_pixels.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_cat_kepler_k2_pixels.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_cat_ps1_medium_deep_ref.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_cat_ps1_medium_deep_ref.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_cat_ps1_ubercal_stars.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_cat_ps1_ubercal_stars.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_cat_satellites.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_cat_satellites.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_catalogue_tables.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_catalogue_tables.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_cfa_detections.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_cfa_detections.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_classification_flags.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_classification_flags.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_cmf_metadata.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_cmf_metadata.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_cross_matches.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_cross_matches.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_cross_matches_external.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_cross_matches_external.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_detection_lists.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_detection_lists.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_detection_lists_atlas.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_detection_lists_atlas.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_followup_photometry.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_followup_photometry.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_followup_telescope_instruments.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_followup_telescope_instruments.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_followup_telescopes.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_followup_telescopes.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_forced_photometry.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_forced_photometry.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_function_lunation.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_function_lunation.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_function_mjdlunation.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_function_mjdlunation.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_gravity_event_annotations.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_gravity_event_annotations.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_guide_star_cat.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_guide_star_cat.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_image_groups.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_image_groups.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_images.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_images.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_latest_object_stats.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_latest_object_stats.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_object_comments.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_object_comments.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_object_group_definitions.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_object_group_definitions.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_object_group_definitions_atlas.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_object_group_definitions_atlas.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_parameter_definitions.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_parameter_definitions.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_photpipe_detections.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_photpipe_detections.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_postage_stamp_images.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_postage_stamp_images.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_postage_stamp_requests.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_postage_stamp_requests.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_postage_stamp_status_codes.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_postage_stamp_status_codes.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_processing_status.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_processing_status.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_search_parameters.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_search_parameters.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_tns_requests.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_tns_requests.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_tphot_detections.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_tphot_detections.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_transient_objects.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_transient_objects.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_transient_reobservations.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_transient_reobservations.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_zoo_requests.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_zoo_requests.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/tcs_zooniverse_scores.sql` & `psat-server-web-0.0.9/psat_server_web/schema/tcs_zooniverse_scores.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/types_gaia_dr2_cassandra.txt` & `psat-server-web-0.0.9/psat_server_web/schema/types_gaia_dr2_cassandra.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/update_database_types_to_tns_types_atlas.sql` & `psat-server-web-0.0.9/psat_server_web/schema/update_database_types_to_tns_types_atlas.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web/schema/update_database_types_to_tns_types_panstarrs.sql` & `psat-server-web-0.0.9/psat_server_web/schema/update_database_types_to_tns_types_panstarrs.sql`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/psat_server_web.egg-info/PKG-INFO` & `psat-server-web-0.0.9/psat_server_web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psat-server-web
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pan-STARRS and ATLAS web interface.
 Home-page: https://github.com/genghisken/psat-server-web
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Description: # psat-server-web
         Python 3 web interface for the Pan-STARRS and ATLAS surveys.
```

### Comparing `psat-server-web-0.0.8/psat_server_web.egg-info/SOURCES.txt` & `psat-server-web-0.0.9/psat_server_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psat-server-web-0.0.8/setup.py` & `psat-server-web-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         return f.read()
 
 setup(
     name="psat-server-web",
     description='Pan-STARRS and ATLAS web interface.',
     long_description=readme(),
     long_description_content_type="text/markdown",
-    version="0.0.8",
+    version="0.0.9",
     author='genghisken',
     author_email='ken.w.smith@gmail.com',
     license='MIT',
     url='https://github.com/genghisken/psat-server-web',
     packages=find_packages(),
     classifiers=[
           'Development Status :: 4 - Beta',
```

