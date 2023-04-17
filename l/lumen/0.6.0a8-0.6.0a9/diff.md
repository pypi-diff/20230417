# Comparing `tmp/lumen-0.6.0a8.tar.gz` & `tmp/lumen-0.6.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumen-0.6.0a8.tar", last modified: Tue Feb  7 14:55:34 2023, max compression
+gzip compressed data, was "lumen-0.6.0a9.tar", last modified: Fri Feb 10 16:35:54 2023, max compression
```

## Comparing `lumen-0.6.0a8.tar` & `lumen-0.6.0a9.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.210555 lumen-0.6.0a8/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-02-07 14:46:50.000000 lumen-0.6.0a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-07 14:46:50.000000 lumen-0.6.0a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-02-07 14:55:34.210555 lumen-0.6.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-02-07 14:46:50.000000 lumen-0.6.0a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.194555 lumen-0.6.0a8/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.194555 lumen-0.6.0a8/examples/gallery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.194555 lumen-0.6.0a8/examples/gallery/bikes/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-02-07 14:46:50.000000 lumen-0.6.0a8/examples/gallery/bikes/bikes.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.194555 lumen-0.6.0a8/examples/gallery/earthquakes/
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-02-07 14:46:50.000000 lumen-0.6.0a8/examples/gallery/earthquakes/earthquakes.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.194555 lumen-0.6.0a8/examples/gallery/nyc_taxi/
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-02-07 14:46:50.000000 lumen-0.6.0a8/examples/gallery/nyc_taxi/nyc_taxi.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.194555 lumen-0.6.0a8/examples/gallery/penguins/
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-02-07 14:46:50.000000 lumen-0.6.0a8/examples/gallery/penguins/penguins.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.194555 lumen-0.6.0a8/examples/gallery/precip/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-02-07 14:46:50.000000 lumen-0.6.0a8/examples/gallery/precip/precipitation.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.194555 lumen-0.6.0a8/examples/gallery/seattle/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-02-07 14:46:50.000000 lumen-0.6.0a8/examples/gallery/seattle/weather.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.194555 lumen-0.6.0a8/examples/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-02-07 14:46:50.000000 lumen-0.6.0a8/examples/user_guide/Pipeline.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.198555 lumen-0.6.0a8/lumen/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-07 14:55:34.000000 lumen-0.6.0a8/lumen/.version
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    21549 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.198555 lumen-0.6.0a8/lumen/command/
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/command/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/command/precache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/command/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    41383 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.198555 lumen-0.6.0a8/lumen/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20085 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    39414 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.198555 lumen-0.6.0a8/lumen/sources/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/sources/ae5.py
--rw-r--r--   0 runner    (1001) docker     (123)    38963 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/sources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/sources/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/sources/intake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/sources/intake_dremio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/sources/intake_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/sources/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.202555 lumen-0.6.0a8/lumen/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.202555 lumen-0.6.0a8/lumen/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/filters/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.202555 lumen-0.6.0a8/lumen/tests/sample_dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sample_dashboard/dashboard.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sample_dashboard/dashboard_legacy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sample_dashboard/source_nested_variable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sample_dashboard/source_variable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sample_dashboard/sql_dashboard.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sample_dashboard/sync_query.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sample_dashboard/sync_query_filters.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sample_dashboard/transform_variable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sample_dashboard/view_transform_variable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sample_dashboard/view_variable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sample_dashboard/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.202555 lumen-0.6.0a8/lumen/tests/sources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sources/catalog.yml
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sources/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sources/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sources/test.db
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sources/test2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sources/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sources/test_derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sources/test_duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sources/test_intake.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/sources/test_intake_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/test_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.202555 lumen-0.6.0a8/lumen/tests/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/transforms/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/transforms/test_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.202555 lumen-0.6.0a8/lumen/tests/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/validation/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/validation/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/validation/test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/validation/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/validation/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/validation/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/validation/test_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/validation/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.206555 lumen-0.6.0a8/lumen/tests/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/tests/views/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.206555 lumen-0.6.0a8/lumen/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26661 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/transforms/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.206555 lumen-0.6.0a8/lumen/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.206555 lumen-0.6.0a8/lumen/ui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    82521 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/assets/csv.png
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/assets/dashboard.png
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/assets/hvplot.png
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/assets/intake.png
--rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/assets/parquet.png
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/assets/perspective.png
--rw-r--r--   0 runner    (1001) docker     (123)    64978 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/assets/rest.png
--rw-r--r--   0 runner    (1001) docker     (123)    31192 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/assets/source.png
--rw-r--r--   0 runner    (1001) docker     (123)    26341 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/assets/tabulator.png
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/assets/target.png
--rw-r--r--   0 runner    (1001) docker     (123)    17518 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/assets/view.png
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/fast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/gallery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    18865 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    13253 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/ui/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.206555 lumen-0.6.0a8/lumen/variables/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15695 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/variables/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.210555 lumen-0.6.0a8/lumen/views/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37761 2023-02-07 14:46:50.000000 lumen-0.6.0a8/lumen/views/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 14:55:34.198555 lumen-0.6.0a8/lumen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-02-07 14:55:34.000000 lumen-0.6.0a8/lumen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-02-07 14:55:34.000000 lumen-0.6.0a8/lumen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 14:55:34.000000 lumen-0.6.0a8/lumen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-07 14:55:34.000000 lumen-0.6.0a8/lumen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-02-07 14:55:34.000000 lumen-0.6.0a8/lumen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-07 14:55:34.000000 lumen-0.6.0a8/lumen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-07 14:46:50.000000 lumen-0.6.0a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-07 14:55:34.210555 lumen-0.6.0a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-02-07 14:46:50.000000 lumen-0.6.0a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.735489 lumen-0.6.0a9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-02-10 16:27:32.000000 lumen-0.6.0a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-10 16:27:32.000000 lumen-0.6.0a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-02-10 16:35:54.735489 lumen-0.6.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-02-10 16:27:32.000000 lumen-0.6.0a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.715489 lumen-0.6.0a9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.715489 lumen-0.6.0a9/examples/gallery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.719489 lumen-0.6.0a9/examples/gallery/bikes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-02-10 16:27:32.000000 lumen-0.6.0a9/examples/gallery/bikes/bikes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.719489 lumen-0.6.0a9/examples/gallery/earthquakes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-02-10 16:27:32.000000 lumen-0.6.0a9/examples/gallery/earthquakes/earthquakes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.719489 lumen-0.6.0a9/examples/gallery/nyc_taxi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-02-10 16:27:32.000000 lumen-0.6.0a9/examples/gallery/nyc_taxi/nyc_taxi.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.719489 lumen-0.6.0a9/examples/gallery/penguins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-02-10 16:27:32.000000 lumen-0.6.0a9/examples/gallery/penguins/penguins.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.719489 lumen-0.6.0a9/examples/gallery/precip/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-02-10 16:27:32.000000 lumen-0.6.0a9/examples/gallery/precip/precipitation.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.719489 lumen-0.6.0a9/examples/gallery/seattle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-02-10 16:27:32.000000 lumen-0.6.0a9/examples/gallery/seattle/weather.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.719489 lumen-0.6.0a9/examples/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-02-10 16:27:32.000000 lumen-0.6.0a9/examples/user_guide/Pipeline.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.723489 lumen-0.6.0a9/lumen/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-10 16:35:54.000000 lumen-0.6.0a9/lumen/.version
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21549 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.723489 lumen-0.6.0a9/lumen/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/command/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/command/precache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/command/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41383 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.723489 lumen-0.6.0a9/lumen/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20085 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39414 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.723489 lumen-0.6.0a9/lumen/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/sources/ae5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38963 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/sources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/sources/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/sources/intake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/sources/intake_dremio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/sources/intake_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/sources/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14171 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.727489 lumen-0.6.0a9/lumen/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.727489 lumen-0.6.0a9/lumen/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/filters/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.727489 lumen-0.6.0a9/lumen/tests/sample_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sample_dashboard/dashboard.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sample_dashboard/dashboard_legacy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sample_dashboard/source_nested_variable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sample_dashboard/source_variable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sample_dashboard/sql_dashboard.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sample_dashboard/sync_query.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sample_dashboard/sync_query_filters.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sample_dashboard/transform_variable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sample_dashboard/view_transform_variable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sample_dashboard/view_variable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sample_dashboard/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.727489 lumen-0.6.0a9/lumen/tests/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sources/catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sources/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sources/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sources/test.db
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sources/test2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sources/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sources/test_derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sources/test_duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sources/test_intake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/sources/test_intake_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.731489 lumen-0.6.0a9/lumen/tests/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/transforms/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/transforms/test_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.731489 lumen-0.6.0a9/lumen/tests/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/validation/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/validation/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/validation/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/validation/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/validation/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/validation/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/validation/test_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/validation/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.731489 lumen-0.6.0a9/lumen/tests/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/tests/views/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.731489 lumen-0.6.0a9/lumen/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26661 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/transforms/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.735489 lumen-0.6.0a9/lumen/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.735489 lumen-0.6.0a9/lumen/ui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    82521 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/assets/csv.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/assets/dashboard.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/assets/hvplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/assets/intake.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/assets/parquet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/assets/perspective.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64978 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/assets/rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31192 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/assets/source.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26341 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/assets/tabulator.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/assets/target.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17518 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/assets/view.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/fast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18865 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13253 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/ui/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.735489 lumen-0.6.0a9/lumen/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15695 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/variables/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.735489 lumen-0.6.0a9/lumen/views/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37776 2023-02-10 16:27:32.000000 lumen-0.6.0a9/lumen/views/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:35:54.723489 lumen-0.6.0a9/lumen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-02-10 16:35:54.000000 lumen-0.6.0a9/lumen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-02-10 16:35:54.000000 lumen-0.6.0a9/lumen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 16:35:54.000000 lumen-0.6.0a9/lumen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-10 16:35:54.000000 lumen-0.6.0a9/lumen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-02-10 16:35:54.000000 lumen-0.6.0a9/lumen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-10 16:35:54.000000 lumen-0.6.0a9/lumen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-10 16:27:32.000000 lumen-0.6.0a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-10 16:35:54.735489 lumen-0.6.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-02-10 16:27:32.000000 lumen-0.6.0a9/setup.py
```

### Comparing `lumen-0.6.0a8/LICENSE` & `lumen-0.6.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/PKG-INFO` & `lumen-0.6.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumen
-Version: 0.6.0a8
+Version: 0.6.0a9
 Summary: A monitoring solution built on Panel.
 Home-page: https://github.com/holoviz/lumen
 Author: HoloViz
 Author-email: developers@holoviz.org
 Maintainer: HoloViz
 Maintainer-email: developers@holoviz.org
 License: BSD
```

### Comparing `lumen-0.6.0a8/README.md` & `lumen-0.6.0a9/README.md`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/examples/gallery/bikes/bikes.yaml` & `lumen-0.6.0a9/examples/gallery/bikes/bikes.yaml`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/examples/gallery/earthquakes/earthquakes.yaml` & `lumen-0.6.0a9/examples/gallery/earthquakes/earthquakes.yaml`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/examples/gallery/nyc_taxi/nyc_taxi.yaml` & `lumen-0.6.0a9/examples/gallery/nyc_taxi/nyc_taxi.yaml`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/examples/gallery/penguins/penguins.yaml` & `lumen-0.6.0a9/examples/gallery/penguins/penguins.yaml`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/examples/gallery/precip/precipitation.yaml` & `lumen-0.6.0a9/examples/gallery/precip/precipitation.yaml`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/examples/gallery/seattle/weather.yaml` & `lumen-0.6.0a9/examples/gallery/seattle/weather.yaml`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/examples/user_guide/Pipeline.ipynb` & `lumen-0.6.0a9/examples/user_guide/Pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/auth.py` & `lumen-0.6.0a9/lumen/auth.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/base.py` & `lumen-0.6.0a9/lumen/base.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/command/__init__.py` & `lumen-0.6.0a9/lumen/command/__init__.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/command/builder.py` & `lumen-0.6.0a9/lumen/command/builder.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/command/precache.py` & `lumen-0.6.0a9/lumen/command/precache.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/command/validate.py` & `lumen-0.6.0a9/lumen/command/validate.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/config.py` & `lumen-0.6.0a9/lumen/config.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/dashboard.py` & `lumen-0.6.0a9/lumen/dashboard.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/filters/base.py` & `lumen-0.6.0a9/lumen/filters/base.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/layout.py` & `lumen-0.6.0a9/lumen/layout.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/panel.py` & `lumen-0.6.0a9/lumen/panel.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/pipeline.py` & `lumen-0.6.0a9/lumen/pipeline.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/rest.py` & `lumen-0.6.0a9/lumen/rest.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/schema.py` & `lumen-0.6.0a9/lumen/schema.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/sources/ae5.py` & `lumen-0.6.0a9/lumen/sources/ae5.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/sources/base.py` & `lumen-0.6.0a9/lumen/sources/base.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/sources/duckdb.py` & `lumen-0.6.0a9/lumen/sources/duckdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,17 +97,15 @@
             enums, min_maxes = [], []
             for name, col_schema in schema.items():
                 if 'enum' in col_schema:
                     enums.append(name)
                 elif 'inclusiveMinimum' in col_schema:
                     min_maxes.append(name)
             for col in enums:
-                distinct_expr = sql_expr
-                for sql_t in (SQLDistinct(columns=[col]), SQLLimit(limit=1000)):
-                    distinct_expr = sql_t.apply(distinct_expr)
+                distinct_expr = SQLDistinct(columns=[col]).apply(sql_expr)
                 distinct_expr = ' '.join(distinct_expr.splitlines())
                 distinct = self._connection.execute(distinct_expr).fetch_df()
                 schema[col]['enum'] = distinct[col].tolist()
 
             minmax_expr = SQLMinMax(columns=min_maxes).apply(sql_expr)
             minmax_expr = ' '.join(minmax_expr.splitlines())
             minmax_data = self._connection.execute(minmax_expr).fetch_df()
```

### Comparing `lumen-0.6.0a8/lumen/sources/intake.py` & `lumen-0.6.0a9/lumen/sources/intake.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/sources/intake_dremio.py` & `lumen-0.6.0a9/lumen/sources/intake_dremio.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/sources/intake_sql.py` & `lumen-0.6.0a9/lumen/sources/intake_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,15 @@
             enums, min_maxes = [], []
             for name, col_schema in schema.items():
                 if 'enum' in col_schema:
                     enums.append(name)
                 elif 'inclusiveMinimum' in col_schema:
                     min_maxes.append(name)
             for col in enums:
-                distinct_transforms = [
-                    SQLDistinct(columns=[col]), SQLLimit(limit=1000)
-                ]
+                distinct_transforms = [SQLDistinct(columns=[col])]
                 distinct = self._read(
                     self._apply_transforms(source, distinct_transforms)
                 )
                 schema[col]['enum'] = distinct[col].to_list()
             minmax_data = self._read(
                 self._apply_transforms(source, [SQLMinMax(columns=min_maxes)])
             )
```

### Comparing `lumen-0.6.0a8/lumen/sources/prometheus.py` & `lumen-0.6.0a9/lumen/sources/prometheus.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/state.py` & `lumen-0.6.0a9/lumen/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing import (
     TYPE_CHECKING, Any, Dict, List, Tuple, cast,
 )
 from weakref import WeakKeyDictionary
 
 import panel as pn
+import yaml
 
 from .util import extract_refs, is_ref
 
 if TYPE_CHECKING:
     from bokeh.document import Document  # type: ignore
 
     from .dashboard import Config
@@ -141,15 +142,15 @@
                 for name, (spec, schema) in filters.items()
             }
             for source, filters in self.global_filters.items()
         }
 
     def to_spec(
         self, auth=None, config=None, defaults=None,
-        pipelines={}, sources={}, layouts=[], variables=None
+        pipelines={}, sources={}, layouts=[], variables=None,
     ):
         """
         Exports the full specification of the supplied components including
         the variable definitions.
 
         Parameters
         ----------
@@ -199,14 +200,30 @@
             context['pipelines'][k] = pipeline.to_spec(context=context)
         if layouts:
             context['layouts'] = [
                 layout.to_spec(context) for layout in layouts
             ]
         return context
 
+    def save_spec(self, filename, **to_spec_kwargs):
+        """Exports the full specification of the supplied components including
+        the variable definitions to a file.
+
+
+        Parameters
+        ----------
+        filename: str | None
+        to_spec_kwargs: parameters passed to lumen.state.to_spec.
+
+        """
+        context = self.to_spec(**to_spec_kwargs)
+
+        with open(filename, 'w') as f:
+            yaml.dump(context, f)
+
     @property
     def global_refs(self) -> List[str]:
         layout_refs = []
         source_specs = self.spec.get('sources', {})
         for layout in self.spec.get('layouts', []):
             if isinstance(layout.get('source'), str):
                 src_ref = layout['source']
```

### Comparing `lumen-0.6.0a8/lumen/tests/conftest.py` & `lumen-0.6.0a9/lumen/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/filters/test_base.py` & `lumen-0.6.0a9/lumen/tests/filters/test_base.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/sample_dashboard/sql_dashboard.yaml` & `lumen-0.6.0a9/lumen/tests/sample_dashboard/sql_dashboard.yaml`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/sources/catalog.yml` & `lumen-0.6.0a9/lumen/tests/sources/catalog.yml`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/sources/test.db` & `lumen-0.6.0a9/lumen/tests/sources/test.db`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/sources/test_base.py` & `lumen-0.6.0a9/lumen/tests/sources/test_base.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/sources/test_derived.py` & `lumen-0.6.0a9/lumen/tests/sources/test_derived.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/sources/test_duckdb.py` & `lumen-0.6.0a9/lumen/tests/sources/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/sources/test_intake.py` & `lumen-0.6.0a9/lumen/tests/sources/test_intake.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/sources/test_intake_sql.py` & `lumen-0.6.0a9/lumen/tests/sources/test_intake_sql.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/test_auth.py` & `lumen-0.6.0a9/lumen/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/test_config.py` & `lumen-0.6.0a9/lumen/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/test_dashboard.py` & `lumen-0.6.0a9/lumen/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/test_layout.py` & `lumen-0.6.0a9/lumen/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/test_pipeline.py` & `lumen-0.6.0a9/lumen/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/test_schema.py` & `lumen-0.6.0a9/lumen/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/test_variables.py` & `lumen-0.6.0a9/lumen/tests/test_variables.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/transforms/test_base.py` & `lumen-0.6.0a9/lumen/tests/transforms/test_base.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/transforms/test_sql.py` & `lumen-0.6.0a9/lumen/tests/transforms/test_sql.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/validation/test_dashboard.py` & `lumen-0.6.0a9/lumen/tests/validation/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/validation/test_filters.py` & `lumen-0.6.0a9/lumen/tests/validation/test_filters.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/validation/test_layout.py` & `lumen-0.6.0a9/lumen/tests/validation/test_layout.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/validation/test_pipeline.py` & `lumen-0.6.0a9/lumen/tests/validation/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/validation/test_sources.py` & `lumen-0.6.0a9/lumen/tests/validation/test_sources.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/validation/test_transform.py` & `lumen-0.6.0a9/lumen/tests/validation/test_transform.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/validation/test_views.py` & `lumen-0.6.0a9/lumen/tests/validation/test_views.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/tests/views/test_base.py` & `lumen-0.6.0a9/lumen/tests/views/test_base.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/transforms/base.py` & `lumen-0.6.0a9/lumen/transforms/base.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/transforms/sql.py` & `lumen-0.6.0a9/lumen/transforms/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,16 @@
                 condition = ' OR '.join([
                     self._range_filter(col, v1, v2) for v1, v2 in val
                 ])
             elif isinstance(val, list):
                 if not val:
                     continue
                 non_null = [v for v in val if v is not None]
-                condition = f"{col} IN ({', '.join(map(repr, non_null))})"
+                str_non_null = "', '".join(n.replace("'", '\\\'') for n in non_null)
+                condition = f"{col} IN ('{str_non_null}')"
                 if not non_null:
                     condition = f'{col} IS NULL'
                 elif len(val) != len(non_null):
                     condition = f'({condition}) OR ({col} IS NULL)'
             elif isinstance(val, tuple):
                 condition = self._range_filter(col, *val)
             else:
```

### Comparing `lumen-0.6.0a8/lumen/ui/assets/csv.png` & `lumen-0.6.0a9/lumen/ui/assets/csv.png`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/assets/dashboard.png` & `lumen-0.6.0a9/lumen/ui/assets/dashboard.png`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/assets/hvplot.png` & `lumen-0.6.0a9/lumen/ui/assets/hvplot.png`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/assets/intake.png` & `lumen-0.6.0a9/lumen/ui/assets/intake.png`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/assets/parquet.png` & `lumen-0.6.0a9/lumen/ui/assets/parquet.png`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/assets/perspective.png` & `lumen-0.6.0a9/lumen/ui/assets/perspective.png`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/assets/rest.png` & `lumen-0.6.0a9/lumen/ui/assets/rest.png`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/assets/source.png` & `lumen-0.6.0a9/lumen/ui/assets/source.png`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/assets/tabulator.png` & `lumen-0.6.0a9/lumen/ui/assets/tabulator.png`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/assets/target.png` & `lumen-0.6.0a9/lumen/ui/assets/target.png`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/assets/view.png` & `lumen-0.6.0a9/lumen/ui/assets/view.png`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/base.py` & `lumen-0.6.0a9/lumen/ui/base.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/builder.py` & `lumen-0.6.0a9/lumen/ui/builder.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/config.py` & `lumen-0.6.0a9/lumen/ui/config.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/dashboard.py` & `lumen-0.6.0a9/lumen/ui/dashboard.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/fast.py` & `lumen-0.6.0a9/lumen/ui/fast.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/gallery.py` & `lumen-0.6.0a9/lumen/ui/gallery.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/launcher.py` & `lumen-0.6.0a9/lumen/ui/launcher.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/layouts.py` & `lumen-0.6.0a9/lumen/ui/layouts.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/main.py` & `lumen-0.6.0a9/lumen/ui/main.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/pipeline.py` & `lumen-0.6.0a9/lumen/ui/pipeline.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/sources.py` & `lumen-0.6.0a9/lumen/ui/sources.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/state.py` & `lumen-0.6.0a9/lumen/ui/state.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/variables.py` & `lumen-0.6.0a9/lumen/ui/variables.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/ui/views.py` & `lumen-0.6.0a9/lumen/ui/views.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/util.py` & `lumen-0.6.0a9/lumen/util.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/validation.py` & `lumen-0.6.0a9/lumen/validation.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/variables/base.py` & `lumen-0.6.0a9/lumen/variables/base.py`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/lumen/views/base.py` & `lumen-0.6.0a9/lumen/views/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1066,8 +1066,8 @@
             encoded = encoded.properties(**self.properties)
         return dict(object=encoded, **self.kwargs)
 
     def get_panel(self) -> pn.pane.Vega:
         return pn.pane.Vega(**self._get_params())
 
 
-__all__ = [name for name, obj in locals().items() if isinstance(obj, type) and issubclass(obj, View)]
+__all__ = [name for name, obj in locals().items() if isinstance(obj, type) and issubclass(obj, View)] + ["Download"]
```

### Comparing `lumen-0.6.0a8/lumen.egg-info/PKG-INFO` & `lumen-0.6.0a9/lumen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumen
-Version: 0.6.0a8
+Version: 0.6.0a9
 Summary: A monitoring solution built on Panel.
 Home-page: https://github.com/holoviz/lumen
 Author: HoloViz
 Author-email: developers@holoviz.org
 Maintainer: HoloViz
 Maintainer-email: developers@holoviz.org
 License: BSD
```

### Comparing `lumen-0.6.0a8/lumen.egg-info/SOURCES.txt` & `lumen-0.6.0a9/lumen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lumen-0.6.0a8/setup.py` & `lumen-0.6.0a9/setup.py`

 * *Files identical despite different names*

