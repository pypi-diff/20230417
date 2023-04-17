# Comparing `tmp/dcm-processor-0.9.9.tar.gz` & `tmp/dcm-processor-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcm-processor-0.9.9.tar", last modified: Sat Apr  1 16:32:03 2023, max compression
+gzip compressed data, was "dcm-processor-1.0.0.tar", last modified: Mon Apr 17 09:55:16 2023, max compression
```

## Comparing `dcm-processor-0.9.9.tar` & `dcm-processor-1.0.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-01 16:32:03.593845 dcm-processor-0.9.9/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1074 2021-05-11 10:55:48.000000 dcm-processor-0.9.9/LICENSE
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6002 2023-04-01 16:32:03.595802 dcm-processor-0.9.9/PKG-INFO
--rwxr-xr-x   0 giles     (1000) giles     (1000)     5502 2023-02-01 17:56:58.000000 dcm-processor-0.9.9/README.md
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-01 16:32:03.337386 dcm-processor-0.9.9/dcm_processor/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       61 2021-10-17 14:30:50.000000 dcm-processor-0.9.9/dcm_processor/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    32972 2023-04-01 15:17:10.000000 dcm-processor-0.9.9/dcm_processor/files.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    39327 2023-04-01 11:58:24.000000 dcm-processor-0.9.9/dcm_processor/script.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-01 16:32:03.320589 dcm-processor-0.9.9/dcm_processor/services/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-01 16:32:03.320185 dcm-processor-0.9.9/dcm_processor/services/base/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-01 16:32:03.371945 dcm-processor-0.9.9/dcm_processor/services/base/module/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-01 16:32:03.481743 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/
--rwxr-xr-x   0 giles     (1000) giles     (1000)   642195 2021-10-17 16:16:14.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)    17869 2021-10-17 16:16:15.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)      406 2023-03-31 12:31:28.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1551 2023-03-31 12:36:10.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    69564 2021-10-17 16:16:15.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-01 16:32:03.503390 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/config/
--rwxr-xr-x   0 giles     (1000) giles     (1000)    59497 2021-10-17 16:16:15.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script
--rwxr-xr-x   0 giles     (1000) giles     (1000)      248 2021-10-17 16:16:15.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/config/hash_table.csv
--rwxr-xr-x   0 giles     (1000) giles     (1000)       86 2021-10-17 16:16:15.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/config/psudonyms.csv
--rwxr-xr-x   0 giles     (1000) giles     (1000)    10424 2021-10-17 16:16:15.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   863881 2021-10-17 16:16:16.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)     3471 2023-03-31 12:35:15.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)  1172845 2021-10-17 16:16:18.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   391834 2021-10-17 16:16:19.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)    28241 2021-10-17 16:16:19.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   338969 2021-10-17 16:16:20.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/util.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1777 2023-03-31 20:09:03.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/utils.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)       26 2021-10-17 16:16:20.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/requirements.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       72 2021-10-17 16:16:20.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/script.sh
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-01 16:32:03.518159 dcm-processor-0.9.9/dcm_processor/services/base/module/storageManager/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/storageManager/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)       97 2021-10-17 16:16:20.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/storageManager/header_codes.json
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6218 2023-01-31 18:15:24.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/storageManager/lib.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    10012 2023-01-31 18:15:43.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/storageManager/main.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-01 16:32:03.524411 dcm-processor-0.9.9/dcm_processor/services/base/module/systemcleaner/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/systemcleaner/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     3806 2023-04-01 16:24:05.000000 dcm-processor-0.9.9/dcm_processor/services/base/module/systemcleaner/main.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-01 16:32:03.539700 dcm-processor-0.9.9/dcm_processor/services/base/registry/
--rwxr-xr-x   0 giles     (1000) giles     (1000)      443 2021-10-17 16:16:20.000000 dcm-processor-0.9.9/dcm_processor/services/base/registry/__init__.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-01 16:32:03.321235 dcm-processor-0.9.9/dcm_processor/services/dcm2nii/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-01 16:32:03.580865 dcm-processor-0.9.9/dcm_processor/services/dcm2nii/module/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     3714 2023-03-24 20:51:54.000000 dcm-processor-0.9.9/dcm_processor/services/dcm2nii/module/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)  1948128 2023-03-02 19:03:11.000000 dcm-processor-0.9.9/dcm_processor/services/dcm2nii/module/dcm2niix
--rwxr-xr-x   0 giles     (1000) giles     (1000)      406 2023-03-24 20:50:04.000000 dcm-processor-0.9.9/dcm_processor/services/dcm2nii/module/lib.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-01 16:32:03.591797 dcm-processor-0.9.9/dcm_processor/services/dcm2nii/registry/
--rwxr-xr-x   0 giles     (1000) giles     (1000)      755 2023-04-01 16:29:56.000000 dcm-processor-0.9.9/dcm_processor/services/dcm2nii/registry/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)      285 2023-04-01 13:10:09.000000 dcm-processor-0.9.9/dcm_processor/services/dcm2nii/registry/settings.json
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6601 2023-02-01 11:09:28.000000 dcm-processor-0.9.9/dcm_processor/worker.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-01 16:32:03.365655 dcm-processor-0.9.9/dcm_processor.egg-info/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6002 2023-04-01 16:32:02.000000 dcm-processor-0.9.9/dcm_processor.egg-info/PKG-INFO
--rwxr-xr-x   0 giles     (1000) giles     (1000)     2341 2023-04-01 16:32:03.000000 dcm-processor-0.9.9/dcm_processor.egg-info/SOURCES.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)        1 2023-04-01 16:32:02.000000 dcm-processor-0.9.9/dcm_processor.egg-info/dependency_links.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       53 2023-04-01 16:32:02.000000 dcm-processor-0.9.9/dcm_processor.egg-info/entry_points.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       67 2023-04-01 16:32:02.000000 dcm-processor-0.9.9/dcm_processor.egg-info/requires.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       14 2023-04-01 16:32:02.000000 dcm-processor-0.9.9/dcm_processor.egg-info/top_level.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       89 2021-10-17 14:23:09.000000 dcm-processor-0.9.9/pyproject.toml
--rwxr-xr-x   0 giles     (1000) giles     (1000)      970 2023-04-01 16:32:03.600442 dcm-processor-0.9.9/setup.cfg
--rwxr-xr-x   0 giles     (1000) giles     (1000)      109 2021-10-17 19:37:23.000000 dcm-processor-0.9.9/setup.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 09:55:16.715927 dcm-processor-1.0.0/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1074 2021-05-11 10:55:48.000000 dcm-processor-1.0.0/LICENSE
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      499 2023-04-17 09:55:16.716750 dcm-processor-1.0.0/PKG-INFO
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 09:55:16.541414 dcm-processor-1.0.0/dcm_processor/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       61 2021-10-17 14:30:50.000000 dcm-processor-1.0.0/dcm_processor/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    15407 2023-04-15 09:02:58.000000 dcm-processor-1.0.0/dcm_processor/argparser.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    33004 2023-04-14 11:38:11.000000 dcm-processor-1.0.0/dcm_processor/files.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    45684 2023-04-13 10:23:49.000000 dcm-processor-1.0.0/dcm_processor/script.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 09:55:16.524925 dcm-processor-1.0.0/dcm_processor/services/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 09:55:16.524435 dcm-processor-1.0.0/dcm_processor/services/base/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 09:55:16.560600 dcm-processor-1.0.0/dcm_processor/services/base/module/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 09:55:16.638233 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   642195 2021-10-17 16:16:14.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    17869 2021-10-17 16:16:15.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      526 2023-04-06 14:13:53.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1551 2023-03-31 12:36:10.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    69564 2021-10-17 16:16:15.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 09:55:16.646008 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/config/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    59497 2021-10-17 16:16:15.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      248 2021-10-17 16:16:15.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/config/hash_table.csv
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       86 2021-10-17 16:16:15.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/config/psudonyms.csv
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    10424 2021-10-17 16:16:15.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   863881 2021-10-17 16:16:16.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     3471 2023-03-31 12:35:15.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)  1172845 2021-10-17 16:16:18.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   391834 2021-10-17 16:16:19.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    28241 2021-10-17 16:16:19.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   338969 2021-10-17 16:16:20.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/util.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1777 2023-03-31 20:09:03.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/utils.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       26 2021-10-17 16:16:20.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/requirements.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       72 2021-10-17 16:16:20.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/script.sh
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 09:55:16.658796 dcm-processor-1.0.0/dcm_processor/services/base/module/storageManager/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/storageManager/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       97 2021-10-17 16:16:20.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/storageManager/header_codes.json
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6218 2023-01-31 18:15:24.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/storageManager/lib.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    10012 2023-01-31 18:15:43.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/storageManager/main.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 09:55:16.665305 dcm-processor-1.0.0/dcm_processor/services/base/module/systemcleaner/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/systemcleaner/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     3806 2023-04-01 16:24:05.000000 dcm-processor-1.0.0/dcm_processor/services/base/module/systemcleaner/main.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 09:55:16.668831 dcm-processor-1.0.0/dcm_processor/services/base/registry/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      443 2021-10-17 16:16:20.000000 dcm-processor-1.0.0/dcm_processor/services/base/registry/__init__.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 09:55:16.525577 dcm-processor-1.0.0/dcm_processor/services/dcm2nii/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 09:55:16.707779 dcm-processor-1.0.0/dcm_processor/services/dcm2nii/module/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     4030 2023-04-14 14:47:11.000000 dcm-processor-1.0.0/dcm_processor/services/dcm2nii/module/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)  1948128 2023-03-02 19:03:11.000000 dcm-processor-1.0.0/dcm_processor/services/dcm2nii/module/dcm2niix
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      406 2023-03-24 20:50:04.000000 dcm-processor-1.0.0/dcm_processor/services/dcm2nii/module/lib.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 09:55:16.713476 dcm-processor-1.0.0/dcm_processor/services/dcm2nii/registry/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1013 2023-04-14 12:17:35.000000 dcm-processor-1.0.0/dcm_processor/services/dcm2nii/registry/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      285 2023-04-01 13:10:09.000000 dcm-processor-1.0.0/dcm_processor/services/dcm2nii/registry/settings.json
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6601 2023-02-01 11:09:28.000000 dcm-processor-1.0.0/dcm_processor/worker.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 09:55:16.556362 dcm-processor-1.0.0/dcm_processor.egg-info/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      499 2023-04-17 09:55:15.000000 dcm-processor-1.0.0/dcm_processor.egg-info/PKG-INFO
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     2358 2023-04-17 09:55:16.000000 dcm-processor-1.0.0/dcm_processor.egg-info/SOURCES.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)        1 2023-04-17 09:55:15.000000 dcm-processor-1.0.0/dcm_processor.egg-info/dependency_links.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       53 2023-04-17 09:55:15.000000 dcm-processor-1.0.0/dcm_processor.egg-info/entry_points.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       76 2023-04-17 09:55:15.000000 dcm-processor-1.0.0/dcm_processor.egg-info/requires.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       14 2023-04-17 09:55:15.000000 dcm-processor-1.0.0/dcm_processor.egg-info/top_level.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       89 2021-10-17 14:23:09.000000 dcm-processor-1.0.0/pyproject.toml
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      980 2023-04-17 09:55:16.722965 dcm-processor-1.0.0/setup.cfg
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      109 2021-10-17 19:37:23.000000 dcm-processor-1.0.0/setup.py
```

### Comparing `dcm-processor-0.9.9/LICENSE` & `dcm-processor-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/files.py` & `dcm-processor-1.0.0/dcm_processor/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,16 +312,16 @@
 LOGS=/logs
 DASHBOARD=/dashboard
 
 SCHEDULER_HOST=http://scheduler
 SCHEDULER_PORT=5000
 SCHEDULER_SETTINGS=/settings.json
 
-ORTHANC_REST_USERNAME=admin
-ORTHANC_REST_PASSWORD=admin
+ORTHANC_REST_USERNAME=dcm-processor
+ORTHANC_REST_PASSWORD=dcm-processor
 ORTHANC_REST_URL=http://orthanc:8042
 ORTHANC_DEFUALT_STORE=pac
 CLEAN_ORTHANC=0
 
 ORTHANC_DICOM_PORT=4242
 ORTHANC_BROWSER_PORT=8042
 DASHBOARD_PORT=5000
@@ -613,15 +613,15 @@
   /**
      "AuthenticationEnabled" : true,
    **/
 
   // The list of the registered users. Because Orthanc uses HTTP
   // Basic Authentication, the passwords are stored as plain text.
   "RegisteredUsers": {
-    "admin": "admin"
+    "dcm-processor": "dcm-processor"
   },
 
 
 
   /**
    * Network topology
    **/
```

### Comparing `dcm-processor-0.9.9/dcm_processor/script.py` & `dcm-processor-1.0.0/dcm_processor/script.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,100 @@
 #!/usr/bin/env python3
 
 from __future__ import print_function
-import os, argparse, json, dotenv
+import os, json, dotenv
 import inquirer as inq
-import tempfile, git
+import tempfile, git, requests, re, shutil
 from ruamel.yaml import YAML
 from . import files as FILES
 from . import worker as WORKER
+from .argparser import parse_args
 
 INSTALLERS = ['local', 'git']
 DEFUALT_DOCKER_SERVICES = ['worker', 'orthanc', 'mongo', 'dashboard', 'scheduler']
+ZIP_FILES = {
+  'application/zip': '.zip',
+  'application/gzip': '.gz',
+  'application/x-rar-compressed': '.rar',
+  'application/x-zip-compressed': '.zip',
+  'application/zip-compressed': '.zip',
+  'application/x-tar': '.tar',
+  'application/vnd.rar': '.rar'  
+}
+
+def getFilename_fromCd(cd):
+  """
+  Get filename from content-disposition
+  """
+  if not cd:
+    return None
+  
+  fname = re.findall('filename=(.+)', cd)
+  if len(fname) == 0:
+    return None
+  
+  return fname[0]
 
-def handle_installer(inst, question, baseDir, isWorker=False):
-  questions = []
-
-  if inst == "git":
-    questions.append(inq.Text("object_path", message=question + " (git url)"))
-
-    if isWorker:
-      questions.append(inq.Text("sub_path", message="Repository sub-folder", default="worker"))
+def handle_installer(args, inst, question, baseDir, isWorker=False):
+  if not args.non_interactive:  
+    questions = []
+
+    if inst == "git" or inst == "web":
+      questions.append(inq.Text("object_path", message=question + " (git/web url)"))
+      if isWorker:
+        questions.append(inq.Text("sub_path", message="Repository sub-folder", default="worker"))
+      else:
+        questions.append(inq.Text("sub_path", message="Repository sub-folder", default="service"))
     else:
-      questions.append(inq.Text("sub_path", message="Repository sub-folder", default="service"))
+      questions.append(inq.Path("object_path", message=question, exists=True, path_type=inq.Path.DIRECTORY, normalize_to_absolute_path=True))
 
+    answers = inq.prompt(questions)
+    object_path = answers['object_path']
+    sub_path = answers['sub_path']
   else:
-    questions.append(inq.Path("object_path", message=question, exists=True, path_type=inq.Path.DIRECTORY, normalize_to_absolute_path=True))
+    object_path = args.object_path
+    sub_path = './' if args.sub_path is None else args.sub_path
 
-  answers = inq.prompt(questions)
+    if args.git:
+      inst = "git"
+    elif args.web:
+      inst = "web"
+    else:
+      inst = "local"
 
   if inst == "git":
-    url = answers["object_path"]
+    url = object_path
     repo = git.Repo.clone_from(url, baseDir)
     repo.submodule_update()
 
-    return os.path.join(baseDir, answers["sub_path"])
+    return os.path.join(baseDir, sub_path)
+  
+  if inst == "web":
+    url = object_path
+    h = requests.head(url=url)
+    content_type = h.headers.get('content-type')
+    if content_type in ZIP_FILES:
+      filename = f"temp{ZIP_FILES.get(content_type)}"
+      r = requests.get(url, allow_redirects=True)
 
-  return answers["object_path"]
+      with open(os.path.join(baseDir, filename), 'wb') as down_file:
+        down_file.write(r.content)
 
-def parse_args():
-  parent_parser = argparse.ArgumentParser(description='A Command line tool for the dicom processor library', add_help=False)
-  parent_parser.add_argument('action', metavar='action', type=str, help='action to be performed, options [create, init, install, remove, backup, build]')
-  parent_parser.add_argument('object', metavar='object', type=str, help='action object, options [service, app]')
-  args = parent_parser.parse_args()
-  return args
+      shutil.unpack_archive(os.path.join(baseDir, filename), os.path.join(baseDir, 'source'))
+      objs = os.listdir(os.path.join(baseDir, 'source'))
+
+      if len(objs) == 1:
+        return os.path.join(baseDir, 'source', objs[0], sub_path) if not sub_path is None else os.path.join(baseDir, 'source', objs[0])
+      else:
+        return os.path.join(baseDir, 'source', sub_path) if not sub_path is None else os.path.join(baseDir, 'source')
+
+    else:
+      raise Exception('Wrong file format for installation!')
+
+  return object_path
 
 def main():
   args = parse_args()
   action = args.action
 
   action_lower = str(action).lower()
 
@@ -136,33 +185,42 @@
     create_service(args)
   if object_lower == "app":
     create_app(args)
   if object_lower == "worker":
     create_worker(args)
 
 def create_app(args):
-  questions = [
-    inq.Text("app_name", message="Enter app name"),
-    inq.Path("app_path", message="Enter app base folder", exists=True, path_type=inq.Path.DIRECTORY, normalize_to_absolute_path=True),
-    inq.Path("mapped_path", message="Enter app mapped folder base", exists=False, path_type=inq.Path.DIRECTORY, normalize_to_absolute_path=True),
-    inq.Text("dicom_port", message="Enter orthanc DICOM port", default="4242"),
-    inq.Text("browser_port", message="Enter orthanc browser port", default="8080"),
-    inq.Text("dashboard_port", message="Enter jobs dashboard port", default="5000"),
-    inq.Text("modality", message="Supported Modality (comma separated)", default="CT,MR"),
-  ]
-  
-  answers = inq.prompt(questions)
-  app_path = answers['app_path']
-  mapped_path = answers['mapped_path']
-  app_name = answers['app_name']
-  dicom_port = answers['dicom_port']
-  browser_port = answers['browser_port']
-  dashboard_port = answers['dashboard_port']
-
-  modality = answers['modality']
+  non_interactive = args.non_interactive
+  if not non_interactive:
+    questions = [
+      inq.Text("app_name", message="Enter app name"),
+      inq.Path("app_path", message="Enter app base folder", exists=True, path_type=inq.Path.DIRECTORY, normalize_to_absolute_path=True),
+      inq.Path("mapped_path", message="Enter app mapped folder base", exists=False, path_type=inq.Path.DIRECTORY, normalize_to_absolute_path=True),
+      inq.Text("dicom_port", message="Enter orthanc DICOM port", default="4242"),
+      inq.Text("browser_port", message="Enter orthanc browser port", default="8080"),
+      inq.Text("dashboard_port", message="Enter jobs dashboard port", default="5000"),
+      inq.Text("modality", message="Supported Modality (comma separated)", default="CT,MR"),
+    ]
+    
+    answers = inq.prompt(questions)
+    app_path = answers['app_path']
+    mapped_path = answers['mapped_path']
+    app_name = answers['app_name']
+    dicom_port = answers['dicom_port']
+    browser_port = answers['browser_port']
+    dashboard_port = answers['dashboard_port']
+    modality = answers['modality']
+  else:
+    app_path = args.app_path
+    mapped_path = args.mapped_path
+    app_name = args.app_name
+    dicom_port = args.dicom_port
+    browser_port = args.browser_port
+    dashboard_port = args.dashboard_port
+    modality = args.modality
 
   existing_apps = load_config("apps")
 
   if app_name in existing_apps:
     print(f"There exist a configured app with name '{app_name}'")
 
   base_path = os.path.abspath(os.path.join(app_path, app_name))
@@ -221,70 +279,90 @@
     
   dashboard_dir_full_path = os.path.join(mapped_folder, dashboard_dir)
   os.system(f"mkdir -p {dashboard_dir_full_path}")
   with open(os.path.join(dashboard_dir_full_path, "auth.json"), "w") as file:
     file.write(FILES.DASHBOARD_AUTH)
 
 def create_worker(args):
-  questions = [
-    inq.Text("worker_name", message="Enter worker name"),
-    inq.Path("worker_path", message="Enter workers folder", exists=True, path_type=inq.Path.DIRECTORY, normalize_to_absolute_path=True),
-    inq.Text("worker_base_image", message="Enter worker base image", default="ubuntu:18.04"),
-    inq.Text("worker_python_version", message="Enter worker python version", default="3.7"),
-    inq.Text("channels", message="Enter job channels (comma separated)", default="default"),
-    inq.Text("worker_description", message="Enter worker description"),
-  ]
+  if not args.non_interactive:
+    questions = [
+      inq.Text("worker_name", message="Enter worker name"),
+      inq.Path("worker_path", message="Enter workers folder", exists=True, path_type=inq.Path.DIRECTORY, normalize_to_absolute_path=True),
+      inq.Text("worker_base_image", message="Enter worker base image", default="ubuntu:18.04"),
+      inq.Text("worker_python_version", message="Enter worker python version", default="3.7"),
+      inq.Text("channels", message="Enter job channels (comma separated)", default="default"),
+      inq.Text("worker_description", message="Enter worker description"),
+    ]
 
-  answers = inq.prompt(questions)
-  worker_name = answers['worker_name']
-  python_version = answers['worker_python_version']
-  base_image = answers["worker_base_image"]
-  channels = answers["channels"]
+    answers = inq.prompt(questions)
+    worker_name = answers['worker_name']
+    worker_path = answers['worker_path']
+    python_version = answers['worker_python_version']
+    base_image = answers["worker_base_image"]
+    channels = answers["channels"]
+    worker_description = answers['worker_description']
+
+  else:
+    worker_name = args.worker_name
+    python_version = args.worker_python_version
+    base_image = args.worker_base_image
+    channels = args.channels
+    worker_path = args.worker_path
+    worker_description = args.worker_description
+    if channels is None: channels = worker_name
 
   worker_settings = {
     "name": worker_name,
+    "description": worker_description,
     "scripts": ["script.sh"],
     "entryScriptPaths": ["/scripts"],
     "baseImage": base_image,
     "environments": [
       {
         "name": "base",
         "requirements": ["requirements.txt"],
         "entryRequirementPaths": ["/requirements"],
         "channels": [s.strip() for s in str(channels).strip().split(",")],
         "pythonVersion": python_version
       }
     ]
   }
 
-  fullpath = os.path.join(answers['worker_path'], answers['worker_name'])
+  fullpath = os.path.join(worker_path, worker_name)
   os.system(f"mkdir -p {fullpath}")
   
   os.system(f"touch {os.path.join(fullpath, 'requirements.txt')}")
 
   files = {
     "settings.json": json.dumps(worker_settings, indent=2),
     "script.sh": "#!/bin/bash"
   }
 
   for fn in files:
     with open(os.path.join(fullpath, fn), 'w') as txt:
       txt.write(files[fn])
 
 def create_service(args):
-  questions = [
-    inq.Text("service_name", message="Enter service name"),
-    inq.Path("service_path", message="Enter service folder", exists=True, path_type=inq.Path.DIRECTORY, normalize_to_absolute_path=True),
-    inq.Text("service_description", message="Enter service description"),
-  ]
+  if not args.non_interactive:
+    questions = [
+      inq.Text("service_name", message="Enter service name"),
+      inq.Path("service_path", message="Enter service folder", exists=True, path_type=inq.Path.DIRECTORY, normalize_to_absolute_path=True),
+      inq.Text("service_description", message="Enter service description"),
+    ]
 
-  answers = inq.prompt(questions)
-  service_name = answers['service_name']
+    answers = inq.prompt(questions)
+    service_name = answers['service_name']
+    service_path = answers['service_path']
+    service_description = answers['service_description']
+  else:
+    service_name = args.service_name
+    service_path = args.service_path
+    service_description = args.service_description
 
-  fullpath = os.path.join(answers['service_path'], answers['service_name'])
+  fullpath = os.path.join(service_path, service_name)
   modulePath = os.path.join(fullpath, "module")
   registryPath = os.path.join(fullpath, "registry")
 
   os.system(f"mkdir -p {modulePath}")
   os.system(f"mkdir -p {registryPath}")
 
   os.system(f"echo 'from .main import callback' > {os.path.join(registryPath, '__init__.py')}")
@@ -323,15 +401,15 @@
       "worker": f"{service_name}.worker",
       "callback": f"{service_name}.callback",
       "dependsOn": None,
       "channel": "default",
       "timeout": "1h",
       "params": {},
       "sortPosition": 0,
-      "description": answers['service_description']
+      "description": service_description
     }
   ]
 
   with open(os.path.join(registryPath, 'main.py'), 'w') as txt:
     txt.writelines(callback_code)
 
   with open(os.path.join(registryPath, 'settings.json'), 'w') as txt:
@@ -349,30 +427,35 @@
 
 def init_app(args, app_name=None):
   existing_apps = load_config("apps")
 
   if len(existing_apps.keys()) == 0:
     print("There are no existing apps")
     return
-  
-  questions = [
-    inq.List("pull_images", message="Pull docker images ?", choices=["Yes", "No"]),
-  ]
 
-  if app_name is None:
+  if not args.non_interactive:  
     questions = [
-      inq.List("app_name", message="Select app to initial", choices=list(existing_apps.keys())),
-    ] + questions
+      inq.List("pull_images", message="Pull docker images ?", choices=["Yes", "No"]),
+    ]
+
+    if app_name is None:
+      questions = [
+        inq.List("app_name", message="Select app to initial", choices=list(existing_apps.keys())),
+      ] + questions
+
+      answers = inq.prompt(questions)
+      app_name = answers['app_name']
+      pull_images = answers['pull_images'] == 'Yes'
+    else:
+      answers = inq.prompt(questions)
+      pull_images = answers['pull_images'] == 'Yes'
 
-    answers = inq.prompt(questions)
-    app_name = answers['app_name']
-    pull_images = answers['pull_images'] == 'Yes'
   else:
-    answers = inq.prompt(questions)
-    pull_images = answers['pull_images'] == 'Yes'
+    app_name = args.app_name if app_name is None else app_name
+    pull_images = args.pull_images
 
 
   config = existing_apps.get(app_name)
 
   if config is None:
     print("Unable to load app configuration!")
     return
@@ -446,34 +529,44 @@
 
 def install_service(args):
   existing_apps = load_config("apps")
   if len(existing_apps.keys()) == 0:
     print("There are no existing apps")
     return
 
-  questions = [
-    inq.List("app_name", message="Select app to install service to", choices=list(existing_apps.keys())),
-    inq.Text("service_name", message="Enter service name"),
-    inq.List("inst_type", message="Select installer", choices=INSTALLERS)
-  ]
+  if not args.non_interactive:
+    questions = [
+      inq.List("app_name", message="Select app to install service to", choices=list(existing_apps.keys())),
+      inq.Text("service_name", message="Enter service name"),
+      inq.List("inst_type", message="Select installer", choices=INSTALLERS)
+    ]
 
-  answers = inq.prompt(questions)
-  app_name = answers['app_name']
-  service_name = answers['service_name']
-  inst_type = answers['inst_type']
+    answers = inq.prompt(questions)
+    app_name = answers['app_name']
+    service_name = answers['service_name']
+    inst_type = answers['inst_type']
+
+  else:
+    app_name = args.app_name
+    service_name = args.service_name
+    inst_type = "local"
+    if args.git:
+      inst_type = 'git'
+    elif args.web:
+      inst_type = 'web'
 
   with tempfile.TemporaryDirectory() as baseDir:
     config = existing_apps.get(app_name)
     services = config.get("services", {})
 
     if service_name in services:
       print(f"A service with name {service_name} already exists!")
       return
 
-    service_path = handle_installer(inst_type, "Enter service path", baseDir)
+    service_path = handle_installer(args, inst_type, "Enter service path", baseDir)
 
     if service_path is None:
       print("Unable install service!")
       return
 
     if config is None:
       print("Unable to load app configuration!")
@@ -495,15 +588,15 @@
 
     cwd = os.getcwd()
 
     os.chdir(os.path.abspath(os.path.join(base_dir)))
     os.system(f"bash service.sh install {service_name} -p {service_dir}")
 
     if inst_type != "local":
-      os.rmdir(service_dir)
+      shutil.rmtree(service_dir, ignore_errors=True)
 
     os.chdir(cwd)
 
     if not "services" in config:
       config["services"] = {}
     
     config["services"][service_name] = {
@@ -516,99 +609,144 @@
 
 def install_worker(args):
   existing_apps = load_config("apps")
   if len(existing_apps.keys()) == 0:
     print("There are no existing apps")
     return
 
-  questions = [
-    inq.List("app_name", message="Select app to install worker to", choices=list(existing_apps.keys())),
-    inq.Text("worker_name", message="Enter worker name"),
-    inq.List("inst_type", message="Select installer", choices=INSTALLERS),
-    inq.List("start_worker", message="Start worker after installation ?", choices=["Yes", "No"], default="No"),
-    inq.List("config_gpu", message="Configure GPU device reservation ?", choices=["Yes", "No"], default="No"),
-  ]
+  if not args.non_interactive:
+    questions = [
+      inq.List("app_name", message="Select app to install worker to", choices=list(existing_apps.keys())),
+      inq.Text("worker_name", message="Enter worker name"),
+      inq.List("inst_type", message="Select installer", choices=INSTALLERS),
+      inq.List("start_worker", message="Start worker after installation ?", choices=["Yes", "No"], default="No"),
+      inq.List("config_gpu", message="Configure GPU device reservation ?", choices=["Yes", "No"], default="No"),
+    ]
+
+    answers = inq.prompt(questions)
+    app_name = answers['app_name']
+    worker_name = answers['worker_name']
+    inst_type = answers['inst_type']
+    config_gpu = answers['config_gpu'] == "Yes"
+    start_worker_after_install = answers['start_worker'] == "Yes"
+  else:
+    app_name = args.app_name
+    worker_name = args.worker_name
+    inst_type = "local"
+    
+    if args.git: inst_type = "git"
+    if args.web: inst_type = "web"
+
+    config_gpu = args.gpu
+    start_worker_after_install = args.start_worker
 
-  answers = inq.prompt(questions)
-  app_name = answers['app_name']
-  worker_name = answers['worker_name']
-  inst_type = answers['inst_type']
-  config_gpu = answers['config_gpu']
-  start_worker_after_install = answers['start_worker']
   device_config = {}
 
   with tempfile.TemporaryDirectory() as baseDir:
-    worker_path = handle_installer(inst_type, "Enter worker path", baseDir, isWorker=True)
+    worker_path = handle_installer(args, inst_type, "Enter worker path", baseDir, isWorker=True)
 
-    if config_gpu == "Yes":
-      device_answers = inq.prompt([
-        inq.Text("device_cap", message="Enter device capabilities (comman separated list)", default="gpu"),
-        inq.Text("driver", message="Enter device driver", default="nvidia"),
-        inq.List("is_deviceid_or_count", message="How would you want to configure the reservation ?", choices=["Device Count", "Device ID"], default="Device Count"),
-      ])
-
-      caps = device_answers["device_cap"]
-      driv = device_answers["driver"]
-      is_dev_or_count = device_answers['is_deviceid_or_count']
-
-      caps = str(caps).split(",")
-
-      if len(caps) > 0:
-        device_config["capabilities"] = caps
-
-      if driv != "":
-        device_config["driver"] = driv  
-
-      if is_dev_or_count == "Device Count":
-        count_answers = inq.prompt([
-          inq.Text("count", message="Enter Device Count (integer) leave empty to use all devices"),
-          inq.Text("device_options", message="Enter driver specific options (comma seperated key:value pairs)"),
+    if config_gpu:
+      if not args.non_interactive:
+        device_answers = inq.prompt([
+          inq.Text("device_cap", message="Enter device capabilities (comman separated list)", default="gpu"),
+          inq.Text("driver", message="Enter device driver", default="nvidia"),
+          inq.List("is_deviceid_or_count", message="How would you want to configure the reservation ?", choices=["Device Count", "Device ID"], default="Device Count"),
         ])
 
-        cnt = count_answers["count"]
-        opts = count_answers["device_options"]
+        caps = device_answers["device_cap"]
+        driv = device_answers["driver"]
+        is_dev_or_count = device_answers['is_deviceid_or_count']
+
+        caps = str(caps).split(",")
+
+        if len(caps) > 0:
+          device_config["capabilities"] = caps
+
+        if driv != "":
+          device_config["driver"] = driv  
+
+        if is_dev_or_count == "Device Count":
+          count_answers = inq.prompt([
+            inq.Text("count", message="Enter Device Count (integer) leave empty to use all devices"),
+            inq.Text("device_options", message="Enter driver specific options (comma seperated key:value pairs)"),
+          ])
+
+          cnt = count_answers["count"]
+          opts = count_answers["device_options"]
+
+          if cnt != "":
+            device_config["count"] = int(cnt)
+          else:
+            device_config["count"] = "all"
+            
+          if opts != "":
+            opts = str(opts).split(",")         
+            for opt in opts:
+              keyval = opt.split(":")
+              if len(keyval) > 1:
+
+                if not "options" in device_config:
+                  device_config["options"] = {}
+                
+                device_config["options"][keyval[0]] = keyval[1]
 
-        if cnt != "":
-          device_config["count"] = int(cnt)
         else:
-          device_config["count"] = "all"
-          
-        if opts != "":
-          opts = str(opts).split(",")         
-          for opt in opts:
-            keyval = opt.split(":")
-            if len(keyval) > 1:
-
-              if not "options" in device_config:
-                device_config["options"] = {}
-              
-              device_config[keyval[0]] = keyval[1]
-
+          deviceid_answers = inq.prompt([
+            inq.Text("deviceids", message="Enter Device IDs (comman separated list)"),
+            inq.Text("device_options", message="Enter driver specific options (comma seperated key:value pairs)"),
+          ])
+
+          devids = deviceid_answers["deviceids"]
+          opts = deviceid_answers["device_options"]
+
+          if devids != "":
+            device_config["device_ids"] = str(devids).split(",")
+            
+          if opts != "":
+            opts = str(opts).split(",")         
+            for opt in opts:
+              keyval = opt.split(":")
+              if len(keyval) > 1:
+
+                if not "options" in device_config:
+                  device_config["options"] = {}
+                
+                device_config["options"][keyval[0]] = keyval[1]
       else:
-        deviceid_answers = inq.prompt([
-          inq.Text("deviceids", message="Enter Device IDs (comman separated list)"),
-          inq.Text("device_options", message="Enter driver specific options (comma seperated key:value pairs)"),
-        ])
+        caps = args.device_cap
+        driv = args.driver
+        is_dev_or_count = device_answers['is_deviceid_or_count']
+
+        caps = str(caps).split(",")
+
+        if len(caps) > 0:
+          device_config["capabilities"] = caps
+
+        if driv != "":
+          device_config["driver"] = driv
+
+        if not args.device_count is None:
+          device_config["count"] = int(args.device_count)
+        elif not args.device_id is None:
+          device_config["device_ids"] = str(args.device_id).split(",")
+        else:
+          device_config["count"] = 'all'
 
-        devids = deviceid_answers["deviceids"]
-        opts = deviceid_answers["device_options"]
+        opts = args.device_options
 
-        if devids != "":
-          device_config["device_ids"] = str(devids).split(",")
-          
         if opts != "":
           opts = str(opts).split(",")         
           for opt in opts:
             keyval = opt.split(":")
             if len(keyval) > 1:
 
               if not "options" in device_config:
                 device_config["options"] = {}
               
-              device_config[keyval[0]] = keyval[1]
+              device_config["options"][keyval[0]] = keyval[1]
 
     worker_name = str(worker_name).lower()
 
     if worker_name in DEFUALT_DOCKER_SERVICES:
       print(f"Worker name cannot be one of: {DEFUALT_DOCKER_SERVICES}")
       return
 
@@ -678,15 +816,15 @@
     if "image" in worker_settings:
       img = worker_settings.get("image")
 
       if not img is None:
         del docker_compose_config["build"]
         docker_compose_config["image"] = img
 
-    if config_gpu == "Yes" and "capabilities" in device_config:
+    if config_gpu and "capabilities" in device_config:
       docker_compose_config["deploy"] = {
         "resources": {
           "reservations": {
             "devices": [device_config]
           }
         }
       }
@@ -712,15 +850,15 @@
 
     cwd = os.getcwd()
     os.chdir(os.path.join(base_dir))
 
     if "build" in docker_compose_config:
       os.system(f"docker-compose build --force-rm {worker_name}")
 
-    if start_worker_after_install == "Yes":
+    if start_worker_after_install:
       os.system(f"docker-compose up -d {worker_name}")
 
     os.chdir(cwd)
 
 def __initialize_worker(base_path, settings):
   code_base_path = os.path.join(base_path)
 
@@ -759,27 +897,32 @@
 
 def remove_app(args):
   existing_apps = load_config("apps")
 
   if len(existing_apps.keys()) == 0:
     print("There are no existing apps")
     return
+  if not args.non_interactive:  
+    questions = [
+      inq.List("app_name", message="Select app to remove", choices=list(existing_apps.keys())),
+      inq.List("remove_base_dir", message="Remove app base directory ?", choices=["Yes", "No"]),
+      inq.List("remove_mapped_dir", message="Remove app mapped folders directory ?", choices=["Yes", "No"]),
+      inq.Text("backup_path", message="Enter backup folder (leave empty to skip backup)")
+    ]
 
-  questions = [
-    inq.List("app_name", message="Select app to remove", choices=list(existing_apps.keys())),
-    inq.List("remove_base_dir", message="Remove app base directory ?", choices=["Yes", "No"]),
-    inq.List("remove_mapped_dir", message="Remove app mapped folders directory ?", choices=["Yes", "No"]),
-    inq.Text("backup_path", message="Enter backup folder (leave empty to skip backup)")
-  ]
-
-  answers = inq.prompt(questions)
-  app_name = answers['app_name']
-  backup_path = answers['backup_path']
-  remove_base = answers['remove_base_dir']
-  remove_mapped = answers['remove_mapped_dir']
+    answers = inq.prompt(questions)
+    app_name = answers['app_name']
+    backup_path = answers['backup_path']
+    remove_base = answers['remove_base_dir'] == "Yes"
+    remove_mapped = answers['remove_mapped_dir'] == "Yes"
+  else:
+    app_name = args.app_name
+    backup_path = args.backup_path
+    remove_base = args.remove_data
+    remove_mapped = args.remove_data
 
   config = existing_apps.get(app_name)
 
   if config is None:
     print("Unable to load app configuration!")
     return
 
@@ -802,50 +945,56 @@
   if not os.path.isfile(env_file):
     print("Missing .env file!")
     return
 
   dotenv.load_dotenv(os.path.abspath(os.path.join(base_dir, '.env')))
   mapped_folder = os.environ.get("BASEDIR")
 
-  if backup_path != "":
+  if (not backup_path is None) and backup_path != "":
     backup_dir = os.path.abspath(backup_path)
     os.system(f"mkdir -p {backup_dir}")
     os.system(f"cp -r {os.path.abspath(os.path.join(base_dir))} {os.path.join(backup_dir, app_name)}")
 
     if not mapped_folder is None:
       os.system(f"cp -r {os.path.abspath(mapped_folder)} {os.path.join(backup_dir, app_name, 'mapped_folder')}")
 
   cwd = os.getcwd()
 
   os.chdir(os.path.abspath(os.path.join(base_dir)))
   os.system(f"bash clean.sh")
   os.chdir(cwd)
 
-  if remove_base == "Yes":
+  if remove_base:
     os.system(f"rm -rf {os.path.abspath(os.path.join(base_dir))}")
   
-  if remove_mapped == "Yes":
+  if remove_mapped:
     os.system(f"rm -rf {os.path.abspath(os.path.join(mapped_folder))}")
 
 def remove_service(args):
   existing_apps = load_config("apps")
   if len(existing_apps.keys()) == 0:
     print("There are no existing apps")
     return
 
-  questions = [
-    inq.List("app_name", message="Select app to remove service from", choices=list(existing_apps.keys())),
-    inq.Text("service_name", message="Enter service name"),
-    inq.Text("backup_path", message="Enter backup folder (leave empty to skip backup)")
-  ]
+  if not args.non_interactive:
+    questions = [
+      inq.List("app_name", message="Select app to remove service from", choices=list(existing_apps.keys())),
+      inq.Text("service_name", message="Enter service name"),
+      inq.Text("backup_path", message="Enter backup folder (leave empty to skip backup)")
+    ]
+
+    answers = inq.prompt(questions)
+    app_name = answers['app_name']
+    service_name = answers['service_name']
+    service_path = answers['backup_path']
+  else:
+    app_name = args.app_name
+    service_name = args.service_name
+    service_path = args.backup_path
 
-  answers = inq.prompt(questions)
-  app_name = answers['app_name']
-  service_name = answers['service_name']
-  service_path = answers['backup_path']
 
   config = existing_apps.get(app_name)
   services = config.get("services", {})
 
   if not service_name in services:
     print(f"There is no service with name {service_name}!")
     return
@@ -867,15 +1016,15 @@
     return
 
   
 
   cwd = os.getcwd()
   os.chdir(os.path.abspath(os.path.join(base_dir)))
 
-  if service_path != "":
+  if (not service_path is None) and  service_path != "":
     service_dir = os.path.abspath(service_path)
     os.system(f"bash service.sh remove {service_name} -b {service_dir}")
   else:
     os.system(f"bash service.sh remove {service_name}")
 
   os.chdir(cwd)
 
@@ -886,24 +1035,30 @@
 
 def remove_worker(args):
   existing_apps = load_config("apps")
   if len(existing_apps.keys()) == 0:
     print("There are no existing apps")
     return
 
-  questions = [
-    inq.List("app_name", message="Select app to remove worker from", choices=list(existing_apps.keys())),
-    inq.Text("worker_name", message="Enter worker name")
-  ]
+  if not args.non_interactive:
+    questions = [
+      inq.List("app_name", message="Select app to remove worker from", choices=list(existing_apps.keys())),
+      inq.Text("worker_name", message="Enter worker name")
+    ]
+
+    answers = inq.prompt(questions)
+    app_name = answers['app_name']
+    worker_name = answers['worker_name']
+  else:
+    app_name = args.app_name
+    worker_name = args.worker_name
 
-  answers = inq.prompt(questions)
-  app_name = answers['app_name']
-  worker_name = answers['worker_name']
   worker_name = str(worker_name).lower()
 
+
   config = existing_apps.get(app_name)
 
   if config is None:
     print("Unable to load app configuration!")
     return
 
   base_dir = config.get("base_dir")
@@ -913,15 +1068,14 @@
     return
 
   existing_workers = config.get("workers")
   if not worker_name in existing_workers:
     print(f"Worker with name {worker_name} does not exist!")
     return
 
-
   cwd = os.getcwd()
   os.chdir(os.path.join(base_dir))
   os.system(f"docker-compose rm -f -s {worker_name}")
   _, image_base = os.path.split(base_dir)
   os.system(f"docker rmi {image_base}_{worker_name}")
   os.system(f"rm -rf {os.path.join(base_dir, 'workers', worker_name)}")
   os.chdir(cwd)
@@ -948,32 +1102,38 @@
 
 def handle_backup(args):
   object_lower = str(args.object).lower()
   if object_lower == "service":
     backup_service(args)
   if object_lower == "app":
     backup_app(args)
+  if object_lower == "worker":
+    backup_worker(args)
 
 def backup_service(args):
   existing_apps = load_config("apps")
 
   if len(existing_apps.keys()) == 0:
     print("There are no existing apps")
     return
+  if not args.non_interactive:
+    questions = [
+      inq.List("app_name", message="Select app to backup service", choices=list(existing_apps.keys())),
+      inq.Text("service_name", message="Enter service name"),
+      inq.Text("backup_path", message="Enter backup folder")
+    ]
 
-  questions = [
-    inq.List("app_name", message="Select app to backup service", choices=list(existing_apps.keys())),
-    inq.Text("service_name", message="Enter service name"),
-    inq.Text("backup_path", message="Enter backup folder")
-  ]
-
-  answers = inq.prompt(questions)
-  app_name = answers['app_name']
-  service_name = answers['service_name']
-  service_path = answers['backup_path']
+    answers = inq.prompt(questions)
+    app_name = answers['app_name']
+    service_name = answers['service_name']
+    service_path = answers['backup_path']
+  else:
+    app_name = args.app_name
+    service_name = args.service_name
+    service_path = args.backup_path
 
   config = existing_apps.get(app_name)
 
   if config is None:
     print("Unable to load app configuration!")
     return
 
@@ -1002,24 +1162,29 @@
 def backup_worker(args):
   existing_apps = load_config("apps")
 
   if len(existing_apps.keys()) == 0:
     print("There are no existing apps")
     return
 
-  questions = [
-    inq.List("app_name", message="Select app to backup worker", choices=list(existing_apps.keys())),
-    inq.Text("worker_name", message="Enter worker name"),
-    inq.Text("backup_path", message="Enter backup folder")
-  ]
+  if not args.non_interactive:  
+    questions = [
+      inq.List("app_name", message="Select app to backup worker", choices=list(existing_apps.keys())),
+      inq.Text("worker_name", message="Enter worker name"),
+      inq.Text("backup_path", message="Enter backup folder")
+    ]
 
-  answers = inq.prompt(questions)
-  app_name = answers['app_name']
-  worker_name = answers['worker_name']
-  backup_path = answers['backup_path']
+    answers = inq.prompt(questions)
+    app_name = answers['app_name']
+    worker_name = answers['worker_name']
+    backup_path = answers['backup_path']
+  else:
+    app_name = args.app_name
+    worker_name = args.worker_name
+    backup_path = args.backup_path
 
   worker_name = str(worker_name).lower()
 
   config = existing_apps.get(app_name)
 
   if config is None:
     print("Unable to load app configuration!")
@@ -1061,23 +1226,26 @@
 
 def backup_app(args):
   existing_apps = load_config("apps")
 
   if len(existing_apps.keys()) == 0:
     print("There are no existing apps")
     return
+  if not args.non_interactive:
+    questions = [
+      inq.List("app_name", message="Select app to backup", choices=list(existing_apps.keys())),
+      inq.Text("backup_path", message="Enter backup folder")
+    ]
 
-  questions = [
-    inq.List("app_name", message="Select app to backup", choices=list(existing_apps.keys())),
-    inq.Text("backup_path", message="Enter backup folder")
-  ]
-
-  answers = inq.prompt(questions)
-  app_name = answers['app_name']
-  backup_path = answers['backup_path']
+    answers = inq.prompt(questions)
+    app_name = answers['app_name']
+    backup_path = answers['backup_path']
+  else:
+    app_name = args.app_name
+    backup_path = args.backup_path
 
   config = existing_apps.get(app_name)
 
   if config is None:
     print("Unable to load app configuration!")
     return
 
@@ -1111,23 +1279,26 @@
     start_app(args)
 
 def start_app(args, app_name=None):
   existing_apps = load_config("apps")
 
   if len(existing_apps.keys()) == 0:
     print("There are no existing apps")
-    return
-
+    return 
+   
   if app_name is None:
-    questions = [
-      inq.List("app_name", message="Select app to start", choices=list(existing_apps.keys())),
-    ]
+    if not args.non_interactive:
+      questions = [
+        inq.List("app_name", message="Select app to start", choices=list(existing_apps.keys())),
+      ]
 
-    answers = inq.prompt(questions)
-    app_name = answers['app_name']
+      answers = inq.prompt(questions)
+      app_name = answers['app_name']
+    else:
+      app_name = args.app_name
 
   config = existing_apps.get(app_name)
 
   if config is None:
     print("Unable to load app configuration!")
     return
 
@@ -1160,20 +1331,23 @@
   existing_apps = load_config("apps")
 
   if len(existing_apps.keys()) == 0:
     print("There are no existing apps")
     return
 
   if app_name is None:
-    questions = [
-      inq.List("app_name", message="Select app to start", choices=list(existing_apps.keys())),
-    ]
+    if not args.non_interactive:
+      questions = [
+        inq.List("app_name", message="Select app to start", choices=list(existing_apps.keys())),
+      ]
 
-    answers = inq.prompt(questions)
-    app_name = answers['app_name']
+      answers = inq.prompt(questions)
+      app_name = answers['app_name']
+    else:
+      app_name = args.app_name
 
   config = existing_apps.get(app_name)
 
   if config is None:
     print("Unable to load app configuration!")
     return
 
@@ -1193,34 +1367,36 @@
 
   os.chdir(os.path.join(base_dir))
   os.system(f"bash stop.sh")
   os.chdir(os.path.join(cwd))
 
 
 
-
 def handle_restart(args):
   object_lower = str(args.object).lower()
   if object_lower == "app":
     restart_app(args)
 
 def restart_app(args, app_name=None):
   existing_apps = load_config("apps")
 
   if len(existing_apps.keys()) == 0:
     print("There are no existing apps")
     return
 
   if app_name is None:
-    questions = [
-      inq.List("app_name", message="Select app to start", choices=list(existing_apps.keys())),
-    ]
+    if not args.non_interactive:
+      questions = [
+        inq.List("app_name", message="Select app to start", choices=list(existing_apps.keys())),
+      ]
 
-    answers = inq.prompt(questions)
-    app_name = answers['app_name']
+      answers = inq.prompt(questions)
+      app_name = answers['app_name']
+    else:
+      app_name = args.app_name
 
   config = existing_apps.get(app_name)
 
   if config is None:
     print("Unable to load app configuration!")
     return
 
@@ -1245,44 +1421,55 @@
 
 
 
 def handle_set(args):
   object_lower = str(args.object).lower()
   if object_lower == "proxy":
     set_proxy(args)
+  if object_lower == "trusted-hosts":
+    set_trusted_hosts(args)
   
 def set_proxy(args):
-  questions = [
-    inq.Text("http_proxy", message="Enter http proxy"),
-    inq.Text("https_proxy", message="Enter https proxy"),
-    inq.Text("ftp_proxy", message="Enter ftp proxy"),
-    inq.Text("no_proxy", message="Enter no proxy urls (comma separated)"),
-  ]
+  if not args.non_interactive:
+    questions = [
+      inq.Text("http_proxy", message="Enter http proxy"),
+      inq.Text("https_proxy", message="Enter https proxy"),
+      inq.Text("ftp_proxy", message="Enter ftp proxy"),
+      inq.Text("no_proxy", message="Enter no proxy urls (comma separated)"),
+    ]
 
-  answers = inq.prompt(questions)
-  
-  p_settings = {
-    "http_proxy": answers["http_proxy"],
-    "https_proxy": answers["https_proxy"],
-    "ftp_proxy": answers["ftp_proxy"],
-    "no_proxy": answers["no_proxy"],
-  }
+    answers = inq.prompt(questions)
+    p_settings = {
+      "http_proxy": answers["http_proxy"],
+      "https_proxy": answers["https_proxy"],
+      "ftp_proxy": answers["ftp_proxy"],
+      "no_proxy": answers["no_proxy"],
+    }
+  else:
+    p_settings = {}
+    if not args.http_proxy is None: p_settings["http_proxy"] = args.http_proxy
+    if not args.https_proxy is None: p_settings["https_proxy"] = args.https_proxy
+    if not args.ftp_proxy is None: p_settings["ftp_proxy"] = args.ftp_proxy
+    if not args.no_proxy is None: p_settings["no_proxy"] = args.no_proxy
 
   update_config("proxies", p_settings)
   print("Proxy settings updated!")
   
 def set_trusted_hosts(args):
-  questions = [
-    inq.Text("trusted_hosts", message="Enter pip trusted hosts"),
-  ]
+  if not args.non_interactive:
+    questions = [
+      inq.Text("trusted_hosts", message="Enter pip trusted hosts"),
+    ]
 
-  answers = inq.prompt(questions)
+    answers = inq.prompt(questions)
   
-  th = answers["trusted_hosts"]
-  th = str(th).split(",")
+    th = answers["trusted_hosts"]
+    th = str(th).split(",")
+  else:
+    th = args.host
   
   update_config("trusted_hosts", th)
   print("Trusted hosts updated!")
 
 
 def handle_list(args):
   object_lower = str(args.object).lower()
@@ -1303,21 +1490,26 @@
 
 def list_services(args):
   existing_apps = load_config("apps")
 
   if len(existing_apps.keys()) == 0:
     print("There are no existing apps")
     return
+  if not args.non_interactive:
+    questions = [
+      inq.List("app_name", message="Select application", choices=list(existing_apps.keys())),
+    ]
 
-  questions = [
-    inq.List("app_name", message="Select application", choices=list(existing_apps.keys())),
-  ]
-
-  answers = inq.prompt(questions)
-  app_name = answers['app_name']
+    answers = inq.prompt(questions)
+    app_name = answers['app_name']
+  else:
+    app_name = args.app_name
+    if not app_name in existing_apps:
+      print(f"There exist no app with name {app_name}")
+      return
 
   config = existing_apps.get(app_name)
   services = config.get("services", {})
 
   print(f"List of services for {app_name}")
   print("--------------------------------------------------------")
 
@@ -1330,20 +1522,27 @@
 def list_workers(args):
   existing_apps = load_config("apps")
 
   if len(existing_apps.keys()) == 0:
     print("There are no existing apps")
     return
 
-  questions = [
-    inq.List("app_name", message="Select application", choices=list(existing_apps.keys())),
-  ]
+  if not args.non_interactive:
+    questions = [
+      inq.List("app_name", message="Select application", choices=list(existing_apps.keys())),
+    ]
+
+    answers = inq.prompt(questions)
+    app_name = answers['app_name']
+  else:
+    app_name = args.app_name
+    if not app_name in existing_apps:
+      print(f"There exist no app with name {app_name}")
+      return
 
-  answers = inq.prompt(questions)
-  app_name = answers['app_name']
 
   config = existing_apps.get(app_name)
   workers = config.get("workers", {})
 
   print(f"List of workers for {app_name}")
   print("--------------------------------------------------------")
```

### Comparing `dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar` & `dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar` & `dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py` & `dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar` & `dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script` & `dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar` & `dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar` & `dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py` & `dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar` & `dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar` & `dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar` & `dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/util.jar` & `dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/util.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/services/base/module/DicomAnonymizerService/utils.py` & `dcm-processor-1.0.0/dcm_processor/services/base/module/DicomAnonymizerService/utils.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/services/base/module/storageManager/lib.py` & `dcm-processor-1.0.0/dcm_processor/services/base/module/storageManager/lib.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/services/base/module/storageManager/main.py` & `dcm-processor-1.0.0/dcm_processor/services/base/module/storageManager/main.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/services/base/module/systemcleaner/main.py` & `dcm-processor-1.0.0/dcm_processor/services/base/module/systemcleaner/main.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/services/dcm2nii/module/__init__.py` & `dcm-processor-1.0.0/dcm_processor/services/dcm2nii/module/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,52 +12,59 @@
     data = json.load(jsfile)
   return data
 
 def worker(jobName, headers, params, added_params, **kwargs):
   a_params = added_params.get(jobName)
   
   if (not DATA is None) and (not a_params is None):
-    if "conversions" in a_params:
-      conversions = a_params.get("conversions", {})
-      for k in conversions.keys():
-        info = conversions.get(k, {})    
-        base = info.get("base")
-        filename = info.get("filename")
-        ext = info.get("ext", ".nii.gz")
+    if "outputs" in a_params:
+      outputs = a_params.get("outputs", {})
+      for k in outputs.keys():
+        nifti_info = outputs.get(k, {}).get("nifti", {})
+        json_info = outputs.get(k, {}).get("json", {})
+        
+        nifti_base = nifti_info.get("base")
+        nifti_filename = nifti_info.get("filename")
+        nifti_ext = nifti_info.get("ext", ".nii.gz")
+
+        json_base = json_info.get("base")
+        json_filename = json_info.get("filename")
+        json_ext = json_info.get("ext", ".json")
+
         dcmpath = headers.get("dcmpath")
 
-        if (not base is None) and (not filename is None) and (not dcmpath is None):
+        if (not nifti_base is None) and (not nifti_filename is None) and (not dcmpath is None):
           dcm2niix = os.path.join(dir_path, "dcm2niix")
-          fullbase = os.path.join(DATA, base)
-          tmpfolder = os.path.join(fullbase, filename)
+          fullbase = os.path.join(DATA, nifti_base)
+          tmpfolder = os.path.join(fullbase, nifti_filename)
           fulldcmpath = os.path.join(DATA, dcmpath, k)
-          command = f"{dcm2niix} -z y -b y -f {filename} -o {tmpfolder} {fulldcmpath}"
+          command = f"{dcm2niix} -z y -b y -f {nifti_filename} -o {tmpfolder} {fulldcmpath}"
           os.system(f"mkdir -p {tmpfolder}")
           os.system(command)
           selected_file = get_max_file(tmpfolder)
           dcm2niix_json_data = {}
           if not selected_file is None:
-            fullFilename = f"{filename}{ext}"
-            json_filename = str(selected_file).strip().replace(".nii.gz", ".json")
+            fullFilename = f"{nifti_filename}{nifti_ext}"
+            selected_file_json = str(selected_file).strip().replace(".nii.gz", ".json")
           
-            if os.path.isfile(json_filename):
-              dcm2niix_json_data = load_json(json_filename)
+            if os.path.isfile(selected_file_json):
+              dcm2niix_json_data = load_json(selected_file_json)
 
             os.system(f"mv {selected_file} {os.path.join(fullbase, fullFilename)}")
             os.system(f"rm -rf {tmpfolder}")
           
           searchText = os.path.join(fulldcmpath, "*.dcm")
           filenames = glob.glob(searchText)
 
           if len(filenames) > 0:
             dcmElem = pydicom.dcmread(filenames[0])
             json_dict = get_dicom_tags(dcmElem)
             json_dict.update(dcm2niix_json_data)
             json_dict = remove_strange_tags(json_dict)
-            with open(os.path.join(fullbase, f"{filename}.json"), "w") as outfile:
+            with open(os.path.join(DATA, json_base, f"{json_filename}{json_ext}"), "w") as outfile:
               json.dump(json_dict, outfile, cls=BytesEncoder, indent=4, sort_keys=True)
 
 def get_dicom_tags(dcmElem: pydicom.Dataset, excTags=None):
   baseTypes = [bytes, float, int, list, str]
   convertTypes = {
     pydicom.uid.UID: str,
     pydicom.valuerep.DSfloat: float,
```

### Comparing `dcm-processor-0.9.9/dcm_processor/services/dcm2nii/module/dcm2niix` & `dcm-processor-1.0.0/dcm_processor/services/dcm2nii/module/dcm2niix`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor/services/dcm2nii/registry/__init__.py` & `dcm-processor-1.0.0/dcm_processor/services/dcm2nii/registry/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,23 +3,34 @@
 def callback(jobName, headers, params, added_params, **kwargs):
   injected_params = {}
   has_items = False
   
   if "seriesIds" in headers:
     seriesIds = headers.get("seriesIds", [])
     baseDir = os.path.join("nifti", headers.get("id"))
-    injected_params["conversions"] = {}
+    injected_params["outputs"] = {}
     for seriesId in seriesIds:
-      out_params = {
-        "output": os.path.join(baseDir, f"{seriesId}.nii.gz"),
+
+      nifti_params = {
+        "type": "nifti",
+        "path": os.path.join(baseDir, f"{seriesId}.nii.gz"),
         "base": baseDir,
         "filename": f"{seriesId}",
         "ext": ".nii.gz"
       }
-      injected_params["conversions"][f"{seriesId}"] = out_params
+
+      json_params = {
+        "type": "json",
+        "path": os.path.join(baseDir, f"{seriesId}.json"),
+        "base": baseDir,
+        "filename": f"{seriesId}",
+        "ext": ".json"
+      }
+      
+      injected_params["outputs"][f"{seriesId}"] = { "nifti": nifti_params, "json": json_params }
       has_items = True
 
   if not params is None:
     clean = params.get("clean", False)
     if clean and has_items:
       injected_params['deleted'] = [baseDir]
```

### Comparing `dcm-processor-0.9.9/dcm_processor/worker.py` & `dcm-processor-1.0.0/dcm_processor/worker.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-0.9.9/dcm_processor.egg-info/SOURCES.txt` & `dcm-processor-1.0.0/dcm_processor.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE
-README.md
 pyproject.toml
 setup.cfg
 setup.py
 dcm_processor/__init__.py
+dcm_processor/argparser.py
 dcm_processor/files.py
 dcm_processor/script.py
 dcm_processor/worker.py
 dcm_processor.egg-info/PKG-INFO
 dcm_processor.egg-info/SOURCES.txt
 dcm_processor.egg-info/dependency_links.txt
 dcm_processor.egg-info/entry_points.txt
```

### Comparing `dcm-processor-0.9.9/setup.cfg` & `dcm-processor-1.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dcm-processor
-version = 0.9.9
+version = 1.0.0
 author = Giles Tetteh
 author_email = giles.tetteh@tum.de
 description = A Command line tool for the dicom processor library
 url = https://github.com/giesekow/dcm-processor-cli
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE
@@ -26,14 +26,15 @@
 install_requires = 
 	python-dotenv
 	inquirer
 	docker-compose
 	PyYAML
 	GitPython
 	ruamel_yaml
+	requests
 
 [options.entry_points]
 console_scripts = 
 	dcm-processor = dcm_processor:main
 
 [options.package_data]
 * = *.md
```

