# Comparing `tmp/gocli-0.9.8.tar.gz` & `tmp/gocli-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gocli-0.9.8.tar", last modified: Thu Jun 25 21:39:18 2020, max compression
+gzip compressed data, was "dist/gocli-0.9.9.tar", last modified: Thu Jul 30 17:35:15 2020, max compression
```

## Comparing `gocli-0.9.8.tar` & `gocli-0.9.9.tar`

### file list

```diff
@@ -1,480 +1,480 @@
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/
--rw-r--r--   0 ianmaurer   (501) staff       (20)       54 2018-11-27 16:45:15.000000 gocli-0.9.8/MANIFEST.in
--rw-r--r--   0 ianmaurer   (501) staff       (20)     6278 2020-06-25 21:39:18.000000 gocli-0.9.8/PKG-INFO
--rw-r--r--   0 ianmaurer   (501) staff       (20)       38 2020-06-25 21:39:18.000000 gocli-0.9.8/setup.cfg
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2427 2020-06-25 21:38:51.000000 gocli-0.9.8/setup.py
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/genomoncology/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      492 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/__init__.py
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/genomoncology/cli/
--rw-r--r--   0 ianmaurer   (501) staff       (20)       68 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/cli/__init__.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)    19003 2020-06-25 21:38:55.000000 gocli-0.9.8/src/genomoncology/cli/commands.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      220 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/cli/const.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     5311 2020-04-28 15:25:56.000000 gocli-0.9.8/src/genomoncology/cli/options.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1188 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/cli/types.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      471 2020-03-31 13:12:57.000000 gocli-0.9.8/src/genomoncology/cli/utils.py
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/genomoncology/kms/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      314 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/kms/__init__.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)    11235 2020-06-25 21:38:17.000000 gocli-0.9.8/src/genomoncology/kms/annotations.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1040 2019-01-28 21:29:34.000000 gocli-0.9.8/src/genomoncology/kms/contents.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1534 2020-05-11 19:37:09.000000 gocli-0.9.8/src/genomoncology/kms/factory.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1255 2019-04-01 14:50:29.000000 gocli-0.9.8/src/genomoncology/kms/genes.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      917 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/kms/match.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1152 2019-01-28 21:29:34.000000 gocli-0.9.8/src/genomoncology/kms/therapies.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      470 2020-04-28 15:25:56.000000 gocli-0.9.8/src/genomoncology/kms/transcripts.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1172 2019-01-28 21:29:34.000000 gocli-0.9.8/src/genomoncology/kms/trials.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      109 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/main.py
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/genomoncology/parse/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      395 2019-04-26 14:24:33.000000 gocli-0.9.8/src/genomoncology/parse/__init__.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     4896 2020-04-28 15:25:56.000000 gocli-0.9.8/src/genomoncology/parse/doctypes.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      595 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/parse/ensures.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      326 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/parse/fieldtypes.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     3497 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/parse/fusions.py
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/genomoncology/pipeline/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      212 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/__init__.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1987 2019-01-30 20:00:19.000000 gocli-0.9.8/src/genomoncology/pipeline/comparators.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2221 2019-04-01 14:50:29.000000 gocli-0.9.8/src/genomoncology/pipeline/converters.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1824 2020-06-25 21:38:17.000000 gocli-0.9.8/src/genomoncology/pipeline/filters.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1733 2019-01-28 21:30:41.000000 gocli-0.9.8/src/genomoncology/pipeline/runner.py
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/genomoncology/pipeline/sinks/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      643 2020-05-11 19:37:09.000000 gocli-0.9.8/src/genomoncology/pipeline/sinks/__init__.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      687 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/sinks/alterations.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2520 2020-04-28 15:25:56.000000 gocli-0.9.8/src/genomoncology/pipeline/sinks/annotations.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1353 2019-04-01 14:50:29.000000 gocli-0.9.8/src/genomoncology/pipeline/sinks/base.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2132 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/sinks/excel.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      995 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/sinks/tsv.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)    11150 2020-06-25 21:38:17.000000 gocli-0.9.8/src/genomoncology/pipeline/sinks/vcf.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2130 2019-04-01 14:50:29.000000 gocli-0.9.8/src/genomoncology/pipeline/sinks/warehouse.py
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      847 2020-06-25 21:38:17.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/__init__.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     9922 2020-05-11 19:37:09.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/aggregated.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      481 2020-06-25 21:38:17.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/annotations_filter.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1234 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/base.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      641 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/bed.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      107 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/const.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2391 2019-08-22 14:04:53.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/delimited.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      850 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/excel.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1992 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/maf.py
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/one_off_sources/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      322 2020-03-31 13:12:57.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/one_off_sources/__init__.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)    14722 2020-05-11 19:37:09.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/one_off_sources/clinvar_xml.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)    14366 2020-04-28 15:25:56.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/one_off_sources/mitomap.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     4859 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/one_off_sources/uniprot.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2732 2019-04-26 14:24:33.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/paths.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     3049 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/smart_lazy_file.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1033 2020-03-31 13:12:57.000000 gocli-0.9.8/src/genomoncology/pipeline/sources/xml.py
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      638 2020-03-31 13:12:50.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/__init__.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     3537 2020-03-31 13:12:50.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/functions.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     4603 2019-01-30 20:00:19.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/mapper_classes.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2236 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/registry.py
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      752 2020-04-28 15:25:56.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/__init__.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1398 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/baylor_decipher.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      694 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/baylor_wgl.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2197 2019-04-26 14:24:33.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/clinvar.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2139 2020-03-31 13:12:57.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/clinvar_xml.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2629 2020-05-11 19:37:09.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/cosmic.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     8034 2020-03-31 13:12:50.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/dbnsfp.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     3514 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/dbsnp.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1398 2019-02-26 14:04:24.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/evs.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2188 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/exac.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1482 2020-03-31 13:12:50.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/gene_type.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      993 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/genie_maf.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     4386 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/gnomad.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2050 2020-03-31 13:12:57.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/hgmd.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      885 2020-04-28 15:25:56.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/hgmd_gene_list.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      905 2020-03-31 13:12:50.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/hpo.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1001 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/markers.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1118 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/mitomap.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     4400 2020-05-11 19:37:09.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/omim.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1045 2020-04-28 15:25:56.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/pli.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1155 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/splicing.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1082 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/thousandgenomes.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1049 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/uniprot.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      943 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/uniprot_domains.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      855 2018-11-27 16:45:15.000000 gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/uniprot_protein_name.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1882 2020-04-28 15:25:56.000000 gocli-0.9.8/src/genomoncology/state.py
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gocli.egg-info/
--rw-r--r--   0 ianmaurer   (501) staff       (20)     6278 2020-06-25 21:39:15.000000 gocli-0.9.8/src/gocli.egg-info/PKG-INFO
--rw-r--r--   0 ianmaurer   (501) staff       (20)    17097 2020-06-25 21:39:15.000000 gocli-0.9.8/src/gocli.egg-info/SOURCES.txt
--rw-r--r--   0 ianmaurer   (501) staff       (20)        1 2020-06-25 21:39:15.000000 gocli-0.9.8/src/gocli.egg-info/dependency_links.txt
--rw-r--r--   0 ianmaurer   (501) staff       (20)       51 2020-06-25 21:39:15.000000 gocli-0.9.8/src/gocli.egg-info/entry_points.txt
--rw-r--r--   0 ianmaurer   (501) staff       (20)      221 2020-06-25 21:39:15.000000 gocli-0.9.8/src/gocli.egg-info/requires.txt
--rw-r--r--   0 ianmaurer   (501) staff       (20)       26 2020-06-25 21:39:15.000000 gocli-0.9.8/src/gocli.egg-info/top_level.txt
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      490 2019-04-11 23:07:34.000000 gocli-0.9.8/src/gosdk/__init__.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     4284 2020-04-28 15:25:56.000000 gocli-0.9.8/src/gosdk/construct.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1519 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/logger.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      613 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/models.py
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/definitions/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      532 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Alteration.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      200 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/AlterationList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1138 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/AlterationsDocument.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      216 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/AlterationsDocumentList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1999 2020-06-25 21:38:17.000000 gocli-0.9.8/src/gosdk/specs/definitions/Annotation.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      105 2019-01-28 21:30:41.000000 gocli-0.9.8/src/gosdk/specs/definitions/AnnotationBundleVersion.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      234 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/AnnotationList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      940 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/AnnotationsDocument.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      169 2019-04-01 14:50:29.000000 gocli-0.9.8/src/gosdk/specs/definitions/AnnotationsDocumentAndNotFoundList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      216 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/AnnotationsDocumentList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2161 2019-01-28 21:30:41.000000 gocli-0.9.8/src/gosdk/specs/definitions/Annotations_MergedDocument.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      230 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Annotations_MergedDocumentList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)       67 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Arguments.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      208 2020-02-05 20:13:21.000000 gocli-0.9.8/src/gosdk/specs/definitions/Assay.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      165 2020-02-05 20:13:21.000000 gocli-0.9.8/src/gosdk/specs/definitions/AssayList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1814 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Case.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      186 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/CaseList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1601 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/CasesDocument.yaml
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)      204 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/CasesDocumentList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      335 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Classification.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1605 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/ClassificationsDocument.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      224 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/ClassificationsDocumentList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      287 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Content.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1244 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/ContentsDocument.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      210 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/ContentsDocumentList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      110 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Counts.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      244 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/CountsList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      223 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DetectedAlteration.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      211 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Document.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      247 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugBase.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      377 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugClassification.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      227 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugCondition.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      887 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugData.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)       99 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugExternalLink.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)       94 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugFdaLabel.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      302 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugGFInclude.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      203 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugGFIncludeComponent.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      307 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugGeneralReferences.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      132 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugGeneticFactors.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      105 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugGoClass.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      165 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugIngredient.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      107 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugIngredientStrength.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)       70 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugLabeller.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      134 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugLiteratureReference.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      145 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugModificationOf.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)       97 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugPfam.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      535 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugPharmacology.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1520 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugPolypeptide.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      702 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugProduct.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      103 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugSeverity.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      377 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugStructuredIndications.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      101 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugSynonym.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      359 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugTarget.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      103 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/DrugWithDrugs.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      355 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/EligibilitiesAsCurated.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      434 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Eligibility.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)       88 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Error.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      469 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Evidence.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      128 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Facets.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      678 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Gene.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      168 2019-04-01 14:50:29.000000 gocli-0.9.8/src/gosdk/specs/definitions/GeneBoundaries.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      200 2019-01-30 20:00:19.000000 gocli-0.9.8/src/gosdk/specs/definitions/GeneBoundariesList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      191 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/GenesList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      137 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/HgvsGMetadata.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      837 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/LabResult.yaml
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)      384 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/LabResultAttachmentFile.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      401 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/LabResultDataFile.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      165 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/LabResultDataFileList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      318 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Location.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      221 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/LogicSet.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      929 2020-02-05 20:13:21.000000 gocli-0.9.8/src/gosdk/specs/definitions/Marker.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      166 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/MarkerList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      178 2020-03-31 13:12:57.000000 gocli-0.9.8/src/gosdk/specs/definitions/MarkerMetaData.yaml
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)     1210 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/MarkersDocument.yaml
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)      208 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/MarkersDocumentList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      126 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/MatchedDisease.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)       90 2020-04-28 15:25:56.000000 gocli-0.9.8/src/gosdk/specs/definitions/Meeting.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      192 2020-04-28 15:25:56.000000 gocli-0.9.8/src/gosdk/specs/definitions/MeetingList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      124 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/NDGenes.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)       50 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewAlteration.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      255 2020-02-05 20:13:21.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewAssay.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1186 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewCase.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      820 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewClassification.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      802 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewContent.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      851 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewDocument.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      297 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewLabResult.yaml
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)      323 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewLabResultAttachmentFile.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      386 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewLabResultDataFile.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      874 2020-02-05 20:13:21.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewMarker.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      324 2020-04-28 15:25:56.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewOncologicTreatment.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      328 2020-02-05 20:13:21.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewPanel.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      719 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewPatient.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      275 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewPatientDiagnosis.yaml
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)      419 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewPatientMetaData.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2375 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewRecommendation.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      120 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewRecommendationsReport.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      218 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewReferenceAttachment.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      379 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewSample.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)       92 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/NewSelectedMarker.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)       88 2019-04-01 14:50:29.000000 gocli-0.9.8/src/gosdk/specs/definitions/NormalizedHGVS.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      155 2019-04-01 14:50:29.000000 gocli-0.9.8/src/gosdk/specs/definitions/NormalizedHGVSList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      124 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/OutOnlyGenesOffPanel.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)       50 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/OutcomeCohorts.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      228 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/OverallContact.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      368 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Pagination.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      160 2020-02-05 20:13:21.000000 gocli-0.9.8/src/gosdk/specs/definitions/Panel.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      165 2020-02-05 20:13:21.000000 gocli-0.9.8/src/gosdk/specs/definitions/PanelList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      299 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Patient.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      227 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/PatientList.yaml
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)      281 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/PatientMetaData.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)       98 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Phenotype.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1578 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/PrognosesDocument.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      212 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/PrognosesDocumentList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      205 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/QuickAdd.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      210 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Recommendation.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      206 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/RecommendationList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      412 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Reference.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      502 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/ReferenceAttachment.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      165 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/RefreshCursor.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      118 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Refs.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      198 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/ResponseList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      495 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Sample.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      146 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/SelectedMarker.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      110 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Settings.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1930 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/TherapiesDocument.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      339 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/TherapiesDocumentList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      344 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/TimeCourse.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      327 2018-12-06 18:19:43.000000 gocli-0.9.8/src/gosdk/specs/definitions/TranscriptList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)       50 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/TreatmentContexts.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)     3984 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/TrialsDocument.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      333 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/TrialsDocumentList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      737 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/Upload.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      600 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/User.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      115 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/UserCredentials.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      244 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/UserToken.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      443 2018-12-19 15:13:45.000000 gocli-0.9.8/src/gosdk/specs/definitions/WarehouseFeature.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      180 2018-12-19 15:13:45.000000 gocli-0.9.8/src/gosdk/specs/definitions/WarehouseFeatureList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      634 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/WarehouseVariant.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      267 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/WarehouseVariantJoin.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      180 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/WarehouseVariantList.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      249 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/definitions/WarehouseVariantPage.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/alterations/
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1714 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/alterations/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/alterations/{pk}/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      412 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/alterations/{pk}/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/actionability/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/{ref}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/{ref}/{alt}/
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1017 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/delete/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/delete/{data_set}#fs/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      247 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/delete/{data_set}#fs/delete.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/generate_hgvs_g/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      685 2019-04-01 14:50:29.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/generate_hgvs_g/get.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2184 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/hgvs/
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1034 2019-01-28 21:30:41.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/hgvs/get.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1047 2019-04-16 15:46:32.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/hgvs/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/hgvs_overrides/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      558 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/hgvs_overrides/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/load/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/load/{data_set}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/load/{data_set}/{data_set_version}#fs/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      703 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/load/{data_set}/{data_set_version}#fs/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/merged/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/merged/{pk}/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      389 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/merged/{pk}/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/refresh/
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1105 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/refresh/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{build_id}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/{ref}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/{ref}/{alt}/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      821 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{data_set}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{data_set}/batch/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      538 2019-04-01 14:50:29.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{data_set}/batch/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      376 2019-04-01 14:50:29.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/delete.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      402 2019-04-01 14:50:29.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/get.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      487 2019-04-01 14:50:29.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/patch.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      485 2019-04-01 14:50:29.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/put.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{identifier}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{identifier}/proximity/
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2278 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{identifier}/proximity/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{pk}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{pk}/collapsed/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      378 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{pk}/collapsed/get.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      373 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{pk}/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)     2245 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/annotations/
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)     1527 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/annotations/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/annotations-time-courses/
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)     1528 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/annotations-time-courses/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/classifications/
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)     1699 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/classifications/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/classifications-match/
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)      780 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/classifications-match/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/content/
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)      789 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/content/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/disease-alterations/
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)     3344 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/disease-alterations/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/filtered-trials/
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)     3500 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/filtered-trials/get.yaml
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)      382 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/like-mine/
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)     2365 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/like-mine/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/markers/
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)     1485 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/markers/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/off-label/
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)     1747 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/off-label/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/prognoses/
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)      566 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/prognoses/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/therapies/
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)     1738 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/therapies/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/trials/
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)     1705 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/trials/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/classifications/
--rw-r--r--   0 ianmaurer   (501) staff       (20)     3000 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/classifications/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/classifications/match/
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1939 2019-01-28 21:29:34.000000 gocli-0.9.8/src/gosdk/specs/paths/api/classifications/match/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/classifications/{pk}/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      432 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/classifications/{pk}/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/contents/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/contents/counts/
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1686 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/contents/counts/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/contents/detail/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/contents/detail/{uuid}/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      351 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/contents/detail/{uuid}/get.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)     3209 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/contents/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/contents/match/
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2453 2019-01-28 21:29:34.000000 gocli-0.9.8/src/gosdk/specs/paths/api/contents/match/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/contents/set/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      799 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/contents/set/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/genes/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/genes/filter_genes/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      587 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/genes/filter_genes/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/genes/gene_boundaries/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      525 2019-01-30 20:00:19.000000 gocli-0.9.8/src/gosdk/specs/paths/api/genes/gene_boundaries/get.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1817 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/genes/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/info/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/info/annotation_bundle/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      279 2019-01-28 21:30:41.000000 gocli-0.9.8/src/gosdk/specs/paths/api/info/annotation_bundle/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/prognoses/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/prognoses/matches/
--rw-r--r--   0 ianmaurer   (501) staff       (20)     3956 2019-01-28 21:29:34.000000 gocli-0.9.8/src/gosdk/specs/paths/api/prognoses/matches/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/region_search/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/region_search/batch/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      439 2020-04-28 15:25:56.000000 gocli-0.9.8/src/gosdk/specs/paths/api/region_search/batch/get.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      549 2020-04-28 15:25:56.000000 gocli-0.9.8/src/gosdk/specs/paths/api/region_search/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/therapies/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/therapies/matches/
--rw-r--r--   0 ianmaurer   (501) staff       (20)     5325 2019-01-28 21:29:34.000000 gocli-0.9.8/src/gosdk/specs/paths/api/therapies/matches/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/trials/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/trials/matches/
--rw-r--r--   0 ianmaurer   (501) staff       (20)     8211 2019-01-28 21:29:34.000000 gocli-0.9.8/src/gosdk/specs/paths/api/trials/matches/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/api/users/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/users/login/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      357 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/users/login/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/warehouse_features/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      437 2018-12-19 15:13:45.000000 gocli-0.9.8/src/gosdk/specs/paths/api/warehouse_features/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/warehouse_variants/
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1625 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/warehouse_variants/get.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      437 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/warehouse_variants/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/api/warehouse_variants/{pk}/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      385 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/api/warehouse_variants/{pk}/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/assays/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      210 2020-03-31 13:12:57.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/assays/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/assays/panels/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      240 2020-03-31 13:12:57.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/assays/panels/get.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      342 2020-02-05 20:13:21.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/assays/panels/post.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      345 2020-02-05 20:13:21.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/assays/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1122 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/get.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      338 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/{case_uuid}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:17.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/{case_uuid}/added-markers/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      476 2020-02-05 20:13:21.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/{case_uuid}/added-markers/post.yaml
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)      235 2020-04-28 15:25:56.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/{case_uuid}/delete.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/{case_uuid}/generate-recommendations/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      318 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/{case_uuid}/generate-recommendations/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/{case_uuid}/lab-results/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      443 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/{case_uuid}/lab-results/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/{case_uuid}/markers/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      339 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/{case_uuid}/markers/get.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      424 2020-04-28 15:25:56.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/{case_uuid}/put.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/{case_uuid}/recommendations/
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1235 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/{case_uuid}/recommendations/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/{case_uuid}/selected_markers/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      493 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/cases/{case_uuid}/selected_markers/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/markers/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/markers/{uuid}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/markers/{uuid}/MarkerMetaData/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      517 2020-02-05 20:13:21.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/markers/{uuid}/MarkerMetaData/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/meetings/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      826 2020-04-28 15:25:56.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/meetings/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      677 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/lab-result-attachments/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      495 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/lab-result-attachments/post.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      354 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/quick-add/
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1749 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/quick-add/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/search/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      914 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/search/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/cases/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      339 2020-03-31 13:12:57.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/cases/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      411 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/get.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      588 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/post.yaml
--rwxr-xr-x   0 ianmaurer   (501) staff       (20)      236 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/delete.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      422 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      414 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/get.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      580 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/patient_meta_data/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      476 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/patient_meta_data/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/samples/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      560 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/samples/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/samples/{barcode_id}/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      399 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/samples/{barcode_id}/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/uploads/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      720 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/uploads/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/uploads/{id}/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      299 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/consult/uploads/{id}/get.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/curation/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/curation/classifications/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      425 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/curation/classifications/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:16.000000 gocli-0.9.8/src/gosdk/specs/paths/curation/concepts/
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/curation/concepts/alterations/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      499 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/curation/concepts/alterations/get.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      372 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/curation/concepts/alterations/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/curation/contents/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      383 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/curation/contents/post.yaml
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/gosdk/specs/paths/curation/contents/{uuid}/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      236 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/paths/curation/contents/{uuid}/delete.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      268 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/specs/specd.yaml
--rw-r--r--   0 ianmaurer   (501) staff       (20)      447 2018-11-27 16:45:15.000000 gocli-0.9.8/src/gosdk/variables.py
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/govcf/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      482 2018-11-27 16:45:15.000000 gocli-0.9.8/src/govcf/__init__.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     1954 2019-01-30 20:00:19.000000 gocli-0.9.8/src/govcf/bed_filter.py
-drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-06-25 21:39:18.000000 gocli-0.9.8/src/govcf/calculate_vaf/
--rw-r--r--   0 ianmaurer   (501) staff       (20)      389 2020-05-14 10:29:36.000000 gocli-0.9.8/src/govcf/calculate_vaf/__init__.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      626 2018-11-27 16:45:15.000000 gocli-0.9.8/src/govcf/calculate_vaf/ad_rd_dp.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      640 2018-11-27 16:45:15.000000 gocli-0.9.8/src/govcf/calculate_vaf/ao_ro_dp.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     2076 2019-04-26 14:24:33.000000 gocli-0.9.8/src/govcf/calculate_vaf/base.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      652 2018-11-27 16:45:15.000000 gocli-0.9.8/src/govcf/calculate_vaf/brli.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      547 2018-11-27 16:45:15.000000 gocli-0.9.8/src/govcf/calculate_vaf/clcbio.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      760 2020-06-25 21:38:17.000000 gocli-0.9.8/src/govcf/calculate_vaf/fao_fdp.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      636 2018-11-27 16:45:15.000000 gocli-0.9.8/src/govcf/calculate_vaf/pheo.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      693 2018-11-27 16:45:15.000000 gocli-0.9.8/src/govcf/calculate_vaf/strelka.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      631 2018-11-27 16:45:15.000000 gocli-0.9.8/src/govcf/calculate_vaf/usc.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)      242 2018-11-27 16:45:15.000000 gocli-0.9.8/src/govcf/calculate_vaf/utils.py
--rw-r--r--   0 ianmaurer   (501) staff       (20)     8363 2020-04-28 15:25:56.000000 gocli-0.9.8/src/govcf/variant_files.py
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       54 2018-11-27 16:45:15.000000 gocli-0.9.9/MANIFEST.in
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     6278 2020-07-30 17:35:15.000000 gocli-0.9.9/PKG-INFO
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       38 2020-07-30 17:35:15.000000 gocli-0.9.9/setup.cfg
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2427 2020-07-30 17:34:37.000000 gocli-0.9.9/setup.py
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/genomoncology/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      492 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/__init__.py
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/genomoncology/cli/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       68 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/cli/__init__.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)    19285 2020-07-30 17:35:08.000000 gocli-0.9.9/src/genomoncology/cli/commands.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      220 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/cli/const.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     5311 2020-04-28 15:25:56.000000 gocli-0.9.9/src/genomoncology/cli/options.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1188 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/cli/types.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      471 2020-03-31 13:12:57.000000 gocli-0.9.9/src/genomoncology/cli/utils.py
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/genomoncology/kms/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      314 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/kms/__init__.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)    11160 2020-07-30 17:33:22.000000 gocli-0.9.9/src/genomoncology/kms/annotations.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1040 2019-01-28 21:29:34.000000 gocli-0.9.9/src/genomoncology/kms/contents.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1534 2020-05-11 19:37:09.000000 gocli-0.9.9/src/genomoncology/kms/factory.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1255 2019-04-01 14:50:29.000000 gocli-0.9.9/src/genomoncology/kms/genes.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      917 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/kms/match.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1152 2019-01-28 21:29:34.000000 gocli-0.9.9/src/genomoncology/kms/therapies.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      470 2020-04-28 15:25:56.000000 gocli-0.9.9/src/genomoncology/kms/transcripts.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1172 2019-01-28 21:29:34.000000 gocli-0.9.9/src/genomoncology/kms/trials.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      109 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/main.py
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/genomoncology/parse/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      395 2019-04-26 14:24:33.000000 gocli-0.9.9/src/genomoncology/parse/__init__.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     4896 2020-04-28 15:25:56.000000 gocli-0.9.9/src/genomoncology/parse/doctypes.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      595 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/parse/ensures.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      326 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/parse/fieldtypes.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     3497 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/parse/fusions.py
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/genomoncology/pipeline/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      212 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/__init__.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1987 2019-01-30 20:00:19.000000 gocli-0.9.9/src/genomoncology/pipeline/comparators.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2221 2019-04-01 14:50:29.000000 gocli-0.9.9/src/genomoncology/pipeline/converters.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1824 2020-06-25 21:38:17.000000 gocli-0.9.9/src/genomoncology/pipeline/filters.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1733 2019-01-28 21:30:41.000000 gocli-0.9.9/src/genomoncology/pipeline/runner.py
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/genomoncology/pipeline/sinks/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      643 2020-05-11 19:37:09.000000 gocli-0.9.9/src/genomoncology/pipeline/sinks/__init__.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      687 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/sinks/alterations.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2520 2020-04-28 15:25:56.000000 gocli-0.9.9/src/genomoncology/pipeline/sinks/annotations.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1353 2019-04-01 14:50:29.000000 gocli-0.9.9/src/genomoncology/pipeline/sinks/base.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2132 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/sinks/excel.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      995 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/sinks/tsv.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)    11150 2020-06-25 21:38:17.000000 gocli-0.9.9/src/genomoncology/pipeline/sinks/vcf.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2130 2019-04-01 14:50:29.000000 gocli-0.9.9/src/genomoncology/pipeline/sinks/warehouse.py
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      847 2020-06-25 21:38:17.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/__init__.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     9922 2020-05-11 19:37:09.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/aggregated.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      481 2020-06-25 21:38:17.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/annotations_filter.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1234 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/base.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      641 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/bed.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      107 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/const.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2391 2019-08-22 14:04:53.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/delimited.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      850 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/excel.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1992 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/maf.py
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/one_off_sources/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      322 2020-03-31 13:12:57.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/one_off_sources/__init__.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)    14722 2020-05-11 19:37:09.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/one_off_sources/clinvar_xml.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)    14366 2020-04-28 15:25:56.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/one_off_sources/mitomap.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     4859 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/one_off_sources/uniprot.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2732 2019-04-26 14:24:33.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/paths.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     3049 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/smart_lazy_file.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1033 2020-03-31 13:12:57.000000 gocli-0.9.9/src/genomoncology/pipeline/sources/xml.py
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      638 2020-03-31 13:12:50.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/__init__.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     3537 2020-03-31 13:12:50.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/functions.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     4603 2019-01-30 20:00:19.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/mapper_classes.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2236 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/registry.py
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      752 2020-04-28 15:25:56.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/__init__.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1398 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/baylor_decipher.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      694 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/baylor_wgl.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2197 2019-04-26 14:24:33.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/clinvar.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2139 2020-03-31 13:12:57.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/clinvar_xml.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2629 2020-05-11 19:37:09.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/cosmic.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     8034 2020-03-31 13:12:50.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/dbnsfp.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     3514 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/dbsnp.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1398 2019-02-26 14:04:24.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/evs.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2188 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/exac.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1482 2020-03-31 13:12:50.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/gene_type.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      993 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/genie_maf.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     4386 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/gnomad.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2050 2020-03-31 13:12:57.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/hgmd.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      885 2020-04-28 15:25:56.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/hgmd_gene_list.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      905 2020-03-31 13:12:50.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/hpo.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1001 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/markers.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1118 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/mitomap.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     4400 2020-05-11 19:37:09.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/omim.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1045 2020-04-28 15:25:56.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/pli.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1155 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/splicing.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1082 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/thousandgenomes.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1049 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/uniprot.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      943 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/uniprot_domains.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      855 2018-11-27 16:45:15.000000 gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/uniprot_protein_name.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1882 2020-04-28 15:25:56.000000 gocli-0.9.9/src/genomoncology/state.py
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gocli.egg-info/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     6278 2020-07-30 17:35:14.000000 gocli-0.9.9/src/gocli.egg-info/PKG-INFO
+-rw-r--r--   0 ianmaurer   (501) staff       (20)    17097 2020-07-30 17:35:14.000000 gocli-0.9.9/src/gocli.egg-info/SOURCES.txt
+-rw-r--r--   0 ianmaurer   (501) staff       (20)        1 2020-07-30 17:35:14.000000 gocli-0.9.9/src/gocli.egg-info/dependency_links.txt
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       51 2020-07-30 17:35:14.000000 gocli-0.9.9/src/gocli.egg-info/entry_points.txt
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      221 2020-07-30 17:35:14.000000 gocli-0.9.9/src/gocli.egg-info/requires.txt
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       26 2020-07-30 17:35:14.000000 gocli-0.9.9/src/gocli.egg-info/top_level.txt
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      490 2019-04-11 23:07:34.000000 gocli-0.9.9/src/gosdk/__init__.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     4284 2020-04-28 15:25:56.000000 gocli-0.9.9/src/gosdk/construct.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1519 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/logger.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      613 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/models.py
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      532 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Alteration.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      200 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/AlterationList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1138 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/AlterationsDocument.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      216 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/AlterationsDocumentList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1999 2020-06-25 21:38:17.000000 gocli-0.9.9/src/gosdk/specs/definitions/Annotation.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      105 2019-01-28 21:30:41.000000 gocli-0.9.9/src/gosdk/specs/definitions/AnnotationBundleVersion.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      234 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/AnnotationList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      940 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/AnnotationsDocument.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      169 2019-04-01 14:50:29.000000 gocli-0.9.9/src/gosdk/specs/definitions/AnnotationsDocumentAndNotFoundList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      216 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/AnnotationsDocumentList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2161 2019-01-28 21:30:41.000000 gocli-0.9.9/src/gosdk/specs/definitions/Annotations_MergedDocument.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      230 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Annotations_MergedDocumentList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       67 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Arguments.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      208 2020-02-05 20:13:21.000000 gocli-0.9.9/src/gosdk/specs/definitions/Assay.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      165 2020-02-05 20:13:21.000000 gocli-0.9.9/src/gosdk/specs/definitions/AssayList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1814 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Case.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      186 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/CaseList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1601 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/CasesDocument.yaml
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)      204 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/CasesDocumentList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      335 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Classification.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1605 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/ClassificationsDocument.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      224 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/ClassificationsDocumentList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      287 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Content.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1244 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/ContentsDocument.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      210 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/ContentsDocumentList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      110 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Counts.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      244 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/CountsList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      223 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DetectedAlteration.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      211 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Document.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      247 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugBase.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      377 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugClassification.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      227 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugCondition.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      887 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugData.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       99 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugExternalLink.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       94 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugFdaLabel.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      302 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugGFInclude.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      203 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugGFIncludeComponent.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      307 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugGeneralReferences.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      132 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugGeneticFactors.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      105 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugGoClass.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      165 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugIngredient.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      107 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugIngredientStrength.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       70 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugLabeller.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      134 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugLiteratureReference.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      145 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugModificationOf.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       97 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugPfam.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      535 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugPharmacology.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1520 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugPolypeptide.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      702 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugProduct.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      103 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugSeverity.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      377 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugStructuredIndications.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      101 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugSynonym.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      359 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugTarget.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      103 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/DrugWithDrugs.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      355 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/EligibilitiesAsCurated.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      434 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Eligibility.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       88 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Error.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      469 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Evidence.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      128 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Facets.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      678 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Gene.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      168 2019-04-01 14:50:29.000000 gocli-0.9.9/src/gosdk/specs/definitions/GeneBoundaries.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      200 2019-01-30 20:00:19.000000 gocli-0.9.9/src/gosdk/specs/definitions/GeneBoundariesList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      191 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/GenesList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      137 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/HgvsGMetadata.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      837 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/LabResult.yaml
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)      384 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/LabResultAttachmentFile.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      401 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/LabResultDataFile.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      165 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/LabResultDataFileList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      318 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Location.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      221 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/LogicSet.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      929 2020-02-05 20:13:21.000000 gocli-0.9.9/src/gosdk/specs/definitions/Marker.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      166 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/MarkerList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      178 2020-03-31 13:12:57.000000 gocli-0.9.9/src/gosdk/specs/definitions/MarkerMetaData.yaml
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)     1210 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/MarkersDocument.yaml
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)      208 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/MarkersDocumentList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      126 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/MatchedDisease.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       90 2020-04-28 15:25:56.000000 gocli-0.9.9/src/gosdk/specs/definitions/Meeting.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      192 2020-04-28 15:25:56.000000 gocli-0.9.9/src/gosdk/specs/definitions/MeetingList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      124 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/NDGenes.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       50 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewAlteration.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      255 2020-02-05 20:13:21.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewAssay.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1186 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewCase.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      820 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewClassification.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      802 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewContent.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      851 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewDocument.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      297 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewLabResult.yaml
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)      323 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewLabResultAttachmentFile.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      386 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewLabResultDataFile.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      874 2020-02-05 20:13:21.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewMarker.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      324 2020-04-28 15:25:56.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewOncologicTreatment.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      328 2020-02-05 20:13:21.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewPanel.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      719 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewPatient.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      275 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewPatientDiagnosis.yaml
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)      419 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewPatientMetaData.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2375 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewRecommendation.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      120 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewRecommendationsReport.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      218 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewReferenceAttachment.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      379 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewSample.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       92 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/NewSelectedMarker.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       88 2019-04-01 14:50:29.000000 gocli-0.9.9/src/gosdk/specs/definitions/NormalizedHGVS.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      155 2019-04-01 14:50:29.000000 gocli-0.9.9/src/gosdk/specs/definitions/NormalizedHGVSList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      124 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/OutOnlyGenesOffPanel.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       50 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/OutcomeCohorts.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      228 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/OverallContact.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      368 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Pagination.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      160 2020-02-05 20:13:21.000000 gocli-0.9.9/src/gosdk/specs/definitions/Panel.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      165 2020-02-05 20:13:21.000000 gocli-0.9.9/src/gosdk/specs/definitions/PanelList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      299 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Patient.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      227 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/PatientList.yaml
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)      281 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/PatientMetaData.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       98 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Phenotype.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1578 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/PrognosesDocument.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      212 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/PrognosesDocumentList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      205 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/QuickAdd.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      210 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Recommendation.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      206 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/RecommendationList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      412 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Reference.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      502 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/ReferenceAttachment.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      165 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/RefreshCursor.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      118 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Refs.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      198 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/ResponseList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      495 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Sample.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      146 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/SelectedMarker.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      110 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Settings.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1930 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/TherapiesDocument.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      339 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/TherapiesDocumentList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      344 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/TimeCourse.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      327 2018-12-06 18:19:43.000000 gocli-0.9.9/src/gosdk/specs/definitions/TranscriptList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)       50 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/TreatmentContexts.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     3984 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/TrialsDocument.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      333 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/TrialsDocumentList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      737 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/Upload.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      600 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/User.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      115 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/UserCredentials.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      244 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/UserToken.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      443 2018-12-19 15:13:45.000000 gocli-0.9.9/src/gosdk/specs/definitions/WarehouseFeature.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      180 2018-12-19 15:13:45.000000 gocli-0.9.9/src/gosdk/specs/definitions/WarehouseFeatureList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      634 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/WarehouseVariant.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      267 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/WarehouseVariantJoin.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      180 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/WarehouseVariantList.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      249 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/definitions/WarehouseVariantPage.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/alterations/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1714 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/alterations/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/alterations/{pk}/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      412 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/alterations/{pk}/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/actionability/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/{ref}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/{ref}/{alt}/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1017 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/delete/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/delete/{data_set}#fs/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      247 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/delete/{data_set}#fs/delete.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/generate_hgvs_g/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      685 2019-04-01 14:50:29.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/generate_hgvs_g/get.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2184 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/hgvs/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1034 2019-01-28 21:30:41.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/hgvs/get.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1047 2019-04-16 15:46:32.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/hgvs/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/hgvs_overrides/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      558 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/hgvs_overrides/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/load/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/load/{data_set}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/load/{data_set}/{data_set_version}#fs/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      703 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/load/{data_set}/{data_set_version}#fs/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/merged/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/merged/{pk}/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      389 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/merged/{pk}/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/refresh/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1105 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/refresh/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{build_id}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/{ref}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/{ref}/{alt}/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      821 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{data_set}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{data_set}/batch/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      538 2019-04-01 14:50:29.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{data_set}/batch/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      376 2019-04-01 14:50:29.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/delete.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      402 2019-04-01 14:50:29.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/get.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      487 2019-04-01 14:50:29.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/patch.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      485 2019-04-01 14:50:29.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{data_set}/{hgvs_g}/put.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{identifier}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{identifier}/proximity/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2278 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{identifier}/proximity/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{pk}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{pk}/collapsed/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      378 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{pk}/collapsed/get.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      373 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{pk}/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)     2245 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/annotations/
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)     1527 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/annotations/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/annotations-time-courses/
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)     1528 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/annotations-time-courses/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/classifications/
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)     1699 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/classifications/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/classifications-match/
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)      780 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/classifications-match/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/content/
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)      789 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/content/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/disease-alterations/
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)     3344 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/disease-alterations/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/filtered-trials/
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)     3500 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/filtered-trials/get.yaml
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)      382 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/like-mine/
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)     2365 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/like-mine/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/markers/
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)     1485 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/markers/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/off-label/
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)     1747 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/off-label/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/prognoses/
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)      566 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/prognoses/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/therapies/
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)     1738 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/therapies/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/trials/
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)     1705 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/trials/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/classifications/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     3000 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/classifications/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/classifications/match/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1939 2019-01-28 21:29:34.000000 gocli-0.9.9/src/gosdk/specs/paths/api/classifications/match/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/classifications/{pk}/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      432 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/classifications/{pk}/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/contents/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/contents/counts/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1686 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/contents/counts/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/contents/detail/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/contents/detail/{uuid}/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      351 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/contents/detail/{uuid}/get.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     3209 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/contents/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/contents/match/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2453 2019-01-28 21:29:34.000000 gocli-0.9.9/src/gosdk/specs/paths/api/contents/match/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/contents/set/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      799 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/contents/set/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/genes/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/genes/filter_genes/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      587 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/genes/filter_genes/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/genes/gene_boundaries/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      525 2019-01-30 20:00:19.000000 gocli-0.9.9/src/gosdk/specs/paths/api/genes/gene_boundaries/get.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1817 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/genes/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/info/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/info/annotation_bundle/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      279 2019-01-28 21:30:41.000000 gocli-0.9.9/src/gosdk/specs/paths/api/info/annotation_bundle/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/prognoses/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/prognoses/matches/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     3956 2019-01-28 21:29:34.000000 gocli-0.9.9/src/gosdk/specs/paths/api/prognoses/matches/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/region_search/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/region_search/batch/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      439 2020-04-28 15:25:56.000000 gocli-0.9.9/src/gosdk/specs/paths/api/region_search/batch/get.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      549 2020-04-28 15:25:56.000000 gocli-0.9.9/src/gosdk/specs/paths/api/region_search/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/therapies/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/therapies/matches/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     5325 2019-01-28 21:29:34.000000 gocli-0.9.9/src/gosdk/specs/paths/api/therapies/matches/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/trials/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/trials/matches/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     8211 2019-01-28 21:29:34.000000 gocli-0.9.9/src/gosdk/specs/paths/api/trials/matches/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/users/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/users/login/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      357 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/users/login/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/warehouse_features/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      437 2018-12-19 15:13:45.000000 gocli-0.9.9/src/gosdk/specs/paths/api/warehouse_features/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/warehouse_variants/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1625 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/warehouse_variants/get.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      437 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/warehouse_variants/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/warehouse_variants/{pk}/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      385 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/api/warehouse_variants/{pk}/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/assays/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      210 2020-03-31 13:12:57.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/assays/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/assays/panels/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      240 2020-03-31 13:12:57.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/assays/panels/get.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      342 2020-02-05 20:13:21.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/assays/panels/post.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      345 2020-02-05 20:13:21.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/assays/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1122 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/get.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      338 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/{case_uuid}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/{case_uuid}/added-markers/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      476 2020-02-05 20:13:21.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/{case_uuid}/added-markers/post.yaml
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)      235 2020-04-28 15:25:56.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/{case_uuid}/delete.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/{case_uuid}/generate-recommendations/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      318 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/{case_uuid}/generate-recommendations/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/{case_uuid}/lab-results/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      443 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/{case_uuid}/lab-results/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/{case_uuid}/markers/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      339 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/{case_uuid}/markers/get.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      424 2020-04-28 15:25:56.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/{case_uuid}/put.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/{case_uuid}/recommendations/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1235 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/{case_uuid}/recommendations/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/{case_uuid}/selected_markers/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      493 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/cases/{case_uuid}/selected_markers/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/markers/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/markers/{uuid}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/markers/{uuid}/MarkerMetaData/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      517 2020-02-05 20:13:21.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/markers/{uuid}/MarkerMetaData/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/meetings/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      826 2020-04-28 15:25:56.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/meetings/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      677 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/lab-result-attachments/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      495 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/lab-result-attachments/post.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      354 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/quick-add/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1749 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/quick-add/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/search/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      914 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/search/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/cases/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      339 2020-03-31 13:12:57.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/cases/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      411 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/get.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      588 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/post.yaml
+-rwxr-xr-x   0 ianmaurer   (501) staff       (20)      236 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/delete.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      422 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      414 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/get.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      580 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/patient_meta_data/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      476 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/patient_meta_data/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/samples/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      560 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/samples/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/samples/{barcode_id}/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      399 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/samples/{barcode_id}/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/uploads/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      720 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/uploads/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/uploads/{id}/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      299 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/consult/uploads/{id}/get.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/curation/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/curation/classifications/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      425 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/curation/classifications/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/curation/concepts/
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/curation/concepts/alterations/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      499 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/curation/concepts/alterations/get.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      372 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/curation/concepts/alterations/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/curation/contents/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      383 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/curation/contents/post.yaml
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/gosdk/specs/paths/curation/contents/{uuid}/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      236 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/paths/curation/contents/{uuid}/delete.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      268 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/specs/specd.yaml
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      447 2018-11-27 16:45:15.000000 gocli-0.9.9/src/gosdk/variables.py
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/govcf/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      482 2018-11-27 16:45:15.000000 gocli-0.9.9/src/govcf/__init__.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     1954 2019-01-30 20:00:19.000000 gocli-0.9.9/src/govcf/bed_filter.py
+drwxr-xr-x   0 ianmaurer   (501) staff       (20)        0 2020-07-30 17:35:15.000000 gocli-0.9.9/src/govcf/calculate_vaf/
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      389 2020-05-14 10:29:36.000000 gocli-0.9.9/src/govcf/calculate_vaf/__init__.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      626 2018-11-27 16:45:15.000000 gocli-0.9.9/src/govcf/calculate_vaf/ad_rd_dp.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      640 2018-11-27 16:45:15.000000 gocli-0.9.9/src/govcf/calculate_vaf/ao_ro_dp.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     2076 2019-04-26 14:24:33.000000 gocli-0.9.9/src/govcf/calculate_vaf/base.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      652 2018-11-27 16:45:15.000000 gocli-0.9.9/src/govcf/calculate_vaf/brli.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      547 2018-11-27 16:45:15.000000 gocli-0.9.9/src/govcf/calculate_vaf/clcbio.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      760 2020-06-25 21:38:17.000000 gocli-0.9.9/src/govcf/calculate_vaf/fao_fdp.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      636 2018-11-27 16:45:15.000000 gocli-0.9.9/src/govcf/calculate_vaf/pheo.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      693 2018-11-27 16:45:15.000000 gocli-0.9.9/src/govcf/calculate_vaf/strelka.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      631 2018-11-27 16:45:15.000000 gocli-0.9.9/src/govcf/calculate_vaf/usc.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)      242 2018-11-27 16:45:15.000000 gocli-0.9.9/src/govcf/calculate_vaf/utils.py
+-rw-r--r--   0 ianmaurer   (501) staff       (20)     8363 2020-04-28 15:25:56.000000 gocli-0.9.9/src/govcf/variant_files.py
```

### Comparing `gocli-0.9.8/PKG-INFO` & `gocli-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gocli
-Version: 0.9.8
+Version: 0.9.9
 Summary: gocli
 Home-page: UNKNOWN
 Author: Ian Maurer
 Author-email: ian@genomoncology.com
 License: Proprietary
 Description: gocli - GenomOncology Command Line Interface
         ============================================
```

### Comparing `gocli-0.9.8/setup.py` & `gocli-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "aioconsole >= 0.1.8",
     "addict >= 2.1.3",
     "requests >= 2.4",
 ]
 
 setup(
     name="gocli",
-    version='0.9.8',
+    version='0.9.9',
     author="Ian Maurer",
     author_email='ian@genomoncology.com',
 
     packages=[
         "genomoncology",
         "genomoncology.kms",
         "genomoncology.cli",
```

### Comparing `gocli-0.9.8/src/genomoncology/cli/commands.py` & `gocli-0.9.9/src/genomoncology/cli/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 # const
 
 DEFAULT_SPECD_PATH = os.path.join(
     os.path.dirname(__file__), "../../gosdk/specs/"
 )
 
-VERSION = "0.9.8"
+VERSION = "0.9.9"
 COPYRIGHT = "Copyright: GenomOncology, LLC"
 
 
 def print_version(ctx, _, value):
     if not value or ctx.resilient_parsing:
         return
     click.echo(f"GO CLI: Version {VERSION}")
@@ -348,14 +348,20 @@
 
     filter_anns = (
         [ann for ann in list(sources.AnnotationsFilterFileSource(filter_file))]
         if filter_file is not None
         else None
     )
 
+    # get the annotation bundle version once instead of once per batch
+    sdk = state.create_sdk(async_enabled=False)
+    annotation_bundle_version = kms.annotations.get_annotation_bundle_version(
+        sdk
+    )
+
     return [
         filter(is_not_skipped_call),
         filter(
             filter_out_ref_unknown(
                 keep_ref_unknown_calls=keep_ref_unknown_calls
             )
         ),
@@ -365,14 +371,15 @@
         create_function(
             state,
             sdk_function,
             fields=fields,
             delete_if_exists=delete_if_exists,
             build=state.build,
             filter_anns=filter_anns,
+            annotation_bundle_version=annotation_bundle_version,
         ),
         concat,
     ]
 
 
 @gocli.command()
 @options.build_option
```

### Comparing `gocli-0.9.8/src/genomoncology/cli/options.py` & `gocli-0.9.9/src/genomoncology/cli/options.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/cli/types.py` & `gocli-0.9.9/src/genomoncology/cli/types.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/kms/annotations.py` & `gocli-0.9.9/src/genomoncology/kms/annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,19 +39,18 @@
 async def async_annotate(
     data,
     sdk=None,
     fields=None,
     delete_if_exists=False,
     build=GRCh37,
     filter_anns=None,
+    annotation_bundle_version=None,
 ):
     csra_batch = convert_to_csra([{**d, "build": build} for d in data])
 
-    annotation_bundle_version = await get_annotation_bundle_version_async(sdk)
-
     if csra_batch:
         annotations_list = await sdk.call_with_retry(
             sdk.annotations.post_annotations,
             batch=csra_batch,
             delete_if_exists=delete_if_exists,
             build=build,
         )
@@ -82,19 +81,18 @@
 def sync_annotate(
     data,
     sdk=None,
     fields=None,
     delete_if_exists=False,
     build=GRCh37,
     filter_anns=None,
+    annotation_bundle_version=None,
 ):
     csra_batch = convert_to_csra([{**d, "build": build} for d in data])
 
-    annotation_bundle_version = get_annotation_bundle_version(sdk)
-
     annotations_list = (
         sdk.call_with_retry(
             sdk.annotations.post_annotations,
             batch=csra_batch,
             delete_if_exists=delete_if_exists,
             build=build,
         )
@@ -392,11 +390,11 @@
     "canonical_p_dot",
     "clinvar__CLNSIG__string",
     "display",
     "mutation_type",
     "representations",
     "hgvs_g",
     "alteration",
-    "gene_annotations"
+    "gene_annotations",
 ]
 
 ANNOTATIONS_SET = set(ANNOTATIONS)
```

### Comparing `gocli-0.9.8/src/genomoncology/kms/contents.py` & `gocli-0.9.9/src/genomoncology/kms/contents.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/kms/factory.py` & `gocli-0.9.9/src/genomoncology/kms/factory.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/kms/genes.py` & `gocli-0.9.9/src/genomoncology/kms/genes.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/kms/match.py` & `gocli-0.9.9/src/genomoncology/kms/match.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/kms/therapies.py` & `gocli-0.9.9/src/genomoncology/kms/therapies.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/kms/trials.py` & `gocli-0.9.9/src/genomoncology/kms/trials.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/parse/doctypes.py` & `gocli-0.9.9/src/genomoncology/parse/doctypes.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/parse/ensures.py` & `gocli-0.9.9/src/genomoncology/parse/ensures.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/parse/fusions.py` & `gocli-0.9.9/src/genomoncology/parse/fusions.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/comparators.py` & `gocli-0.9.9/src/genomoncology/pipeline/comparators.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/converters.py` & `gocli-0.9.9/src/genomoncology/pipeline/converters.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/filters.py` & `gocli-0.9.9/src/genomoncology/pipeline/filters.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/runner.py` & `gocli-0.9.9/src/genomoncology/pipeline/runner.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sinks/__init__.py` & `gocli-0.9.9/src/genomoncology/pipeline/sinks/__init__.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sinks/alterations.py` & `gocli-0.9.9/src/genomoncology/pipeline/sinks/alterations.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sinks/annotations.py` & `gocli-0.9.9/src/genomoncology/pipeline/sinks/annotations.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sinks/base.py` & `gocli-0.9.9/src/genomoncology/pipeline/sinks/base.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sinks/excel.py` & `gocli-0.9.9/src/genomoncology/pipeline/sinks/excel.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sinks/tsv.py` & `gocli-0.9.9/src/genomoncology/pipeline/sinks/tsv.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sinks/vcf.py` & `gocli-0.9.9/src/genomoncology/pipeline/sinks/vcf.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sinks/warehouse.py` & `gocli-0.9.9/src/genomoncology/pipeline/sinks/warehouse.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sources/__init__.py` & `gocli-0.9.9/src/genomoncology/pipeline/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sources/aggregated.py` & `gocli-0.9.9/src/genomoncology/pipeline/sources/aggregated.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sources/base.py` & `gocli-0.9.9/src/genomoncology/pipeline/sources/base.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sources/bed.py` & `gocli-0.9.9/src/genomoncology/pipeline/sources/bed.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sources/delimited.py` & `gocli-0.9.9/src/genomoncology/pipeline/sources/delimited.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sources/excel.py` & `gocli-0.9.9/src/genomoncology/pipeline/sources/excel.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sources/maf.py` & `gocli-0.9.9/src/genomoncology/pipeline/sources/maf.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sources/one_off_sources/clinvar_xml.py` & `gocli-0.9.9/src/genomoncology/pipeline/sources/one_off_sources/clinvar_xml.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sources/one_off_sources/mitomap.py` & `gocli-0.9.9/src/genomoncology/pipeline/sources/one_off_sources/mitomap.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sources/one_off_sources/uniprot.py` & `gocli-0.9.9/src/genomoncology/pipeline/sources/one_off_sources/uniprot.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sources/paths.py` & `gocli-0.9.9/src/genomoncology/pipeline/sources/paths.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sources/smart_lazy_file.py` & `gocli-0.9.9/src/genomoncology/pipeline/sources/smart_lazy_file.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/sources/xml.py` & `gocli-0.9.9/src/genomoncology/pipeline/sources/xml.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/__init__.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/functions.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/functions.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/mapper_classes.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/mapper_classes.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/registry.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/registry.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/__init__.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/__init__.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/baylor_decipher.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/baylor_decipher.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/baylor_wgl.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/baylor_wgl.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/clinvar.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/clinvar.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/clinvar_xml.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/clinvar_xml.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/cosmic.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/cosmic.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/dbnsfp.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/dbnsfp.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/dbsnp.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/dbsnp.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/evs.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/evs.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/exac.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/exac.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/gene_type.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/gene_type.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/genie_maf.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/genie_maf.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/gnomad.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/gnomad.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/hgmd.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/hgmd.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/hgmd_gene_list.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/hgmd_gene_list.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/hpo.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/hpo.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/markers.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/markers.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/mitomap.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/mitomap.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/omim.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/omim.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/pli.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/pli.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/splicing.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/splicing.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/thousandgenomes.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/thousandgenomes.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/uniprot.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/uniprot.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/uniprot_domains.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/uniprot_domains.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/pipeline/transformers/tx/uniprot_protein_name.py` & `gocli-0.9.9/src/genomoncology/pipeline/transformers/tx/uniprot_protein_name.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/genomoncology/state.py` & `gocli-0.9.9/src/genomoncology/state.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gocli.egg-info/PKG-INFO` & `gocli-0.9.9/src/gocli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gocli
-Version: 0.9.8
+Version: 0.9.9
 Summary: gocli
 Home-page: UNKNOWN
 Author: Ian Maurer
 Author-email: ian@genomoncology.com
 License: Proprietary
 Description: gocli - GenomOncology Command Line Interface
         ============================================
```

### Comparing `gocli-0.9.8/src/gocli.egg-info/SOURCES.txt` & `gocli-0.9.9/src/gocli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/construct.py` & `gocli-0.9.9/src/gosdk/construct.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/logger.py` & `gocli-0.9.9/src/gosdk/logger.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/models.py` & `gocli-0.9.9/src/gosdk/models.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/Alteration.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/Alteration.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/AlterationsDocument.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/AlterationsDocument.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/Annotation.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/Annotation.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/AnnotationsDocument.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/AnnotationsDocument.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/Annotations_MergedDocument.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/Annotations_MergedDocument.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/Case.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/Case.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/CasesDocument.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/CasesDocument.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/ClassificationsDocument.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/ClassificationsDocument.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/ContentsDocument.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/ContentsDocument.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/DrugData.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/DrugData.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/DrugPharmacology.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/DrugPharmacology.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/DrugPolypeptide.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/DrugPolypeptide.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/DrugProduct.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/DrugProduct.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/Gene.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/Gene.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/LabResult.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/LabResult.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/Marker.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/Marker.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/MarkersDocument.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/MarkersDocument.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/NewCase.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/NewCase.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/NewClassification.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/NewClassification.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/NewContent.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/NewContent.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/NewDocument.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/NewDocument.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/NewMarker.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/NewMarker.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/NewPatient.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/NewPatient.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/NewRecommendation.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/NewRecommendation.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/PrognosesDocument.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/PrognosesDocument.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/TherapiesDocument.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/TherapiesDocument.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/TrialsDocument.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/TrialsDocument.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/Upload.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/Upload.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/User.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/User.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/definitions/WarehouseVariant.yaml` & `gocli-0.9.9/src/gosdk/specs/definitions/WarehouseVariant.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/alterations/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/alterations/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/annotations/actionability/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/annotations/generate_hgvs_g/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/annotations/generate_hgvs_g/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/annotations/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/annotations/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/annotations/hgvs/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/annotations/hgvs/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/annotations/hgvs/post.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/annotations/hgvs/post.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/annotations/hgvs_overrides/post.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/annotations/hgvs_overrides/post.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/annotations/load/{data_set}/{data_set_version}#fs/post.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/annotations/load/{data_set}/{data_set_version}#fs/post.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/annotations/refresh/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/annotations/refresh/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{build_id}/{chromosome}/{start}/{ref}/{alt}/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{data_set}/batch/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{data_set}/batch/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/annotations/{identifier}/proximity/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/annotations/{identifier}/proximity/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/cases/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/cases/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/annotations/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/annotations/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/annotations-time-courses/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/annotations-time-courses/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/classifications/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/classifications/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/classifications-match/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/classifications-match/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/content/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/content/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/disease-alterations/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/disease-alterations/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/filtered-trials/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/filtered-trials/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/like-mine/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/like-mine/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/markers/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/markers/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/off-label/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/off-label/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/prognoses/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/prognoses/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/therapies/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/therapies/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/cases/{pk}/trials/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/cases/{pk}/trials/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/classifications/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/classifications/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/classifications/match/post.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/classifications/match/post.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/contents/counts/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/contents/counts/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/contents/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/contents/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/contents/match/post.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/contents/match/post.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/contents/set/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/contents/set/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/genes/filter_genes/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/genes/filter_genes/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/genes/gene_boundaries/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/genes/gene_boundaries/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/genes/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/genes/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/prognoses/matches/post.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/prognoses/matches/post.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/region_search/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/region_search/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/therapies/matches/post.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/therapies/matches/post.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/trials/matches/post.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/trials/matches/post.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/api/warehouse_variants/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/api/warehouse_variants/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/consult/cases/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/consult/cases/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/consult/cases/{case_uuid}/recommendations/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/consult/cases/{case_uuid}/recommendations/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/consult/markers/{uuid}/MarkerMetaData/post.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/consult/markers/{uuid}/MarkerMetaData/post.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/consult/meetings/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/consult/meetings/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/consult/patients/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/consult/patients/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/consult/patients/quick-add/post.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/consult/patients/quick-add/post.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/consult/patients/search/get.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/consult/patients/search/get.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/post.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/data-files/{data_file_uuid}/markers/post.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/post.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/lab-results/{lab_result_uuid}/data-files/post.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/consult/patients/{uuid}/samples/post.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/consult/patients/{uuid}/samples/post.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/gosdk/specs/paths/consult/uploads/post.yaml` & `gocli-0.9.9/src/gosdk/specs/paths/consult/uploads/post.yaml`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/govcf/bed_filter.py` & `gocli-0.9.9/src/govcf/bed_filter.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/govcf/calculate_vaf/ad_rd_dp.py` & `gocli-0.9.9/src/govcf/calculate_vaf/ad_rd_dp.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/govcf/calculate_vaf/ao_ro_dp.py` & `gocli-0.9.9/src/govcf/calculate_vaf/ao_ro_dp.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/govcf/calculate_vaf/base.py` & `gocli-0.9.9/src/govcf/calculate_vaf/base.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/govcf/calculate_vaf/brli.py` & `gocli-0.9.9/src/govcf/calculate_vaf/brli.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/govcf/calculate_vaf/clcbio.py` & `gocli-0.9.9/src/govcf/calculate_vaf/clcbio.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/govcf/calculate_vaf/fao_fdp.py` & `gocli-0.9.9/src/govcf/calculate_vaf/fao_fdp.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/govcf/calculate_vaf/pheo.py` & `gocli-0.9.9/src/govcf/calculate_vaf/pheo.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/govcf/calculate_vaf/strelka.py` & `gocli-0.9.9/src/govcf/calculate_vaf/strelka.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/govcf/calculate_vaf/usc.py` & `gocli-0.9.9/src/govcf/calculate_vaf/usc.py`

 * *Files identical despite different names*

### Comparing `gocli-0.9.8/src/govcf/variant_files.py` & `gocli-0.9.9/src/govcf/variant_files.py`

 * *Files identical despite different names*

