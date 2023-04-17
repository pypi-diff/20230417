# Comparing `tmp/django-geostore-0.7.2.tar.gz` & `tmp/django-geostore-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-geostore-0.7.2.tar", last modified: Mon Mar  6 16:12:42 2023, max compression
+gzip compressed data, was "django-geostore-0.7.3.tar", last modified: Mon Apr 17 13:13:30 2023, max compression
```

## Comparing `django-geostore-0.7.2.tar` & `django-geostore-0.7.3.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (122)     8031 2023-03-06 16:12:32.000000 django-geostore-0.7.2/CHANGES.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/django_geostore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3835 2023-03-06 16:12:42.000000 django-geostore-0.7.2/django_geostore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      237 2023-03-06 16:12:42.000000 django-geostore-0.7.2/django_geostore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-06 16:12:42.000000 django-geostore-0.7.2/django_geostore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-03-06 16:12:42.000000 django-geostore-0.7.2/django_geostore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    11151 2023-03-06 16:12:42.000000 django-geostore-0.7.2/django_geostore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-03-06 16:12:32.000000 django-geostore-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/db/
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/db/lookups.py
--rw-r--r--   0 runner    (1001) docker     (122)     4169 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/db/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/db/managers.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/db/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/routing/
--rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/routing/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2640 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/tiles/
--rw-r--r--   0 runner    (1001) docker     (122)    10245 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/tiles/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)    10149 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/tiles/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      488 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/tiles/funcs.py
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/tiles/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/tiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      827 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/tiles/sigtools.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3567 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/import_export/
--rw-r--r--   0 runner    (1001) docker     (122)     6748 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/import_export/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     4126 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/import_export/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2771 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/import_export/exports.py
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/VERSION.md
--rw-r--r--   0 runner    (1001) docker     (122)     1750 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/templates/geostore/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/templates/geostore/emails/
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/templates/geostore/emails/exports_no_data.html
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/templates/geostore/emails/exports.html
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/templates/geostore/emails/exports_no_data.txt
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/templates/geostore/emails/exports.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/management/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      568 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/management/commands/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)     8061 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/management/commands/layer_processing.py
--rw-r--r--   0 runner    (1001) docker     (122)     4761 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/management/commands/import_geojson.py
--rw-r--r--   0 runner    (1001) docker     (122)     4477 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/management/commands/import_osm.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5320 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/management/commands/import_csv.py
--rw-r--r--   0 runner    (1001) docker     (122)     2746 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/management/commands/layer_edit.py
--rw-r--r--   0 runner    (1001) docker     (122)     4807 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/management/commands/import_shapefile.py
--rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/management/commands/fill_tiles_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/validators.py
--rw-r--r--   0 runner    (1001) docker     (122)     5808 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/renderers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0045_auto_20210429_0818.py
--rw-r--r--   0 runner    (1001) docker     (122)      410 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0026_auto_20190613_1529.py
--rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0029_auto_20190926_0803.py
--rw-r--r--   0 runner    (1001) docker     (122)      657 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0022_auto_20190417_1610.py
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0038_auto_20200128_1442.py
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0025_auto_20190613_1341.py
--rw-r--r--   0 runner    (1001) docker     (122)      684 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0047_alter_feature_properties.py
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0018_auto_20190228_1655.py
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0020_auto_20190401_1139.py
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0040_merge_20200625_1508.py
--rw-r--r--   0 runner    (1001) docker     (122)      461 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0039_auto_20200131_1758.py
--rw-r--r--   0 runner    (1001) docker     (122)      419 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0042_auto_20201015_1328.py
--rw-r--r--   0 runner    (1001) docker     (122)      617 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0011_auto_20180711_0831.py
--rw-r--r--   0 runner    (1001) docker     (122)      644 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0023_layer_type_geom.py
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0038_auto_20200625_1244.py
--rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0037_auto_20200624_1440.py
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0046_auto_20211013_1334.py
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0030_auto_20191007_1459.py
--rw-r--r--   0 runner    (1001) docker     (122)      488 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0031_layer_authorized_groups.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0024_layer_geom_type.py
--rw-r--r--   0 runner    (1001) docker     (122)      456 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0032_auto_20191016_0844.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0015_auto_20181005_1302.py
--rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0027_layergroup.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0018_auto_20190326_1049.py
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0041_auto_20200625_1515.py
--rw-r--r--   0 runner    (1001) docker     (122)      397 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0035_layerextrageom_editable.py
--rw-r--r--   0 runner    (1001) docker     (122)     2680 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0033_featureextrageom_layerextrageom.py
--rw-r--r--   0 runner    (1001) docker     (122)      320 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0028_remove_layer_group.py
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0014_auto_20180918_1210.py
--rw-r--r--   0 runner    (1001) docker     (122)      808 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0016_auto_20181120_1059.py
--rw-r--r--   0 runner    (1001) docker     (122)      555 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0034_auto_20191209_0902.py
--rw-r--r--   0 runner    (1001) docker     (122)     5119 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0044_auto_20201106_1638.py
--rw-r--r--   0 runner    (1001) docker     (122)      558 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0017_auto_20181114_0806.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0037_auto_20200127_1357.py
--rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0036_auto_20200116_0926.py
--rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0021_auto_20190415_0945.py
--rw-r--r--   0 runner    (1001) docker     (122)      431 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0042_layer_routable.py
--rw-r--r--   0 runner    (1001) docker     (122)     2991 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      276 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0019_merge_20190329_1056.py
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0043_merge_20201023_1209.py
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/migrations/0013_auto_20180919_1146.py
--rw-r--r--   0 runner    (1001) docker     (122)    16685 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      863 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/views/
--rw-r--r--   0 runner    (1001) docker     (122)      863 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/views/mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)    13953 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/locale/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/locale/fr/LC_MESSAGES/django.mo
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)      590 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 16:12:42.000000 django-geostore-0.7.2/geostore/serializers/
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/serializers/geojson.py
--rw-r--r--   0 runner    (1001) docker     (122)     6018 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      862 2023-03-06 16:12:32.000000 django-geostore-0.7.2/geostore/transformations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-03-06 16:12:32.000000 django-geostore-0.7.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)      290 2023-03-06 16:12:32.000000 django-geostore-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-06 16:12:42.000000 django-geostore-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)    11151 2023-03-06 16:12:42.000000 django-geostore-0.7.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.313646 django-geostore-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     8204 2023-04-17 13:13:19.000000 django-geostore-0.7.3/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-04-17 13:13:19.000000 django-geostore-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    11185 2023-04-17 13:13:30.313646 django-geostore-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-04-17 13:13:19.000000 django-geostore-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.285646 django-geostore-0.7.3/django_geostore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11185 2023-04-17 13:13:30.000000 django-geostore-0.7.3/django_geostore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3835 2023-04-17 13:13:30.000000 django-geostore-0.7.3/django_geostore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 13:13:30.000000 django-geostore-0.7.3/django_geostore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-04-17 13:13:30.000000 django-geostore-0.7.3/django_geostore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-17 13:13:30.000000 django-geostore-0.7.3/django_geostore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.289646 django-geostore-0.7.3/geostore/
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/VERSION.md
+-rw-r--r--   0 runner    (1001) docker     (122)      863 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      590 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.289646 django-geostore-0.7.3/geostore/db/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/db/functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/db/lookups.py
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/db/managers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4169 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/db/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2640 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.289646 django-geostore-0.7.3/geostore/import_export/
+-rw-r--r--   0 runner    (1001) docker     (122)     2771 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/import_export/exports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4126 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/import_export/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6748 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/import_export/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.281646 django-geostore-0.7.3/geostore/locale/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.281646 django-geostore-0.7.3/geostore/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.289646 django-geostore-0.7.3/geostore/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/locale/en/LC_MESSAGES/django.mo
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.281646 django-geostore-0.7.3/geostore/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.289646 django-geostore-0.7.3/geostore/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4787 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/locale/fr/LC_MESSAGES/django.mo
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.289646 django-geostore-0.7.3/geostore/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.297646 django-geostore-0.7.3/geostore/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/management/commands/fill_tiles_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5320 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/management/commands/import_csv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4761 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/management/commands/import_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4477 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/management/commands/import_osm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4807 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/management/commands/import_shapefile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2746 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/management/commands/layer_edit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8061 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/management/commands/layer_processing.py
+-rw-r--r--   0 runner    (1001) docker     (122)      568 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/management/commands/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.309646 django-geostore-0.7.3/geostore/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2991 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0011_auto_20180711_0831.py
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0013_auto_20180919_1146.py
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0014_auto_20180918_1210.py
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0015_auto_20181005_1302.py
+-rw-r--r--   0 runner    (1001) docker     (122)      808 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0016_auto_20181120_1059.py
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0017_auto_20181114_0806.py
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0018_auto_20190228_1655.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0018_auto_20190326_1049.py
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0019_merge_20190329_1056.py
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0020_auto_20190401_1139.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0021_auto_20190415_0945.py
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0022_auto_20190417_1610.py
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0023_layer_type_geom.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0024_layer_geom_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0025_auto_20190613_1341.py
+-rw-r--r--   0 runner    (1001) docker     (122)      410 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0026_auto_20190613_1529.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0027_layergroup.py
+-rw-r--r--   0 runner    (1001) docker     (122)      320 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0028_remove_layer_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0029_auto_20190926_0803.py
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0030_auto_20191007_1459.py
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0031_layer_authorized_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)      456 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0032_auto_20191016_0844.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2680 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0033_featureextrageom_layerextrageom.py
+-rw-r--r--   0 runner    (1001) docker     (122)      555 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0034_auto_20191209_0902.py
+-rw-r--r--   0 runner    (1001) docker     (122)      397 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0035_layerextrageom_editable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0036_auto_20200116_0926.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0037_auto_20200127_1357.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0037_auto_20200624_1440.py
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0038_auto_20200128_1442.py
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0038_auto_20200625_1244.py
+-rw-r--r--   0 runner    (1001) docker     (122)      461 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0039_auto_20200131_1758.py
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0040_merge_20200625_1508.py
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0041_auto_20200625_1515.py
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0042_auto_20201015_1328.py
+-rw-r--r--   0 runner    (1001) docker     (122)      431 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0042_layer_routable.py
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0043_merge_20201023_1209.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5119 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0044_auto_20201106_1638.py
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0045_auto_20210429_0818.py
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0046_auto_20211013_1334.py
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/0047_alter_feature_properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16685 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5808 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/renderers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.309646 django-geostore-0.7.3/geostore/routing/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/routing/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.309646 django-geostore-0.7.3/geostore/serializers/
+-rw-r--r--   0 runner    (1001) docker     (122)     6018 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/serializers/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1750 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.281646 django-geostore-0.7.3/geostore/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.281646 django-geostore-0.7.3/geostore/templates/geostore/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.309646 django-geostore-0.7.3/geostore/templates/geostore/emails/
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/templates/geostore/emails/exports.html
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/templates/geostore/emails/exports.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/templates/geostore/emails/exports_no_data.html
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/templates/geostore/emails/exports_no_data.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.309646 django-geostore-0.7.3/geostore/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3567 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/tests/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.313646 django-geostore-0.7.3/geostore/tiles/
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/tiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/tiles/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/tiles/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10149 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/tiles/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10351 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/tiles/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/tiles/sigtools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (122)      862 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 13:13:30.313646 django-geostore-0.7.3/geostore/views/
+-rw-r--r--   0 runner    (1001) docker     (122)    13953 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      863 2023-04-17 13:13:19.000000 django-geostore-0.7.3/geostore/views/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-17 13:13:30.313646 django-geostore-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-04-17 13:13:19.000000 django-geostore-0.7.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-geostore-0.7.2/CHANGES.md` & `django-geostore-0.7.3/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGELOG
 =========
 
+0.7.3          (2023-04-17)
+---------------------------
+
+* Support django 4.2
+* Allow layer access with group limit to superusers
+* Drop django 2.2 and python 3.6 support
+
+
 0.7.2          (2023-03-06)
 ---------------------------
 
 * Allow dates and objects in feature properties by using DjangoJSONEncoder
 
 
 0.7.1          (2023-03-03)
```

### Comparing `django-geostore-0.7.2/django_geostore.egg-info/SOURCES.txt` & `django-geostore-0.7.3/django_geostore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/django_geostore.egg-info/PKG-INFO` & `django-geostore-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: django-geostore
-Version: 0.7.2
+Version: 0.7.3
 Summary: Django geographic store and vector tile generation
 Home-page: https://github.com/Terralego/django-geostore.git
 Author: Makina Corpus
 Author-email: terralego-pypi@makina-corpus.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 [![Build Status](https://travis-ci.org/Terralego/django-geostore.svg?branch=master)](https://travis-ci.org/Terralego/django-geostore/)
 [![codecov](https://codecov.io/gh/Terralego/django-geostore/branch/master/graph/badge.svg)](https://codecov.io/gh/Terralego/django-geostore)
 [![Maintainability](https://api.codeclimate.com/v1/badges/b6119d8175fa6f5f5949/maintainability)](https://codeclimate.com/github/Terralego/django-geostore/maintainability)
 [![Documentation Status](https://readthedocs.org/projects/django-geostore/badge/?version=latest)](https://django-geostore.readthedocs.io/en/latest/?badge=latest)
@@ -109,14 +105,22 @@
 pip install -e .[dev]
 ```
 
 
 CHANGELOG
 =========
 
+0.7.3          (2023-04-17)
+---------------------------
+
+* Support django 4.2
+* Allow layer access with group limit to superusers
+* Drop django 2.2 and python 3.6 support
+
+
 0.7.2          (2023-03-06)
 ---------------------------
 
 * Allow dates and objects in feature properties by using DjangoJSONEncoder
 
 
 0.7.1          (2023-03-03)
@@ -467,9 +471,7 @@
 
 0.3.0      (2019-09-09)
 -----------------------
 
 First public tag
 
 * Terra app extracted from terracommon.terra
-
-
```

### Comparing `django-geostore-0.7.2/README.md` & `django-geostore-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/db/mixins.py` & `django-geostore-0.7.3/geostore/db/mixins.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/routing/mixins.py` & `django-geostore-0.7.3/geostore/routing/mixins.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/filters.py` & `django-geostore-0.7.3/geostore/filters.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/tokens.py` & `django-geostore-0.7.3/geostore/tokens.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/tiles/mixins.py` & `django-geostore-0.7.3/geostore/tiles/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
             groups, layergroup = tiles_token_generator.decode_idb64(idb64)
 
             if groups and layergroup and tiles_token_generator.check_token(token, groups, layergroup):
                 return groups
         return []
 
     def is_authorized(self, layer):
+        if self.request.user.is_authenticated and self.request.user.is_superuser:
+            return True
         if layer.authorized_groups.exists():
             return layer.authorized_groups.filter(pk__in=self.authenticated_groups).exists()
         return True
 
 
 class MVTViewMixin(AuthenticatedGroupsMixin):
     tile_response_class = HttpResponse
```

### Comparing `django-geostore-0.7.2/geostore/tiles/helpers.py` & `django-geostore-0.7.3/geostore/tiles/helpers.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/tiles/decorators.py` & `django-geostore-0.7.3/geostore/tiles/decorators.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/tiles/sigtools.py` & `django-geostore-0.7.3/geostore/tiles/sigtools.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/signals.py` & `django-geostore-0.7.3/geostore/signals.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/tests/factories.py` & `django-geostore-0.7.3/geostore/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/urls.py` & `django-geostore-0.7.3/geostore/urls.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/import_export/imports.py` & `django-geostore-0.7.3/geostore/import_export/imports.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/import_export/helpers.py` & `django-geostore-0.7.3/geostore/import_export/helpers.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/import_export/exports.py` & `django-geostore-0.7.3/geostore/import_export/exports.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/settings.py` & `django-geostore-0.7.3/geostore/settings.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/tasks.py` & `django-geostore-0.7.3/geostore/tasks.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/management/commands/mixins.py` & `django-geostore-0.7.3/geostore/management/commands/mixins.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/management/commands/layer_processing.py` & `django-geostore-0.7.3/geostore/management/commands/layer_processing.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/management/commands/import_geojson.py` & `django-geostore-0.7.3/geostore/management/commands/import_geojson.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/management/commands/import_osm.py` & `django-geostore-0.7.3/geostore/management/commands/import_osm.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/management/commands/import_csv.py` & `django-geostore-0.7.3/geostore/management/commands/import_csv.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/management/commands/layer_edit.py` & `django-geostore-0.7.3/geostore/management/commands/layer_edit.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/management/commands/import_shapefile.py` & `django-geostore-0.7.3/geostore/management/commands/import_shapefile.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/management/commands/fill_tiles_cache.py` & `django-geostore-0.7.3/geostore/management/commands/fill_tiles_cache.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/validators.py` & `django-geostore-0.7.3/geostore/validators.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/renderers.py` & `django-geostore-0.7.3/geostore/renderers.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/permissions.py` & `django-geostore-0.7.3/geostore/permissions.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0045_auto_20210429_0818.py` & `django-geostore-0.7.3/geostore/migrations/0045_auto_20210429_0818.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0029_auto_20190926_0803.py` & `django-geostore-0.7.3/geostore/migrations/0029_auto_20190926_0803.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0022_auto_20190417_1610.py` & `django-geostore-0.7.3/geostore/migrations/0022_auto_20190417_1610.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0038_auto_20200128_1442.py` & `django-geostore-0.7.3/geostore/migrations/0038_auto_20200128_1442.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0025_auto_20190613_1341.py` & `django-geostore-0.7.3/geostore/migrations/0025_auto_20190613_1341.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0047_alter_feature_properties.py` & `django-geostore-0.7.3/geostore/migrations/0047_alter_feature_properties.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0018_auto_20190228_1655.py` & `django-geostore-0.7.3/geostore/migrations/0018_auto_20190228_1655.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0020_auto_20190401_1139.py` & `django-geostore-0.7.3/geostore/migrations/0020_auto_20190401_1139.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0011_auto_20180711_0831.py` & `django-geostore-0.7.3/geostore/migrations/0011_auto_20180711_0831.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0023_layer_type_geom.py` & `django-geostore-0.7.3/geostore/migrations/0023_layer_type_geom.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0038_auto_20200625_1244.py` & `django-geostore-0.7.3/geostore/migrations/0038_auto_20200625_1244.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0037_auto_20200624_1440.py` & `django-geostore-0.7.3/geostore/migrations/0037_auto_20200624_1440.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0046_auto_20211013_1334.py` & `django-geostore-0.7.3/geostore/migrations/0046_auto_20211013_1334.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0030_auto_20191007_1459.py` & `django-geostore-0.7.3/geostore/migrations/0030_auto_20191007_1459.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0024_layer_geom_type.py` & `django-geostore-0.7.3/geostore/migrations/0024_layer_geom_type.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0027_layergroup.py` & `django-geostore-0.7.3/geostore/migrations/0027_layergroup.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0018_auto_20190326_1049.py` & `django-geostore-0.7.3/geostore/migrations/0018_auto_20190326_1049.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0041_auto_20200625_1515.py` & `django-geostore-0.7.3/geostore/migrations/0041_auto_20200625_1515.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0033_featureextrageom_layerextrageom.py` & `django-geostore-0.7.3/geostore/migrations/0033_featureextrageom_layerextrageom.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0016_auto_20181120_1059.py` & `django-geostore-0.7.3/geostore/migrations/0016_auto_20181120_1059.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0034_auto_20191209_0902.py` & `django-geostore-0.7.3/geostore/migrations/0034_auto_20191209_0902.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0044_auto_20201106_1638.py` & `django-geostore-0.7.3/geostore/migrations/0044_auto_20201106_1638.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0017_auto_20181114_0806.py` & `django-geostore-0.7.3/geostore/migrations/0017_auto_20181114_0806.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0037_auto_20200127_1357.py` & `django-geostore-0.7.3/geostore/migrations/0037_auto_20200127_1357.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0036_auto_20200116_0926.py` & `django-geostore-0.7.3/geostore/migrations/0036_auto_20200116_0926.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0021_auto_20190415_0945.py` & `django-geostore-0.7.3/geostore/migrations/0021_auto_20190415_0945.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0001_initial.py` & `django-geostore-0.7.3/geostore/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/migrations/0013_auto_20180919_1146.py` & `django-geostore-0.7.3/geostore/migrations/0013_auto_20180919_1146.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/models.py` & `django-geostore-0.7.3/geostore/models.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/__init__.py` & `django-geostore-0.7.3/geostore/__init__.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/views/mixins.py` & `django-geostore-0.7.3/geostore/views/mixins.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/views/__init__.py` & `django-geostore-0.7.3/geostore/views/__init__.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/locale/fr/LC_MESSAGES/django.mo` & `django-geostore-0.7.3/geostore/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/apps.py` & `django-geostore-0.7.3/geostore/apps.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/serializers/geojson.py` & `django-geostore-0.7.3/geostore/serializers/geojson.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/serializers/__init__.py` & `django-geostore-0.7.3/geostore/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/geostore/transformations.py` & `django-geostore-0.7.3/geostore/transformations.py`

 * *Files identical despite different names*

### Comparing `django-geostore-0.7.2/setup.py` & `django-geostore-0.7.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,17 +32,15 @@
         'Intended Audience :: Developers',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3',
     ],
     install_requires=[
         'django>=2.2',
         'django-token-tools',
         'djangorestframework>=3.10',
         "djangorestframework-gis>=0.15",
         "gpxpy",
```

### Comparing `django-geostore-0.7.2/PKG-INFO` & `django-geostore-0.7.3/django_geostore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: django-geostore
-Version: 0.7.2
+Version: 0.7.3
 Summary: Django geographic store and vector tile generation
 Home-page: https://github.com/Terralego/django-geostore.git
 Author: Makina Corpus
 Author-email: terralego-pypi@makina-corpus.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 [![Build Status](https://travis-ci.org/Terralego/django-geostore.svg?branch=master)](https://travis-ci.org/Terralego/django-geostore/)
 [![codecov](https://codecov.io/gh/Terralego/django-geostore/branch/master/graph/badge.svg)](https://codecov.io/gh/Terralego/django-geostore)
 [![Maintainability](https://api.codeclimate.com/v1/badges/b6119d8175fa6f5f5949/maintainability)](https://codeclimate.com/github/Terralego/django-geostore/maintainability)
 [![Documentation Status](https://readthedocs.org/projects/django-geostore/badge/?version=latest)](https://django-geostore.readthedocs.io/en/latest/?badge=latest)
@@ -109,14 +105,22 @@
 pip install -e .[dev]
 ```
 
 
 CHANGELOG
 =========
 
+0.7.3          (2023-04-17)
+---------------------------
+
+* Support django 4.2
+* Allow layer access with group limit to superusers
+* Drop django 2.2 and python 3.6 support
+
+
 0.7.2          (2023-03-06)
 ---------------------------
 
 * Allow dates and objects in feature properties by using DjangoJSONEncoder
 
 
 0.7.1          (2023-03-03)
@@ -467,9 +471,7 @@
 
 0.3.0      (2019-09-09)
 -----------------------
 
 First public tag
 
 * Terra app extracted from terracommon.terra
-
-
```

