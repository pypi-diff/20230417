# Comparing `tmp/django-advanced-report-builder-0.1.8.tar.gz` & `tmp/django-advanced-report-builder-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-advanced-report-builder-0.1.8.tar", last modified: Mon Mar  6 12:37:21 2023, max compression
+gzip compressed data, was "django-advanced-report-builder-0.1.9.tar", last modified: Thu Mar 30 07:56:09 2023, max compression
```

## Comparing `django-advanced-report-builder-0.1.8.tar` & `django-advanced-report-builder-0.1.9.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.344963 django-advanced-report-builder-0.1.8/
--rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       91 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)      683 2023-03-06 12:37:21.344796 django-advanced-report-builder-0.1.8/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      171 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.294912 django-advanced-report-builder-0.1.8/advanced_report_builder/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     4012 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/admin.py
--rw-r--r--   0 tom        (501) staff       (20)      218 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/apps.py
--rw-r--r--   0 tom        (501) staff       (20)     3394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/columns.py
--rw-r--r--   0 tom        (501) staff       (20)       40 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/customise.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.296026 django-advanced-report-builder-0.1.8/advanced_report_builder/data_merge/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/data_merge/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3830 2023-03-06 12:34:46.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/data_merge/utils.py
--rw-r--r--   0 tom        (501) staff       (20)      869 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/data_merge/widget.py
--rw-r--r--   0 tom        (501) staff       (20)     5477 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/duplicate.py
--rw-r--r--   0 tom        (501) staff       (20)      192 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/exceptions.py
--rw-r--r--   0 tom        (501) staff       (20)    10853 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/field_types.py
--rw-r--r--   0 tom        (501) staff       (20)    13799 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/filter_query.py
--rw-r--r--   0 tom        (501) staff       (20)     7914 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/globals.py
--rw-r--r--   0 tom        (501) staff       (20)     1315 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/includes.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.300006 django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/
--rw-r--r--   0 tom        (501) staff       (20)    14109 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)      591 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/0002_auto_20220209_1657.py
--rw-r--r--   0 tom        (501) staff       (20)     1734 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/0003_auto_20220215_1219.py
--rw-r--r--   0 tom        (501) staff       (20)      955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/0004_customreport.py
--rw-r--r--   0 tom        (501) staff       (20)     3623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/0005_auto_20220303_0958.py
--rw-r--r--   0 tom        (501) staff       (20)      914 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/0006_auto_20220310_1147.py
--rw-r--r--   0 tom        (501) staff       (20)      607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/0007_auto_20220322_1939.py
--rw-r--r--   0 tom        (501) staff       (20)      827 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/0008_auto_20220404_1144.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    18911 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/models.py
--rw-r--r--   0 tom        (501) staff       (20)      532 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/report_builder.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.263128 django-advanced-report-builder-0.1.8/advanced_report_builder/static/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.278514 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.263429 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/chart-js/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.304172 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/chart-js/js/
--rw-r--r--   0 tom        (501) staff       (20)   334540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js
--rw-r--r--   0 tom        (501) staff       (20)   405847 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js
--rw-r--r--   0 tom        (501) staff       (20)   193925 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js
--rw-r--r--   0 tom        (501) staff       (20)     1430 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js
--rw-r--r--   0 tom        (501) staff       (20)    12893 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.304537 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/
--rw-r--r--   0 tom        (501) staff       (20)    72125 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js
--rw-r--r--   0 tom        (501) staff       (20)     2352 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.264444 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/d3/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.307901 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/d3/js/
--rw-r--r--   0 tom        (501) staff       (20)   575002 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js
--rw-r--r--   0 tom        (501) staff       (20)   275533 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.264065 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/d3-funnel/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.305742 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/
--rw-r--r--   0 tom        (501) staff       (20)   205600 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js
--rw-r--r--   0 tom        (501) staff       (20)    58945 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.264814 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dashboard/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.308846 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dashboard/js/
--rw-r--r--   0 tom        (501) staff       (20)      563 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.265242 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.313800 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/
--rwxr-xr-x   0 tom        (501) staff       (20)      578 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore
--rwxr-xr-x   0 tom        (501) staff       (20)      122 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/.travis.yml
--rwxr-xr-x   0 tom        (501) staff       (20)     1176 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt
--rwxr-xr-x   0 tom        (501) staff       (20)     3291 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.314166 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/bin/
--rwxr-xr-x   0 tom        (501) staff       (20)     1442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer
--rwxr-xr-x   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/bower.json
--rwxr-xr-x   0 tom        (501) staff       (20)     5175 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3374 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1758 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js
--rwxr-xr-x   0 tom        (501) staff       (20)     5190 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/index.js
--rwxr-xr-x   0 tom        (501) staff       (20)      920 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/package.json
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.277472 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/jquery_extendext/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.314906 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/
--rwxr-xr-x   0 tom        (501) staff       (20)     4390 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1324 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.279878 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.316492 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/css/
--rwxr-xr-x   0 tom        (501) staff       (20)     3765 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css
--rwxr-xr-x   0 tom        (501) staff       (20)     3253 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css
--rwxr-xr-x   0 tom        (501) staff       (20)     3756 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css
--rwxr-xr-x   0 tom        (501) staff       (20)     3248 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.326889 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/
--rwxr-xr-x   0 tom        (501) staff       (20)     2962 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3082 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2494 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1431 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2309 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3273 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2672 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2662 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3216 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2917 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2952 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2522 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2299 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1412 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2645 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2787 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2451 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1310 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2627 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2782 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3062 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2503 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.329507 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/js/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.279572 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.329847 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/
--rwxr-xr-x   0 tom        (501) staff       (20)     1212 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js
--rwxr-xr-x   0 tom        (501) staff       (20)   191499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js
--rwxr-xr-x   0 tom        (501) staff       (20)    72607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js
--rwxr-xr-x   0 tom        (501) staff       (20)   201158 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js
--rwxr-xr-x   0 tom        (501) staff       (20)    77072 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.330331 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/scss/
--rwxr-xr-x   0 tom        (501) staff       (20)      442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/scss/dark.scss
--rwxr-xr-x   0 tom        (501) staff       (20)     3887 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.332669 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/
--rwxr-xr-x   0 tom        (501) staff       (20)      266 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-checkbox.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-tooltip-errors.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss
--rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_invert.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      469 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_sortable.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/bt-tooltip-errors.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss
--rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/invert.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      465 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/sortable.scss
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.280741 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.333214 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.333793 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.334040 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/bar/
--rw-r--r--   0 tom        (501) staff       (20)     4581 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.334516 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/funnel/
--rw-r--r--   0 tom        (501) staff       (20)     1362 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html
--rw-r--r--   0 tom        (501) staff       (20)     1007 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.334736 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/line/
--rw-r--r--   0 tom        (501) staff       (20)     4020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      486 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/modal.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.334971 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/pie/
--rw-r--r--   0 tom        (501) staff       (20)     2084 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      858 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/report.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.335218 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/data_merge/
--rw-r--r--   0 tom        (501) staff       (20)     2966 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.336381 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/datatables/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.336866 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/datatables/fields/
--rw-r--r--   0 tom        (501) staff       (20)      254 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/datatables/fields/modal.html
--rw-r--r--   0 tom        (501) staff       (20)     3329 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html
--rw-r--r--   0 tom        (501) staff       (20)      377 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/datatables/modal.html
--rw-r--r--   0 tom        (501) staff       (20)      593 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html
--rw-r--r--   0 tom        (501) staff       (20)      256 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/datatables/query_modal.html
--rw-r--r--   0 tom        (501) staff       (20)     1127 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/datatables/report.html
--rw-r--r--   0 tom        (501) staff       (20)     8185 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.337782 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/kanban/
--rw-r--r--   0 tom        (501) staff       (20)      499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/kanban/description_modal.html
--rw-r--r--   0 tom        (501) staff       (20)     2038 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      308 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/kanban/modal.html
--rw-r--r--   0 tom        (501) staff       (20)     1961 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/kanban/report.html
--rw-r--r--   0 tom        (501) staff       (20)     3468 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/query_builder.html
--rw-r--r--   0 tom        (501) staff       (20)     9491 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/select_column.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.338496 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/single_values/
--rw-r--r--   0 tom        (501) staff       (20)     1896 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html
--rw-r--r--   0 tom        (501) staff       (20)     1643 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/single_values/report.html
--rw-r--r--   0 tom        (501) staff       (20)      327 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/toggle.py
--rw-r--r--   0 tom        (501) staff       (20)     3830 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/urls.py
--rw-r--r--   0 tom        (501) staff       (20)     4447 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/utils.py
--rw-r--r--   0 tom        (501) staff       (20)    12521 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/variable_date.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.341831 django-advanced-report-builder-0.1.8/advanced_report_builder/views/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    11541 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/bar_charts.py
--rw-r--r--   0 tom        (501) staff       (20)    16346 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/charts_base.py
--rw-r--r--   0 tom        (501) staff       (20)     3020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/custom.py
--rw-r--r--   0 tom        (501) staff       (20)     8659 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/dashboard.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.342825 django-advanced-report-builder-0.1.8/advanced_report_builder/views/datatables/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/datatables/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     6801 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/datatables/datatables.py
--rw-r--r--   0 tom        (501) staff       (20)    25412 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/datatables/modal.py
--rw-r--r--   0 tom        (501) staff       (20)    11394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/datatables/utils.py
--rw-r--r--   0 tom        (501) staff       (20)     8725 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/funnel_charts.py
--rw-r--r--   0 tom        (501) staff       (20)    32161 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/kanban.py
--rw-r--r--   0 tom        (501) staff       (20)    12979 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/line_charts.py
--rw-r--r--   0 tom        (501) staff       (20)    21031 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/modals_base.py
--rw-r--r--   0 tom        (501) staff       (20)     8686 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/pie_charts.py
--rw-r--r--   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/report.py
--rw-r--r--   0 tom        (501) staff       (20)     7812 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/report_utils_mixin.py
--rw-r--r--   0 tom        (501) staff       (20)     4750 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/reports.py
--rw-r--r--   0 tom        (501) staff       (20)    20470 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/single_values.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.343454 django-advanced-report-builder-0.1.8/advanced_report_builder/views/targets/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/targets/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3021 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/targets/utils.py
--rw-r--r--   0 tom        (501) staff       (20)      898 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.8/advanced_report_builder/views/targets/views.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-06 12:37:21.344533 django-advanced-report-builder-0.1.8/django_advanced_report_builder.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)      683 2023-03-06 12:37:21.000000 django-advanced-report-builder-0.1.8/django_advanced_report_builder.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)    10752 2023-03-06 12:37:21.000000 django-advanced-report-builder-0.1.8/django_advanced_report_builder.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-06 12:37:21.000000 django-advanced-report-builder-0.1.8/django_advanced_report_builder.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)      149 2023-03-06 12:37:21.000000 django-advanced-report-builder-0.1.8/django_advanced_report_builder.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       24 2023-03-06 12:37:21.000000 django-advanced-report-builder-0.1.8/django_advanced_report_builder.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-03-06 12:37:21.345007 django-advanced-report-builder-0.1.8/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      974 2023-03-06 12:35:54.000000 django-advanced-report-builder-0.1.8/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.223733 django-advanced-report-builder-0.1.9/
+-rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       91 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)      683 2023-03-30 07:56:09.223515 django-advanced-report-builder-0.1.9/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      171 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.156204 django-advanced-report-builder-0.1.9/advanced_report_builder/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     4012 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/admin.py
+-rw-r--r--   0 tom        (501) staff       (20)      218 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/apps.py
+-rw-r--r--   0 tom        (501) staff       (20)     3394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/columns.py
+-rw-r--r--   0 tom        (501) staff       (20)       40 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/customise.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.157728 django-advanced-report-builder-0.1.9/advanced_report_builder/data_merge/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/data_merge/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3830 2023-03-06 12:34:46.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/data_merge/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)      951 2023-03-29 16:03:43.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/data_merge/widget.py
+-rw-r--r--   0 tom        (501) staff       (20)     5477 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/duplicate.py
+-rw-r--r--   0 tom        (501) staff       (20)      192 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/exceptions.py
+-rw-r--r--   0 tom        (501) staff       (20)    10853 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/field_types.py
+-rw-r--r--   0 tom        (501) staff       (20)    13799 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/filter_query.py
+-rw-r--r--   0 tom        (501) staff       (20)     7914 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/globals.py
+-rw-r--r--   0 tom        (501) staff       (20)     1315 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/includes.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.161951 django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)    14109 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)      591 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/0002_auto_20220209_1657.py
+-rw-r--r--   0 tom        (501) staff       (20)     1734 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/0003_auto_20220215_1219.py
+-rw-r--r--   0 tom        (501) staff       (20)      955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/0004_customreport.py
+-rw-r--r--   0 tom        (501) staff       (20)     3623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/0005_auto_20220303_0958.py
+-rw-r--r--   0 tom        (501) staff       (20)      914 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/0006_auto_20220310_1147.py
+-rw-r--r--   0 tom        (501) staff       (20)      607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/0007_auto_20220322_1939.py
+-rw-r--r--   0 tom        (501) staff       (20)      827 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/0008_auto_20220404_1144.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    18911 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/models.py
+-rw-r--r--   0 tom        (501) staff       (20)      532 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/report_builder.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.126205 django-advanced-report-builder-0.1.9/advanced_report_builder/static/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.131614 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.126643 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/chart-js/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.166525 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/chart-js/js/
+-rw-r--r--   0 tom        (501) staff       (20)   334540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js
+-rw-r--r--   0 tom        (501) staff       (20)   405847 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js
+-rw-r--r--   0 tom        (501) staff       (20)   193925 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js
+-rw-r--r--   0 tom        (501) staff       (20)     1430 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js
+-rw-r--r--   0 tom        (501) staff       (20)    12893 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.167216 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/
+-rw-r--r--   0 tom        (501) staff       (20)    72125 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js
+-rw-r--r--   0 tom        (501) staff       (20)     2352 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.127694 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/d3/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.171965 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/d3/js/
+-rw-r--r--   0 tom        (501) staff       (20)   575002 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js
+-rw-r--r--   0 tom        (501) staff       (20)   275533 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.127269 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/d3-funnel/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.168469 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/
+-rw-r--r--   0 tom        (501) staff       (20)   205600 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js
+-rw-r--r--   0 tom        (501) staff       (20)    58945 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.128090 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dashboard/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.175490 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dashboard/js/
+-rw-r--r--   0 tom        (501) staff       (20)      563 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.128746 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.181099 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/
+-rwxr-xr-x   0 tom        (501) staff       (20)      578 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore
+-rwxr-xr-x   0 tom        (501) staff       (20)      122 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/.travis.yml
+-rwxr-xr-x   0 tom        (501) staff       (20)     1176 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt
+-rwxr-xr-x   0 tom        (501) staff       (20)     3291 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.181452 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/bin/
+-rwxr-xr-x   0 tom        (501) staff       (20)     1442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer
+-rwxr-xr-x   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/bower.json
+-rwxr-xr-x   0 tom        (501) staff       (20)     5175 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3374 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1758 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     5190 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/index.js
+-rwxr-xr-x   0 tom        (501) staff       (20)      920 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/package.json
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.131277 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/jquery_extendext/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.182258 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/
+-rwxr-xr-x   0 tom        (501) staff       (20)     4390 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1324 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.133297 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.183450 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/css/
+-rwxr-xr-x   0 tom        (501) staff       (20)     3765 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css
+-rwxr-xr-x   0 tom        (501) staff       (20)     3253 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css
+-rwxr-xr-x   0 tom        (501) staff       (20)     3756 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css
+-rwxr-xr-x   0 tom        (501) staff       (20)     3248 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.189592 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/
+-rwxr-xr-x   0 tom        (501) staff       (20)     2962 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3082 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2494 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1431 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2309 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3273 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2672 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2662 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3216 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2917 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2952 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2522 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2299 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1412 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2645 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2787 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2451 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1310 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2627 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2782 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3062 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2503 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.191581 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/js/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.132970 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.191928 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/
+-rwxr-xr-x   0 tom        (501) staff       (20)     1212 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js
+-rwxr-xr-x   0 tom        (501) staff       (20)   191499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js
+-rwxr-xr-x   0 tom        (501) staff       (20)    72607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js
+-rwxr-xr-x   0 tom        (501) staff       (20)   201158 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js
+-rwxr-xr-x   0 tom        (501) staff       (20)    77072 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.192585 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/scss/
+-rwxr-xr-x   0 tom        (501) staff       (20)      442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/scss/dark.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)     3887 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.198601 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/
+-rwxr-xr-x   0 tom        (501) staff       (20)      266 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-checkbox.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-tooltip-errors.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_invert.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      469 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_sortable.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/bt-tooltip-errors.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/invert.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      465 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/sortable.scss
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.134043 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.199778 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.200675 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.200998 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/bar/
+-rw-r--r--   0 tom        (501) staff       (20)     4581 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.202077 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/funnel/
+-rw-r--r--   0 tom        (501) staff       (20)     1362 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)     1007 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.202542 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/line/
+-rw-r--r--   0 tom        (501) staff       (20)     4020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      486 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/modal.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.203022 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/pie/
+-rw-r--r--   0 tom        (501) staff       (20)     2084 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      858 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/report.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.203369 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/data_merge/
+-rw-r--r--   0 tom        (501) staff       (20)     2975 2023-03-29 15:59:37.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.205912 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/datatables/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.206761 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/datatables/fields/
+-rw-r--r--   0 tom        (501) staff       (20)      254 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/datatables/fields/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     3329 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html
+-rw-r--r--   0 tom        (501) staff       (20)      377 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/datatables/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)      593 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html
+-rw-r--r--   0 tom        (501) staff       (20)      256 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/datatables/query_modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     1127 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/datatables/report.html
+-rw-r--r--   0 tom        (501) staff       (20)     8185 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.208360 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/kanban/
+-rw-r--r--   0 tom        (501) staff       (20)      499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/kanban/description_modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     2038 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      308 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/kanban/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     1961 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/kanban/report.html
+-rw-r--r--   0 tom        (501) staff       (20)     3468 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/query_builder.html
+-rw-r--r--   0 tom        (501) staff       (20)     9491 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/select_column.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.209521 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/single_values/
+-rw-r--r--   0 tom        (501) staff       (20)     1896 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     1643 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/single_values/report.html
+-rw-r--r--   0 tom        (501) staff       (20)      327 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/toggle.py
+-rw-r--r--   0 tom        (501) staff       (20)     3830 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/urls.py
+-rw-r--r--   0 tom        (501) staff       (20)     4447 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)    12521 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/variable_date.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.216150 django-advanced-report-builder-0.1.9/advanced_report_builder/views/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    11541 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/bar_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)    16346 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/charts_base.py
+-rw-r--r--   0 tom        (501) staff       (20)     3020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/custom.py
+-rw-r--r--   0 tom        (501) staff       (20)     8659 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/dashboard.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.219152 django-advanced-report-builder-0.1.9/advanced_report_builder/views/datatables/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/datatables/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     6801 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/datatables/datatables.py
+-rw-r--r--   0 tom        (501) staff       (20)    25412 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/datatables/modal.py
+-rw-r--r--   0 tom        (501) staff       (20)    11394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/datatables/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     8725 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/funnel_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)    32161 2023-03-29 16:04:49.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/kanban.py
+-rw-r--r--   0 tom        (501) staff       (20)    12979 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/line_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)    21031 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/modals_base.py
+-rw-r--r--   0 tom        (501) staff       (20)     8686 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/pie_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/report.py
+-rw-r--r--   0 tom        (501) staff       (20)     7812 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/report_utils_mixin.py
+-rw-r--r--   0 tom        (501) staff       (20)     4750 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/reports.py
+-rw-r--r--   0 tom        (501) staff       (20)    20470 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/single_values.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.220764 django-advanced-report-builder-0.1.9/advanced_report_builder/views/targets/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/targets/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3021 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/targets/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)      898 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.1.9/advanced_report_builder/views/targets/views.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-03-30 07:56:09.223170 django-advanced-report-builder-0.1.9/django_advanced_report_builder.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)      683 2023-03-30 07:56:09.000000 django-advanced-report-builder-0.1.9/django_advanced_report_builder.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)    10752 2023-03-30 07:56:09.000000 django-advanced-report-builder-0.1.9/django_advanced_report_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-03-30 07:56:09.000000 django-advanced-report-builder-0.1.9/django_advanced_report_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)      149 2023-03-30 07:56:09.000000 django-advanced-report-builder-0.1.9/django_advanced_report_builder.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       24 2023-03-30 07:56:09.000000 django-advanced-report-builder-0.1.9/django_advanced_report_builder.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-03-30 07:56:09.223791 django-advanced-report-builder-0.1.9/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      974 2023-03-29 15:59:37.000000 django-advanced-report-builder-0.1.9/setup.py
```

### Comparing `django-advanced-report-builder-0.1.8/LICENSE` & `django-advanced-report-builder-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/PKG-INFO` & `django-advanced-report-builder-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-report-builder
-Version: 0.1.8
+Version: 0.1.9
 Summary: Django app that allows you to build reports from modals
 Home-page: https://github.com/django-advance-utils/django-advanced-report-builder
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/admin.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/admin.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/columns.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/columns.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/data_merge/utils.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/data_merge/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/duplicate.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/duplicate.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/field_types.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/field_types.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/filter_query.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/filter_query.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/globals.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/globals.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/includes.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/includes.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/0001_initial.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/0002_auto_20220209_1657.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/0002_auto_20220209_1657.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/0003_auto_20220215_1219.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/0003_auto_20220215_1219.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/0004_customreport.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/0004_customreport.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/0005_auto_20220303_0958.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/0005_auto_20220303_0958.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/0006_auto_20220310_1147.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/0006_auto_20220310_1147.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/0007_auto_20220322_1939.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/0007_auto_20220322_1939.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/migrations/0008_auto_20220404_1144.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/migrations/0008_auto_20220404_1144.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/models.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/models.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/report_builder.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/report_builder.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/README.md` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/README.md`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/index.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/index.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/dot/js/package.json` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/dot/js/package.json`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss` & `django-advanced-report-builder-0.1.9/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/charts/report.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/charts/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <textarea name="{{ widget.name }}" id="{{ widget.attrs.id }}_textarea">{{ widget.value }}</textarea>
 
 <script>
 
     function setup_tiny_{{ widget.attrs.id }}() {
         tinymce.init({
             selector: '#{{ widget.attrs.id }}_textarea',
-            height: 150,
+            height: {{ height }},
             menubar: false,
             content_css: [
                 '//fonts.googleapis.com/css?family=Lato:300,300i,400,400i'],
             {% if disabled %}readonly : 1,
                 toolbar: ' | '{% else %}
             forced_root_block: '',
             force_br_newlines: true,
```

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/datatables/report.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/datatables/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/kanban/report.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/kanban/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/query_builder.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/query_builder.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/select_column.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/select_column.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/templates/advanced_report_builder/single_values/report.html` & `django-advanced-report-builder-0.1.9/advanced_report_builder/templates/advanced_report_builder/single_values/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/urls.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/urls.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/utils.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/variable_date.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/variable_date.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/views/bar_charts.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/views/bar_charts.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/views/charts_base.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/views/charts_base.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/views/custom.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/views/custom.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/views/dashboard.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/views/dashboard.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/views/datatables/datatables.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/views/datatables/datatables.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/views/datatables/modal.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/views/datatables/modal.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/views/datatables/utils.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/views/datatables/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/views/funnel_charts.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/views/funnel_charts.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/views/kanban.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/views/kanban.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/views/line_charts.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/views/line_charts.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/views/modals_base.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/views/modals_base.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/views/pie_charts.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/views/pie_charts.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/views/report_utils_mixin.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/views/report_utils_mixin.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/views/reports.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/views/reports.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/views/single_values.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/views/single_values.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/views/targets/utils.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/views/targets/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/advanced_report_builder/views/targets/views.py` & `django-advanced-report-builder-0.1.9/advanced_report_builder/views/targets/views.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/django_advanced_report_builder.egg-info/PKG-INFO` & `django-advanced-report-builder-0.1.9/django_advanced_report_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-report-builder
-Version: 0.1.8
+Version: 0.1.9
 Summary: Django app that allows you to build reports from modals
 Home-page: https://github.com/django-advance-utils/django-advanced-report-builder
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-advanced-report-builder-0.1.8/django_advanced_report_builder.egg-info/SOURCES.txt` & `django-advanced-report-builder-0.1.9/django_advanced_report_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.1.8/setup.py` & `django-advanced-report-builder-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-advanced-report-builder",
-    version="0.1.8",
+    version="0.1.9",
     author="Thomas Turner",
     description="Django app that allows you to build reports from modals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/django-advance-utils/django-advanced-report-builder",
     include_package_data=True,
     packages=['advanced_report_builder'],
```

