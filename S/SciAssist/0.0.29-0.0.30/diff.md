# Comparing `tmp/SciAssist-0.0.29.tar.gz` & `tmp/SciAssist-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SciAssist-0.0.29.tar", last modified: Fri Apr 14 07:34:22 2023, max compression
+gzip compressed data, was "SciAssist-0.0.30.tar", last modified: Mon Apr 17 02:28:17 2023, max compression
```

## Comparing `SciAssist-0.0.29.tar` & `SciAssist-0.0.30.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.097593 SciAssist-0.0.29/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    21150 2022-09-28 02:29:12.000000 SciAssist-0.0.29/LICENSE
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       38 2022-09-28 02:29:12.000000 SciAssist-0.0.29/MANIFEST.in
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-14 07:34:22.097593 SciAssist-0.0.29/PKG-INFO
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6208 2022-11-05 13:55:02.000000 SciAssist-0.0.29/README.md
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1379 2023-04-14 07:14:09.000000 SciAssist-0.0.29/pyproject.toml
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      635 2023-04-14 07:34:22.101593 SciAssist-0.0.29/setup.cfg
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       96 2022-09-28 02:29:12.000000 SciAssist-0.0.29/setup.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.089592 SciAssist-0.0.29/src/
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.089592 SciAssist-0.0.29/src/SciAssist/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      818 2023-04-14 07:10:04.000000 SciAssist-0.0.29/src/SciAssist/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.089592 SciAssist-0.0.29/src/SciAssist/bin/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      668 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.089592 SciAssist-0.0.29/src/SciAssist/bin/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      916 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.089592 SciAssist-0.0.29/src/SciAssist/bin/doc2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    11558 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/LICENSE
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.089592 SciAssist-0.0.29/src/SciAssist/bin/doc2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      158 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/__pycache__/__init__.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.089592 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      167 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      227 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/__pycache__/config.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    15546 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       59 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/config.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      179 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2874 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    15434 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4449 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      186 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6183 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5972 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6614 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1019 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2736 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     9058 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        8 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/pdf_to_tei.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3622 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    27209 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    16382 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/s2orc.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      173 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2743 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     8839 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3531 2023-03-15 13:25:23.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3144 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    11737 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6935 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4235 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      585 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/bin/doc2json/scripts/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       73 2022-10-04 11:07:26.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/scripts/run_grobid_linux.sh
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      751 2022-10-04 11:09:22.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      275 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/bin/doc2json/setup.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/datamodules/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/datamodules/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4113 2023-03-26 03:08:44.000000 SciAssist-0.0.29/src/SciAssist/datamodules/acl_datamodule.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.093593 SciAssist-0.0.29/src/SciAssist/datamodules/components/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/datamodules/components/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      370 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/datamodules/components/cora_label.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3112 2022-11-05 13:55:02.000000 SciAssist-0.0.29/src/SciAssist/datamodules/cora_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3357 2023-04-14 07:10:04.000000 SciAssist-0.0.29/src/SciAssist/datamodules/dataset_extraction_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3198 2022-11-10 14:45:14.000000 SciAssist-0.0.29/src/SciAssist/datamodules/fid_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2948 2022-11-27 14:04:32.000000 SciAssist-0.0.29/src/SciAssist/datamodules/general_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4331 2022-12-14 08:45:15.000000 SciAssist-0.0.29/src/SciAssist/datamodules/longsumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     3179 2023-04-02 03:32:15.000000 SciAssist-0.0.29/src/SciAssist/datamodules/mup_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     7753 2023-03-18 16:34:11.000000 SciAssist-0.0.29/src/SciAssist/datamodules/mup_mup_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6862 2023-04-14 07:04:55.000000 SciAssist-0.0.29/src/SciAssist/datamodules/mup_scisumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5865 2023-04-14 07:09:42.000000 SciAssist-0.0.29/src/SciAssist/datamodules/scisumm_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4850 2023-02-23 16:55:34.000000 SciAssist-0.0.29/src/SciAssist/datamodules/test_datamodule.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4211 2022-12-18 15:08:30.000000 SciAssist-0.0.29/src/SciAssist/datamodules/xsum_datamodule.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.097593 SciAssist-0.0.29/src/SciAssist/models/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/models/__init__.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.097593 SciAssist-0.0.29/src/SciAssist/models/components/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/models/components/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1554 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/models/components/bart_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2845 2023-04-14 07:10:04.000000 SciAssist-0.0.29/src/SciAssist/models/components/bert_dataset_extraction.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1547 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/models/components/bert_token_classifier.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    10090 2022-12-05 04:05:34.000000 SciAssist-0.0.29/src/SciAssist/models/components/fid_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1728 2023-04-14 06:59:33.000000 SciAssist-0.0.29/src/SciAssist/models/components/flant5_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1565 2022-11-21 03:52:20.000000 SciAssist-0.0.29/src/SciAssist/models/components/frost_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1590 2022-11-08 07:42:28.000000 SciAssist-0.0.29/src/SciAssist/models/components/longt5_summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     6869 2022-11-19 15:12:24.000000 SciAssist-0.0.29/src/SciAssist/models/cora_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     8632 2023-04-14 07:10:04.000000 SciAssist-0.0.29/src/SciAssist/models/dataset_extraction_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    13319 2023-04-02 03:32:15.000000 SciAssist-0.0.29/src/SciAssist/models/mup_bart_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     7880 2022-11-15 05:02:37.000000 SciAssist-0.0.29/src/SciAssist/models/mup_fid_module.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     8141 2023-04-14 07:09:36.000000 SciAssist-0.0.29/src/SciAssist/models/mup_frost_module.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.097593 SciAssist-0.0.29/src/SciAssist/pipelines/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4193 2023-04-14 07:13:16.000000 SciAssist-0.0.29/src/SciAssist/pipelines/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    12872 2023-04-14 07:10:04.000000 SciAssist-0.0.29/src/SciAssist/pipelines/dataset_extraction.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2056 2022-11-05 13:55:02.000000 SciAssist-0.0.29/src/SciAssist/pipelines/pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    13826 2022-11-05 13:55:02.000000 SciAssist-0.0.29/src/SciAssist/pipelines/reference_string_parsing.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    14508 2023-04-14 07:09:05.000000 SciAssist-0.0.29/src/SciAssist/pipelines/summarization.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    12861 2023-04-14 07:08:00.000000 SciAssist-0.0.29/src/SciAssist/pipelines/summarization_origin.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1950 2023-02-20 05:27:12.000000 SciAssist-0.0.29/src/SciAssist/pipelines/testing_pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4003 2022-11-05 13:55:02.000000 SciAssist-0.0.29/src/SciAssist/pipelines/training_pipeline.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      786 2022-09-28 02:29:12.000000 SciAssist-0.0.29/src/SciAssist/test.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2022-10-02 15:49:40.000000 SciAssist-0.0.29/src/SciAssist/train.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2852 2022-11-27 16:49:31.000000 SciAssist-0.0.29/src/SciAssist/training_args.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.097593 SciAssist-0.0.29/src/SciAssist/utils/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     4733 2023-02-03 14:21:07.000000 SciAssist-0.0.29/src/SciAssist/utils/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2714 2023-03-25 10:51:15.000000 SciAssist-0.0.29/src/SciAssist/utils/acl.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.097593 SciAssist-0.0.29/src/SciAssist/utils/collators/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2323 2022-11-10 14:30:40.000000 SciAssist-0.0.29/src/SciAssist/utils/collators/CollatorForFid.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-11-06 14:22:00.000000 SciAssist-0.0.29/src/SciAssist/utils/collators/__init__.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1232 2023-01-11 16:34:32.000000 SciAssist-0.0.29/src/SciAssist/utils/data_reader.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    75293 2023-04-14 07:10:04.000000 SciAssist-0.0.29/src/SciAssist/utils/data_utils.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    60999 2023-04-14 06:53:22.000000 SciAssist-0.0.29/src/SciAssist/utils/data_utils2.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1751 2023-03-01 06:47:44.000000 SciAssist-0.0.29/src/SciAssist/utils/evaluate_sr.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      661 2023-03-25 10:26:12.000000 SciAssist-0.0.29/src/SciAssist/utils/extract_acl.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5324 2023-03-30 02:58:27.000000 SciAssist-0.0.29/src/SciAssist/utils/extract_keysents.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1912 2023-01-09 01:58:56.000000 SciAssist-0.0.29/src/SciAssist/utils/extract_keywords.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2655 2023-04-05 08:52:04.000000 SciAssist-0.0.29/src/SciAssist/utils/extract_keywords_flant5.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1573 2023-03-19 09:05:48.000000 SciAssist-0.0.29/src/SciAssist/utils/extract_keywords_tfidf.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1703 2023-04-05 08:45:37.000000 SciAssist-0.0.29/src/SciAssist/utils/extract_keywords_yake.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5041 2023-03-25 10:36:56.000000 SciAssist-0.0.29/src/SciAssist/utils/pdf2text.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1502 2023-03-07 08:47:10.000000 SciAssist-0.0.29/src/SciAssist/utils/testset.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     2261 2023-03-27 00:48:06.000000 SciAssist-0.0.29/src/SciAssist/utils/windows_pdf2text.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1499 2023-03-22 11:40:06.000000 SciAssist-0.0.29/src/SciAssist/utils/xml2txt.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.089592 SciAssist-0.0.29/src/SciAssist.egg-info/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-14 07:34:22.000000 SciAssist-0.0.29/src/SciAssist.egg-info/PKG-INFO
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     5460 2023-04-14 07:34:22.000000 SciAssist-0.0.29/src/SciAssist.egg-info/SOURCES.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)        1 2023-04-14 07:34:22.000000 SciAssist-0.0.29/src/SciAssist.egg-info/dependency_links.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       98 2023-04-14 07:34:22.000000 SciAssist-0.0.29/src/SciAssist.egg-info/entry_points.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)      356 2023-04-14 07:34:22.000000 SciAssist-0.0.29/src/SciAssist.egg-info/requires.txt
--rw-rw-r--   0 yixi      (1025) yixi      (1027)       65 2023-04-14 07:34:22.000000 SciAssist-0.0.29/src/SciAssist.egg-info/top_level.txt
--rwxrwxr-x   0 yixi      (1025) yixi      (1027)     1321 2023-03-05 16:03:26.000000 SciAssist-0.0.29/src/chatsonic.py
--rwxrwxr-x   0 yixi      (1025) yixi      (1027)     7944 2022-12-04 10:40:25.000000 SciAssist-0.0.29/src/convert_pegasus.py
--rwxrwxr-x   0 yixi      (1025) yixi      (1027)      690 2022-12-10 17:44:58.000000 SciAssist-0.0.29/src/process.py
-drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-14 07:34:22.097593 SciAssist-0.0.29/tests/
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1095 2022-12-11 12:29:46.000000 SciAssist-0.0.29/tests/test_rsp.py
--rw-rw-r--   0 yixi      (1025) yixi      (1027)     1129 2022-12-11 12:29:46.000000 SciAssist-0.0.29/tests/test_summ.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.605965 SciAssist-0.0.30/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    21150 2022-09-28 02:29:12.000000 SciAssist-0.0.30/LICENSE
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       38 2022-09-28 02:29:12.000000 SciAssist-0.0.30/MANIFEST.in
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-17 02:28:17.605965 SciAssist-0.0.30/PKG-INFO
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6208 2022-11-05 13:55:02.000000 SciAssist-0.0.30/README.md
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1379 2023-04-17 02:28:09.000000 SciAssist-0.0.30/pyproject.toml
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      635 2023-04-17 02:28:17.605965 SciAssist-0.0.30/setup.cfg
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       96 2022-09-28 02:29:12.000000 SciAssist-0.0.30/setup.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.577964 SciAssist-0.0.30/src/
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.577964 SciAssist-0.0.30/src/SciAssist/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      818 2023-04-14 07:10:04.000000 SciAssist-0.0.30/src/SciAssist/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.577964 SciAssist-0.0.30/src/SciAssist/bin/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      668 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.581965 SciAssist-0.0.30/src/SciAssist/bin/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      916 2023-03-15 13:25:23.000000 SciAssist-0.0.30/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.581965 SciAssist-0.0.30/src/SciAssist/bin/doc2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    11558 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/LICENSE
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.581965 SciAssist-0.0.30/src/SciAssist/bin/doc2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      158 2023-03-15 13:25:23.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.581965 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.581965 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      167 2023-03-15 13:25:23.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      227 2023-03-15 13:25:23.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/__pycache__/config.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    15546 2023-03-15 13:25:23.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       59 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/config.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.581965 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.581965 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      179 2023-03-15 13:25:23.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2874 2023-03-15 13:25:23.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    15434 2023-03-15 13:25:23.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.585965 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4449 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.585965 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      186 2023-03-15 13:25:23.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6183 2023-03-15 13:25:23.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5972 2023-03-15 13:25:23.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6614 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1019 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2736 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     9058 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        8 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/pdf_to_tei.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3622 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    27209 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    16382 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/s2orc.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.585965 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.585965 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      173 2023-03-15 13:25:23.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2743 2023-03-15 13:25:23.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     8839 2023-03-15 13:25:23.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3531 2023-03-15 13:25:23.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3144 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    11737 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6935 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4235 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      585 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.589965 SciAssist-0.0.30/src/SciAssist/bin/doc2json/scripts/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       73 2022-10-04 11:07:26.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/scripts/run_grobid_linux.sh
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      751 2022-10-04 11:09:22.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      275 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/bin/doc2json/setup.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.589965 SciAssist-0.0.30/src/SciAssist/datamodules/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/datamodules/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4113 2023-03-26 03:08:44.000000 SciAssist-0.0.30/src/SciAssist/datamodules/acl_datamodule.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.593965 SciAssist-0.0.30/src/SciAssist/datamodules/components/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/datamodules/components/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      370 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/datamodules/components/cora_label.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3112 2022-11-05 13:55:02.000000 SciAssist-0.0.30/src/SciAssist/datamodules/cora_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3357 2023-04-14 07:10:04.000000 SciAssist-0.0.30/src/SciAssist/datamodules/dataset_extraction_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3198 2022-11-10 14:45:14.000000 SciAssist-0.0.30/src/SciAssist/datamodules/fid_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2948 2022-11-27 14:04:32.000000 SciAssist-0.0.30/src/SciAssist/datamodules/general_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4331 2022-12-14 08:45:15.000000 SciAssist-0.0.30/src/SciAssist/datamodules/longsumm_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     3179 2023-04-02 03:32:15.000000 SciAssist-0.0.30/src/SciAssist/datamodules/mup_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     7753 2023-03-18 16:34:11.000000 SciAssist-0.0.30/src/SciAssist/datamodules/mup_mup_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6865 2023-04-15 15:40:45.000000 SciAssist-0.0.30/src/SciAssist/datamodules/mup_scisumm_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5865 2023-04-14 07:09:42.000000 SciAssist-0.0.30/src/SciAssist/datamodules/scisumm_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4850 2023-02-23 16:55:34.000000 SciAssist-0.0.30/src/SciAssist/datamodules/test_datamodule.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4211 2022-12-18 15:08:30.000000 SciAssist-0.0.30/src/SciAssist/datamodules/xsum_datamodule.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.593965 SciAssist-0.0.30/src/SciAssist/models/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/models/__init__.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.593965 SciAssist-0.0.30/src/SciAssist/models/components/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/models/components/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1554 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/models/components/bart_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2845 2023-04-14 07:10:04.000000 SciAssist-0.0.30/src/SciAssist/models/components/bert_dataset_extraction.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1547 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/models/components/bert_token_classifier.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    10090 2022-12-05 04:05:34.000000 SciAssist-0.0.30/src/SciAssist/models/components/fid_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1728 2023-04-14 06:59:33.000000 SciAssist-0.0.30/src/SciAssist/models/components/flant5_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1565 2022-11-21 03:52:20.000000 SciAssist-0.0.30/src/SciAssist/models/components/frost_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1590 2022-11-08 07:42:28.000000 SciAssist-0.0.30/src/SciAssist/models/components/longt5_summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     6869 2022-11-19 15:12:24.000000 SciAssist-0.0.30/src/SciAssist/models/cora_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     8632 2023-04-14 07:10:04.000000 SciAssist-0.0.30/src/SciAssist/models/dataset_extraction_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    13319 2023-04-02 03:32:15.000000 SciAssist-0.0.30/src/SciAssist/models/mup_bart_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     7880 2022-11-15 05:02:37.000000 SciAssist-0.0.30/src/SciAssist/models/mup_fid_module.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     8141 2023-04-14 07:09:36.000000 SciAssist-0.0.30/src/SciAssist/models/mup_frost_module.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.597965 SciAssist-0.0.30/src/SciAssist/pipelines/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4287 2023-04-17 02:07:27.000000 SciAssist-0.0.30/src/SciAssist/pipelines/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    12872 2023-04-14 07:10:04.000000 SciAssist-0.0.30/src/SciAssist/pipelines/dataset_extraction.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2056 2022-11-05 13:55:02.000000 SciAssist-0.0.30/src/SciAssist/pipelines/pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    13826 2022-11-05 13:55:02.000000 SciAssist-0.0.30/src/SciAssist/pipelines/reference_string_parsing.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    14540 2023-04-17 02:10:32.000000 SciAssist-0.0.30/src/SciAssist/pipelines/summarization.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    12861 2023-04-14 07:08:00.000000 SciAssist-0.0.30/src/SciAssist/pipelines/summarization_origin.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1950 2023-02-20 05:27:12.000000 SciAssist-0.0.30/src/SciAssist/pipelines/testing_pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4003 2022-11-05 13:55:02.000000 SciAssist-0.0.30/src/SciAssist/pipelines/training_pipeline.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      786 2022-09-28 02:29:12.000000 SciAssist-0.0.30/src/SciAssist/test.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      787 2022-10-02 15:49:40.000000 SciAssist-0.0.30/src/SciAssist/train.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2852 2022-11-27 16:49:31.000000 SciAssist-0.0.30/src/SciAssist/training_args.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.601965 SciAssist-0.0.30/src/SciAssist/utils/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     4733 2023-02-03 14:21:07.000000 SciAssist-0.0.30/src/SciAssist/utils/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2714 2023-03-25 10:51:15.000000 SciAssist-0.0.30/src/SciAssist/utils/acl.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.605965 SciAssist-0.0.30/src/SciAssist/utils/collators/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2323 2022-11-10 14:30:40.000000 SciAssist-0.0.30/src/SciAssist/utils/collators/CollatorForFid.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        0 2022-11-06 14:22:00.000000 SciAssist-0.0.30/src/SciAssist/utils/collators/__init__.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1232 2023-01-11 16:34:32.000000 SciAssist-0.0.30/src/SciAssist/utils/data_reader.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    75554 2023-04-17 02:22:31.000000 SciAssist-0.0.30/src/SciAssist/utils/data_utils.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    60999 2023-04-14 06:53:22.000000 SciAssist-0.0.30/src/SciAssist/utils/data_utils2.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1751 2023-03-01 06:47:44.000000 SciAssist-0.0.30/src/SciAssist/utils/evaluate_sr.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      661 2023-03-25 10:26:12.000000 SciAssist-0.0.30/src/SciAssist/utils/extract_acl.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5324 2023-03-30 02:58:27.000000 SciAssist-0.0.30/src/SciAssist/utils/extract_keysents.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1912 2023-01-09 01:58:56.000000 SciAssist-0.0.30/src/SciAssist/utils/extract_keywords.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2655 2023-04-05 08:52:04.000000 SciAssist-0.0.30/src/SciAssist/utils/extract_keywords_flant5.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1573 2023-03-19 09:05:48.000000 SciAssist-0.0.30/src/SciAssist/utils/extract_keywords_tfidf.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1703 2023-04-05 08:45:37.000000 SciAssist-0.0.30/src/SciAssist/utils/extract_keywords_yake.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5041 2023-03-25 10:36:56.000000 SciAssist-0.0.30/src/SciAssist/utils/pdf2text.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1502 2023-03-07 08:47:10.000000 SciAssist-0.0.30/src/SciAssist/utils/testset.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     2261 2023-03-27 00:48:06.000000 SciAssist-0.0.30/src/SciAssist/utils/windows_pdf2text.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1499 2023-03-22 11:40:06.000000 SciAssist-0.0.30/src/SciAssist/utils/xml2txt.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.577964 SciAssist-0.0.30/src/SciAssist.egg-info/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)    30858 2023-04-17 02:28:17.000000 SciAssist-0.0.30/src/SciAssist.egg-info/PKG-INFO
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     5460 2023-04-17 02:28:17.000000 SciAssist-0.0.30/src/SciAssist.egg-info/SOURCES.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)        1 2023-04-17 02:28:17.000000 SciAssist-0.0.30/src/SciAssist.egg-info/dependency_links.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       98 2023-04-17 02:28:17.000000 SciAssist-0.0.30/src/SciAssist.egg-info/entry_points.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)      356 2023-04-17 02:28:17.000000 SciAssist-0.0.30/src/SciAssist.egg-info/requires.txt
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)       65 2023-04-17 02:28:17.000000 SciAssist-0.0.30/src/SciAssist.egg-info/top_level.txt
+-rwxrwxr-x   0 yixi      (1025) yixi      (1027)     1321 2023-03-05 16:03:26.000000 SciAssist-0.0.30/src/chatsonic.py
+-rwxrwxr-x   0 yixi      (1025) yixi      (1027)     7944 2022-12-04 10:40:25.000000 SciAssist-0.0.30/src/convert_pegasus.py
+-rwxrwxr-x   0 yixi      (1025) yixi      (1027)      690 2022-12-10 17:44:58.000000 SciAssist-0.0.30/src/process.py
+drwxrwxr-x   0 yixi      (1025) yixi      (1027)        0 2023-04-17 02:28:17.605965 SciAssist-0.0.30/tests/
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1095 2022-12-11 12:29:46.000000 SciAssist-0.0.30/tests/test_rsp.py
+-rw-rw-r--   0 yixi      (1025) yixi      (1027)     1129 2022-12-11 12:29:46.000000 SciAssist-0.0.30/tests/test_summ.py
```

### Comparing `SciAssist-0.0.29/LICENSE` & `SciAssist-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/PKG-INFO` & `SciAssist-0.0.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciAssist
-Version: 0.0.29
+Version: 0.0.30
 Summary: A toolkit for Scientific Document Processing
 Author-email: WING-NUS <dingyixi@hotmail.com>
 Maintainer-email: Yixi Ding <dingyixi@hotmail.com>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `SciAssist-0.0.29/README.md` & `SciAssist-0.0.30/README.md`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/pyproject.toml` & `SciAssist-0.0.30/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SciAssist"
-version = "0.0.29"
+version = "0.0.30"
 authors = [
   { name="WING-NUS", email="dingyixi@hotmail.com" },
 ]
 maintainers = [
   { name="Yixi Ding", email="dingyixi@hotmail.com" },
 ]
 description = "A toolkit for Scientific Document Processing"
```

### Comparing `SciAssist-0.0.29/setup.cfg` & `SciAssist-0.0.30/setup.cfg`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/__init__.py` & `SciAssist-0.0.30/src/SciAssist/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/__init__.py` & `SciAssist-0.0.30/src/SciAssist/bin/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc` & `SciAssist-0.0.30/src/SciAssist/bin/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/LICENSE` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/LICENSE`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/__pycache__/s2orc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/process_pdf.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/__pycache__/tei_to_json.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/Readme.md`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/client.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/__pycache__/grobid_client.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/client.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/config.yaml`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid.properties`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/grobid/grobid_client.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/process_pdf.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/grobid2json/tei_to_json.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/s2orc.py` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/s2orc.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/citation_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/grobid_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/__pycache__/refspan_util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/citation_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/grobid_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/latex_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/refspan_util.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/doc2json/utils/soup_utils.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh` & `SciAssist-0.0.30/src/SciAssist/bin/doc2json/scripts/setup_grobid_linux.sh`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/datamodules/acl_datamodule.py` & `SciAssist-0.0.30/src/SciAssist/datamodules/acl_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/datamodules/cora_datamodule.py` & `SciAssist-0.0.30/src/SciAssist/datamodules/cora_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/datamodules/dataset_extraction_datamodule.py` & `SciAssist-0.0.30/src/SciAssist/datamodules/dataset_extraction_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/datamodules/fid_datamodule.py` & `SciAssist-0.0.30/src/SciAssist/datamodules/fid_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/datamodules/general_datamodule.py` & `SciAssist-0.0.30/src/SciAssist/datamodules/general_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/datamodules/longsumm_datamodule.py` & `SciAssist-0.0.30/src/SciAssist/datamodules/longsumm_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/datamodules/mup_datamodule.py` & `SciAssist-0.0.30/src/SciAssist/datamodules/mup_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/datamodules/mup_mup_datamodule.py` & `SciAssist-0.0.30/src/SciAssist/datamodules/mup_mup_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/datamodules/mup_scisumm_datamodule.py` & `SciAssist-0.0.30/src/SciAssist/datamodules/mup_scisumm_datamodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                         'I05-3025', 'J06-1003', 'J08-2005', 'H91-1026', 'C94-1032', 'C94-1027', 'H93-1051', 'C88-2147',
                         'H92-1045', 'C90-3063', 'C90-3044', 'C94-2174', 'D07-1074', 'H93-1052', 'N03-2021', 'C88-2121',
                         'C92-2070', 'C00-2137', 'W97-0703', 'H94-1020', 'C90-3030', 'H01-1035', 'C96-1055', 'H93-1061',
                         'C96-1005', 'C00-1044', 'C92-1038', 'C00-2163', 'C90-3052', 'J94-2003', 'C04-1073']
         texts = []
         summaries = []
         keywords = []
-        with open("/home/yixi/project/scisumm-corpus/data/Training-Set-2019/Task2/From-ScisummNet-2019/scisumm.csv",
+        with open("/home/yixi/project/scisumm-corpus/data/Training-Set-2019/Task2/From-ScisummNet-2019/scisumm_kw.csv",
                   'r', newline='', encoding='ISO-8859-1') as f:
             rows = csv.reader(f)
             # Get Column names
             keys = next(rows)
             # Add values by column
             for row in rows:
                 k_list = row[1].split(",")
```

### Comparing `SciAssist-0.0.29/src/SciAssist/datamodules/scisumm_datamodule.py` & `SciAssist-0.0.30/src/SciAssist/datamodules/scisumm_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/datamodules/test_datamodule.py` & `SciAssist-0.0.30/src/SciAssist/datamodules/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/datamodules/xsum_datamodule.py` & `SciAssist-0.0.30/src/SciAssist/datamodules/xsum_datamodule.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/models/components/bart_summarization.py` & `SciAssist-0.0.30/src/SciAssist/models/components/bart_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/models/components/bert_dataset_extraction.py` & `SciAssist-0.0.30/src/SciAssist/models/components/bert_dataset_extraction.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/models/components/bert_token_classifier.py` & `SciAssist-0.0.30/src/SciAssist/models/components/bert_token_classifier.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/models/components/fid_summarization.py` & `SciAssist-0.0.30/src/SciAssist/models/components/fid_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/models/components/flant5_summarization.py` & `SciAssist-0.0.30/src/SciAssist/models/components/flant5_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/models/components/frost_summarization.py` & `SciAssist-0.0.30/src/SciAssist/models/components/frost_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/models/components/longt5_summarization.py` & `SciAssist-0.0.30/src/SciAssist/models/components/longt5_summarization.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/models/cora_module.py` & `SciAssist-0.0.30/src/SciAssist/models/cora_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/models/dataset_extraction_module.py` & `SciAssist-0.0.30/src/SciAssist/models/dataset_extraction_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/models/mup_bart_module.py` & `SciAssist-0.0.30/src/SciAssist/models/mup_bart_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/models/mup_fid_module.py` & `SciAssist-0.0.30/src/SciAssist/models/mup_fid_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/models/mup_frost_module.py` & `SciAssist-0.0.30/src/SciAssist/models/mup_frost_module.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/pipelines/__init__.py` & `SciAssist-0.0.30/src/SciAssist/pipelines/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,32 +27,32 @@
             "model": BertForTokenClassifier,
             "model_dict_url": "https://huggingface.co/spaces/wing-nus/SciAssist/resolve/main/scibert-uncased.pt",
             "data_utils": DataUtilsForTokenClassification,
         },
     },
 
     "single-doc-summarization": {
-        "bart-cnn-on-mup": {
-            "model": FlanT5ForSummarization,
-            "model_dict_url": "https://huggingface.co/spaces/dyxohjl666/Controlled-summarization/resolve/main/flant5-mup-scisumm.pt",
-            "data_utils": DataUtilsForSeq2Seq,
-        },
+        # "bart-cnn-on-mup": {
+        #     "model": FlanT5ForSummarization,
+        #     "model_dict_url": "https://huggingface.co/spaces/dyxohjl666/Controlled-summarization/resolve/main/flant5-mup-scisumm.pt",
+        #     "data_utils": DataUtilsForSeq2Seq,
+        # },
         "default": {
             "model": FlanT5ForSummarization,
-            "model_dict_url": "https://huggingface.co/spaces/dyxohjl666/Controlled-summarization/resolve/main/flant5-mup-scisumm.pt",
+            "model_dict_url": "https://huggingface.co/spaces/dyxohjl666/Controlled-summarization/resolve/main/flant5-base.pt",
             "data_utils": DataUtilsForSeq2Seq,
         },
         "t5": {
             "model": FlanT5ForSummarization,
             "model_dict_url": None,
             "data_utils": DataUtilsForT5,
         },
         "flan-t5": {
             "model": FlanT5ForSummarization,
-            "model_dict_url": None,
+            "model_dict_url": "https://huggingface.co/spaces/dyxohjl666/Controlled-summarization/resolve/main/flant5-base.pt",
             "data_utils": DataUtilsForFlanT5,
         }
     },
 
     "controlled-summarization": {
         "default": {
             "model": FlanT5ForSummarization,
```

### Comparing `SciAssist-0.0.29/src/SciAssist/pipelines/dataset_extraction.py` & `SciAssist-0.0.30/src/SciAssist/pipelines/dataset_extraction.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/pipelines/pipeline.py` & `SciAssist-0.0.30/src/SciAssist/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/pipelines/reference_string_parsing.py` & `SciAssist-0.0.30/src/SciAssist/pipelines/reference_string_parsing.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/pipelines/summarization.py` & `SciAssist-0.0.30/src/SciAssist/pipelines/summarization.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,25 +48,26 @@
         model_max_length (`int`, *optional*): The max sequence length the model accepts.
         max_source_length (`int`, *optional*): The max length of the input text.
         max_target_length (`int`, *optional*): The max length of the generated summary.
     """
 
     def __init__(
             self, model_name: str = "default", device="gpu",
+            task_name = "controlled-summarization",
             cache_dir=None,
             output_dir=None,
             temp_dir=None,
             tokenizer=None,
-            checkpoint="facebook/bart-large-cnn",
+            checkpoint="google/flan-t5-base",
             model_max_length=1024,
             max_source_length=1024,
             max_target_length=500,
             os_name=None,
     ):
-        super().__init__(task_name="controlled-summarization", model_name=model_name, device=device,
+        super().__init__(task_name=task_name, model_name=model_name, device=device,
                          cache_dir=cache_dir, output_dir=output_dir, temp_dir=temp_dir)
         # self.model.load_state_dict(
         #     torch.load("/home/dingyx/project/SciAssist/src/pretrained/flant5_scisumm_mup/flant5-base-mix-mup-scisumm-keywords.pt"))
         # self.model.load_state_dict(
         #     torch.load("/home/yixi/project/sciassist/src/pretrained/flant5_mup/flant5-base-mup-scisumm-repeat10.pt")
         # )
         # self.model.load_state_dict(
```

### Comparing `SciAssist-0.0.29/src/SciAssist/pipelines/summarization_origin.py` & `SciAssist-0.0.30/src/SciAssist/pipelines/summarization_origin.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/pipelines/testing_pipeline.py` & `SciAssist-0.0.30/src/SciAssist/pipelines/testing_pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/pipelines/training_pipeline.py` & `SciAssist-0.0.30/src/SciAssist/pipelines/training_pipeline.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/test.py` & `SciAssist-0.0.30/src/SciAssist/test.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/train.py` & `SciAssist-0.0.30/src/SciAssist/train.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/training_args.py` & `SciAssist-0.0.30/src/SciAssist/training_args.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/utils/__init__.py` & `SciAssist-0.0.30/src/SciAssist/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/utils/acl.py` & `SciAssist-0.0.30/src/SciAssist/utils/acl.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/utils/collators/CollatorForFid.py` & `SciAssist-0.0.30/src/SciAssist/utils/collators/CollatorForFid.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/utils/data_reader.py` & `SciAssist-0.0.30/src/SciAssist/utils/data_reader.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/utils/data_utils.py` & `SciAssist-0.0.30/src/SciAssist/utils/data_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -612,166 +612,166 @@
             batch_size=8,
             collate_fn=self.collator(),
         )
 
         return dataloader
 
 
-class DataUtilsForFiD():
-    """
-
-    Args:
-        tokenizer (`PretrainedTokenizer`, default to None):
-            The tokenizer for tokenization.
-        checkpoint (`str`):
-            The checkpoint from which the tokenizer is loaded.
-        model_max_length (`int`, *optional*): The max sequence length the model accepts.
-        max_source_length (`int`, *optional*): The max length of the input text.
-        max_target_length (`int`, *optional*): The max length of the generated summary.
-    """
-
-    def __init__(self, tokenizer = None, model_class = FiDT5,
-                 checkpoint = "google/flan-t5-large",
-                 model_max_length = 64,
-                 max_source_length = 64,
-                 max_target_length = 128,
-                 ):
-
-        self.checkpoint = checkpoint
-        self.model_max_length = model_max_length
-        self.max_source_length = max_source_length
-        self.max_target_length = max_target_length
-        self.model_class = model_class
-
-        if tokenizer is None:
-            self.tokenizer = AutoTokenizer.from_pretrained(
-                self.checkpoint,
-                model_max_length = self.model_max_length,
-                cache_dir=BASE_CACHE_DIR,
-            )
-        else:
-            self.tokenizer = tokenizer
-
-
-    def tokenize_and_align_labels(self, examples, inputs_column="text", labels_column="summary", token_per_paragraph=50):
-
-        """
-
-        Process the dataset for model input, for example, do tokenization and prepare label_ids.
-
-        Args:
-            examples (`Dataset`): { "text": [s1, s2, ...], "summary": [l1, l2, ...]}
-            inputs (`str`): The name of input column
-            labels (`str`): The name of target column
-
-        Returns:
-            `Dict`: {"input_ids": input_ids, "attention_mask": attention_mask, "labels": label_ids }
-
-        """
-
-        # Select input column
-        inputs = examples[inputs_column]
-        dataset = {"paragraphs": []}
-
-        for input in inputs:
-            texts = ["Please give a summary of the following text: "]
-            tokens = input.split(" ")
-            index = 0
-            while index+token_per_paragraph < min(len(tokens),120*token_per_paragraph):
-                p = " ".join(tokens[index:index+token_per_paragraph])
-                texts.append(p)
-                index += token_per_paragraph
-            texts.append(" ".join(tokens[index:index+token_per_paragraph]))
-            dataset["paragraphs"].append(texts)
-
-
-        # Select target column
-        if labels_column in examples.keys():
-            labels = examples[labels_column]
-            dataset["labels"] = labels
-
-        return dataset
-
-    def collator(self):
-
-        """
-
-        The collating function.
-
-        Returns:
-            `function`: A collating function.
-
-            For example, **DataCollatorForSeq2Seq(...)**.
-
-            You can also custom a collating function, but remember that `collator()` needs to return a **function**.
-        """
-
-        from SciAssist.utils.collators.CollatorForFid import DataCollatorForFid
-
-        return DataCollatorForFid(self.max_source_length, self.tokenizer, self.max_target_length)
-
-    def postprocess(self, preds, labels):
-
-        """
-        Process model's outputs and get the final results rather than simple ids.
-
-        Args:
-            preds (Tensor): Prediction labels, the output of the model.
-            labels (Tensor): True labels
-
-        Returns:
-            `(LongTensor, LongTensor)`: decoded_preds, decoded_labels
-
-        """
-
-        decoded_preds = self.tokenizer.batch_decode(preds, skip_special_tokens=True)
-
-        labels = np.array(labels.to("cpu"))
-        # Replace -100 in the labels as we can't decode them.
-        labels = np.where(labels != -100, labels, self.tokenizer.pad_token_id)
-
-        decoded_labels = self.tokenizer.batch_decode(labels, skip_special_tokens=True)
-
-        decoded_preds = [pred.strip() for pred in decoded_preds]
-        decoded_labels = [label.strip() for label in decoded_labels]
-
-        # rougeLSum expects newline after each sentence
-        decoded_preds = ["\n".join(nltk.sent_tokenize(pred)) for pred in decoded_preds]
-        decoded_labels = ["\n".join(nltk.sent_tokenize(label)) for label in decoded_labels]
-
-        return decoded_preds, decoded_labels
-
-    def get_dataloader(self, dataset, inputs_column="text", labels_column="summary"):
-
-        """
-        Generate DataLoader for a dataset.
-
-        Args:
-            dataset (`Dataset`): The raw dataset.
-            inputs_column (`str`): Column name of the inputs.
-            labels_column (`str`): Column name of the labels.
-
-        Returns:
-            `DataLoader`: A dataloader for the dataset. Will be used for inference.
-        """
-
-        tokenized_example = dataset.map(
-            lambda x: self.tokenize_and_align_labels(x, inputs_column=inputs_column, labels_column=labels_column),
-            batched=True,
-            remove_columns=dataset.column_names
-        )
-        dataloader = DataLoader(
-            dataset=tokenized_example,
-            batch_size=8,
-            collate_fn=self.collator(),
-        )
-
-        return dataloader
-
+# class DataUtilsForFiD():
+#     """
+#
+#     Args:
+#         tokenizer (`PretrainedTokenizer`, default to None):
+#             The tokenizer for tokenization.
+#         checkpoint (`str`):
+#             The checkpoint from which the tokenizer is loaded.
+#         model_max_length (`int`, *optional*): The max sequence length the model accepts.
+#         max_source_length (`int`, *optional*): The max length of the input text.
+#         max_target_length (`int`, *optional*): The max length of the generated summary.
+#     """
+#
+#     def __init__(self, tokenizer = None, model_class = FiDT5,
+#                  checkpoint = "google/flan-t5-large",
+#                  model_max_length = 64,
+#                  max_source_length = 64,
+#                  max_target_length = 128,
+#                  ):
+#
+#         self.checkpoint = checkpoint
+#         self.model_max_length = model_max_length
+#         self.max_source_length = max_source_length
+#         self.max_target_length = max_target_length
+#         self.model_class = model_class
+#
+#         if tokenizer is None:
+#             self.tokenizer = AutoTokenizer.from_pretrained(
+#                 self.checkpoint,
+#                 model_max_length = self.model_max_length,
+#                 cache_dir=BASE_CACHE_DIR,
+#             )
+#         else:
+#             self.tokenizer = tokenizer
+#
+#
+#     def tokenize_and_align_labels(self, examples, inputs_column="text", labels_column="summary", token_per_paragraph=50):
+#
+#         """
+#
+#         Process the dataset for model input, for example, do tokenization and prepare label_ids.
+#
+#         Args:
+#             examples (`Dataset`): { "text": [s1, s2, ...], "summary": [l1, l2, ...]}
+#             inputs (`str`): The name of input column
+#             labels (`str`): The name of target column
+#
+#         Returns:
+#             `Dict`: {"input_ids": input_ids, "attention_mask": attention_mask, "labels": label_ids }
+#
+#         """
+#
+#         # Select input column
+#         inputs = examples[inputs_column]
+#         dataset = {"paragraphs": []}
+#
+#         for input in inputs:
+#             texts = ["Please give a summary of the following text: "]
+#             tokens = input.split(" ")
+#             index = 0
+#             while index+token_per_paragraph < min(len(tokens),120*token_per_paragraph):
+#                 p = " ".join(tokens[index:index+token_per_paragraph])
+#                 texts.append(p)
+#                 index += token_per_paragraph
+#             texts.append(" ".join(tokens[index:index+token_per_paragraph]))
+#             dataset["paragraphs"].append(texts)
+#
+#
+#         # Select target column
+#         if labels_column in examples.keys():
+#             labels = examples[labels_column]
+#             dataset["labels"] = labels
+#
+#         return dataset
+#
+#     def collator(self):
+#
+#         """
+#
+#         The collating function.
+#
+#         Returns:
+#             `function`: A collating function.
+#
+#             For example, **DataCollatorForSeq2Seq(...)**.
+#
+#             You can also custom a collating function, but remember that `collator()` needs to return a **function**.
+#         """
+#
+#         from SciAssist.utils.collators.CollatorForFid import DataCollatorForFid
+#
+#         return DataCollatorForFid(self.max_source_length, self.tokenizer, self.max_target_length)
+#
+#     def postprocess(self, preds, labels):
+#
+#         """
+#         Process model's outputs and get the final results rather than simple ids.
+#
+#         Args:
+#             preds (Tensor): Prediction labels, the output of the model.
+#             labels (Tensor): True labels
+#
+#         Returns:
+#             `(LongTensor, LongTensor)`: decoded_preds, decoded_labels
+#
+#         """
+#
+#         decoded_preds = self.tokenizer.batch_decode(preds, skip_special_tokens=True)
+#
+#         labels = np.array(labels.to("cpu"))
+#         # Replace -100 in the labels as we can't decode them.
+#         labels = np.where(labels != -100, labels, self.tokenizer.pad_token_id)
+#
+#         decoded_labels = self.tokenizer.batch_decode(labels, skip_special_tokens=True)
+#
+#         decoded_preds = [pred.strip() for pred in decoded_preds]
+#         decoded_labels = [label.strip() for label in decoded_labels]
+#
+#         # rougeLSum expects newline after each sentence
+#         decoded_preds = ["\n".join(nltk.sent_tokenize(pred)) for pred in decoded_preds]
+#         decoded_labels = ["\n".join(nltk.sent_tokenize(label)) for label in decoded_labels]
+#
+#         return decoded_preds, decoded_labels
+#
+#     def get_dataloader(self, dataset, inputs_column="text", labels_column="summary"):
+#
+#         """
+#         Generate DataLoader for a dataset.
+#
+#         Args:
+#             dataset (`Dataset`): The raw dataset.
+#             inputs_column (`str`): Column name of the inputs.
+#             labels_column (`str`): Column name of the labels.
+#
+#         Returns:
+#             `DataLoader`: A dataloader for the dataset. Will be used for inference.
+#         """
+#
+#         tokenized_example = dataset.map(
+#             lambda x: self.tokenize_and_align_labels(x, inputs_column=inputs_column, labels_column=labels_column),
+#             batched=True,
+#             remove_columns=dataset.column_names
+#         )
+#         dataloader = DataLoader(
+#             dataset=tokenized_example,
+#             batch_size=8,
+#             collate_fn=self.collator(),
+#         )
+#
+#         return dataloader
 #
+# #
 #
 # class DataUtilsForFrost():
 #     """
 #
 #     Args:
 #         tokenizer (`PretrainedTokenizer`, default to None):
 #             The tokenizer for tokenization.
@@ -1159,15 +1159,15 @@
         inputs = examples[inputs_column]
         prompts = [ self.prompt for i in inputs ]
 
         # kw_instructions = ["{}"]
         def kw(prompt, keyword):
             # i = randint(1,10)
             if keyword is not None:
-                return "Keywords: " + str(", ".join(keyword)) + ". " + prompt + "talking about these keywords " if keyword is not None else prompt
+                return "Keywords: [ " + str(", ".join(keyword)) + " ]. " + prompt + "based on these keywords " if keyword is not None else prompt
             return prompt
             # return prompt + "that focuses on " + str(", ".join(keyword)) + " " if keyword is not None else prompt
         def leng(prompt, length):
             if length is not None:
                 return prompt + ", which has less than " + str(length) + " words " if length is not None else prompt
             return prompt
```

### Comparing `SciAssist-0.0.29/src/SciAssist/utils/data_utils2.py` & `SciAssist-0.0.30/src/SciAssist/utils/data_utils2.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/utils/evaluate_sr.py` & `SciAssist-0.0.30/src/SciAssist/utils/evaluate_sr.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/utils/extract_acl.py` & `SciAssist-0.0.30/src/SciAssist/utils/extract_acl.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/utils/extract_keysents.py` & `SciAssist-0.0.30/src/SciAssist/utils/extract_keysents.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/utils/extract_keywords.py` & `SciAssist-0.0.30/src/SciAssist/utils/extract_keywords.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/utils/extract_keywords_flant5.py` & `SciAssist-0.0.30/src/SciAssist/utils/extract_keywords_flant5.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/utils/extract_keywords_tfidf.py` & `SciAssist-0.0.30/src/SciAssist/utils/extract_keywords_tfidf.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/utils/extract_keywords_yake.py` & `SciAssist-0.0.30/src/SciAssist/utils/extract_keywords_yake.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/utils/pdf2text.py` & `SciAssist-0.0.30/src/SciAssist/utils/pdf2text.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/utils/testset.py` & `SciAssist-0.0.30/src/SciAssist/utils/testset.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/utils/windows_pdf2text.py` & `SciAssist-0.0.30/src/SciAssist/utils/windows_pdf2text.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist/utils/xml2txt.py` & `SciAssist-0.0.30/src/SciAssist/utils/xml2txt.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/SciAssist.egg-info/PKG-INFO` & `SciAssist-0.0.30/src/SciAssist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciAssist
-Version: 0.0.29
+Version: 0.0.30
 Summary: A toolkit for Scientific Document Processing
 Author-email: WING-NUS <dingyixi@hotmail.com>
 Maintainer-email: Yixi Ding <dingyixi@hotmail.com>
 License: Attribution-NonCommercial-ShareAlike 4.0 International
         
         =======================================================================
```

### Comparing `SciAssist-0.0.29/src/SciAssist.egg-info/SOURCES.txt` & `SciAssist-0.0.30/src/SciAssist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/chatsonic.py` & `SciAssist-0.0.30/src/chatsonic.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/convert_pegasus.py` & `SciAssist-0.0.30/src/convert_pegasus.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/src/process.py` & `SciAssist-0.0.30/src/process.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/tests/test_rsp.py` & `SciAssist-0.0.30/tests/test_rsp.py`

 * *Files identical despite different names*

### Comparing `SciAssist-0.0.29/tests/test_summ.py` & `SciAssist-0.0.30/tests/test_summ.py`

 * *Files identical despite different names*

