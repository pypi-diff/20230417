# Comparing `tmp/cubicweb-seda-0.8.0.tar.gz` & `tmp/cubicweb-seda-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubicweb-seda-0.8.0.tar", last modified: Wed Mar  8 06:22:31 2017, max compression
+gzip compressed data, was "dist/cubicweb-seda-0.9.0.tar", last modified: Tue Mar 21 14:09:02 2017, max compression
```

## Comparing `cubicweb-seda-0.8.0.tar` & `cubicweb-seda-0.9.0.tar`

### file list

```diff
@@ -1,132 +1,133 @@
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-08 06:22:31.000000 cubicweb-seda-0.8.0/
--rw-r--r--   0 narval     (111) narval     (116)       93 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/dev-requirements.txt
--rw-r--r--   0 narval     (111) narval     (116)      508 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/MANIFEST.in
--rw-rw-r--   0 narval     (111) narval     (116)       59 2017-03-08 06:22:31.000000 cubicweb-seda-0.8.0/setup.cfg
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-08 06:22:31.000000 cubicweb-seda-0.8.0/cubicweb_seda/
--rw-r--r--   0 narval     (111) narval     (116)    24969 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/xsd2yams.py
--rw-r--r--   0 narval     (111) narval     (116)     9399 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/xsd2uicfg.py
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-08 06:22:31.000000 cubicweb-seda-0.8.0/cubicweb_seda/entities/
--rw-r--r--   0 narval     (111) narval     (116)     5191 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/entities/itree.py
--rw-r--r--   0 narval     (111) narval     (116)    76869 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/entities/profile_generation.py
--rw-r--r--   0 narval     (111) narval     (116)    10149 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/entities/custom.py
--rw-r--r--   0 narval     (111) narval     (116)     8636 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/entities/__init__.py
--rw-r--r--   0 narval     (111) narval     (116)    11129 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/entities/html_generation.py
--rw-r--r--   0 narval     (111) narval     (116)     9931 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/entities/diag.py
--rw-r--r--   0 narval     (111) narval     (116)    30822 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/entities/generated.py
--rw-r--r--   0 narval     (111) narval     (116)    23937 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/xsd.py
--rw-r--r--   0 narval     (111) narval     (116)     7338 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/dataimport.py
--rw-r--r--   0 narval     (111) narval     (116)    15206 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/hooks.py
--rw-r--r--   0 narval     (111) narval     (116)     3494 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/xsd2concepts.py
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-08 06:22:31.000000 cubicweb-seda-0.8.0/cubicweb_seda/schema/
--rw-r--r--   0 narval     (111) narval     (116)     7195 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/schema/__init__.py
--rw-r--r--   0 narval     (111) narval     (116)    99820 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/schema/seda2.py
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-08 06:22:31.000000 cubicweb-seda-0.8.0/cubicweb_seda/views/
--rw-r--r--   0 narval     (111) narval     (116)     6851 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/views/jqtree.py
--rw-r--r--   0 narval     (111) narval     (116)     5465 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/views/patches.py
--rw-r--r--   0 narval     (111) narval     (116)     5334 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/views/export.py
--rw-r--r--   0 narval     (111) narval     (116)    10144 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/views/simplified.py
--rw-r--r--   0 narval     (111) narval     (116)    45668 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/views/archiveunit.py
--rw-r--r--   0 narval     (111) narval     (116)    10594 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/views/archivetransfer.py
--rw-r--r--   0 narval     (111) narval     (116)   102878 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/views/uicfg.py
--rw-r--r--   0 narval     (111) narval     (116)     4918 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/views/clone.py
--rw-r--r--   0 narval     (111) narval     (116)    14506 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/views/viewlib.py
--rw-r--r--   0 narval     (111) narval     (116)     2805 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/views/sedalib.py
--rw-r--r--   0 narval     (111) narval     (116)    13285 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/views/dataobject.py
--rw-r--r--   0 narval     (111) narval     (116)     7509 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/views/__init__.py
--rw-r--r--   0 narval     (111) narval     (116)     8791 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/views/mgmt_rules.py
--rw-r--r--   0 narval     (111) narval     (116)    12308 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/views/widgets.py
--rw-r--r--   0 narval     (111) narval     (116)     4280 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/views/sedatree.py
--rw-r--r--   0 narval     (111) narval     (116)     1225 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/views/facets.py
--rw-r--r--   0 narval     (111) narval     (116)     5504 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/site_cubicweb.py
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-08 06:22:31.000000 cubicweb-seda-0.8.0/cubicweb_seda/xsd/
--rw-r--r--   0 narval     (111) narval     (116)    50275 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/xsd/seda-2.0-ontology.xsd
--rw-r--r--   0 narval     (111) narval     (116)     8299 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/xsd/xlink.xsd
--rw-r--r--   0 narval     (111) narval     (116)    42934 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/xsd/seda-2.0-main.xsd
--rw-r--r--   0 narval     (111) narval     (116)     8836 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/xsd/xml.xsd
--rw-r--r--   0 narval     (111) narval     (116)     4706 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/xsd/seda-2.0-descriptive.xsd
--rw-r--r--   0 narval     (111) narval     (116)    24418 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/xsd/seda-2.0-management.xsd
--rw-r--r--   0 narval     (111) narval     (116)    25322 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/xsd/seda-2.0-technical.xsd
--rw-r--r--   0 narval     (111) narval     (116)    16210 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/xsd/seda-2.0-types.xsd
--rw-r--r--   0 narval     (111) narval     (116)      863 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/__pkginfo__.py
--rw-r--r--   0 narval     (111) narval     (116)     2261 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/__init__.py
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-08 06:22:31.000000 cubicweb-seda-0.8.0/cubicweb_seda/i18n/
--rw-r--r--   0 narval     (111) narval     (116)   175151 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/i18n/fr.po
--rw-r--r--   0 narval     (111) narval     (116)   163227 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/i18n/en.po
--rw-r--r--   0 narval     (111) narval     (116)       34 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/i18n/static-messages.pot
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-08 06:22:31.000000 cubicweb-seda-0.8.0/cubicweb_seda/data/
--rw-r--r--   0 narval     (111) narval     (116)   100626 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/data/tree.jquery.js
--rw-r--r--   0 narval     (111) narval     (116)      577 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/data/cubes.seda.css
--rw-r--r--   0 narval     (111) narval     (116)     4137 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/data/jqtree.css
--rw-r--r--   0 narval     (111) narval     (116)      243 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/data/cubes.jqtree.css
--rw-r--r--   0 narval     (111) narval     (116)     1273 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/data/cubes.seda.js
--rw-r--r--   0 narval     (111) narval     (116)     1526 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/data/cubes.editionext.js
--rw-r--r--   0 narval     (111) narval     (116)     1520 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/data/cubes.seda.form.js
--rw-r--r--   0 narval     (111) narval     (116)     3623 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/data/cubes.jqtree.js
--rw-r--r--   0 narval     (111) narval     (116)     4226 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/data/cubes.skoscomplete.js
--rw-r--r--   0 narval     (111) narval     (116)      292 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/makefile
--rw-r--r--   0 narval     (111) narval     (116)       43 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/uiprops.py
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-08 06:22:31.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/
--rw-r--r--   0 narval     (111) narval     (116)     1125 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/0.8.0_Any.py
--rw-r--r--   0 narval     (111) narval     (116)     1043 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/postcreate.py
--rw-r--r--   0 narval     (111) narval     (116)      131 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/0.5.1_Any.py
--rw-r--r--   0 narval     (111) narval     (116)     2392 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/0.6.0_Any.py
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-08 06:22:31.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/
--rw-r--r--   0 narval     (111) narval     (116)   131456 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/languages.csv
--rw-r--r--   0 narval     (111) narval     (116)     2469 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/level_type.csv
--rw-r--r--   0 narval     (111) narval     (116)      202 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/measurement_units_type.csv
--rw-r--r--   0 narval     (111) narval     (116)      115 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/final_action_storage_code_type.csv
--rw-r--r--   0 narval     (111) narval     (116)    64714 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/mime_types.csv
--rw-r--r--   0 narval     (111) narval     (116)      177 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/legal_status.csv
--rw-r--r--   0 narval     (111) narval     (116)     1498 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/dissemination.csv
--rw-r--r--   0 narval     (111) narval     (116)      187 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/final_action_appraisal_code_type.csv
--rw-r--r--   0 narval     (111) narval     (116)      583 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/encodings.csv
--rw-r--r--   0 narval     (111) narval     (116)      150 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/classification_levels.csv
--rw-r--r--   0 narval     (111) narval     (116)     3877 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/document_type_code.csv
--rw-r--r--   0 narval     (111) narval     (116)      182 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/code_keyword_type.csv
--rw-r--r--   0 narval     (111) narval     (116)      628 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/digest_algorithms.csv
--rw-r--r--   0 narval     (111) narval     (116)      176 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/measurement_weight_units_type.csv
--rw-r--r--   0 narval     (111) narval     (116)      149 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/event_types.csv
--rw-r--r--   0 narval     (111) narval     (116)      271 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/dua.csv
--rw-r--r--   0 narval     (111) narval     (116)    29311 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/file_formats.csv
--rw-r--r--   0 narval     (111) narval     (116)     7022 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/migration/data/access_control.csv
--rw-r--r--   0 narval     (111) narval     (116)     3214 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/cubicweb_seda/xsd2entities.py
--rw-r--r--   0 narval     (111) narval     (116)     1250 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/tox.ini
--rw-r--r--   0 narval     (111) narval     (116)       52 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/README
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-08 06:22:31.000000 cubicweb-seda-0.8.0/cubicweb_seda.egg-info/
--rw-rw-r--   0 narval     (111) narval     (116)        1 2017-03-08 06:05:08.000000 cubicweb-seda-0.8.0/cubicweb_seda.egg-info/not-zip-safe
--rw-rw-r--   0 narval     (111) narval     (116)       14 2017-03-08 06:22:29.000000 cubicweb-seda-0.8.0/cubicweb_seda.egg-info/top_level.txt
--rw-rw-r--   0 narval     (111) narval     (116)       39 2017-03-08 06:22:29.000000 cubicweb-seda-0.8.0/cubicweb_seda.egg-info/entry_points.txt
--rw-rw-r--   0 narval     (111) narval     (116)     3833 2017-03-08 06:22:29.000000 cubicweb-seda-0.8.0/cubicweb_seda.egg-info/SOURCES.txt
--rw-rw-r--   0 narval     (111) narval     (116)        1 2017-03-08 06:22:29.000000 cubicweb-seda-0.8.0/cubicweb_seda.egg-info/dependency_links.txt
--rw-rw-r--   0 narval     (111) narval     (116)      518 2017-03-08 06:22:29.000000 cubicweb-seda-0.8.0/cubicweb_seda.egg-info/PKG-INFO
--rw-rw-r--   0 narval     (111) narval     (116)      161 2017-03-08 06:22:29.000000 cubicweb-seda-0.8.0/cubicweb_seda.egg-info/requires.txt
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-08 06:22:31.000000 cubicweb-seda-0.8.0/doc/
--rw-r--r--   0 narval     (111) narval     (116)     2100 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/doc/profils.rst
--rw-r--r--   0 narval     (111) narval     (116)      198 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/doc/index.rst
--rw-r--r--   0 narval     (111) narval     (116)     8116 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/doc/conf.py
--rw-rw-r--   0 narval     (111) narval     (116)      518 2017-03-08 06:22:31.000000 cubicweb-seda-0.8.0/PKG-INFO
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-08 06:22:31.000000 cubicweb-seda-0.8.0/test/
--rw-r--r--   0 narval     (111) narval     (116)     6176 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/test_html_generation.py
--rw-r--r--   0 narval     (111) narval     (116)     2391 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/pytestconf.py
--rw-r--r--   0 narval     (111) narval     (116)     6927 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/test_diag.py
--rw-r--r--   0 narval     (111) narval     (116)    13259 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/test_entities.py
--rw-r--r--   0 narval     (111) narval     (116)    16361 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/test_schema.py
--rw-r--r--   0 narval     (111) narval     (116)     1272 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/test_dataimport.py
--rw-r--r--   0 narval     (111) narval     (116)     4252 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/testutils.py
--rw-r--r--   0 narval     (111) narval     (116)    14487 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/test_xsd2yams.py
--rw-r--r--   0 narval     (111) narval     (116)    10416 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/test_hooks.py
--rw-r--r--   0 narval     (111) narval     (116)    31980 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/test_views.py
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-08 06:22:31.000000 cubicweb-seda-0.8.0/test/data/
--rw-r--r--   0 narval     (111) narval     (116)    11890 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/data/BV2.0_min.xml
--rw-r--r--   0 narval     (111) narval     (116)    13473 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/data/exArchiveTransfer1_SEDA2_min.xml
--rw-r--r--   0 narval     (111) narval     (116)    22493 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/data/seda_1_export.rng
--rw-r--r--   0 narval     (111) narval     (116)     8126 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/data/relaxng.rng
--rw-r--r--   0 narval     (111) narval     (116)     8450 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/data/exArchiveTransfert2_SEDA2_min.xml
--rw-r--r--   0 narval     (111) narval     (116)        5 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/data/bootstrap_cubes
--rw-r--r--   0 narval     (111) narval     (116)    20767 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/data/seda_02_export.rng
--rw-r--r--   0 narval     (111) narval     (116)    26454 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/data/seda_1_export.xsd
--rw-r--r--   0 narval     (111) narval     (116)    23996 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/data/seda_02_export.xsd
--rw-r--r--   0 narval     (111) narval     (116)    71264 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/data/XMLSchema.xsd
--rw-r--r--   0 narval     (111) narval     (116)     2468 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/data/seda_02_bordereau_ref.xml
--rw-r--r--   0 narval     (111) narval     (116)    47235 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/test/test_profile_generation.py
--rw-r--r--   0 narval     (111) narval     (116)     2587 2017-03-08 06:05:01.000000 cubicweb-seda-0.8.0/setup.py
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-21 14:09:02.000000 cubicweb-seda-0.9.0/
+-rw-r--r--   0 narval     (111) narval     (116)        7 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/dev-requirements.txt
+-rw-r--r--   0 narval     (111) narval     (116)      508 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/MANIFEST.in
+-rw-rw-r--   0 narval     (111) narval     (116)       59 2017-03-21 14:09:02.000000 cubicweb-seda-0.9.0/setup.cfg
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-21 14:09:02.000000 cubicweb-seda-0.9.0/cubicweb_seda/
+-rw-r--r--   0 narval     (111) narval     (116)    24969 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/xsd2yams.py
+-rw-r--r--   0 narval     (111) narval     (116)     9399 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/xsd2uicfg.py
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-21 14:09:02.000000 cubicweb-seda-0.9.0/cubicweb_seda/entities/
+-rw-r--r--   0 narval     (111) narval     (116)     5191 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/entities/itree.py
+-rw-r--r--   0 narval     (111) narval     (116)    79165 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/entities/profile_generation.py
+-rw-r--r--   0 narval     (111) narval     (116)    11555 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/entities/custom.py
+-rw-r--r--   0 narval     (111) narval     (116)     8816 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/entities/__init__.py
+-rw-r--r--   0 narval     (111) narval     (116)    11129 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/entities/html_generation.py
+-rw-r--r--   0 narval     (111) narval     (116)     9931 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/entities/diag.py
+-rw-r--r--   0 narval     (111) narval     (116)    30822 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/entities/generated.py
+-rw-r--r--   0 narval     (111) narval     (116)    23937 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/xsd.py
+-rw-r--r--   0 narval     (111) narval     (116)     7336 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/dataimport.py
+-rw-r--r--   0 narval     (111) narval     (116)    15206 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/hooks.py
+-rw-r--r--   0 narval     (111) narval     (116)     3494 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/xsd2concepts.py
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-21 14:09:02.000000 cubicweb-seda-0.9.0/cubicweb_seda/schema/
+-rw-r--r--   0 narval     (111) narval     (116)     8374 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/schema/__init__.py
+-rw-r--r--   0 narval     (111) narval     (116)    99820 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/schema/seda2.py
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-21 14:09:02.000000 cubicweb-seda-0.9.0/cubicweb_seda/views/
+-rw-r--r--   0 narval     (111) narval     (116)     6851 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/views/jqtree.py
+-rw-r--r--   0 narval     (111) narval     (116)     5465 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/views/patches.py
+-rw-r--r--   0 narval     (111) narval     (116)     5334 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/views/export.py
+-rw-r--r--   0 narval     (111) narval     (116)     8034 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/views/simplified.py
+-rw-r--r--   0 narval     (111) narval     (116)    47240 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/views/archiveunit.py
+-rw-r--r--   0 narval     (111) narval     (116)    10594 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/views/archivetransfer.py
+-rw-r--r--   0 narval     (111) narval     (116)   102878 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/views/uicfg.py
+-rw-r--r--   0 narval     (111) narval     (116)     4918 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/views/clone.py
+-rw-r--r--   0 narval     (111) narval     (116)    14506 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/views/viewlib.py
+-rw-r--r--   0 narval     (111) narval     (116)     2805 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/views/sedalib.py
+-rw-r--r--   0 narval     (111) narval     (116)    13285 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/views/dataobject.py
+-rw-r--r--   0 narval     (111) narval     (116)     7726 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/views/__init__.py
+-rw-r--r--   0 narval     (111) narval     (116)     9516 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/views/mgmt_rules.py
+-rw-r--r--   0 narval     (111) narval     (116)    13579 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/views/widgets.py
+-rw-r--r--   0 narval     (111) narval     (116)     4300 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/views/sedatree.py
+-rw-r--r--   0 narval     (111) narval     (116)     1225 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/views/facets.py
+-rw-r--r--   0 narval     (111) narval     (116)     5671 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/site_cubicweb.py
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-21 14:09:02.000000 cubicweb-seda-0.9.0/cubicweb_seda/xsd/
+-rw-r--r--   0 narval     (111) narval     (116)    50275 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/xsd/seda-2.0-ontology.xsd
+-rw-r--r--   0 narval     (111) narval     (116)     8299 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/xsd/xlink.xsd
+-rw-r--r--   0 narval     (111) narval     (116)    42934 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/xsd/seda-2.0-main.xsd
+-rw-r--r--   0 narval     (111) narval     (116)     8836 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/xsd/xml.xsd
+-rw-r--r--   0 narval     (111) narval     (116)     4706 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/xsd/seda-2.0-descriptive.xsd
+-rw-r--r--   0 narval     (111) narval     (116)    24418 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/xsd/seda-2.0-management.xsd
+-rw-r--r--   0 narval     (111) narval     (116)    25322 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/xsd/seda-2.0-technical.xsd
+-rw-r--r--   0 narval     (111) narval     (116)    16210 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/xsd/seda-2.0-types.xsd
+-rw-r--r--   0 narval     (111) narval     (116)      863 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/__pkginfo__.py
+-rw-r--r--   0 narval     (111) narval     (116)     2261 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/__init__.py
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-21 14:09:02.000000 cubicweb-seda-0.9.0/cubicweb_seda/i18n/
+-rw-r--r--   0 narval     (111) narval     (116)   175843 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/i18n/fr.po
+-rw-r--r--   0 narval     (111) narval     (116)   163680 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/i18n/en.po
+-rw-r--r--   0 narval     (111) narval     (116)       34 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/i18n/static-messages.pot
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-21 14:09:02.000000 cubicweb-seda-0.9.0/cubicweb_seda/data/
+-rw-r--r--   0 narval     (111) narval     (116)   100626 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/data/tree.jquery.js
+-rw-r--r--   0 narval     (111) narval     (116)      577 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/data/cubes.seda.css
+-rw-r--r--   0 narval     (111) narval     (116)     4137 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/data/jqtree.css
+-rw-r--r--   0 narval     (111) narval     (116)      243 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/data/cubes.jqtree.css
+-rw-r--r--   0 narval     (111) narval     (116)     1273 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/data/cubes.seda.js
+-rw-r--r--   0 narval     (111) narval     (116)     1526 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/data/cubes.editionext.js
+-rw-r--r--   0 narval     (111) narval     (116)     1520 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/data/cubes.seda.form.js
+-rw-r--r--   0 narval     (111) narval     (116)     3623 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/data/cubes.jqtree.js
+-rw-r--r--   0 narval     (111) narval     (116)     6662 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/data/cubes.skoscomplete.js
+-rw-r--r--   0 narval     (111) narval     (116)      292 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/makefile
+-rw-r--r--   0 narval     (111) narval     (116)       43 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/uiprops.py
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-21 14:09:02.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/
+-rw-r--r--   0 narval     (111) narval     (116)     1311 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/0.9.0_Any.py
+-rw-r--r--   0 narval     (111) narval     (116)     1125 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/0.8.0_Any.py
+-rw-r--r--   0 narval     (111) narval     (116)     1043 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/postcreate.py
+-rw-r--r--   0 narval     (111) narval     (116)      131 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/0.5.1_Any.py
+-rw-r--r--   0 narval     (111) narval     (116)     2392 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/0.6.0_Any.py
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-21 14:09:02.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/
+-rw-r--r--   0 narval     (111) narval     (116)   131456 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/languages.csv
+-rw-r--r--   0 narval     (111) narval     (116)     2469 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/level_type.csv
+-rw-r--r--   0 narval     (111) narval     (116)      202 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/measurement_units_type.csv
+-rw-r--r--   0 narval     (111) narval     (116)      115 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/final_action_storage_code_type.csv
+-rw-r--r--   0 narval     (111) narval     (116)    64714 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/mime_types.csv
+-rw-r--r--   0 narval     (111) narval     (116)      177 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/legal_status.csv
+-rw-r--r--   0 narval     (111) narval     (116)     1498 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/dissemination.csv
+-rw-r--r--   0 narval     (111) narval     (116)      187 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/final_action_appraisal_code_type.csv
+-rw-r--r--   0 narval     (111) narval     (116)      583 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/encodings.csv
+-rw-r--r--   0 narval     (111) narval     (116)      150 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/classification_levels.csv
+-rw-r--r--   0 narval     (111) narval     (116)     3877 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/document_type_code.csv
+-rw-r--r--   0 narval     (111) narval     (116)      327 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/code_keyword_type.csv
+-rw-r--r--   0 narval     (111) narval     (116)      628 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/digest_algorithms.csv
+-rw-r--r--   0 narval     (111) narval     (116)      176 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/measurement_weight_units_type.csv
+-rw-r--r--   0 narval     (111) narval     (116)      149 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/event_types.csv
+-rw-r--r--   0 narval     (111) narval     (116)      271 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/dua.csv
+-rw-r--r--   0 narval     (111) narval     (116)    29311 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/file_formats.csv
+-rw-r--r--   0 narval     (111) narval     (116)     7022 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/migration/data/access_control.csv
+-rw-r--r--   0 narval     (111) narval     (116)     3214 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/cubicweb_seda/xsd2entities.py
+-rw-r--r--   0 narval     (111) narval     (116)     1250 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/tox.ini
+-rw-r--r--   0 narval     (111) narval     (116)       52 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/README
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-21 14:09:02.000000 cubicweb-seda-0.9.0/cubicweb_seda.egg-info/
+-rw-rw-r--   0 narval     (111) narval     (116)        1 2017-03-21 14:02:28.000000 cubicweb-seda-0.9.0/cubicweb_seda.egg-info/not-zip-safe
+-rw-rw-r--   0 narval     (111) narval     (116)       14 2017-03-21 14:08:59.000000 cubicweb-seda-0.9.0/cubicweb_seda.egg-info/top_level.txt
+-rw-rw-r--   0 narval     (111) narval     (116)       39 2017-03-21 14:08:59.000000 cubicweb-seda-0.9.0/cubicweb_seda.egg-info/entry_points.txt
+-rw-rw-r--   0 narval     (111) narval     (116)     3870 2017-03-21 14:08:59.000000 cubicweb-seda-0.9.0/cubicweb_seda.egg-info/SOURCES.txt
+-rw-rw-r--   0 narval     (111) narval     (116)        1 2017-03-21 14:08:59.000000 cubicweb-seda-0.9.0/cubicweb_seda.egg-info/dependency_links.txt
+-rw-rw-r--   0 narval     (111) narval     (116)      518 2017-03-21 14:08:59.000000 cubicweb-seda-0.9.0/cubicweb_seda.egg-info/PKG-INFO
+-rw-rw-r--   0 narval     (111) narval     (116)      161 2017-03-21 14:08:59.000000 cubicweb-seda-0.9.0/cubicweb_seda.egg-info/requires.txt
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-21 14:09:02.000000 cubicweb-seda-0.9.0/doc/
+-rw-r--r--   0 narval     (111) narval     (116)     2100 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/doc/profils.rst
+-rw-r--r--   0 narval     (111) narval     (116)      198 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/doc/index.rst
+-rw-r--r--   0 narval     (111) narval     (116)     8116 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/doc/conf.py
+-rw-rw-r--   0 narval     (111) narval     (116)      518 2017-03-21 14:09:02.000000 cubicweb-seda-0.9.0/PKG-INFO
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-21 14:09:02.000000 cubicweb-seda-0.9.0/test/
+-rw-r--r--   0 narval     (111) narval     (116)     6176 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/test_html_generation.py
+-rw-r--r--   0 narval     (111) narval     (116)     2391 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/pytestconf.py
+-rw-r--r--   0 narval     (111) narval     (116)     6927 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/test_diag.py
+-rw-r--r--   0 narval     (111) narval     (116)    15200 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/test_entities.py
+-rw-r--r--   0 narval     (111) narval     (116)    17944 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/test_schema.py
+-rw-r--r--   0 narval     (111) narval     (116)     1272 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/test_dataimport.py
+-rw-r--r--   0 narval     (111) narval     (116)     4252 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/testutils.py
+-rw-r--r--   0 narval     (111) narval     (116)    14487 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/test_xsd2yams.py
+-rw-r--r--   0 narval     (111) narval     (116)    10416 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/test_hooks.py
+-rw-r--r--   0 narval     (111) narval     (116)    31241 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/test_views.py
+drwxrwxr-x   0 narval     (111) narval     (116)        0 2017-03-21 14:09:02.000000 cubicweb-seda-0.9.0/test/data/
+-rw-r--r--   0 narval     (111) narval     (116)    11890 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/data/BV2.0_min.xml
+-rw-r--r--   0 narval     (111) narval     (116)    13473 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/data/exArchiveTransfer1_SEDA2_min.xml
+-rw-r--r--   0 narval     (111) narval     (116)    22822 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/data/seda_1_export.rng
+-rw-r--r--   0 narval     (111) narval     (116)     8126 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/data/relaxng.rng
+-rw-r--r--   0 narval     (111) narval     (116)     8450 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/data/exArchiveTransfert2_SEDA2_min.xml
+-rw-r--r--   0 narval     (111) narval     (116)        5 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/data/bootstrap_cubes
+-rw-r--r--   0 narval     (111) narval     (116)    21443 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/data/seda_02_export.rng
+-rw-r--r--   0 narval     (111) narval     (116)    26961 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/data/seda_1_export.xsd
+-rw-r--r--   0 narval     (111) narval     (116)    24970 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/data/seda_02_export.xsd
+-rw-r--r--   0 narval     (111) narval     (116)    71264 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/data/XMLSchema.xsd
+-rw-r--r--   0 narval     (111) narval     (116)     2468 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/data/seda_02_bordereau_ref.xml
+-rw-r--r--   0 narval     (111) narval     (116)    47494 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/test/test_profile_generation.py
+-rw-r--r--   0 narval     (111) narval     (116)     2587 2017-03-21 14:02:21.000000 cubicweb-seda-0.9.0/setup.py
```

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/xsd2yams.py` & `cubicweb-seda-0.9.0/cubicweb_seda/xsd2yams.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/xsd2uicfg.py` & `cubicweb-seda-0.9.0/cubicweb_seda/xsd2uicfg.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/entities/itree.py` & `cubicweb-seda-0.9.0/cubicweb_seda/entities/itree.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/entities/profile_generation.py` & `cubicweb-seda-0.9.0/cubicweb_seda/entities/profile_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,29 +206,32 @@
         minimum == 1.
         """
         if minimum == 1:
             return parent
         else:
             return self.element('rng:optional', parent)
 
-    def rng_value(self, element, qualified_datatype, fixed_value=None):
+    def rng_value(self, element, qualified_datatype, fixed_value=None, default_value=None):
         """Given a (etree) schema element, a data type (e.g. 'xsd:token') and an optional fixed
         value, add RNG declaration to the element to declare the datatype and fix the value if
         necessary.
         """
         prefix, datatype = qualified_datatype.split(':')
         if prefix != 'xsd':
             # XXX RelaxNG compatible version of custom types? this would allow
             # `type_attrs['datatypeLibrary'] = self.namespaces[prefix]`. In the mean time, turn
             # every custom type to string, supposing transfer are also checked against the original
             # schema (as agape v1 was doing).
             datatype = 'string'
         type_attrs = {'type': datatype}
         if fixed_value is not None:
             self.element('rng:value', element, type_attrs, text=fixed_value)
+        elif default_value is not None:
+            element.attrib[self.qname('a:defaultValue')] = default_value
+            self.element('rng:data', element, type_attrs)
         else:
             self.element('rng:data', element, type_attrs)
 
 
 class SEDA2ExportAdapter(EntityAdapter):
     """Abstract base class for export of SEDA profile."""
     __abstract__ = True
@@ -747,26 +750,14 @@
 
     def _create_hierarchy(self, parent, tags):
         for tag in tags:
             parent = self.element(tag, parent)
         return parent
 
 
-def climb_rule_holders(transfer_or_archive_unit):
-    """Starting from a transfer or archive unit entity, yield entity that may be linked to management
-    rule until the root (transfer) is reached.
-    """
-    while transfer_or_archive_unit is not None:
-        if transfer_or_archive_unit.cw_etype == 'SEDAArchiveTransfer':
-            yield transfer_or_archive_unit
-        else:
-            yield transfer_or_archive_unit.first_level_choice.content_sequence
-        transfer_or_archive_unit = transfer_or_archive_unit.cw_adapt_to('ITreeBase').parent()
-
-
 def _safe_cardinality(entity):
     """Return entity's cardinality if some entity is given, else None."""
     if entity is None:
         return None
     return entity.user_cardinality
 
 
@@ -831,19 +822,27 @@
         'attributeFormDefault': 'unqualified',
         'elementFormDefault': 'qualified',
         'version': '1.0',
     }
 
     concepts_language = 'seda-1'
 
-    def element_schema(self, parent, name, xsd_type=None, fixed_value=None, cardinality='1',
-                       documentation=None, xsd_attributes=()):
+    def element_schema(self, parent, name, xsd_type=None,
+                       fixed_value=None, default_value=None,
+                       cardinality='1', documentation=None,
+                       xsd_attributes=(), extra_attributes=None):
+        assert not (fixed_value and default_value), \
+            'only one of fixed_value or default_value may be specified'
         attributes = {'name': name}
+        if extra_attributes is not None:
+            attributes.update(extra_attributes)
         if fixed_value is not None:
             attributes['fixed'] = text_type(fixed_value)
+        elif default_value is not None:
+            attributes['default'] = text_type(default_value)
         if xsd_type is not None and not xsd_attributes:
             attributes['type'] = xsd_type
         assert cardinality in ('0..1', '0..n', '1', '1..n')
         if cardinality != '1':
             if cardinality[0] == '0':
                 attributes['minOccurs'] = '0'
             if cardinality[-1] == 'n':
@@ -884,29 +883,15 @@
         #              attributes={'namespace': 'http://www.w3.org/XML/1998/namespace',
         #                          'schemaLocation': 'http://www.w3.org/2001/xml.xsd'})
         self.xsd_transfer(root, self.entity)
         return root
 
     def xsd_transfer(self, parent, archive_transfer):
         """Append XSD elements for the archive transfer to the given parent node."""
-        transfer_node = self.element_schema(parent, 'ArchiveTransfer',
-                                            documentation=archive_transfer.title,
-                                            xsd_attributes=[XAttr('Id', 'xsd:ID')])
-        for comment in archive_transfer.comments:
-            self.element_schema(transfer_node, 'Comment', 'udt:TextType',
-                                fixed_value=comment.comment,
-                                cardinality=comment.user_cardinality,
-                                documentation=comment.user_annotation,
-                                xsd_attributes=[XAttr('languageID', 'xsd:language')])
-        self.element_schema(transfer_node, 'Date', 'udt:DateTimeType')
-        self.element_schema(transfer_node, 'TransferIdentifier', 'qdt:ArchivesIDType',
-                            xsd_attributes=self.xsd_attributes_scheme())
-        for agency_type in ('TransferringAgency', 'ArchivalAgency'):
-            self.xsd_agency(transfer_node, agency_type)
-
+        transfer_node = self.xsd_transfer_base(parent, archive_transfer)
         for archive_unit in archive_transfer.archive_units:
             self.xsd_archive(transfer_node, archive_unit)
 
     def xsd_archive(self, parent, archive_unit):
         """Append XSD elements for an archive to the given parent node."""
         archive_node = self.element_schema(parent, 'Archive',
                                            cardinality=archive_unit.user_cardinality,
@@ -923,19 +908,19 @@
                             fixed_value=name_entity.title,
                             documentation=name_entity.user_annotation,
                             xsd_attributes=[XAttr('languageID', 'xsd:language')])
         content_entity = self.archive_unit_content(archive_unit)
         self.xsd_transferring_agency_archive_identifier(archive_node, content_entity,
                                                         'TransferringAgencyArchiveIdentifier')
         self.xsd_content_description(archive_node, content_entity)
-        appraisal_rule_entity = self.archive_unit_appraisal_rule(archive_unit)
+        appraisal_rule_entity = archive_unit.inherited_rule('appraisal')
         if appraisal_rule_entity:
             self.xsd_appraisal_rule(archive_node, appraisal_rule_entity)
         # not optional in seda 1
-        access_rule_entity = self.archive_unit_access_rule(archive_unit)
+        access_rule_entity = archive_unit.inherited_rule('access')
         self.xsd_access_rule(archive_node, access_rule_entity)
         self.xsd_children(archive_node, archive_unit)
 
     archive_object_tag_name = 'ArchiveObject'
 
     def xsd_archive_object(self, parent, archive_unit):
         """Append XSD elements for the archive object to the given parent node."""
@@ -952,18 +937,18 @@
                                                         'TransferringAgencyObjectIdentifier')
         if (self.__regid__.startswith('SEDA-1.0')
                 or content_entity.start_date
                 or content_entity.end_date
                 or content_entity.description
                 or content_entity.keywords):
             self.xsd_content_description(ao_node, content_entity)
-        appraisal_rule_entity = self.archive_unit_appraisal_rule(archive_unit)
+        appraisal_rule_entity = archive_unit.inherited_rule('appraisal')
         if appraisal_rule_entity:
             self.xsd_appraisal_rule(ao_node, appraisal_rule_entity)
-        access_rule_entity = self.archive_unit_access_rule(archive_unit)
+        access_rule_entity = archive_unit.inherited_rule('access')
         if access_rule_entity:
             self.xsd_access_rule(ao_node, access_rule_entity)
         self.xsd_children(ao_node, archive_unit)
 
         return ao_node
 
     def xsd_document(self, parent, data_object):
@@ -972,27 +957,47 @@
                                             cardinality=data_object.user_cardinality,
                                             documentation=data_object.user_annotation,
                                             xsd_attributes=[XAttr('Id', 'xsd:ID')])
 
         self.xsd_system_id(document_node, data_object)
         self.xsd_attachment(document_node, data_object)
         self.xsd_date_created(document_node, data_object)
+        self.xsd_integrity(document_node, data_object)
         self.xsd_document_type(document_node, data_object)
 
     def xsd_children(self, parent, entity):
         """Iter on archive/archive object children, which may be either
         archive objects or documents, and append XSD elements for them to the given parent node.
         """
         for au_or_bdo in entity.cw_adapt_to('ITreeBase').iterchildren():
             if au_or_bdo.cw_etype == 'SEDABinaryDataObject':
                 self.xsd_document(parent, au_or_bdo)
             else:
                 assert au_or_bdo.cw_etype == 'SEDAArchiveUnit'
                 self.xsd_archive_object(parent, au_or_bdo)
 
+    def xsd_transfer_base(self, parent, archive_transfer):
+        """Create ArchiveTransfer element and add child which are common in 0.2 and 1.0.
+        """
+        transfer_node = self.element_schema(parent, 'ArchiveTransfer',
+                                            documentation=archive_transfer.title,
+                                            xsd_attributes=[XAttr('Id', 'xsd:ID')])
+        for comment in archive_transfer.comments:
+            self.element_schema(transfer_node, 'Comment', 'udt:TextType',
+                                fixed_value=comment.comment,
+                                cardinality=comment.user_cardinality,
+                                documentation=comment.user_annotation,
+                                xsd_attributes=[XAttr('languageID', 'xsd:language')])
+        self.element_schema(transfer_node, 'Date', 'udt:DateTimeType')
+        self.element_schema(transfer_node, 'TransferIdentifier', 'qdt:ArchivesIDType',
+                            xsd_attributes=self.xsd_attributes_scheme())
+        for agency_type in ('TransferringAgency', 'ArchivalAgency'):
+            self.xsd_agency(transfer_node, agency_type)
+        return transfer_node
+
     def xsd_attachment(self, parent, data_object):
         _safe_concept = partial(_safe_concept_value, concepts_language=self.concepts_language)
 
         format_id = data_object.format_id
         encoding = data_object.encoding
         mime_type = data_object.mime_type
         self.element_schema(parent, 'Attachment', 'qdt:ArchivesBinaryObjectType',
@@ -1171,14 +1176,23 @@
                                                           cardinality=when_card),
                                                     XAttr('languageID', 'xsd:language')])
 
     def xsd_originating_agency(self, parent, content):
         if content.originating_agency:
             self.xsd_agency(parent, 'OriginatingAgency', content.originating_agency)
 
+    def xsd_integrity(self, parent, data_object):
+        algorithm = data_object.seda_algorithm[0] if data_object.seda_algorithm else None
+        self.element_schema(parent, 'Integrity', 'qdt:ArchivesHashcodeBinaryObjectType',
+                            cardinality='0..1',
+                            xsd_attributes=[XAttr('algorithme', 'xsd:string',
+                                                  cardinality='1',
+                                                  fixed_value=_concept_value(
+                                                      algorithm, self.concepts_language))])
+
     # extracted from xsd_keyword to allow parametrization for SEDA 1.0 vs 0.2 generation
     kw_tag_name = 'Keyword'
     kw_content_tag_type = 'qdt:KeywordContentType'
     kw_content_tag_attributes = [XAttr('role', 'xsd:token'),
                                  XAttr('languageID', 'xsd:language')]
 
     def xsd_keyword(self, parent, keyword):
@@ -1230,30 +1244,18 @@
         ]
         # if scheme is not None:
         #     # schemeID XXX move to saem
         #     attributes[0]['fixed'] = scheme.ark
         #     attributes[0]['use'] = 'required'
         return attributes
 
-    def archive_unit_access_rule(self, archive_unit):
-        for rule_holder in climb_rule_holders(archive_unit):
-            if rule_holder.reverse_seda_access_rule:
-                return rule_holder.reverse_seda_access_rule[0]
-        return None
-
     def archive_unit_name(self, archive_unit):
         seq = archive_unit.first_level_choice.content_sequence
         return seq.title
 
-    def archive_unit_appraisal_rule(self, archive_unit):
-        for rule_holder in climb_rule_holders(archive_unit):
-            if rule_holder.reverse_seda_appraisal_rule:
-                return rule_holder.reverse_seda_appraisal_rule[0]
-        return None
-
     def agency_name(self, agency):
         return agency.agency.dc_title() if agency and agency.agency else None
 
     def agency_id(self, agency):
         return text_type(agency.agency.eid) if agency and agency.agency else None
 
     def archive_unit_content(self, archive_unit):
@@ -1276,19 +1278,30 @@
     """Adapter to build an XSD representation of a SEDA profile, using SEDA 0.2 specification"""
     __regid__ = 'SEDA-0.2.xsd'
 
     namespaces = SEDA1XSDExport.namespaces.copy()
     namespaces[None] = 'fr:gouv:ae:archive:draft:standard_echange_v0.2'
     namespaces['qdt'] = 'fr:gouv:ae:archive:draft:standard_echange_v0.2:QualifiedDataType:1'
     namespaces['udt'] = 'urn:un:unece:uncefact:data:standard:UnqualifiedDataType:6'
+    namespaces['seda'] = 'fr:gouv:culture:archivesdefrance:seda:v2.0'
 
     root_attributes = SEDA1XSDExport.root_attributes.copy()
     root_attributes['targetNamespace'] = 'fr:gouv:ae:archive:draft:standard_echange_v0.2'
     root_attributes['version'] = '1.1'
 
+    def xsd_transfer(self, parent, archive_transfer):
+        """Append XSD elements for the archive transfer to the given parent node."""
+        transfer_node = self.xsd_transfer_base(parent, archive_transfer)
+
+        for data_object in archive_transfer.binary_data_objects:
+            self.xsd_integrity(transfer_node, data_object)
+
+        for archive_unit in archive_transfer.archive_units:
+            self.xsd_archive(transfer_node, archive_unit)
+
     def xsd_archive(self, parent, archive_unit):
         """Append XSD elements for an archive to the given parent node."""
         archive_node = self.element_schema(parent, 'Contains',
                                            cardinality=archive_unit.user_cardinality,
                                            documentation=archive_unit.user_annotation,
                                            xsd_attributes=[XAttr('Id', 'xsd:ID')])
         transfer = archive_unit.cw_adapt_to('ITreeBase').parent()
@@ -1305,19 +1318,19 @@
                             fixed_value=name_entity.title,
                             documentation=name_entity.user_annotation,
                             xsd_attributes=[XAttr('languageID', 'xsd:language')])
         self.xsd_transferring_agency_archive_identifier(archive_node, content_entity,
                                                         'TransferringAgencyArchiveIdentifier')
         self.xsd_content_description(archive_node, content_entity)
 
-        appraisal_rule_entity = self.archive_unit_appraisal_rule(archive_unit)
+        appraisal_rule_entity = archive_unit.inherited_rule('appraisal')
         if appraisal_rule_entity:
             self.xsd_appraisal_rule(archive_node, appraisal_rule_entity)
         # in SEDA 0.2, access restriction is not mandatory
-        access_rule_entity = self.archive_unit_access_rule(archive_unit)
+        access_rule_entity = archive_unit.inherited_rule('access')
         if access_rule_entity:
             self.xsd_access_rule(archive_node, access_rule_entity)
         self.xsd_children(archive_node, archive_unit)
         return archive_node
 
     def xsd_archive_object(self, parent, archive_unit):
         """Append XSD elements for the archive object to the given parent node."""
@@ -1328,17 +1341,19 @@
         self.xsd_description_level(ao_node, content_entity.description_level_concept)
         # actually DescriptionLevel should be before Name (ie. currently the last and first
         # elements)
         ao_node.insert(0, ao_node[-1])
 
     def xsd_document(self, parent, data_object):
         """Append XSD elements for the document to the given parent node."""
+        xmlid = eid2xmlid(data_object.eid)
         document_node = self.element_schema(parent, 'Document',
                                             cardinality=data_object.user_cardinality,
                                             documentation=data_object.user_annotation,
+                                            extra_attributes={'seda:profid': xmlid},
                                             xsd_attributes=[XAttr('Id', 'xsd:ID')])
 
         self.xsd_attachment(document_node, data_object)
         self.xsd_date_created(document_node, data_object)
         self.xsd_system_id(document_node, data_object)
         self.xsd_document_type(document_node, data_object)
 
@@ -1357,40 +1372,57 @@
         if content.custodial_history_items:
             item = content.custodial_history_items[0]
             self.element_schema(parent, 'CustodialHistory', 'udt:TextType',
                                 cardinality=item.user_cardinality,
                                 documentation=item.user_annotation,
                                 xsd_attributes=[XAttr('languageID', 'xsd:language')])
 
+    def xsd_integrity(self, parent, data_object):
+        integrity = self.element_schema(parent, 'Integrity', cardinality='0..1')
+        algorithm = data_object.seda_algorithm[0] if data_object.seda_algorithm else None
+        self.element_schema(integrity, 'Contains', 'qdt:ArchivesHashcodeBinaryObjectType',
+                            xsd_attributes=[XAttr('algorithme', 'xsd:string',
+                                                  cardinality='1',
+                                                  fixed_value=_concept_value(
+                                                      algorithm, self.concepts_language))])
+        self.element_schema(integrity, 'UnitIdentifier', 'qdt:ArchivesIDType',
+                            default_value=eid2xmlid(data_object.eid))
+
     system_id_tag_name = 'Identification'
     # in SEDA 0.2, ArchiveObject tag name is 'Contains' (as for Archive)
     archive_object_tag_name = 'Contains'
     # in SEDA 0.2, AccessRestrictionRule tag name is 'AccessRestriction'
     access_restriction_tag_name = 'AccessRestriction'
     # in SEDA 0.2, keyword tag name is 'ContentDescriptive', not 'Keyword' and keyword content type
     # is TextType and there is no 'role' attribute
     kw_tag_name = 'ContentDescriptive'
     kw_content_tag_type = 'udt:TextType'
     kw_content_tag_attributes = [XAttr('languageID', 'xsd:language')]
 
 
 class OldSEDARNGExportMixin(RNGMixin):
 
-    def element_schema(self, parent, name, xsd_type=None, fixed_value=None, cardinality='1',
-                       documentation=None, xsd_attributes=()):
+    def element_schema(self, parent, name, xsd_type=None,
+                       fixed_value=None, default_value=None,
+                       cardinality='1', documentation=None,
+                       xsd_attributes=(), extra_attributes=None):
+        assert not (fixed_value and default_value), \
+            'only one of fixed_value or default_value may be specified'
         attributes = {'name': name}
+        if extra_attributes is not None:
+            attributes.update(extra_attributes)
         if documentation:
             attributes['documentation'] = documentation
         parent = self.rng_element_parent(parent, *minmax_cardinality(cardinality))
         element = self.element('rng:element', parent, attributes)
         for xattr in xsd_attributes:
             self.attribute_schema(element, xattr)
 
         if xsd_type is not None:
-            self.rng_value(element, xsd_type, fixed_value)
+            self.rng_value(element, xsd_type, fixed_value, default_value)
         else:
             assert fixed_value is None
         return element
 
     def attribute_schema(self, parent, xattr):
         if xattr.cardinality is None:
             return  # XXX prohibit?
@@ -1425,14 +1457,16 @@
     """Adapter to build an RNG representation of a simplified SEDA profile, using SEDA 0.2
     specification.
     """
     __regid__ = 'SEDA-0.2.rng'
 
     namespaces = SEDA1XSDExport.namespaces.copy()
     namespaces['rng'] = 'http://relaxng.org/ns/structure/1.0'
+    namespaces['a'] = 'http://relaxng.org/ns/compatibility/annotations/1.0'
+    namespaces['seda'] = 'fr:gouv:culture:archivesdefrance:seda:v2.0'
     root_attributes = {
         'ns': 'fr:gouv:ae:archive:draft:standard_echange_v0.2',
         'datatypeLibrary': 'http://www.w3.org/2001/XMLSchema-datatypes',
     }
 
 
 def xsd_element_cardinality(occ, card_entity):
```

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/entities/custom.py` & `cubicweb-seda-0.9.0/cubicweb_seda/entities/custom.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,24 +10,52 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <http://www.gnu.org/licenses/>.
 
-from . import generated
+from ..xsd2yams import RULE_TYPES
+from . import generated, itree
 
 
 def _extract_title(annotation):
     """Return the first line in the annotation to use as a title"""
     annotation = annotation.strip()
     assert annotation
     return annotation.splitlines()[0]
 
 
+def _climb_rule_holders(transfer_or_archive_unit):
+    """Starting from a transfer or archive unit entity, yield entity that may be linked to
+    management rule until the root (transfer) is reached.
+    """
+    while transfer_or_archive_unit is not None:
+        if transfer_or_archive_unit.cw_etype == 'SEDASeqAltArchiveUnitArchiveUnitRefIdManagement':
+            yield transfer_or_archive_unit
+            transfer_or_archive_unit = itree.parent_archive_unit(transfer_or_archive_unit)
+        elif transfer_or_archive_unit.cw_etype == 'SEDAArchiveTransfer':
+            yield transfer_or_archive_unit
+        else:
+            yield transfer_or_archive_unit.first_level_choice.content_sequence
+        transfer_or_archive_unit = transfer_or_archive_unit.cw_adapt_to('ITreeBase').parent()
+
+
+def _inherited_rule(self, rule_type):
+    """Return the rule entity of the given type, defined on this unit or in its nearest parent
+    possible defining it, or None if no matching rule has been found.
+    """
+    assert rule_type in RULE_TYPES
+    rtype = 'reverse_seda_{}_rule'.format(rule_type)
+    for rule_holder in _climb_rule_holders(self):
+        if getattr(rule_holder, rtype):
+            return getattr(rule_holder, rtype)[0]
+    return None
+
+
 class SEDAArchiveTransfer(generated.SEDAArchiveTransfer):
 
     def dc_title(self):
         return self.title
 
     @property
     def formats_compat(self):
@@ -53,14 +81,16 @@
     def physical_data_objects(self):
         return self.reverse_seda_physical_data_object
 
     @property
     def binary_data_objects(self):
         return self.reverse_seda_binary_data_object
 
+    inherited_rule = _inherited_rule
+
 
 class SEDAArchiveUnit(generated.SEDAArchiveUnit):
 
     def dc_title(self):
         return _extract_title(self.user_annotation)
 
     @property
@@ -73,14 +103,16 @@
     @property
     def first_level_choice(self):
         """Return the choice element of an archive unit (SEDAAltArchiveUnitArchiveUnitRefId),
         holding either a reference or descriptive content
         """
         return self.related('seda_alt_archive_unit_archive_unit_ref_id', 'subject').one()
 
+    inherited_rule = _inherited_rule
+
 
 class SEDABinaryDataObject(generated.SEDABinaryDataObject):
 
     def dc_title(self):
         return _extract_title(self.user_annotation)
 
     @property
@@ -186,14 +218,16 @@
 
     @property
     def originating_agency(self):
         if self.reverse_seda_originating_agency_from:
             return self.reverse_seda_originating_agency_from[0]
         return None
 
+    inherited_rule = _inherited_rule
+
 
 class SEDAKeyword(generated.SEDAKeyword):
 
     @property
     def reference(self):
         return (self.reverse_seda_keyword_reference_from[0]
                 if self.reverse_seda_keyword_reference_from else None)
```

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/entities/__init__.py` & `cubicweb-seda-0.9.0/cubicweb_seda/entities/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,61 +70,64 @@
         if icontained is not None and icontained.container:
             container = icontained.container
         elif parent.cw_adapt_to('IContainer'):
             container = parent
     return parent, container
 
 
-def _seda_container_from_context(rset, entity):
+def _seda_container_from_context(rset, entity, **kwargs):
     if entity is None:
-        entity = rset.one()
+        if 'row' in kwargs:
+            entity = rset.get_entity(kwargs['row'], kwargs.get('col', 0))
+        else:
+            entity = rset.one()
     # protect against unrelated entity types
     if not entity.cw_etype.startswith('SEDA'):
         return None
     if entity.cw_etype != 'SEDAArchiveTransfer':
         entity = parent_and_container(entity)[1]
     return entity
 
 
 @objectify_predicate
 def component_unit(cls, req, rset=None, entity=None, **kwargs):
     """Predicate returning 1 score if context entity is within "component" archive unit (i.e.
     container root is not a SEDAArchiveTransfer but a SEDAArchiveUnit).
     """
-    entity = _seda_container_from_context(rset, entity)
+    entity = _seda_container_from_context(rset, entity, **kwargs)
     return 1 if entity.cw_etype == 'SEDAArchiveUnit' else 0
 
 
 @objectify_predicate
 def simplified_profile(cls, req, rset=None, entity=None, **kwargs):
     """Predicate returning 1 score if context entity is within a simplified profile."""
-    entity = _seda_container_from_context(rset, entity)
+    entity = _seda_container_from_context(rset, entity, **kwargs)
     if entity is None:
         return 0
     if entity.cw_etype == 'SEDAArchiveUnit':
         # XXX archive unit component, for now suppose it's "simplified"
         return 1
     return 1 if entity.simplified_profile else 0
 
 
-def is_full_seda2_profile(entity=None, rset=None):
+def is_full_seda2_profile(entity=None, rset=None, **kwargs):
     """Return 1 if context entity is within a full seda2 profile, else 0."""
-    entity = _seda_container_from_context(rset, entity)
+    entity = _seda_container_from_context(rset, entity, **kwargs)
     if entity is None:
         return 1
     if entity.cw_etype == 'SEDAArchiveUnit':
         # XXX archive unit component, for now suppose it's "simplified"
         return 0
     return 0 if entity.simplified_profile else 1
 
 
 @objectify_predicate
 def full_seda2_profile(cls, req, rset=None, entity=None, **kwargs):
     """Predicate returning 1 score if context entity is within a full seda2 profile."""
-    return is_full_seda2_profile(entity, rset)
+    return is_full_seda2_profile(entity, rset, **kwargs)
 
 
 def rule_type_from_etype(etype):
     """Return the rule type (e.g. 'access') from an etype enclosing the information
     (e.g. 'SEDAAltAccessRulePreventInheritance', 'SEDASeqAaccessRuleRule' or 'SEDAAccessRule')
     """
     if etype.startswith('SEDAAlt'):
```

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/entities/html_generation.py` & `cubicweb-seda-0.9.0/cubicweb_seda/entities/html_generation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/entities/diag.py` & `cubicweb-seda-0.9.0/cubicweb_seda/entities/diag.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/entities/generated.py` & `cubicweb-seda-0.9.0/cubicweb_seda/entities/generated.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/xsd.py` & `cubicweb-seda-0.9.0/cubicweb_seda/xsd.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/dataimport.py` & `cubicweb-seda-0.9.0/cubicweb_seda/dataimport.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     (u'SEDA 2 : Unités de mesure',
      'seda_unit', ('SEDAWidth', 'SEDAHeight', 'SEDADepth',
                    'SEDADiameter', 'SEDALength', 'SEDAThickness'),
      'measurement_units_type.csv'),
     (u'SEDA 2 : Unités de poids',
      'seda_unit', 'SEDAWeight',
      'measurement_weight_units_type.csv'),
-    (u'SEDA 2 : Types de mot-clé',
+    (u'SEDA : Types de mot-clé',
      'seda_keyword_type_to', (),
      'code_keyword_type.csv'),
     (u'SEDA 2 : Status légaux',
      'seda_legal_status_to', (),
      'legal_status.csv'),
     (u'SEDA : Niveaux de description',
      'seda_description_level', (),
```

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/hooks.py` & `cubicweb-seda-0.9.0/cubicweb_seda/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/xsd2concepts.py` & `cubicweb-seda-0.9.0/cubicweb_seda/xsd2concepts.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/schema/__init__.py` & `cubicweb-seda-0.9.0/cubicweb_seda/schema/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 # with this program. If not, see <http://www.gnu.org/licenses/>.
 """cubicweb-seda schema"""
 
 from yams.buildobjs import RelationType, RelationDefinition
 from yams.buildobjs import String
 
 from cubicweb import _
-from cubicweb.schema import ERQLExpression, RRQLExpression
+from cubicweb.schema import ERQLExpression, RRQLExpression, RQLConstraint
+
 from cubes.skos import schema as skos
 
 _('1')
 _('0..1')
 _('0..n')
 _('1..n')
 
@@ -86,28 +87,31 @@
 
 class container(RelationType):
     __permissions__ = {'add': (), 'delete': (), 'read': ()}
     cardinality = '1*'
     inlined = False
 
 
-class clone_of_archive_transfer(RelationDefinition):
+class _clone_of(RelationDefinition):
+    __permissions__ = {'read': ('managers', 'users', 'guests'),
+                       'add': ('managers', 'users',),
+                       'delete': ()}
     name = 'clone_of'
-    subject = 'SEDAArchiveTransfer'
-    object = 'SEDAArchiveTransfer'
     cardinality = '?*'
     inlined = True
 
 
-class clone_of_archive_unit(RelationDefinition):
-    name = 'clone_of'
+class clone_of_archive_transfer(_clone_of):
+    subject = 'SEDAArchiveTransfer'
+    object = 'SEDAArchiveTransfer'
+
+
+class clone_of_archive_unit(_clone_of):
     subject = 'SEDAArchiveUnit'
     object = 'SEDAArchiveUnit'
-    cardinality = '?*'
-    inlined = True
 
 
 class title(RelationDefinition):
     subject = 'SEDAArchiveTransfer'
     object = 'String'
     description = _('title for this profile, not used in the generated schema')
     cardinality = '11'
@@ -119,14 +123,29 @@
     object = 'Boolean'
     default = False
     description = _('simplified profiles are compatible with older version of SEDA, but have not '
                     'the full SEDA 2 expressivness')
     cardinality = '11'
 
 
+class code_keyword_type(RelationDefinition):
+    __permissions__ = {
+        'read': ('managers', 'users', 'guests'),
+        'add': ('managers', RRQLExpression('U has_update_permission S')),
+        'delete': ('managers', RRQLExpression('U has_update_permission S')),
+    }
+    subject = 'ConceptScheme'
+    object = 'Concept'
+    cardinality = '?*'
+    inlined = True
+    description = _('SEDA code keyword type for this scheme')
+    constraints = [RQLConstraint('O in_scheme CS, CS scheme_relation_type RT, '
+                                 'RT name "seda_keyword_type_to"')]
+
+
 class compat_list(RelationDefinition):
     __permissions__ = {'read': ('managers', 'users', 'guests',),
                        'add': (),
                        'update': ()}
     subject = 'SEDAArchiveTransfer'
     object = 'String'
     description = _("names of format in which the profile may be exported (e.g. 'SEDA 2, SEDA 1')")
@@ -168,17 +187,27 @@
                      ERQLExpression('U has_{action}_permission C, '
                                     'X container C'.format(action=action)),
                      ERQLExpression('NOT EXISTS(X container C), U in_group G, '
                                     'G name IN ("managers", "users")')))
     # set permissions on all relation defs related to the compound graph according to permission on
     # the container entity
     for rdef, role in iter_all_rdefs(schema, 'SEDAArchiveTransfer'):
+        if rdef.rtype == 'clone_of':
+            continue
         if role == 'subject':
             target_etype, var = rdef.subject, 'S'
         else:
             target_etype, var = rdef.object, 'O'
-        if target_etype == 'SEDAArchiveTransfer':
-            expr = 'U has_update_permission {0}'.format(var)
+        rrql_exprs = []
+        if target_etype == 'SEDAArchiveUnit':
+            rrql_exprs.append('U has_update_permission {0}, NOT EXISTS({0} container C)'
+                              .format(var, var))
+            rrql_exprs.append('U has_update_permission C, {0} container C'.format(var))
+
         else:
-            expr = 'U has_update_permission C, {0} container C'.format(var)
+            if target_etype == 'SEDAArchiveTransfer':
+                rrql_exprs.append('U has_update_permission {0}'.format(var))
+            else:
+                rrql_exprs.append('U has_update_permission C, {0} container C'.format(var))
+        permissions = ['managers'] + [RRQLExpression(expr) for expr in rrql_exprs]
         for action in ('add', 'delete'):
-            rdef.set_action_permissions(action, ('managers', RRQLExpression(expr)))
+            rdef.set_action_permissions(action, permissions)
```

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/schema/seda2.py` & `cubicweb-seda-0.9.0/cubicweb_seda/schema/seda2.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/views/jqtree.py` & `cubicweb-seda-0.9.0/cubicweb_seda/views/jqtree.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/views/patches.py` & `cubicweb-seda-0.9.0/cubicweb_seda/views/patches.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/views/export.py` & `cubicweb-seda-0.9.0/cubicweb_seda/views/export.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/views/simplified.py` & `cubicweb-seda-0.9.0/cubicweb_seda/views/simplified.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 # You should have received a copy of the GNU Lesser General Public License along
 # with this program. If not, see <http://www.gnu.org/licenses/>.
 """cubicweb-seda views configuration / overrides for simplified profiles."""
 
 from logilab.common.registry import objectify_predicate
 
 from cubicweb.predicates import is_instance
-from cubicweb.web.views import uicfg, autoform, formrenderers
+from cubicweb.web.views import uicfg, autoform
 
+from ..xsd2yams import RULE_TYPES
 from ..entities import simplified_profile
 from . import CONTENT_ETYPE, copy_rtag
 # ensure those are registered first
 from . import mgmt_rules, archivetransfer, dataobject, archiveunit  # noqa
 
 
 # Add arbitrary score using `yes` to overtake e.g. afs for DataObjectReference defined in content
@@ -143,72 +144,21 @@
 class StartDateInlineEntityCreationFormView(autoform.InlineEntityCreationFormView):
     __select__ = (autoform.InlineEntityCreationFormView.__select__
                   & simplified_start_date())
     removejs = None
     form_renderer_id = 'notitle'
 
 
-# simplified profil will have a single appraisal/access rule, hence 'ignore inherited rules' is
-# enough, no need for explicit rule deactivation. This implies:
-# 1. hide explicit rule deactivation
-# 2. force appearance (hence choice) of the ignore all rules entity
-# 3. adapt alternative's title, so it doesn't appear like an alternative
-
-# 1. hide explicit rule deactivation
-simplified_afs.tag_object_of(('*', 'seda_ref_non_rule_id_from', '*'),
-                             'main', 'hidden')
-
-
-class AltInheritanceAutomaticEntityForm(autoform.AutomaticEntityForm):
-    __select__ = (is_instance('SEDAAltAccessRulePreventInheritance',
-                              'SEDAAltAppraisalRulePreventInheritance')
-                  & simplified_profile())
-
-    # 3. adapt alternative's title, so it doesn't appear like an alternative
-    def __init__(self, *args, **kwargs):
-        super(AltInheritanceAutomaticEntityForm, self).__init__(*args, **kwargs)
-        self.form_renderer_id = 'not-an-alt'
-
-    # 2. force appearance (hence choice) of the ignore all rules entity
-    def should_display_inline_creation_form(self, rschema, existing, card):
-        if not existing and rschema == 'seda_prevent_inheritance':
-            return True
-        return super(AltInheritanceAutomaticEntityForm, self).should_display_inline_creation_form(
-            rschema, existing, card)
-
-
-# 2. force appearance (hence choice) of the ignore all rules entity
-
-@objectify_predicate
-def simplified_prevent_inheritance(cls, req, rtype=None, pform=None, **kwargs):
-    if isinstance(pform, AltInheritanceAutomaticEntityForm) and rtype == 'seda_prevent_inheritance':
-        return 1
-    return 0
-
-
-class PreventInheritanceInlineEntityEditionFormView(autoform.InlineEntityEditionFormView):
-    __select__ = (autoform.InlineEntityEditionFormView.__select__
-                  & simplified_prevent_inheritance())
-    removejs = None
-
-
-class PreventInheritanceInlineEntityCreationFormView(autoform.InlineEntityCreationFormView):
-    __select__ = (autoform.InlineEntityCreationFormView.__select__
-                  & simplified_prevent_inheritance())
-    removejs = None
-
-
-class NotAnAltEntityInlinedFormRenderer(formrenderers.EntityInlinedFormRenderer):
-    """Custom form renderer that remove 'Alternative :' from an alternative's inlined form's title.
-    """
-    __regid__ = 'not-an-alt'
-
-    def render_title(self, w, form, values):
-        values['title'] = values['title'].split(':', 1)[1]
-        super(NotAnAltEntityInlinedFormRenderer, self).render_title(w, form, values)
+# simplified profil will have a single appraisal/access rule, hence we can remove all the
+# inheritance control mecanism: override will simply mean redefining a rule at some point in the
+# tree.
+for rule_type in RULE_TYPES:
+    etype = 'SEDA{0}Rule'.format(rule_type.capitalize())
+    rtype = 'seda_alt_{0}_rule_prevent_inheritance'.format(rule_type)
+    simplified_afs.tag_subject_of((etype, rtype, '*'), 'main', 'hidden')
 
 
 # SEDAArchiveTransfer customization
 for rtype, role in archivetransfer.at_ordered_fields:
     if not rtype.endswith('agency'):
         assert role == 'object'
         if rtype in ('seda_archival_agreement', 'seda_comment'):
```

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/views/archiveunit.py` & `cubicweb-seda-0.9.0/cubicweb_seda/views/archiveunit.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from six import text_type
 
 from logilab.mtconverter import xml_escape
 from logilab.common.registry import objectify_predicate
 from logilab.common.decorators import monkeypatch
 
 from cubicweb import tags, _
-from cubicweb.predicates import is_instance
+from cubicweb.predicates import is_instance, match_form_params, specified_etype_implements
 from cubicweb.view import EntityView
 from cubicweb.web.views import autoform, baseviews, tabs, uicfg
 
 from cubicweb_compound import views as compound
 from cubes.relationwidget import views as rwdg
 
 from ..xsd import un_camel_case
@@ -92,15 +92,15 @@
     'simple_keyword', or if given entity is not linked to a keyword reference.
     """
     try:
         # first check for unit_type specified in form params
         unit_type = req.form['keyword_type']
         return int(unit_type == 'simple_keyword')
     except KeyError:
-        if not entity.reverse_seda_keyword_reference_from:
+        if entity is not None and not entity.reverse_seda_keyword_reference_from:
             return 1
         return 0
 
 
 @objectify_predicate
 def typed_reference(cls, req, entity=None, **kwargs):
     """Return positive score for content's typed data object references (IsPartOf, VersionOf, etc.),
@@ -587,15 +587,18 @@
                 kwt_value = self._cw._('<no type specified>')
             msg = xml_escape(self._cw._('keyword type: {0}').format(kwt_value))
             self.w(u'<br/><span>{0} {1}</span>'.format(msg, kwt.view('seda.xsdmeta')))
 
 
 afs.tag_subject_of(('SEDAKeywordReference', 'seda_keyword_reference_to_scheme', '*'),
                    'main', 'attributes')
+affk.set_field_kwargs('SEDAKeywordReference', 'seda_keyword_reference_to_scheme',
+                      help=_('select a type to filter out unrelated vocabularies'))
 affk.set_field_kwargs('SEDAKeywordReference', 'seda_keyword_reference_to',
+                      help=_('select first a vocabulary then type here to prompt auto-completion'),
                       widget=widgets.ConceptAutoCompleteWidget(
                           slave_name='seda_keyword_reference_to',
                           master_name='seda_keyword_reference_to_scheme'))
 affk.set_fields_order('SEDAKeywordReference', ['user_cardinality',
                                                'seda_keyword_reference_to_scheme',
                                                'seda_keyword_reference_to'])
 
@@ -606,24 +609,48 @@
 kw_simple_afs = copy_rtag(afs, __name__,
                           is_instance('SEDAKeyword') & is_simple_keyword())
 kw_simple_afs.tag_attribute(('SEDAKeyword', 'keyword_content'), 'main', 'attributes')
 kw_simple_afs.tag_object_of(
     ('*', 'seda_keyword_reference_from', 'SEDAKeyword'),
     'main', 'hidden')
 # but one ordering is enough to rule them all
-affk.set_fields_order('SEDAKeyword', ['keyword_content', ('seda_keyword_reference_from', 'object')])
+affk.set_fields_order('SEDAKeyword', [('seda_keyword_type_from', 'object'),
+                                      'keyword_content',
+                                      ('seda_keyword_reference_from', 'object')])
+
+affk.set_field_kwargs('SEDAKeywordType', 'seda_keyword_type_to',
+                      widget=widgets.KeywordTypeMasterWidget(
+                          slave_base_name='seda_keyword_reference_to_scheme'))
 
 
 class ComplexKeywordAutomaticEntityForm(autoform.AutomaticEntityForm):
     __select__ = (is_instance('SEDAKeyword') & ~is_simple_keyword())
 
     def should_display_inline_creation_form(self, rschema, existing, card):
-        # 1. force creation of one appraisal/access rule
-        if rschema == 'seda_keyword_reference_from':
+        # force display of type and keyword
+        if not existing and rschema in ('seda_keyword_type_from', 'seda_keyword_reference_from'):
             return True
+        return False
+
+    def should_display_add_new_relation_link(self, rschema, existing, card):
+        return False
+
+
+class ComplexKeywordEditionFormView(autoform.InlineEntityEditionFormView):
+    __select__ = (autoform.InlineEntityEditionFormView.__select__
+                  & is_instance('SEDAKeywordType', 'SEDAKeywordReference')
+                  & ~is_simple_keyword())
+    removejs = None
+
+
+class ComplexKeywordCreationFormView(autoform.InlineEntityCreationFormView):
+    __select__ = (autoform.InlineEntityCreationFormView.__select__
+                  & specified_etype_implements('SEDAKeywordType', 'SEDAKeywordReference')
+                  & ~is_simple_keyword())
+    removejs = None
 
 
 # relations tab ################################################################
 
 class ArchiveUnitRelationsTab(ArchiveUnitContentTab):
     """Display content's relations about a full seda2  archive unit."""
 
@@ -1100,7 +1127,11 @@
     """Don't display any title nor remove link for DataObjectReference in the context of a
     simplified profile.
     """
 
     __select__ = (widgets.NoTitleEntityInlinedFormRenderer.__select__
                   & is_instance('SEDADataObjectReference')
                   & simplified_profile())
+
+
+copy_afs = copy_rtag(afs, __name__, afs.__select__ & match_form_params(vid='copy'))
+copy_afs.tag_subject_of(('*', 'seda_alt_archive_unit_archive_unit_ref_id', '*'), 'main', 'hidden')
```

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/views/archivetransfer.py` & `cubicweb-seda-0.9.0/cubicweb_seda/views/archivetransfer.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/views/uicfg.py` & `cubicweb-seda-0.9.0/cubicweb_seda/views/uicfg.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/views/clone.py` & `cubicweb-seda-0.9.0/cubicweb_seda/views/clone.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/views/viewlib.py` & `cubicweb-seda-0.9.0/cubicweb_seda/views/viewlib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/views/sedalib.py` & `cubicweb-seda-0.9.0/cubicweb_seda/views/sedalib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/views/dataobject.py` & `cubicweb-seda-0.9.0/cubicweb_seda/views/dataobject.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/views/__init__.py` & `cubicweb-seda-0.9.0/cubicweb_seda/views/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,19 @@
 afs.tag_subject_of(('*', 'container', '*'), 'main', 'hidden')
 afs.tag_object_of(('*', 'container', '*'), 'main', 'hidden')
 
 pvs.tag_subject_of(('*', 'scheme_relation_type', '*'), 'hidden')
 pvs.tag_subject_of(('*', 'scheme_entity_type', '*'), 'hidden')
 pvs.tag_object_of(('*', 'seda_keyword_reference_to_scheme', '*'), 'hidden')
 
+afs.tag_subject_of(('*', 'code_keyword_type', '*'), 'main', 'attributes')
+pvs.tag_subject_of(('*', 'code_keyword_type', '*'), 'attributes')
+afs.tag_object_of(('*', 'code_keyword_type', '*'), 'main', 'hidden')
+pvs.tag_object_of(('*', 'code_keyword_type', '*'), 'hidden')
+
 aff.tag_attribute(('*', 'user_cardinality'), SEDAMetaField)
 afs.tag_attribute(('*', 'user_annotation'), 'main', 'hidden')
 for etype in FIRST_LEVEL_ETYPES:
     aff.tag_attribute((etype, 'user_cardinality'), ff.StringField)
     afs.tag_attribute((etype, 'user_annotation'), 'main', 'attributes')
 
 
@@ -137,16 +142,15 @@
     """
     vreg = req.vreg
     eschema = vreg.schema.eschema(etype)
     if eschema.has_perm(req, 'add'):
         if klass is None:
             klass = 'icon-plus-circled pull-right'
         url = vreg['etypes'].etype_class(etype).cw_create_url(req, **urlparams)
-        return tags.a(msg, href=url, klass=klass,
-                      title=req.__('New %s' % etype))
+        return tags.a(msg, href=url, klass=klass)
     return u''
 
 
 def has_rel_perm(action, entity, rtype, role, target_etype=None, target_entity=None):
     """Return True if the user has the permission for `action` on the relation `rtype` where
     `entity` is `role`. Either target entity type or target entity could also be specified.
     """
```

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/views/mgmt_rules.py` & `cubicweb-seda-0.9.0/cubicweb_seda/views/mgmt_rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from six import text_type
 
 from logilab.mtconverter import xml_escape
 
 from cubicweb.predicates import is_instance
 from cubicweb.web import INTERNAL_FIELD_VALUE
-from cubicweb.web.views import uicfg
+from cubicweb.web.views import reledit, uicfg
 
 from ..entities import parent_and_container, rule_type_from_etype
 from . import viewlib
 from . import uicfg as sedauicfg  # noqa - ensure those rules are defined first
 
 
 affk = uicfg.autoform_field_kwargs
@@ -176,7 +176,22 @@
             #     XXX
             if reassessing_authorization.need_reassessing_authorization:
                 need_human = _('need human intervention')
             else:
                 need_human = _('without human intervention')
             self.w(u'<div>{0}</div>'.format(xml_escape(need_human)))
         super(ClassificationRuleComplexLinkEntityAttributeView, self).entity_call(entity)
+
+
+class MgmtRuleAutoClickAndEditFormView(reledit.AutoClickAndEditFormView):
+    __select__ = (reledit.AutoClickAndEditFormView.__select__
+                  & is_instance('SEDASeqAltArchiveUnitArchiveUnitRefIdManagement'))
+
+    def _compute_default_value(self, rschema, role):
+        if rschema.type.endswith('_rule'):
+            rule_type = rschema.type[len('seda_'):-len('_rule')]
+            rule = self.entity.inherited_rule(rule_type)
+            if rule:
+                return rule.view('seda.reledit.text') + u'<p><mark>{}</mark></p>'.format(
+                    self._cw._(u'inherited value'))
+        return super(MgmtRuleAutoClickAndEditFormView, self)._compute_default_value(
+            rschema, role)
```

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/views/widgets.py` & `cubicweb-seda-0.9.0/cubicweb_seda/views/widgets.py`

 * *Files 15% similar despite different names*

```diff
@@ -102,14 +102,45 @@
             # register the association between the value and the field, because on entity creation,
             # process_posted will be recalled on the newly created field, and if we don't do that it
             # won't find the proper value (this is very nasty)
             form.formvalues[(subfield, form)] = equivalent_eids
             yield (subfield, equivalent_eids)
 
 
+class KeywordTypeMasterWidget(fw.Select):
+    """
+    Usage::
+
+      affk = uicfg.autoform_field_kwargs
+      affk.set_field_kwargs('KeywordType', 'keyword_type_to',
+                            widget=widgets.KeywordTypeMasterWidget(
+                            slave_base_name='seda_keyword_reference_to_scheme'))
+    """
+
+    def __init__(self, slave_base_name, **kwargs):
+        super(KeywordTypeMasterWidget, self).__init__(**kwargs)
+        self.slave_base_name = slave_base_name
+
+    def _render(self, form, field, render):
+        req = form._cw
+
+        vocabularies_data = []
+        for eid, title, uri, keyword_type in req.execute(
+                'Any CS,CST,CSU,CSKT WHERE CS title CST, CS cwuri CSU, CS code_keyword_type CSKT?'):
+            vocabularies_data.append({'eid': eid, 'title': title or uri,
+                                      'keyword_type': keyword_type})
+        vocabularies_data.sort(key=lambda x: x['title'])
+
+        req.add_js(('cubicweb.js', 'cubicweb.ajax.js', 'cubes.skoscomplete.js'))
+        req.add_onload(js.typed_vocabularies.initKeywordTypeMasterWidget(
+            field.dom_id(form, self.suffix), self.slave_base_name, vocabularies_data))
+
+        return super(KeywordTypeMasterWidget, self)._render(form, field, render)
+
+
 class ConceptAutoCompleteWidget(fw.TextInput):
     """Derive from simple text input to create an autocompletion widget if a scheme is specified,
     otherwise free text is fine if `optional` argument is true. In such case:
 
     * `slave_name` is expected to be the name of the concept attribute, or the text attribute if
       optional is true),
```

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/views/sedatree.py` & `cubicweb-seda-0.9.0/cubicweb_seda/views/sedatree.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 from ..entities import simplified_profile, component_unit
 from . import jqtree
 
 
 class ProfileTreeComponent(component.EntityCtxComponent):
     """Display the whole profile tree."""
     __regid__ = 'seda.tree'
-    __select__ = component.EntityCtxComponent.__select__ & adaptable('ITreeBase')
+    __select__ = (component.EntityCtxComponent.__select__
+                  & adaptable('ITreeBase'))
     context = 'left'
     order = -1
     title = _('SEDA profile tree')
 
     def render_body(self, w):
         self._cw.add_css('cubes.jqtree.css')
         self.entity.view('jqtree.treeview', w=w)
```

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/views/facets.py` & `cubicweb-seda-0.9.0/cubicweb_seda/views/facets.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/site_cubicweb.py` & `cubicweb-seda-0.9.0/cubicweb_seda/site_cubicweb.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,17 @@
 @monkeypatch(rtags.RelationTags)
 def __init__(self, __module__=None):
     super(rtags.RelationTags, self).__init__()
     self._tagdefs = {}
 
 
 Entity.cw_skip_copy_for.append(('container', 'subject'))
+Entity.cw_skip_copy_for.append(('container', 'object'))
+Entity.cw_skip_copy_for.append(('clone_of', 'subject'))
+Entity.cw_skip_copy_for.append(('clone_of', 'object'))
 
 
 # auto-configuration of custom fields ##############################################################
 # (https://www.cubicweb.org/ticket/14474840)
 # other part in views/patches
 
 from cubicweb.web import formfields  # noqa
```

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/xsd/seda-2.0-ontology.xsd` & `cubicweb-seda-0.9.0/cubicweb_seda/xsd/seda-2.0-ontology.xsd`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/xsd/xlink.xsd` & `cubicweb-seda-0.9.0/cubicweb_seda/xsd/xlink.xsd`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/xsd/seda-2.0-main.xsd` & `cubicweb-seda-0.9.0/cubicweb_seda/xsd/seda-2.0-main.xsd`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/xsd/xml.xsd` & `cubicweb-seda-0.9.0/cubicweb_seda/xsd/xml.xsd`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/xsd/seda-2.0-descriptive.xsd` & `cubicweb-seda-0.9.0/cubicweb_seda/xsd/seda-2.0-descriptive.xsd`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/xsd/seda-2.0-management.xsd` & `cubicweb-seda-0.9.0/cubicweb_seda/xsd/seda-2.0-management.xsd`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/xsd/seda-2.0-technical.xsd` & `cubicweb-seda-0.9.0/cubicweb_seda/xsd/seda-2.0-technical.xsd`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/xsd/seda-2.0-types.xsd` & `cubicweb-seda-0.9.0/cubicweb_seda/xsd/seda-2.0-types.xsd`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/__pkginfo__.py` & `cubicweb-seda-0.9.0/cubicweb_seda/__pkginfo__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # pylint: disable=W0622
 """cubicweb-seda application packaging information"""
 
 modname = 'seda'
 distname = 'cubicweb-seda'
 
-numversion = (0, 8, 0)
+numversion = (0, 9, 0)
 version = '.'.join(str(num) for num in numversion)
 
 license = 'LGPL'
 author = 'LOGILAB S.A. (Paris, FRANCE)'
 author_email = 'contact@logilab.fr'
 description = 'Data Exchange Standard for Archival'
 web = 'http://www.cubicweb.org/project/%s' % distname
 
 __depends__ = {
     'cubicweb': '>= 3.24',
     'six': '>= 1.4.0',
     'cubicweb-eac': None,
     'cubicweb-skos': '>= 0.12.1',
-    'cubicweb-compound': '>= 0.4',
+    'cubicweb-compound': '>= 0.6',
     'cubicweb-relationwidget': '>= 0.4',
     'cubicweb-squareui': None,
     'pyxst': None,
     'rdflib': '>= 4.1',
 }
 __recommends__ = {}
```

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/__init__.py` & `cubicweb-seda-0.9.0/cubicweb_seda/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/i18n/fr.po` & `cubicweb-seda-0.9.0/cubicweb_seda/i18n/fr.po`

 * *Files 2% similar despite different names*

```diff
@@ -571,14 +571,17 @@
 
 msgid "SEDA 1.0 RNG export"
 msgstr "export SEDA 1.0 RNG"
 
 msgid "SEDA 2.0 RNG export"
 msgstr "export SEDA 2.0 RNG"
 
+msgid "SEDA code keyword type for this scheme"
+msgstr "Type SEDA des mot-clés de ce vocabulaire"
+
 msgid "SEDA profile tree"
 msgstr "arbre du profil SEDA"
 
 msgid "SEDAAccessRule"
 msgstr ""
 
 msgid "SEDAAccessRuleCodeListVersion"
@@ -1257,49 +1260,49 @@
 msgid "SEDAIsVersionOf"
 msgstr "version de"
 
 msgid "SEDAIsVersionOf_plural"
 msgstr ""
 
 msgid "SEDAJuridictional"
-msgstr "Juridiction administrative"
+msgstr "juridiction administrative"
 
 msgid "SEDAJuridictional_plural"
-msgstr "Juridictions administratives"
+msgstr "juridictions administratives"
 
 msgid "SEDAKeyword"
-msgstr "Descripteur"
+msgstr "descripteur"
 
 msgctxt ""
 "inlined:SEDASeqAltArchiveUnitArchiveUnitRefIdManagement.seda_keyword.object"
 msgid "SEDAKeyword"
 msgstr ""
 
 msgid "SEDAKeywordReference"
-msgstr "Descripteur"
+msgstr "descripteur"
 
 msgctxt "inlined:SEDAKeyword.seda_keyword_reference_from.object"
 msgid "SEDAKeywordReference"
 msgstr ""
 
 msgid "SEDAKeywordReference_plural"
-msgstr "Descripteurs"
+msgstr "descripteurs"
 
 msgid "SEDAKeywordType"
 msgstr "type"
 
 msgctxt "inlined:SEDAKeyword.seda_keyword_type_from.object"
 msgid "SEDAKeywordType"
 msgstr ""
 
 msgid "SEDAKeywordType_plural"
 msgstr ""
 
 msgid "SEDAKeyword_plural"
-msgstr "Descripteurs"
+msgstr "descripteurs"
 
 msgid "SEDALanguage"
 msgstr "langue"
 
 msgctxt ""
 "inlined:SEDASeqAltArchiveUnitArchiveUnitRefIdManagement.seda_language_from."
 "object"
@@ -3917,14 +3920,28 @@
 msgid "clone_of_object"
 msgstr ""
 
 msgctxt "SEDAArchiveUnit"
 msgid "clone_of_object"
 msgstr ""
 
+msgid "code_keyword_type"
+msgstr "type de mot-clés"
+
+msgctxt "ConceptScheme"
+msgid "code_keyword_type"
+msgstr ""
+
+msgid "code_keyword_type_object"
+msgstr ""
+
+msgctxt "Concept"
+msgid "code_keyword_type_object"
+msgstr ""
+
 msgctxt "SEDAComment"
 msgid "comment"
 msgstr "valeur"
 
 msgid "compat_list"
 msgstr "formats supportés"
 
@@ -4754,14 +4771,17 @@
 msgctxt "SEDAFormatLitteral"
 msgid "format_litteral"
 msgstr ""
 
 msgid "import_unit"
 msgstr "unité d'archive du référentiel"
 
+msgid "inherited value"
+msgstr "valeur héritée"
+
 msgid "juridictional"
 msgstr "juridication administrative"
 
 msgctxt "SEDAJuridictional"
 msgid "juridictional"
 msgstr ""
 
@@ -6479,15 +6499,15 @@
 msgstr ""
 
 msgctxt "SEDAKeyword"
 msgid "seda_keyword_type_from_object"
 msgstr ""
 
 msgid "seda_keyword_type_to"
-msgstr "type"
+msgstr "valeur"
 
 msgctxt "SEDAKeywordType"
 msgid "seda_keyword_type_to"
 msgstr ""
 
 msgid "seda_keyword_type_to_object"
 msgstr ""
@@ -7826,14 +7846,20 @@
 msgid "seda_writer_to_object"
 msgstr ""
 
 msgctxt "AuthorityRecord"
 msgid "seda_writer_to_object"
 msgstr ""
 
+msgid "select a type to filter out unrelated vocabularies"
+msgstr "sélectionnez un type pour filtrer les vocabulaires correspondants"
+
+msgid "select first a vocabulary then type here to prompt auto-completion"
+msgstr "sélectionnez un vocabulaire avant de taper dans ce champ pour activer la complétion automatique"
+
 msgid "service_level"
 msgstr "valeur"
 
 msgctxt "SEDAServiceLevel"
 msgid "service_level"
 msgstr ""
```

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/i18n/en.po` & `cubicweb-seda-0.9.0/cubicweb_seda/i18n/en.po`

 * *Files 0% similar despite different names*

```diff
@@ -561,14 +561,17 @@
 
 msgid "SEDA 1.0 RNG export"
 msgstr ""
 
 msgid "SEDA 2.0 RNG export"
 msgstr ""
 
+msgid "SEDA code keyword type for this scheme"
+msgstr ""
+
 msgid "SEDA profile tree"
 msgstr ""
 
 msgid "SEDAAccessRule"
 msgstr ""
 
 msgid "SEDAAccessRuleCodeListVersion"
@@ -3903,14 +3906,28 @@
 msgid "clone_of_object"
 msgstr ""
 
 msgctxt "SEDAArchiveUnit"
 msgid "clone_of_object"
 msgstr ""
 
+msgid "code_keyword_type"
+msgstr ""
+
+msgctxt "ConceptScheme"
+msgid "code_keyword_type"
+msgstr ""
+
+msgid "code_keyword_type_object"
+msgstr ""
+
+msgctxt "Concept"
+msgid "code_keyword_type_object"
+msgstr ""
+
 msgctxt "SEDAComment"
 msgid "comment"
 msgstr ""
 
 msgid "compat_list"
 msgstr ""
 
@@ -4735,14 +4752,17 @@
 msgctxt "SEDAFormatLitteral"
 msgid "format_litteral"
 msgstr ""
 
 msgid "import_unit"
 msgstr ""
 
+msgid "inherited value"
+msgstr ""
+
 msgid "juridictional"
 msgstr ""
 
 msgctxt "SEDAJuridictional"
 msgid "juridictional"
 msgstr ""
 
@@ -7805,14 +7825,20 @@
 msgid "seda_writer_to_object"
 msgstr ""
 
 msgctxt "AuthorityRecord"
 msgid "seda_writer_to_object"
 msgstr ""
 
+msgid "select a type to filter out unrelated vocabularies"
+msgstr ""
+
+msgid "select first a vocabulary then type here to prompt auto-completion"
+msgstr ""
+
 msgid "service_level"
 msgstr ""
 
 msgctxt "SEDAServiceLevel"
 msgid "service_level"
 msgstr ""
```

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/data/tree.jquery.js` & `cubicweb-seda-0.9.0/cubicweb_seda/data/tree.jquery.js`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/data/cubes.seda.css` & `cubicweb-seda-0.9.0/cubicweb_seda/data/cubes.seda.css`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/data/jqtree.css` & `cubicweb-seda-0.9.0/cubicweb_seda/data/jqtree.css`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/data/cubes.seda.js` & `cubicweb-seda-0.9.0/cubicweb_seda/data/cubes.seda.js`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/data/cubes.editionext.js` & `cubicweb-seda-0.9.0/cubicweb_seda/data/cubes.editionext.js`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/data/cubes.seda.form.js` & `cubicweb-seda-0.9.0/cubicweb_seda/data/cubes.seda.form.js`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/data/cubes.jqtree.js` & `cubicweb-seda-0.9.0/cubicweb_seda/data/cubes.jqtree.js`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/migration/0.8.0_Any.py` & `cubicweb-seda-0.9.0/cubicweb_seda/migration/0.8.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/migration/postcreate.py` & `cubicweb-seda-0.9.0/cubicweb_seda/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/migration/0.6.0_Any.py` & `cubicweb-seda-0.9.0/cubicweb_seda/migration/0.6.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/migration/data/languages.csv` & `cubicweb-seda-0.9.0/cubicweb_seda/migration/data/languages.csv`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/migration/data/level_type.csv` & `cubicweb-seda-0.9.0/cubicweb_seda/migration/data/level_type.csv`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/migration/data/mime_types.csv` & `cubicweb-seda-0.9.0/cubicweb_seda/migration/data/mime_types.csv`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/migration/data/dissemination.csv` & `cubicweb-seda-0.9.0/cubicweb_seda/migration/data/dissemination.csv`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/migration/data/encodings.csv` & `cubicweb-seda-0.9.0/cubicweb_seda/migration/data/encodings.csv`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/migration/data/document_type_code.csv` & `cubicweb-seda-0.9.0/cubicweb_seda/migration/data/document_type_code.csv`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/migration/data/digest_algorithms.csv` & `cubicweb-seda-0.9.0/cubicweb_seda/migration/data/digest_algorithms.csv`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/migration/data/file_formats.csv` & `cubicweb-seda-0.9.0/cubicweb_seda/migration/data/file_formats.csv`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/migration/data/access_control.csv` & `cubicweb-seda-0.9.0/cubicweb_seda/migration/data/access_control.csv`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda/xsd2entities.py` & `cubicweb-seda-0.9.0/cubicweb_seda/xsd2entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/tox.ini` & `cubicweb-seda-0.9.0/tox.ini`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda.egg-info/SOURCES.txt` & `cubicweb-seda-0.9.0/cubicweb_seda.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 cubicweb_seda/entities/profile_generation.py
 cubicweb_seda/i18n/en.po
 cubicweb_seda/i18n/fr.po
 cubicweb_seda/i18n/static-messages.pot
 cubicweb_seda/migration/0.5.1_Any.py
 cubicweb_seda/migration/0.6.0_Any.py
 cubicweb_seda/migration/0.8.0_Any.py
+cubicweb_seda/migration/0.9.0_Any.py
 cubicweb_seda/migration/postcreate.py
 cubicweb_seda/migration/data/access_control.csv
 cubicweb_seda/migration/data/classification_levels.csv
 cubicweb_seda/migration/data/code_keyword_type.csv
 cubicweb_seda/migration/data/digest_algorithms.csv
 cubicweb_seda/migration/data/dissemination.csv
 cubicweb_seda/migration/data/document_type_code.csv
```

### Comparing `cubicweb-seda-0.8.0/cubicweb_seda.egg-info/PKG-INFO` & `cubicweb-seda-0.9.0/cubicweb_seda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cubicweb-seda
-Version: 0.8.0
+Version: 0.9.0
 Summary: Data Exchange Standard for Archival
 Home-page: http://www.cubicweb.org/project/cubicweb-seda
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Description: Summary
         -------
```

### Comparing `cubicweb-seda-0.8.0/doc/profils.rst` & `cubicweb-seda-0.9.0/doc/profils.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/doc/conf.py` & `cubicweb-seda-0.9.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/PKG-INFO` & `cubicweb-seda-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cubicweb-seda
-Version: 0.8.0
+Version: 0.9.0
 Summary: Data Exchange Standard for Archival
 Home-page: http://www.cubicweb.org/project/cubicweb-seda
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Description: Summary
         -------
```

### Comparing `cubicweb-seda-0.8.0/test/test_html_generation.py` & `cubicweb-seda-0.9.0/test/test_html_generation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/test/pytestconf.py` & `cubicweb-seda-0.9.0/test/pytestconf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/test/test_diag.py` & `cubicweb-seda-0.9.0/test/test_diag.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/test/test_entities.py` & `cubicweb-seda-0.9.0/test/test_entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from logilab.common import attrdict
 
 from cubicweb.devtools.testlib import CubicWebTC
 
 from cubicweb_seda.entities import (seda_profile_container_def, simplified_profile,
                                     full_seda2_profile, parent_and_container,
-                                    rule_type_from_etype)
+                                    rule_type_from_etype, custom)
 
 from testutils import create_archive_unit, create_data_object
 
 
 def sort_container(container_def):
     for k, v in container_def:
         yield k, sorted(v)
@@ -130,18 +130,39 @@
 
             clone = cnx.create_entity('SEDAArchiveTransfer', title=u'Clone', clone_of=transfer)
             cnx.commit()
 
             self.assertEqual((clone.reverse_seda_message_digest_algorithm_code_list_version_from[0].
                              seda_message_digest_algorithm_code_list_version_to[0].eid),
                              scheme.eid)
-            seq = clone.archive_units[0]. first_level_choice.content_sequence
+            seq = clone.archive_units[0].first_level_choice.content_sequence
             self.assertEqual(seq.title.title, 'hello')
             self.assertEqual(transfer.binary_data_objects[0].seda_algorithm[0].eid, concept.eid)
 
+    def test_container_clone_clone(self):
+        """Functional test for SEDA component clone."""
+        with self.admin_access.repo_cnx() as cnx:
+            unit, unit_alt, unit_alt_seq = create_archive_unit(None, cnx=cnx)
+            cnx.commit()
+
+            cloned = cnx.create_entity(unit.cw_etype, user_annotation=u'x', clone_of=unit)
+            cnx.commit()
+            cloned.cw_clear_all_caches()
+
+            cloned2 = cnx.create_entity(unit.cw_etype, user_annotation=u'Y')
+            # mimick what's occurs when you're using the copy form
+            cloned2.copy_relations(cloned.eid)  # 1. copy relation
+            self.assertFalse(cloned2.clone_of)
+            cloned2.cw_set(clone_of=cloned.eid)  # 2. execute __linkto (which trigger cloning)
+
+            cnx.commit()
+
+            cloned2.cw_clear_all_caches()
+            self.assertEqual(len(cloned2.seda_alt_archive_unit_archive_unit_ref_id), 1)
+
 
 class FakeEntity(object):
     cw_etype = 'Whatever'
 
     def __init__(self, _cw):
         self._cw = _cw
 
@@ -273,10 +294,28 @@
 
     def test_title(self):
         with self.admin_access.client_cnx() as cnx:
             for etype in ('SEDAArchiveUnit', 'SEDABinaryDataObject', 'SEDAPhysicalDataObject'):
                 ent = cnx.create_entity(etype, user_annotation=u'bla bla\nbli bli blo\n')
                 self.assertEqual(ent.dc_title(), u'bla bla')
 
+    def test_climb_rule_holders(self):
+        with self.admin_access.client_cnx() as cnx:
+            transfer = cnx.create_entity('SEDAArchiveTransfer', title=u'test profile')
+            unit, _, unit_alt_seq = create_archive_unit(transfer)
+            subunit, _, subunit_alt_seq = create_archive_unit(unit_alt_seq)
+            cnx.commit()
+
+            self.assertEqual(list(custom._climb_rule_holders(subunit_alt_seq)),
+                             [subunit_alt_seq, unit_alt_seq, transfer])
+            self.assertEqual(list(custom._climb_rule_holders(subunit)),
+                             [subunit_alt_seq, unit_alt_seq, transfer])
+            self.assertEqual(list(custom._climb_rule_holders(unit_alt_seq)),
+                             [unit_alt_seq, transfer])
+            self.assertEqual(list(custom._climb_rule_holders(unit)),
+                             [unit_alt_seq, transfer])
+            self.assertEqual(list(custom._climb_rule_holders(transfer)),
+                             [transfer])
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cubicweb-seda-0.8.0/test/test_schema.py` & `cubicweb-seda-0.9.0/test/test_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -233,14 +233,29 @@
 
             for search in ('name', 'annotation', 'fixed'):
                 with self.subTest(search=search):
                     rset = cnx.execute('Any X WHERE X has_text %(search)s',
                                        {'search': search[::-1]})
                     self.assertEqual([r for r, in rset.rows], [transfer.eid])
 
+    def test_scheme_code_keyword_type_constraint(self):
+        with self.admin_access.repo_cnx() as cnx:
+            ckt_scheme = testutils.scheme_for_type(cnx, 'seda_keyword_type_to', None)
+            ckt_concept = ckt_scheme.add_concept(label=u'geoname')
+            scheme = testutils.scheme_for_type(cnx, 'seda_mime_type_to', None)
+            concept = scheme.add_concept(label=u'text/plain')
+            cnx.commit()
+
+            with self.assertRaises(ValidationError):
+                scheme.cw_set(code_keyword_type=concept)
+                cnx.commit()
+
+            scheme.cw_set(code_keyword_type=ckt_concept)
+            cnx.commit()
+
 
 class SecurityTC(CubicWebTC):
 
     @contextmanager
     def assertUnauthorized(self, cnx):
         with self.assertRaises(Unauthorized) as cm:
             yield cm
@@ -322,11 +337,33 @@
             with self.assertUnauthorized(cnx):
                 unit.cw_delete()
         with self.admin_access.repo_cnx() as cnx:
             unit = cnx.entity_from_eid(unit.eid)
             unit.cw_delete()
             cnx.commit()
 
+    def test_users_can_create_unit(self):
+        with self.admin_access.cnx() as cnx:
+            self.create_user(cnx, 'bob')
+        with self.new_access('bob').cnx() as cnx:
+            unit, unit_alt, unit_alt_seq = testutils.create_archive_unit(None, cnx=cnx)
+            cnx.commit()
+
+    def test_users_can_clone(self):
+        """Functional test for SEDA component clone."""
+        with self.admin_access.repo_cnx() as cnx:
+            self.create_user(cnx, login='alice')
+            unit, unit_alt, unit_alt_seq = testutils.create_archive_unit(None, cnx=cnx)
+            cnx.commit()
+
+        with self.new_access('alice').repo_cnx() as cnx:
+            unit = cnx.entity_from_eid(unit.eid)
+            cloned = cnx.create_entity(unit.cw_etype, user_annotation=u'x', clone_of=unit)
+            cnx.commit()
+            cloned.cw_clear_all_caches()
+
+            self.assertTrue(cloned.first_level_choice.content_sequence)
+
 
 if __name__ == '__main__':
     import unittest
     unittest.main()
```

### Comparing `cubicweb-seda-0.8.0/test/test_dataimport.py` & `cubicweb-seda-0.9.0/test/test_dataimport.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/test/testutils.py` & `cubicweb-seda-0.9.0/test/testutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/test/test_xsd2yams.py` & `cubicweb-seda-0.9.0/test/test_xsd2yams.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/test/test_hooks.py` & `cubicweb-seda-0.9.0/test/test_hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/test/test_views.py` & `cubicweb-seda-0.9.0/test/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,16 +382,14 @@
     def test_rule_form(self):
         with self.admin_access.web_request() as req:
             for rule_type in ('access', 'appraisal'):
                 form = self.create_and_link_form(req, 'SEDA{0}Rule'.format(rule_type.capitalize()))
                 self.assertInlinedFields(form, [
                     ('seda_seq_{0}_rule_rule'.format(rule_type),
                      'RuleRuleInlineEntityCreationFormView'),
-                    ('seda_alt_{0}_rule_prevent_inheritance'.format(rule_type),
-                     'InlineAddNewLinkView'),
                 ])
                 self.assertNoRemove(form, 'seda_seq_{0}_rule_rule'.format(rule_type), 'subject')
 
     def test_rule_rule_form(self):
         with self.admin_access.web_request() as req:
             for rule_type in ('access', 'appraisal'):
                 form = self.create_and_link_form(
@@ -401,25 +399,14 @@
                 self.assertNotIn('user_cardinality', other_fields)
                 self.assertInlinedFields(form, [
                     ('seda_start_date', 'StartDateInlineEntityCreationFormView'),
                 ])
                 self.assertNoRemove(form, 'seda_start_date', 'object')
                 self.assertNoTitle(form, 'seda_start_date', 'object')
 
-    def test_prevent_inheritance_form(self):
-        with self.admin_access.web_request() as req:
-            for rule_type in ('access', 'appraisal'):
-                form = self.create_and_link_form(req, 'SEDAAlt{0}RulePreventInheritance'.format(
-                    rule_type.capitalize()))
-                self.assertInlinedFields(form, [
-                    ('seda_prevent_inheritance', 'PreventInheritanceInlineEntityCreationFormView'),
-                ])
-                self.assertNoRemove(form, 'seda_prevent_inheritance', 'object')
-                self.assertEqual(form.form_renderer_id, 'not-an-alt')
-
     def test_create_data_object_full(self):
         with self.admin_access.web_request() as req:
             req.entity_from_eid(self.transfer_eid).cw_set(simplified_profile=False)
             req.cnx.commit()
             form = self.create_inlined_form(req, 'SEDADataObjectReference', formtype='inlined')
             self.assertEqual(entity_fields(form.fields),
                              ['seda_data_object_reference_id'])
```

### Comparing `cubicweb-seda-0.8.0/test/data/BV2.0_min.xml` & `cubicweb-seda-0.9.0/test/data/BV2.0_min.xml`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/test/data/exArchiveTransfer1_SEDA2_min.xml` & `cubicweb-seda-0.9.0/test/data/exArchiveTransfer1_SEDA2_min.xml`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/test/data/seda_1_export.rng` & `cubicweb-seda-0.9.0/test/data/seda_1_export.rng`

 * *Files 0% similar despite different names*

#### Comparing `cubicweb-seda-0.8.0/test/data/seda_1_export.rng` & `cubicweb-seda-0.9.0/test/data/seda_1_export.rng`

```diff
@@ -539,14 +539,22 @@
                   <rng:value type="string">6</rng:value>
                 </rng:attribute>
                 <rng:attribute name="filename">
                   <rng:value type="string">this_is_the_filename.pdf</rng:value>
                 </rng:attribute>
                 <rng:data type="string"/>
               </rng:element>
+              <rng:optional>
+                <rng:element name="Integrity">
+                  <rng:attribute name="algorithme">
+                    <rng:value type="string">md5</rng:value>
+                  </rng:attribute>
+                  <rng:data type="string"/>
+                </rng:element>
+              </rng:optional>
               <rng:element name="Type">
                 <rng:attribute name="listVersionID">
                   <rng:value type="token">edition 2009</rng:value>
                 </rng:attribute>
                 <rng:value type="string">CDO</rng:value>
               </rng:element>
             </rng:element>
```

### Comparing `cubicweb-seda-0.8.0/test/data/relaxng.rng` & `cubicweb-seda-0.9.0/test/data/relaxng.rng`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/test/data/exArchiveTransfert2_SEDA2_min.xml` & `cubicweb-seda-0.9.0/test/data/exArchiveTransfert2_SEDA2_min.xml`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/test/data/seda_02_export.rng` & `cubicweb-seda-0.9.0/test/data/seda_02_export.rng`

 * *Files 1% similar despite different names*

#### Comparing `cubicweb-seda-0.8.0/test/data/seda_02_export.rng` & `cubicweb-seda-0.9.0/test/data/seda_02_export.rng`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<rng:grammar xmlns:rng="http://relaxng.org/ns/structure/1.0" xmlns:clmIANACharacterSetCode="urn:un:unece:uncefact:codelist:standard:IANA:CharacterSetCode:2007-05-14" xmlns:udt="urn:un:unece:uncefact:data:standard:UnqualifiedDataType:10" xmlns:clmDAFFileTypeCode="urn:un:unece:uncefact:codelist:draft:DAF:fileTypeCode:2009-08-18" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:qdt="fr:gouv:culture:archivesdefrance:seda:v1.0:QualifiedDataType:1" xmlns:clmIANAMIMEMediaType="urn:un:unece:uncefact:codelist:standard:IANA:MIMEMediaType:2008-11-12" xmlns:clm60133="urn:un:unece:uncefact:codelist:standard:6:0133:40106" xmlns="fr:gouv:culture:archivesdefrance:seda:v1.0" datatypeLibrary="http://www.w3.org/2001/XMLSchema-datatypes" ns="fr:gouv:ae:archive:draft:standard_echange_v0.2">
+<rng:grammar xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0" xmlns:clmDAFFileTypeCode="urn:un:unece:uncefact:codelist:draft:DAF:fileTypeCode:2009-08-18" xmlns:clmIANACharacterSetCode="urn:un:unece:uncefact:codelist:standard:IANA:CharacterSetCode:2007-05-14" xmlns:clmIANAMIMEMediaType="urn:un:unece:uncefact:codelist:standard:IANA:MIMEMediaType:2008-11-12" xmlns:clm60133="urn:un:unece:uncefact:codelist:standard:6:0133:40106" xmlns:qdt="fr:gouv:culture:archivesdefrance:seda:v1.0:QualifiedDataType:1" xmlns:rng="http://relaxng.org/ns/structure/1.0" xmlns:seda="fr:gouv:culture:archivesdefrance:seda:v2.0" xmlns:udt="urn:un:unece:uncefact:data:standard:UnqualifiedDataType:10" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="fr:gouv:culture:archivesdefrance:seda:v1.0" datatypeLibrary="http://www.w3.org/2001/XMLSchema-datatypes" ns="fr:gouv:ae:archive:draft:standard_echange_v0.2">
   <rng:start>
     <rng:element name="ArchiveTransfer">
       <xsd:annotation>
         <xsd:documentation>my profile title &amp;&amp;</xsd:documentation>
       </xsd:annotation>
       <rng:optional>
         <rng:attribute name="Id">
@@ -130,14 +130,27 @@
         </rng:element>
         <rng:optional>
           <rng:element name="Name">
             <rng:data type="string"/>
           </rng:element>
         </rng:optional>
       </rng:element>
+      <rng:optional>
+        <rng:element name="Integrity">
+          <rng:element name="Contains">
+            <rng:attribute name="algorithme">
+              <rng:value type="string">md5</rng:value>
+            </rng:attribute>
+            <rng:data type="string"/>
+          </rng:element>
+          <rng:element name="UnitIdentifier" a:defaultValue="id%(bdo-eid)s">
+            <rng:data type="string"/>
+          </rng:element>
+        </rng:element>
+      </rng:optional>
       <rng:oneOrMore>
         <rng:element name="Contains">
           <xsd:annotation>
             <xsd:documentation>archive unit title</xsd:documentation>
           </xsd:annotation>
           <rng:optional>
             <rng:attribute name="Id">
@@ -478,15 +491,15 @@
                 <rng:element name="StartDate">
                   <rng:data type="string"/>
                 </rng:element>
               </rng:element>
             </rng:element>
           </rng:oneOrMore>
           <rng:zeroOrMore>
-            <rng:element name="Document">
+            <rng:element name="Document" seda:profid="id%(bdo-eid)s">
               <xsd:annotation>
                 <xsd:documentation>data object title</xsd:documentation>
               </xsd:annotation>
               <rng:optional>
                 <rng:attribute name="Id">
                   <rng:data type="ID"/>
                 </rng:attribute>
```

### Comparing `cubicweb-seda-0.8.0/test/data/seda_1_export.xsd` & `cubicweb-seda-0.9.0/test/data/seda_1_export.xsd`

 * *Files 1% similar despite different names*

#### Comparing `cubicweb-seda-0.8.0/test/data/seda_1_export.xsd` & `cubicweb-seda-0.9.0/test/data/seda_1_export.xsd`

```diff
@@ -435,14 +435,23 @@
                             <xsd:attribute fixed="this_is_the_filename.pdf" name="filename" type="xsd:string" use="required"/>
                             <xsd:attribute name="characterSetCode" type="clmIANACharacterSetCode:CharacterSetCodeContentType" use="prohibited"/>
                             <xsd:attribute name="uri" type="xsd:anyURI" use="prohibited"/>
                           </xsd:extension>
                         </xsd:simpleContent>
                       </xsd:complexType>
                     </xsd:element>
+                    <xsd:element minOccurs="0" name="Integrity">
+                      <xsd:complexType>
+                        <xsd:simpleContent>
+                          <xsd:extension base="qdt:ArchivesHashcodeBinaryObjectType">
+                            <xsd:attribute fixed="md5" name="algorithme" type="xsd:string" use="required"/>
+                          </xsd:extension>
+                        </xsd:simpleContent>
+                      </xsd:complexType>
+                    </xsd:element>
                     <xsd:element fixed="CDO" name="Type">
                       <xsd:complexType>
                         <xsd:simpleContent>
                           <xsd:extension base="qdt:CodeDocumentType">
                             <xsd:attribute fixed="edition 2009" name="listVersionID" type="xsd:token" use="required"/>
                           </xsd:extension>
                         </xsd:simpleContent>
```

### Comparing `cubicweb-seda-0.8.0/test/data/seda_02_export.xsd` & `cubicweb-seda-0.9.0/test/data/seda_02_export.xsd`

 * *Files 2% similar despite different names*

#### Comparing `cubicweb-seda-0.8.0/test/data/seda_02_export.xsd` & `cubicweb-seda-0.9.0/test/data/seda_02_export.xsd`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<xsd:schema xmlns:udt="urn:un:unece:uncefact:data:standard:UnqualifiedDataType:6" xmlns:qdt="fr:gouv:ae:archive:draft:standard_echange_v0.2:QualifiedDataType:1" xmlns:clm60133="urn:un:unece:uncefact:codelist:standard:6:0133:40106" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:clmIANACharacterSetCode="urn:un:unece:uncefact:codelist:standard:IANA:CharacterSetCode:2007-05-14" xmlns:clmDAFFileTypeCode="urn:un:unece:uncefact:codelist:draft:DAF:fileTypeCode:2009-08-18" xmlns:clmIANAMIMEMediaType="urn:un:unece:uncefact:codelist:standard:IANA:MIMEMediaType:2008-11-12" xmlns="fr:gouv:ae:archive:draft:standard_echange_v0.2" attributeFormDefault="unqualified" elementFormDefault="qualified" targetNamespace="fr:gouv:ae:archive:draft:standard_echange_v0.2" version="1.1">
+<xsd:schema xmlns:a="http://relaxng.org/ns/compatibility/annotations/1.0" xmlns:clmDAFFileTypeCode="urn:un:unece:uncefact:codelist:draft:DAF:fileTypeCode:2009-08-18" xmlns:clmIANACharacterSetCode="urn:un:unece:uncefact:codelist:standard:IANA:CharacterSetCode:2007-05-14" xmlns:clmIANAMIMEMediaType="urn:un:unece:uncefact:codelist:standard:IANA:MIMEMediaType:2008-11-12" xmlns:clm60133="urn:un:unece:uncefact:codelist:standard:6:0133:40106" xmlns:qdt="fr:gouv:culture:archivesdefrance:seda:v1.0:QualifiedDataType:1" xmlns:rng="http://relaxng.org/ns/structure/1.0" xmlns:seda="fr:gouv:culture:archivesdefrance:seda:v2.0" xmlns:udt="urn:un:unece:uncefact:data:standard:UnqualifiedDataType:10" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="fr:gouv:culture:archivesdefrance:seda:v1.0" attributeFormDefault="unqualified" elementFormDefault="qualified" targetNamespace="fr:gouv:ae:archive:draft:standard_echange_v0.2" version="1.1">
   <xsd:element name="ArchiveTransfer">
     <xsd:annotation>
       <xsd:documentation>my profile title &amp;&amp;</xsd:documentation>
     </xsd:annotation>
     <xsd:complexType>
       <xsd:sequence>
         <xsd:element fixed="my profile description &amp;&amp;" name="Comment">
@@ -68,14 +68,30 @@
                   </xsd:simpleContent>
                 </xsd:complexType>
               </xsd:element>
               <xsd:element minOccurs="0" name="Name" type="udt:TextType"/>
             </xsd:sequence>
           </xsd:complexType>
         </xsd:element>
+        <xsd:element minOccurs="0" name="Integrity">
+          <xsd:complexType>
+            <xsd:sequence>
+              <xsd:element name="Contains">
+                <xsd:complexType>
+                  <xsd:simpleContent>
+                    <xsd:extension base="qdt:ArchivesHashcodeBinaryObjectType">
+                      <xsd:attribute fixed="md5" name="algorithme" type="xsd:string" use="required"/>
+                    </xsd:extension>
+                  </xsd:simpleContent>
+                </xsd:complexType>
+              </xsd:element>
+              <xsd:element default="id%(bdo-eid)s" name="UnitIdentifier" type="qdt:ArchivesIDType"/>
+            </xsd:sequence>
+          </xsd:complexType>
+        </xsd:element>
         <xsd:element maxOccurs="unbounded" name="Contains">
           <xsd:annotation>
             <xsd:documentation>archive unit title</xsd:documentation>
           </xsd:annotation>
           <xsd:complexType>
             <xsd:sequence>
               <xsd:element fixed="fr" name="DescriptionLanguage">
@@ -375,15 +391,15 @@
                         <xsd:attribute name="Id" type="xsd:ID" use="optional"/>
                       </xsd:complexType>
                     </xsd:element>
                   </xsd:sequence>
                   <xsd:attribute name="Id" type="xsd:ID" use="optional"/>
                 </xsd:complexType>
               </xsd:element>
-              <xsd:element maxOccurs="unbounded" minOccurs="0" name="Document">
+              <xsd:element maxOccurs="unbounded" minOccurs="0" name="Document" seda:profid="id%(bdo-eid)s">
                 <xsd:annotation>
                   <xsd:documentation>data object title</xsd:documentation>
                 </xsd:annotation>
                 <xsd:complexType>
                   <xsd:sequence>
                     <xsd:element name="Attachment">
                       <xsd:complexType>
```

### Comparing `cubicweb-seda-0.8.0/test/data/XMLSchema.xsd` & `cubicweb-seda-0.9.0/test/data/XMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/test/data/seda_02_bordereau_ref.xml` & `cubicweb-seda-0.9.0/test/data/seda_02_bordereau_ref.xml`

 * *Files identical despite different names*

### Comparing `cubicweb-seda-0.8.0/test/test_profile_generation.py` & `cubicweb-seda-0.9.0/test/test_profile_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -721,14 +721,15 @@
 
             concepts = {}
             for rtype, etype, value in [
                     ('seda_format_id_to', None, u'fmt/123'),
                     ('seda_encoding_to', None, u'6'),
                     ('seda_type_to', None, u'CDO'),
                     ('seda_description_level', None, u'file'),
+                    ('seda_algorithm', 'SEDABinaryDataObject', u'md5'),
                     ('seda_rule', 'SEDASeqAppraisalRuleRule', u'P10Y'),
                     ('seda_rule', 'SEDASeqAccessRuleRule', u'AR038'),
                     ('seda_final_action', 'SEDAAppraisalRule', u'detruire'),
             ]:
                 scheme = testutils.scheme_for_type(cnx, rtype, etype, value)
                 concepts[value] = scheme.reverse_in_scheme[0]
 
@@ -804,14 +805,15 @@
                                                     reverse_seda_start_date=create('SEDAStartDate'),
                                                     seda_rule=concepts['AR038']))
 
             # Add minimal document to first level archive
             ref = create('SEDADataObjectReference', seda_data_object_reference=unit_alt_seq)
             bdo = testutils.create_data_object(transfer, user_cardinality=u'0..n',
                                                filename=u'this_is_the_filename.pdf',
+                                               seda_algorithm=concepts['md5'],
                                                reverse_seda_data_object_reference_id=ref)
 
             create('SEDAFormatId',
                    user_cardinality=u'1',
                    seda_format_id_from=bdo,
                    seda_format_id_to=concepts['fmt/123'])
             create('SEDAEncoding',
@@ -822,14 +824,15 @@
             # Add another sub archive unit
             _, _, subunit2_alt_seq = testutils.create_archive_unit(unit_alt_seq,
                                                                    user_cardinality=u'1..n')
 
             cnx.commit()
 
         self.transfer_eid = transfer.eid
+        self.bdo_eid = bdo.eid
         self.file_concept_eid = concepts['file'].eid
         self.agent_eid = agent.eid
 
     def _test_profile(self, adapter_id, expected_file):
         with self.admin_access.client_cnx() as cnx:
             transfer = cnx.entity_from_eid(self.transfer_eid)
             file_concept = cnx.entity_from_eid(self.file_concept_eid)
@@ -849,15 +852,16 @@
                     stream.write(orig_content)
                 print('Regenerated expected file as {}.new'.format(expected_file))
 
             root = etree.fromstring(generated_xsd)
             self.assertXmlValid(root)
             with open(self.datapath(expected_file)) as expected:
                 self.assertXmlEqual(expected.read()
-                                    % {'concept-uri': binary_type(file_concept.cwuri),
+                                    % {'bdo-eid': binary_type(self.bdo_eid),
+                                       'concept-uri': binary_type(file_concept.cwuri),
                                        'scheme-uri': binary_type(file_concept.scheme.cwuri),
                                        'agent-id': binary_type(agent.eid),
                                        'agent-name': binary_type(agent.dc_title())},
                                     generated_xsd)
             return adapter, root
```

### Comparing `cubicweb-seda-0.8.0/setup.py` & `cubicweb-seda-0.9.0/setup.py`

 * *Files identical despite different names*

