# Comparing `tmp/dataflows-0.3.7.tar.gz` & `tmp/dataflows-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataflows-0.3.7.tar", last modified: Sun Oct 17 15:58:24 2021, max compression
+gzip compressed data, was "dataflows-0.3.8.tar", last modified: Mon Oct 18 12:34:41 2021, max compression
```

## Comparing `dataflows-0.3.7.tar` & `dataflows-0.3.8.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 15:58:24.500895 dataflows-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-10-17 15:58:19.000000 dataflows-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      159 2021-10-17 15:58:19.000000 dataflows-0.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      614 2021-10-17 15:58:19.000000 dataflows-0.3.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     6415 2021-10-17 15:58:24.500895 dataflows-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4987 2021-10-17 15:58:19.000000 dataflows-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 15:58:24.492895 dataflows-0.3.7/dataflows/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      221 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 15:58:24.492895 dataflows-0.3.7/dataflows/base/
--rw-r--r--   0 runner    (1001) docker     (121)      291 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      451 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/base/datastream.py
--rw-r--r--   0 runner    (1001) docker     (121)     3958 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/base/datastream_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/base/flow.py
--rw-r--r--   0 runner    (1001) docker     (121)      241 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/base/package_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)      265 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/base/resource_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2340 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/base/schema_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)     8745 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 15:58:24.492895 dataflows-0.3.7/dataflows/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)      232 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      633 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/helpers/datapackage_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4143 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/helpers/extended_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     3727 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/helpers/iterable_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)      947 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/helpers/resource_matcher.py
--rw-r--r--   0 runner    (1001) docker     (121)      308 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/helpers/resources_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)      337 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/helpers/row_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/helpers/rows_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 15:58:24.496894 dataflows-0.3.7/dataflows/processors/
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3274 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/add_computed_field.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/add_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     4475 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (121)      503 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/conditional.py
--rw-r--r--   0 runner    (1001) docker     (121)      849 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/deduplicate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/delete_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 15:58:24.500895 dataflows-0.3.7/dataflows/processors/dumpers/
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/dumpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4238 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/dumpers/dumper_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6388 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/dumpers/file_dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 15:58:24.500895 dataflows-0.3.7/dataflows/processors/dumpers/formats/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/dumpers/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2560 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/dumpers/formats/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2675 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/dumpers/formats/format_csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2949 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/dumpers/formats/format_excel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1354 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/dumpers/formats/format_geojson.py
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/dumpers/formats/format_json.py
--rw-r--r--   0 runner    (1001) docker     (121)      721 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/dumpers/to_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     5712 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/dumpers/to_sql.py
--rw-r--r--   0 runner    (1001) docker     (121)      620 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/dumpers/to_zip.py
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/filter_rows.py
--rw-r--r--   0 runner    (1001) docker     (121)      576 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/finalizer.py
--rw-r--r--   0 runner    (1001) docker     (121)      738 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/find_replace.py
--rw-r--r--   0 runner    (1001) docker     (121)    14021 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/join.py
--rw-r--r--   0 runner    (1001) docker     (121)    11349 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/load.py
--rw-r--r--   0 runner    (1001) docker     (121)     3278 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/parallelize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 15:58:24.500895 dataflows-0.3.7/dataflows/processors/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2299 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/parsers/excel_xml_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1994 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/parsers/sql_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/parsers/xml_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2342 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/printer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/rename_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/select_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)      652 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/set_primary_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     2554 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/set_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     2224 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/sort_rows.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/sources.py
--rw-r--r--   0 runner    (1001) docker     (121)      826 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/stream.py
--rw-r--r--   0 runner    (1001) docker     (121)     3372 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/unpivot.py
--rw-r--r--   0 runner    (1001) docker     (121)      651 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/unstream.py
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/update_package.py
--rw-r--r--   0 runner    (1001) docker     (121)      604 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/update_resource.py
--rw-r--r--   0 runner    (1001) docker     (121)      627 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/update_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      137 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/update_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/processors/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 15:58:24.500895 dataflows-0.3.7/dataflows/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     3324 2021-10-17 15:58:19.000000 dataflows-0.3.7/dataflows/templates/main.tpl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 15:58:24.492895 dataflows-0.3.7/dataflows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6415 2021-10-17 15:58:24.000000 dataflows-0.3.7/dataflows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2708 2021-10-17 15:58:24.000000 dataflows-0.3.7/dataflows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-17 15:58:24.000000 dataflows-0.3.7/dataflows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-10-17 15:58:24.000000 dataflows-0.3.7/dataflows.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-17 15:58:24.000000 dataflows-0.3.7/dataflows.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      264 2021-10-17 15:58:24.000000 dataflows-0.3.7/dataflows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-10-17 15:58:24.000000 dataflows-0.3.7/dataflows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-10-17 15:58:24.500895 dataflows-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2169 2021-10-17 15:58:19.000000 dataflows-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 12:34:41.759094 dataflows-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-10-18 12:34:37.000000 dataflows-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2021-10-18 12:34:37.000000 dataflows-0.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      614 2021-10-18 12:34:37.000000 dataflows-0.3.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     6415 2021-10-18 12:34:41.759094 dataflows-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4987 2021-10-18 12:34:37.000000 dataflows-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 12:34:41.755094 dataflows-0.3.8/dataflows/
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/VERSION
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 12:34:41.755094 dataflows-0.3.8/dataflows/base/
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      451 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/base/datastream.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3958 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/base/datastream_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      612 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2027 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/base/flow.py
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/base/package_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/base/resource_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2340 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/base/schema_validator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8745 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 12:34:41.755094 dataflows-0.3.8/dataflows/helpers/
+-rw-r--r--   0 runner    (1001) docker     (121)      232 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      633 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/helpers/datapackage_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4143 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/helpers/extended_json.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3727 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/helpers/iterable_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)      947 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/helpers/resource_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/helpers/resources_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/helpers/row_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/helpers/rows_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 12:34:41.759094 dataflows-0.3.8/dataflows/processors/
+-rw-r--r--   0 runner    (1001) docker     (121)     1133 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3274 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/add_computed_field.py
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/add_field.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1486 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4475 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (121)      503 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (121)      849 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/deduplicate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1795 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/delete_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 12:34:41.759094 dataflows-0.3.8/dataflows/processors/dumpers/
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/dumpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4238 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/dumpers/dumper_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6388 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/dumpers/file_dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 12:34:41.759094 dataflows-0.3.8/dataflows/processors/dumpers/formats/
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/dumpers/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2560 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/dumpers/formats/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2675 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/dumpers/formats/format_csv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2949 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/dumpers/formats/format_excel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1354 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/dumpers/formats/format_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1945 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/dumpers/formats/format_json.py
+-rw-r--r--   0 runner    (1001) docker     (121)      721 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/dumpers/to_path.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5712 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/dumpers/to_sql.py
+-rw-r--r--   0 runner    (1001) docker     (121)      620 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/dumpers/to_zip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1949 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/filter_rows.py
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/finalizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/find_replace.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14021 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/join.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11349 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/load.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3278 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/parallelize.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 12:34:41.759094 dataflows-0.3.8/dataflows/processors/parsers/
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2299 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/parsers/excel_xml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1994 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/parsers/sql_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1588 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/parsers/xml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2342 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/printer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2208 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/rename_fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1901 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/select_fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)      652 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/set_primary_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2666 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/set_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2224 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/sort_rows.py
+-rw-r--r--   0 runner    (1001) docker     (121)      956 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/sources.py
+-rw-r--r--   0 runner    (1001) docker     (121)      826 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/stream.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3372 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/unpivot.py
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/unstream.py
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/update_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (121)      627 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/update_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)      137 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/update_stats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2242 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/processors/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 12:34:41.759094 dataflows-0.3.8/dataflows/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     3324 2021-10-18 12:34:37.000000 dataflows-0.3.8/dataflows/templates/main.tpl.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 12:34:41.755094 dataflows-0.3.8/dataflows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6415 2021-10-18 12:34:41.000000 dataflows-0.3.8/dataflows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2708 2021-10-18 12:34:41.000000 dataflows-0.3.8/dataflows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-18 12:34:41.000000 dataflows-0.3.8/dataflows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-10-18 12:34:41.000000 dataflows-0.3.8/dataflows.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-18 12:34:41.000000 dataflows-0.3.8/dataflows.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2021-10-18 12:34:41.000000 dataflows-0.3.8/dataflows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-10-18 12:34:41.000000 dataflows-0.3.8/dataflows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       67 2021-10-18 12:34:41.759094 dataflows-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2169 2021-10-18 12:34:37.000000 dataflows-0.3.8/setup.py
```

### Comparing `dataflows-0.3.7/LICENSE` & `dataflows-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/Makefile` & `dataflows-0.3.8/Makefile`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/PKG-INFO` & `dataflows-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataflows
-Version: 0.3.7
+Version: 0.3.8
 Summary: A nifty data processing framework, based on data packages
 Home-page: https://github.com/datahq/dataflows
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Description: # ![logo](logo-s.png) DataFlows
```

### Comparing `dataflows-0.3.7/README.md` & `dataflows-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/base/datastream_processor.py` & `dataflows-0.3.8/dataflows/base/datastream_processor.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/base/exceptions.py` & `dataflows-0.3.8/dataflows/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/base/flow.py` & `dataflows-0.3.8/dataflows/base/flow.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/base/schema_validator.py` & `dataflows-0.3.8/dataflows/base/schema_validator.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/cli.py` & `dataflows-0.3.8/dataflows/cli.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/helpers/datapackage_processor.py` & `dataflows-0.3.8/dataflows/helpers/datapackage_processor.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/helpers/extended_json.py` & `dataflows-0.3.8/dataflows/helpers/extended_json.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/helpers/iterable_loader.py` & `dataflows-0.3.8/dataflows/helpers/iterable_loader.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/helpers/resource_matcher.py` & `dataflows-0.3.8/dataflows/helpers/resource_matcher.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/__init__.py` & `dataflows-0.3.8/dataflows/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/add_computed_field.py` & `dataflows-0.3.8/dataflows/processors/add_computed_field.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/checkpoint.py` & `dataflows-0.3.8/dataflows/processors/checkpoint.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/concatenate.py` & `dataflows-0.3.8/dataflows/processors/concatenate.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/deduplicate.py` & `dataflows-0.3.8/dataflows/processors/deduplicate.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/delete_fields.py` & `dataflows-0.3.8/dataflows/processors/delete_fields.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/dumpers/dumper_base.py` & `dataflows-0.3.8/dataflows/processors/dumpers/dumper_base.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/dumpers/file_dumper.py` & `dataflows-0.3.8/dataflows/processors/dumpers/file_dumper.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/dumpers/formats/base.py` & `dataflows-0.3.8/dataflows/processors/dumpers/formats/base.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/dumpers/formats/format_csv.py` & `dataflows-0.3.8/dataflows/processors/dumpers/formats/format_csv.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/dumpers/formats/format_excel.py` & `dataflows-0.3.8/dataflows/processors/dumpers/formats/format_excel.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/dumpers/formats/format_geojson.py` & `dataflows-0.3.8/dataflows/processors/dumpers/formats/format_geojson.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/dumpers/formats/format_json.py` & `dataflows-0.3.8/dataflows/processors/dumpers/formats/format_json.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/dumpers/to_path.py` & `dataflows-0.3.8/dataflows/processors/dumpers/to_path.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/dumpers/to_sql.py` & `dataflows-0.3.8/dataflows/processors/dumpers/to_sql.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/dumpers/to_zip.py` & `dataflows-0.3.8/dataflows/processors/dumpers/to_zip.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/duplicate.py` & `dataflows-0.3.8/dataflows/processors/duplicate.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/filter_rows.py` & `dataflows-0.3.8/dataflows/processors/filter_rows.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/finalizer.py` & `dataflows-0.3.8/dataflows/processors/finalizer.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/find_replace.py` & `dataflows-0.3.8/dataflows/processors/find_replace.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/join.py` & `dataflows-0.3.8/dataflows/processors/join.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/load.py` & `dataflows-0.3.8/dataflows/processors/load.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/parallelize.py` & `dataflows-0.3.8/dataflows/processors/parallelize.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/parsers/excel_xml_parser.py` & `dataflows-0.3.8/dataflows/processors/parsers/excel_xml_parser.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/parsers/sql_parser.py` & `dataflows-0.3.8/dataflows/processors/parsers/sql_parser.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/parsers/xml_parser.py` & `dataflows-0.3.8/dataflows/processors/parsers/xml_parser.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/printer.py` & `dataflows-0.3.8/dataflows/processors/printer.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/rename_fields.py` & `dataflows-0.3.8/dataflows/processors/rename_fields.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/select_fields.py` & `dataflows-0.3.8/dataflows/processors/select_fields.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/set_primary_key.py` & `dataflows-0.3.8/dataflows/processors/set_primary_key.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/set_type.py` & `dataflows-0.3.8/dataflows/processors/set_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def __init__(self, name, resources=-1, regex=True, on_error=None, transform=None, **options):
         super(set_type, self).__init__()
         if not regex:
             name = re.escape(name)
         self.name = re.compile(f'^{name}$')
         self.options = options
         self.resources = resources
-        self.field_names = []
+        self.field_names = dict()
         self.on_error = on_error
         self.transform = self.wrap_transformer(transform) if transform else None
 
     def wrap_transformer(self, transform):
         assert callable(transform)
         try:
             sig = signature(transform).parameters
@@ -31,29 +31,30 @@
             if 'row' in sig:
                 kw['row'] = row
             if 'field_name' in sig:
                 kw['field_name'] = field_name
             return transform(v, **kw)
         return func
 
-    def transformer(self, rows):
+    def transformer(self, rows, field_names):
         for row in rows:
-            for field_name in self.field_names:
+            for field_name in field_names:
                 row[field_name] = self.transform(row.get(field_name), field_name=field_name, row=row)
             yield row
 
     def process_resources(self, resources):
         for res in resources:
             if self.matcher.match(res.res.name):
-                if len(self.field_names) > 0:
+                field_names = self.field_names.get(res.res.name, [])
+                if len(field_names) > 0:
                     it = res
                     if self.transform is not None:
-                        it = self.transformer(it)
+                        it = self.transformer(it, field_names)
                     yield schema_validator(res.res, it,
-                                           field_names=self.field_names,
+                                           field_names=field_names,
                                            on_error=self.on_error)
                 else:
                     yield res
             else:
                 yield res
 
     def process_datapackage(self, dp):
@@ -61,11 +62,11 @@
         self.matcher = ResourceMatcher(self.resources, dp)
         added = False
         for res in dp.descriptor['resources']:
             if self.matcher.match(res['name']):
                 for field in res['schema']['fields']:
                     if self.name.match(field['name']):
                         field.update(self.options)
-                        self.field_names.append(field['name'])
+                        self.field_names.setdefault(res['name'], []).append(field['name'])
                         added = True
         assert added, 'Failed to find field {} in schema'.format(self.name)
         return dp
```

### Comparing `dataflows-0.3.7/dataflows/processors/sort_rows.py` & `dataflows-0.3.8/dataflows/processors/sort_rows.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/sources.py` & `dataflows-0.3.8/dataflows/processors/sources.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/stream.py` & `dataflows-0.3.8/dataflows/processors/stream.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/unpivot.py` & `dataflows-0.3.8/dataflows/processors/unpivot.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/unstream.py` & `dataflows-0.3.8/dataflows/processors/unstream.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/update_resource.py` & `dataflows-0.3.8/dataflows/processors/update_resource.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/update_schema.py` & `dataflows-0.3.8/dataflows/processors/update_schema.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/processors/validate.py` & `dataflows-0.3.8/dataflows/processors/validate.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows/templates/main.tpl.py` & `dataflows-0.3.8/dataflows/templates/main.tpl.py`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/dataflows.egg-info/PKG-INFO` & `dataflows-0.3.8/dataflows.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataflows
-Version: 0.3.7
+Version: 0.3.8
 Summary: A nifty data processing framework, based on data packages
 Home-page: https://github.com/datahq/dataflows
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Description: # ![logo](logo-s.png) DataFlows
```

### Comparing `dataflows-0.3.7/dataflows.egg-info/SOURCES.txt` & `dataflows-0.3.8/dataflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataflows-0.3.7/setup.py` & `dataflows-0.3.8/setup.py`

 * *Files identical despite different names*

