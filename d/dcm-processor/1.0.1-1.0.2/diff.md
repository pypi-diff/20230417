# Comparing `tmp/dcm-processor-1.0.1.tar.gz` & `tmp/dcm-processor-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcm-processor-1.0.1.tar", last modified: Mon Apr 17 10:00:22 2023, max compression
+gzip compressed data, was "dcm-processor-1.0.2.tar", last modified: Mon Apr 17 10:46:55 2023, max compression
```

## Comparing `dcm-processor-1.0.1.tar` & `dcm-processor-1.0.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:00:22.025366 dcm-processor-1.0.1/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1074 2021-05-11 10:55:48.000000 dcm-processor-1.0.1/LICENSE
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6065 2023-04-17 10:00:22.025684 dcm-processor-1.0.1/PKG-INFO
--rwxr-xr-x   0 giles     (1000) giles     (1000)     5564 2023-04-17 09:57:36.000000 dcm-processor-1.0.1/README.md
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:00:21.816222 dcm-processor-1.0.1/dcm_processor/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       61 2021-10-17 14:30:50.000000 dcm-processor-1.0.1/dcm_processor/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    15407 2023-04-15 09:02:58.000000 dcm-processor-1.0.1/dcm_processor/argparser.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    33004 2023-04-14 11:38:11.000000 dcm-processor-1.0.1/dcm_processor/files.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    45684 2023-04-13 10:23:49.000000 dcm-processor-1.0.1/dcm_processor/script.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:00:21.794969 dcm-processor-1.0.1/dcm_processor/services/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:00:21.794400 dcm-processor-1.0.1/dcm_processor/services/base/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:00:21.850890 dcm-processor-1.0.1/dcm_processor/services/base/module/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:00:21.938679 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/
--rwxr-xr-x   0 giles     (1000) giles     (1000)   642195 2021-10-17 16:16:14.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)    17869 2021-10-17 16:16:15.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)      526 2023-04-06 14:13:53.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1551 2023-03-31 12:36:10.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    69564 2021-10-17 16:16:15.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:00:21.951320 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/config/
--rwxr-xr-x   0 giles     (1000) giles     (1000)    59497 2021-10-17 16:16:15.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script
--rwxr-xr-x   0 giles     (1000) giles     (1000)      248 2021-10-17 16:16:15.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/config/hash_table.csv
--rwxr-xr-x   0 giles     (1000) giles     (1000)       86 2021-10-17 16:16:15.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/config/psudonyms.csv
--rwxr-xr-x   0 giles     (1000) giles     (1000)    10424 2021-10-17 16:16:15.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   863881 2021-10-17 16:16:16.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)     3471 2023-03-31 12:35:15.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)  1172845 2021-10-17 16:16:18.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   391834 2021-10-17 16:16:19.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)    28241 2021-10-17 16:16:19.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   338969 2021-10-17 16:16:20.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/util.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1777 2023-03-31 20:09:03.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/utils.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)       26 2021-10-17 16:16:20.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/requirements.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       72 2021-10-17 16:16:20.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/script.sh
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:00:21.977162 dcm-processor-1.0.1/dcm_processor/services/base/module/storageManager/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/storageManager/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)       97 2021-10-17 16:16:20.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/storageManager/header_codes.json
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6218 2023-01-31 18:15:24.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/storageManager/lib.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    10012 2023-01-31 18:15:43.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/storageManager/main.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:00:21.983667 dcm-processor-1.0.1/dcm_processor/services/base/module/systemcleaner/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/systemcleaner/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     3806 2023-04-01 16:24:05.000000 dcm-processor-1.0.1/dcm_processor/services/base/module/systemcleaner/main.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:00:21.988628 dcm-processor-1.0.1/dcm_processor/services/base/registry/
--rwxr-xr-x   0 giles     (1000) giles     (1000)      443 2021-10-17 16:16:20.000000 dcm-processor-1.0.1/dcm_processor/services/base/registry/__init__.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:00:21.796056 dcm-processor-1.0.1/dcm_processor/services/dcm2nii/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:00:22.020178 dcm-processor-1.0.1/dcm_processor/services/dcm2nii/module/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     4030 2023-04-14 14:47:11.000000 dcm-processor-1.0.1/dcm_processor/services/dcm2nii/module/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)  1948128 2023-03-02 19:03:11.000000 dcm-processor-1.0.1/dcm_processor/services/dcm2nii/module/dcm2niix
--rwxr-xr-x   0 giles     (1000) giles     (1000)      406 2023-03-24 20:50:04.000000 dcm-processor-1.0.1/dcm_processor/services/dcm2nii/module/lib.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:00:22.024162 dcm-processor-1.0.1/dcm_processor/services/dcm2nii/registry/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1013 2023-04-14 12:17:35.000000 dcm-processor-1.0.1/dcm_processor/services/dcm2nii/registry/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)      285 2023-04-01 13:10:09.000000 dcm-processor-1.0.1/dcm_processor/services/dcm2nii/registry/settings.json
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6601 2023-02-01 11:09:28.000000 dcm-processor-1.0.1/dcm_processor/worker.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:00:21.843164 dcm-processor-1.0.1/dcm_processor.egg-info/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6065 2023-04-17 10:00:21.000000 dcm-processor-1.0.1/dcm_processor.egg-info/PKG-INFO
--rwxr-xr-x   0 giles     (1000) giles     (1000)     2368 2023-04-17 10:00:21.000000 dcm-processor-1.0.1/dcm_processor.egg-info/SOURCES.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)        1 2023-04-17 10:00:21.000000 dcm-processor-1.0.1/dcm_processor.egg-info/dependency_links.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       53 2023-04-17 10:00:21.000000 dcm-processor-1.0.1/dcm_processor.egg-info/entry_points.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       76 2023-04-17 10:00:21.000000 dcm-processor-1.0.1/dcm_processor.egg-info/requires.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       14 2023-04-17 10:00:21.000000 dcm-processor-1.0.1/dcm_processor.egg-info/top_level.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       89 2021-10-17 14:23:09.000000 dcm-processor-1.0.1/pyproject.toml
--rwxr-xr-x   0 giles     (1000) giles     (1000)      980 2023-04-17 10:00:22.027285 dcm-processor-1.0.1/setup.cfg
--rwxr-xr-x   0 giles     (1000) giles     (1000)      109 2021-10-17 19:37:23.000000 dcm-processor-1.0.1/setup.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:55.093347 dcm-processor-1.0.2/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1074 2021-05-11 10:55:48.000000 dcm-processor-1.0.2/LICENSE
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-04-17 10:46:55.093894 dcm-processor-1.0.2/PKG-INFO
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     5834 2023-04-17 10:06:58.000000 dcm-processor-1.0.2/README.md
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:54.828586 dcm-processor-1.0.2/dcm_processor/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       61 2021-10-17 14:30:50.000000 dcm-processor-1.0.2/dcm_processor/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    15407 2023-04-15 09:02:58.000000 dcm-processor-1.0.2/dcm_processor/argparser.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    33004 2023-04-14 11:38:11.000000 dcm-processor-1.0.2/dcm_processor/files.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    45679 2023-04-17 10:31:24.000000 dcm-processor-1.0.2/dcm_processor/script.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:54.778662 dcm-processor-1.0.2/dcm_processor/services/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:54.776954 dcm-processor-1.0.2/dcm_processor/services/base/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:54.875309 dcm-processor-1.0.2/dcm_processor/services/base/module/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:54.994779 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   642195 2021-10-17 16:16:14.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    17869 2021-10-17 16:16:15.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      526 2023-04-06 14:13:53.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1551 2023-03-31 12:36:10.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    69564 2021-10-17 16:16:15.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:55.015758 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/config/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    59497 2021-10-17 16:16:15.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      248 2021-10-17 16:16:15.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/config/hash_table.csv
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       86 2021-10-17 16:16:15.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/config/psudonyms.csv
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    10424 2021-10-17 16:16:15.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   863881 2021-10-17 16:16:16.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     3471 2023-03-31 12:35:15.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)  1172845 2021-10-17 16:16:18.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   391834 2021-10-17 16:16:19.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    28241 2021-10-17 16:16:19.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)   338969 2021-10-17 16:16:20.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/util.jar
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1777 2023-03-31 20:09:03.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/utils.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       26 2021-10-17 16:16:20.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/requirements.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       72 2021-10-17 16:16:20.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/script.sh
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:55.028789 dcm-processor-1.0.2/dcm_processor/services/base/module/storageManager/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/storageManager/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       97 2021-10-17 16:16:20.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/storageManager/header_codes.json
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6218 2023-01-31 18:15:24.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/storageManager/lib.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)    10012 2023-01-31 18:15:43.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/storageManager/main.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:55.036364 dcm-processor-1.0.2/dcm_processor/services/base/module/systemcleaner/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/systemcleaner/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     3806 2023-04-01 16:24:05.000000 dcm-processor-1.0.2/dcm_processor/services/base/module/systemcleaner/main.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:55.040232 dcm-processor-1.0.2/dcm_processor/services/base/registry/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      443 2021-10-17 16:16:20.000000 dcm-processor-1.0.2/dcm_processor/services/base/registry/__init__.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:54.793572 dcm-processor-1.0.2/dcm_processor/services/dcm2nii/
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:55.080412 dcm-processor-1.0.2/dcm_processor/services/dcm2nii/module/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     4030 2023-04-14 14:47:11.000000 dcm-processor-1.0.2/dcm_processor/services/dcm2nii/module/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)  1948128 2023-03-02 19:03:11.000000 dcm-processor-1.0.2/dcm_processor/services/dcm2nii/module/dcm2niix
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      406 2023-03-24 20:50:04.000000 dcm-processor-1.0.2/dcm_processor/services/dcm2nii/module/lib.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:55.090362 dcm-processor-1.0.2/dcm_processor/services/dcm2nii/registry/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     1013 2023-04-14 12:17:35.000000 dcm-processor-1.0.2/dcm_processor/services/dcm2nii/registry/__init__.py
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      285 2023-04-01 13:10:09.000000 dcm-processor-1.0.2/dcm_processor/services/dcm2nii/registry/settings.json
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6601 2023-02-01 11:09:28.000000 dcm-processor-1.0.2/dcm_processor/worker.py
+drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-04-17 10:46:54.860542 dcm-processor-1.0.2/dcm_processor.egg-info/
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-04-17 10:46:53.000000 dcm-processor-1.0.2/dcm_processor.egg-info/PKG-INFO
+-rwxr-xr-x   0 giles     (1000) giles     (1000)     2368 2023-04-17 10:46:54.000000 dcm-processor-1.0.2/dcm_processor.egg-info/SOURCES.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)        1 2023-04-17 10:46:53.000000 dcm-processor-1.0.2/dcm_processor.egg-info/dependency_links.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       53 2023-04-17 10:46:53.000000 dcm-processor-1.0.2/dcm_processor.egg-info/entry_points.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       76 2023-04-17 10:46:53.000000 dcm-processor-1.0.2/dcm_processor.egg-info/requires.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       14 2023-04-17 10:46:53.000000 dcm-processor-1.0.2/dcm_processor.egg-info/top_level.txt
+-rwxr-xr-x   0 giles     (1000) giles     (1000)       89 2021-10-17 14:23:09.000000 dcm-processor-1.0.2/pyproject.toml
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      980 2023-04-17 10:46:55.098413 dcm-processor-1.0.2/setup.cfg
+-rwxr-xr-x   0 giles     (1000) giles     (1000)      109 2021-10-17 19:37:23.000000 dcm-processor-1.0.2/setup.py
```

### Comparing `dcm-processor-1.0.1/LICENSE` & `dcm-processor-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/PKG-INFO` & `dcm-processor-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcm-processor
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Command line tool for the dicom processor library
 Home-page: https://github.com/giesekow/dcm-processor-cli
 Author: Giles Tetteh
 Author-email: giles.tetteh@tum.de
 Keywords: orthanc,dicom,worker,processor,translation,medical
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,17 +17,18 @@
 
 ## DEPENDENCIES
 1. Python (version  >= 3.6)
 1. Docker
 2. Docker Compose  (you can install with `pip` package manager with the command `pip install docker-compose`)
 
 ### NOTES ON DEPENDENCIES
-1. Current user should have access to execute docker commands without sudo. This can be normally achieved in linux with the command below:  
+1. Current version of the library supports only unix (linux and macOS). However the library was developed and well tested on Ubuntu 20.04.
+2. Current user should have access to execute docker commands without sudo. This can be normally achieved in linux with the command below:  
 `sudo usermod -aG docker $USER`
-2. You need to make sure you have the current version of `docker-compose` installed.
+3. You need to make sure you have the current version of `docker-compose` installed.
 
 
 ## INSTALLATION
 `pip install dcm-processor`
 
 ## CREATE AN APPLICATION
 1. Run the command below and follow the prompt.  
@@ -122,7 +123,10 @@
 
 ## REMOVE WORKER
 1. Run command below and follow prompt to remove a worker.  
 `dcm-processor remove worker`
 
 ## TO DOS
 1. Add documentation for non-interactive (-o) mode.
+2. Add autostart function to start applications at boot time.
+3. Support windows environment.
+4. Run tests on other linux systems.
```

### Comparing `dcm-processor-1.0.1/README.md` & `dcm-processor-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 
 ## DEPENDENCIES
 1. Python (version  >= 3.6)
 1. Docker
 2. Docker Compose  (you can install with `pip` package manager with the command `pip install docker-compose`)
 
 ### NOTES ON DEPENDENCIES
-1. Current user should have access to execute docker commands without sudo. This can be normally achieved in linux with the command below:  
+1. Current version of the library supports only unix (linux and macOS). However the library was developed and well tested on Ubuntu 20.04.
+2. Current user should have access to execute docker commands without sudo. This can be normally achieved in linux with the command below:  
 `sudo usermod -aG docker $USER`
-2. You need to make sure you have the current version of `docker-compose` installed.
+3. You need to make sure you have the current version of `docker-compose` installed.
 
 
 ## INSTALLATION
 `pip install dcm-processor`
 
 ## CREATE AN APPLICATION
 1. Run the command below and follow the prompt.  
@@ -107,8 +108,11 @@
 
 
 ## REMOVE WORKER
 1. Run command below and follow prompt to remove a worker.  
 `dcm-processor remove worker`
 
 ## TO DOS
-1. Add documentation for non-interactive (-o) mode.
+1. Add documentation for non-interactive (-o) mode.
+2. Add autostart function to start applications at boot time.
+3. Support windows environment.
+4. Run tests on other linux systems.
```

### Comparing `dcm-processor-1.0.1/dcm_processor/argparser.py` & `dcm-processor-1.0.2/dcm_processor/argparser.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/files.py` & `dcm-processor-1.0.2/dcm_processor/files.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/script.py` & `dcm-processor-1.0.2/dcm_processor/script.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,23 +37,23 @@
 def handle_installer(args, inst, question, baseDir, isWorker=False):
   if not args.non_interactive:  
     questions = []
 
     if inst == "git" or inst == "web":
       questions.append(inq.Text("object_path", message=question + " (git/web url)"))
       if isWorker:
-        questions.append(inq.Text("sub_path", message="Repository sub-folder", default="worker"))
+        questions.append(inq.Text("sub_path", message="Repository sub-folder", default="./"))
       else:
-        questions.append(inq.Text("sub_path", message="Repository sub-folder", default="service"))
+        questions.append(inq.Text("sub_path", message="Repository sub-folder", default="./"))
     else:
       questions.append(inq.Path("object_path", message=question, exists=True, path_type=inq.Path.DIRECTORY, normalize_to_absolute_path=True))
 
     answers = inq.prompt(questions)
     object_path = answers['object_path']
-    sub_path = answers['sub_path']
+    sub_path = answers.get('sub_path')
   else:
     object_path = args.object_path
     sub_path = './' if args.sub_path is None else args.sub_path
 
     if args.git:
       inst = "git"
     elif args.web:
```

### Comparing `dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar` & `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar` & `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py` & `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py` & `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar` & `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script` & `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar` & `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar` & `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py` & `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar` & `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar` & `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar` & `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/util.jar` & `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/util.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/base/module/DicomAnonymizerService/utils.py` & `dcm-processor-1.0.2/dcm_processor/services/base/module/DicomAnonymizerService/utils.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/base/module/storageManager/lib.py` & `dcm-processor-1.0.2/dcm_processor/services/base/module/storageManager/lib.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/base/module/storageManager/main.py` & `dcm-processor-1.0.2/dcm_processor/services/base/module/storageManager/main.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/base/module/systemcleaner/main.py` & `dcm-processor-1.0.2/dcm_processor/services/base/module/systemcleaner/main.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/dcm2nii/module/__init__.py` & `dcm-processor-1.0.2/dcm_processor/services/dcm2nii/module/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/dcm2nii/module/dcm2niix` & `dcm-processor-1.0.2/dcm_processor/services/dcm2nii/module/dcm2niix`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/services/dcm2nii/registry/__init__.py` & `dcm-processor-1.0.2/dcm_processor/services/dcm2nii/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor/worker.py` & `dcm-processor-1.0.2/dcm_processor/worker.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/dcm_processor.egg-info/PKG-INFO` & `dcm-processor-1.0.2/dcm_processor.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcm-processor
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Command line tool for the dicom processor library
 Home-page: https://github.com/giesekow/dcm-processor-cli
 Author: Giles Tetteh
 Author-email: giles.tetteh@tum.de
 Keywords: orthanc,dicom,worker,processor,translation,medical
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,17 +17,18 @@
 
 ## DEPENDENCIES
 1. Python (version  >= 3.6)
 1. Docker
 2. Docker Compose  (you can install with `pip` package manager with the command `pip install docker-compose`)
 
 ### NOTES ON DEPENDENCIES
-1. Current user should have access to execute docker commands without sudo. This can be normally achieved in linux with the command below:  
+1. Current version of the library supports only unix (linux and macOS). However the library was developed and well tested on Ubuntu 20.04.
+2. Current user should have access to execute docker commands without sudo. This can be normally achieved in linux with the command below:  
 `sudo usermod -aG docker $USER`
-2. You need to make sure you have the current version of `docker-compose` installed.
+3. You need to make sure you have the current version of `docker-compose` installed.
 
 
 ## INSTALLATION
 `pip install dcm-processor`
 
 ## CREATE AN APPLICATION
 1. Run the command below and follow the prompt.  
@@ -122,7 +123,10 @@
 
 ## REMOVE WORKER
 1. Run command below and follow prompt to remove a worker.  
 `dcm-processor remove worker`
 
 ## TO DOS
 1. Add documentation for non-interactive (-o) mode.
+2. Add autostart function to start applications at boot time.
+3. Support windows environment.
+4. Run tests on other linux systems.
```

### Comparing `dcm-processor-1.0.1/dcm_processor.egg-info/SOURCES.txt` & `dcm-processor-1.0.2/dcm_processor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.0.1/setup.cfg` & `dcm-processor-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dcm-processor
-version = 1.0.1
+version = 1.0.2
 author = Giles Tetteh
 author_email = giles.tetteh@tum.de
 description = A Command line tool for the dicom processor library
 url = https://github.com/giesekow/dcm-processor-cli
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE
```

