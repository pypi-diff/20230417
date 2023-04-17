# Comparing `tmp/xpotato-0.1.4.tar.gz` & `tmp/xpotato-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpotato-0.1.4.tar", last modified: Mon Oct  3 14:24:07 2022, max compression
+gzip compressed data, was "xpotato-0.1.5.tar", last modified: Mon Apr 17 11:37:16 2023, max compression
```

## Comparing `xpotato-0.1.4.tar` & `xpotato-0.1.5.tar`

### file list

```diff
@@ -1,121 +1,88 @@
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.814500 xpotato-0.1.4/
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.794500 xpotato-0.1.4/.github/
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.804500 xpotato-0.1.4/.github/workflows/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      449 2021-11-22 10:38:58.000000 xpotato-0.1.4/.github/workflows/pylint.yml
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     1825 2021-12-17 11:31:02.000000 xpotato-0.1.4/.gitignore
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     5202 2022-01-11 13:59:08.000000 xpotato-0.1.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      254 2022-01-11 13:59:08.000000 xpotato-0.1.4/CONTRIBUTING.md
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     1071 2021-11-22 10:38:58.000000 xpotato-0.1.4/LICENSE
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)       27 2021-11-29 19:46:14.000000 xpotato-0.1.4/MANIFEST.in
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)    39592 2022-10-03 14:24:07.814500 xpotato-0.1.4/PKG-INFO
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)    35487 2022-05-06 08:16:28.000000 xpotato-0.1.4/README.md
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.804500 xpotato-0.1.4/docs/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     2216 2021-12-17 11:31:02.000000 xpotato-0.1.4/docs/README_advanced_mode.md
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     1703 2021-11-22 10:38:58.000000 xpotato-0.1.4/docs/experiments.md
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.804500 xpotato-0.1.4/features/
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.804500 xpotato-0.1.4/features/crowdtruth/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     1106 2022-03-09 10:46:32.000000 xpotato-0.1.4/features/crowdtruth/README.md
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      682 2021-11-22 10:38:58.000000 xpotato-0.1.4/features/crowdtruth/crowd_cause_features_ud.json
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     3276 2022-05-06 08:54:38.000000 xpotato-0.1.4/features/crowdtruth/crowd_treat_features_ud.json
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)    15589 2022-03-09 10:46:32.000000 xpotato-0.1.4/features/crowdtruth/crowdtruth.ipynb
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     1380 2022-03-09 10:46:32.000000 xpotato-0.1.4/features/crowdtruth/data.sh
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.804500 xpotato-0.1.4/features/food/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     1073 2022-03-09 10:46:32.000000 xpotato-0.1.4/features/food/README.md
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      868 2022-03-09 10:46:32.000000 xpotato-0.1.4/features/food/data.sh
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     9719 2022-03-09 10:46:32.000000 xpotato-0.1.4/features/food/food.ipynb
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      535 2021-11-22 10:38:58.000000 xpotato-0.1.4/features/food/food_cause_features_ud.json
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     1085 2021-11-22 10:38:58.000000 xpotato-0.1.4/features/food/food_treat_features_ud.json
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.804500 xpotato-0.1.4/features/hasoc/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     1829 2021-11-22 10:38:58.000000 xpotato-0.1.4/features/hasoc/2019_train_features.json
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     3307 2021-12-15 09:03:12.000000 xpotato-0.1.4/features/hasoc/2020_train_features_task1.json
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     3690 2021-11-22 10:38:58.000000 xpotato-0.1.4/features/hasoc/2021_train_features_task1.json
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)    20448 2022-03-09 10:46:32.000000 xpotato-0.1.4/features/hasoc/README.md
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      890 2022-03-09 10:46:32.000000 xpotato-0.1.4/features/hasoc/data.sh
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)   214537 2021-11-22 10:38:58.000000 xpotato-0.1.4/features/hasoc/hasoc_2019_test_normalized.csv
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)  1095812 2021-11-22 10:38:58.000000 xpotato-0.1.4/features/hasoc/hasoc_2019_train_normalized.csv
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)   219317 2021-11-22 10:38:58.000000 xpotato-0.1.4/features/hasoc/hasoc_2020_en_test_new_normalized.csv
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)   345562 2021-11-22 10:38:58.000000 xpotato-0.1.4/features/hasoc/hasoc_2020_en_train_new.xlsx
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)   510968 2021-11-22 10:38:58.000000 xpotato-0.1.4/features/hasoc/hasoc_2020_en_train_new_normalized.csv
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)   233593 2021-11-22 10:38:58.000000 xpotato-0.1.4/features/hasoc/hasoc_2021_test_normalized.csv
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)   747443 2021-11-22 10:38:58.000000 xpotato-0.1.4/features/hasoc/hasoc_2021_train_normalized.csv
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.804500 xpotato-0.1.4/features/semeval/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      559 2022-03-09 10:46:32.000000 xpotato-0.1.4/features/semeval/README.md
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      386 2022-03-09 10:46:32.000000 xpotato-0.1.4/features/semeval/data.sh
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      337 2022-02-21 10:40:57.000000 xpotato-0.1.4/features/semeval/test_features.json
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.804500 xpotato-0.1.4/files/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)    13232 2021-12-17 11:31:02.000000 xpotato-0.1.4/files/potato_logo.png
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     7597 2021-12-15 09:03:12.000000 xpotato-0.1.4/files/re_example.svg
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.804500 xpotato-0.1.4/frontend/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)        0 2021-12-17 11:31:02.000000 xpotato-0.1.4/frontend/__init__.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)    50814 2022-09-12 12:27:20.000000 xpotato-0.1.4/frontend/app.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)    22530 2022-09-12 12:27:20.000000 xpotato-0.1.4/frontend/utils.py
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.814500 xpotato-0.1.4/notebooks/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)    91219 2022-04-21 12:11:30.000000 xpotato-0.1.4/notebooks/hasoc_examples.ipynb
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)    18798 2022-03-09 10:46:32.000000 xpotato-0.1.4/notebooks/openie.ipynb
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)    84851 2022-03-09 10:46:32.000000 xpotato-0.1.4/notebooks/relation_examples.ipynb
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.814500 xpotato-0.1.4/scripts/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      620 2022-03-09 10:46:32.000000 xpotato-0.1.4/scripts/convert_pickle.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      523 2022-09-12 12:27:20.000000 xpotato-0.1.4/scripts/convert_rules.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     4507 2022-09-12 12:27:20.000000 xpotato-0.1.4/scripts/evaluate.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     5144 2022-09-12 12:27:20.000000 xpotato-0.1.4/scripts/evaluate_hatexplain.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)    12988 2022-09-12 12:27:20.000000 xpotato-0.1.4/scripts/read_hatexplain.py
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.814500 xpotato-0.1.4/services/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     1820 2021-12-17 11:31:02.000000 xpotato-0.1.4/services/main.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)       79 2022-10-03 14:24:07.814500 xpotato-0.1.4/setup.cfg
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     1549 2022-10-03 14:23:18.000000 xpotato-0.1.4/setup.py
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.814500 xpotato-0.1.4/tests/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      153 2022-03-09 10:46:32.000000 xpotato-0.1.4/tests/features.json
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      106 2022-03-09 10:46:32.000000 xpotato-0.1.4/tests/features.tsv
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      156 2022-03-09 10:46:32.000000 xpotato-0.1.4/tests/features_openie.tsv
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     2834 2022-03-09 10:46:32.000000 xpotato-0.1.4/tests/test_ruleset.py
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.814500 xpotato-0.1.4/xpotato/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)        0 2021-11-29 19:46:14.000000 xpotato-0.1.4/xpotato/__init__.py
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.814500 xpotato-0.1.4/xpotato/__pycache__/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      140 2021-11-29 19:46:19.000000 xpotato-0.1.4/xpotato/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.814500 xpotato-0.1.4/xpotato/dataset/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)        0 2021-11-29 19:46:14.000000 xpotato-0.1.4/xpotato/dataset/__init__.py
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.814500 xpotato-0.1.4/xpotato/dataset/__pycache__/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      148 2021-11-29 19:46:19.000000 xpotato-0.1.4/xpotato/dataset/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     6224 2022-04-21 11:18:14.000000 xpotato-0.1.4/xpotato/dataset/__pycache__/dataset.cpython-39.pyc
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     1098 2022-04-18 12:49:03.000000 xpotato-0.1.4/xpotato/dataset/__pycache__/sample.cpython-39.pyc
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     3180 2022-03-09 13:37:33.000000 xpotato-0.1.4/xpotato/dataset/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     5333 2022-05-06 08:16:22.000000 xpotato-0.1.4/xpotato/dataset/dataset.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     2829 2022-09-12 12:27:20.000000 xpotato-0.1.4/xpotato/dataset/explainable_dataset.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     1176 2022-09-12 12:27:20.000000 xpotato-0.1.4/xpotato/dataset/explainable_sample.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     1198 2021-11-29 19:46:14.000000 xpotato-0.1.4/xpotato/dataset/relation_dataset.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     1516 2022-05-06 08:16:22.000000 xpotato-0.1.4/xpotato/dataset/relation_sample.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      745 2022-03-09 10:46:32.000000 xpotato-0.1.4/xpotato/dataset/sample.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     5127 2022-03-09 10:46:32.000000 xpotato-0.1.4/xpotato/dataset/utils.py
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.814500 xpotato-0.1.4/xpotato/features/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)        0 2022-09-12 12:27:20.000000 xpotato-0.1.4/xpotato/features/__init__.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     1166 2022-09-12 12:27:20.000000 xpotato-0.1.4/xpotato/features/utils.py
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.814500 xpotato-0.1.4/xpotato/graph_extractor/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)        0 2021-11-29 19:46:14.000000 xpotato-0.1.4/xpotato/graph_extractor/__init__.py
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.814500 xpotato-0.1.4/xpotato/graph_extractor/__pycache__/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      156 2021-11-29 19:46:19.000000 xpotato-0.1.4/xpotato/graph_extractor/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)    12135 2022-07-19 07:16:28.000000 xpotato-0.1.4/xpotato/graph_extractor/__pycache__/extract.cpython-39.pyc
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      855 2022-03-09 13:37:33.000000 xpotato-0.1.4/xpotato/graph_extractor/__pycache__/graph.cpython-39.pyc
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     5105 2022-05-06 11:59:17.000000 xpotato-0.1.4/xpotato/graph_extractor/__pycache__/rule.cpython-39.pyc
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.814500 xpotato-0.1.4/xpotato/graph_extractor/cache/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     4321 2022-04-19 16:27:01.000000 xpotato-0.1.4/xpotato/graph_extractor/cache/UD_FL.json
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)    22497 2022-04-19 16:27:01.000000 xpotato-0.1.4/xpotato/graph_extractor/cache/de_nlp_cache.json
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)    18264 2022-09-12 12:27:20.000000 xpotato-0.1.4/xpotato/graph_extractor/extract.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      468 2022-03-09 10:46:32.000000 xpotato-0.1.4/xpotato/graph_extractor/graph.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     4584 2022-09-12 12:27:20.000000 xpotato-0.1.4/xpotato/graph_extractor/rule.py
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.814500 xpotato-0.1.4/xpotato/models/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)        0 2021-11-29 19:46:14.000000 xpotato-0.1.4/xpotato/models/__init__.py
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.814500 xpotato-0.1.4/xpotato/models/__pycache__/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      147 2021-11-29 19:46:20.000000 xpotato-0.1.4/xpotato/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     4322 2021-12-17 11:35:50.000000 xpotato-0.1.4/xpotato/models/__pycache__/model.cpython-39.pyc
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     5800 2022-02-07 12:43:35.000000 xpotato-0.1.4/xpotato/models/__pycache__/trainer.cpython-39.pyc
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     4375 2022-06-09 09:00:27.000000 xpotato-0.1.4/xpotato/models/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     3395 2021-12-17 11:31:02.000000 xpotato-0.1.4/xpotato/models/model.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     5796 2022-02-07 12:34:26.000000 xpotato-0.1.4/xpotato/models/trainer.py
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     7248 2022-05-06 08:16:22.000000 xpotato-0.1.4/xpotato/models/utils.py
-drwxr-xr-x   0 adaamko   (1000) adaamko   (1000)        0 2022-10-03 14:24:07.814500 xpotato-0.1.4/xpotato.egg-info/
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)    39592 2022-10-03 14:24:07.000000 xpotato-0.1.4/xpotato.egg-info/PKG-INFO
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)     3058 2022-10-03 14:24:07.000000 xpotato-0.1.4/xpotato.egg-info/SOURCES.txt
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)        1 2022-10-03 14:24:07.000000 xpotato-0.1.4/xpotato.egg-info/dependency_links.txt
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)        1 2021-11-29 10:41:05.000000 xpotato-0.1.4/xpotato.egg-info/not-zip-safe
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)      298 2022-10-03 14:24:07.000000 xpotato-0.1.4/xpotato.egg-info/requires.txt
--rw-r--r--   0 adaamko   (1000) adaamko   (1000)       17 2022-10-03 14:24:07.000000 xpotato-0.1.4/xpotato.egg-info/top_level.txt
+drwxr-xr-x   0 adamkovacs   (501) staff       (20)        0 2023-04-17 11:37:16.615473 xpotato-0.1.5/
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     1071 2021-08-25 08:01:24.000000 xpotato-0.1.5/LICENSE
+-rw-r--r--   0 adamkovacs   (501) staff       (20)       27 2021-11-29 19:33:59.000000 xpotato-0.1.5/MANIFEST.in
+-rw-r--r--   0 adamkovacs   (501) staff       (20)    36725 2023-04-17 11:37:16.615594 xpotato-0.1.5/PKG-INFO
+-rw-r--r--   0 adamkovacs   (501) staff       (20)    35921 2022-11-23 10:35:27.000000 xpotato-0.1.5/README.md
+drwxr-xr-x   0 adamkovacs   (501) staff       (20)        0 2023-04-17 11:37:16.600517 xpotato-0.1.5/frontend/
+-rw-r--r--   0 adamkovacs   (501) staff       (20)        0 2021-12-17 11:42:08.000000 xpotato-0.1.5/frontend/__init__.py
+-rw-r--r--   0 adamkovacs   (501) staff       (20)    50813 2022-12-12 18:15:59.000000 xpotato-0.1.5/frontend/app.py
+-rw-r--r--   0 adamkovacs   (501) staff       (20)    22227 2022-12-12 18:15:19.000000 xpotato-0.1.5/frontend/utils.py
+-rw-r--r--   0 adamkovacs   (501) staff       (20)       79 2023-04-17 11:37:16.615880 xpotato-0.1.5/setup.cfg
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     1548 2023-04-17 11:33:47.000000 xpotato-0.1.5/setup.py
+drwxr-xr-x   0 adamkovacs   (501) staff       (20)        0 2023-04-17 11:37:16.601162 xpotato-0.1.5/xpotato/
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     6148 2022-02-22 09:44:47.000000 xpotato-0.1.5/xpotato/.DS_Store
+-rw-r--r--   0 adamkovacs   (501) staff       (20)        0 2021-11-29 19:33:59.000000 xpotato-0.1.5/xpotato/__init__.py
+drwxr-xr-x   0 adamkovacs   (501) staff       (20)        0 2023-04-17 11:37:16.602753 xpotato-0.1.5/xpotato/__pycache__/
+-rw-r--r--   0 adamkovacs   (501) staff       (20)      163 2022-11-23 10:58:03.000000 xpotato-0.1.5/xpotato/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)      157 2022-06-27 10:17:59.000000 xpotato-0.1.5/xpotato/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)      161 2021-11-30 14:17:18.000000 xpotato-0.1.5/xpotato/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 adamkovacs   (501) staff       (20)        0 2023-04-17 11:37:16.604492 xpotato-0.1.5/xpotato/dataset/
+-rw-r--r--   0 adamkovacs   (501) staff       (20)        0 2021-11-29 19:33:59.000000 xpotato-0.1.5/xpotato/dataset/__init__.py
+drwxr-xr-x   0 adamkovacs   (501) staff       (20)        0 2023-04-17 11:37:16.607338 xpotato-0.1.5/xpotato/dataset/__pycache__/
+-rw-r--r--   0 adamkovacs   (501) staff       (20)      171 2022-11-23 10:58:03.000000 xpotato-0.1.5/xpotato/dataset/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)      165 2022-06-27 10:18:04.000000 xpotato-0.1.5/xpotato/dataset/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)      169 2021-11-30 14:17:18.000000 xpotato-0.1.5/xpotato/dataset/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     6687 2023-02-10 13:24:33.000000 xpotato-0.1.5/xpotato/dataset/__pycache__/dataset.cpython-310.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     6638 2023-03-27 13:21:55.000000 xpotato-0.1.5/xpotato/dataset/__pycache__/dataset.cpython-37.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     6754 2023-03-13 14:30:58.000000 xpotato-0.1.5/xpotato/dataset/__pycache__/dataset.cpython-39.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     1126 2022-11-23 10:58:34.000000 xpotato-0.1.5/xpotato/dataset/__pycache__/sample.cpython-310.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     1087 2023-03-27 13:21:55.000000 xpotato-0.1.5/xpotato/dataset/__pycache__/sample.cpython-37.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     1119 2022-11-23 15:21:23.000000 xpotato-0.1.5/xpotato/dataset/__pycache__/sample.cpython-39.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     3299 2023-02-10 13:24:36.000000 xpotato-0.1.5/xpotato/dataset/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     3320 2023-03-27 13:21:57.000000 xpotato-0.1.5/xpotato/dataset/__pycache__/utils.cpython-37.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     3316 2023-03-13 14:31:00.000000 xpotato-0.1.5/xpotato/dataset/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     5962 2022-12-12 18:15:19.000000 xpotato-0.1.5/xpotato/dataset/dataset.py
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     2829 2022-11-23 10:35:27.000000 xpotato-0.1.5/xpotato/dataset/explainable_dataset.py
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     1177 2022-12-12 18:15:19.000000 xpotato-0.1.5/xpotato/dataset/explainable_sample.py
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     1199 2022-12-12 18:15:19.000000 xpotato-0.1.5/xpotato/dataset/relation_dataset.py
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     1518 2022-12-12 18:15:19.000000 xpotato-0.1.5/xpotato/dataset/relation_sample.py
+-rw-r--r--   0 adamkovacs   (501) staff       (20)      745 2022-11-23 10:35:27.000000 xpotato-0.1.5/xpotato/dataset/sample.py
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     5201 2022-12-12 18:15:19.000000 xpotato-0.1.5/xpotato/dataset/utils.py
+drwxr-xr-x   0 adamkovacs   (501) staff       (20)        0 2023-04-17 11:37:16.607677 xpotato-0.1.5/xpotato/features/
+-rw-r--r--   0 adamkovacs   (501) staff       (20)        0 2022-11-23 10:35:27.000000 xpotato-0.1.5/xpotato/features/__init__.py
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     1167 2022-11-23 10:35:27.000000 xpotato-0.1.5/xpotato/features/utils.py
+drwxr-xr-x   0 adamkovacs   (501) staff       (20)        0 2023-04-17 11:37:16.608282 xpotato-0.1.5/xpotato/graph_extractor/
+-rw-r--r--   0 adamkovacs   (501) staff       (20)        0 2021-11-29 19:33:59.000000 xpotato-0.1.5/xpotato/graph_extractor/__init__.py
+drwxr-xr-x   0 adamkovacs   (501) staff       (20)        0 2023-04-17 11:37:16.611107 xpotato-0.1.5/xpotato/graph_extractor/__pycache__/
+-rw-r--r--   0 adamkovacs   (501) staff       (20)      179 2022-11-23 10:58:34.000000 xpotato-0.1.5/xpotato/graph_extractor/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)      173 2022-06-27 10:17:59.000000 xpotato-0.1.5/xpotato/graph_extractor/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)      177 2021-11-30 14:17:19.000000 xpotato-0.1.5/xpotato/graph_extractor/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)    12970 2023-03-27 12:53:24.000000 xpotato-0.1.5/xpotato/graph_extractor/__pycache__/extract.cpython-310.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)    12981 2023-03-27 13:21:55.000000 xpotato-0.1.5/xpotato/graph_extractor/__pycache__/extract.cpython-37.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)    12942 2023-03-13 14:40:35.000000 xpotato-0.1.5/xpotato/graph_extractor/__pycache__/extract.cpython-39.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     1578 2023-02-10 13:24:36.000000 xpotato-0.1.5/xpotato/graph_extractor/__pycache__/graph.cpython-310.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     1549 2023-03-27 13:21:55.000000 xpotato-0.1.5/xpotato/graph_extractor/__pycache__/graph.cpython-37.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     1571 2023-03-13 14:30:58.000000 xpotato-0.1.5/xpotato/graph_extractor/__pycache__/graph.cpython-39.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     5001 2023-03-27 13:21:57.000000 xpotato-0.1.5/xpotato/graph_extractor/__pycache__/rule.cpython-37.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     5126 2022-11-23 15:21:23.000000 xpotato-0.1.5/xpotato/graph_extractor/__pycache__/rule.cpython-39.pyc
+drwxr-xr-x   0 adamkovacs   (501) staff       (20)        0 2023-04-17 11:37:16.611621 xpotato-0.1.5/xpotato/graph_extractor/cache/
+-rw-r--r--   0 adamkovacs   (501) staff       (20)    11576 2023-03-13 17:50:18.000000 xpotato-0.1.5/xpotato/graph_extractor/cache/UD_FL.json
+-rw-r--r--   0 adamkovacs   (501) staff       (20)    47897 2023-03-13 17:50:18.000000 xpotato-0.1.5/xpotato/graph_extractor/cache/en_nlp_cache.json
+-rw-r--r--   0 adamkovacs   (501) staff       (20)    20694 2023-03-13 14:39:35.000000 xpotato-0.1.5/xpotato/graph_extractor/extract.py
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     1200 2022-12-12 18:15:20.000000 xpotato-0.1.5/xpotato/graph_extractor/graph.py
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     4584 2022-11-23 10:35:27.000000 xpotato-0.1.5/xpotato/graph_extractor/rule.py
+drwxr-xr-x   0 adamkovacs   (501) staff       (20)        0 2023-04-17 11:37:16.612443 xpotato-0.1.5/xpotato/models/
+-rw-r--r--   0 adamkovacs   (501) staff       (20)        0 2021-11-29 19:33:59.000000 xpotato-0.1.5/xpotato/models/__init__.py
+drwxr-xr-x   0 adamkovacs   (501) staff       (20)        0 2023-04-17 11:37:16.615234 xpotato-0.1.5/xpotato/models/__pycache__/
+-rw-r--r--   0 adamkovacs   (501) staff       (20)      170 2022-11-23 10:58:58.000000 xpotato-0.1.5/xpotato/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)      164 2023-03-27 13:21:57.000000 xpotato-0.1.5/xpotato/models/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)      168 2021-11-30 17:32:16.000000 xpotato-0.1.5/xpotato/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     4317 2023-02-10 13:24:41.000000 xpotato-0.1.5/xpotato/models/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     4333 2023-03-27 13:22:02.000000 xpotato-0.1.5/xpotato/models/__pycache__/model.cpython-37.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     4343 2023-03-13 14:31:01.000000 xpotato-0.1.5/xpotato/models/__pycache__/model.cpython-39.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     5864 2023-02-10 13:24:36.000000 xpotato-0.1.5/xpotato/models/__pycache__/trainer.cpython-310.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     5729 2023-03-27 13:21:57.000000 xpotato-0.1.5/xpotato/models/__pycache__/trainer.cpython-37.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     5809 2023-03-13 14:31:00.000000 xpotato-0.1.5/xpotato/models/__pycache__/trainer.cpython-39.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     4438 2022-11-23 10:59:04.000000 xpotato-0.1.5/xpotato/models/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     4496 2023-03-27 13:22:02.000000 xpotato-0.1.5/xpotato/models/__pycache__/utils.cpython-37.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     4396 2022-11-23 15:21:22.000000 xpotato-0.1.5/xpotato/models/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     3397 2022-12-12 18:15:20.000000 xpotato-0.1.5/xpotato/models/model.py
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     5778 2022-12-12 18:15:20.000000 xpotato-0.1.5/xpotato/models/trainer.py
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     7248 2022-11-23 10:35:27.000000 xpotato-0.1.5/xpotato/models/utils.py
+drwxr-xr-x   0 adamkovacs   (501) staff       (20)        0 2023-04-17 11:37:16.602137 xpotato-0.1.5/xpotato.egg-info/
+-rw-r--r--   0 adamkovacs   (501) staff       (20)    36725 2023-04-17 11:37:16.000000 xpotato-0.1.5/xpotato.egg-info/PKG-INFO
+-rw-r--r--   0 adamkovacs   (501) staff       (20)     2941 2023-04-17 11:37:16.000000 xpotato-0.1.5/xpotato.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkovacs   (501) staff       (20)        1 2023-04-17 11:37:16.000000 xpotato-0.1.5/xpotato.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkovacs   (501) staff       (20)        1 2021-11-29 17:30:30.000000 xpotato-0.1.5/xpotato.egg-info/not-zip-safe
+-rw-r--r--   0 adamkovacs   (501) staff       (20)      299 2023-04-17 11:37:16.000000 xpotato-0.1.5/xpotato.egg-info/requires.txt
+-rw-r--r--   0 adamkovacs   (501) staff       (20)       17 2023-04-17 11:37:16.000000 xpotato-0.1.5/xpotato.egg-info/top_level.txt
```

### Comparing `xpotato-0.1.4/LICENSE` & `xpotato-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xpotato-0.1.4/PKG-INFO` & `xpotato-0.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,434 +1,424 @@
-Metadata-Version: 2.1
-Name: xpotato
-Version: 0.1.4
-Summary: XAI human-in-the-loop information extraction framework
-Home-page: https://github.com/adaamko/POTATO
-Author: Adam Kovacs, Gabor Recski
-Author-email: adam.kovacs@tuwien.ac.at, gabor.recski@tuwien.ac.at
-License: MIT
-Description: <p align="center">
-          <img src="https://raw.githubusercontent.com/adaamko/POTATO/dev/files/potato_logo.png" />
-        </p>
-        
-        # POTATO: exPlainable infOrmation exTrAcTion framewOrk
-        POTATO is a human-in-the-loop XAI framework for extracting and evaluating interpretable graph features for any classification problem in Natural Language Processing.
-        
-        ## Built systems
-        
-        To get started with rule-systems we provide rule-based features prebuilt with POTATO on different datasets (e.g. our paper _Offensive text detection on English Twitter with deep learning models and rule-based systems_ for the HASOC2021 shared task). If you are interested in that, you can go under _features/_ for more info!
-        
-        ## Install and Quick Start
-        Check out our quick demonstration (~2 min) video about the tool:
-        https://youtu.be/PkQ71wUSeNU
-        
-        There is a longer version with a detailed method description and presented background research (~1 hour): https://youtu.be/6R_V1WfIjsU
-        
-        ### Setup
-        The tool is heavily dependent upon the [tuw-nlp](https://github.com/recski/tuw-nlp) repository. You can install tuw-nlp with pip:
-        
-        ```
-        pip install tuw-nlp
-        ```
-        Then follow the [instructions](https://github.com/recski/tuw-nlp) to setup the package.
-        
-        
-        Then install POTATO from pip:
-        
-        ```
-        pip install xpotato
-        ```
-        
-        Or you can install it from source:
-        
-        ```
-        pip install -e .
-        ```
-        
-        ### Usage
-        
-        - POTATO is an IE tool that works on graphs, currently we support three types of graphs: AMR, UD and [Fourlang](https://github.com/kornai/4lang). 
-        
-        - In the README we provide examples with fourlang semantic graphs. Make sure to follow the instructions in the [tuw_nlp](https://github.com/recski/tuw-nlp) repo to be able to build fourlang graphs. 
-        
-        - If you are interested in AMR graphs, you can go to the [hasoc](https://github.com/adaamko/POTATO/tree/main/features/hasoc) folder To get started with rule-systems prebuilt with POTATO on the HASOC dataset (we also presented a paper named _Offensive text detection on English Twitter with deep learning models and rule-based systems_ for the HASOC2021 shared task). 
-        
-        - We also provide experiments on the [CrowdTruth](https://github.com/CrowdTruth/Medical-Relation-Extraction) medical relation extraction datasets with UD graphs, go to the [crowdtruth](https://github.com/adaamko/POTATO/tree/main/features/crowdtruth) folder for more info!
-        
-        - POTATO can also handle unlabeled, or partially labeled data, see [advanced](###advanced-mode) mode to get to know more.
-        
-        __To see complete working examples go under the _notebooks/_ folder to see experiments on HASOC and on the Semeval relation extraction dataset.__
-        
-        First import packages from potato:
-        ```python
-        from xpotato.dataset.dataset import Dataset
-        from xpotato.models.trainer import GraphTrainer
-        ```
-        
-        First we demonstrate POTATO's capabilities with a few sentences manually picked from the dataset.
-        
-        __Note that we replaced the two entitites in question with _XXX_ and _YYY_.__
-        
-        ```python
-        sentences = [("Governments and industries in nations around the world are pouring XXX into YYY.", "Entity-Destination(e1,e2)"),
-                    ("The scientists poured XXX into pint YYY.", "Entity-Destination(e1,e2)"),
-                    ("The suspect pushed the XXX into a deep YYY.", "Entity-Destination(e1,e2)"),
-                    ("The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.", "Other"),
-                    ("The entity1 to buy papers is pushed into the next entity2.", "Entity-Destination(e1,e2)"),
-                    ("An unnamed XXX was pushed into the YYY.", "Entity-Destination(e1,e2)"),
-                    ("Since then, numerous independent feature XXX have journeyed into YYY.", "Other"),
-                    ("For some reason, the XXX was blinded from his own YYY about the incommensurability of time.", "Other"),
-                    ("Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.", "Other"),
-                    ("Olympics have already poured one XXX into the YYY.", "Entity-Destination(e1,e2)"),
-                    ("After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.", "Entity-Destination(e1,e2)"),
-                    ("I placed the XXX in a natural YYY, at the base of a part of the fallen arch.", "Entity-Destination(e1,e2)"),
-                    ("The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.", "Other"),
-                    ("The XXX leaked from every conceivable YYY.", "Other"),
-                    ("The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse.", "Entity-Destination(e1,e2)"),
-                    ("The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.", "Other"),
-                    ("Gaza XXX recover from three YYY of war.", "Other"),
-                    ("This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.", "Other")]
-        ```
-        
-        Initialize the dataset and also provide a label encoding. Then parse the sentences into graphs. Currently we provide three types of graphs: _ud_, _fourlang_, _amr_. Also provide the language you want to parse, currently we support English (en) and German (de).
-        
-        ```python
-        dataset = Dataset(sentences, label_vocab={"Other":0, "Entity-Destination(e1,e2)": 1}, lang="en")
-        dataset.set_graphs(dataset.parse_graphs(graph_format="ud"))
-        ```
-        
-        Check the dataset:
-        ```python
-        df = dataset.to_dataframe()
-        ```
-        
-        We can also check any of the graphs:
-        ### Check any of the graphs parsed
-        
-        ```python
-        from xpotato.models.utils import to_dot
-        from graphviz import Source
-        
-        Source(to_dot(df.iloc[0].graph))
-        ```
-        ![graph](https://raw.githubusercontent.com/adaamko/POTATO/main/files/re_example.svg)
-        
-        ### Rules
-        
-        If the dataset is prepared and the graphs are parsed, we can write rules to match labels. We can write rules either manually or extract
-        them automatically (POTATO also provides a frontend that tries to do both).
-        
-        The simplest rule would be just a node in the graph:
-        ```python
-        # The syntax of the rules is List[List[rules that we want to match], List[rules that shouldn't be in the matched graphs], Label of the rule]
-        rule_to_match = [[["(u_1 / into)"], [], "Entity-Destination(e1,e2)"]]
-        ```
-        
-        Init the rule matcher:
-        ```python
-        from xpotato.graph_extractor.extract import FeatureEvaluator
-        evaluator = FeatureEvaluator()
-        ```
-        
-        Match the rules in the dataset:
-        ```python
-        #match single feature
-        df = dataset.to_dataframe()
-        evaluator.match_features(df, rule_to_match)
-        ```
-        
-        |    | Sentence                                                                                                                        | Predicted label           | Matched rule                                        |
-        |---:|:--------------------------------------------------------------------------------------------------------------------------------|:--------------------------|:----------------------------------------------------|
-        |  0 | Governments and industries in nations around the world are pouring XXX into YYY.                                                | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        |  1 | The scientists poured XXX into pint YYY.                                                                                        | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        |  2 | The suspect pushed the XXX into a deep YYY.                                                                                     | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        |  3 | The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.                                  | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        |  4 | The entity1 to buy papers is pushed into the next entity2.                                                                      | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        |  5 | An unnamed XXX was pushed into the YYY.                                                                                         | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        |  6 | Since then, numerous independent feature XXX have journeyed into YYY.                                                           | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        |  7 | For some reason, the XXX was blinded from his own YYY about the incommensurability of time.                                     |                           |                                                     |
-        |  8 | Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.           |                           |                                                     |
-        |  9 | Olympics have already poured one XXX into the YYY.                                                                              | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        | 10 | After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.                            |                           |                                                     |
-        | 11 | I placed the XXX in a natural YYY, at the base of a part of the fallen arch.                                                    |                           |                                                     |
-        | 12 | The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.            |                           |                                                     |
-        | 13 | The XXX leaked from every conceivable YYY.                                                                                      |                           |                                                     |
-        | 14 | The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse. | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        | 15 | The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.                   |                           |                                                     |
-        | 16 | Gaza XXX recover from three YYY of war.                                                                                         |                           |                                                     |
-        | 17 | This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.  |                           |                                                     |
-        
-        
-        
-        You can see in the dataset that the rules only matched the instances where the "into" node was present.
-        
-        One of the core features of our tool is that we are also able to match subgraphs. To describe a graph, we use the [PENMAN](https://github.com/goodmami/penman) notation. 
-        
-        E.g. the string _(u_1 / into :1 (u_3 / pour))_ would describe a graph with two nodes ("into" and "pour") and a single directed edge with the label "1" between them.
-        ```python
-        #match a simple graph feature
-        evaluator.match_features(df, [[["(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))"], [], "Entity-Destination(e1,e2)"]])
-        ```
-        
-        Describing a subgraph with the string "(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))" will return only three examples instead of 9 (when we only had a single node as a feature)
-        |    | Sentence                                                                                                                        | Predicted label           | Matched rule                                                                       |
-        |---:|:--------------------------------------------------------------------------------------------------------------------------------|:--------------------------|:-----------------------------------------------------------------------------------|
-        |  0 | Governments and industries in nations around the world are pouring XXX into YYY.                                                | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        |  1 | The scientists poured XXX into pint YYY.                                                                                        | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        |  2 | The suspect pushed the XXX into a deep YYY.                                                                                     |                           |                                                                                    |
-        |  3 | The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.                                  |                           |                                                                                    |
-        |  4 | The entity1 to buy papers is pushed into the next entity2.                                                                      |                           |                                                                                    |
-        |  5 | An unnamed XXX was pushed into the YYY.                                                                                         |                           |                                                                                    |
-        |  6 | Since then, numerous independent feature XXX have journeyed into YYY.                                                           |                           |                                                                                    |
-        |  7 | For some reason, the XXX was blinded from his own YYY about the incommensurability of time.                                     |                           |                                                                                    |
-        |  8 | Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.           |                           |                                                                                    |
-        |  9 | Olympics have already poured one XXX into the YYY.                                                                              | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        | 10 | After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.                            |                           |                                                                                    |
-        | 11 | I placed the XXX in a natural YYY, at the base of a part of the fallen arch.                                                    |                           |                                                                                    |
-        | 12 | The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.            |                           |                                                                                    |
-        | 13 | The XXX leaked from every conceivable YYY.                                                                                      |                           |                                                                                    |
-        | 14 | The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse. |                           |                                                                                    |
-        | 15 | The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.                   |                           |                                                                                    |
-        | 16 | Gaza XXX recover from three YYY of war.                                                                                         |                           |                                                                                    |
-        | 17 | This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.  |                           |                                                                                    |
-        
-        
-        We can also add negated features that we don't want to match (e.g. this won't match the first row where 'pour' is present):
-        ```python
-        #match a simple graph feature
-        evaluator.match_features(df, [[["(u_1 / into :2 (u_3 / YYY))"], ["(u_2 / pour)"], "Entity-Destination(e1,e2)"]])
-        ```
-        
-        |    | Sentence                                                                                                                        | Predicted label           | Matched rule                                                                     |
-        |---:|:--------------------------------------------------------------------------------------------------------------------------------|:--------------------------|:---------------------------------------------------------------------------------|
-        |  0 | Governments and industries in nations around the world are pouring XXX into YYY.                                                |                           |                                                                                  |
-        |  1 | The scientists poured XXX into pint YYY.                                                                                        |                           |                                                                                  |
-        |  2 | The suspect pushed the XXX into a deep YYY.                                                                                     | Entity-Destination(e1,e2) | [['(u_1 / into :2 (u_3 / YYY))'], ['(u_2 / pour)'], 'Entity-Destination(e1,e2)'] |
-        |  3 | The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.                                  | Entity-Destination(e1,e2) | [['(u_1 / into :2 (u_3 / YYY))'], ['(u_2 / pour)'], 'Entity-Destination(e1,e2)'] |
-        |  4 | The entity1 to buy papers is pushed into the next entity2.                                                                      |                           |                                                                                  |
-        |  5 | An unnamed XXX was pushed into the YYY.                                                                                         | Entity-Destination(e1,e2) | [['(u_1 / into :2 (u_3 / YYY))'], ['(u_2 / pour)'], 'Entity-Destination(e1,e2)'] |
-        |  6 | Since then, numerous independent feature XXX have journeyed into YYY.                                                           | Entity-Destination(e1,e2) | [['(u_1 / into :2 (u_3 / YYY))'], ['(u_2 / pour)'], 'Entity-Destination(e1,e2)'] |
-        |  7 | For some reason, the XXX was blinded from his own YYY about the incommensurability of time.                                     |                           |                                                                                  |
-        |  8 | Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.           |                           |                                                                                  |
-        |  9 | Olympics have already poured one XXX into the YYY.                                                                              |                           |                                                                                  |
-        | 10 | After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.                            |                           |                                                                                  |
-        | 11 | I placed the XXX in a natural YYY, at the base of a part of the fallen arch.                                                    |                           |                                                                                  |
-        | 12 | The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.            |                           |                                                                                  |
-        | 13 | The XXX leaked from every conceivable YYY.                                                                                      |                           |                                                                                  |
-        | 14 | The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse. |                           |                                                                                  |
-        | 15 | The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.                   |                           |                                                                                  |
-        | 16 | Gaza XXX recover from three YYY of war.                                                                                         |                           |                                                                                  |
-        | 17 | This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.  |                           |                                                                                  |
-        
-        If we don't want to specify nodes, regex can also be used in place of the node and edge-names:
-        
-        ```python
-        #regex can be used to match any node (this will match instances where 'into' is connected to any node with '1' edge)
-        evaluator.match_features(df, [[["(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))"], [], "Entity-Destination(e1,e2)"]])
-        ```
-        
-        |    | Sentence                                                                                                                        | Predicted label           | Matched rule                                                                     |
-        |---:|:--------------------------------------------------------------------------------------------------------------------------------|:--------------------------|:---------------------------------------------------------------------------------|
-        |  0 | Governments and industries in nations around the world are pouring XXX into YYY.                                                | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        |  1 | The scientists poured XXX into pint YYY.                                                                                        | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        |  2 | The suspect pushed the XXX into a deep YYY.                                                                                     | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        |  3 | The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.                                  | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        |  4 | The entity1 to buy papers is pushed into the next entity2.                                                                      |                           |                                                                                  |
-        |  5 | An unnamed XXX was pushed into the YYY.                                                                                         | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        |  6 | Since then, numerous independent feature XXX have journeyed into YYY.                                                           | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        |  7 | For some reason, the XXX was blinded from his own YYY about the incommensurability of time.                                     |                           |                                                                                  |
-        |  8 | Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.           |                           |                                                                                  |
-        |  9 | Olympics have already poured one XXX into the YYY.                                                                              | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        | 10 | After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.                            |                           |                                                                                  |
-        | 11 | I placed the XXX in a natural YYY, at the base of a part of the fallen arch.                                                    |                           |                                                                                  |
-        | 12 | The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.            |                           |                                                                                  |
-        | 13 | The XXX leaked from every conceivable YYY.                                                                                      |                           |                                                                                  |
-        | 14 | The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse. |                           |                                                                                  |
-        | 15 | The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.                   |                           |                                                                                  |
-        | 16 | Gaza XXX recover from three YYY of war.                                                                                         |                           |                                                                                  |
-        | 17 | This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.  |                           |                                                                                  |
-        
-        We can also train regex rules from a training data, this will automatically replace regex '.*' with nodes that are 
-        'good enough' statistically based on the provided dataframe.
-        
-        ```python
-        evaluator.train_feature("Entity-Destination(e1,e2)", "(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))", df)
-        ```
-        
-        This returns '(u_1 / into :1 (u_2 / push|pour) :2 (u_3 / YYY))' (replaced '.*' with _push_ and _pour_)
-        
-        ### Learning rules
-        
-        To extract rules automatically, train the dataset with graph features and rank them based on relevancy:
-        
-        ```python
-        df = dataset.to_dataframe()
-        trainer = GraphTrainer(df)
-        #extract features
-        features = trainer.prepare_and_train()
-        
-        from xpotato.dataset.utils import save_dataframe
-        from sklearn.model_selection import train_test_split
-        
-        train, val = train_test_split(df, test_size=0.2, random_state=1234)
-        
-        #save train and validation, this is important for the frontend to work
-        save_dataframe(train, 'train.tsv')
-        save_dataframe(val, 'val.tsv')
-        
-        import json
-        
-        #also save the ranked features
-        with open("features.json", "w+") as f:
-            json.dump(features, f)
-        
-        ```
-        
-        You can also save the parsed graphs for evaluation or for caching:
-        
-        ```python
-        import pickle
-        with open("graphs.pickle", "wb") as f:
-            pickle.dump(val.graph, f)
-        ```
-        
-        ## Frontend
-        
-        If the DataFrame is ready with the parsed graphs, the UI can be started to inspect the extracted rules and modify them. The frontend is a streamlit app, the simplest way of starting it is (the training and the validation dataset must be provided):
-        
-        ```
-        streamlit run frontend/app.py -- -t notebooks/train.tsv -v notebooks/val.tsv -g ud
-        ```
-        
-        it can be also started with the extracted features:
-        
-        ```
-        streamlit run frontend/app.py -- -t notebooks/train.tsv -v notebooks/val.tsv -g ud -sr notebooks/features.json
-        ```
-        
-        if you already used the UI and extracted the features manually and you want to load it, you can run:
-        ```
-        streamlit run frontend/app.py -- -t notebooks/train.tsv -v notebooks/val.tsv -g ud -sr notebooks/features.json -hr notebooks/manual_features.json
-        ```
-        
-        ### Advanced mode
-        
-        If labels are not or just partially provided, the frontend can be started also in _advanced_ mode, where the user can _annotate_ a few examples at the start, then the system gradually offers rules based on the provided examples. 
-        
-        
-        Dataset without labels can be initialized with:
-        ```python
-        sentences = [("Governments and industries in nations around the world are pouring XXX into YYY.", ""),
-                    ("The scientists poured XXX into pint YYY.", ""),
-                    ("The suspect pushed the XXX into a deep YYY.", ""),
-                    ("The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.", ""),
-                    ("The entity1 to buy papers is pushed into the next entity2.", ""),
-                    ("An unnamed XXX was pushed into the YYY.", ""),
-                    ("Since then, numerous independent feature XXX have journeyed into YYY.", ""),
-                    ("For some reason, the XXX was blinded from his own YYY about the incommensurability of time.", ""),
-                    ("Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.", ""),
-                    ("Olympics have already poured one XXX into the YYY.", ""),
-                    ("After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.", ""),
-                    ("I placed the XXX in a natural YYY, at the base of a part of the fallen arch.", ""),
-                    ("The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.", ""),
-                    ("The XXX leaked from every conceivable YYY.", ""),
-                    ("The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse.", ""),
-                    ("The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.", ""),
-                    ("Gaza XXX recover from three YYY of war.", ""),
-                    ("This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.", "")]
-        ```
-        
-        
-        Then, the frontend can be started:
-        ```
-        streamlit run frontend/app.py -- -t notebooks/unsupervised_dataset.tsv -g ud -m advanced
-        ```
-        
-        Once the frontend starts up and you define the labels, you are faced with the annotation interface. You can search elements by clicking on the appropriate column name and applying the desired filter. You can annotate instances by checking the checkbox at the beginning of the line. You can check multiple checkboxs at a time. Once you've selected the utterances you want to annotate, click on the _Annotate_ button. The annotated samples will appear in the lower table. You can clear the annotation of certain elements by selecting them in the second table and clicking _Clear annotation_.
-        
-        Once you have some annotated data, you can train rules by clicking the _Train!_ button. It is recommended to set the _Rank features based on accuracy_ to True, if you have just a few samples. You will get a similar interface as in supervised mode, you can generate rule suggestions, and write your own rules as usual. Once you are satisfied with the rules, select each of them and click _annotate based on selected_. This process might take a while if you are working with large data. You should get all the rule matches marked in the first and the second tables. You can order the tables by each column, so it's easier to check. You will have to manually accept the annotations generated this way for them to appear in the second table.
-        
-        - You can read about the use of the advanced mode in the [docs](https://github.com/adaamko/POTATO/tree/main/docs/README_advanced_mode.md)
-        
-        
-        ## Evaluate
-        If you have the features ready and you want to evaluate them on a test set, you can run:
-        
-        ```python
-        python scripts/evaluate.py -t ud -f notebooks/features.json -d notebooks/val.tsv
-        ```
-        
-        The result will be a _csv_ file with the labels and the matched rules.
-        
-        ## Service
-        If you are ready with the extracted features and want to use our package in production for inference (generating predictions for sentences), we also provide a REST API built on POTATO (based on [fastapi](https://github.com/tiangolo/fastapi)).
-        
-        First install FastAPI and [Uvicorn](https://www.uvicorn.org/)
-        ```bash
-        pip install fastapi
-        pip install "uvicorn[standard]"
-        ```
-        
-        To start the service, you should set _language_, _graph\_type_ and the _features_  for the service. This can be done through enviroment variables.
-        
-        Example:
-        ```bash
-        export FEATURE_PATH=/home/adaamko/projects/POTATO/features/semeval/test_features.json
-        export GRAPH_FORMAT=ud
-        export LANG=en
-        ```
-        
-        Then, start the REST API:
-        ```python
-        python services/main.py
-        ```
-        
-        It will start a service running on _localhost_ on port _8000_ (it will also initialize the correct models).
-        
-        Then you can use any client to make post requests:
-        ```bash
-        curl -X POST localhost:8000 -H 'Content-Type: application/json' -d '{"text":"The suspect pushed the XXX into a deep YYY.\nSparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week."}'
-        ```
-        
-        The answer will be a list with the predicted labels (if none of the rules match, it will return "NONE"):
-        ```bash
-        ["Entity-Destination(e1,e2)","NONE"]
-        ```
-        
-        The streamlit frontend also has an inference mode, where the implemented rule-system can be used for inference. It can be started with:
-        
-        ```bash
-        streamlit run frontend/app.py -- -hr features/semeval/test_features.json -m inference
-        ```
-        
-        ## Contributing
-        
-        We welcome all contributions! Please fork this repository and create a branch for your modifications. We suggest getting in touch with us first, by opening an issue or by writing an email to Adam Kovacs or Gabor Recski at firstname.lastname@tuwien.ac.at
-        
-        ## Citing
-        
-        If you use the library, please cite our [paper](https://arxiv.org/abs/2201.13230)
-        
-        ```bib
-        @article{Kovacs:2022,
-          title={{POTATO: exPlainable infOrmation exTrAcTion framewOrk}},
-          author={Kov{\'a}cs, {\'A}d{\'a}m and G{\'e}mes, Kinga and Ikl{\'o}di, Eszter and Recski, G{\'a}bor},
-          journal={arXiv preprint arXiv:2201.13230},
-          year={2022}
-        }
-        ```
-        
-        ## License 
-        
-        MIT license
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
+<p align="center">
+  <img src="https://raw.githubusercontent.com/adaamko/POTATO/dev/files/potato_logo.png" />
+</p>
+
+# POTATO: exPlainable infOrmation exTrAcTion framewOrk
+POTATO is a human-in-the-loop XAI framework for extracting and evaluating interpretable graph features for any classification problem in Natural Language Processing.
+
+## Built systems
+
+To get started with rule-systems we provide rule-based features prebuilt with POTATO on different datasets (e.g. our paper _Offensive text detection on English Twitter with deep learning models and rule-based systems_ for the HASOC2021 shared task). If you are interested in that, you can go under _features/_ for more info!
+
+## Install and Quick Start
+Check out our quick demonstration (~2 min) video about the tool:
+https://youtu.be/PkQ71wUSeNU
+
+There is a longer version with a detailed method description and presented background research (~1 hour): https://youtu.be/6R_V1WfIjsU
+
+### Setup
+The tool is heavily dependent upon the [tuw-nlp](https://github.com/recski/tuw-nlp) repository. You can install tuw-nlp with pip:
+
+```
+pip install tuw-nlp
+```
+Then follow the [instructions](https://github.com/recski/tuw-nlp) to setup the package.
+
+
+Then install POTATO from pip:
+
+```
+pip install xpotato
+```
+
+Or you can install it from source:
+
+```
+pip install -e .
+```
+
+### Usage
+
+- POTATO is an IE tool that works on graphs, currently we support three types of graphs: AMR, UD and [Fourlang](https://github.com/kornai/4lang). 
+
+- In the README we provide examples with fourlang semantic graphs. Make sure to follow the instructions in the [tuw_nlp](https://github.com/recski/tuw-nlp) repo to be able to build fourlang graphs. 
+
+- If you are interested in AMR graphs, you can go to the [hasoc](https://github.com/adaamko/POTATO/tree/main/features/hasoc) folder To get started with rule-systems prebuilt with POTATO on the HASOC dataset (we also presented a paper named _Offensive text detection on English Twitter with deep learning models and rule-based systems_ for the HASOC2021 shared task). 
+
+- We also provide experiments on the [CrowdTruth](https://github.com/CrowdTruth/Medical-Relation-Extraction) medical relation extraction datasets with UD graphs, go to the [crowdtruth](https://github.com/adaamko/POTATO/tree/main/features/crowdtruth) folder for more info!
+
+- POTATO can also handle unlabeled, or partially labeled data, see [advanced](###advanced-mode) mode to get to know more.
+
+__To see complete working examples go under the _notebooks/_ folder to see experiments on HASOC and on the Semeval relation extraction dataset.__
+
+First import packages from potato:
+```python
+from xpotato.dataset.dataset import Dataset
+from xpotato.models.trainer import GraphTrainer
+```
+
+First we demonstrate POTATO's capabilities with a few sentences manually picked from the dataset.
+
+__Note that we replaced the two entitites in question with _XXX_ and _YYY_.__
+
+```python
+sentences = [("Governments and industries in nations around the world are pouring XXX into YYY.", "Entity-Destination(e1,e2)"),
+            ("The scientists poured XXX into pint YYY.", "Entity-Destination(e1,e2)"),
+            ("The suspect pushed the XXX into a deep YYY.", "Entity-Destination(e1,e2)"),
+            ("The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.", "Other"),
+            ("The entity1 to buy papers is pushed into the next entity2.", "Entity-Destination(e1,e2)"),
+            ("An unnamed XXX was pushed into the YYY.", "Entity-Destination(e1,e2)"),
+            ("Since then, numerous independent feature XXX have journeyed into YYY.", "Other"),
+            ("For some reason, the XXX was blinded from his own YYY about the incommensurability of time.", "Other"),
+            ("Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.", "Other"),
+            ("Olympics have already poured one XXX into the YYY.", "Entity-Destination(e1,e2)"),
+            ("After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.", "Entity-Destination(e1,e2)"),
+            ("I placed the XXX in a natural YYY, at the base of a part of the fallen arch.", "Entity-Destination(e1,e2)"),
+            ("The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.", "Other"),
+            ("The XXX leaked from every conceivable YYY.", "Other"),
+            ("The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse.", "Entity-Destination(e1,e2)"),
+            ("The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.", "Other"),
+            ("Gaza XXX recover from three YYY of war.", "Other"),
+            ("This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.", "Other")]
+```
+
+Initialize the dataset and also provide a label encoding. Then parse the sentences into graphs. Currently we provide three types of graphs: _ud_, _fourlang_, _amr_. Also provide the language you want to parse, currently we support English (en) and German (de).
+
+```python
+dataset = Dataset(sentences, label_vocab={"Other":0, "Entity-Destination(e1,e2)": 1}, lang="en")
+dataset.set_graphs(dataset.parse_graphs(graph_format="ud"))
+```
+
+Check the dataset:
+```python
+df = dataset.to_dataframe()
+```
+
+We can also check any of the graphs:
+### Check any of the graphs parsed
+
+```python
+from xpotato.models.utils import to_dot
+from graphviz import Source
+
+Source(to_dot(df.iloc[0].graph))
+```
+![graph](https://raw.githubusercontent.com/adaamko/POTATO/main/files/re_example.svg)
+
+### Rules
+
+If the dataset is prepared and the graphs are parsed, we can write rules to match labels. We can write rules either manually or extract
+them automatically (POTATO also provides a frontend that tries to do both).
+
+The simplest rule would be just a node in the graph:
+```python
+# The syntax of the rules is List[List[rules that we want to match], List[rules that shouldn't be in the matched graphs], Label of the rule]
+rule_to_match = [[["(u_1 / into)"], [], "Entity-Destination(e1,e2)"]]
+```
+
+Init the rule matcher:
+```python
+from xpotato.graph_extractor.extract import FeatureEvaluator
+evaluator = FeatureEvaluator()
+```
+
+Match the rules in the dataset:
+```python
+#match single feature
+df = dataset.to_dataframe()
+evaluator.match_features(df, rule_to_match)
+```
+
+|    | Sentence                                                                                                                        | Predicted label           | Matched rule                                        |
+|---:|:--------------------------------------------------------------------------------------------------------------------------------|:--------------------------|:----------------------------------------------------|
+|  0 | Governments and industries in nations around the world are pouring XXX into YYY.                                                | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+|  1 | The scientists poured XXX into pint YYY.                                                                                        | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+|  2 | The suspect pushed the XXX into a deep YYY.                                                                                     | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+|  3 | The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.                                  | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+|  4 | The entity1 to buy papers is pushed into the next entity2.                                                                      | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+|  5 | An unnamed XXX was pushed into the YYY.                                                                                         | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+|  6 | Since then, numerous independent feature XXX have journeyed into YYY.                                                           | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+|  7 | For some reason, the XXX was blinded from his own YYY about the incommensurability of time.                                     |                           |                                                     |
+|  8 | Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.           |                           |                                                     |
+|  9 | Olympics have already poured one XXX into the YYY.                                                                              | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+| 10 | After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.                            |                           |                                                     |
+| 11 | I placed the XXX in a natural YYY, at the base of a part of the fallen arch.                                                    |                           |                                                     |
+| 12 | The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.            |                           |                                                     |
+| 13 | The XXX leaked from every conceivable YYY.                                                                                      |                           |                                                     |
+| 14 | The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse. | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+| 15 | The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.                   |                           |                                                     |
+| 16 | Gaza XXX recover from three YYY of war.                                                                                         |                           |                                                     |
+| 17 | This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.  |                           |                                                     |
+
+
+
+You can see in the dataset that the rules only matched the instances where the "into" node was present.
+
+One of the core features of our tool is that we are also able to match subgraphs. To describe a graph, we use the [PENMAN](https://github.com/goodmami/penman) notation. 
+
+E.g. the string _(u_1 / into :1 (u_3 / pour))_ would describe a graph with two nodes ("into" and "pour") and a single directed edge with the label "1" between them.
+```python
+#match a simple graph feature
+evaluator.match_features(df, [[["(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))"], [], "Entity-Destination(e1,e2)"]])
+```
+
+Describing a subgraph with the string "(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))" will return only three examples instead of 9 (when we only had a single node as a feature)
+|    | Sentence                                                                                                                        | Predicted label           | Matched rule                                                                       |
+|---:|:--------------------------------------------------------------------------------------------------------------------------------|:--------------------------|:-----------------------------------------------------------------------------------|
+|  0 | Governments and industries in nations around the world are pouring XXX into YYY.                                                | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+|  1 | The scientists poured XXX into pint YYY.                                                                                        | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+|  2 | The suspect pushed the XXX into a deep YYY.                                                                                     |                           |                                                                                    |
+|  3 | The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.                                  |                           |                                                                                    |
+|  4 | The entity1 to buy papers is pushed into the next entity2.                                                                      |                           |                                                                                    |
+|  5 | An unnamed XXX was pushed into the YYY.                                                                                         |                           |                                                                                    |
+|  6 | Since then, numerous independent feature XXX have journeyed into YYY.                                                           |                           |                                                                                    |
+|  7 | For some reason, the XXX was blinded from his own YYY about the incommensurability of time.                                     |                           |                                                                                    |
+|  8 | Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.           |                           |                                                                                    |
+|  9 | Olympics have already poured one XXX into the YYY.                                                                              | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+| 10 | After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.                            |                           |                                                                                    |
+| 11 | I placed the XXX in a natural YYY, at the base of a part of the fallen arch.                                                    |                           |                                                                                    |
+| 12 | The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.            |                           |                                                                                    |
+| 13 | The XXX leaked from every conceivable YYY.                                                                                      |                           |                                                                                    |
+| 14 | The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse. |                           |                                                                                    |
+| 15 | The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.                   |                           |                                                                                    |
+| 16 | Gaza XXX recover from three YYY of war.                                                                                         |                           |                                                                                    |
+| 17 | This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.  |                           |                                                                                    |
+
+
+We can also add negated features that we don't want to match (e.g. this won't match the first row where 'pour' is present):
+```python
+#match a simple graph feature
+evaluator.match_features(df, [[["(u_1 / into :2 (u_3 / YYY))"], ["(u_2 / pour)"], "Entity-Destination(e1,e2)"]])
+```
+
+|    | Sentence                                                                                                                        | Predicted label           | Matched rule                                                                     |
+|---:|:--------------------------------------------------------------------------------------------------------------------------------|:--------------------------|:---------------------------------------------------------------------------------|
+|  0 | Governments and industries in nations around the world are pouring XXX into YYY.                                                |                           |                                                                                  |
+|  1 | The scientists poured XXX into pint YYY.                                                                                        |                           |                                                                                  |
+|  2 | The suspect pushed the XXX into a deep YYY.                                                                                     | Entity-Destination(e1,e2) | [['(u_1 / into :2 (u_3 / YYY))'], ['(u_2 / pour)'], 'Entity-Destination(e1,e2)'] |
+|  3 | The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.                                  | Entity-Destination(e1,e2) | [['(u_1 / into :2 (u_3 / YYY))'], ['(u_2 / pour)'], 'Entity-Destination(e1,e2)'] |
+|  4 | The entity1 to buy papers is pushed into the next entity2.                                                                      |                           |                                                                                  |
+|  5 | An unnamed XXX was pushed into the YYY.                                                                                         | Entity-Destination(e1,e2) | [['(u_1 / into :2 (u_3 / YYY))'], ['(u_2 / pour)'], 'Entity-Destination(e1,e2)'] |
+|  6 | Since then, numerous independent feature XXX have journeyed into YYY.                                                           | Entity-Destination(e1,e2) | [['(u_1 / into :2 (u_3 / YYY))'], ['(u_2 / pour)'], 'Entity-Destination(e1,e2)'] |
+|  7 | For some reason, the XXX was blinded from his own YYY about the incommensurability of time.                                     |                           |                                                                                  |
+|  8 | Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.           |                           |                                                                                  |
+|  9 | Olympics have already poured one XXX into the YYY.                                                                              |                           |                                                                                  |
+| 10 | After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.                            |                           |                                                                                  |
+| 11 | I placed the XXX in a natural YYY, at the base of a part of the fallen arch.                                                    |                           |                                                                                  |
+| 12 | The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.            |                           |                                                                                  |
+| 13 | The XXX leaked from every conceivable YYY.                                                                                      |                           |                                                                                  |
+| 14 | The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse. |                           |                                                                                  |
+| 15 | The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.                   |                           |                                                                                  |
+| 16 | Gaza XXX recover from three YYY of war.                                                                                         |                           |                                                                                  |
+| 17 | This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.  |                           |                                                                                  |
+
+If we don't want to specify nodes, regex can also be used in place of the node and edge-names:
+
+```python
+#regex can be used to match any node (this will match instances where 'into' is connected to any node with '1' edge)
+evaluator.match_features(df, [[["(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))"], [], "Entity-Destination(e1,e2)"]])
+```
+
+|    | Sentence                                                                                                                        | Predicted label           | Matched rule                                                                     |
+|---:|:--------------------------------------------------------------------------------------------------------------------------------|:--------------------------|:---------------------------------------------------------------------------------|
+|  0 | Governments and industries in nations around the world are pouring XXX into YYY.                                                | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+|  1 | The scientists poured XXX into pint YYY.                                                                                        | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+|  2 | The suspect pushed the XXX into a deep YYY.                                                                                     | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+|  3 | The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.                                  | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+|  4 | The entity1 to buy papers is pushed into the next entity2.                                                                      |                           |                                                                                  |
+|  5 | An unnamed XXX was pushed into the YYY.                                                                                         | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+|  6 | Since then, numerous independent feature XXX have journeyed into YYY.                                                           | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+|  7 | For some reason, the XXX was blinded from his own YYY about the incommensurability of time.                                     |                           |                                                                                  |
+|  8 | Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.           |                           |                                                                                  |
+|  9 | Olympics have already poured one XXX into the YYY.                                                                              | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+| 10 | After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.                            |                           |                                                                                  |
+| 11 | I placed the XXX in a natural YYY, at the base of a part of the fallen arch.                                                    |                           |                                                                                  |
+| 12 | The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.            |                           |                                                                                  |
+| 13 | The XXX leaked from every conceivable YYY.                                                                                      |                           |                                                                                  |
+| 14 | The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse. |                           |                                                                                  |
+| 15 | The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.                   |                           |                                                                                  |
+| 16 | Gaza XXX recover from three YYY of war.                                                                                         |                           |                                                                                  |
+| 17 | This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.  |                           |                                                                                  |
+
+We can also train regex rules from a training data, this will automatically replace regex '.*' with nodes that are 
+'good enough' statistically based on the provided dataframe.
+
+```python
+evaluator.train_feature("Entity-Destination(e1,e2)", "(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))", df)
+```
+
+This returns '(u_1 / into :1 (u_2 / push|pour) :2 (u_3 / YYY))' (replaced '.*' with _push_ and _pour_)
+
+### Learning rules
+
+To extract rules automatically, train the dataset with graph features and rank them based on relevancy:
+
+```python
+df = dataset.to_dataframe()
+trainer = GraphTrainer(df)
+#extract features
+features = trainer.prepare_and_train()
+
+from xpotato.dataset.utils import save_dataframe
+from sklearn.model_selection import train_test_split
+
+train, val = train_test_split(df, test_size=0.2, random_state=1234)
+
+#save train and validation, this is important for the frontend to work
+save_dataframe(train, 'train.tsv')
+save_dataframe(val, 'val.tsv')
+
+import json
+
+#also save the ranked features
+with open("features.json", "w+") as f:
+    json.dump(features, f)
+
+```
+
+You can also save the parsed graphs for evaluation or for caching:
+
+```python
+import pickle
+with open("graphs.pickle", "wb") as f:
+    pickle.dump(val.graph, f)
+```
+
+## Frontend
+
+If the DataFrame is ready with the parsed graphs, the UI can be started to inspect the extracted rules and modify them. The frontend is a streamlit app, the simplest way of starting it is (the training and the validation dataset must be provided):
+
+```
+streamlit run frontend/app.py -- -t notebooks/train.tsv -v notebooks/val.tsv -g ud
+```
+
+it can be also started with the extracted features:
+
+```
+streamlit run frontend/app.py -- -t notebooks/train.tsv -v notebooks/val.tsv -g ud -sr notebooks/features.json
+```
+
+if you already used the UI and extracted the features manually and you want to load it, you can run:
+```
+streamlit run frontend/app.py -- -t notebooks/train.tsv -v notebooks/val.tsv -g ud -sr notebooks/features.json -hr notebooks/manual_features.json
+```
+
+### Advanced mode
+
+If labels are not or just partially provided, the frontend can be started also in _advanced_ mode, where the user can _annotate_ a few examples at the start, then the system gradually offers rules based on the provided examples. 
+
+
+Dataset without labels can be initialized with:
+```python
+sentences = [("Governments and industries in nations around the world are pouring XXX into YYY.", ""),
+            ("The scientists poured XXX into pint YYY.", ""),
+            ("The suspect pushed the XXX into a deep YYY.", ""),
+            ("The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.", ""),
+            ("The entity1 to buy papers is pushed into the next entity2.", ""),
+            ("An unnamed XXX was pushed into the YYY.", ""),
+            ("Since then, numerous independent feature XXX have journeyed into YYY.", ""),
+            ("For some reason, the XXX was blinded from his own YYY about the incommensurability of time.", ""),
+            ("Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.", ""),
+            ("Olympics have already poured one XXX into the YYY.", ""),
+            ("After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.", ""),
+            ("I placed the XXX in a natural YYY, at the base of a part of the fallen arch.", ""),
+            ("The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.", ""),
+            ("The XXX leaked from every conceivable YYY.", ""),
+            ("The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse.", ""),
+            ("The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.", ""),
+            ("Gaza XXX recover from three YYY of war.", ""),
+            ("This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.", "")]
+```
+
+
+Then, the frontend can be started:
+```
+streamlit run frontend/app.py -- -t notebooks/unsupervised_dataset.tsv -g ud -m advanced
+```
+
+Once the frontend starts up and you define the labels, you are faced with the annotation interface. You can search elements by clicking on the appropriate column name and applying the desired filter. You can annotate instances by checking the checkbox at the beginning of the line. You can check multiple checkboxs at a time. Once you've selected the utterances you want to annotate, click on the _Annotate_ button. The annotated samples will appear in the lower table. You can clear the annotation of certain elements by selecting them in the second table and clicking _Clear annotation_.
+
+Once you have some annotated data, you can train rules by clicking the _Train!_ button. It is recommended to set the _Rank features based on accuracy_ to True, if you have just a few samples. You will get a similar interface as in supervised mode, you can generate rule suggestions, and write your own rules as usual. Once you are satisfied with the rules, select each of them and click _annotate based on selected_. This process might take a while if you are working with large data. You should get all the rule matches marked in the first and the second tables. You can order the tables by each column, so it's easier to check. You will have to manually accept the annotations generated this way for them to appear in the second table.
+
+- You can read about the use of the advanced mode in the [docs](https://github.com/adaamko/POTATO/tree/main/docs/README_advanced_mode.md)
+
+
+## Evaluate
+If you have the features ready and you want to evaluate them on a test set, you can run:
+
+```python
+python scripts/evaluate.py -t ud -f notebooks/features.json -d notebooks/val.tsv
+```
+
+The result will be a _csv_ file with the labels and the matched rules.
+
+## Service
+If you are ready with the extracted features and want to use our package in production for inference (generating predictions for sentences), we also provide a REST API built on POTATO (based on [fastapi](https://github.com/tiangolo/fastapi)).
+
+First install FastAPI and [Uvicorn](https://www.uvicorn.org/)
+```bash
+pip install fastapi
+pip install "uvicorn[standard]"
+```
+
+To start the service, you should set _language_, _graph\_type_ and the _features_  for the service. This can be done through enviroment variables.
+
+Example:
+```bash
+export FEATURE_PATH=/home/adaamko/projects/POTATO/features/semeval/test_features.json
+export GRAPH_FORMAT=ud
+export LANG=en
+```
+
+Then, start the REST API:
+```python
+python services/main.py
+```
+
+It will start a service running on _localhost_ on port _8000_ (it will also initialize the correct models).
+
+Then you can use any client to make post requests:
+```bash
+curl -X POST localhost:8000 -H 'Content-Type: application/json' -d '{"text":"The suspect pushed the XXX into a deep YYY.\nSparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week."}'
+```
+
+The answer will be a list with the predicted labels (if none of the rules match, it will return "NONE"):
+```bash
+["Entity-Destination(e1,e2)","NONE"]
+```
+
+The streamlit frontend also has an inference mode, where the implemented rule-system can be used for inference. It can be started with:
+
+```bash
+streamlit run frontend/app.py -- -hr features/semeval/test_features.json -m inference
+```
+
+## Contributing
+
+We welcome all contributions! Please fork this repository and create a branch for your modifications. We suggest getting in touch with us first, by opening an issue or by writing an email to Adam Kovacs or Gabor Recski at firstname.lastname@tuwien.ac.at
+
+## Citing
+
+If you use the library, please cite our [paper](https://dl.acm.org/doi/abs/10.1145/3511808.3557196) published in CIKM 2022:
+
+```bib
+@inproceedings{Kovacs:2022,
+author = {Kov\'{a}cs, \'{A}d\'{a}m and G\'{e}mes, Kinga and Ikl\'{o}di, Eszter and Recski, G\'{a}bor},
+title = {POTATO: ExPlainable InfOrmation ExTrAcTion FramewOrk},
+year = {2022},
+isbn = {9781450392365},
+publisher = {Association for Computing Machinery},
+address = {New York, NY, USA},
+url = {https://doi.org/10.1145/3511808.3557196},
+doi = {10.1145/3511808.3557196},
+booktitle = {Proceedings of the 31st ACM International Conference on Information & Knowledge Management},
+pages = {4897–4901},
+numpages = {5},
+keywords = {explainability, explainable, hitl},
+location = {Atlanta, GA, USA},
+series = {CIKM '22}
+}
+```
+
+## License 
+
+MIT license
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xpotato-0.1.4/README.md` & `xpotato-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: xpotato
+Version: 0.1.5
+Summary: XAI human-in-the-loop information extraction framework
+Home-page: https://github.com/adaamko/POTATO
+Author: Adam Kovacs, Gabor Recski
+Author-email: adam.kovacs@tuwien.ac.at, gabor.recski@tuwien.ac.at
+License: MIT
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
   <img src="https://raw.githubusercontent.com/adaamko/POTATO/dev/files/potato_logo.png" />
 </p>
 
 # POTATO: exPlainable infOrmation exTrAcTion framewOrk
 POTATO is a human-in-the-loop XAI framework for extracting and evaluating interpretable graph features for any classification problem in Natural Language Processing.
 
@@ -394,21 +415,33 @@
 
 ## Contributing
 
 We welcome all contributions! Please fork this repository and create a branch for your modifications. We suggest getting in touch with us first, by opening an issue or by writing an email to Adam Kovacs or Gabor Recski at firstname.lastname@tuwien.ac.at
 
 ## Citing
 
-If you use the library, please cite our [paper](https://arxiv.org/abs/2201.13230)
+If you use the library, please cite our [paper](https://dl.acm.org/doi/abs/10.1145/3511808.3557196) published in CIKM 2022:
 
 ```bib
-@article{Kovacs:2022,
-  title={{POTATO: exPlainable infOrmation exTrAcTion framewOrk}},
-  author={Kov{\'a}cs, {\'A}d{\'a}m and G{\'e}mes, Kinga and Ikl{\'o}di, Eszter and Recski, G{\'a}bor},
-  journal={arXiv preprint arXiv:2201.13230},
-  year={2022}
+@inproceedings{Kovacs:2022,
+author = {Kov\'{a}cs, \'{A}d\'{a}m and G\'{e}mes, Kinga and Ikl\'{o}di, Eszter and Recski, G\'{a}bor},
+title = {POTATO: ExPlainable InfOrmation ExTrAcTion FramewOrk},
+year = {2022},
+isbn = {9781450392365},
+publisher = {Association for Computing Machinery},
+address = {New York, NY, USA},
+url = {https://doi.org/10.1145/3511808.3557196},
+doi = {10.1145/3511808.3557196},
+booktitle = {Proceedings of the 31st ACM International Conference on Information & Knowledge Management},
+pages = {4897–4901},
+numpages = {5},
+keywords = {explainability, explainable, hitl},
+location = {Atlanta, GA, USA},
+series = {CIKM '22}
 }
 ```
 
 ## License 
 
 MIT license
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xpotato-0.1.4/frontend/app.py` & `xpotato-0.1.5/frontend/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 import argparse
 import copy
+import json
 import os
 import time
-import json
-import streamlit as st
+
 import pandas as pd
 import penman
+import streamlit as st
 from graphviz import Source
-
 from st_aggrid import AgGrid, GridOptionsBuilder, GridUpdateMode
 from tuw_nlp.graph.utils import graph_to_pn
-
 from utils import (
-    train_df,
     add_rule_manually,
     annotate_df,
     extract_data_from_dataframe,
     get_df_from_rules,
     graph_viewer,
     init_evaluator,
     init_extractor,
     init_session_states,
+    match_texts,
     rank_and_suggest,
     read_df,
+    read_ruleset,
     rerun,
     rule_chooser,
-    save_ruleset,
-    read_ruleset,
     save_after_modify,
     save_dataframe,
-    match_texts,
+    save_ruleset,
     show_ml_feature,
     st_stdout,
     to_dot,
+    train_df,
 )
 
 
 def inference_mode(evaluator, hand_made_rules):
     st.sidebar.title("Inference Mode")
     st.sidebar.markdown(
         """
```

### Comparing `xpotato-0.1.4/frontend/utils.py` & `xpotato-0.1.5/frontend/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import copy
 import json
 import re
 import sys
 from ast import literal_eval
-
 from collections import defaultdict
-from graphviz import Source
+from contextlib import contextmanager
+from io import StringIO
+from threading import current_thread
+
 import pandas as pd
-from st_aggrid import AgGrid, GridOptionsBuilder, GridUpdateMode
-import streamlit as st
 import penman
+import streamlit as st
 import torch
+from graphviz import Source
+from st_aggrid import AgGrid, GridOptionsBuilder, GridUpdateMode
 from streamlit.report_thread import REPORT_CONTEXT_ATTR_NAME
+from tuw_nlp.graph.utils import GraphFormulaPatternMatcher, graph_to_pn
 
+from xpotato.dataset.dataset import Dataset
 from xpotato.dataset.utils import default_pn_to_graph
-from xpotato.graph_extractor.graph import PotatoGraph
 from xpotato.graph_extractor.extract import FeatureEvaluator, GraphExtractor
+from xpotato.graph_extractor.graph import PotatoGraph
+from xpotato.graph_extractor.rule import Rule, RuleSet
 from xpotato.models.trainer import GraphTrainer
-from xpotato.dataset.utils import default_pn_to_graph
-from xpotato.graph_extractor.rule import RuleSet, Rule
-from tuw_nlp.graph.utils import GraphFormulaPatternMatcher, graph_to_pn
-
-from contextlib import contextmanager
-from io import StringIO
-from threading import current_thread
 
 
 def rerun():
     raise st.experimental_rerun()
 
 
 @st.cache(
@@ -247,41 +246,35 @@
     save_rules = hand_made_rules or "saved_features.tsv"
     save_ruleset(save_rules, st.session_state.features)
     st.session_state.rows_to_delete = []
     rerun()
 
 
 def filter_label(df, label):
-    df["label"] = df.apply(lambda x: label if label in literal_eval(x["labels"]) else "NOT", axis=1)
+    df["label"] = df.apply(
+        lambda x: label if label in literal_eval(x["labels"]) else "NOT", axis=1
+    )
     df["label_id"] = df.apply(lambda x: 0 if x["label"] == "NOT" else 1, axis=1)
 
 
 @st.cache(allow_output_mutation=True)
 def read_df(path, label=None, binary=False):
-    if binary:
-        df = pd.read_pickle(path)
-    else:
-        df = pd.read_csv(path, sep="\t")
-        graphs = []
-        for graph in df["graph"]:
-            potato_graph = PotatoGraph(graph_str=graph)
-            graphs.append(potato_graph.graph)
-        df["graph"] = graphs
+    dataset = Dataset(path=path, binary=binary)
+    df = dataset.to_dataframe()
+
     if label is not None:
         filter_label(df, label)
     return df
 
 
 def save_dataframe(data, path):
     if ".pickle" in path:
         data.to_pickle(path)
     else:
-        graphs = data["graph"]
-        data["graph"] = [graph_to_pn(graph) for graph in graphs]
-        data.to_csv(path, sep="\t", index=False)
+        Dataset.save_dataframe(data, path)
 
 
 def train_df(df, min_edge=0, rank=False):
     with st_stdout("code"):
         trainer = GraphTrainer(df)
         features = trainer.prepare_and_train(min_edge=min_edge, rank=rank)
```

### Comparing `xpotato-0.1.4/setup.py` & `xpotato-0.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from setuptools import find_packages, setup
 
-
-
-
 setup(
     name="xpotato",
-    version="0.1.4",
+    version="0.1.5",
     description="XAI human-in-the-loop information extraction framework",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/adaamko/POTATO",
     author="Adam Kovacs, Gabor Recski",
     author_email="adam.kovacs@tuwien.ac.at, gabor.recski@tuwien.ac.at",
     license="MIT",
@@ -20,23 +17,23 @@
         "scikit-learn == 1.0.2",
         "eli5 == 0.11.0",
         "jinja2 == 3.0.1",
         "graphviz == 0.18.2",
         "penman >= 1.2.1",
         "networkx == 2.6.3",
         "rank_bm25 == 0.2.1",
-        "streamlit == 1.3.1",
+        "streamlit == 1.15.0",
         "streamlit-aggrid == 0.2.3.post2",
         "scikit-criteria == 0.5",
-        "tuw-nlp == 0.0.9",
+        "tuw-nlp == 0.1.0",
         "amrlib == 0.6.0",
         "protobuf==3.20.0",
         "pytest >= 7.1.3",
         "fastapi",
-        "uvicorn[standard]"
+        "uvicorn[standard]",
     ],
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
```

### Comparing `xpotato-0.1.4/xpotato/dataset/__pycache__/dataset.cpython-39.pyc` & `xpotato-0.1.5/xpotato/dataset/__pycache__/dataset.cpython-37.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Apr 20 07:22:19 2022 UTC, .py size: 5333 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,389 +1,415 @@
-00000000: 610d 0d0a 0000 0000 abb4 5f62 d514 0000  a........._b....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
-00000050: 6403 6c06 5a07 6400 6403 6c08 5a09 6400  d.l.Z.d.d.l.Z.d.
-00000060: 6404 6c0a 6d0a 5a0a 0100 6400 6405 6c0b  d.l.m.Z...d.d.l.
-00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
-00000080: 0100 6400 6407 6c0f 6d10 5a10 0100 6400  ..d.d.l.m.Z...d.
-00000090: 6408 6c11 6d12 5a12 0100 4700 6409 640a  d.l.m.Z...G.d.d.
-000000a0: 8400 640a 8302 5a13 6403 5300 290b e900  ..d...Z.d.S.)...
-000000b0: 0000 0029 01da 0149 2903 da04 4c69 7374  ...)...I)...List
-000000c0: da05 5475 706c 65da 0444 6963 744e 2901  ..Tuple..DictN).
-000000d0: da04 7471 646d a901 da0b 6772 6170 685f  ..tqdm....graph_
-000000e0: 746f 5f70 6e29 01da 0653 616d 706c 6529  to_pn)...Sample)
-000000f0: 01da 0e47 7261 7068 4578 7472 6163 746f  ...GraphExtracto
-00000100: 72a9 01da 0b50 6f74 6174 6f47 7261 7068  r....PotatoGraph
-00000110: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000120: 0007 0000 0040 0000 0073 1e01 0000 6500  .....@...s....e.
-00000130: 5a01 6400 5a02 6401 6900 6402 6401 6403  Z.d.Z.d.i.d.d.d.
-00000140: 6401 6401 6607 6503 6504 6505 6505 6602  d.d.f.e.e.e.e.f.
-00000150: 1900 1900 6506 6505 6507 6602 1900 6401  ....e.e.e.f...d.
-00000160: 6404 9c03 6405 6406 8405 5a08 6509 650a  d...d.d...Z.e.e.
-00000170: 6a0b 6505 6401 6407 9c03 6408 6409 8404  j.e.d.d...d.d...
-00000180: 8301 5a0c 6424 6503 650d 6a0e 1900 6401  ..Z.d$e.e.j...d.
-00000190: 640a 9c02 640b 640c 8405 5a0f 6425 6503  d...d.d...Z.d%e.
-000001a0: 6504 6505 6505 6602 1900 1900 6505 6510  e.e.e.f.....e.e.
-000001b0: 6503 6511 1900 640d 9c04 640e 640f 8405  e.e...d...d.d...
-000001c0: 5a12 650d 6a0e 650d 6a0e 6410 9c02 6411  Z.e.j.e.j.d...d.
-000001d0: 6412 8404 5a13 6426 6510 650a 6a0b 6413  d...Z.d&e.e.j.d.
-000001e0: 9c02 6414 6415 8405 5a14 6427 6505 6503  ..d.d...Z.d'e.e.
-000001f0: 6515 1900 6417 9c02 6418 6419 8405 5a16  e...d...d.d...Z.
-00000200: 6503 6515 1900 6401 640a 9c02 641a 641b  e.e...d.d...d.d.
-00000210: 8404 5a17 6428 6505 6510 6401 641c 9c03  ..Z.d(e.e.d.d...
-00000220: 641d 641e 8405 5a18 6505 6401 641f 9c02  d.d...Z.e.d.d...
-00000230: 6420 6421 8404 5a19 6505 6401 641f 9c02  d d!..Z.e.d.d...
-00000240: 6422 6423 8404 5a1a 6401 5300 2929 da07  d"d#..Z.d.S.))..
-00000250: 4461 7461 7365 744e da02 656e 4629 03da  DatasetN..enF)..
-00000260: 0865 7861 6d70 6c65 73da 0b6c 6162 656c  .examples..label
-00000270: 5f76 6f63 6162 da06 7265 7475 726e 6308  _vocab..returnc.
-00000280: 0000 0000 0000 0000 0000 0008 0000 0005  ................
-00000290: 0000 0043 0000 0073 4400 0000 7c02 7c00  ...C...sD...|.|.
-000002a0: 5f00 7c04 721c 7c00 6a01 7c04 7c05 6401  _.|.r.|.j.|.|.d.
-000002b0: 8d02 7c00 5f02 6e0e 7c00 6a01 7c01 6402  ..|._.n.|.j.|.d.
-000002c0: 8d01 7c00 5f02 7403 7c03 7c06 7c07 6403  ..|._.t.|.|.|.d.
-000002d0: 8d03 7c00 5f04 6400 7c00 5f05 6400 5300  ..|._.d.|._.d.S.
-000002e0: 2904 4e29 02da 0470 6174 68da 0662 696e  ).N)...path..bin
-000002f0: 6172 7929 0172 0f00 0000 2903 da04 6c61  ary).r....)...la
-00000300: 6e67 da09 6361 6368 655f 6469 72da 0863  ng..cache_dir..c
-00000310: 6163 6865 5f66 6e29 0672 1000 0000 da0c  ache_fn).r......
-00000320: 7265 6164 5f64 6174 6173 6574 da08 5f64  read_dataset.._d
-00000330: 6174 6173 6574 720a 0000 00da 0965 7874  atasetr......ext
-00000340: 7261 6374 6f72 da06 6772 6170 6873 2908  ractor..graphs).
-00000350: da04 7365 6c66 720f 0000 0072 1000 0000  ..selfr....r....
-00000360: 7214 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00000370: 1500 0000 7216 0000 00a9 0072 1c00 0000  ....r......r....
-00000380: fa38 2f68 6f6d 652f 6164 6161 6d6b 6f2f  .8/home/adaamko/
-00000390: 7072 6f6a 6563 7473 2f50 4f54 4154 4f2f  projects/POTATO/
-000003a0: 7870 6f74 6174 6f2f 6461 7461 7365 742f  xpotato/dataset/
-000003b0: 6461 7461 7365 742e 7079 da08 5f5f 696e  dataset.py..__in
-000003c0: 6974 5f5f 0f00 0000 7310 0000 0000 0a06  it__....s.......
-000003d0: 0104 0112 020e 0202 0106 ff08 037a 1044  .............z.D
-000003e0: 6174 6173 6574 2e5f 5f69 6e69 745f 5f29  ataset.__init__)
-000003f0: 03da 0264 6672 1200 0000 7211 0000 0063  ...dfr....r....c
-00000400: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00000410: 0500 0000 4300 0000 7332 0000 0064 0164  ....C...s2...d.d
-00000420: 0284 007c 0064 0319 00a0 00a1 0044 0083  ...|.d.......D..
-00000430: 017d 027c 027c 0064 033c 007c 006a 017c  .}.|.|.d.<.|.j.|
-00000440: 0164 0464 0564 068d 0301 0064 0053 0029  .d.d.d.....d.S.)
-00000450: 074e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
-00000460: 0000 0004 0000 0053 0000 0073 1400 0000  .......S...s....
-00000470: 6700 7c00 5d0c 7d01 7400 7c01 8301 9102  g.|.].}.t.|.....
-00000480: 7104 5300 721c 0000 0072 0700 0000 a902  q.S.r....r......
-00000490: da02 2e30 da05 6772 6170 6872 1c00 0000  ...0..graphr....
-000004a0: 721c 0000 0072 1d00 0000 da0a 3c6c 6973  r....r......<lis
-000004b0: 7463 6f6d 703e 2600 0000 f300 0000 007a  tcomp>&........z
-000004c0: 2a44 6174 6173 6574 2e73 6176 655f 6461  *Dataset.save_da
-000004d0: 7461 6672 616d 652e 3c6c 6f63 616c 733e  taframe.<locals>
-000004e0: 2e3c 6c69 7374 636f 6d70 3e72 2200 0000  .<listcomp>r"...
-000004f0: 46fa 0109 a902 da05 696e 6465 78da 0373  F.......index..s
-00000500: 6570 2902 da06 746f 6c69 7374 da06 746f  ep)...tolist..to
-00000510: 5f63 7376 2903 721f 0000 0072 1200 0000  _csv).r....r....
-00000520: 721a 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
-00000530: 1d00 0000 da0e 7361 7665 5f64 6174 6166  ......save_dataf
-00000540: 7261 6d65 2400 0000 7306 0000 0000 0216  rame$...s.......
-00000550: 0108 017a 1644 6174 6173 6574 2e73 6176  ...z.Dataset.sav
-00000560: 655f 6461 7461 6672 616d 6529 0272 1a00  e_dataframe).r..
-00000570: 0000 7211 0000 0063 0200 0000 0000 0000  ..r....c........
-00000580: 0000 0000 0700 0000 0700 0000 4300 0000  ............C...
-00000590: 7394 0000 0067 007d 0274 007c 0183 0144  s....g.}.t.|...D
-000005a0: 005d 825c 027d 037d 047c 04a0 0174 0274  .].\.}.}.|...t.t
-000005b0: 03a0 047c 04a1 0183 01a1 0101 007c 00a0  ...|.........|..
-000005c0: 057c 04a1 017d 0464 0164 0284 0074 0674  .|...}.d.d...t.t
-000005d0: 03a0 077c 04a1 0174 0864 0364 048d 0344  ...|...t.d.d...D
-000005e0: 0083 017d 0574 087c 0583 0164 056b 0472  ...}.t.|...d.k.r
-000005f0: 7c74 0964 0683 0101 0074 0a7c 04a0 0b7c  |t.d.....t.|...|
-00000600: 0564 0719 00a0 0ca1 00a1 0183 017d 066e  .d...........}.n
-00000610: 0874 0a7c 0483 017d 067c 02a0 0d7c 06a1  .t.|...}.|...|..
-00000620: 0101 0071 0c7c 0253 0029 084e 6301 0000  ...q.|.S.).Nc...
-00000630: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00000640: 0053 0000 0073 1000 0000 6700 7c00 5d08  .S...s....g.|.].
-00000650: 7d01 7c01 9102 7104 5300 721c 0000 0072  }.|...q.S.r....r
-00000660: 1c00 0000 2902 7221 0000 00da 0163 721c  ....).r!.....cr.
-00000670: 0000 0072 1c00 0000 721d 0000 0072 2300  ...r....r....r#.
-00000680: 0000 3100 0000 7304 0000 0006 0202 ff7a  ..1...s........z
-00000690: 2844 6174 6173 6574 2e70 7275 6e65 5f67  (Dataset.prune_g
-000006a0: 7261 7068 732e 3c6c 6f63 616c 733e 2e3c  raphs.<locals>.<
-000006b0: 6c69 7374 636f 6d70 3e54 2902 da03 6b65  listcomp>T)...ke
-000006c0: 79da 0772 6576 6572 7365 e901 0000 007a  y..reverse.....z
-000006d0: 4457 4152 4e49 4e47 3a20 6772 6170 6820  DWARNING: graph 
-000006e0: 6861 7320 6d75 6c74 6970 6c65 2063 6f6e  has multiple con
-000006f0: 6e65 6374 6564 2063 6f6d 706f 6e65 6e74  nected component
-00000700: 732c 2074 616b 696e 6720 7468 6520 6c61  s, taking the la
-00000710: 7267 6573 7472 0100 0000 290e da09 656e  rgestr....)...en
-00000720: 756d 6572 6174 655a 1172 656d 6f76 655f  umerateZ.remove_
-00000730: 6e6f 6465 735f 6672 6f6d da04 6c69 7374  nodes_from..list
-00000740: da02 6e78 5a08 6973 6f6c 6174 6573 da13  ..nxZ.isolates..
-00000750: 5f72 616e 646f 6d5f 706f 7374 7072 6f63  _random_postproc
-00000760: 6573 73da 0673 6f72 7465 645a 1b77 6561  ess..sortedZ.wea
-00000770: 6b6c 795f 636f 6e6e 6563 7465 645f 636f  kly_connected_co
-00000780: 6d70 6f6e 656e 7473 da03 6c65 6eda 0570  mponents..len..p
-00000790: 7269 6e74 7208 0000 005a 0873 7562 6772  rintr....Z.subgr
-000007a0: 6170 68da 0463 6f70 79da 0661 7070 656e  aph..copy..appen
-000007b0: 6429 0772 1b00 0000 721a 0000 00da 0a67  d).r....r......g
-000007c0: 7261 7068 735f 7374 72da 0169 7222 0000  raphs_str..ir"..
-000007d0: 00da 0167 5a04 675f 706e 721c 0000 0072  ...gZ.g_pnr....r
-000007e0: 1c00 0000 721d 0000 00da 0c70 7275 6e65  ....r......prune
-000007f0: 5f67 7261 7068 732a 0000 0073 2200 0000  _graphs*...s"...
-00000800: 0001 0401 1001 1402 0a02 0602 0201 0cff  ................
-00000810: 04fe 0606 0c01 0201 02ff 0403 1802 0802  ................
-00000820: 0c02 7a14 4461 7461 7365 742e 7072 756e  ..z.Dataset.prun
-00000830: 655f 6772 6170 6873 2904 720f 0000 0072  e_graphs).r....r
-00000840: 1200 0000 7213 0000 0072 1100 0000 6304  ....r....r....c.
-00000850: 0000 0000 0000 0000 0000 0006 0000 0004  ................
-00000860: 0000 0043 0000 0073 8600 0000 7400 7c01  ...C...s....t.|.
-00000870: 8301 7d01 7c01 721a 6401 6402 8400 7c01  ..}.|.r.d.d...|.
-00000880: 4400 8301 5300 7c02 727a 7c03 7256 7401  D...S.|.rz|.rVt.
-00000890: a002 7c02 a101 7d04 7c00 a003 7c04 6a04  ..|...}.|...|.j.
-000008a0: a005 a100 a101 7d05 7c04 6a06 6403 6701  ......}.|.j.d.g.
-000008b0: 6404 6405 8d02 0100 7c05 7c04 6403 3c00  d.d.....|.|.d.<.
-000008c0: 6e0e 7401 6a07 7c02 6406 6407 8d02 7d04  n.t.j.|.d.d...}.
-000008d0: 6408 6402 8400 7408 7c04 a009 a100 8301  d.d...t.|.......
-000008e0: 4400 8301 5300 740a 6409 8301 8201 6400  D...S.t.d.....d.
-000008f0: 5300 290a 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-00000900: 0000 0200 0000 0500 0000 5300 0000 7318  ..........S...s.
-00000910: 0000 0067 007c 005d 107d 0174 007c 0174  ...g.|.].}.t.|.t
-00000920: 0183 0083 0291 0271 0453 0072 1c00 0000  .......q.S.r....
-00000930: a902 7209 0000 0072 0c00 0000 2902 7221  ..r....r....).r!
-00000940: 0000 00da 0765 7861 6d70 6c65 721c 0000  .....exampler...
-00000950: 0072 1c00 0000 721d 0000 0072 2300 0000  .r....r....r#...
-00000960: 4b00 0000 7224 0000 007a 2844 6174 6173  K...r$...z(Datas
-00000970: 6574 2e72 6561 645f 6461 7461 7365 742e  et.read_dataset.
-00000980: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00000990: 6d70 3e72 2200 0000 5429 02da 0763 6f6c  mp>r"...T)...col
-000009a0: 756d 6e73 5a07 696e 706c 6163 6572 2500  umnsZ.inplacer%.
-000009b0: 0000 2901 7228 0000 0063 0100 0000 0000  ..).r(...c......
-000009c0: 0000 0000 0000 0300 0000 0700 0000 5300  ..............S.
-000009d0: 0000 7338 0000 0067 007c 005d 305c 027d  ..s8...g.|.]0\.}
-000009e0: 017d 0274 007c 0264 0019 007c 0264 0119  .}.t.|.d...|.d..
-000009f0: 0066 0274 017c 0264 0219 0064 038d 017c  .f.t.|.d...d...|
-00000a00: 0264 0419 0064 058d 0391 0271 0453 0029  .d...d.....q.S.)
-00000a10: 06da 0474 6578 74da 056c 6162 656c 7222  ...text..labelr"
-00000a20: 0000 00a9 01da 0967 7261 7068 5f73 7472  .......graph_str
-00000a30: da08 6c61 6265 6c5f 6964 2902 da0c 706f  ..label_id)...po
-00000a40: 7461 746f 5f67 7261 7068 7244 0000 0072  tato_graphrD...r
-00000a50: 3d00 0000 2903 7221 0000 00da 015f 723e  =...).r!....._r>
-00000a60: 0000 0072 1c00 0000 721c 0000 0072 1d00  ...r....r....r..
-00000a70: 0000 7223 0000 0055 0000 0073 0c00 0000  ..r#...U...s....
-00000a80: 0606 06fb 0201 0e01 0c01 06fd 7a1c 4e6f  ............z.No
-00000a90: 2065 7861 6d70 6c65 7320 6f72 2070 6174   examples or pat
-00000aa0: 6820 7072 6f76 6964 6564 290b 7231 0000  h provided).r1..
-00000ab0: 00da 0270 64da 0b72 6561 645f 7069 636b  ...pd..read_pick
-00000ac0: 6c65 723c 0000 0072 2200 0000 7229 0000  ler<...r"...r)..
-00000ad0: 00da 0464 726f 705a 0872 6561 645f 6373  ...dropZ.read_cs
-00000ae0: 7672 0600 0000 5a08 6974 6572 726f 7773  vr....Z.iterrows
-00000af0: da0a 5661 6c75 6545 7272 6f72 2906 721b  ..ValueError).r.
-00000b00: 0000 0072 0f00 0000 7212 0000 0072 1300  ...r....r....r..
-00000b10: 0000 721f 0000 0072 3900 0000 721c 0000  ..r....r9...r...
-00000b20: 0072 1c00 0000 721d 0000 0072 1700 0000  .r....r....r....
-00000b30: 4300 0000 731c 0000 0000 0608 0104 010e  C...s...........
-00000b40: 0104 0104 010a 0110 0110 010a 020e 0206  ................
-00000b50: 060a fa06 097a 1444 6174 6173 6574 2e72  .....z.Dataset.r
-00000b60: 6561 645f 6461 7461 7365 7429 0272 2200  ead_dataset).r".
-00000b70: 0000 7211 0000 0063 0200 0000 0000 0000  ..r....c........
-00000b80: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
-00000b90: 7342 0000 007c 016a 0064 0164 028d 0144  sB...|.j.d.d...D
-00000ba0: 005d 305c 027d 027d 0374 017c 0364 0319  .]0\.}.}.t.|.d..
-00000bb0: 00a0 02a1 0083 0164 046b 0472 0c7c 0364  .......d.k.r.|.d
-00000bc0: 0319 00a0 02a1 0064 0519 007c 0364 033c  .......d...|.d.<
-00000bd0: 0071 0c7c 0153 0029 064e 5429 01da 0464  .q.|.S.).NT)...d
-00000be0: 6174 61da 046e 616d 6572 2f00 0000 7201  ata..namer/...r.
-00000bf0: 0000 0029 03da 056e 6f64 6573 7235 0000  ...)...nodesr5..
-00000c00: 00da 0573 706c 6974 2904 721b 0000 0072  ...split).r....r
-00000c10: 2200 0000 da04 6e6f 6465 da04 6174 7472  ".....node..attr
-00000c20: 721c 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
-00000c30: 3300 0000 6100 0000 7308 0000 0000 0114  3...a...s.......
-00000c40: 0114 0116 027a 1b44 6174 6173 6574 2e5f  .....z.Dataset._
-00000c50: 7261 6e64 6f6d 5f70 6f73 7470 726f 6365  random_postproce
-00000c60: 7373 2902 da09 6173 5f70 656e 6d61 6e72  ss)...as_penmanr
-00000c70: 1100 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00000c80: 0003 0000 0008 0000 0003 0000 0073 5000  .............sP.
-00000c90: 0000 7400 a001 6401 6402 8400 8801 6a02  ..t...d.d.....j.
-00000ca0: 4400 8301 6403 6402 8400 8801 6a02 4400  D...d.d.....j.D.
-00000cb0: 8301 8701 6601 6404 6402 8408 8801 6a02  ....f.d.d.....j.
-00000cc0: 4400 8301 8700 6601 6405 6402 8408 8801  D.....f.d.d.....
-00000cd0: 6a02 4400 8301 6406 9c04 a101 7d02 7c02  j.D...d.....}.|.
-00000ce0: 5300 2907 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-00000cf0: 0000 0200 0000 0300 0000 5300 0000 7312  ..........S...s.
-00000d00: 0000 0067 007c 005d 0a7d 017c 016a 0091  ...g.|.].}.|.j..
-00000d10: 0271 0453 0072 1c00 0000 a901 7240 0000  .q.S.r......r@..
-00000d20: 00a9 0272 2100 0000 da06 7361 6d70 6c65  ...r!.....sample
+00000000: 420d 0d0a 0000 0000 b76f 9763 4a17 0000  B........o.cJ...
+00000010: e300 0000 0000 0000 0000 0000 0003 0000  ................
+00000020: 0040 0000 0073 9600 0000 6400 6401 6c00  .@...s....d.d.l.
+00000030: 5a00 6400 6402 6c01 6d02 5a02 0100 6400  Z.d.d.l.m.Z...d.
+00000040: 6403 6c03 6d04 5a04 6d05 5a05 6d06 5a06  d.l.m.Z.m.Z.m.Z.
+00000050: 0100 6400 6401 6c07 5a08 6400 6401 6c09  ..d.d.l.Z.d.d.l.
+00000060: 5a0a 6400 6404 6c0b 6d0c 5a0c 0100 6400  Z.d.d.l.m.Z...d.
+00000070: 6405 6c0d 6d0d 5a0d 0100 6400 6406 6c0e  d.l.m.Z...d.d.l.
+00000080: 6d0f 5a0f 6d10 5a10 0100 6400 6407 6c11  m.Z.m.Z...d.d.l.
+00000090: 6d12 5a12 0100 6400 6408 6c13 6d14 5a14  m.Z...d.d.l.m.Z.
+000000a0: 0100 6400 6409 6c15 6d16 5a16 0100 4700  ..d.d.l.m.Z...G.
+000000b0: 640a 640b 8400 640b 8302 5a17 6401 5300  d.d...d...Z.d.S.
+000000c0: 290c e900 0000 004e 2901 da01 4929 03da  )......N)...I)..
+000000d0: 0444 6963 74da 044c 6973 74da 0554 7570  .Dict..List..Tup
+000000e0: 6c65 2901 da0a 6a73 6f6e 5f67 7261 7068  le)...json_graph
+000000f0: 2901 da04 7471 646d 2902 da16 6368 6563  )...tqdm)...chec
+00000100: 6b5f 6966 5f73 7472 5f69 735f 7065 6e6d  k_if_str_is_penm
+00000110: 616e da0b 6772 6170 685f 746f 5f70 6e29  an..graph_to_pn)
+00000120: 01da 0653 616d 706c 6529 01da 0e47 7261  ...Sample)...Gra
+00000130: 7068 4578 7472 6163 746f 7229 01da 0b50  phExtractor)...P
+00000140: 6f74 6174 6f47 7261 7068 6300 0000 0000  otatoGraphc.....
+00000150: 0000 0000 0000 0007 0000 0040 0000 0073  ...........@...s
+00000160: 2201 0000 6500 5a01 6400 5a02 6401 6900  "...e.Z.d.Z.d.i.
+00000170: 6402 6401 6403 6401 6401 6607 6503 6504  d.d.d.d.d.f.e.e.
+00000180: 6505 6505 6602 1900 1900 6506 6505 6507  e.e.f.....e.e.e.
+00000190: 6602 1900 6401 6404 9c03 6405 6406 8405  f...d.d...d.d...
+000001a0: 5a08 6509 650a 6a0b 6505 6401 6407 9c03  Z.e.e.j.e.d.d...
+000001b0: 6408 6409 8404 8301 5a0c 6425 6503 650d  d.d.....Z.d%e.e.
+000001c0: 6a0e 1900 6401 640a 9c02 640b 640c 8405  j...d.d...d.d...
+000001d0: 5a0f 6426 6503 6504 6505 6505 6602 1900  Z.d&e.e.e.e.f...
+000001e0: 1900 6505 6510 6503 6511 1900 640d 9c04  ..e.e.e.e...d...
+000001f0: 640e 640f 8405 5a12 650d 6a0e 650d 6a0e  d.d...Z.e.j.e.j.
+00000200: 6410 9c02 6411 6412 8404 5a13 6427 6510  d...d.d...Z.d'e.
+00000210: 6510 650a 6a0b 6413 9c03 6414 6415 8405  e.e.j.d...d.d...
+00000220: 5a14 6428 6505 6503 6515 1900 6417 9c02  Z.d(e.e.e...d...
+00000230: 6418 6419 8405 5a16 6503 6515 1900 6401  d.d...Z.e.e...d.
+00000240: 640a 9c02 641a 641b 8404 5a17 6429 6505  d...d.d...Z.d)e.
+00000250: 6510 6401 641c 9c03 641d 641e 8405 5a18  e.d.d...d.d...Z.
+00000260: 6505 6401 641f 9c02 6420 6421 8404 5a19  e.d.d...d d!..Z.
+00000270: 642a 6505 6401 641f 9c02 6423 6424 8405  d*e.d.d...d#d$..
+00000280: 5a1a 6401 5300 292b da07 4461 7461 7365  Z.d.S.)+..Datase
+00000290: 744e da02 656e 4629 03da 0865 7861 6d70  tN..enF)...examp
+000002a0: 6c65 73da 0b6c 6162 656c 5f76 6f63 6162  les..label_vocab
+000002b0: da06 7265 7475 726e 6308 0000 0000 0000  ..returnc.......
+000002c0: 0008 0000 0005 0000 0043 0000 0073 4400  .........C...sD.
+000002d0: 0000 7c02 7c00 5f00 7c04 721c 7c00 6a01  ..|.|._.|.r.|.j.
+000002e0: 7c04 7c05 6401 8d02 7c00 5f02 6e0e 7c00  |.|.d...|._.n.|.
+000002f0: 6a01 7c01 6402 8d01 7c00 5f02 7403 7c03  j.|.d...|._.t.|.
+00000300: 7c06 7c07 6403 8d03 7c00 5f04 6400 7c00  |.|.d...|._.d.|.
+00000310: 5f05 6400 5300 2904 4e29 02da 0470 6174  _.d.S.).N)...pat
+00000320: 68da 0662 696e 6172 7929 0172 0f00 0000  h..binary).r....
+00000330: 2903 da04 6c61 6e67 da09 6361 6368 655f  )...lang..cache_
+00000340: 6469 72da 0863 6163 6865 5f66 6e29 0672  dir..cache_fn).r
+00000350: 1000 0000 da0c 7265 6164 5f64 6174 6173  ......read_datas
+00000360: 6574 da08 5f64 6174 6173 6574 720b 0000  et.._datasetr...
+00000370: 00da 0965 7874 7261 6374 6f72 da06 6772  ...extractor..gr
+00000380: 6170 6873 2908 da04 7365 6c66 720f 0000  aphs)...selfr...
+00000390: 0072 1000 0000 7214 0000 0072 1200 0000  .r....r....r....
+000003a0: 7213 0000 0072 1500 0000 7216 0000 00a9  r....r....r.....
+000003b0: 0072 1c00 0000 fa4d 2f55 7365 7273 2f61  .r.....M/Users/a
+000003c0: 6461 6d6b 6f76 6163 732f 7072 6f6a 6563  damkovacs/projec
+000003d0: 7473 2f65 7870 2d72 656c 6174 696f 6e2d  ts/exp-relation-
+000003e0: 6578 7472 6163 7469 6f6e 2f78 706f 7461  extraction/xpota
+000003f0: 746f 2f64 6174 6173 6574 2f64 6174 6173  to/dataset/datas
+00000400: 6574 2e70 79da 085f 5f69 6e69 745f 5f11  et.py..__init__.
+00000410: 0000 0073 0e00 0000 000a 0601 0401 1202  ...s............
+00000420: 0e02 0201 0e02 7a10 4461 7461 7365 742e  ......z.Dataset.
+00000430: 5f5f 696e 6974 5f5f 2903 da02 6466 7212  __init__)...dfr.
+00000440: 0000 0072 1100 0000 6302 0000 0000 0000  ...r....c.......
+00000450: 0003 0000 0005 0000 0043 0000 0073 3200  .........C...s2.
+00000460: 0000 6401 6402 8400 7c00 6403 1900 a000  ..d.d...|.d.....
+00000470: a100 4400 8301 7d02 7c02 7c00 6403 3c00  ..D...}.|.|.d.<.
+00000480: 7c00 6a01 7c01 6404 6405 6406 8d03 0100  |.j.|.d.d.d.....
+00000490: 6400 5300 2907 4e63 0100 0000 0000 0000  d.S.).Nc........
+000004a0: 0200 0000 0700 0000 5300 0000 732e 0000  ........S...s...
+000004b0: 0067 007c 005d 267d 0174 007c 0183 0174  .g.|.]&}.t.|...t
+000004c0: 016a 026b 0272 2674 03a0 0474 05a0 067c  .j.k.r&t...t...|
+000004d0: 01a1 01a1 016e 027c 0191 0271 0453 0072  .....n.|...q.S.r
+000004e0: 1c00 0000 2907 da04 7479 7065 da02 6e78  ....)...type..nx
+000004f0: da07 4469 4772 6170 68da 046a 736f 6eda  ..DiGraph..json.
+00000500: 0564 756d 7073 7206 0000 00da 0e61 646a  .dumpsr......adj
+00000510: 6163 656e 6379 5f64 6174 6129 02da 022e  acency_data)....
+00000520: 30da 0167 721c 0000 0072 1c00 0000 721d  0..gr....r....r.
+00000530: 0000 00fa 0a3c 6c69 7374 636f 6d70 3e29  .....<listcomp>)
+00000540: 0000 0073 0200 0000 0601 7a2a 4461 7461  ...s......z*Data
+00000550: 7365 742e 7361 7665 5f64 6174 6166 7261  set.save_datafra
+00000560: 6d65 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  me.<locals>.<lis
+00000570: 7463 6f6d 703e da05 6772 6170 6846 fa01  tcomp>..graphF..
+00000580: 0929 02da 0569 6e64 6578 da03 7365 7029  .)...index..sep)
+00000590: 02da 0674 6f6c 6973 74da 0674 6f5f 6373  ...tolist..to_cs
+000005a0: 7629 0372 1f00 0000 7212 0000 0072 1a00  v).r....r....r..
+000005b0: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+000005c0: 00da 0e73 6176 655f 6461 7461 6672 616d  ...save_datafram
+000005d0: 6526 0000 0073 0800 0000 0003 0601 1002  e&...s..........
+000005e0: 0801 7a16 4461 7461 7365 742e 7361 7665  ..z.Dataset.save
+000005f0: 5f64 6174 6166 7261 6d65 2902 721a 0000  _dataframe).r...
+00000600: 0072 1100 0000 6302 0000 0000 0000 0007  .r....c.........
+00000610: 0000 0007 0000 0043 0000 0073 9800 0000  .......C...s....
+00000620: 6700 7d02 788e 7400 7c01 8301 4400 5d82  g.}.x.t.|...D.].
+00000630: 5c02 7d03 7d04 7c04 a001 7402 7403 a004  \.}.}.|...t.t...
+00000640: 7c04 a101 8301 a101 0100 7c00 a005 7c04  |.........|...|.
+00000650: a101 7d04 6401 6402 8400 7406 7403 a007  ..}.d.d...t.t...
+00000660: 7c04 a101 7408 6403 6404 8d03 4400 8301  |...t.d.d...D...
+00000670: 7d05 7408 7c05 8301 6405 6b04 727e 7409  }.t.|...d.k.r~t.
+00000680: 6406 8301 0100 740a 7c04 a00b 7c05 6407  d.....t.|...|.d.
+00000690: 1900 a00c a100 a101 8301 7d06 6e08 740a  ..........}.n.t.
+000006a0: 7c04 8301 7d06 7c02 a00d 7c06 a101 0100  |...}.|...|.....
+000006b0: 710e 5700 7c02 5300 2908 4e63 0100 0000  q.W.|.S.).Nc....
+000006c0: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
+000006d0: 7310 0000 0067 007c 005d 087d 017c 0191  s....g.|.].}.|..
+000006e0: 0271 0453 0072 1c00 0000 721c 0000 0029  .q.S.r....r....)
+000006f0: 0272 2600 0000 da01 6372 1c00 0000 721c  .r&.....cr....r.
+00000700: 0000 0072 1d00 0000 7228 0000 0037 0000  ...r....r(...7..
+00000710: 0073 0200 0000 0601 7a28 4461 7461 7365  .s......z(Datase
+00000720: 742e 7072 756e 655f 6772 6170 6873 2e3c  t.prune_graphs.<
+00000730: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00000740: 703e 5429 02da 036b 6579 da07 7265 7665  p>T)...key..reve
+00000750: 7273 65e9 0100 0000 7a44 5741 524e 494e  rse.....zDWARNIN
+00000760: 473a 2067 7261 7068 2068 6173 206d 756c  G: graph has mul
+00000770: 7469 706c 6520 636f 6e6e 6563 7465 6420  tiple connected 
+00000780: 636f 6d70 6f6e 656e 7473 2c20 7461 6b69  components, taki
+00000790: 6e67 2074 6865 206c 6172 6765 7374 7201  ng the largestr.
+000007a0: 0000 0029 0eda 0965 6e75 6d65 7261 7465  ...)...enumerate
+000007b0: da11 7265 6d6f 7665 5f6e 6f64 6573 5f66  ..remove_nodes_f
+000007c0: 726f 6dda 046c 6973 7472 2100 0000 da08  rom..listr!.....
+000007d0: 6973 6f6c 6174 6573 da13 5f72 616e 646f  isolates.._rando
+000007e0: 6d5f 706f 7374 7072 6f63 6573 73da 0673  m_postprocess..s
+000007f0: 6f72 7465 64da 1b77 6561 6b6c 795f 636f  orted..weakly_co
+00000800: 6e6e 6563 7465 645f 636f 6d70 6f6e 656e  nnected_componen
+00000810: 7473 da03 6c65 6eda 0570 7269 6e74 7209  ts..len..printr.
+00000820: 0000 00da 0873 7562 6772 6170 68da 0463  .....subgraph..c
+00000830: 6f70 79da 0661 7070 656e 6429 0772 1b00  opy..append).r..
+00000840: 0000 721a 0000 00da 0a67 7261 7068 735f  ..r......graphs_
+00000850: 7374 72da 0169 7229 0000 0072 2700 0000  str..ir)...r'...
+00000860: 5a04 675f 706e 721c 0000 0072 1c00 0000  Z.g_pnr....r....
+00000870: 721d 0000 00da 0c70 7275 6e65 5f67 7261  r......prune_gra
+00000880: 7068 732f 0000 0073 1c00 0000 0001 0401  phs/...s........
+00000890: 1201 1402 0a03 0601 0201 1603 0c01 0201  ................
+000008a0: 0602 1802 0802 0e02 7a14 4461 7461 7365  ........z.Datase
+000008b0: 742e 7072 756e 655f 6772 6170 6873 2904  t.prune_graphs).
+000008c0: 720f 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+000008d0: 1100 0000 6304 0000 0000 0000 0007 0000  ....c...........
+000008e0: 0004 0000 0043 0000 0073 b000 0000 7c01  .....C...s....|.
+000008f0: 7212 6401 6402 8400 7c01 4400 8301 5300  r.d.d...|.D...S.
+00000900: 7c02 72a4 7c03 7280 7400 a001 7c02 a101  |.r.|.r.t...|...
+00000910: 7d04 6403 6402 8400 7c04 6404 1900 a002  }.d.d...|.d.....
+00000920: a100 4400 8301 7d05 7403 7c05 6405 1900  ..D...}.t.|.d...
+00000930: 8301 7404 6b02 728e 7405 7c05 6405 1900  ..t.k.r.t.|.d...
+00000940: 8301 728e 7c00 a006 7c04 6a07 a002 a100  ..r.|...|.j.....
+00000950: a101 7d06 7c04 6a08 6404 6701 6406 6407  ..}.|.j.d.g.d.d.
+00000960: 8d02 0100 7c06 7c04 6404 3c00 6e0e 7400  ....|.|.d.<.n.t.
+00000970: 6a09 7c02 6408 6409 8d02 7d04 640a 6402  j.|.d.d...}.d.d.
+00000980: 8400 740a 7c04 a00b a100 8301 4400 8301  ..t.|.......D...
+00000990: 5300 740c 640b 8301 8201 6400 5300 290c  S.t.d.....d.S.).
+000009a0: 4e63 0100 0000 0000 0000 0200 0000 0500  Nc..............
+000009b0: 0000 5300 0000 7318 0000 0067 007c 005d  ..S...s....g.|.]
+000009c0: 107d 0174 007c 0174 0183 0083 0291 0271  .}.t.|.t.......q
+000009d0: 0453 0072 1c00 0000 2902 720a 0000 0072  .S.r....).r....r
+000009e0: 0c00 0000 2902 7226 0000 00da 0765 7861  ....).r&.....exa
+000009f0: 6d70 6c65 721c 0000 0072 1c00 0000 721d  mpler....r....r.
+00000a00: 0000 0072 2800 0000 4f00 0000 7302 0000  ...r(...O...s...
+00000a10: 0006 007a 2844 6174 6173 6574 2e72 6561  ...z(Dataset.rea
+00000a20: 645f 6461 7461 7365 742e 3c6c 6f63 616c  d_dataset.<local
+00000a30: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
+00000a40: 0000 0000 0000 0200 0000 0300 0000 5300  ..............S.
+00000a50: 0000 7310 0000 0067 007c 005d 087d 017c  ..s....g.|.].}.|
+00000a60: 0191 0271 0453 0072 1c00 0000 721c 0000  ...q.S.r....r...
+00000a70: 0029 0272 2600 0000 7229 0000 0072 1c00  .).r&...r)...r..
+00000a80: 0000 721c 0000 0072 1d00 0000 7228 0000  ..r....r....r(..
+00000a90: 0053 0000 0073 0200 0000 0600 7229 0000  .S...s......r)..
+00000aa0: 0072 0100 0000 5429 02da 0763 6f6c 756d  .r....T)...colum
+00000ab0: 6e73 da07 696e 706c 6163 6572 2a00 0000  ns..inplacer*...
+00000ac0: 2901 722c 0000 0063 0100 0000 0000 0000  ).r,...c........
+00000ad0: 0300 0000 0700 0000 5300 0000 7338 0000  ........S...s8..
+00000ae0: 0067 007c 005d 305c 027d 017d 0274 007c  .g.|.]0\.}.}.t.|
+00000af0: 0264 0019 007c 0264 0119 0066 0274 017c  .d...|.d...f.t.|
+00000b00: 0264 0219 0064 038d 017c 0264 0419 0064  .d...d...|.d...d
+00000b10: 058d 0391 0271 0453 0029 06da 0474 6578  .....q.S.)...tex
+00000b20: 74da 056c 6162 656c 7229 0000 0029 0172  t..labelr)...).r
+00000b30: 2900 0000 da08 6c61 6265 6c5f 6964 2902  ).....label_id).
+00000b40: da0c 706f 7461 746f 5f67 7261 7068 7248  ..potato_graphrH
+00000b50: 0000 0029 0272 0a00 0000 720c 0000 0029  ...).r....r....)
+00000b60: 0372 2600 0000 da01 5f72 4300 0000 721c  .r&....._rC...r.
+00000b70: 0000 0072 1c00 0000 721d 0000 0072 2800  ...r....r....r(.
+00000b80: 0000 5c00 0000 7302 0000 0006 057a 1c4e  ..\...s......z.N
+00000b90: 6f20 6578 616d 706c 6573 206f 7220 7061  o examples or pa
+00000ba0: 7468 2070 726f 7669 6465 6429 0dda 0270  th provided)...p
+00000bb0: 64da 0b72 6561 645f 7069 636b 6c65 722d  d..read_pickler-
+00000bc0: 0000 0072 2000 0000 da03 7374 7272 0800  ...r .....strr..
+00000bd0: 0000 7242 0000 0072 2900 0000 da04 6472  ..rB...r).....dr
+00000be0: 6f70 da08 7265 6164 5f63 7376 7207 0000  op..read_csvr...
+00000bf0: 00da 0869 7465 7272 6f77 73da 0a56 616c  ...iterrows..Val
+00000c00: 7565 4572 726f 7229 0772 1b00 0000 720f  ueError).r....r.
+00000c10: 0000 0072 1200 0000 7213 0000 0072 1f00  ...r....r....r..
+00000c20: 0000 721a 0000 0072 4000 0000 721c 0000  ..r....r@...r...
+00000c30: 0072 1c00 0000 721d 0000 0072 1700 0000  .r....r....r....
+00000c40: 4800 0000 731c 0000 0000 0604 010e 0104  H...s...........
+00000c50: 0104 010a 0116 011c 0110 0110 010a 020e  ................
+00000c60: 0306 0510 037a 1444 6174 6173 6574 2e72  .....z.Dataset.r
+00000c70: 6561 645f 6461 7461 7365 7429 0272 2900  ead_dataset).r).
+00000c80: 0000 7211 0000 0063 0200 0000 0000 0000  ..r....c........
+00000c90: 0400 0000 0400 0000 4300 0000 7346 0000  ........C...sF..
+00000ca0: 0078 407c 016a 0064 0164 028d 0144 005d  .x@|.j.d.d...D.]
+00000cb0: 305c 027d 027d 0374 017c 0364 0319 00a0  0\.}.}.t.|.d....
+00000cc0: 02a1 0083 0164 046b 0472 0e7c 0364 0319  .....d.k.r.|.d..
+00000cd0: 00a0 02a1 0064 0519 007c 0364 033c 0071  .....d...|.d.<.q
+00000ce0: 0e57 007c 0153 0029 064e 5429 01da 0464  .W.|.S.).NT)...d
+00000cf0: 6174 61da 046e 616d 6572 3300 0000 7201  ata..namer3...r.
+00000d00: 0000 0029 03da 056e 6f64 6573 723b 0000  ...)...nodesr;..
+00000d10: 00da 0573 706c 6974 2904 721b 0000 0072  ...split).r....r
+00000d20: 2900 0000 da04 6e6f 6465 da04 6174 7472  ).....node..attr
 00000d30: 721c 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
-00000d40: 2300 0000 6b00 0000 7224 0000 007a 2844  #...k...r$...z(D
-00000d50: 6174 6173 6574 2e74 6f5f 6461 7461 6672  ataset.to_datafr
-00000d60: 616d 652e 3c6c 6f63 616c 733e 2e3c 6c69  ame.<locals>.<li
-00000d70: 7374 636f 6d70 3e63 0100 0000 0000 0000  stcomp>c........
-00000d80: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
-00000d90: 7312 0000 0067 007c 005d 0a7d 017c 016a  s....g.|.].}.|.j
-00000da0: 0091 0271 0453 0072 1c00 0000 2901 7241  ...q.S.r....).rA
-00000db0: 0000 0072 5300 0000 721c 0000 0072 1c00  ...rS...r....r..
-00000dc0: 0000 721d 0000 0072 2300 0000 6c00 0000  ..r....r#...l...
-00000dd0: 7224 0000 0063 0100 0000 0000 0000 0000  r$...c..........
-00000de0: 0000 0200 0000 0500 0000 1300 0000 7318  ..............s.
-00000df0: 0000 0067 007c 005d 107d 017c 01a0 0088  ...g.|.].}.|....
-00000e00: 006a 01a1 0191 0271 0453 0072 1c00 0000  .j.....q.S.r....
-00000e10: 2902 5a0c 6765 745f 6c61 6265 6c5f 6964  ).Z.get_label_id
-00000e20: 7210 0000 0072 5300 0000 2901 721b 0000  r....rS...).r...
-00000e30: 0072 1c00 0000 721d 0000 0072 2300 0000  .r....r....r#...
-00000e40: 6d00 0000 7302 0000 0006 0163 0100 0000  m...s......c....
-00000e50: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00000e60: 1300 0000 7322 0000 0067 007c 005d 1a7d  ....s"...g.|.].}
-00000e70: 0188 0072 1674 007c 016a 0183 016e 067c  ...r.t.|.j...n.|
-00000e80: 016a 016a 0291 0271 0453 0072 1c00 0000  .j.j...q.S.r....
-00000e90: 2903 da03 7374 7272 4500 0000 7222 0000  )...strrE...r"..
-00000ea0: 0072 5300 0000 a901 7251 0000 0072 1c00  .rS.....rQ...r..
-00000eb0: 0000 721d 0000 0072 2300 0000 7000 0000  ..r....r#...p...
-00000ec0: 7304 0000 0006 0202 ff29 0472 4000 0000  s........).r@...
-00000ed0: 7241 0000 0072 4400 0000 7222 0000 0029  rA...rD...r"...)
-00000ee0: 0372 4700 0000 da09 4461 7461 4672 616d  .rG.....DataFram
-00000ef0: 6572 1800 0000 2903 721b 0000 0072 5100  er....).r....rQ.
-00000f00: 0000 721f 0000 0072 1c00 0000 2902 7251  ..r....r....).rQ
-00000f10: 0000 0072 1b00 0000 721d 0000 00da 0c74  ...r....r......t
-00000f20: 6f5f 6461 7461 6672 616d 6568 0000 0073  o_dataframeh...s
-00000f30: 1800 0000 0001 0402 0e01 0e01 0a01 04ff  ................
-00000f40: 0403 0a02 04fe 04fa 04ff 040d 7a14 4461  ............z.Da
-00000f50: 7461 7365 742e 746f 5f64 6174 6166 7261  taset.to_datafra
-00000f60: 6d65 da08 666f 7572 6c61 6e67 2902 da0c  me..fourlang)...
-00000f70: 6772 6170 685f 666f 726d 6174 7211 0000  graph_formatr...
-00000f80: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
-00000f90: 0000 0500 0000 4300 0000 7334 0000 0074  ......C...s4...t
-00000fa0: 007c 006a 01a0 0264 0164 0284 007c 006a  .|.j...d.d...|.j
-00000fb0: 0344 0083 017c 01a1 0283 017d 0264 0364  .D...|.....}.d.d
-00000fc0: 0284 007c 0244 0083 017c 005f 047c 006a  ...|.D...|._.|.j
-00000fd0: 0453 0029 044e 6301 0000 0000 0000 0000  .S.).Nc.........
-00000fe0: 0000 0002 0000 0003 0000 0053 0000 0073  ...........S...s
-00000ff0: 1200 0000 6700 7c00 5d0a 7d01 7c01 6a00  ....g.|.].}.|.j.
-00001000: 9102 7104 5300 721c 0000 0072 5200 0000  ..q.S.r....rR...
-00001010: 7253 0000 0072 1c00 0000 721c 0000 0072  rS...r....r....r
-00001020: 1d00 0000 7223 0000 007b 0000 0072 2400  ....r#...{...r$.
-00001030: 0000 7a28 4461 7461 7365 742e 7061 7273  ..z(Dataset.pars
-00001040: 655f 6772 6170 6873 2e3c 6c6f 6361 6c73  e_graphs.<locals
-00001050: 3e2e 3c6c 6973 7463 6f6d 703e 6301 0000  >.<listcomp>c...
-00001060: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00001070: 0053 0000 0073 1400 0000 6700 7c00 5d0c  .S...s....g.|.].
-00001080: 7d01 7400 7c01 8301 9102 7104 5300 721c  }.t.|.....q.S.r.
-00001090: 0000 0072 0b00 0000 7220 0000 0072 1c00  ...r....r ...r..
-000010a0: 0000 721c 0000 0072 1d00 0000 7223 0000  ..r....r....r#..
-000010b0: 007f 0000 0072 2400 0000 2905 7231 0000  .....r$...).r1..
-000010c0: 0072 1900 0000 5a0e 7061 7273 655f 6974  .r....Z.parse_it
-000010d0: 6572 6162 6c65 7218 0000 0072 1a00 0000  erabler....r....
-000010e0: 2903 721b 0000 0072 5a00 0000 721a 0000  ).r....rZ...r...
-000010f0: 0072 1c00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00001100: da0c 7061 7273 655f 6772 6170 6873 7800  ..parse_graphsx.
-00001110: 0000 730e 0000 0000 0102 0106 0110 ff02  ..s.............
-00001120: ff04 0610 017a 1444 6174 6173 6574 2e70  .....z.Dataset.p
-00001130: 6172 7365 5f67 7261 7068 7363 0200 0000  arse_graphsc....
-00001140: 0000 0000 0000 0000 0400 0000 0600 0000  ................
-00001150: 4300 0000 7338 0000 0074 007c 006a 017c  C...s8...t.|.j.|
-00001160: 0183 0244 005d 265c 027d 027d 037c 036a  ...D.]&\.}.}.|.j
-00001170: 02a0 0374 04a0 057c 036a 02a1 01a1 0101  ...t...|.j......
-00001180: 007c 02a0 067c 03a1 0101 0071 0c64 0053  .|...|.....q.d.S
-00001190: 0029 014e 2907 da03 7a69 7072 1800 0000  .).N)...zipr....
-000011a0: 7222 0000 005a 1172 656d 6f76 655f 6564  r"...Z.remove_ed
-000011b0: 6765 735f 6672 6f6d 7232 0000 005a 0e73  ges_fromr2...Z.s
-000011c0: 656c 666c 6f6f 705f 6564 6765 735a 0973  elfloop_edgesZ.s
-000011d0: 6574 5f67 7261 7068 2904 721b 0000 0072  et_graph).r....r
-000011e0: 1a00 0000 7254 0000 0072 4500 0000 721c  ....rT...rE...r.
-000011f0: 0000 0072 1c00 0000 721d 0000 00da 0a73  ...r....r......s
-00001200: 6574 5f67 7261 7068 7382 0000 0073 0600  et_graphs....s..
-00001210: 0000 0001 1401 1401 7a12 4461 7461 7365  ........z.Datase
-00001220: 742e 7365 745f 6772 6170 6873 2903 7212  t.set_graphs).r.
-00001230: 0000 0072 1300 0000 7211 0000 0063 0300  ...r....r....c..
-00001240: 0000 0000 0000 0000 0000 0800 0000 0800  ................
-00001250: 0000 4300 0000 7396 0000 007c 0272 3864  ..C...s....|.r8d
-00001260: 0164 0284 0074 00a0 017c 01a1 0144 0083  .d...t...|...D..
-00001270: 017d 037c 00a0 027c 03a1 017d 0464 0364  .}.|...|...}.d.d
-00001280: 0284 007c 0444 0083 017d 037c 037c 005f  ...|.D...}.|.|._
-00001290: 036e 4e74 047c 0164 0483 028f 347d 057c  .nNt.|.d....4}.|
-000012a0: 0544 005d 1e7d 0674 057c 06a0 06a1 0064  .D.].}.t.|.....d
-000012b0: 058d 017d 077c 006a 03a0 077c 07a1 0101  ...}.|.j...|....
-000012c0: 0071 4857 0064 0004 0004 0083 0301 006e  .qHW.d.........n
-000012d0: 1031 0073 7c30 0001 0001 0001 0059 0001  .1.s|0.......Y..
-000012e0: 007c 00a0 087c 006a 03a1 0101 0064 0053  .|...|.j.....d.S
-000012f0: 0029 064e 6301 0000 0000 0000 0000 0000  .).Nc...........
-00001300: 0002 0000 0003 0000 0053 0000 0073 1000  .........S...s..
-00001310: 0000 6700 7c00 5d08 7d01 7c01 9102 7104  ..g.|.].}.|...q.
-00001320: 5300 721c 0000 0072 1c00 0000 7220 0000  S.r....r....r ..
-00001330: 0072 1c00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00001340: 7223 0000 0089 0000 0072 2400 0000 7a27  r#.......r$...z'
-00001350: 4461 7461 7365 742e 6c6f 6164 5f67 7261  Dataset.load_gra
-00001360: 7068 732e 3c6c 6f63 616c 733e 2e3c 6c69  phs.<locals>.<li
-00001370: 7374 636f 6d70 3e63 0100 0000 0000 0000  stcomp>c........
-00001380: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
-00001390: 7316 0000 0067 007c 005d 0e7d 0174 007c  s....g.|.].}.t.|
-000013a0: 0164 008d 0191 0271 0453 0029 0172 4200  .d.....q.S.).rB.
-000013b0: 0000 720b 0000 0072 2000 0000 721c 0000  ..r....r ...r...
-000013c0: 0072 1c00 0000 721d 0000 0072 2300 0000  .r....r....r#...
-000013d0: 8c00 0000 7224 0000 00da 0272 6272 4200  ....r$.....rbrB.
-000013e0: 0000 2909 7247 0000 0072 4800 0000 723c  ..).rG...rH...r<
-000013f0: 0000 0072 1a00 0000 da04 6f70 656e 720c  ...r......openr.
-00001400: 0000 00da 0573 7472 6970 7238 0000 0072  .....stripr8...r
-00001410: 5d00 0000 2908 721b 0000 0072 1200 0000  ]...).r....r....
-00001420: 7213 0000 0072 1a00 0000 7243 0000 00da  r....r....rC....
-00001430: 0166 da04 6c69 6e65 7222 0000 0072 1c00  .f..liner"...r..
-00001440: 0000 721c 0000 0072 1d00 0000 da0b 6c6f  ..r....r......lo
-00001450: 6164 5f67 7261 7068 7387 0000 0073 1400  ad_graphs....s..
-00001460: 0000 0001 0401 1401 0a02 0e01 0802 0c01  ................
-00001470: 0801 0e01 2c02 7a13 4461 7461 7365 742e  ....,.z.Dataset.
-00001480: 6c6f 6164 5f67 7261 7068 7329 0272 1200  load_graphs).r..
-00001490: 0000 7211 0000 0063 0200 0000 0000 0000  ..r....c........
-000014a0: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
-000014b0: 7320 0000 007c 006a 0064 0164 028d 017d  s ...|.j.d.d...}
-000014c0: 027c 026a 017c 0164 0364 0464 058d 0301  .|.j.|.d.d.d....
-000014d0: 0064 0053 0029 064e 5472 5600 0000 4672  .d.S.).NTrV...Fr
-000014e0: 2500 0000 7226 0000 0029 0272 5800 0000  %...r&...).rX...
-000014f0: 722a 0000 0029 0372 1b00 0000 7212 0000  r*...).r....r...
-00001500: 0072 1f00 0000 721c 0000 0072 1c00 0000  .r....r....r....
-00001510: 721d 0000 00da 0c73 6176 655f 6461 7461  r......save_data
-00001520: 7365 7496 0000 0073 0400 0000 0001 0c01  set....s........
-00001530: 7a14 4461 7461 7365 742e 7361 7665 5f64  z.Dataset.save_d
-00001540: 6174 6173 6574 6302 0000 0000 0000 0000  atasetc.........
-00001550: 0000 0004 0000 0008 0000 0043 0000 0073  ...........C...s
-00001560: 4c00 0000 7400 7c01 6401 8302 8f2e 7d02  L...t.|.d.....}.
-00001570: 7c00 6a01 4400 5d16 7d03 7c02 a002 7403  |.j.D.].}.|...t.
-00001580: 7c03 8301 6402 1700 a101 0100 7112 5700  |...d.......q.W.
-00001590: 6400 0400 0400 8303 0100 6e10 3100 733e  d.........n.1.s>
-000015a0: 3000 0100 0100 0100 5900 0100 6400 5300  0.......Y...d.S.
-000015b0: 2903 4eda 0277 62da 010a 2904 725f 0000  ).N..wb...).r_..
-000015c0: 0072 1a00 0000 da05 7772 6974 6572 5500  .r......writerU.
-000015d0: 0000 2904 721b 0000 0072 1200 0000 7261  ..).r....r....ra
-000015e0: 0000 0072 2200 0000 721c 0000 0072 1c00  ...r"...r....r..
-000015f0: 0000 721d 0000 00da 0b73 6176 655f 6772  ..r......save_gr
-00001600: 6170 6873 9a00 0000 7306 0000 0000 010c  aphs....s.......
-00001610: 010a 017a 1344 6174 6173 6574 2e73 6176  ...z.Dataset.sav
-00001620: 655f 6772 6170 6873 2901 4e29 034e 4e46  e_graphs).N).NNF
-00001630: 2901 4629 0172 5900 0000 2901 4629 1bda  ).F).rY...).F)..
-00001640: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00001650: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00001660: 655f 5f72 0300 0000 7204 0000 0072 5500  e__r....r....rU.
-00001670: 0000 7205 0000 00da 0369 6e74 721e 0000  ..r......intr...
-00001680: 00da 0c73 7461 7469 636d 6574 686f 6472  ...staticmethodr
-00001690: 4700 0000 7257 0000 0072 2b00 0000 7232  G...rW...r+...r2
-000016a0: 0000 005a 0744 6947 7261 7068 723c 0000  ...Z.DiGraphr<..
-000016b0: 00da 0462 6f6f 6c72 0900 0000 7217 0000  ...boolr....r...
-000016c0: 0072 3300 0000 7258 0000 0072 0c00 0000  .r3...rX...r....
-000016d0: 725b 0000 0072 5d00 0000 7263 0000 0072  r[...r]...rc...r
-000016e0: 6400 0000 7268 0000 0072 1c00 0000 721c  d...rh...r....r.
-000016f0: 0000 0072 1c00 0000 721d 0000 0072 0d00  ...r....r....r..
-00001700: 0000 0e00 0000 733e 0000 0008 0302 0102  ......s>........
-00001710: 0102 0102 0102 0102 0102 f802 020e 010a  ................
-00001720: 0602 f70c 1502 0116 0518 1b00 0100 0100  ................
-00001730: fc02 020e 0102 0102 0106 fb0c 1e14 0714  ................
-00001740: 1016 0a14 0514 0f10 0472 0d00 0000 2914  .........r....).
-00001750: da02 7265 7202 0000 00da 0674 7970 696e  ..rer......typin
-00001760: 6772 0300 0000 7204 0000 0072 0500 0000  gr....r....r....
-00001770: 5a08 6e65 7477 6f72 6b78 7232 0000 00da  Z.networkxr2....
-00001780: 0670 616e 6461 7372 4700 0000 7206 0000  .pandasrG...r...
-00001790: 005a 1374 7577 5f6e 6c70 2e67 7261 7068  .Z.tuw_nlp.graph
-000017a0: 2e75 7469 6c73 7208 0000 005a 1678 706f  .utilsr....Z.xpo
-000017b0: 7461 746f 2e64 6174 6173 6574 2e73 616d  tato.dataset.sam
-000017c0: 706c 6572 0900 0000 5a1f 7870 6f74 6174  pler....Z.xpotat
-000017d0: 6f2e 6772 6170 685f 6578 7472 6163 746f  o.graph_extracto
-000017e0: 722e 6578 7472 6163 7472 0a00 0000 5a1d  r.extractr....Z.
-000017f0: 7870 6f74 6174 6f2e 6772 6170 685f 6578  xpotato.graph_ex
-00001800: 7472 6163 746f 722e 6772 6170 6872 0c00  tractor.graphr..
-00001810: 0000 720d 0000 0072 1c00 0000 721c 0000  ..r....r....r...
-00001820: 0072 1c00 0000 721d 0000 00da 083c 6d6f  .r....r......<mo
-00001830: 6475 6c65 3e01 0000 0073 1200 0000 0c01  dule>....s......
-00001840: 1402 0801 0802 0c01 0c01 0c01 0c01 0c03  ................
+00000d40: 3800 0000 6700 0000 7308 0000 0000 0116  8...g...s.......
+00000d50: 0114 0118 027a 1b44 6174 6173 6574 2e5f  .....z.Dataset._
+00000d60: 7261 6e64 6f6d 5f70 6f73 7470 726f 6365  random_postproce
+00000d70: 7373 2903 da09 6173 5f70 656e 6d61 6eda  ss)...as_penman.
+00000d80: 0761 735f 6a73 6f6e 7211 0000 0063 0300  .as_jsonr....c..
+00000d90: 0000 0000 0000 0400 0000 0800 0000 0300  ................
+00000da0: 0000 7352 0000 0074 00a0 0164 0164 0284  ..sR...t...d.d..
+00000db0: 0088 026a 0244 0083 0164 0364 0284 0088  ...j.D...d.d....
+00000dc0: 026a 0244 0083 0187 0266 0164 0464 0284  .j.D.....f.d.d..
+00000dd0: 0888 026a 0244 0083 0187 0087 0166 0264  ...j.D.......f.d
+00000de0: 0564 0284 0888 026a 0244 0083 0164 069c  .d.....j.D...d..
+00000df0: 04a1 017d 037c 0353 0029 074e 6301 0000  ...}.|.S.).Nc...
+00000e00: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
+00000e10: 0073 1200 0000 6700 7c00 5d0a 7d01 7c01  .s....g.|.].}.|.
+00000e20: 6a00 9102 7104 5300 721c 0000 0029 0172  j...q.S.r....).r
+00000e30: 4600 0000 2902 7226 0000 00da 0673 616d  F...).r&.....sam
+00000e40: 706c 6572 1c00 0000 721c 0000 0072 1d00  pler....r....r..
+00000e50: 0000 7228 0000 0073 0000 0073 0200 0000  ..r(...s...s....
+00000e60: 0600 7a28 4461 7461 7365 742e 746f 5f64  ..z(Dataset.to_d
+00000e70: 6174 6166 7261 6d65 2e3c 6c6f 6361 6c73  ataframe.<locals
+00000e80: 3e2e 3c6c 6973 7463 6f6d 703e 6301 0000  >.<listcomp>c...
+00000e90: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
+00000ea0: 0073 1200 0000 6700 7c00 5d0a 7d01 7c01  .s....g.|.].}.|.
+00000eb0: 6a00 9102 7104 5300 721c 0000 0029 0172  j...q.S.r....).r
+00000ec0: 4700 0000 2902 7226 0000 0072 5a00 0000  G...).r&...rZ...
+00000ed0: 721c 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
+00000ee0: 2800 0000 7400 0000 7302 0000 0006 0063  (...t...s......c
+00000ef0: 0100 0000 0000 0000 0200 0000 0500 0000  ................
+00000f00: 1300 0000 7318 0000 0067 007c 005d 107d  ....s....g.|.].}
+00000f10: 017c 01a0 0088 006a 01a1 0191 0271 0453  .|.....j.....q.S
+00000f20: 0072 1c00 0000 2902 5a0c 6765 745f 6c61  .r....).Z.get_la
+00000f30: 6265 6c5f 6964 7210 0000 0029 0272 2600  bel_idr....).r&.
+00000f40: 0000 725a 0000 0029 0172 1b00 0000 721c  ..rZ...).r....r.
+00000f50: 0000 0072 1d00 0000 7228 0000 0076 0000  ...r....r(...v..
+00000f60: 0073 0200 0000 0600 6301 0000 0000 0000  .s......c.......
+00000f70: 0002 0000 0004 0000 0013 0000 0073 3200  .............s2.
+00000f80: 0000 6700 7c00 5d2a 7d01 8801 7216 7400  ..g.|.]*}...r.t.
+00000f90: 7c01 6a01 8301 6e16 8800 7224 7c01 6a01  |.j...n...r$|.j.
+00000fa0: a002 a100 6e08 7c01 6a01 6a03 6a04 9102  ....n.|.j.j.j...
+00000fb0: 7104 5300 721c 0000 0029 0572 4d00 0000  q.S.r....).rM...
+00000fc0: 7249 0000 00da 0774 6f5f 6469 6374 7229  rI.....to_dictr)
+00000fd0: 0000 00da 0147 2902 7226 0000 0072 5a00  .....G).r&...rZ.
+00000fe0: 0000 2902 7259 0000 0072 5800 0000 721c  ..).rY...rX...r.
+00000ff0: 0000 0072 1d00 0000 7228 0000 0079 0000  ...r....r(...y..
+00001000: 0073 0200 0000 0605 2904 7246 0000 0072  .s......).rF...r
+00001010: 4700 0000 7248 0000 0072 2900 0000 2903  G...rH...r)...).
+00001020: 724b 0000 00da 0944 6174 6146 7261 6d65  rK.....DataFrame
+00001030: 7218 0000 0029 0472 1b00 0000 7258 0000  r....).r....rX..
+00001040: 0072 5900 0000 721f 0000 0072 1c00 0000  .rY...r....r....
+00001050: 2903 7259 0000 0072 5800 0000 721b 0000  ).rY...rX...r...
+00001060: 0072 1d00 0000 da0c 746f 5f64 6174 6166  .r......to_dataf
+00001070: 7261 6d65 6e00 0000 730e 0000 0000 0304  ramen...s.......
+00001080: 020e 010e 0212 030c 0510 047a 1444 6174  ...........z.Dat
+00001090: 6173 6574 2e74 6f5f 6461 7461 6672 616d  aset.to_datafram
+000010a0: 65da 0866 6f75 726c 616e 6729 02da 0c67  e..fourlang)...g
+000010b0: 7261 7068 5f66 6f72 6d61 7472 1100 0000  raph_formatr....
+000010c0: 6302 0000 0000 0000 0003 0000 0005 0000  c...............
+000010d0: 0043 0000 0073 3400 0000 7400 7c00 6a01  .C...s4...t.|.j.
+000010e0: a002 6401 6402 8400 7c00 6a03 4400 8301  ..d.d...|.j.D...
+000010f0: 7c01 a102 8301 7d02 6403 6402 8400 7c02  |.....}.d.d...|.
+00001100: 4400 8301 7c00 5f04 7c00 6a04 5300 2904  D...|._.|.j.S.).
+00001110: 4e63 0100 0000 0000 0000 0200 0000 0300  Nc..............
+00001120: 0000 5300 0000 7312 0000 0067 007c 005d  ..S...s....g.|.]
+00001130: 0a7d 017c 016a 0091 0271 0453 0072 1c00  .}.|.j...q.S.r..
+00001140: 0000 2901 7246 0000 0029 0272 2600 0000  ..).rF...).r&...
+00001150: 725a 0000 0072 1c00 0000 721c 0000 0072  rZ...r....r....r
+00001160: 1d00 0000 7228 0000 0087 0000 0073 0200  ....r(.......s..
+00001170: 0000 0600 7a28 4461 7461 7365 742e 7061  ....z(Dataset.pa
+00001180: 7273 655f 6772 6170 6873 2e3c 6c6f 6361  rse_graphs.<loca
+00001190: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 6301  ls>.<listcomp>c.
+000011a0: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
+000011b0: 0000 0073 1600 0000 6700 7c00 5d0e 7d01  ...s....g.|.].}.
+000011c0: 7400 7c01 6400 8d01 9102 7104 5300 2901  t.|.d.....q.S.).
+000011d0: 2901 7229 0000 0029 0172 0c00 0000 2902  ).r)...).r....).
+000011e0: 7226 0000 0072 2900 0000 721c 0000 0072  r&...r)...r....r
+000011f0: 1c00 0000 721d 0000 0072 2800 0000 8b00  ....r....r(.....
+00001200: 0000 7302 0000 0006 0029 0572 3600 0000  ..s......).r6...
+00001210: 7219 0000 00da 0e70 6172 7365 5f69 7465  r......parse_ite
+00001220: 7261 626c 6572 1800 0000 721a 0000 0029  rabler....r....)
+00001230: 0372 1b00 0000 7260 0000 0072 1a00 0000  .r....r`...r....
+00001240: 721c 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
+00001250: 0c70 6172 7365 5f67 7261 7068 7384 0000  .parse_graphs...
+00001260: 0073 0a00 0000 0001 0201 0601 1604 1001  .s..............
+00001270: 7a14 4461 7461 7365 742e 7061 7273 655f  z.Dataset.parse_
+00001280: 6772 6170 6873 6302 0000 0000 0000 0004  graphsc.........
+00001290: 0000 0006 0000 0043 0000 0073 4000 0000  .......C...s@...
+000012a0: 783a 7400 7c00 6a01 7c01 8302 4400 5d2a  x:t.|.j.|...D.]*
+000012b0: 5c02 7d02 7d03 7c03 6a02 6a03 a004 7405  \.}.}.|.j.j...t.
+000012c0: a006 7c03 6a02 6a03 a101 a101 0100 7c02  ..|.j.j.......|.
+000012d0: a007 7c03 a101 0100 710e 5700 6400 5300  ..|.....q.W.d.S.
+000012e0: 2901 4e29 08da 037a 6970 7218 0000 0072  ).N)...zipr....r
+000012f0: 2900 0000 725c 0000 00da 1172 656d 6f76  )...r\.....remov
+00001300: 655f 6564 6765 735f 6672 6f6d 7221 0000  e_edges_fromr!..
+00001310: 00da 0e73 656c 666c 6f6f 705f 6564 6765  ...selfloop_edge
+00001320: 73da 0973 6574 5f67 7261 7068 2904 721b  s..set_graph).r.
+00001330: 0000 0072 1a00 0000 725a 0000 0072 4900  ...r....rZ...rI.
+00001340: 0000 721c 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+00001350: 00da 0a73 6574 5f67 7261 7068 738e 0000  ...set_graphs...
+00001360: 0073 0800 0000 0001 1601 0801 1002 7a12  .s............z.
+00001370: 4461 7461 7365 742e 7365 745f 6772 6170  Dataset.set_grap
+00001380: 6873 2903 7212 0000 0072 1300 0000 7211  hs).r....r....r.
+00001390: 0000 0063 0300 0000 0000 0000 0800 0000  ...c............
+000013a0: 0900 0000 4300 0000 7386 0000 007c 0272  ....C...s....|.r
+000013b0: 3864 0164 0284 0074 00a0 017c 01a1 0144  8d.d...t...|...D
+000013c0: 0083 017d 037c 00a0 027c 03a1 017d 0464  ...}.|...|...}.d
+000013d0: 0364 0284 007c 0444 0083 017d 037c 037c  .d...|.D...}.|.|
+000013e0: 005f 036e 3e74 047c 0164 0483 028f 2e7d  ._.n>t.|.d.....}
+000013f0: 0578 267c 0544 005d 1e7d 0674 057c 06a0  .x&|.D.].}.t.|..
+00001400: 06a1 0064 058d 017d 077c 006a 03a0 077c  ...d...}.|.j...|
+00001410: 07a1 0101 0071 4a57 0057 0064 0051 0052  .....qJW.W.d.Q.R
+00001420: 0058 007c 00a0 087c 006a 03a1 0101 0064  .X.|...|.j.....d
+00001430: 0053 0029 064e 6301 0000 0000 0000 0002  .S.).Nc.........
+00001440: 0000 0003 0000 0053 0000 0073 1000 0000  .......S...s....
+00001450: 6700 7c00 5d08 7d01 7c01 9102 7104 5300  g.|.].}.|...q.S.
+00001460: 721c 0000 0072 1c00 0000 2902 7226 0000  r....r....).r&..
+00001470: 0072 2900 0000 721c 0000 0072 1c00 0000  .r)...r....r....
+00001480: 721d 0000 0072 2800 0000 9700 0000 7302  r....r(.......s.
+00001490: 0000 0006 007a 2744 6174 6173 6574 2e6c  .....z'Dataset.l
+000014a0: 6f61 645f 6772 6170 6873 2e3c 6c6f 6361  oad_graphs.<loca
+000014b0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 6301  ls>.<listcomp>c.
+000014c0: 0000 0000 0000 0002 0000 0005 0000 0053  ...............S
+000014d0: 0000 0073 1600 0000 6700 7c00 5d0e 7d01  ...s....g.|.].}.
+000014e0: 7400 7c01 6400 8d01 9102 7104 5300 2901  t.|.d.....q.S.).
+000014f0: 2901 7229 0000 0029 0172 0c00 0000 2902  ).r)...).r....).
+00001500: 7226 0000 0072 2900 0000 721c 0000 0072  r&...r)...r....r
+00001510: 1c00 0000 721d 0000 0072 2800 0000 9a00  ....r....r(.....
+00001520: 0000 7302 0000 0006 00da 0272 6229 0172  ..s........rb).r
+00001530: 2900 0000 2909 724b 0000 0072 4c00 0000  )...).rK...rL...
+00001540: 7242 0000 0072 1a00 0000 da04 6f70 656e  rB...r......open
+00001550: 720c 0000 00da 0573 7472 6970 723f 0000  r......stripr?..
+00001560: 0072 6700 0000 2908 721b 0000 0072 1200  .rg...).r....r..
+00001570: 0000 7213 0000 0072 1a00 0000 5a09 6772  ..r....r....Z.gr
+00001580: 6170 685f 7374 72da 0166 da04 6c69 6e65  aph_str..f..line
+00001590: 7229 0000 0072 1c00 0000 721c 0000 0072  r)...r....r....r
+000015a0: 1d00 0000 da0b 6c6f 6164 5f67 7261 7068  ......load_graph
+000015b0: 7395 0000 0073 1400 0000 0001 0401 1401  s....s..........
+000015c0: 0a02 0e01 0802 0c01 0a01 0e01 1a02 7a13  ..............z.
+000015d0: 4461 7461 7365 742e 6c6f 6164 5f67 7261  Dataset.load_gra
+000015e0: 7068 7329 0272 1200 0000 7211 0000 0063  phs).r....r....c
+000015f0: 0200 0000 0000 0000 0300 0000 0400 0000  ................
+00001600: 4300 0000 7318 0000 007c 00a0 00a1 007d  C...s....|.....}
+00001610: 027c 00a0 017c 027c 01a1 0201 0064 0053  .|...|.|.....d.S
+00001620: 0029 014e 2902 725e 0000 0072 2f00 0000  .).N).r^...r/...
+00001630: 2903 721b 0000 0072 1200 0000 721f 0000  ).r....r....r...
+00001640: 0072 1c00 0000 721c 0000 0072 1d00 0000  .r....r....r....
+00001650: da0c 7361 7665 5f64 6174 6173 6574 a400  ..save_dataset..
+00001660: 0000 7304 0000 0000 0108 017a 1444 6174  ..s........z.Dat
+00001670: 6173 6574 2e73 6176 655f 6461 7461 7365  aset.save_datase
+00001680: 74da 0464 6963 7463 0300 0000 0000 0000  t..dictc........
+00001690: 0500 0000 0900 0000 4300 0000 7368 0000  ........C...sh..
+000016a0: 0074 007c 0164 0183 028f 547d 0378 4c7c  .t.|.d....T}.xL|
+000016b0: 006a 0144 005d 427d 047c 0264 026b 0272  .j.D.]B}.|.d.k.r
+000016c0: 3a74 02a0 037c 046a 047c 03a1 0201 007c  :t...|.j.|.....|
+000016d0: 03a0 0564 03a1 0101 0071 147c 0264 046b  ...d.....q.|.d.k
+000016e0: 0272 147c 03a0 0574 067c 0483 019b 0064  .r.|...t.|.....d
+000016f0: 039d 02a1 0101 0071 1457 0057 0064 0051  .......q.W.W.d.Q
+00001700: 0052 0058 0064 0053 0029 054e da02 7762  .R.X.d.S.).N..wb
+00001710: 726f 0000 00da 010a da06 7065 6e6d 616e  ro........penman
+00001720: 2907 7269 0000 0072 1a00 0000 7223 0000  ).ri...r....r#..
+00001730: 00da 0464 756d 7072 2900 0000 da05 7772  ...dumpr).....wr
+00001740: 6974 6572 4d00 0000 2905 721b 0000 0072  iterM...).r....r
+00001750: 1200 0000 7220 0000 0072 6b00 0000 7229  ....r ...rk...r)
+00001760: 0000 0072 1c00 0000 721c 0000 0072 1d00  ...r....r....r..
+00001770: 0000 da0b 7361 7665 5f67 7261 7068 73a8  ....save_graphs.
+00001780: 0000 0073 0e00 0000 0001 0c01 0c01 0801  ...s............
+00001790: 0e01 0c01 0801 7a13 4461 7461 7365 742e  ......z.Dataset.
+000017a0: 7361 7665 5f67 7261 7068 7329 014e 2903  save_graphs).N).
+000017b0: 4e4e 4629 0246 4629 0172 5f00 0000 2901  NNF).FF).r_...).
+000017c0: 4629 0172 6f00 0000 291b da08 5f5f 6e61  F).ro...)...__na
+000017d0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+000017e0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7204  ..__qualname__r.
+000017f0: 0000 0072 0500 0000 724d 0000 0072 0300  ...r....rM...r..
+00001800: 0000 da03 696e 7472 1e00 0000 da0c 7374  ....intr......st
+00001810: 6174 6963 6d65 7468 6f64 724b 0000 0072  aticmethodrK...r
+00001820: 5d00 0000 722f 0000 0072 2100 0000 7222  ]...r/...r!...r"
+00001830: 0000 0072 4200 0000 da04 626f 6f6c 720a  ...rB.....boolr.
+00001840: 0000 0072 1700 0000 7238 0000 0072 5e00  ...r....r8...r^.
+00001850: 0000 720c 0000 0072 6200 0000 7267 0000  ..r....rb...rg..
+00001860: 0072 6d00 0000 726e 0000 0072 7500 0000  .rm...rn...ru...
+00001870: 721c 0000 0072 1c00 0000 721c 0000 0072  r....r....r....r
+00001880: 1d00 0000 720d 0000 0010 0000 0073 2e00  ....r........s..
+00001890: 0000 0803 0201 0201 0201 0201 0201 0201  ................
+000018a0: 1c01 0e0c 0201 1608 181b 0001 0001 1401  ................
+000018b0: 121a 1408 0601 1014 160a 1407 140f 1004  ................
+000018c0: 720d 0000 0029 1872 2300 0000 da02 7265  r....).r#.....re
+000018d0: 7202 0000 00da 0674 7970 696e 6772 0300  r......typingr..
+000018e0: 0000 7204 0000 0072 0500 0000 da08 6e65  ..r....r......ne
+000018f0: 7477 6f72 6b78 7221 0000 00da 0670 616e  tworkxr!.....pan
+00001900: 6461 7372 4b00 0000 5a12 6e65 7477 6f72  dasrK...Z.networ
+00001910: 6b78 2e72 6561 6477 7269 7465 7206 0000  kx.readwriter...
+00001920: 0072 0700 0000 da13 7475 775f 6e6c 702e  .r......tuw_nlp.
+00001930: 6772 6170 682e 7574 696c 7372 0800 0000  graph.utilsr....
+00001940: 7209 0000 005a 1678 706f 7461 746f 2e64  r....Z.xpotato.d
+00001950: 6174 6173 6574 2e73 616d 706c 6572 0a00  ataset.sampler..
+00001960: 0000 da1f 7870 6f74 6174 6f2e 6772 6170  ....xpotato.grap
+00001970: 685f 6578 7472 6163 746f 722e 6578 7472  h_extractor.extr
+00001980: 6163 7472 0b00 0000 da1d 7870 6f74 6174  actr......xpotat
+00001990: 6f2e 6772 6170 685f 6578 7472 6163 746f  o.graph_extracto
+000019a0: 722e 6772 6170 6872 0c00 0000 720d 0000  r.graphr....r...
+000019b0: 0072 1c00 0000 721c 0000 0072 1c00 0000  .r....r....r....
+000019c0: 721d 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+000019d0: 0000 0073 1600 0000 0801 0c01 1402 0801  ...s............
+000019e0: 0801 0c01 0c01 1002 0c01 0c01 0c03       ..............
```

### Comparing `xpotato-0.1.4/xpotato/dataset/__pycache__/sample.cpython-39.pyc` & `xpotato-0.1.5/xpotato/dataset/__pycache__/sample.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Mar  9 10:46:32 2022 UTC, .py size: 745 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8885 2862 e902 0000  a.........(b....
+00000000: 610d 0d0a 0000 0000 6ff7 7d63 e902 0000  a.......o.}c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 4700 6403 6404  d.l.m.Z...G.d.d.
 00000050: 8400 6404 8302 5a05 6405 5300 2906 e900  ..d...Z.d.S.)...
 00000060: 0000 0029 02da 0444 6963 74da 0554 7570  ...)...Dict..Tup
 00000070: 6c65 2901 da0b 506f 7461 746f 4772 6170  le)...PotatoGrap
@@ -20,50 +20,51 @@
 00000130: 0000 0400 0000 0200 0000 4300 0000 7324  ..........C...s$
 00000140: 0000 007c 0164 0119 007c 005f 007c 0164  ...|.d...|._.|.d
 00000150: 0219 007c 005f 017c 037c 005f 027c 027c  ...|._.|.|._.|.|
 00000160: 005f 0364 0053 0029 034e 7201 0000 00e9  ._.d.S.).Nr.....
 00000170: 0100 0000 2904 da04 7465 7874 da05 6c61  ....)...text..la
 00000180: 6265 6c72 0800 0000 7207 0000 0029 04da  belr....r....)..
 00000190: 0473 656c 6672 0600 0000 7207 0000 0072  .selfr....r....r
-000001a0: 0800 0000 a900 720e 0000 00fa 372f 686f  ......r.....7/ho
-000001b0: 6d65 2f61 6461 616d 6b6f 2f70 726f 6a65  me/adaamko/proje
-000001c0: 6374 732f 504f 5441 544f 2f78 706f 7461  cts/POTATO/xpota
-000001d0: 746f 2f64 6174 6173 6574 2f73 616d 706c  to/dataset/sampl
-000001e0: 652e 7079 da08 5f5f 696e 6974 5f5f 0700  e.py..__init__..
-000001f0: 0000 7308 0000 0000 060a 010a 0106 017a  ..s............z
-00000200: 0f53 616d 706c 652e 5f5f 696e 6974 5f5f  .Sample.__init__
-00000210: 2902 da05 6772 6170 6872 0900 0000 6302  )...graphr....c.
-00000220: 0000 0000 0000 0000 0000 0002 0000 0002  ................
-00000230: 0000 0043 0000 0073 0a00 0000 7c01 7c00  ...C...s....|.|.
-00000240: 5f00 6400 5300 a901 4e29 0172 0700 0000  _.d.S...N).r....
-00000250: 2902 720d 0000 0072 1100 0000 720e 0000  ).r....r....r...
-00000260: 0072 0e00 0000 720f 0000 00da 0973 6574  .r....r......set
-00000270: 5f67 7261 7068 1200 0000 7302 0000 0000  _graph....s.....
-00000280: 017a 1053 616d 706c 652e 7365 745f 6772  .z.Sample.set_gr
-00000290: 6170 6829 01da 0b6c 6162 656c 5f76 6f63  aph)...label_voc
-000002a0: 6162 6302 0000 0000 0000 0000 0000 0002  abc.............
-000002b0: 0000 0002 0000 0043 0000 0073 3200 0000  .......C...s2...
-000002c0: 7c00 6a00 6400 7501 7210 7c00 6a00 5300  |.j.d.u.r.|.j.S.
-000002d0: 7c00 6a01 722a 7c00 6a01 7c01 7600 722a  |.j.r*|.j.|.v.r*
-000002e0: 7c01 7c00 6a01 1900 5300 6400 5300 6400  |.|.j...S.d.S.d.
-000002f0: 5300 7212 0000 0029 0272 0800 0000 720c  S.r....).r....r.
-00000300: 0000 0029 0272 0d00 0000 7214 0000 0072  ...).r....r....r
-00000310: 0e00 0000 720e 0000 0072 0f00 0000 da0c  ....r....r......
-00000320: 6765 745f 6c61 6265 6c5f 6964 1500 0000  get_label_id....
-00000330: 730a 0000 0000 010a 0106 0110 010a 027a  s..............z
-00000340: 1353 616d 706c 652e 6765 745f 6c61 6265  .Sample.get_labe
-00000350: 6c5f 6964 2902 4e4e 290b da08 5f5f 6e61  l_id).NN)...__na
-00000360: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000370: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7203  ..__qualname__r.
-00000380: 0000 00da 0373 7472 7204 0000 00da 0369  .....strr......i
-00000390: 6e74 7210 0000 0072 1300 0000 7202 0000  ntr....r....r...
-000003a0: 0072 1500 0000 720e 0000 0072 0e00 0000  .r....r....r....
-000003b0: 720e 0000 0072 0f00 0000 7205 0000 0006  r....r....r.....
-000003c0: 0000 0073 1400 0000 0804 0001 00fc 0202  ...s............
-000003d0: 0a01 0201 0201 02fb 0c0b 1003 7205 0000  ............r...
-000003e0: 004e 2906 da06 7479 7069 6e67 7202 0000  .N)...typingr...
-000003f0: 0072 0300 0000 da1d 7870 6f74 6174 6f2e  .r......xpotato.
-00000400: 6772 6170 685f 6578 7472 6163 746f 722e  graph_extractor.
-00000410: 6772 6170 6872 0400 0000 7205 0000 0072  graphr....r....r
-00000420: 0e00 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
-00000430: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000440: 0073 0400 0000 1002 0c03                 .s........
+000001a0: 0800 0000 a900 720e 0000 00fa 4c2f 5573  ......r.....L/Us
+000001b0: 6572 732f 6164 616d 6b6f 7661 6373 2f70  ers/adamkovacs/p
+000001c0: 726f 6a65 6374 732f 6578 702d 7265 6c61  rojects/exp-rela
+000001d0: 7469 6f6e 2d65 7874 7261 6374 696f 6e2f  tion-extraction/
+000001e0: 7870 6f74 6174 6f2f 6461 7461 7365 742f  xpotato/dataset/
+000001f0: 7361 6d70 6c65 2e70 79da 085f 5f69 6e69  sample.py..__ini
+00000200: 745f 5f07 0000 0073 0800 0000 0006 0a01  t__....s........
+00000210: 0a01 0601 7a0f 5361 6d70 6c65 2e5f 5f69  ....z.Sample.__i
+00000220: 6e69 745f 5f29 02da 0567 7261 7068 7209  nit__)...graphr.
+00000230: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00000240: 0200 0000 0200 0000 4300 0000 730a 0000  ........C...s...
+00000250: 007c 017c 005f 0064 0053 00a9 014e 2901  .|.|._.d.S...N).
+00000260: 7207 0000 0029 0272 0d00 0000 7211 0000  r....).r....r...
+00000270: 0072 0e00 0000 720e 0000 0072 0f00 0000  .r....r....r....
+00000280: da09 7365 745f 6772 6170 6812 0000 0073  ..set_graph....s
+00000290: 0200 0000 0001 7a10 5361 6d70 6c65 2e73  ......z.Sample.s
+000002a0: 6574 5f67 7261 7068 2901 da0b 6c61 6265  et_graph)...labe
+000002b0: 6c5f 766f 6361 6263 0200 0000 0000 0000  l_vocabc........
+000002c0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+000002d0: 7332 0000 007c 006a 0064 0075 0172 107c  s2...|.j.d.u.r.|
+000002e0: 006a 0053 007c 006a 0172 2a7c 006a 017c  .j.S.|.j.r*|.j.|
+000002f0: 0176 0072 2a7c 017c 006a 0119 0053 0064  .v.r*|.|.j...S.d
+00000300: 0053 0064 0053 0072 1200 0000 2902 7208  .S.d.S.r....).r.
+00000310: 0000 0072 0c00 0000 2902 720d 0000 0072  ...r....).r....r
+00000320: 1400 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
+00000330: 0000 00da 0c67 6574 5f6c 6162 656c 5f69  .....get_label_i
+00000340: 6415 0000 0073 0a00 0000 0001 0a01 0601  d....s..........
+00000350: 1001 0a02 7a13 5361 6d70 6c65 2e67 6574  ....z.Sample.get
+00000360: 5f6c 6162 656c 5f69 6429 024e 4e29 0bda  _label_id).NN)..
+00000370: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000380: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000390: 655f 5f72 0300 0000 da03 7374 7272 0400  e__r......strr..
+000003a0: 0000 da03 696e 7472 1000 0000 7213 0000  ....intr....r...
+000003b0: 0072 0200 0000 7215 0000 0072 0e00 0000  .r....r....r....
+000003c0: 720e 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
+000003d0: 0500 0000 0600 0000 7314 0000 0008 0400  ........s.......
+000003e0: 0100 fc02 020a 0102 0102 0102 fb0c 0b10  ................
+000003f0: 0372 0500 0000 4e29 06da 0674 7970 696e  .r....N)...typin
+00000400: 6772 0200 0000 7203 0000 00da 1d78 706f  gr....r......xpo
+00000410: 7461 746f 2e67 7261 7068 5f65 7874 7261  tato.graph_extra
+00000420: 6374 6f72 2e67 7261 7068 7204 0000 0072  ctor.graphr....r
+00000430: 0500 0000 720e 0000 0072 0e00 0000 720e  ....r....r....r.
+00000440: 0000 0072 0f00 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000450: 653e 0100 0000 7304 0000 0010 020c 03    e>....s........
```

### Comparing `xpotato-0.1.4/xpotato/dataset/__pycache__/utils.cpython-39.pyc` & `xpotato-0.1.5/xpotato/dataset/__pycache__/utils.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Mar  9 10:46:32 2022 UTC, .py size: 5127 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,199 +1,208 @@
-00000000: 610d 0d0a 0000 0000 8885 2862 0714 0000  a.........(b....
+00000000: 610d 0d0a 0000 0000 b76f 9763 5114 0000  a........o.cQ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 5a03 6400 6402 6c04 5a05 6400 6402 6c06  Z.d.d.l.Z.d.d.l.
-00000050: 5a07 6400 6403 6c08 6d09 5a09 0100 6400  Z.d.d.l.m.Z...d.
-00000060: 6404 6c08 6d0a 5a0a 0100 6505 6a0b 650c  d.l.m.Z...e.j.e.
-00000070: 6402 6405 9c03 6406 6407 8404 5a0d 6410  d.d...d.d...Z.d.
-00000080: 6409 640a 8401 5a0e 6411 640b 640c 8401  d.d...Z.d.d.d...
-00000090: 5a0f 6412 640e 640f 8401 5a10 6402 5300  Z.d.d.d...Z.d.S.
-000000a0: 2913 e900 0000 0029 01da 0b64 6566 6175  )......)...defau
-000000b0: 6c74 6469 6374 4e29 01da 1470 7265 7072  ltdictN)...prepr
-000000c0: 6f63 6573 735f 6e6f 6465 5f61 6c74 6fa9  ocess_node_alto.
-000000d0: 01da 0b67 7261 7068 5f74 6f5f 706e 2903  ...graph_to_pn).
-000000e0: da02 6466 da04 7061 7468 da06 7265 7475  ..df..path..retu
-000000f0: 726e 6302 0000 0000 0000 0000 0000 0004  rnc.............
-00000100: 0000 0005 0000 0043 0000 0073 3a00 0000  .......C...s:...
-00000110: 7c00 a000 a100 7d02 6401 6402 8400 7c02  |.....}.d.d...|.
-00000120: 6403 1900 a001 a100 4400 8301 7d03 7c03  d.......D...}.|.
-00000130: 7c02 6403 3c00 7c02 6a02 7c01 6404 6405  |.d.<.|.j.|.d.d.
-00000140: 6406 8d03 0100 6400 5300 2907 4e63 0100  d.....d.S.).Nc..
-00000150: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00000160: 0000 5300 0000 7314 0000 0067 007c 005d  ..S...s....g.|.]
-00000170: 0c7d 0174 007c 0183 0191 0271 0453 00a9  .}.t.|.....q.S..
-00000180: 0072 0400 0000 2902 da02 2e30 da05 6772  .r....)....0..gr
-00000190: 6170 6872 0900 0000 7209 0000 00fa 362f  aphr....r.....6/
-000001a0: 686f 6d65 2f61 6461 616d 6b6f 2f70 726f  home/adaamko/pro
-000001b0: 6a65 6374 732f 504f 5441 544f 2f78 706f  jects/POTATO/xpo
-000001c0: 7461 746f 2f64 6174 6173 6574 2f75 7469  tato/dataset/uti
-000001d0: 6c73 2e70 79da 0a3c 6c69 7374 636f 6d70  ls.py..<listcomp
-000001e0: 3e0c 0000 00f3 0000 0000 7a22 7361 7665  >.........z"save
-000001f0: 5f64 6174 6166 7261 6d65 2e3c 6c6f 6361  _dataframe.<loca
-00000200: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 720b  ls>.<listcomp>r.
-00000210: 0000 0046 fa01 0929 02da 0569 6e64 6578  ...F...)...index
-00000220: da03 7365 7029 03da 0463 6f70 79da 0674  ..sep)...copy..t
-00000230: 6f6c 6973 74da 0674 6f5f 6373 7629 0472  olist..to_csv).r
-00000240: 0600 0000 7207 0000 005a 0a64 665f 746f  ....r....Z.df_to
-00000250: 5f73 6176 65da 0667 7261 7068 7372 0900  _save..graphsr..
-00000260: 0000 7209 0000 0072 0c00 0000 da0e 7361  ..r....r......sa
-00000270: 7665 5f64 6174 6166 7261 6d65 0a00 0000  ve_dataframe....
-00000280: 7308 0000 0000 0108 0116 0108 0172 1600  s............r..
-00000290: 0000 da05 636f 6c6f 7263 0200 0000 0000  ....colorc......
-000002a0: 0000 0000 0000 0500 0000 0700 0000 4300  ..............C.
-000002b0: 0000 73b0 0000 0074 00a0 01a1 007d 0264  ..s....t.....}.d
-000002c0: 017d 037c 00a0 02a1 0044 005d 927d 0474  .}.|.....D.].}.t
-000002d0: 037c 0464 0219 0074 0474 0566 0283 0272  .|.d...t.t.f...r
-000002e0: 2c71 147c 026a 067c 0464 0219 0074 077c  ,q.|.j.|.d...t.|
-000002f0: 0464 0319 0083 0164 048d 0201 007c 0464  .d.....d.....|.d
-00000300: 0519 0064 066b 0272 6c7c 0464 0219 007d  ...d.k.rl|.d...}
-00000310: 037c 026a 067c 0464 0719 0064 0664 048d  .|.j.|.d...d.d..
-00000320: 0201 007c 02a0 087c 0464 0719 007c 0464  ...|...|.d...|.d
-00000330: 0219 00a1 0201 007c 027c 0464 0719 0019  .......|.|.d....
-00000340: 007c 0464 0219 0019 00a0 097c 0174 077c  .|.d.......|.t.|
-00000350: 0464 0519 0083 0169 01a1 0101 0071 147c  .d.....i.....q.|
-00000360: 027c 0366 0253 0029 087a 3763 6f6e 7665  .|.f.S.).z7conve
-00000370: 7274 2064 6570 656e 6465 6e63 792d 7061  rt dependency-pa
-00000380: 7273 6564 2073 7461 6e7a 6120 5365 6e74  rsed stanza Sent
-00000390: 656e 6365 2074 6f20 6e78 2e44 6947 7261  ence to nx.DiGra
-000003a0: 7068 4eda 0269 64da 056c 656d 6d61 a901  phN..id..lemma..
-000003b0: da04 6e61 6d65 da06 6465 7072 656c da04  ..name..deprel..
-000003c0: 726f 6f74 da04 6865 6164 290a da02 6e78  root..head)...nx
-000003d0: da07 4469 4772 6170 68da 0774 6f5f 6469  ..DiGraph..to_di
-000003e0: 6374 da0a 6973 696e 7374 616e 6365 da04  ct..isinstance..
-000003f0: 6c69 7374 da05 7475 706c 65da 0861 6464  list..tuple..add
-00000400: 5f6e 6f64 6572 0300 0000 da08 6164 645f  _noder......add_
-00000410: 6564 6765 da06 7570 6461 7465 2905 da03  edge..update)...
-00000420: 7365 6eda 0965 6467 655f 6174 7472 da01  sen..edge_attr..
-00000430: 47da 0772 6f6f 745f 6964 da04 776f 7264  G..root_id..word
-00000440: 7209 0000 0072 0900 0000 720c 0000 00da  r....r....r.....
-00000450: 0b75 645f 746f 5f67 7261 7068 1100 0000  .ud_to_graph....
-00000460: 731c 0000 0000 0208 0104 010c 0112 0202  s...............
-00000470: 011a 010c 0108 0112 0114 0114 010e ff06  ................
-00000480: 0472 2d00 0000 6302 0000 0000 0000 0000  .r-...c.........
-00000490: 0000 000d 0000 0006 0000 0043 0000 0073  ...........C...s
-000004a0: 9801 0000 7400 a001 7c00 a101 7d02 7402  ....t...|...}.t.
-000004b0: a003 a100 7d03 7404 7405 8301 7d04 6401  ....}.t.t...}.d.
-000004c0: 7d05 7406 7c02 6a07 8301 4400 5d8e 5c02  }.t.|.j...D.].\.
-000004d0: 7d06 7d07 7c06 6401 6b02 7270 7c05 7d08  }.}.|.d.k.rp|.}.
-000004e0: 7c07 6402 1900 7d09 7c09 734c 6403 7d09  |.d...}.|.sLd.}.
-000004f0: 7c03 6a08 7c08 7c09 6404 8d02 0100 7c05  |.j.|.|.d.....|.
-00000500: 7c04 7c07 6401 1900 3c00 7c05 6405 3700  |.|.d...<.|.d.7.
-00000510: 7d05 7128 7c07 6405 1900 6406 6b02 7228  }.q(|.d...d.k.r(
-00000520: 7c07 6402 1900 7228 7c07 6402 1900 7d09  |.d...r(|.d...}.
-00000530: 7c09 7394 6403 7d09 7c03 6a08 7c05 7c09  |.s.d.}.|.j.|.|.
-00000540: 6404 8d02 0100 7c05 7c04 7c07 6401 1900  d.....|.|.|.d...
-00000550: 3c00 7c05 6405 3700 7d05 7128 7c02 6a07  <.|.d.7.}.q(|.j.
-00000560: 4400 5dd0 7d07 7c07 6405 1900 6406 6b03  D.].}.|.d...d.k.
-00000570: 72be 7c07 6405 1900 a009 6407 a101 6405  r.|.d.....d...d.
-00000580: 1900 7d0a 7c07 6401 1900 7d0b 7c07 6402  ..}.|.d...}.|.d.
-00000590: 1900 7d0c 7c0b 7c04 7601 9001 7226 7c05  ..}.|.|.v...r&|.
-000005a0: 7c04 7c0b 3c00 7c0b 7d09 7c09 9001 7310  |.|.<.|.}.|...s.
-000005b0: 6403 7d09 7c03 6a08 7c05 7c09 6404 8d02  d.}.|.j.|.|.d...
-000005c0: 0100 7c05 6405 3700 7d05 7c0c 7c04 7601  ..|.d.7.}.|.|.v.
-000005d0: 9001 725c 7c05 7c04 7c0c 3c00 7c0c 7d09  ..r\|.|.|.<.|.}.
-000005e0: 7c09 9001 7346 6403 7d09 7c03 6a08 7c05  |...sFd.}.|.j.|.
-000005f0: 7c09 6404 8d02 0100 7c05 6405 3700 7d05  |.d.....|.d.7.}.
-00000600: 7c03 a00a 7c04 7c0b 1900 7c04 7c0c 1900  |...|.|...|.|...
-00000610: a102 0100 7c03 7c04 7c0b 1900 1900 7c04  ....|.|.|.....|.
-00000620: 7c0c 1900 1900 a00b 7c01 7c0a 6901 a101  |.......|.|.i...
-00000630: 0100 71be 7c03 7c08 6602 5300 2908 4e72  ..q.|.|.f.S.).Nr
-00000640: 0100 0000 e902 0000 00da 044e 6f6e 6572  ...........Noner
-00000650: 1a00 0000 e901 0000 00fa 093a 696e 7374  ...........:inst
-00000660: 616e 6365 fa01 3a29 0cda 0270 6eda 0664  ance..:)...pn..d
-00000670: 6563 6f64 6572 1f00 0000 7220 0000 0072  ecoder....r ...r
-00000680: 0200 0000 da03 696e 74da 0965 6e75 6d65  ......int..enume
-00000690: 7261 7465 da07 7472 6970 6c65 7372 2500  rate..triplesr%.
-000006a0: 0000 da05 7370 6c69 7472 2600 0000 7227  ....splitr&...r'
-000006b0: 0000 0029 0dda 0672 6177 5f64 6c72 2900  ...)...raw_dlr).
-000006c0: 0000 da01 6772 2a00 0000 da0a 6368 6172  ....gr*.....char
-000006d0: 5f74 6f5f 6964 da07 6e65 7874 5f69 64da  _to_id..next_id.
-000006e0: 0169 da04 7472 6970 722b 0000 0072 1b00  .i..tripr+...r..
-000006f0: 0000 da04 6564 6765 da03 7372 63da 0374  ....edge..src..t
-00000700: 6774 7209 0000 0072 0900 0000 720c 0000  gtr....r....r...
-00000710: 00da 1364 6566 6175 6c74 5f70 6e5f 746f  ...default_pn_to
-00000720: 5f67 7261 7068 2500 0000 7356 0000 0000  _graph%...sV....
-00000730: 010a 0108 0208 0104 0112 0108 0104 0108  ................
-00000740: 0104 0104 010e 010c 010a 020c 0108 0108  ................
-00000750: 0104 0104 010e 010c 010a 020a 010c 0112  ................
-00000760: 0108 0108 010a 0108 0104 0106 0104 010e  ................
-00000770: 0108 010a 0108 0104 0106 0104 010e 0108  ................
-00000780: 0214 0120 0272 4200 0000 4663 0300 0000  ... .rB...Fc....
-00000790: 0000 0000 0000 0000 0e00 0000 0600 0000  ................
-000007a0: 4300 0000 7388 0200 0074 00a0 017c 00a1  C...s....t...|..
-000007b0: 017d 0374 02a0 03a1 007d 0474 0474 0583  .}.t.....}.t.t..
-000007c0: 017d 0564 017d 0674 067c 036a 0783 0144  .}.d.}.t.|.j...D
-000007d0: 0090 015d 025c 027d 077d 087c 0764 016b  ...].\.}.}.|.d.k
-000007e0: 0272 aa7c 067d 0964 027c 0864 0319 0076  .r.|.}.d.|.d...v
-000007f0: 0072 6864 02a0 087c 0864 0319 00a0 0964  .rhd...|.d.....d
-00000800: 02a1 0164 0064 0485 0219 00a1 017d 0a6e  ...d.d.......}.n
-00000810: 087c 0864 0319 007d 0a7c 0272 867c 0a72  .|.d...}.|.r.|.r
-00000820: 8274 0a7c 0a83 017d 0a6e 0464 057d 0a7c  .t.|...}.n.d.}.|
-00000830: 046a 0b7c 097c 0a64 068d 0201 007c 067c  .j.|.|.d.....|.|
-00000840: 057c 0864 0119 003c 007c 0664 0737 007d  .|.d...<.|.d.7.}
-00000850: 0671 287c 0864 0719 0064 086b 0272 287c  .q(|.d...d.k.r(|
-00000860: 0864 0319 0072 2864 027c 0864 0319 0076  .d...r(d.|.d...v
-00000870: 0072 e864 02a0 087c 0864 0319 00a0 0964  .r.d...|.d.....d
-00000880: 02a1 0164 0064 0485 0219 00a1 017d 0a6e  ...d.d.......}.n
-00000890: 087c 0864 0319 007d 0a7c 0290 0172 0a7c  .|.d...}.|...r.|
-000008a0: 0a90 0172 0674 0a7c 0a83 017d 0a6e 0464  ...r.t.|...}.n.d
-000008b0: 057d 0a7c 046a 0b7c 067c 0a64 068d 0201  .}.|.j.|.|.d....
-000008c0: 007c 067c 057c 0864 0119 003c 007c 0664  .|.|.|.d...<.|.d
-000008d0: 0737 007d 0671 287c 036a 0744 0090 015d  .7.}.q(|.j.D...]
-000008e0: 487d 087c 0864 0719 0064 086b 0390 0172  H}.|.d...d.k...r
-000008f0: 3464 09a0 087c 0864 0719 00a0 0964 0aa1  4d...|.d.....d..
-00000900: 0164 0719 00a0 0964 02a1 01a1 017d 0b7c  .d.....d.....}.|
-00000910: 0864 0119 007d 0c7c 0864 0319 007d 0d7c  .d...}.|.d...}.|
-00000920: 0c7c 0576 0190 0172 e07c 067c 057c 0c3c  .|.v...r.|.|.|.<
-00000930: 0064 027c 0c76 0090 0172 ac64 02a0 087c  .d.|.v...r.d...|
-00000940: 0ca0 0964 02a1 0164 0064 0485 0219 00a1  ...d...d.d......
-00000950: 017d 0a6e 047c 0c7d 0a7c 0290 0172 ca7c  .}.n.|.}.|...r.|
-00000960: 0a90 0172 c674 0a7c 0a83 017d 0a6e 0464  ...r.t.|...}.n.d
-00000970: 057d 0a7c 046a 0b7c 067c 0a64 068d 0201  .}.|.j.|.|.d....
-00000980: 007c 0664 0737 007d 067c 0d7c 0576 0190  .|.d.7.}.|.|.v..
-00000990: 0272 4a7c 067c 057c 0d3c 0064 027c 0d76  .rJ|.|.|.<.d.|.v
-000009a0: 0090 0272 1664 02a0 087c 0da0 0964 02a1  ...r.d...|...d..
-000009b0: 0164 0064 0485 0219 00a1 017d 0a6e 047c  .d.d.......}.n.|
-000009c0: 0d7d 0a7c 0290 0272 347c 0a90 0272 3074  .}.|...r4|...r0t
-000009d0: 0a7c 0a83 017d 0a6e 0464 057d 0a7c 046a  .|...}.n.d.}.|.j
-000009e0: 0b7c 067c 0a64 068d 0201 007c 0664 0737  .|.|.d.....|.d.7
-000009f0: 007d 067c 04a0 0c7c 057c 0c19 007c 057c  .}.|...|.|...|.|
-00000a00: 0d19 00a1 0201 007c 047c 057c 0c19 0019  .......|.|.|....
-00000a10: 007c 057c 0d19 0019 00a0 0d7c 017c 0b69  .|.|.......|.|.i
-00000a20: 01a1 0101 0090 0171 347c 047c 0966 0253  .......q4|.|.f.S
-00000a30: 0029 0b4e 7201 0000 00fa 012d 722e 0000  .).Nr......-r...
-00000a40: 00e9 ffff ffff 722f 0000 0072 1a00 0000  ......r/...r....
-00000a50: 7230 0000 0072 3100 0000 da00 7232 0000  r0...r1.....r2..
-00000a60: 0029 0e72 3300 0000 7234 0000 0072 1f00  .).r3...r4...r..
-00000a70: 0000 7220 0000 0072 0200 0000 7235 0000  ..r ...r....r5..
-00000a80: 0072 3600 0000 7237 0000 00da 046a 6f69  .r6...r7.....joi
-00000a90: 6e72 3800 0000 7203 0000 0072 2500 0000  nr8...r....r%...
-00000aa0: 7226 0000 0072 2700 0000 290e 7239 0000  r&...r'...).r9..
-00000ab0: 0072 2900 0000 5a0b 636c 6561 6e5f 6e6f  .r)...Z.clean_no
-00000ac0: 6465 7372 3a00 0000 722a 0000 0072 3b00  desr:...r*...r;.
-00000ad0: 0000 723c 0000 0072 3d00 0000 723e 0000  ..r<...r=...r>..
-00000ae0: 0072 2b00 0000 721b 0000 0072 3f00 0000  .r+...r....r?...
-00000af0: 7240 0000 0072 4100 0000 7209 0000 0072  r@...rA...r....r
-00000b00: 0900 0000 720c 0000 00da 0f61 6d72 5f70  ....r......amr_p
-00000b10: 6e5f 746f 5f67 7261 7068 5800 0000 7376  n_to_graphX...sv
-00000b20: 0000 0000 010a 0108 0208 0104 0114 0108  ................
-00000b30: 0104 010c 011e 0208 0104 0104 010a 0204  ................
-00000b40: 010e 010c 010a 020c 0108 010c 011e 0208  ................
-00000b50: 0106 0106 010a 0204 010e 010c 010a 020c  ................
-00000b60: 010e 011e 0108 0108 010a 0108 010a 011a  ................
-00000b70: 0204 0106 0106 010a 0204 010e 0108 010a  ................
-00000b80: 0108 010a 011a 0204 0106 0106 010a 0204  ................
-00000b90: 010e 0108 0214 0122 0272 4700 0000 2901  .......".rG...).
-00000ba0: 7217 0000 0029 0172 1700 0000 2902 7217  r....).r....).r.
-00000bb0: 0000 0046 2911 da0b 636f 6c6c 6563 7469  ...F)...collecti
-00000bc0: 6f6e 7372 0200 0000 da08 6e65 7477 6f72  onsr......networ
-00000bd0: 6b78 721f 0000 00da 0670 616e 6461 73da  kxr......pandas.
-00000be0: 0270 64da 0670 656e 6d61 6e72 3300 0000  .pd..penmanr3...
-00000bf0: da13 7475 775f 6e6c 702e 6772 6170 682e  ..tuw_nlp.graph.
-00000c00: 7574 696c 7372 0300 0000 7205 0000 00da  utilsr....r.....
-00000c10: 0944 6174 6146 7261 6d65 da03 7374 7272  .DataFrame..strr
-00000c20: 1600 0000 722d 0000 0072 4200 0000 7247  ....r-...rB...rG
-00000c30: 0000 0072 0900 0000 7209 0000 0072 0900  ...r....r....r..
-00000c40: 0000 720c 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000c50: 3e01 0000 0073 1200 0000 0c02 0801 0801  >....s..........
-00000c60: 0801 0c01 0c03 1407 0a14 0a33            ...........3
+00000020: 0004 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
+00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
+00000040: 0100 6400 6401 6c03 5a04 6400 6401 6c05  ..d.d.l.Z.d.d.l.
+00000050: 5a06 6400 6401 6c07 5a08 6400 6403 6c09  Z.d.d.l.Z.d.d.l.
+00000060: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
+00000070: 0100 6506 6a0d 650e 6401 6405 9c03 6406  ..e.j.e.d.d...d.
+00000080: 6407 8404 5a0f 6410 6409 640a 8401 5a10  d...Z.d.d.d...Z.
+00000090: 6411 640b 640c 8401 5a11 6412 640e 640f  d.d.d...Z.d.d.d.
+000000a0: 8401 5a12 6401 5300 2913 e900 0000 004e  ..Z.d.S.)......N
+000000b0: 2901 da0b 6465 6661 756c 7464 6963 7429  )...defaultdict)
+000000c0: 01da 0a6a 736f 6e5f 6772 6170 6829 01da  ...json_graph)..
+000000d0: 1470 7265 7072 6f63 6573 735f 6e6f 6465  .preprocess_node
+000000e0: 5f61 6c74 6f29 03da 0264 66da 0470 6174  _alto)...df..pat
+000000f0: 68da 0672 6574 7572 6e63 0200 0000 0000  h..returnc......
+00000100: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
+00000110: 0000 733a 0000 007c 00a0 00a1 007d 0264  ..s:...|.....}.d
+00000120: 0164 0284 007c 0064 0319 00a0 01a1 0044  .d...|.d.......D
+00000130: 0083 017d 037c 037c 0264 033c 007c 026a  ...}.|.|.d.<.|.j
+00000140: 027c 0164 0464 0564 068d 0301 0064 0053  .|.d.d.d.....d.S
+00000150: 0029 074e 6301 0000 0000 0000 0000 0000  .).Nc...........
+00000160: 0002 0000 0007 0000 0053 0000 0073 2e00  .........S...s..
+00000170: 0000 6700 7c00 5d26 7d01 7400 7c01 8301  ..g.|.]&}.t.|...
+00000180: 7401 6a02 6b02 7226 7403 a004 7405 a006  t.j.k.r&t...t...
+00000190: 7c01 a101 a101 6e02 7c01 9102 7104 5300  |.....n.|...q.S.
+000001a0: a900 2907 da04 7479 7065 da02 6e78 da07  ..)...type..nx..
+000001b0: 4469 4772 6170 68da 046a 736f 6eda 0564  DiGraph..json..d
+000001c0: 756d 7073 7203 0000 00da 0e61 646a 6163  umpsr......adjac
+000001d0: 656e 6379 5f64 6174 6129 02da 022e 30da  ency_data)....0.
+000001e0: 0167 7208 0000 0072 0800 0000 fa4b 2f55  .gr....r.....K/U
+000001f0: 7365 7273 2f61 6461 6d6b 6f76 6163 732f  sers/adamkovacs/
+00000200: 7072 6f6a 6563 7473 2f65 7870 2d72 656c  projects/exp-rel
+00000210: 6174 696f 6e2d 6578 7472 6163 7469 6f6e  ation-extraction
+00000220: 2f78 706f 7461 746f 2f64 6174 6173 6574  /xpotato/dataset
+00000230: 2f75 7469 6c73 2e70 79da 0a3c 6c69 7374  /utils.py..<list
+00000240: 636f 6d70 3e0d 0000 0073 0400 0000 0602  comp>....s......
+00000250: 02ff 7a22 7361 7665 5f64 6174 6166 7261  ..z"save_datafra
+00000260: 6d65 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  me.<locals>.<lis
+00000270: 7463 6f6d 703e da05 6772 6170 6846 fa01  tcomp>..graphF..
+00000280: 0929 02da 0569 6e64 6578 da03 7365 7029  .)...index..sep)
+00000290: 03da 0463 6f70 79da 0674 6f6c 6973 74da  ...copy..tolist.
+000002a0: 0674 6f5f 6373 7629 0472 0500 0000 7206  .to_csv).r....r.
+000002b0: 0000 005a 0a64 665f 746f 5f73 6176 65da  ...Z.df_to_save.
+000002c0: 0667 7261 7068 7372 0800 0000 7208 0000  .graphsr....r...
+000002d0: 0072 1100 0000 da0e 7361 7665 5f64 6174  .r......save_dat
+000002e0: 6166 7261 6d65 0b00 0000 730c 0000 0000  aframe....s.....
+000002f0: 0108 0106 020a fe06 0408 0172 1b00 0000  ...........r....
+00000300: da05 636f 6c6f 7263 0200 0000 0000 0000  ..colorc........
+00000310: 0000 0000 0500 0000 0700 0000 4300 0000  ............C...
+00000320: 73b0 0000 0074 00a0 01a1 007d 0264 017d  s....t.....}.d.}
+00000330: 037c 00a0 02a1 0044 005d 927d 0474 037c  .|.....D.].}.t.|
+00000340: 0464 0219 0074 0474 0566 0283 0272 2c71  .d...t.t.f...r,q
+00000350: 147c 026a 067c 0464 0219 0074 077c 0464  .|.j.|.d...t.|.d
+00000360: 0319 0083 0164 048d 0201 007c 0464 0519  .....d.....|.d..
+00000370: 0064 066b 0272 6c7c 0464 0219 007d 037c  .d.k.rl|.d...}.|
+00000380: 026a 067c 0464 0719 0064 0664 048d 0201  .j.|.d...d.d....
+00000390: 007c 02a0 087c 0464 0719 007c 0464 0219  .|...|.d...|.d..
+000003a0: 00a1 0201 007c 027c 0464 0719 0019 007c  .....|.|.d.....|
+000003b0: 0464 0219 0019 00a0 097c 0174 077c 0464  .d.......|.t.|.d
+000003c0: 0519 0083 0169 01a1 0101 0071 147c 027c  .....i.....q.|.|
+000003d0: 0366 0253 0029 087a 3763 6f6e 7665 7274  .f.S.).z7convert
+000003e0: 2064 6570 656e 6465 6e63 792d 7061 7273   dependency-pars
+000003f0: 6564 2073 7461 6e7a 6120 5365 6e74 656e  ed stanza Senten
+00000400: 6365 2074 6f20 6e78 2e44 6947 7261 7068  ce to nx.DiGraph
+00000410: 4eda 0269 64da 056c 656d 6d61 a901 da04  N..id..lemma....
+00000420: 6e61 6d65 da06 6465 7072 656c da04 726f  name..deprel..ro
+00000430: 6f74 da04 6865 6164 290a 720a 0000 0072  ot..head).r....r
+00000440: 0b00 0000 da07 746f 5f64 6963 74da 0a69  ......to_dict..i
+00000450: 7369 6e73 7461 6e63 65da 046c 6973 74da  sinstance..list.
+00000460: 0574 7570 6c65 da08 6164 645f 6e6f 6465  .tuple..add_node
+00000470: 7204 0000 00da 0861 6464 5f65 6467 65da  r......add_edge.
+00000480: 0675 7064 6174 6529 05da 0373 656e da09  .update)...sen..
+00000490: 6564 6765 5f61 7474 72da 0147 da07 726f  edge_attr..G..ro
+000004a0: 6f74 5f69 64da 0477 6f72 6472 0800 0000  ot_id..wordr....
+000004b0: 7208 0000 0072 1100 0000 da0b 7564 5f74  r....r......ud_t
+000004c0: 6f5f 6772 6170 6815 0000 0073 1c00 0000  o_graph....s....
+000004d0: 0002 0801 0401 0c01 1202 0201 1a01 0c01  ................
+000004e0: 0801 1201 1401 1401 0eff 0604 7230 0000  ............r0..
+000004f0: 0063 0200 0000 0000 0000 0000 0000 0d00  .c..............
+00000500: 0000 0600 0000 4300 0000 7398 0100 0074  ......C...s....t
+00000510: 00a0 017c 00a1 017d 0274 02a0 03a1 007d  ...|...}.t.....}
+00000520: 0374 0474 0583 017d 0464 017d 0574 067c  .t.t...}.d.}.t.|
+00000530: 026a 0783 0144 005d 8e5c 027d 067d 077c  .j...D.].\.}.}.|
+00000540: 0664 016b 0272 707c 057d 087c 0764 0219  .d.k.rp|.}.|.d..
+00000550: 007d 097c 0973 4c64 037d 097c 036a 087c  .}.|.sLd.}.|.j.|
+00000560: 087c 0964 048d 0201 007c 057c 047c 0764  .|.d.....|.|.|.d
+00000570: 0119 003c 007c 0564 0537 007d 0571 287c  ...<.|.d.7.}.q(|
+00000580: 0764 0519 0064 066b 0272 287c 0764 0219  .d...d.k.r(|.d..
+00000590: 0072 287c 0764 0219 007d 097c 0973 9464  .r(|.d...}.|.s.d
+000005a0: 037d 097c 036a 087c 057c 0964 048d 0201  .}.|.j.|.|.d....
+000005b0: 007c 057c 047c 0764 0119 003c 007c 0564  .|.|.|.d...<.|.d
+000005c0: 0537 007d 0571 287c 026a 0744 005d d07d  .7.}.q(|.j.D.].}
+000005d0: 077c 0764 0519 0064 066b 0372 be7c 0764  .|.d...d.k.r.|.d
+000005e0: 0519 00a0 0964 07a1 0164 0519 007d 0a7c  .....d...d...}.|
+000005f0: 0764 0119 007d 0b7c 0764 0219 007d 0c7c  .d...}.|.d...}.|
+00000600: 0b7c 0476 0190 0172 267c 057c 047c 0b3c  .|.v...r&|.|.|.<
+00000610: 007c 0b7d 097c 0990 0173 1064 037d 097c  .|.}.|...s.d.}.|
+00000620: 036a 087c 057c 0964 048d 0201 007c 0564  .j.|.|.d.....|.d
+00000630: 0537 007d 057c 0c7c 0476 0190 0172 5c7c  .7.}.|.|.v...r\|
+00000640: 057c 047c 0c3c 007c 0c7d 097c 0990 0173  .|.|.<.|.}.|...s
+00000650: 4664 037d 097c 036a 087c 057c 0964 048d  Fd.}.|.j.|.|.d..
+00000660: 0201 007c 0564 0537 007d 057c 03a0 0a7c  ...|.d.7.}.|...|
+00000670: 047c 0b19 007c 047c 0c19 00a1 0201 007c  .|...|.|.......|
+00000680: 037c 047c 0b19 0019 007c 047c 0c19 0019  .|.|.....|.|....
+00000690: 00a0 0b7c 017c 0a69 01a1 0101 0071 be7c  ...|.|.i.....q.|
+000006a0: 037c 0866 0253 0029 084e 7201 0000 00e9  .|.f.S.).Nr.....
+000006b0: 0200 0000 da04 4e6f 6e65 721f 0000 00e9  ......Noner.....
+000006c0: 0100 0000 fa09 3a69 6e73 7461 6e63 65fa  ......:instance.
+000006d0: 013a 290c da02 706e da06 6465 636f 6465  .:)...pn..decode
+000006e0: 720a 0000 0072 0b00 0000 7202 0000 00da  r....r....r.....
+000006f0: 0369 6e74 da09 656e 756d 6572 6174 65da  .int..enumerate.
+00000700: 0774 7269 706c 6573 7228 0000 00da 0573  .triplesr(.....s
+00000710: 706c 6974 7229 0000 0072 2a00 0000 290d  plitr)...r*...).
+00000720: da06 7261 775f 646c 722c 0000 0072 1000  ..raw_dlr,...r..
+00000730: 0000 722d 0000 00da 0a63 6861 725f 746f  ..r-.....char_to
+00000740: 5f69 64da 076e 6578 745f 6964 da01 69da  _id..next_id..i.
+00000750: 0474 7269 7072 2e00 0000 7220 0000 00da  .tripr....r ....
+00000760: 0465 6467 65da 0373 7263 da03 7467 7472  .edge..src..tgtr
+00000770: 0800 0000 7208 0000 0072 1100 0000 da13  ....r....r......
+00000780: 6465 6661 756c 745f 706e 5f74 6f5f 6772  default_pn_to_gr
+00000790: 6170 6829 0000 0073 5600 0000 0001 0a01  aph)...sV.......
+000007a0: 0802 0801 0401 1201 0801 0401 0801 0401  ................
+000007b0: 0401 0e01 0c01 0a02 0c01 0801 0801 0401  ................
+000007c0: 0401 0e01 0c01 0a02 0a01 0c01 1201 0801  ................
+000007d0: 0801 0a01 0801 0401 0601 0401 0e01 0801  ................
+000007e0: 0a01 0801 0401 0601 0401 0e01 0802 1401  ................
+000007f0: 2002 7244 0000 0046 6303 0000 0000 0000   .rD...Fc.......
+00000800: 0000 0000 000e 0000 0006 0000 0043 0000  .............C..
+00000810: 0073 8802 0000 7400 a001 7c00 a101 7d03  .s....t...|...}.
+00000820: 7402 a003 a100 7d04 7404 7405 8301 7d05  t.....}.t.t...}.
+00000830: 6401 7d06 7406 7c03 6a07 8301 4400 9001  d.}.t.|.j...D...
+00000840: 5d02 5c02 7d07 7d08 7c07 6401 6b02 72aa  ].\.}.}.|.d.k.r.
+00000850: 7c06 7d09 6402 7c08 6403 1900 7600 7268  |.}.d.|.d...v.rh
+00000860: 6402 a008 7c08 6403 1900 a009 6402 a101  d...|.d.....d...
+00000870: 6400 6404 8502 1900 a101 7d0a 6e08 7c08  d.d.......}.n.|.
+00000880: 6403 1900 7d0a 7c02 7286 7c0a 7282 740a  d...}.|.r.|.r.t.
+00000890: 7c0a 8301 7d0a 6e04 6405 7d0a 7c04 6a0b  |...}.n.d.}.|.j.
+000008a0: 7c09 7c0a 6406 8d02 0100 7c06 7c05 7c08  |.|.d.....|.|.|.
+000008b0: 6401 1900 3c00 7c06 6407 3700 7d06 7128  d...<.|.d.7.}.q(
+000008c0: 7c08 6407 1900 6408 6b02 7228 7c08 6403  |.d...d.k.r(|.d.
+000008d0: 1900 7228 6402 7c08 6403 1900 7600 72e8  ..r(d.|.d...v.r.
+000008e0: 6402 a008 7c08 6403 1900 a009 6402 a101  d...|.d.....d...
+000008f0: 6400 6404 8502 1900 a101 7d0a 6e08 7c08  d.d.......}.n.|.
+00000900: 6403 1900 7d0a 7c02 9001 720a 7c0a 9001  d...}.|...r.|...
+00000910: 7206 740a 7c0a 8301 7d0a 6e04 6405 7d0a  r.t.|...}.n.d.}.
+00000920: 7c04 6a0b 7c06 7c0a 6406 8d02 0100 7c06  |.j.|.|.d.....|.
+00000930: 7c05 7c08 6401 1900 3c00 7c06 6407 3700  |.|.d...<.|.d.7.
+00000940: 7d06 7128 7c03 6a07 4400 9001 5d48 7d08  }.q(|.j.D...]H}.
+00000950: 7c08 6407 1900 6408 6b03 9001 7234 6409  |.d...d.k...r4d.
+00000960: a008 7c08 6407 1900 a009 640a a101 6407  ..|.d.....d...d.
+00000970: 1900 a009 6402 a101 a101 7d0b 7c08 6401  ....d.....}.|.d.
+00000980: 1900 7d0c 7c08 6403 1900 7d0d 7c0c 7c05  ..}.|.d...}.|.|.
+00000990: 7601 9001 72e0 7c06 7c05 7c0c 3c00 6402  v...r.|.|.|.<.d.
+000009a0: 7c0c 7600 9001 72ac 6402 a008 7c0c a009  |.v...r.d...|...
+000009b0: 6402 a101 6400 6404 8502 1900 a101 7d0a  d...d.d.......}.
+000009c0: 6e04 7c0c 7d0a 7c02 9001 72ca 7c0a 9001  n.|.}.|...r.|...
+000009d0: 72c6 740a 7c0a 8301 7d0a 6e04 6405 7d0a  r.t.|...}.n.d.}.
+000009e0: 7c04 6a0b 7c06 7c0a 6406 8d02 0100 7c06  |.j.|.|.d.....|.
+000009f0: 6407 3700 7d06 7c0d 7c05 7601 9002 724a  d.7.}.|.|.v...rJ
+00000a00: 7c06 7c05 7c0d 3c00 6402 7c0d 7600 9002  |.|.|.<.d.|.v...
+00000a10: 7216 6402 a008 7c0d a009 6402 a101 6400  r.d...|...d...d.
+00000a20: 6404 8502 1900 a101 7d0a 6e04 7c0d 7d0a  d.......}.n.|.}.
+00000a30: 7c02 9002 7234 7c0a 9002 7230 740a 7c0a  |...r4|...r0t.|.
+00000a40: 8301 7d0a 6e04 6405 7d0a 7c04 6a0b 7c06  ..}.n.d.}.|.j.|.
+00000a50: 7c0a 6406 8d02 0100 7c06 6407 3700 7d06  |.d.....|.d.7.}.
+00000a60: 7c04 a00c 7c05 7c0c 1900 7c05 7c0d 1900  |...|.|...|.|...
+00000a70: a102 0100 7c04 7c05 7c0c 1900 1900 7c05  ....|.|.|.....|.
+00000a80: 7c0d 1900 1900 a00d 7c01 7c0b 6901 a101  |.......|.|.i...
+00000a90: 0100 9001 7134 7c04 7c09 6602 5300 290b  ....q4|.|.f.S.).
+00000aa0: 4e72 0100 0000 da01 2d72 3100 0000 e9ff  Nr......-r1.....
+00000ab0: ffff ff72 3200 0000 721f 0000 0072 3300  ...r2...r....r3.
+00000ac0: 0000 7234 0000 00da 0072 3500 0000 290e  ..r4.....r5...).
+00000ad0: 7236 0000 0072 3700 0000 720a 0000 0072  r6...r7...r....r
+00000ae0: 0b00 0000 7202 0000 0072 3800 0000 7239  ....r....r8...r9
+00000af0: 0000 0072 3a00 0000 da04 6a6f 696e 723b  ...r:.....joinr;
+00000b00: 0000 0072 0400 0000 7228 0000 0072 2900  ...r....r(...r).
+00000b10: 0000 722a 0000 0029 0e72 3c00 0000 722c  ..r*...).r<...r,
+00000b20: 0000 005a 0b63 6c65 616e 5f6e 6f64 6573  ...Z.clean_nodes
+00000b30: 7210 0000 0072 2d00 0000 723d 0000 0072  r....r-...r=...r
+00000b40: 3e00 0000 723f 0000 0072 4000 0000 722e  >...r?...r@...r.
+00000b50: 0000 0072 2000 0000 7241 0000 0072 4200  ...r ...rA...rB.
+00000b60: 0000 7243 0000 0072 0800 0000 7208 0000  ..rC...r....r...
+00000b70: 0072 1100 0000 da0f 616d 725f 706e 5f74  .r......amr_pn_t
+00000b80: 6f5f 6772 6170 685c 0000 0073 7600 0000  o_graph\...sv...
+00000b90: 0001 0a01 0802 0801 0401 1401 0801 0401  ................
+00000ba0: 0c01 1e02 0801 0401 0401 0a02 0401 0e01  ................
+00000bb0: 0c01 0a02 0c01 0801 0c01 1e02 0801 0601  ................
+00000bc0: 0601 0a02 0401 0e01 0c01 0a02 0c01 0e01  ................
+00000bd0: 1e01 0801 0801 0a01 0801 0a01 1a02 0401  ................
+00000be0: 0601 0601 0a02 0401 0e01 0801 0a01 0801  ................
+00000bf0: 0a01 1a02 0401 0601 0601 0a02 0401 0e01  ................
+00000c00: 0802 1401 2202 7249 0000 0029 0172 1c00  ....".rI...).r..
+00000c10: 0000 2901 721c 0000 0029 0272 1c00 0000  ..).r....).r....
+00000c20: 4629 1372 0c00 0000 da0b 636f 6c6c 6563  F).r......collec
+00000c30: 7469 6f6e 7372 0200 0000 da08 6e65 7477  tionsr......netw
+00000c40: 6f72 6b78 720a 0000 00da 0670 616e 6461  orkxr......panda
+00000c50: 73da 0270 64da 0670 656e 6d61 6e72 3600  s..pd..penmanr6.
+00000c60: 0000 da12 6e65 7477 6f72 6b78 2e72 6561  ....networkx.rea
+00000c70: 6477 7269 7465 7203 0000 00da 1374 7577  dwriter......tuw
+00000c80: 5f6e 6c70 2e67 7261 7068 2e75 7469 6c73  _nlp.graph.utils
+00000c90: 7204 0000 00da 0944 6174 6146 7261 6d65  r......DataFrame
+00000ca0: da03 7374 7272 1b00 0000 7230 0000 0072  ..strr....r0...r
+00000cb0: 4400 0000 7249 0000 0072 0800 0000 7208  D...rI...r....r.
+00000cc0: 0000 0072 0800 0000 7211 0000 00da 083c  ...r....r......<
+00000cd0: 6d6f 6475 6c65 3e01 0000 0073 1400 0000  module>....s....
+00000ce0: 0801 0c02 0801 0801 0801 0c01 0c03 140a  ................
+00000cf0: 0a14 0a33                                ...3
```

### Comparing `xpotato-0.1.4/xpotato/dataset/dataset.py` & `xpotato-0.1.5/xpotato/dataset/dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+import json
 from re import I
-from typing import List, Tuple, Dict
+from typing import Dict, List, Tuple
 
 import networkx as nx
 import pandas as pd
-
+from networkx.readwrite import json_graph
 from tqdm import tqdm
-from tuw_nlp.graph.utils import graph_to_pn
+from tuw_nlp.graph.utils import check_if_str_is_penman, graph_to_pn
+
 from xpotato.dataset.sample import Sample
 from xpotato.graph_extractor.extract import GraphExtractor
 from xpotato.graph_extractor.graph import PotatoGraph
 
 
 class Dataset:
     def __init__(
@@ -31,15 +33,18 @@
         self.extractor = GraphExtractor(
             lang=lang, cache_dir=cache_dir, cache_fn=cache_fn
         )
         self.graphs = None
 
     @staticmethod
     def save_dataframe(df: pd.DataFrame, path: str) -> None:
-        graphs = [graph_to_pn(graph) for graph in df["graph"].tolist()]
+        graphs = [
+            json.dumps(json_graph.adjacency_data(g)) if type(g) == nx.DiGraph else g
+            for g in df["graph"].tolist()
+        ]
         df["graph"] = graphs
         df.to_csv(path, index=False, sep="\t")
 
     def prune_graphs(self, graphs: List[nx.DiGraph] = None) -> None:
         graphs_str = []
         for i, graph in enumerate(graphs):
             graph.remove_nodes_from(list(nx.isolates(graph)))
@@ -66,30 +71,31 @@
 
     def read_dataset(
         self,
         examples: List[Tuple[str, str]] = None,
         path: str = None,
         binary: bool = False,
     ) -> List[Sample]:
-        examples = list(examples)
         if examples:
             return [Sample(example, PotatoGraph()) for example in examples]
         elif path:
             if binary:
                 df = pd.read_pickle(path)
-                graphs_str = self.prune_graphs(df.graph.tolist())
-                df.drop(columns=["graph"], inplace=True)
-                df["graph"] = graphs_str
+                graphs = [graph for graph in df["graph"].tolist()]
+                if type(graphs[0]) == str and check_if_str_is_penman(graphs[0]):
+                    graphs_str = self.prune_graphs(df.graph.tolist())
+                    df.drop(columns=["graph"], inplace=True)
+                    df["graph"] = graphs_str
             else:
                 df = pd.read_csv(path, sep="\t")
 
             return [
                 Sample(
                     (example["text"], example["label"]),
-                    potato_graph=PotatoGraph(graph_str=example["graph"]),
+                    potato_graph=PotatoGraph(graph=example["graph"]),
                     label_id=example["label_id"],
                 )
                 for _, example in tqdm(df.iterrows())
             ]
         else:
             raise ValueError("No examples or path provided")
 
@@ -97,61 +103,73 @@
     def _random_postprocess(self, graph: nx.DiGraph) -> nx.DiGraph:
         for node, attr in graph.nodes(data=True):
             if len(attr["name"].split()) > 1:
                 attr["name"] = attr["name"].split()[0]
 
         return graph
 
-    def to_dataframe(self, as_penman: bool = False) -> pd.DataFrame:
+    def to_dataframe(
+        self, as_penman: bool = False, as_json: bool = False
+    ) -> pd.DataFrame:
         df = pd.DataFrame(
             {
                 "text": [sample.text for sample in self._dataset],
                 "label": [sample.label for sample in self._dataset],
                 "label_id": [
                     sample.get_label_id(self.label_vocab) for sample in self._dataset
                 ],
                 "graph": [
-                    str(sample.potato_graph) if as_penman else sample.potato_graph.graph
+                    str(sample.potato_graph)
+                    if as_penman
+                    else sample.potato_graph.to_dict()
+                    if as_json
+                    else sample.potato_graph.graph.G
                     for sample in self._dataset
                 ],
             }
         )
         return df
 
     def parse_graphs(self, graph_format: str = "fourlang") -> List[PotatoGraph]:
         graphs = list(
             self.extractor.parse_iterable(
                 [sample.text for sample in self._dataset], graph_format
             )
         )
 
-        self.graphs = [PotatoGraph(graph) for graph in graphs]
+        self.graphs = [PotatoGraph(graph=graph) for graph in graphs]
         return self.graphs
 
     def set_graphs(self, graphs: List[PotatoGraph]) -> None:
         for sample, potato_graph in zip(self._dataset, graphs):
-            potato_graph.graph.remove_edges_from(nx.selfloop_edges(potato_graph.graph))
+            potato_graph.graph.G.remove_edges_from(
+                nx.selfloop_edges(potato_graph.graph.G)
+            )
             sample.set_graph(potato_graph)
 
     def load_graphs(self, path: str, binary: bool = False) -> None:
         if binary:
             graphs = [graph for graph in pd.read_pickle(path)]
             graph_str = self.prune_graphs(graphs)
 
-            graphs = [PotatoGraph(graph_str=graph) for graph in graph_str]
+            graphs = [PotatoGraph(graph=graph) for graph in graph_str]
             self.graphs = graphs
         else:
             with open(path, "rb") as f:
                 for line in f:
-                    graph = PotatoGraph(graph_str=line.strip())
+                    graph = PotatoGraph(graph=line.strip())
                     self.graphs.append(graph)
 
         self.set_graphs(self.graphs)
 
     def save_dataset(self, path: str) -> None:
-        df = self.to_dataframe(as_penman=True)
-        df.to_csv(path, index=False, sep="\t")
+        df = self.to_dataframe()
+        self.save_dataframe(df, path)
 
-    def save_graphs(self, path: str) -> None:
+    def save_graphs(self, path: str, type="dict") -> None:
         with open(path, "wb") as f:
             for graph in self.graphs:
-                f.write(str(graph) + "\n")
+                if type == "dict":
+                    json.dump(graph.graph, f)
+                    f.write("\n")
+                elif type == "penman":
+                    f.write(f"{str(graph)}\n")
```

### Comparing `xpotato-0.1.4/xpotato/dataset/explainable_dataset.py` & `xpotato-0.1.5/xpotato/dataset/explainable_dataset.py`

 * *Files identical despite different names*

### Comparing `xpotato-0.1.4/xpotato/dataset/explainable_sample.py` & `xpotato-0.1.5/xpotato/dataset/explainable_sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import Tuple, Dict
+from typing import Dict, Tuple
+
 import networkx as nx
-from xpotato.dataset.sample import Sample
 
+from xpotato.dataset.sample import Sample
 from xpotato.graph_extractor.graph import PotatoGraph
 
 
 class ExplainableSample(Sample):
     def __init__(
         self,
         example: Tuple[str, str],
```

### Comparing `xpotato-0.1.4/xpotato/dataset/relation_dataset.py` & `xpotato-0.1.5/xpotato/dataset/relation_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Dict, List, Tuple
 
 import pandas as pd
+
 from xpotato.dataset.dataset import Dataset
 from xpotato.dataset.relation_sample import RelationSample
 
 
 class RelationDataset(Dataset):
     def __init__(
         self, examples: List[Tuple[str, str]], label_vocab: Dict[str, int], lang="en"
```

### Comparing `xpotato-0.1.4/xpotato/dataset/relation_sample.py` & `xpotato-0.1.5/xpotato/dataset/relation_sample.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Tuple
+
 import networkx as nx
+
 from xpotato.dataset.sample import Sample
 
 
 class RelationSample(Sample):
     def __init__(self, example: Tuple[str, str]) -> None:
         super().__init__(example=example)
         self.e1 = example[2]
```

### Comparing `xpotato-0.1.4/xpotato/dataset/sample.py` & `xpotato-0.1.5/xpotato/dataset/sample.py`

 * *Files identical despite different names*

### Comparing `xpotato-0.1.4/xpotato/dataset/utils.py` & `xpotato-0.1.5/xpotato/dataset/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+import json
 from collections import defaultdict
 
 import networkx as nx
 import pandas as pd
 import penman as pn
+from networkx.readwrite import json_graph
 from tuw_nlp.graph.utils import preprocess_node_alto
-from tuw_nlp.graph.utils import graph_to_pn
 
 
 def save_dataframe(df: pd.DataFrame, path: str) -> None:
     df_to_save = df.copy()
-    graphs = [graph_to_pn(graph) for graph in df_to_save["graph"].tolist()]
+    graphs = [
+        json.dumps(json_graph.adjacency_data(g)) if type(g) == nx.DiGraph else g
+        for g in df["graph"].tolist()
+    ]
     df_to_save["graph"] = graphs
     df_to_save.to_csv(path, index=False, sep="\t")
 
 
 def ud_to_graph(sen, edge_attr="color"):
     """convert dependency-parsed stanza Sentence to nx.DiGraph"""
     G = nx.DiGraph()
```

### Comparing `xpotato-0.1.4/xpotato/features/utils.py` & `xpotato-0.1.5/xpotato/features/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -33,8 +33,8 @@
         for k in features:
             lab = k[2]
             if label and label != lab:
                 continue
             labels.add(lab)
             all_features.append(k)
 
-    return all_features, labels
+    return all_features, labels
```

### Comparing `xpotato-0.1.4/xpotato/graph_extractor/__pycache__/extract.cpython-39.pyc` & `xpotato-0.1.5/xpotato/graph_extractor/__pycache__/extract.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Jul  4 09:01:31 2022 UTC, .py size: 18264 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,759 +1,809 @@
-00000000: 610d 0d0a 0000 0000 6bac c262 5847 0000  a.......k..bXG..
+00000000: 610d 0d0a 0000 0000 a735 0f64 d650 0000  a........5.d.P..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 bc00 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 8c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a05 6400 6401 6c06 5a07 6400 6401 6c08  Z.d.d.l.Z.d.d.l.
-00000060: 5a08 6400 6401 6c09 5a0a 6400 6403 6c0b  Z.d.d.l.Z.d.d.l.
-00000070: 6d0c 5a0c 0100 6400 6404 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
-00000080: 0100 6400 6405 6c0f 6d0f 5a0f 0100 6400  ..d.d.l.m.Z...d.
-00000090: 6406 6c10 6d11 5a11 0100 6400 6407 6c12  d.l.m.Z...d.d.l.
-000000a0: 6d13 5a13 6d14 5a14 0100 6400 6408 6c15  m.Z.m.Z...d.d.l.
-000000b0: 6d16 5a16 0100 6400 6409 6c17 6d18 5a18  m.Z...d.d.l.m.Z.
-000000c0: 6d19 5a19 6d1a 5a1a 0100 4700 640a 640b  m.Z.m.Z...G.d.d.
-000000d0: 8400 640b 8302 5a1b 4700 640c 640d 8400  ..d...Z.G.d.d...
-000000e0: 640d 8302 5a1c 6401 5300 290e e900 0000  d...Z.d.S.).....
-000000f0: 004e 2901 da0b 6465 6661 756c 7464 6963  .N)...defaultdic
-00000100: 7429 01da 0e44 6947 7261 7068 4d61 7463  t)...DiGraphMatc
-00000110: 6865 7229 01da 1f70 7265 6369 7369 6f6e  her)...precision
-00000120: 5f72 6563 616c 6c5f 6673 636f 7265 5f73  _recall_fscore_s
-00000130: 7570 706f 7274 2901 da04 7471 646d 2901  upport)...tqdm).
-00000140: da0b 5465 7874 546f 346c 616e 6729 02da  ..TextTo4lang)..
-00000150: 1347 7261 7068 466f 726d 756c 614d 6174  .GraphFormulaMat
-00000160: 6368 6572 da1a 4772 6170 6846 6f72 6d75  cher..GraphFormu
-00000170: 6c61 5061 7474 6572 6e4d 6174 6368 6572  laPatternMatcher
-00000180: 2901 da14 4361 6368 6564 5374 616e 7a61  )...CachedStanza
-00000190: 5069 7065 6c69 6e65 2903 da13 6465 6661  Pipeline)...defa
-000001a0: 756c 745f 706e 5f74 6f5f 6772 6170 68da  ult_pn_to_graph.
-000001b0: 0b75 645f 746f 5f67 7261 7068 da0f 616d  .ud_to_graph..am
-000001c0: 725f 706e 5f74 6f5f 6772 6170 6863 0000  r_pn_to_graphc..
-000001d0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-000001e0: 0000 4000 0000 7330 0000 0065 005a 0164  ..@...s0...e.Z.d
-000001f0: 005a 0264 0b64 0264 0384 015a 0364 0464  .Z.d.d.d...Z.d.d
-00000200: 0584 005a 0464 0664 0784 005a 0564 0c64  ...Z.d.d...Z.d.d
-00000210: 0964 0a84 015a 0664 0153 0029 0dda 0e47  .d...Z.d.S.)...G
-00000220: 7261 7068 4578 7472 6163 746f 724e 6304  raphExtractorNc.
-00000230: 0000 0000 0000 0000 0000 0004 0000 0005  ................
-00000240: 0000 0043 0000 0073 6200 0000 7c01 6400  ...C...sb...|.d.
-00000250: 7500 721e 7400 6a01 a002 7400 6a01 a003  u.r.t.j...t.j...
-00000260: 7404 a101 6401 a102 7d01 7c02 6400 7500  t...d...}.|.d.u.
-00000270: 723a 7400 6a01 a002 7c01 7c03 9b00 6402  r:t.j...|.|...d.
-00000280: 9d02 a102 7d02 7c01 7c00 5f05 7c02 7c00  ....}.|.|._.|.|.
-00000290: 5f06 7c03 7c00 5f07 6400 7c00 5f08 6400  _.|.|._.d.|._.d.
-000002a0: 7c00 5f09 6400 7c00 5f0a 6400 5300 2903  |._.d.|._.d.S.).
-000002b0: 4eda 0563 6163 6865 7a0f 5f6e 6c70 5f63  N..cachez._nlp_c
-000002c0: 6163 6865 2e6a 736f 6e29 0bda 026f 73da  ache.json)...os.
-000002d0: 0470 6174 68da 046a 6f69 6eda 0764 6972  .path..join..dir
-000002e0: 6e61 6d65 da08 5f5f 6669 6c65 5f5f da09  name..__file__..
-000002f0: 6361 6368 655f 6469 72da 0863 6163 6865  cache_dir..cache
-00000300: 5f66 6eda 046c 616e 67da 036e 6c70 da07  _fn..lang..nlp..
-00000310: 6d61 7463 6865 72da 0861 6d72 5f73 746f  matcher..amr_sto
-00000320: 6729 04da 0473 656c 6672 1400 0000 7215  g)...selfr....r.
-00000330: 0000 0072 1600 0000 a900 721b 0000 00fa  ...r......r.....
-00000340: 402f 686f 6d65 2f61 6461 616d 6b6f 2f70  @/home/adaamko/p
-00000350: 726f 6a65 6374 732f 504f 5441 544f 2f78  rojects/POTATO/x
-00000360: 706f 7461 746f 2f67 7261 7068 5f65 7874  potato/graph_ext
-00000370: 7261 6374 6f72 2f65 7874 7261 6374 2e70  ractor/extract.p
-00000380: 79da 085f 5f69 6e69 745f 5f17 0000 0073  y..__init__....s
-00000390: 1400 0000 0001 0801 1601 0801 1401 0601  ................
-000003a0: 0601 0601 0601 0601 7a17 4772 6170 6845  ........z.GraphE
-000003b0: 7874 7261 6374 6f72 2e5f 5f69 6e69 745f  xtractor.__init_
-000003c0: 5f63 0100 0000 0000 0000 0000 0000 0200  _c..............
-000003d0: 0000 0200 0000 4300 0000 7320 0000 007c  ......C...s ...|
-000003e0: 006a 0064 006b 0272 1c64 0164 006c 017d  .j.d.k.r.d.d.l.}
-000003f0: 017c 01a0 02a1 007c 005f 0064 0053 00a9  .|.....|._.d.S..
-00000400: 024e 7201 0000 0029 0372 1900 0000 da06  .Nr....).r......
-00000410: 616d 726c 6962 5a0f 6c6f 6164 5f73 746f  amrlibZ.load_sto
-00000420: 675f 6d6f 6465 6c29 0272 1a00 0000 721f  g_model).r....r.
-00000430: 0000 0072 1b00 0000 721b 0000 0072 1c00  ...r....r....r..
-00000440: 0000 da08 696e 6974 5f61 6d72 2300 0000  ....init_amr#...
-00000450: 7306 0000 0000 010a 0108 027a 1747 7261  s..........z.Gra
-00000460: 7068 4578 7472 6163 746f 722e 696e 6974  phExtractor.init
-00000470: 5f61 6d72 6301 0000 0000 0000 0000 0000  _amrc...........
-00000480: 0002 0000 0004 0000 0043 0000 0073 4200  .........C...sB.
-00000490: 0000 7c00 6a00 6400 6b02 723e 7c00 6a01  ..|.j.d.k.r>|.j.
-000004a0: 6401 6b02 7224 7402 6a03 6402 6403 6404  d.k.r$t.j.d.d.d.
-000004b0: 8d02 7d01 6e0c 7402 a003 7c00 6a01 a101  ..}.n.t...|.j...
-000004c0: 7d01 7404 7c01 7c00 6a05 8302 7c00 5f00  }.t.|.|.j...|._.
-000004d0: 6400 5300 2905 4e5a 0665 6e5f 6269 6fda  d.S.).NZ.en_bio.
-000004e0: 0265 6e5a 0563 7261 6674 2901 da07 7061  .enZ.craft)...pa
-000004f0: 636b 6167 6529 0672 1700 0000 7216 0000  ckage).r....r...
-00000500: 00da 0673 7461 6e7a 61da 0850 6970 656c  ...stanza..Pipel
-00000510: 696e 6572 0900 0000 7215 0000 0029 0272  iner....r....).r
-00000520: 1a00 0000 7217 0000 0072 1b00 0000 721b  ....r....r....r.
-00000530: 0000 0072 1c00 0000 da08 696e 6974 5f6e  ...r......init_n
-00000540: 6c70 2900 0000 730a 0000 0000 010a 010a  lp)...s.........
-00000550: 0110 020c 017a 1747 7261 7068 4578 7472  .....z.GraphExtr
-00000560: 6163 746f 722e 696e 6974 5f6e 6c70 da08  actor.init_nlp..
-00000570: 666f 7572 6c61 6e67 6304 0000 0000 0000  fourlangc.......
-00000580: 0000 0000 000d 0000 0008 0000 0063 0000  .............c..
-00000590: 0073 5c01 0000 7c03 720a 7c03 7c00 5f00  .s\...|.r.|.|._.
-000005a0: 7c02 6401 6b02 72a2 7401 7c00 6a00 7c00  |.d.k.r.t.|.j.|.
-000005b0: 6a02 7c00 6a03 6402 8d03 8f6a 7d04 7404  j.|.j.d....j}.t.
-000005c0: 7c01 8301 4400 5d50 7d05 7405 7c04 7c05  |...D.]P}.t.|.|.
-000005d0: 6403 6404 8d02 8301 7d06 7c06 6405 1900  d.d.....}.|.d...
-000005e0: 7d07 7c06 6406 6400 8502 1900 4400 5d20  }.|.d.d.....D.] 
-000005f0: 7d08 7406 6407 7c05 9b00 6408 9d03 8301  }.t.d.|...d.....
-00000600: 8201 7407 a008 7c07 7c08 a102 7d07 7158  ..t...|.|...}.qX
-00000610: 7c07 5600 0100 7130 5700 6400 0400 0400  |.V...q0W.d.....
-00000620: 8303 0100 6e10 3100 7396 3000 0100 0100  ....n.1.s.0.....
-00000630: 0100 5900 0100 6eb6 7c02 6409 6b02 9001  ..Y...n.|.d.k...
-00000640: 7212 7c00 a009 a100 0100 7404 7c01 8301  r.|.......t.|...
-00000650: 4400 5d52 7d05 7c00 a00a 7c05 a101 7d09  D.]R}.|...|...}.
-00000660: 740b 7c09 6a0c 6405 1900 8301 5c02 7d07  t.|.j.d.....\.}.
-00000670: 7d0a 7c09 6a0c 6406 6400 8502 1900 4400  }.|.j.d.d.....D.
-00000680: 5d1c 7d0b 740b 7c0b 8301 5c02 7d08 7d0a  ].}.t.|...\.}.}.
-00000690: 7407 a008 7c07 7c08 a102 7d07 71ea 7c07  t...|.|...}.q.|.
-000006a0: 5600 0100 71bc 6e46 7c02 640a 6b02 9001  V...q.nF|.d.k...
-000006b0: 7258 7c00 a00d a100 0100 7404 7c01 8301  rX|.......t.|...
-000006c0: 4400 5d2a 7d05 7c00 6a0e a00f 7c05 6701  D.]*}.|.j...|.g.
-000006d0: a101 7d0c 7410 7c0c 6405 1900 8301 5c02  ..}.t.|.d.....\.
-000006e0: 7d07 7d0a 7c07 5600 0100 9001 712c 6400  }.}.|.V.....q,d.
-000006f0: 5300 290b 4e72 2600 0000 2903 7216 0000  S.).Nr&...).r...
-00000700: 005a 096e 6c70 5f63 6163 6865 7214 0000  .Z.nlp_cacher...
-00000710: 0046 2901 5a06 7373 706c 6974 7201 0000  .F).Z.ssplitr...
-00000720: 00e9 0100 0000 7a21 7365 6e74 656e 6365  ......z!sentence
-00000730: 2073 686f 756c 6420 6e6f 7420 6265 2073   should not be s
-00000740: 706c 6974 2075 703a 20fa 0121 da02 7564  plit up: ..!..ud
-00000750: 5a03 616d 7229 1172 1600 0000 7206 0000  Z.amr).r....r...
-00000760: 0072 1500 0000 7214 0000 0072 0500 0000  .r....r....r....
-00000770: da04 6c69 7374 da0a 5661 6c75 6545 7272  ..list..ValueErr
-00000780: 6f72 da02 6e78 da07 636f 6d70 6f73 6572  or..nx..composer
-00000790: 2500 0000 7217 0000 0072 0b00 0000 da09  %...r....r......
-000007a0: 7365 6e74 656e 6365 7372 2000 0000 7219  sentencesr ...r.
-000007b0: 0000 005a 0b70 6172 7365 5f73 656e 7473  ...Z.parse_sents
-000007c0: 720c 0000 0029 0d72 1a00 0000 da08 6974  r....).r......it
-000007d0: 6572 6162 6c65 da0a 6772 6170 685f 7479  erable..graph_ty
-000007e0: 7065 7216 0000 005a 0374 666c da03 7365  per....Z.tfl..se
-000007f0: 6e5a 0966 6c5f 6772 6170 6873 da01 67da  nZ.fl_graphs..g.
-00000800: 016e da03 646f 63da 015f 5a07 646f 635f  .n..doc.._Z.doc_
-00000810: 7365 6eda 0667 7261 7068 7372 1b00 0000  sen..graphsr....
-00000820: 721b 0000 0072 1c00 0000 da0e 7061 7273  r....r......pars
-00000830: 655f 6974 6572 6162 6c65 3100 0000 733a  e_iterable1...s:
-00000840: 0000 0000 0104 0106 0108 0102 010c ff06  ................
-00000850: 0202 010c 0110 0108 0110 0110 010e 0128  ...............(
-00000860: 020a 0108 010c 010a 0112 0112 010c 010e  ................
-00000870: 010a 020a 0108 010c 010e 0110 017a 1d47  .............z.G
-00000880: 7261 7068 4578 7472 6163 746f 722e 7061  raphExtractor.pa
-00000890: 7273 655f 6974 6572 6162 6c65 2903 4e4e  rse_iterable).NN
-000008a0: 4e29 0272 2600 0000 4e29 07da 085f 5f6e  N).r&...N)...__n
-000008b0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-000008c0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-000008d0: 1d00 0000 7220 0000 0072 2500 0000 7237  ....r ...r%...r7
-000008e0: 0000 0072 1b00 0000 721b 0000 0072 1b00  ...r....r....r..
-000008f0: 0000 721c 0000 0072 0d00 0000 1600 0000  ..r....r........
-00000900: 7308 0000 0008 010a 0c08 0608 0872 0d00  s............r..
-00000910: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000920: 0000 0004 0000 0040 0000 0073 8200 0000  .......@...s....
-00000930: 6500 5a01 6400 5a02 641c 6403 6404 8401  e.Z.d.Z.d.d.d...
-00000940: 5a03 6405 6406 8400 5a04 6407 6408 8400  Z.d.d...Z.d.d...
-00000950: 5a05 6402 6402 6506 6402 6604 6409 640a  Z.d.d.e.d.f.d.d.
-00000960: 8401 5a07 641d 640b 640c 8401 5a08 640d  ..Z.d.d.d...Z.d.
-00000970: 640e 8400 5a09 640f 6410 8400 5a0a 6411  d...Z.d.d...Z.d.
-00000980: 6412 8400 5a0b 641e 6413 6414 8401 5a0c  d...Z.d.d.d...Z.
-00000990: 6415 6416 8400 5a0d 6417 6418 8400 5a0e  d.d...Z.d.d...Z.
-000009a0: 6401 6506 6602 6419 641a 8401 5a0f 641b  d.e.f.d.d...Z.d.
-000009b0: 5300 291f da10 4665 6174 7572 6545 7661  S.)...FeatureEva
-000009c0: 6c75 6174 6f72 7229 0000 0046 6303 0000  luatorr)...Fc...
-000009d0: 0000 0000 0000 0000 0003 0000 0002 0000  ................
-000009e0: 0043 0000 0073 1000 0000 7c01 7c00 5f00  .C...s....|.|._.
-000009f0: 7c02 7c00 5f01 6400 5300 2901 4e29 02da  |.|._.d.S.).N)..
-00000a00: 0c67 7261 7068 5f66 6f72 6d61 74da 0e63  .graph_format..c
-00000a10: 6173 655f 7365 6e73 6974 6976 6529 0372  ase_sensitive).r
-00000a20: 1a00 0000 723c 0000 0072 3d00 0000 721b  ....r<...r=...r.
-00000a30: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
-00000a40: 0000 5300 0000 7304 0000 0000 0106 017a  ..S...s........z
-00000a50: 1946 6561 7475 7265 4576 616c 7561 746f  .FeatureEvaluato
-00000a60: 722e 5f5f 696e 6974 5f5f 6303 0000 0000  r.__init__c.....
-00000a70: 0000 0000 0000 001b 0000 0006 0000 0063  ...............c
-00000a80: 0000 0073 9201 0000 6900 7d03 7400 7c02  ...s....i.}.t.|.
-00000a90: 8301 4400 5dbe 5c02 7d04 7d05 7401 7c05  ..D.].\.}.}.t.|.
-00000aa0: 8301 6401 6b02 732e 4a00 6402 7c05 9b00  ..d.k.s.J.d.|...
-00000ab0: 9d02 8301 8201 7c05 6403 1900 7d06 7c05  ......|.d...}.|.
-00000ac0: 6404 1900 7d07 7c06 4400 5d32 7d08 7402  d...}.|.D.]2}.t.
-00000ad0: a003 7c08 a101 7d09 7c09 6a04 6403 1900  ..|...}.|.j.d...
-00000ae0: 6403 1900 7d0a 7c0a 6405 6b02 7342 4a00  d...}.|.d.k.sBJ.
-00000af0: 6406 7c0a 9b00 9d02 8301 8201 7142 7c07  d.|.........qB|.
-00000b00: 4400 5d32 7d0b 7402 a003 7c0b a101 7d09  D.]2}.t...|...}.
-00000b10: 7c09 6a04 6403 1900 6403 1900 7d0a 7c0a  |.j.d...d...}.|.
-00000b20: 6405 6b02 737a 4a00 6406 7c0a 9b00 9d02  d.k.szJ.d.|.....
-00000b30: 8301 8201 717a 7c05 6407 1900 7c03 7c04  ....qz|.d...|.|.
-00000b40: 3c00 7c05 6400 6407 8502 1900 7c02 7c04  <.|.d.d.....|.|.
-00000b50: 3c00 710c 7405 7c02 7406 7c00 6a07 6408  <.q.t.|.t.|.j.d.
-00000b60: 8d03 7d0c 7c0c 6a08 7c01 6409 640a 8d02  ..}.|.j.|.d.d...
-00000b70: 7d0d 7c0d 4400 5d9e 5c03 7d0e 7d04 7d0f  }.|.D.].\.}.}.}.
-00000b80: 640b 7c0e 6901 7d10 7c03 7c04 1900 7d11  d.|.i.}.|.|...}.
-00000b90: 7400 7c11 8301 4400 5d7a 5c02 7d12 7d13  t.|...D.]z\.}.}.
-00000ba0: 7c0f 7c12 1900 7d14 6900 7d15 7c14 6a09  |.|...}.i.}.|.j.
-00000bb0: 6409 640c 8d01 4400 5d30 5c02 7d16 7d17  d.d...D.]0\.}.}.
-00000bc0: 7c17 640d 1900 7d18 640e 7c17 7600 9001  |.d...}.d.|.v...
-00000bd0: 7252 7c17 640e 1900 6e06 7c17 640f 1900  rR|.d...n.|.d...
-00000be0: 7c15 7c18 3c00 9001 7130 7c13 a00a a100  |.|.<...q0|.....
-00000bf0: 4400 5d16 5c02 7d19 7d1a 7c15 7c1a 1900  D.].\.}.}.|.|...
-00000c00: 7c10 7c19 3c00 9001 716a 7c10 5600 0100  |.|.<...qj|.V...
-00000c10: 9001 7110 71ee 6400 5300 2910 4ee9 0400  ..q.q.d.S.).N...
-00000c20: 0000 7a2a 4665 6174 7572 6520 6d75 7374  ..z*Feature must
-00000c30: 2062 6520 6120 342d 7475 706c 6520 666f   be a 4-tuple fo
-00000c40: 7220 4f70 656e 4945 2c20 6e6f 7420 7201  r OpenIE, not r.
-00000c50: 0000 0072 2700 0000 5a03 755f 307a 1f54  ...r'...Z.u_0z.T
-00000c60: 6865 2049 4473 206d 7573 7420 7374 6172  he IDs must star
-00000c70: 7420 6672 6f6d 2030 2c20 6e6f 7420 e903  t from 0, not ..
-00000c80: 0000 00a9 02da 0963 6f6e 7665 7274 6572  .......converter
-00000c90: 723d 0000 0054 a901 da10 7265 7475 726e  r=...T....return
-00000ca0: 5f73 7562 6772 6170 6873 da08 7265 6c61  _subgraphs..rela
-00000cb0: 7469 6f6e a901 da04 6461 7461 da07 6d61  tion....data..ma
-00000cc0: 7070 696e 67da 0665 6e74 6974 79da 046e  pping..entity..n
-00000cd0: 616d 6529 0bda 0965 6e75 6d65 7261 7465  ame)...enumerate
-00000ce0: da03 6c65 6eda 0270 6eda 0664 6563 6f64  ..len..pn..decod
-00000cf0: 65da 0774 7269 706c 6573 7207 0000 0072  e..triplesr....r
-00000d00: 0a00 0000 723d 0000 00da 056d 6174 6368  ....r=.....match
-00000d10: da05 6e6f 6465 73da 0569 7465 6d73 291b  ..nodes..items).
-00000d20: 721a 0000 00da 0567 7261 7068 da08 6665  r......graph..fe
-00000d30: 6174 7572 6573 5a17 6665 6174 7572 655f  aturesZ.feature_
-00000d40: 746f 5f6d 6172 6b65 645f 6e6f 6465 73da  to_marked_nodes.
-00000d50: 0169 da07 6665 6174 7572 655a 1170 6f73  .i..featureZ.pos
-00000d60: 6974 6976 655f 6665 6174 7572 6573 5a11  itive_featuresZ.
-00000d70: 6e65 6761 7469 7665 5f66 6561 7475 7265  negative_feature
-00000d80: 73da 0870 6f73 6974 6976 65da 0170 da05  s..positive..p..
-00000d90: 6669 7273 74da 086e 6567 6174 6976 6572  first..negativer
-00000da0: 1800 0000 da05 6665 6174 73da 036b 6579  ......feats..key
-00000db0: da09 7375 6267 7261 7068 73da 0774 7269  ..subgraphs..tri
-00000dc0: 706c 6574 da0c 6d61 726b 6564 5f6e 6f64  plet..marked_nod
-00000dd0: 6573 da01 6ada 046e 6f64 65da 0873 7562  es..j..node..sub
-00000de0: 6772 6170 685a 0c6e 6f64 655f 746f 5f6e  graphZ.node_to_n
-00000df0: 6f64 65da 0269 64da 0a67 7261 7068 5f6e  ode..id..graph_n
-00000e00: 6f64 6572 4700 0000 da01 6bda 0176 721b  oderG.....k..vr.
-00000e10: 0000 0072 1b00 0000 721c 0000 00da 0861  ...r....r......a
-00000e20: 6e6e 6f74 6174 6559 0000 0073 4a00 0000  nnotateY...sJ...
-00000e30: 0001 0402 1002 0aff 0402 08fe 0404 0801  ................
-00000e40: 0802 0801 0a01 0e01 1802 0801 0a01 0e01  ................
-00000e50: 1802 0c01 1202 0201 08ff 0603 0e02 0e01  ................
-00000e60: 0801 0801 1001 0802 0401 1401 0803 06ff  ................
-00000e70: 0c02 06fd 0a06 1001 1002 7a19 4665 6174  ..........z.Feat
-00000e80: 7572 6545 7661 6c75 6174 6f72 2e61 6e6e  ureEvaluator.ann
-00000e90: 6f74 6174 6563 0300 0000 0000 0000 0000  otatec..........
-00000ea0: 0000 0800 0000 0500 0000 4300 0000 734c  ..........C...sL
-00000eb0: 0000 007c 016a 00a0 01a1 007d 0367 007d  ...|.j.....}.g.}
-00000ec0: 047c 0344 005d 1e7d 057c 00a0 027c 057c  .|.D.].}.|...|.|
-00000ed0: 02a1 027d 067c 04a0 0374 047c 0683 01a1  ...}.|...t.|....
-00000ee0: 0101 0071 127c 016a 05a0 01a1 007c 0464  ...q.|.j.....|.d
-00000ef0: 019c 027d 0774 06a0 077c 07a1 0153 0029  ...}.t...|...S.)
-00000f00: 024e 2902 da08 5365 6e74 656e 6365 5a08  .N)...SentenceZ.
-00000f10: 5472 6970 6c65 7473 2908 7252 0000 00da  Triplets).rR....
-00000f20: 0674 6f6c 6973 7472 6600 0000 da06 6170  .tolistrf.....ap
-00000f30: 7065 6e64 722a 0000 00da 0474 6578 74da  pendr*.....text.
-00000f40: 0270 64da 0944 6174 6146 7261 6d65 2908  .pd..DataFrame).
-00000f50: 721a 0000 00da 0764 6174 6173 6574 7253  r......datasetrS
-00000f60: 0000 0072 3600 0000 da08 7472 6970 6c65  ...r6.....triple
-00000f70: 7473 7252 0000 00da 0972 656c 6174 696f  tsrR.....relatio
-00000f80: 6e73 da01 6472 1b00 0000 721b 0000 0072  ns..dr....r....r
-00000f90: 1c00 0000 da12 616e 6e6f 7461 7465 5f64  ......annotate_d
-00000fa0: 6174 6166 7261 6d65 8a00 0000 7312 0000  ataframe....s...
-00000fb0: 0000 010a 0204 0108 010c 0110 0208 0102  ................
-00000fc0: fe06 057a 2346 6561 7475 7265 4576 616c  ...z#FeatureEval
-00000fd0: 7561 746f 722e 616e 6e6f 7461 7465 5f64  uator.annotate_d
-00000fe0: 6174 6166 7261 6d65 6307 0000 0000 0000  ataframec.......
-00000ff0: 0000 0000 0011 0000 0009 0000 0043 0000  .............C..
-00001000: 0073 a400 0000 7c01 6a00 a001 a100 7d07  .s....|.j.....}.
-00001010: 6700 7d08 6700 7d09 6700 7d0a 7c05 7c02  g.}.g.}.g.}.|.|.
-00001020: 7402 7c00 6a03 6401 8d03 7d0b 7404 7405  t.|.j.d...}.t.t.
-00001030: 7c07 8301 8301 4400 5d44 5c02 7d0c 7d0d  |.....D.]D\.}.}.
-00001040: 7c0b 6a06 7c0d 6402 6403 8d02 7d0e 7c03  |.j.|.d.d...}.|.
-00001050: 7264 7c00 6a07 7c0e 7c02 7c08 7c09 7c0a  rd|.j.|.|.|.|.|.
-00001060: 7c06 6404 8d06 0100 7132 7c00 a008 7c0e  |.d.....q2|...|.
-00001070: 7c02 7c08 7c09 7c0a a105 0100 7132 7c01  |.|.|.|.....q2|.
-00001080: 6a09 a001 a100 7c09 7c08 6405 9c03 7d0f  j.....|.|.d...}.
-00001090: 7c04 7296 7c0a 7c0f 6406 3c00 740a a00b  |.r.|.|.d.<.t...
-000010a0: 7c0f a101 7d10 7c10 5300 2907 4e72 4000  |...}.|.S.).Nr@.
-000010b0: 0000 5472 4200 0000 2901 da11 616c 6c6f  ..TrB...)...allo
-000010c0: 775f 6d75 6c74 695f 6772 6170 6829 0372  w_multi_graph).r
-000010d0: 6700 0000 7a0f 5072 6564 6963 7465 6420  g...z.Predicted 
-000010e0: 6c61 6265 6c7a 0c4d 6174 6368 6564 2072  labelz.Matched r
-000010f0: 756c 657a 104d 6174 6368 6564 2073 7562  ulez.Matched sub
-00001100: 6772 6170 6829 0c72 5200 0000 7268 0000  graph).rR...rh..
-00001110: 0072 0a00 0000 723d 0000 0072 0500 0000  .r....r=...r....
-00001120: 724a 0000 0072 4f00 0000 da0b 6d61 7463  rJ...rO.....matc
-00001130: 685f 6d75 6c74 69da 0f6d 6174 6368 5f6e  h_multi..match_n
-00001140: 6f74 5f6d 756c 7469 726a 0000 0072 6b00  ot_multirj...rk.
-00001150: 0000 726c 0000 0029 1172 1a00 0000 726d  ..rl...).r....rm
-00001160: 0000 0072 5300 0000 da05 6d75 6c74 6972  ...rS.....multir
-00001170: 4300 0000 da0d 6772 6170 685f 6d61 7463  C.....graph_matc
-00001180: 6865 7272 7200 0000 7236 0000 00da 076d  herrr...r6.....m
-00001190: 6174 6368 6573 da09 7072 6564 6963 7465  atches..predicte
-000011a0: 64da 0e6d 6174 6368 6564 5f67 7261 7068  d..matched_graph
-000011b0: 7372 1800 0000 7254 0000 0072 3200 0000  sr....rT...r2...
-000011c0: 725a 0000 0072 7000 0000 da02 6466 721b  rZ...rp.....dfr.
-000011d0: 0000 0072 1b00 0000 721c 0000 00da 0e6d  ...r....r......m
-000011e0: 6174 6368 5f66 6561 7475 7265 7398 0000  atch_features...
-000011f0: 0073 3a00 0000 0009 0a02 0401 0401 0402  .s:.............
-00001200: 0201 08ff 0604 1401 0e01 0401 0401 0201  ................
-00001210: 0201 0201 0201 0201 02fa 0809 0401 0aff  ................
-00001220: 0605 0801 0201 02fd 0605 0401 0802 0a01  ................
-00001230: 7a1f 4665 6174 7572 6545 7661 6c75 6174  z.FeatureEvaluat
-00001240: 6f72 2e6d 6174 6368 5f66 6561 7475 7265  or.match_feature
-00001250: 7363 0700 0000 0000 0000 0000 0000 0d00  sc..............
-00001260: 0000 0500 0000 4300 0000 7390 0000 0067  ......C...s....g
-00001270: 007d 0767 007d 0867 007d 097c 0144 005d  .}.g.}.g.}.|.D.]
-00001280: 385c 037d 0a7d 0b7d 0c7c 0a7c 0776 0173  8\.}.}.}.|.|.v.s
-00001290: 267c 0672 107c 08a0 007c 027c 0b19 00a1  &|.r.|...|.|....
-000012a0: 0101 007c 09a0 007c 0ca1 0101 007c 07a0  ...|...|.....|..
-000012b0: 007c 0aa1 0101 0071 107c 0773 6e7c 03a0  .|.....q.|.sn|..
-000012c0: 0064 01a1 0101 007c 04a0 0064 01a1 0101  .d.....|...d....
-000012d0: 007c 05a0 0064 01a1 0101 006e 1e7c 03a0  .|...d.....n.|..
-000012e0: 007c 08a1 0101 007c 04a0 007c 07a1 0101  .|.....|...|....
-000012f0: 007c 05a0 007c 09a1 0101 0064 0053 00a9  .|...|.....d.S..
-00001300: 024e da00 a901 7269 0000 0029 0d72 1a00  .N....ri...).r..
-00001310: 0000 725a 0000 0072 5300 0000 7277 0000  ..rZ...rS...rw..
-00001320: 0072 7800 0000 7279 0000 0072 7200 0000  .rx...ry...rr...
-00001330: da04 6b65 7973 5a0d 6d61 7463 6865 645f  ..keysZ.matched_
-00001340: 7275 6c65 735a 116d 6174 6368 6564 5f73  rulesZ.matched_s
-00001350: 7562 6772 6170 6873 725b 0000 0072 5500  ubgraphsr[...rU.
-00001360: 0000 7236 0000 0072 1b00 0000 721b 0000  ..r6...r....r...
-00001370: 0072 1c00 0000 7273 0000 00c6 0000 0073  .r....rs.......s
-00001380: 1e00 0000 0009 0401 0401 0401 0e01 0c01  ................
-00001390: 0e01 0a01 0c01 0401 0a01 0a01 0c02 0a01  ................
-000013a0: 0a01 7a1c 4665 6174 7572 6545 7661 6c75  ..z.FeatureEvalu
-000013b0: 6174 6f72 2e6d 6174 6368 5f6d 756c 7469  ator.match_multi
-000013c0: 6306 0000 0000 0000 0000 0000 0009 0000  c...............
-000013d0: 0005 0000 0043 0000 0073 5800 0000 7c01  .....C...sX...|.
-000013e0: 4400 5d30 5c03 7d06 7d07 7d08 7c03 a000  D.]0\.}.}.}.|...
-000013f0: 7c02 7c07 1900 a101 0100 7c04 a000 7c06  |.|.......|...|.
-00001400: a101 0100 7c05 a000 7c08 a101 0100 0100  ....|...|.......
-00001410: 7154 7104 7c03 a000 6401 a101 0100 7c05  qTq.|...d.....|.
-00001420: a000 6401 a101 0100 7c04 a000 6401 a101  ..d.....|...d...
-00001430: 0100 6400 5300 727c 0000 0072 7e00 0000  ..d.S.r|...r~...
-00001440: 2909 721a 0000 0072 5a00 0000 7253 0000  ).r....rZ...rS..
-00001450: 0072 7700 0000 7278 0000 0072 7900 0000  .rw...rx...ry...
-00001460: 725b 0000 0072 5500 0000 7236 0000 0072  r[...rU...r6...r
-00001470: 1b00 0000 721b 0000 0072 1c00 0000 7274  ....r....r....rt
-00001480: 0000 00e0 0000 0073 1000 0000 0001 0e01  .......s........
-00001490: 0e01 0a01 0a01 0602 0a01 0a01 7a20 4665  ............z Fe
-000014a0: 6174 7572 6545 7661 6c75 6174 6f72 2e6d  atureEvaluator.m
-000014b0: 6174 6368 5f6e 6f74 5f6d 756c 7469 6303  atch_not_multic.
-000014c0: 0000 0000 0000 0000 0000 0004 0000 0003  ................
-000014d0: 0000 0003 0000 0073 2c00 0000 7c02 6401  .......s,...|.d.
-000014e0: 6901 8900 7c01 a000 a100 7d03 8700 6601  i...|.....}...f.
-000014f0: 6402 6403 8408 7c01 6a01 4400 8301 7c03  d.d...|.j.D...|.
-00001500: 6404 3c00 7c03 5300 2905 4e72 2700 0000  d.<.|.S.).Nr'...
-00001510: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001520: 0004 0000 0013 0000 0073 2000 0000 6700  .........s ...g.
-00001530: 7c00 5d18 7d01 7c01 8800 7600 7218 8800  |.].}.|...v.r...
-00001540: 7c01 1900 6e02 6400 9102 7104 5300 2901  |...n.d...q.S.).
-00001550: 7201 0000 0072 1b00 0000 2902 da02 2e30  r....r....)....0
-00001560: da04 6974 656d a901 da06 6d61 7070 6572  ..item....mapper
-00001570: 721b 0000 0072 1c00 0000 da0a 3c6c 6973  r....r......<lis
-00001580: 7463 6f6d 703e ef00 0000 7302 0000 0006  tcomp>....s.....
-00001590: 017a 3446 6561 7475 7265 4576 616c 7561  .z4FeatureEvalua
-000015a0: 746f 722e 6f6e 655f 7665 7273 7573 5f72  tor.one_versus_r
-000015b0: 6573 742e 3c6c 6f63 616c 733e 2e3c 6c69  est.<locals>.<li
-000015c0: 7374 636f 6d70 3eda 0f6f 6e65 5f76 6572  stcomp>..one_ver
-000015d0: 7375 735f 7265 7374 2902 da04 636f 7079  sus_rest)...copy
-000015e0: da05 6c61 6265 6c29 0472 1a00 0000 727a  ..label).r....rz
-000015f0: 0000 0072 4800 0000 5a12 6f6e 655f 7665  ...rH...Z.one_ve
-00001600: 7273 7573 5f72 6573 745f 6466 721b 0000  rsus_rest_dfr...
-00001610: 0072 8200 0000 721c 0000 0072 8500 0000  .r....r....r....
-00001620: eb00 0000 730c 0000 0000 0108 0208 010a  ....s...........
-00001630: 0104 ff0a 047a 2046 6561 7475 7265 4576  .....z FeatureEv
-00001640: 616c 7561 746f 722e 6f6e 655f 7665 7273  aluator.one_vers
-00001650: 7573 5f72 6573 7463 0500 0000 0000 0000  us_restc........
-00001660: 0000 0000 0b00 0000 0c00 0000 0300 0000  ................
-00001670: 7398 0000 007c 037d 057c 00a0 007c 0188  s....|.}.|...|..
-00001680: 017c 05a1 035c 0289 007d 0667 007d 0774  .|...\...}.g.}.t
-00001690: 0188 0183 0144 005d 585c 027d 087d 097c  .....D.]X\.}.}.|
-000016a0: 07a0 027c 0988 006a 037c 0819 006a 0488  ...|...j.|...j..
-000016b0: 006a 037c 0819 006a 0588 006a 037c 0819  .j.|...j...j.|..
-000016c0: 006a 0688 006a 037c 0819 006a 0774 0888  .j...j.|...j.t..
-000016d0: 006a 037c 0819 006a 0983 0174 0888 006a  .j.|...j...t...j
-000016e0: 037c 0819 006a 0a83 0166 07a1 0101 0071  .|...j...f.....q
-000016f0: 2287 0087 0166 0264 0164 0284 087d 0a74  "....f.d.d...}.t
-00001700: 0b7c 077c 0a64 0364 048d 0353 0029 054e  .|.|.d.d...S.).N
-00001710: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001720: 0006 0000 0013 0000 0073 1a00 0000 7400  .........s....t.
-00001730: 8800 6a01 8801 a002 7c00 6401 1900 a101  ..j.....|.d.....
-00001740: 1900 6a03 8301 5300 721e 0000 0029 0472  ..j...S.r....).r
-00001750: 4b00 0000 da04 696c 6f63 da05 696e 6465  K.....iloc..inde
-00001760: 78da 1454 7275 655f 706f 7369 7469 7665  x..True_positive
-00001770: 5f67 7261 7068 7329 0172 5500 0000 a902  _graphs).rU.....
-00001780: 727a 0000 0072 5300 0000 721b 0000 0072  rz...rS...r....r
-00001790: 1c00 0000 da04 7261 6e6b 0d01 0000 7302  ......rank....s.
-000017a0: 0000 0000 017a 2c46 6561 7475 7265 4576  .....z,FeatureEv
-000017b0: 616c 7561 746f 722e 7261 6e6b 5f66 6561  aluator.rank_fea
-000017c0: 7475 7265 732e 3c6c 6f63 616c 733e 2e72  tures.<locals>.r
-000017d0: 616e 6b54 2902 725b 0000 00da 0772 6576  ankT).r[.....rev
-000017e0: 6572 7365 290c da10 6576 616c 7561 7465  erse)...evaluate
-000017f0: 5f66 6561 7475 7265 724a 0000 0072 6900  _featurerJ...ri.
-00001800: 0000 7288 0000 00da 0950 7265 6369 7369  ..r......Precisi
-00001810: 6f6e da06 5265 6361 6c6c da06 4673 636f  on..Recall..Fsco
-00001820: 7265 da07 5375 7070 6f72 7472 4b00 0000  re..SupportrK...
-00001830: da12 5472 7565 5f70 6f73 6974 6976 655f  ..True_positive_
-00001840: 7365 6e73 da13 4661 6c73 655f 706f 7369  sens..False_posi
-00001850: 7469 7665 5f73 656e 73da 0673 6f72 7465  tive_sens..sorte
-00001860: 6429 0b72 1a00 0000 da02 636c 7253 0000  d).r......clrS..
-00001870: 005a 096f 7269 675f 6461 7461 da0f 6661  .Z.orig_data..fa
-00001880: 6c73 655f 6e65 6761 7469 7665 735a 0b73  lse_negativesZ.s
-00001890: 7562 7365 745f 6461 7461 da08 6163 6375  ubset_data..accu
-000018a0: 7261 6379 5a0d 6665 6174 7572 6573 5f73  racyZ.features_s
-000018b0: 7461 7472 5400 0000 7255 0000 0072 8c00  tatrT...rU...r..
-000018c0: 0000 721b 0000 0072 8b00 0000 721c 0000  ..r....r....r...
-000018d0: 00da 0d72 616e 6b5f 6665 6174 7572 6573  ...rank_features
-000018e0: f500 0000 7320 0000 0000 0604 0112 0204  ....s ..........
-000018f0: 0210 0104 0202 010a 010a 010a 010a 010e  ................
-00001900: 010e f902 ff06 0c0e 037a 1e46 6561 7475  .........z.Featu
-00001910: 7265 4576 616c 7561 746f 722e 7261 6e6b  reEvaluator.rank
-00001920: 5f66 6561 7475 7265 7363 0500 0000 0000  _featuresc......
-00001930: 0000 0000 0000 2100 0000 0e00 0000 4300  ......!.......C.
-00001940: 0000 73c0 0200 0074 007c 0267 0167 0067  ..s....t.|.g.g.g
-00001950: 0067 0367 0174 017c 006a 0264 018d 037d  .g.g.t.|.j.d...}
-00001960: 057c 056a 0364 0219 0064 0219 007d 0674  .|.j.d...d...}.t
-00001970: 047c 0664 0219 0074 0583 0272 7074 067c  .|.d...t...rpt.|
-00001980: 0664 0219 0064 0319 0083 0164 046b 0272  .d...d.....d.k.r
-00001990: 5c7c 0664 0219 0064 0319 005c 027d 077d  \|.d...d...\.}.}
-000019a0: 0871 7e7c 0664 0219 0064 0319 005c 037d  .q~|.d...d...\.}
-000019b0: 097d 077d 086e 0e7c 0664 0219 0064 0002  .}.}.n.|.d...d..
-000019c0: 007d 077d 087c 036a 07a0 08a1 007d 0a7c  .}.}.|.j.....}.|
-000019d0: 00a0 097c 037c 01a1 026a 09a0 08a1 007d  ...|.|...j.....}
-000019e0: 0b64 057d 0c67 007d 0d74 0a7c 0c64 0683  .d.}.g.}.t.|.d..
-000019f0: 0290 018f f67d 0e74 0b7c 0a83 0144 0090  .....}.t.|...D..
-00001a00: 015d da5c 027d 0f7d 1064 0764 0884 007c  .].\.}.}.d.d...|
-00001a10: 056a 0c7c 1064 0964 0a8d 0244 0083 017d  .j.|.d.d...D...}
-00001a20: 117c 1144 0090 015d b25c 027d 127d 137c  .|.D...].\.}.}.|
-00001a30: 1344 0090 015d a27d 1467 007d 157c 146a  .D...].}.g.}.|.j
-00001a40: 0d64 0964 0b8d 0144 005d 865c 027d 167d  .d.d...D.].\.}.}
-00001a50: 177c 1590 0173 027c 1764 0c19 007d 187c  .|...s.|.d...}.|
-00001a60: 1764 0d19 007c 076a 0d76 0090 0172 4a7c  .d...|.j.v...rJ|
-00001a70: 076a 0d7c 1764 0d19 0019 0064 0c19 0064  .j.|.d.....d...d
-00001a80: 0e6b 0290 0172 4a7c 15a0 0e7c 18a1 0101  .k...rJ|...|....
-00001a90: 007c 0864 0075 0190 0172 027c 1764 0d19  .|.d.u...r.|.d..
-00001aa0: 007c 086a 0d76 0090 0172 027c 086a 0d7c  .|.j.v...r.|.j.|
-00001ab0: 1764 0d19 0019 0064 0c19 0064 0e6b 0290  .d.....d...d.k..
-00001ac0: 0172 027c 15a0 0e7c 18a1 0101 0090 0171  .r.|...|.......q
-00001ad0: 027c 1590 0273 3a64 0f64 1084 007c 146a  .|...s:d.d...|.j
-00001ae0: 0f64 0964 0b8d 0144 0083 017d 197c 076a  .d.d...D...}.|.j
-00001af0: 0f64 0964 0b8d 0144 005d 3c5c 037d 1a7d  .d.d...D.]<\.}.}
-00001b00: 1b7d 1c7c 1c64 1119 0064 0e6b 0290 0172  .}.|.d...d.k...r
-00001b10: b27c 10a0 107c 197c 1a19 007c 197c 1b19  .|...|.|...|.|..
-00001b20: 00a1 0264 1119 007d 1d7c 15a0 0e7c 1da1  ...d...}.|...|..
-00001b30: 0101 0090 0171 b27c 086a 0f64 0964 0b8d  .....q.|.j.d.d..
-00001b40: 0144 005d 3c5c 037d 1a7d 1b7d 1c7c 1c64  .D.]<\.}.}.}.|.d
-00001b50: 1119 0064 0e6b 0290 0172 fc7c 10a0 107c  ...d.k...r.|...|
-00001b60: 197c 1a19 007c 197c 1b19 00a1 0264 1119  .|...|.|.....d..
-00001b70: 007d 1d7c 15a0 0e7c 1da1 0101 0090 0171  .}.|...|.......q
-00001b80: fc64 12a0 117c 15a1 017d 1e7c 0b7c 0f19  .d...|...}.|.|..
-00001b90: 007d 1f7c 036a 127c 0f19 006a 137d 207c  .}.|.j.|...j.} |
-00001ba0: 0ea0 147c 029b 0064 137c 1e9b 0064 137c  ...|...d.|...d.|
-00001bb0: 209b 0064 137c 1f9b 0064 149d 08a1 0101   ..d.|...d......
-00001bc0: 007c 0da0 0e7c 027c 1e7c 2074 157c 1f83  .|...|.|.| t.|..
-00001bd0: 0166 04a1 0101 0071 ec71 de71 b857 0064  .f.....q.q.q.W.d
-00001be0: 0004 0004 0083 0301 006e 1231 0090 0273  .........n.1...s
-00001bf0: ac30 0001 0001 0001 0059 0001 007c 00a0  .0.......Y...|..
-00001c00: 167c 0da1 0153 0029 154e 2901 723d 0000  .|...S.).N).r=..
-00001c10: 0072 0100 0000 7227 0000 00e9 0200 0000  .r....r'........
-00001c20: 7a14 7472 6169 6e65 645f 6665 6174 7572  z.trained_featur
-00001c30: 6573 2e74 7376 7a02 772b 6301 0000 0000  es.tsvz.w+c.....
-00001c40: 0000 0000 0000 0004 0000 0005 0000 0053  ...............S
-00001c50: 0000 0073 1a00 0000 6700 7c00 5d12 5c03  ...s....g.|.].\.
-00001c60: 7d01 7d02 7d03 7c02 7c03 6602 9102 7104  }.}.}.|.|.f...q.
-00001c70: 5300 721b 0000 0072 1b00 0000 2904 7280  S.r....r....).r.
-00001c80: 0000 0072 5b00 0000 7254 0000 0072 6100  ...r[...rT...ra.
-00001c90: 0000 721b 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-00001ca0: 0072 8400 0000 2301 0000 f300 0000 007a  .r....#........z
-00001cb0: 3246 6561 7475 7265 4576 616c 7561 746f  2FeatureEvaluato
-00001cc0: 722e 7472 6169 6e5f 6665 6174 7572 652e  r.train_feature.
-00001cd0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00001ce0: 6d70 3e54 7242 0000 0072 4500 0000 7249  mp>TrB...rE...rI
-00001cf0: 0000 0072 4700 0000 fa02 2e2a 6301 0000  ...rG......*c...
-00001d00: 0000 0000 0000 0000 0004 0000 0005 0000  ................
-00001d10: 0053 0000 0073 1800 0000 6900 7c00 5d10  .S...s....i.|.].
-00001d20: 5c03 7d01 7d02 7d03 7c02 7c01 9302 7104  \.}.}.}.|.|...q.
-00001d30: 5300 721b 0000 0072 1b00 0000 2904 7280  S.r....r....).r.
-00001d40: 0000 00da 0175 7265 0000 0072 3500 0000  .....ure...r5...
-00001d50: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
-00001d60: 0a3c 6469 6374 636f 6d70 3e2f 0100 0072  .<dictcomp>/...r
-00001d70: 9b00 0000 7a32 4665 6174 7572 6545 7661  ....z2FeatureEva
-00001d80: 6c75 6174 6f72 2e74 7261 696e 5f66 6561  luator.train_fea
-00001d90: 7475 7265 2e3c 6c6f 6361 6c73 3e2e 3c64  ture.<locals>.<d
-00001da0: 6963 7463 6f6d 703e da05 636f 6c6f 72fa  ictcomp>..color.
-00001db0: 012c fa01 09da 010a 2917 7208 0000 0072  .,......).r....r
-00001dc0: 0a00 0000 723d 0000 005a 0570 6174 7473  ....r=...Z.patts
-00001dd0: da0a 6973 696e 7374 616e 6365 da05 7475  ..isinstance..tu
-00001de0: 706c 6572 4b00 0000 7252 0000 0072 6800  plerK...rR...rh.
-00001df0: 0000 7285 0000 00da 046f 7065 6e72 4a00  ..r......openrJ.
-00001e00: 0000 724f 0000 0072 5000 0000 7269 0000  ..rO...rP...ri..
-00001e10: 00da 0565 6467 6573 da0d 6765 745f 6564  ...edges..get_ed
-00001e20: 6765 5f64 6174 6172 1100 0000 7288 0000  ge_datar....r...
-00001e30: 0072 6a00 0000 da05 7772 6974 65da 0373  .rj.....write..s
-00001e40: 7472 da0f 636c 7573 7465 725f 6665 6174  tr..cluster_feat
-00001e50: 7572 6529 2172 1a00 0000 7296 0000 0072  ure)!r....r....r
-00001e60: 5500 0000 7246 0000 0072 3c00 0000 7276  U...rF...r<...rv
-00001e70: 0000 005a 0966 6561 745f 7061 7474 5a05  ...Z.feat_pattZ.
-00001e80: 7061 7474 315a 0570 6174 7432 7235 0000  patt1Z.patt2r5..
-00001e90: 0072 3600 0000 da06 6c61 6265 6c73 7210  .r6.....labelsr.
-00001ea0: 0000 00da 1074 7261 696e 6564 5f66 6561  .....trained_fea
-00001eb0: 7475 7265 73da 0166 7254 0000 0072 3200  tures..frT...r2.
-00001ec0: 0000 7277 0000 005a 0a70 6174 745f 696e  ..rw...Z.patt_in
-00001ed0: 6465 7872 4f00 0000 7252 0000 0072 5000  dexrO...rR...rP.
-00001ee0: 0000 da0a 6e6f 6465 5f69 6e64 6578 7260  ....node_indexr`
-00001ef0: 0000 00da 096e 6f64 655f 6e61 6d65 5a08  .....node_nameZ.
-00001f00: 6732 5f74 6f5f 6731 729d 0000 0072 6500  g2_to_g1r....re.
-00001f10: 0000 da05 6174 7472 73da 0465 6467 65da  ....attrs..edge.
-00001f20: 096e 6f64 6573 5f73 7472 7287 0000 00da  .nodes_strr.....
-00001f30: 0873 656e 7465 6e63 6572 1b00 0000 721b  .sentencer....r.
-00001f40: 0000 0072 1c00 0000 da0d 7472 6169 6e5f  ...r......train_
-00001f50: 6665 6174 7572 6512 0100 0073 5c00 0000  feature....s\...
-00001f60: 0001 1a01 0e01 0e01 1401 1202 1402 0e02  ................
-00001f70: 0a01 1201 0401 0401 0e01 1201 1801 0e01  ................
-00001f80: 0a01 0401 1401 0601 0801 2801 0a01 3201  ..........(...2.
-00001f90: 0e01 0601 1601 1601 0e01 1201 02ff 0403  ................
-00001fa0: 0e01 1601 0e01 1201 02ff 0403 0e01 0a01  ................
-00001fb0: 0801 0c01 2201 0401 0eff 2a04 7a1e 4665  ....".....*.z.Fe
-00001fc0: 6174 7572 6545 7661 6c75 6174 6f72 2e74  atureEvaluator.t
-00001fd0: 7261 696e 5f66 6561 7475 7265 6302 0000  rain_featurec...
-00001fe0: 0000 0000 0000 0000 0011 0000 0008 0000  ................
-00001ff0: 0043 0000 0073 3e01 0000 6900 7d02 7400  .C...s>...i.}.t.
-00002000: 6a01 a002 6401 a101 7242 7403 6402 8301  j...d...rBt.d...
-00002010: 8f1a 7d03 7404 a005 7c03 a101 7d02 5700  ..}.t...|...}.W.
-00002020: 6400 0400 0400 8303 0100 6e10 3100 7338  d.........n.1.s8
-00002030: 3000 0100 0100 0100 5900 0100 6900 7d04  0.......Y...i.}.
-00002040: 7c01 4400 5d2c 7d05 7406 7c05 6403 1900  |.D.],}.t.|.d...
-00002050: 8301 7c04 7c05 6404 1900 6405 1700 7c05  ..|.|.d...d...|.
-00002060: 6403 1900 1700 3c00 7c05 6406 1900 7d06  d.....<.|.d...}.
-00002070: 714a 7407 a008 a100 7d07 7c04 4400 5d7a  qJt.....}.|.D.]z
-00002080: 7d08 7c04 7c08 1900 6404 6b02 729a 6407  }.|.|...d.k.r.d.
-00002090: 7d09 6e04 6408 7d09 7c07 6a09 7c08 7c09  }.n.d.}.|.j.|.|.
-000020a0: 6409 8d02 0100 7c08 a00a 6405 a101 6406  d.....|...d...d.
-000020b0: 1900 7d0a 7c0a 7c02 7600 7284 7c02 7c0a  ..}.|.|.v.r.|.|.
-000020c0: 1900 7d0b 7c0b 4400 5d2e 7d0c 7c0b 7c0c  ..}.|.D.].}.|.|.
-000020d0: 1900 7d0d 7c0d 4400 5d1c 7d0e 7c0c 640a  ..}.|.D.].}.|.d.
-000020e0: 6b02 72de 7c07 6a0b 7c08 7c0e 7c0c 6409  k.r.|.j.|.|.|.d.
-000020f0: 8d03 0100 71de 71ce 7184 7c00 a00c 7c01  ....q.q.q.|...|.
-00002100: a101 7d0f 6700 7d10 7c0f 9001 7230 7c10  ..}.g.}.|...r0|.
-00002110: a00d 7c06 a00e 640b 640c a00f 7c0f a101  ..|...d.d...|...
-00002120: 6404 a103 a101 0100 6e0a 7c10 a00d 7c06  d.......n.|...|.
-00002130: a101 0100 7c10 5300 290d 4e5a 1a6c 6f6e  ....|.S.).NZ.lon
-00002140: 676d 616e 5f7a 6572 6f5f 7061 7468 735f  gman_zero_paths_
-00002150: 6f6e 655f 6578 707a 1f6c 6f6e 676d 616e  one_expz.longman
-00002160: 5f7a 6572 6f5f 7061 7468 735f 6f6e 655f  _zero_paths_one_
-00002170: 6578 702e 6a73 6f6e 723f 0000 0072 2700  exp.jsonr?...r'.
-00002180: 0000 7235 0000 0072 0100 0000 da05 6772  ..r5...r......gr
-00002190: 6565 6eda 0372 6564 2901 729f 0000 00da  een..red).r.....
-000021a0: 0131 729c 0000 00fa 017c 2910 720f 0000  .1r......|).r...
-000021b0: 0072 1000 0000 da06 6973 6669 6c65 72a5  .r......isfiler.
-000021c0: 0000 00da 046a 736f 6eda 046c 6f61 64da  .....json..load.
-000021d0: 0369 6e74 722c 0000 00da 0c4d 756c 7469  .intr,.....Multi
-000021e0: 4469 4772 6170 68da 0861 6464 5f6e 6f64  DiGraph..add_nod
-000021f0: 65da 0573 706c 6974 da08 6164 645f 6564  e..split..add_ed
-00002200: 6765 da0c 7365 6c65 6374 5f77 6f72 6473  ge..select_words
-00002210: 7269 0000 00da 0772 6570 6c61 6365 7211  ri.....replacer.
-00002220: 0000 0029 1172 1a00 0000 72ac 0000 0072  ...).r....r....r
-00002230: 3600 0000 72ad 0000 00da 0577 6f72 6473  6...r......words
-00002240: da06 6669 656c 6473 7255 0000 0072 5200  ..fieldsrU...rR.
-00002250: 0000 da04 776f 7264 729f 0000 005a 0a77  ....wordr....Z.w
-00002260: 6f72 645f 636c 6561 6e5a 0968 7970 6572  ord_cleanZ.hyper
-00002270: 6e79 6d73 5a08 6879 7065 726e 796d 5a0e  nymsZ.hypernymZ.
-00002280: 6879 7065 726e 796d 5f77 6f72 6473 da01  hypernym_words..
-00002290: 77da 0e73 656c 6563 7465 645f 776f 7264  w..selected_word
-000022a0: 735a 0d77 6f72 645f 6665 6174 7572 6573  sZ.word_features
-000022b0: 721b 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
-000022c0: aa00 0000 4601 0000 7338 0000 0000 0104  ....F...s8......
-000022d0: 010c 010a 0128 0204 0108 0120 010a 0108  .....(..... ....
-000022e0: 0208 010c 0106 0204 010e 010e 0108 0108  ................
-000022f0: 0108 0108 0108 0108 0116 020a 0204 0206  ................
-00002300: 011c 020a 027a 2046 6561 7475 7265 4576  .....z FeatureEv
-00002310: 616c 7561 746f 722e 636c 7573 7465 725f  aluator.cluster_
-00002320: 6665 6174 7572 6563 0200 0000 0000 0000  featurec........
-00002330: 0000 0000 1000 0000 0600 0000 4300 0000  ............C...
-00002340: 73b0 0100 0067 007d 0267 007d 037c 0144  s....g.}.g.}.|.D
-00002350: 005d 247d 047c 02a0 007c 0464 0119 00a1  .]$}.|...|.d....
-00002360: 0101 007c 03a0 0074 017c 0464 0219 0083  ...|...t.|.d....
-00002370: 01a1 0101 0071 0c64 0364 0484 0074 027c  .....q.d.d...t.|
-00002380: 0283 0144 0083 017d 057c 0544 005d a67d  ...D...}.|.D.].}
-00002390: 0674 037c 0383 0144 005d 985c 027d 077d  .t.|...D.].\.}.}
-000023a0: 087c 0872 807c 027c 0719 007c 066b 0272  .|.r.|.|...|.k.r
-000023b0: 807c 057c 0619 0064 0505 0019 0064 0137  .|.|...d.....d.7
-000023c0: 0003 003c 007c 0872 a47c 027c 0719 007c  ...<.|.r.|.|...|
-000023d0: 066b 0372 a47c 057c 0619 0064 0605 0019  .k.r.|.|...d....
-000023e0: 0064 0137 0003 003c 007c 0873 c87c 027c  .d.7...<.|.s.|.|
-000023f0: 0719 007c 066b 0272 c87c 057c 0619 0064  ...|.k.r.|.|...d
-00002400: 0705 0019 0064 0137 0003 003c 007c 0873  .....d.7...<.|.s
-00002410: 547c 027c 0719 007c 066b 0372 547c 057c  T|.|...|.k.rT|.|
-00002420: 0619 0064 0805 0019 0064 0137 0003 003c  ...d.....d.7...<
-00002430: 0071 5471 487c 0544 005d 647d 067c 057c  .qTqH|.D.]d}.|.|
-00002440: 0619 0064 0519 007d 097c 057c 0619 0064  ...d...}.|.|...d
-00002450: 0719 007d 0a7c 057c 0619 0064 0819 007d  ...}.|.|...d...}
-00002460: 0b7c 057c 0619 0064 0619 007d 0c7c 097c  .|.|...d...}.|.|
-00002470: 097c 0a17 001b 007d 0d7c 097c 097c 0c17  .|.....}.|.|.|..
-00002480: 001b 007d 0e7c 0d7c 057c 0619 0064 093c  ...}.|.|.|...d.<
-00002490: 007c 0e7c 057c 0619 0064 0a3c 0071 f474  .|.|.|...d.<.q.t
-000024a0: 0283 007d 0f7c 0544 005d 467d 067c 057c  ...}.|.D.]F}.|.|
-000024b0: 0619 0064 0919 0064 0b6b 0490 0172 647c  ...d...d.k...rd|
-000024c0: 057c 0619 0064 0519 0064 016b 0490 0173  .|...d...d.k...s
-000024d0: 9e7c 057c 0619 0064 0a19 0064 0c6b 0490  .|.|...d...d.k..
-000024e0: 0172 647c 0fa0 047c 06a1 0101 0090 0171  .rd|...|.......q
-000024f0: 647c 0f53 0029 0d4e 7227 0000 0072 3f00  d|.S.).Nr'...r?.
-00002500: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00002510: 0000 0008 0000 0053 0000 0073 1c00 0000  .......S...s....
-00002520: 6900 7c00 5d14 7d01 7c01 6400 6400 6400  i.|.].}.|.d.d.d.
-00002530: 6400 6401 9c04 9302 7104 5300 2902 7201  d.d.....q.S.).r.
-00002540: 0000 0029 04da 0254 50da 0246 50da 0254  ...)...TP..FP..T
-00002550: 4eda 0246 4e72 1b00 0000 2902 7280 0000  N..FNr....).r...
-00002560: 0072 c500 0000 721b 0000 0072 1b00 0000  .r....r....r....
-00002570: 721c 0000 0072 9e00 0000 7301 0000 7302  r....r....s...s.
-00002580: 0000 0006 017a 3146 6561 7475 7265 4576  .....z1FeatureEv
-00002590: 616c 7561 746f 722e 7365 6c65 6374 5f77  aluator.select_w
-000025a0: 6f72 6473 2e3c 6c6f 6361 6c73 3e2e 3c64  ords.<locals>.<d
-000025b0: 6963 7463 6f6d 703e 72c8 0000 0072 cb00  ictcomp>r....r..
-000025c0: 0000 72c9 0000 0072 ca00 0000 da09 7072  ..r....r......pr
-000025d0: 6563 6973 696f 6eda 0672 6563 616c 6c67  ecision..recallg
-000025e0: cdcc cccc cccc ec3f 677b 14ae 47e1 7a84  .......?g{..G.z.
-000025f0: 3f29 0572 6900 0000 72bc 0000 00da 0373  ?).ri...r......s
-00002600: 6574 724a 0000 00da 0361 6464 2910 721a  etrJ.....add).r.
-00002610: 0000 0072 ac00 0000 7253 0000 0072 ab00  ...r....rS...r..
-00002620: 0000 72c4 0000 005a 1177 6f72 6473 5f74  ..r....Z.words_t
-00002630: 6f5f 6d65 6173 7572 6573 72c5 0000 0072  o_measuresr....r
-00002640: 5400 0000 7287 0000 0072 c800 0000 72c9  T...r....r....r.
-00002650: 0000 0072 ca00 0000 72cb 0000 0072 cc00  ...r....r....r..
-00002660: 0000 72cd 0000 0072 c700 0000 721b 0000  ..r....r....r...
-00002670: 0072 1b00 0000 721c 0000 0072 c100 0000  .r....r....r....
-00002680: 6c01 0000 7348 0000 0000 0104 0104 0208  l...sH..........
-00002690: 010e 0114 0106 0106 ff06 0308 0110 0110  ................
-000026a0: 0114 0110 0114 0110 0114 0110 0118 0208  ................
-000026b0: 010c 010c 010c 010c 020c 010c 020c 010e  ................
-000026c0: 0206 0208 0112 010e ff04 020e fe04 040e  ................
-000026d0: 027a 1d46 6561 7475 7265 4576 616c 7561  .z.FeatureEvalua
-000026e0: 746f 722e 7365 6c65 6374 5f77 6f72 6473  tor.select_words
-000026f0: 6306 0000 0000 0000 0000 0000 0023 0000  c............#..
-00002700: 0006 0000 0043 0000 0073 0203 0000 6700  .....C...s....g.
-00002710: 7d06 7c03 6a00 a001 a100 7d07 7c00 a002  }.|.j.....}.|...
-00002720: 7c03 7c01 a102 6a02 a001 a100 7d08 6700  |.|...j.....}.g.
-00002730: 7d09 7403 7404 8301 7d0a 6700 7d0b 6700  }.t.t...}.g.}.g.
-00002740: 7d0c 6700 7d0d 7c05 7c02 7405 7c00 6a06  }.g.}.|.|.t.|.j.
-00002750: 6401 8d03 7d0e 7407 7c07 8301 4400 5d96  d...}.t.|...D.].
-00002760: 5c02 7d0f 7d10 7c0e a008 7c10 a101 7d11  \.}.}.|...|...}.
-00002770: 6402 7d12 7c11 4400 5d22 5c02 7d13 7d14  d.}.|.D.]"\.}.}.
-00002780: 7c0a 7c0f 1900 a009 7c02 7c14 1900 6402  |.|.....|.|...d.
-00002790: 1900 a101 0100 6403 7d12 716a 7c09 a009  ......d.}.qj|...
-000027a0: 7c12 a101 0100 7c12 6402 6b02 7250 7c08  |.....|.d.k.rP|.
-000027b0: 7c0f 1900 6403 6b02 7250 7c0b a009 7c10  |...d.k.rP|...|.
-000027c0: a101 0100 7c03 6a0a 7c0f 1900 6a0b 7d15  ....|.j.|...j.}.
-000027d0: 7c03 6a0a 7c0f 1900 6a0c 7d16 7c0c a009  |.j.|...j.}.|...
-000027e0: 7c15 7c16 6602 a101 0100 7c0d a009 7c0f  |.|.f.....|...|.
-000027f0: a101 0100 7150 6700 7d17 740d 7c08 7c09  ....qPg.}.t.|.|.
-00002800: 6400 6404 8d03 4400 5d2c 7d18 740e 7c18  d.d...D.],}.t.|.
-00002810: 8301 6403 6b04 9001 721c 7c17 a009 7c18  ..d.k...r.|...|.
-00002820: 6403 1900 a101 0100 71fa 7c17 a009 6402  d.......q.|...d.
-00002830: a101 0100 71fa 7c02 4400 9001 5db8 7d19  ....q.|.D...].}.
-00002840: 7c19 6402 1900 6701 7d1a 6700 7d1b 6700  |.d...g.}.g.}.g.
-00002850: 7d1c 6700 7d1d 6700 7d1e 6700 7d1f 6700  }.g.}.g.}.g.}.g.
-00002860: 7d20 6700 7d21 7407 7c07 8301 4400 5dd6  } g.}!t.|...D.].
-00002870: 5c02 7d0f 7d10 7c0a 7c0f 1900 7d11 7c19  \.}.}.|.|...}.|.
-00002880: 6402 1900 7c11 7600 9001 7282 6403 6e02  d...|.v...r.d.n.
-00002890: 6402 7d12 7c12 6403 6b02 9001 72d8 7c08  d.}.|.d.k...r.|.
-000028a0: 7c0f 1900 6402 6b02 9001 72d8 7c1b a009  |...d.k...r.|...
-000028b0: 7c10 a101 0100 7c03 6a0a 7c0f 1900 6a0b  |.....|.j.|...j.
-000028c0: 7d15 7c03 6a0a 7c0f 1900 6a0c 7d16 7c1c  }.|.j.|...j.}.|.
-000028d0: a009 7c15 7c16 6602 a101 0100 7c1d a009  ..|.|.f.....|...
-000028e0: 7c0f a101 0100 7c12 6403 6b02 9002 722a  |.....|.d.k...r*
-000028f0: 7c08 7c0f 1900 6403 6b02 9002 722a 7c1e  |.|...d.k...r*|.
-00002900: a009 7c10 a101 0100 7c03 6a0a 7c0f 1900  ..|.....|.j.|...
-00002910: 6a0b 7d15 7c03 6a0a 7c0f 1900 6a0c 7d16  j.}.|.j.|...j.}.
-00002920: 7c1f a009 7c15 7c16 6602 a101 0100 7c20  |...|.|.f.....| 
-00002930: a009 7c0f a101 0100 7c21 a009 7c12 a101  ..|.....|!..|...
-00002940: 0100 9001 7160 740d 7c08 7c21 6400 6404  ....q`t.|.|!d.d.
-00002950: 8d03 4400 5d2e 7d18 740e 7c18 8301 6403  ..D.].}.t.|...d.
-00002960: 6b04 9002 7268 7c1a a009 7c18 6403 1900  k...rh|...|.d...
-00002970: a101 0100 6e0a 7c1a a009 6402 a101 0100  ....n.|...d.....
-00002980: 9002 7146 7c1a a009 7c1b a101 0100 7c1a  ..qF|...|.....|.
-00002990: a009 7c1c a101 0100 7c1a a009 7c1d a101  ..|.....|...|...
-000029a0: 0100 7c1a a009 7c1e a101 0100 7c1a a009  ..|...|.....|...
-000029b0: 7c1f a101 0100 7c1a a009 7c20 a101 0100  |.....|...| ....
-000029c0: 7c1a a009 7c0b a101 0100 7c1a a009 7c0c  |...|.....|...|.
-000029d0: a101 0100 7c1a a009 7c0d a101 0100 7c1a  ....|...|.....|.
-000029e0: a009 7c21 a101 0100 7c06 a009 7c1a a101  ..|!....|...|...
-000029f0: 0100 9001 712c 740f 6a10 7c06 6700 6405  ....q,t.j.|.g.d.
-00002a00: a201 6406 8d02 7d22 7c22 7c17 6602 5300  ..d...}"|"|.f.S.
-00002a10: 2907 4e72 4000 0000 7201 0000 0072 2700  ).Nr@...r....r'.
-00002a20: 0000 2901 da07 6176 6572 6167 6529 0fda  ..)...average)..
-00002a30: 0746 6561 7475 7265 728f 0000 0072 9000  .Featurer....r..
-00002a40: 0000 7291 0000 0072 9200 0000 5a15 4661  ..r....r....Z.Fa
-00002a50: 6c73 655f 706f 7369 7469 7665 5f67 7261  lse_positive_gra
-00002a60: 7068 7372 9400 0000 5a16 4661 6c73 655f  phsr....Z.False_
-00002a70: 706f 7369 7469 7665 5f69 6e64 6963 6573  positive_indices
-00002a80: 728a 0000 0072 9300 0000 5a15 5472 7565  r....r....Z.True
-00002a90: 5f70 6f73 6974 6976 655f 696e 6469 6365  _positive_indice
-00002aa0: 735a 1546 616c 7365 5f6e 6567 6174 6976  sZ.False_negativ
-00002ab0: 655f 6772 6170 6873 5a13 4661 6c73 655f  e_graphsZ.False_
-00002ac0: 6e65 6761 7469 7665 5f73 656e 735a 1646  negative_sensZ.F
-00002ad0: 616c 7365 5f6e 6567 6174 6976 655f 696e  alse_negative_in
-00002ae0: 6469 6365 735a 0950 7265 6469 6374 6564  dicesZ.Predicted
-00002af0: 2901 da07 636f 6c75 6d6e 7329 1172 5200  )...columns).rR.
-00002b00: 0000 7268 0000 0072 8500 0000 7202 0000  ..rh...r....r...
-00002b10: 0072 2a00 0000 720a 0000 0072 3d00 0000  .r*...r....r=...
-00002b20: 724a 0000 0072 4f00 0000 7269 0000 0072  rJ...rO...ri...r
-00002b30: 8800 0000 726a 0000 0072 8700 0000 7204  ....rj...r....r.
-00002b40: 0000 0072 4b00 0000 726b 0000 0072 6c00  ...rK...rk...rl.
-00002b50: 0000 2923 721a 0000 0072 9600 0000 7253  ..)#r....r....rS
-00002b60: 0000 0072 4600 0000 723c 0000 0072 7600  ...rF...r<...rv.
-00002b70: 0000 5a10 6d65 6173 7572 655f 6665 6174  ..Z.measure_feat
-00002b80: 7572 6573 7236 0000 0072 ab00 0000 5a0f  uresr6...r....Z.
-00002b90: 7768 6f6c 655f 7072 6564 6963 7465 64da  whole_predicted.
-00002ba0: 076d 6174 6368 6564 5a0b 6661 6c73 655f  .matchedZ.false_
-00002bb0: 6e65 675f 675a 0b66 616c 7365 5f6e 6567  neg_gZ.false_neg
-00002bc0: 5f73 5a11 6661 6c73 655f 6e65 675f 696e  _sZ.false_neg_in
-00002bd0: 6469 6365 7372 1800 0000 7254 0000 0072  dicesr....rT...r
-00002be0: 3200 0000 725a 0000 0072 8700 0000 725b  2...rZ...r....r[
-00002bf0: 0000 0072 5500 0000 7231 0000 00da 036c  ...rU...r1.....l
-00002c00: 6162 7298 0000 005a 0370 6366 da04 6665  abr....Z.pcf..fe
-00002c10: 6174 da07 6d65 6173 7572 655a 0b66 616c  at..measureZ.fal
-00002c20: 7365 5f70 6f73 5f67 5a0b 6661 6c73 655f  se_pos_gZ.false_
-00002c30: 706f 735f 735a 1166 616c 7365 5f70 6f73  pos_sZ.false_pos
-00002c40: 5f69 6e64 6963 6573 5a0a 7472 7565 5f70  _indicesZ.true_p
-00002c50: 6f73 5f67 5a0a 7472 7565 5f70 6f73 5f73  os_gZ.true_pos_s
-00002c60: 5a10 7472 7565 5f70 6f73 5f69 6e64 6963  Z.true_pos_indic
-00002c70: 6573 7278 0000 0072 7a00 0000 721b 0000  esrx...rz...r...
-00002c80: 0072 1b00 0000 721c 0000 0072 8e00 0000  .r....r....r....
-00002c90: 9801 0000 7398 0000 0000 0804 010a 0112  ....s...........
-00002ca0: 0204 0108 0304 0104 0104 0102 0108 ff06  ................
-00002cb0: 0310 010a 0104 010c 0116 0106 010a 0214  ................
-00002cc0: 010a 010c 010c 010e 010c 0204 0102 0106  ................
-00002cd0: ff0a 030e 0110 020c 020a 010a 0104 0104  ................
-00002ce0: 0104 0104 0104 0104 0104 0110 0108 0116  ................
-00002cf0: 0118 010a 010c 010c 010e 010a 0118 010a  ................
-00002d00: 010c 010c 010e 010a 010e 0112 010e 0110  ................
-00002d10: 020e 010a 010a 010a 010a 010a 010a 010a  ................
-00002d20: 010a 010a 010a 010e 0204 0102 0106 fe06  ................
-00002d30: 157a 2146 6561 7475 7265 4576 616c 7561  .z!FeatureEvalua
-00002d40: 746f 722e 6576 616c 7561 7465 5f66 6561  tor.evaluate_fea
-00002d50: 7475 7265 4e29 0272 2900 0000 4629 0146  tureN).r)...F).F
-00002d60: 2901 7229 0000 0029 1072 3800 0000 7239  ).r)...).r8...r9
-00002d70: 0000 0072 3a00 0000 721d 0000 0072 6600  ...r:...r....rf.
-00002d80: 0000 7271 0000 0072 0800 0000 727b 0000  ..rq...r....r{..
-00002d90: 0072 7300 0000 7274 0000 0072 8500 0000  .rs...rt...r....
-00002da0: 7299 0000 0072 b400 0000 72aa 0000 0072  r....r....r....r
-00002db0: c100 0000 728e 0000 0072 1b00 0000 721b  ....r....r....r.
-00002dc0: 0000 0072 1b00 0000 721c 0000 0072 3b00  ...r....r....r;.
-00002dd0: 0000 5200 0000 7326 0000 0008 010a 0608  ..R...s&........
-00002de0: 3108 1202 0102 0102 0102 f90a 3500 f90a  1...........5...
-00002df0: 1a08 0b08 0a08 1d0a 3408 2608 3102 0102  ........4.&.1...
-00002e00: fa72 3b00 0000 291d 72ba 0000 0072 0f00  .r;...).r....r..
-00002e10: 0000 da0b 636f 6c6c 6563 7469 6f6e 7372  ....collectionsr
-00002e20: 0200 0000 da08 6e65 7477 6f72 6b78 722c  ......networkxr,
-00002e30: 0000 00da 0670 616e 6461 7372 6b00 0000  .....pandasrk...
-00002e40: 7223 0000 005a 0670 656e 6d61 6e72 4c00  r#...Z.penmanrL.
-00002e50: 0000 5a1f 6e65 7477 6f72 6b78 2e61 6c67  ..Z.networkx.alg
-00002e60: 6f72 6974 686d 732e 6973 6f6d 6f72 7068  orithms.isomorph
-00002e70: 6973 6d72 0300 0000 5a0f 736b 6c65 6172  ismr....Z.sklear
-00002e80: 6e2e 6d65 7472 6963 7372 0400 0000 7205  n.metricsr....r.
-00002e90: 0000 005a 1d74 7577 5f6e 6c70 2e67 7261  ...Z.tuw_nlp.gra
-00002ea0: 6d6d 6172 2e74 6578 745f 746f 5f34 6c61  mmar.text_to_4la
-00002eb0: 6e67 7206 0000 00da 1374 7577 5f6e 6c70  ngr......tuw_nlp
-00002ec0: 2e67 7261 7068 2e75 7469 6c73 7207 0000  .graph.utilsr...
-00002ed0: 0072 0800 0000 5a15 7475 775f 6e6c 702e  .r....Z.tuw_nlp.
-00002ee0: 7465 7874 2e70 6970 656c 696e 6572 0900  text.pipeliner..
-00002ef0: 0000 da15 7870 6f74 6174 6f2e 6461 7461  ....xpotato.data
-00002f00: 7365 742e 7574 696c 7372 0a00 0000 720b  set.utilsr....r.
-00002f10: 0000 0072 0c00 0000 720d 0000 0072 3b00  ...r....r....r;.
-00002f20: 0000 721b 0000 0072 1b00 0000 721b 0000  ..r....r....r...
-00002f30: 0072 1c00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00002f40: 0100 0000 731e 0000 0008 0108 010c 0208  ....s...........
-00002f50: 0108 0108 0108 010c 010c 010c 010c 0110  ................
-00002f60: 040c 0214 030e 3c                        ......<
+00000060: 5a09 6400 6403 6c0a 6d0b 5a0b 0100 6400  Z.d.d.l.m.Z...d.
+00000070: 6404 6c0c 6d0c 5a0c 0100 6400 6405 6c0d  d.l.m.Z...d.d.l.
+00000080: 6d0e 5a0e 0100 6400 6406 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
+00000090: 6d11 5a11 6d12 5a12 0100 4700 6407 6408  m.Z.m.Z...G.d.d.
+000000a0: 8400 6408 8302 5a13 4700 6409 640a 8400  ..d...Z.G.d.d...
+000000b0: 640a 8302 5a14 6401 5300 290b e900 0000  d...Z.d.S.).....
+000000c0: 004e 2901 da0b 6465 6661 756c 7464 6963  .N)...defaultdic
+000000d0: 7429 01da 1f70 7265 6369 7369 6f6e 5f72  t)...precision_r
+000000e0: 6563 616c 6c5f 6673 636f 7265 5f73 7570  ecall_fscore_sup
+000000f0: 706f 7274 2901 da04 7471 646d 2901 da1a  port)...tqdm)...
+00000100: 4772 6170 6846 6f72 6d75 6c61 5061 7474  GraphFormulaPatt
+00000110: 6572 6e4d 6174 6368 6572 2903 da0f 616d  ernMatcher)...am
+00000120: 725f 706e 5f74 6f5f 6772 6170 68da 1364  r_pn_to_graph..d
+00000130: 6566 6175 6c74 5f70 6e5f 746f 5f67 7261  efault_pn_to_gra
+00000140: 7068 da0b 7564 5f74 6f5f 6772 6170 6863  ph..ud_to_graphc
+00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000160: 0300 0000 4000 0000 7328 0000 0065 005a  ....@...s(...e.Z
+00000170: 0164 005a 0264 0964 0264 0384 015a 0364  .d.Z.d.d.d...Z.d
+00000180: 0464 0584 005a 0464 0a64 0764 0884 015a  .d...Z.d.d.d...Z
+00000190: 0564 0153 0029 0bda 0e47 7261 7068 4578  .d.S.)...GraphEx
+000001a0: 7472 6163 746f 724e 6304 0000 0000 0000  tractorNc.......
+000001b0: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
+000001c0: 0073 7a00 0000 7c01 6400 7500 721e 7400  .sz...|.d.u.r.t.
+000001d0: 6a01 a002 7400 6a01 a003 7404 a101 6401  j...t.j...t...d.
+000001e0: a102 7d01 7c02 6400 7500 723a 7400 6a01  ..}.|.d.u.r:t.j.
+000001f0: a002 7c01 7c03 9b00 6402 9d02 a102 7d02  ..|.|...d.....}.
+00000200: 7c01 7c00 5f05 7c02 7c00 5f06 7c03 7c00  |.|._.|.|._.|.|.
+00000210: 5f07 6400 7c00 5f08 6400 7c00 5f09 6400  _.d.|._.d.|._.d.
+00000220: 7c00 5f0a 6400 7c00 5f0b 6400 7c00 5f0c  |._.d.|._.d.|._.
+00000230: 6400 7c00 5f0d 6400 7c00 5f0e 6400 5300  d.|._.d.|._.d.S.
+00000240: 2903 4eda 0563 6163 6865 7a0f 5f6e 6c70  ).N..cachez._nlp
+00000250: 5f63 6163 6865 2e6a 736f 6e29 0fda 026f  _cache.json)...o
+00000260: 73da 0470 6174 68da 046a 6f69 6eda 0764  s..path..join..d
+00000270: 6972 6e61 6d65 da08 5f5f 6669 6c65 5f5f  irname..__file__
+00000280: da09 6361 6368 655f 6469 72da 0863 6163  ..cache_dir..cac
+00000290: 6865 5f66 6eda 046c 616e 67da 076d 6174  he_fn..lang..mat
+000002a0: 6368 6572 da09 7564 5f70 6172 7365 72da  cher..ud_parser.
+000002b0: 0966 6c5f 7061 7273 6572 da0a 616d 725f  .fl_parser..amr_
+000002c0: 7061 7273 6572 da0b 7563 6361 5f70 6172  parser..ucca_par
+000002d0: 7365 72da 0a73 6470 5f70 6172 7365 72da  ser..sdp_parser.
+000002e0: 0a64 7273 5f70 6172 7365 7229 04da 0473  .drs_parser)...s
+000002f0: 656c 6672 1000 0000 7211 0000 0072 1200  elfr....r....r..
+00000300: 0000 a900 721b 0000 00fa 552f 5573 6572  ....r.....U/User
+00000310: 732f 6164 616d 6b6f 7661 6373 2f70 726f  s/adamkovacs/pro
+00000320: 6a65 6374 732f 6578 702d 7265 6c61 7469  jects/exp-relati
+00000330: 6f6e 2d65 7874 7261 6374 696f 6e2f 7870  on-extraction/xp
+00000340: 6f74 6174 6f2f 6772 6170 685f 6578 7472  otato/graph_extr
+00000350: 6163 746f 722f 6578 7472 6163 742e 7079  actor/extract.py
+00000360: da08 5f5f 696e 6974 5f5f 1000 0000 731c  ..__init__....s.
+00000370: 0000 0000 0108 0116 0108 0114 0106 0106  ................
+00000380: 0106 0106 0206 0106 0106 0106 0106 017a  ...............z
+00000390: 1747 7261 7068 4578 7472 6163 746f 722e  .GraphExtractor.
+000003a0: 5f5f 696e 6974 5f5f 6302 0000 0000 0000  __init__c.......
+000003b0: 0000 0000 0008 0000 0005 0000 0043 0000  .............C..
+000003c0: 0073 a201 0000 7c01 6401 6b02 7238 7c00  .s....|.d.k.r8|.
+000003d0: 6a00 6400 6b02 7234 6402 6403 6c01 6d02  j.d.k.r4d.d.l.m.
+000003e0: 7d02 0100 7c02 7c00 6a03 7c00 6a04 7c00  }...|.|.j.|.j.|.
+000003f0: 6a05 6404 8d03 7c00 5f00 9001 6e66 7c01  j.d...|._...nf|.
+00000400: 6405 6b02 7270 7c00 6a06 6400 6b02 726c  d.k.rp|.j.d.k.rl
+00000410: 6402 6406 6c07 6d08 7d03 0100 7c03 7c00  d.d.l.m.}...|.|.
+00000420: 6a03 7c00 6a04 7c00 6a05 6404 8d03 7c00  j.|.j.|.j.d...|.
+00000430: 5f06 9001 6e2e 7c01 6407 6b02 72b2 7c00  _...n.|.d.k.r.|.
+00000440: 6a09 6400 6b02 72b0 7c00 6a03 6408 6b03  j.d.k.r.|.j.d.k.
+00000450: 729c 740a 6409 7c00 6a03 9b00 9d02 8301  r.t.d.|.j.......
+00000460: 8201 6402 640a 6c0b 6d0c 7d04 0100 7c04  ..d.d.l.m.}...|.
+00000470: 8300 7c00 5f09 6eec 7c01 640b 6b02 72f4  ..|._.n.|.d.k.r.
+00000480: 7c00 6a0d 6400 6b02 72f2 7c00 6a03 6408  |.j.d.k.r.|.j.d.
+00000490: 6b03 72de 740a 640c 7c00 6a03 9b00 9d02  k.r.t.d.|.j.....
+000004a0: 8301 8201 6402 640d 6c0e 6d0f 7d05 0100  ....d.d.l.m.}...
+000004b0: 7c05 8300 7c00 5f0d 6eaa 7c01 640e 6b02  |...|._.n.|.d.k.
+000004c0: 9001 7242 7c00 6a10 6400 6b02 9001 729e  ..rB|.j.d.k...r.
+000004d0: 7c00 6a03 6408 6b03 9001 7226 740a 640f  |.j.d.k...r&t.d.
+000004e0: 7c00 6a03 9b00 9d02 8301 8201 6402 6410  |.j.........d.d.
+000004f0: 6c11 6d12 7d06 0100 7c06 7c00 6a03 6411  l.m.}...|.|.j.d.
+00000500: 8d01 7c00 5f10 6e5c 7c01 6412 6b02 9001  ..|._.n\|.d.k...
+00000510: 7290 7c00 6a13 6400 6b02 9001 729e 7c00  r.|.j.d.k...r.|.
+00000520: 6a03 6408 6b03 9001 7274 740a 6413 7c00  j.d.k...rtt.d.|.
+00000530: 6a03 9b00 9d02 8301 8201 6402 6414 6c14  j.........d.d.l.
+00000540: 6d15 7d07 0100 7c07 7c00 6a03 6411 8d01  m.}...|.|.j.d...
+00000550: 7c00 5f13 6e0e 740a 6415 7c01 9b00 9d02  |._.n.t.d.|.....
+00000560: 8301 8201 6400 5300 2916 4eda 0275 6472  ....d.S.).N..udr
+00000570: 0100 0000 2901 da08 5465 7874 546f 5544  ....)...TextToUD
+00000580: 2903 7212 0000 005a 096e 6c70 5f63 6163  ).r....Z.nlp_cac
+00000590: 6865 7210 0000 00da 0866 6f75 726c 616e  her......fourlan
+000005a0: 6729 01da 0b54 6578 7454 6f34 6c61 6e67  g)...TextTo4lang
+000005b0: da03 616d 72da 0265 6e7a 2943 7572 7265  ..amr..enz)Curre
+000005c0: 6e74 6c79 206f 6e6c 7920 656e 676c 6973  ntly only englis
+000005d0: 6820 414d 5220 6973 2073 7570 706f 7274  h AMR is support
+000005e0: 6564 3a20 2901 da09 5465 7874 546f 414d  ed: )...TextToAM
+000005f0: 52da 0475 6363 617a 2a43 7572 7265 6e74  R..uccaz*Current
+00000600: 6c79 206f 6e6c 7920 656e 676c 6973 6820  ly only english 
+00000610: 5543 4341 2069 7320 7375 7070 6f72 7465  UCCA is supporte
+00000620: 643a 2029 01da 0a54 6578 7454 6f55 4343  d: )...TextToUCC
+00000630: 41da 0373 6470 7a29 4375 7272 656e 746c  A..sdpz)Currentl
+00000640: 7920 6f6e 6c79 2065 6e67 6c69 7368 2053  y only english S
+00000650: 4450 2069 7320 7375 7070 6f72 7465 643a  DP is supported:
+00000660: 2029 01da 0954 6578 7454 6f53 4450 2901   )...TextToSDP).
+00000670: 7212 0000 00da 0364 7273 7a29 4375 7272  r......drsz)Curr
+00000680: 656e 746c 7920 6f6e 6c79 2065 6e67 6c69  ently only engli
+00000690: 7368 2044 5253 2069 7320 7375 7070 6f72  sh DRS is suppor
+000006a0: 7465 643a 2029 01da 0954 6578 7454 6f44  ted: )...TextToD
+000006b0: 5253 7a19 4375 7272 656e 746c 7920 6e6f  RSz.Currently no
+000006c0: 7420 7375 7070 6f72 7465 643a 2029 1672  t supported: ).r
+000006d0: 1400 0000 5a1a 7475 775f 6e6c 702e 6772  ....Z.tuw_nlp.gr
+000006e0: 616d 6d61 722e 7465 7874 5f74 6f5f 7564  ammar.text_to_ud
+000006f0: 721f 0000 0072 1200 0000 7211 0000 0072  r....r....r....r
+00000700: 1000 0000 7215 0000 005a 1d74 7577 5f6e  ....r....Z.tuw_n
+00000710: 6c70 2e67 7261 6d6d 6172 2e74 6578 745f  lp.grammar.text_
+00000720: 746f 5f34 6c61 6e67 7221 0000 0072 1600  to_4langr!...r..
+00000730: 0000 da0a 5661 6c75 6545 7272 6f72 5a1b  ....ValueErrorZ.
+00000740: 7475 775f 6e6c 702e 6772 616d 6d61 722e  tuw_nlp.grammar.
+00000750: 7465 7874 5f74 6f5f 616d 7272 2400 0000  text_to_amrr$...
+00000760: 7217 0000 005a 1c74 7577 5f6e 6c70 2e67  r....Z.tuw_nlp.g
+00000770: 7261 6d6d 6172 2e74 6578 745f 746f 5f75  rammar.text_to_u
+00000780: 6363 6172 2600 0000 7218 0000 005a 1b74  ccar&...r....Z.t
+00000790: 7577 5f6e 6c70 2e67 7261 6d6d 6172 2e74  uw_nlp.grammar.t
+000007a0: 6578 745f 746f 5f73 6470 7228 0000 0072  ext_to_sdpr(...r
+000007b0: 1900 0000 5a1b 7475 775f 6e6c 702e 6772  ....Z.tuw_nlp.gr
+000007c0: 616d 6d61 722e 7465 7874 5f74 6f5f 6472  ammar.text_to_dr
+000007d0: 7372 2a00 0000 2908 721a 0000 00da 0a67  sr*...).r......g
+000007e0: 7261 7068 5f74 7970 6572 1f00 0000 7221  raph_typer....r!
+000007f0: 0000 0072 2400 0000 7226 0000 0072 2800  ...r$...r&...r(.
+00000800: 0000 722a 0000 0072 1b00 0000 721b 0000  ..r*...r....r...
+00000810: 0072 1c00 0000 da0e 696e 6974 5f72 6573  .r......init_res
+00000820: 6f75 7263 6573 2100 0000 735a 0000 0000  ources!...sZ....
+00000830: 0108 010a 010c 0202 010c ff0c 0408 010a  ................
+00000840: 010c 0202 010c ff0c 0408 010a 010a 0102  ................
+00000850: 010a ff04 030c 020a 0208 010a 010a 0102  ................
+00000860: 010a ff04 030c 020a 020a 010c 010c 0102  ................
+00000870: 010a ff04 030c 0210 010a 010c 010c 0102  ................
+00000880: 010a ff04 030c 0210 037a 1d47 7261 7068  .........z.Graph
+00000890: 4578 7472 6163 746f 722e 696e 6974 5f72  Extractor.init_r
+000008a0: 6573 6f75 7263 6573 7220 0000 0063 0400  esourcesr ...c..
+000008b0: 0000 0000 0000 0000 0000 0a00 0000 0800  ................
+000008c0: 0000 6300 0000 73d0 0100 007c 0372 0a7c  ..c...s....|.r.|
+000008d0: 037c 005f 007c 00a0 017c 02a1 0101 007c  .|._.|...|.....|
+000008e0: 0264 016b 0272 947c 006a 028f 5e7d 0474  .d.k.r.|.j..^}.t
+000008f0: 037c 0183 0144 005d 447d 0574 047c 047c  .|...D.]D}.t.|.|
+00000900: 0564 0264 038d 0283 017d 067c 0664 0419  .d.d.....}.|.d..
+00000910: 007d 077c 0664 0564 0085 0219 0044 005d  .}.|.d.d.....D.]
+00000920: 147d 0874 0564 067c 059b 0064 079d 0383  .}.t.d.|...d....
+00000930: 0182 0171 547c 0756 0001 0071 2c57 0064  ...qT|.V...q,W.d
+00000940: 0004 0004 0083 0301 006e 1031 0073 8630  .........n.1.s.0
+00000950: 0001 0001 0001 0059 0001 0090 016e 387c  .......Y.....n8|
+00000960: 0264 086b 0272 ee74 037c 0183 0144 005d  .d.k.r.t.|...D.]
+00000970: 467d 0574 047c 006a 067c 0564 0264 038d  F}.t.|.j.|.d.d..
+00000980: 0283 017d 097c 0964 0419 007d 077c 0964  ...}.|.d...}.|.d
+00000990: 0564 0085 0219 0044 005d 147d 0874 0564  .d.....D.].}.t.d
+000009a0: 067c 059b 0064 079d 0383 0182 0171 ce7c  .|...d.......q.|
+000009b0: 0756 0001 0071 a46e de7c 0264 096b 0290  .V...q.n.|.d.k..
+000009c0: 0172 2274 037c 0183 0144 005d 1e7d 057c  .r"t.|...D.].}.|
+000009d0: 00a0 077c 05a1 017d 0774 047c 0783 0164  ...|...}.t.|...d
+000009e0: 0419 0056 0001 0090 0171 006e aa7c 0264  ...V.....q.n.|.d
+000009f0: 0a6b 0290 0172 5674 037c 0183 0144 005d  .k...rVt.|...D.]
+00000a00: 1e7d 057c 00a0 087c 05a1 017d 0774 047c  .}.|...|...}.t.|
+00000a10: 0783 0164 0419 0056 0001 0090 0171 346e  ...d...V.....q4n
+00000a20: 767c 0264 0b6b 0290 0172 8a74 037c 0183  v|.d.k...r.t.|..
+00000a30: 0144 005d 1e7d 057c 00a0 097c 05a1 017d  .D.].}.|...|...}
+00000a40: 0774 047c 0783 0164 0419 0056 0001 0090  .t.|...d...V....
+00000a50: 0171 686e 427c 0264 0c6b 0290 0172 be74  .qhnB|.d.k...r.t
+00000a60: 037c 0183 0144 005d 1e7d 057c 00a0 0a7c  .|...D.].}.|...|
+00000a70: 05a1 017d 0774 047c 0783 0164 0419 0056  ...}.t.|...d...V
+00000a80: 0001 0090 0171 9c6e 0e74 0564 0d7c 029b  .....q.n.t.d.|..
+00000a90: 009d 0283 0182 0164 0053 0029 0e4e 7220  .......d.S.).Nr 
+00000aa0: 0000 0046 2901 5a06 7373 706c 6974 7201  ...F).Z.ssplitr.
+00000ab0: 0000 00e9 0100 0000 7a21 7365 6e74 656e  ........z!senten
+00000ac0: 6365 2073 686f 756c 6420 6e6f 7420 6265  ce should not be
+00000ad0: 2073 706c 6974 2075 703a 20fa 0121 721e   split up: ..!r.
+00000ae0: 0000 0072 2200 0000 7225 0000 0072 2700  ...r"...r%...r'.
+00000af0: 0000 7229 0000 007a 1a43 7572 7272 656e  ..r)...z.Currren
+00000b00: 746c 7920 6e6f 7420 7375 7070 6f72 7465  tly not supporte
+00000b10: 643a 2029 0b72 1200 0000 722d 0000 0072  d: ).r....r-...r
+00000b20: 1500 0000 7204 0000 00da 046c 6973 7472  ....r......listr
+00000b30: 2b00 0000 7214 0000 0072 1600 0000 7217  +...r....r....r.
+00000b40: 0000 0072 1800 0000 7219 0000 0029 0a72  ...r....r....).r
+00000b50: 1a00 0000 da08 6974 6572 6162 6c65 722c  ......iterabler,
+00000b60: 0000 0072 1200 0000 5a03 7466 6cda 0373  ...r....Z.tfl..s
+00000b70: 656e 5a09 666c 5f67 7261 7068 73da 0167  enZ.fl_graphs..g
+00000b80: da01 6e5a 0975 645f 6772 6170 6873 721b  ..nZ.ud_graphsr.
+00000b90: 0000 0072 1b00 0000 721c 0000 00da 0e70  ...r....r......p
+00000ba0: 6172 7365 5f69 7465 7261 626c 655c 0000  arse_iterable\..
+00000bb0: 0073 4600 0000 0001 0401 0601 0a01 0801  .sF.............
+00000bc0: 0801 0c01 1001 0801 1001 1201 2a02 0801  ............*...
+00000bd0: 0c01 1201 0801 1001 1201 0a02 0a01 0c01  ................
+00000be0: 0a02 1402 0a01 0c01 0a02 1402 0a01 0c01  ................
+00000bf0: 0a02 1402 0a01 0c01 0a02 1402 7a1d 4772  ............z.Gr
+00000c00: 6170 6845 7874 7261 6374 6f72 2e70 6172  aphExtractor.par
+00000c10: 7365 5f69 7465 7261 626c 6529 034e 4e4e  se_iterable).NNN
+00000c20: 2902 7220 0000 004e 2906 da08 5f5f 6e61  ).r ...N)...__na
+00000c30: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000c40: da0c 5f5f 7175 616c 6e61 6d65 5f5f 721d  ..__qualname__r.
+00000c50: 0000 0072 2d00 0000 7235 0000 0072 1b00  ...r-...r5...r..
+00000c60: 0000 721b 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+00000c70: 0072 0900 0000 0f00 0000 7306 0000 0008  .r........s.....
+00000c80: 010a 1108 3b72 0900 0000 6300 0000 0000  ....;r....c.....
+00000c90: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
+00000ca0: 0000 0073 8200 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00000cb0: 641c 6403 6404 8401 5a03 6405 6406 8400  d.d.d...Z.d.d...
+00000cc0: 5a04 6407 6408 8400 5a05 6402 6402 6506  Z.d.d...Z.d.d.e.
+00000cd0: 6402 6604 6409 640a 8401 5a07 641d 640b  d.f.d.d...Z.d.d.
+00000ce0: 640c 8401 5a08 640d 640e 8400 5a09 640f  d...Z.d.d...Z.d.
+00000cf0: 6410 8400 5a0a 6411 6412 8400 5a0b 641e  d...Z.d.d...Z.d.
+00000d00: 6413 6414 8401 5a0c 6415 6416 8400 5a0d  d.d...Z.d.d...Z.
+00000d10: 6417 6418 8400 5a0e 6401 6506 6602 6419  d.d...Z.d.e.f.d.
+00000d20: 641a 8401 5a0f 641b 5300 291f da10 4665  d...Z.d.S.)...Fe
+00000d30: 6174 7572 6545 7661 6c75 6174 6f72 721e  atureEvaluatorr.
+00000d40: 0000 0046 6303 0000 0000 0000 0000 0000  ...Fc...........
+00000d50: 0003 0000 0002 0000 0043 0000 0073 1000  .........C...s..
+00000d60: 0000 7c01 7c00 5f00 7c02 7c00 5f01 6400  ..|.|._.|.|._.d.
+00000d70: 5300 2901 4e29 02da 0c67 7261 7068 5f66  S.).N)...graph_f
+00000d80: 6f72 6d61 74da 0e63 6173 655f 7365 6e73  ormat..case_sens
+00000d90: 6974 6976 6529 0372 1a00 0000 723a 0000  itive).r....r:..
+00000da0: 0072 3b00 0000 721b 0000 0072 1b00 0000  .r;...r....r....
+00000db0: 721c 0000 0072 1d00 0000 8d00 0000 7304  r....r........s.
+00000dc0: 0000 0000 0106 017a 1946 6561 7475 7265  .......z.Feature
+00000dd0: 4576 616c 7561 746f 722e 5f5f 696e 6974  Evaluator.__init
+00000de0: 5f5f 6303 0000 0000 0000 0000 0000 001b  __c.............
+00000df0: 0000 0006 0000 0063 0000 0073 9201 0000  .......c...s....
+00000e00: 6900 7d03 7400 7c02 8301 4400 5dbe 5c02  i.}.t.|...D.].\.
+00000e10: 7d04 7d05 7401 7c05 8301 6401 6b02 732e  }.}.t.|...d.k.s.
+00000e20: 4a00 6402 7c05 9b00 9d02 8301 8201 7c05  J.d.|.........|.
+00000e30: 6403 1900 7d06 7c05 6404 1900 7d07 7c06  d...}.|.d...}.|.
+00000e40: 4400 5d32 7d08 7402 a003 7c08 a101 7d09  D.]2}.t...|...}.
+00000e50: 7c09 6a04 6403 1900 6403 1900 7d0a 7c0a  |.j.d...d...}.|.
+00000e60: 6405 6b02 7342 4a00 6406 7c0a 9b00 9d02  d.k.sBJ.d.|.....
+00000e70: 8301 8201 7142 7c07 4400 5d32 7d0b 7402  ....qB|.D.]2}.t.
+00000e80: a003 7c0b a101 7d09 7c09 6a04 6403 1900  ..|...}.|.j.d...
+00000e90: 6403 1900 7d0a 7c0a 6405 6b02 737a 4a00  d...}.|.d.k.szJ.
+00000ea0: 6406 7c0a 9b00 9d02 8301 8201 717a 7c05  d.|.........qz|.
+00000eb0: 6407 1900 7c03 7c04 3c00 7c05 6400 6407  d...|.|.<.|.d.d.
+00000ec0: 8502 1900 7c02 7c04 3c00 710c 7405 7c02  ....|.|.<.q.t.|.
+00000ed0: 7406 7c00 6a07 6408 8d03 7d0c 7c0c 6a08  t.|.j.d...}.|.j.
+00000ee0: 7c01 6409 640a 8d02 7d0d 7c0d 4400 5d9e  |.d.d...}.|.D.].
+00000ef0: 5c03 7d0e 7d04 7d0f 640b 7c0e 6901 7d10  \.}.}.}.d.|.i.}.
+00000f00: 7c03 7c04 1900 7d11 7400 7c11 8301 4400  |.|...}.t.|...D.
+00000f10: 5d7a 5c02 7d12 7d13 7c0f 7c12 1900 7d14  ]z\.}.}.|.|...}.
+00000f20: 6900 7d15 7c14 6a09 6409 640c 8d01 4400  i.}.|.j.d.d...D.
+00000f30: 5d30 5c02 7d16 7d17 7c17 640d 1900 7d18  ]0\.}.}.|.d...}.
+00000f40: 640e 7c17 7600 9001 7252 7c17 640e 1900  d.|.v...rR|.d...
+00000f50: 6e06 7c17 640f 1900 7c15 7c18 3c00 9001  n.|.d...|.|.<...
+00000f60: 7130 7c13 a00a a100 4400 5d16 5c02 7d19  q0|.....D.].\.}.
+00000f70: 7d1a 7c15 7c1a 1900 7c10 7c19 3c00 9001  }.|.|...|.|.<...
+00000f80: 716a 7c10 5600 0100 9001 7110 71ee 6400  qj|.V.....q.q.d.
+00000f90: 5300 2910 4ee9 0400 0000 7a2a 4665 6174  S.).N.....z*Feat
+00000fa0: 7572 6520 6d75 7374 2062 6520 6120 342d  ure must be a 4-
+00000fb0: 7475 706c 6520 666f 7220 4f70 656e 4945  tuple for OpenIE
+00000fc0: 2c20 6e6f 7420 7201 0000 0072 2e00 0000  , not r....r....
+00000fd0: 5a03 755f 307a 1f54 6865 2049 4473 206d  Z.u_0z.The IDs m
+00000fe0: 7573 7420 7374 6172 7420 6672 6f6d 2030  ust start from 0
+00000ff0: 2c20 6e6f 7420 e903 0000 00a9 02da 0963  , not .........c
+00001000: 6f6e 7665 7274 6572 723b 0000 0054 a901  onverterr;...T..
+00001010: da10 7265 7475 726e 5f73 7562 6772 6170  ..return_subgrap
+00001020: 6873 da08 7265 6c61 7469 6f6e a901 da04  hs..relation....
+00001030: 6461 7461 da07 6d61 7070 696e 67da 0665  data..mapping..e
+00001040: 6e74 6974 79da 046e 616d 6529 0bda 0965  ntity..name)...e
+00001050: 6e75 6d65 7261 7465 da03 6c65 6eda 0270  numerate..len..p
+00001060: 6eda 0664 6563 6f64 65da 0774 7269 706c  n..decode..tripl
+00001070: 6573 7205 0000 0072 0700 0000 723b 0000  esr....r....r;..
+00001080: 00da 056d 6174 6368 da05 6e6f 6465 73da  ...match..nodes.
+00001090: 0569 7465 6d73 291b 721a 0000 00da 0567  .items).r......g
+000010a0: 7261 7068 da08 6665 6174 7572 6573 5a17  raph..featuresZ.
+000010b0: 6665 6174 7572 655f 746f 5f6d 6172 6b65  feature_to_marke
+000010c0: 645f 6e6f 6465 73da 0169 da07 6665 6174  d_nodes..i..feat
+000010d0: 7572 655a 1170 6f73 6974 6976 655f 6665  ureZ.positive_fe
+000010e0: 6174 7572 6573 5a11 6e65 6761 7469 7665  aturesZ.negative
+000010f0: 5f66 6561 7475 7265 73da 0870 6f73 6974  _features..posit
+00001100: 6976 65da 0170 da05 6669 7273 74da 086e  ive..p..first..n
+00001110: 6567 6174 6976 6572 1300 0000 da05 6665  egativer......fe
+00001120: 6174 73da 036b 6579 da09 7375 6267 7261  ats..key..subgra
+00001130: 7068 73da 0774 7269 706c 6574 da0c 6d61  phs..triplet..ma
+00001140: 726b 6564 5f6e 6f64 6573 da01 6ada 046e  rked_nodes..j..n
+00001150: 6f64 65da 0873 7562 6772 6170 685a 0c6e  ode..subgraphZ.n
+00001160: 6f64 655f 746f 5f6e 6f64 65da 0269 645a  ode_to_node..idZ
+00001170: 0a67 7261 7068 5f6e 6f64 6572 4500 0000  .graph_noderE...
+00001180: da01 6bda 0176 721b 0000 0072 1b00 0000  ..k..vr....r....
+00001190: 721c 0000 00da 0861 6e6e 6f74 6174 6593  r......annotate.
+000011a0: 0000 0073 4a00 0000 0001 0402 1002 0aff  ...sJ...........
+000011b0: 0402 08fe 0404 0801 0802 0801 0a01 0e01  ................
+000011c0: 1802 0801 0a01 0e01 1802 0c01 1202 0201  ................
+000011d0: 08ff 0603 0e02 0e01 0801 0801 1001 0802  ................
+000011e0: 0401 1401 0803 06ff 0c02 06fd 0a06 1001  ................
+000011f0: 1002 7a19 4665 6174 7572 6545 7661 6c75  ..z.FeatureEvalu
+00001200: 6174 6f72 2e61 6e6e 6f74 6174 6563 0300  ator.annotatec..
+00001210: 0000 0000 0000 0000 0000 0800 0000 0500  ................
+00001220: 0000 4300 0000 734c 0000 007c 016a 00a0  ..C...sL...|.j..
+00001230: 01a1 007d 0367 007d 047c 0344 005d 1e7d  ...}.g.}.|.D.].}
+00001240: 057c 00a0 027c 057c 02a1 027d 067c 04a0  .|...|.|...}.|..
+00001250: 0374 047c 0683 01a1 0101 0071 127c 016a  .t.|.......q.|.j
+00001260: 05a0 01a1 007c 0464 019c 027d 0774 06a0  .....|.d...}.t..
+00001270: 077c 07a1 0153 0029 024e 2902 da08 5365  .|...S.).N)...Se
+00001280: 6e74 656e 6365 5a08 5472 6970 6c65 7473  ntenceZ.Triplets
+00001290: 2908 7250 0000 00da 0674 6f6c 6973 7472  ).rP.....tolistr
+000012a0: 6300 0000 da06 6170 7065 6e64 7230 0000  c.....appendr0..
+000012b0: 00da 0474 6578 74da 0270 64da 0944 6174  ...text..pd..Dat
+000012c0: 6146 7261 6d65 2908 721a 0000 00da 0764  aFrame).r......d
+000012d0: 6174 6173 6574 7251 0000 00da 0667 7261  atasetrQ.....gra
+000012e0: 7068 73da 0874 7269 706c 6574 7372 5000  phs..tripletsrP.
+000012f0: 0000 5a09 7265 6c61 7469 6f6e 73da 0164  ..Z.relations..d
+00001300: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
+00001310: 1261 6e6e 6f74 6174 655f 6461 7461 6672  .annotate_datafr
+00001320: 616d 65c4 0000 0073 1200 0000 0001 0a02  ame....s........
+00001330: 0401 0801 0c01 1002 0801 02fe 0605 7a23  ..............z#
+00001340: 4665 6174 7572 6545 7661 6c75 6174 6f72  FeatureEvaluator
+00001350: 2e61 6e6e 6f74 6174 655f 6461 7461 6672  .annotate_datafr
+00001360: 616d 6563 0700 0000 0000 0000 0000 0000  amec............
+00001370: 1100 0000 0900 0000 4300 0000 73a4 0000  ........C...s...
+00001380: 007c 016a 00a0 01a1 007d 0767 007d 0867  .|.j.....}.g.}.g
+00001390: 007d 0967 007d 0a7c 057c 0274 027c 006a  .}.g.}.|.|.t.|.j
+000013a0: 0364 018d 037d 0b74 0474 057c 0783 0183  .d...}.t.t.|....
+000013b0: 0144 005d 445c 027d 0c7d 0d7c 0b6a 067c  .D.]D\.}.}.|.j.|
+000013c0: 0d64 0264 038d 027d 0e7c 0372 647c 006a  .d.d...}.|.rd|.j
+000013d0: 077c 0e7c 027c 087c 097c 0a7c 0664 048d  .|.|.|.|.|.|.d..
+000013e0: 0601 0071 327c 00a0 087c 0e7c 027c 087c  ...q2|...|.|.|.|
+000013f0: 097c 0aa1 0501 0071 327c 016a 09a0 01a1  .|.....q2|.j....
+00001400: 007c 097c 0864 059c 037d 0f7c 0472 967c  .|.|.d...}.|.r.|
+00001410: 0a7c 0f64 063c 0074 0aa0 0b7c 0fa1 017d  .|.d.<.t...|...}
+00001420: 107c 1053 0029 074e 723e 0000 0054 7240  .|.S.).Nr>...Tr@
+00001430: 0000 0029 01da 1161 6c6c 6f77 5f6d 756c  ...)...allow_mul
+00001440: 7469 5f67 7261 7068 2903 7264 0000 007a  ti_graph).rd...z
+00001450: 0f50 7265 6469 6374 6564 206c 6162 656c  .Predicted label
+00001460: 7a0c 4d61 7463 6865 6420 7275 6c65 7a10  z.Matched rulez.
+00001470: 4d61 7463 6865 6420 7375 6267 7261 7068  Matched subgraph
+00001480: 290c 7250 0000 0072 6500 0000 7207 0000  ).rP...re...r...
+00001490: 0072 3b00 0000 7204 0000 0072 4800 0000  .r;...r....rH...
+000014a0: 724d 0000 00da 0b6d 6174 6368 5f6d 756c  rM.....match_mul
+000014b0: 7469 da0f 6d61 7463 685f 6e6f 745f 6d75  ti..match_not_mu
+000014c0: 6c74 6972 6700 0000 7268 0000 0072 6900  ltirg...rh...ri.
+000014d0: 0000 2911 721a 0000 0072 6a00 0000 7251  ..).r....rj...rQ
+000014e0: 0000 00da 056d 756c 7469 7241 0000 00da  .....multirA....
+000014f0: 0d67 7261 7068 5f6d 6174 6368 6572 726f  .graph_matcherro
+00001500: 0000 0072 6b00 0000 da07 6d61 7463 6865  ...rk.....matche
+00001510: 73da 0970 7265 6469 6374 6564 da0e 6d61  s..predicted..ma
+00001520: 7463 6865 645f 6772 6170 6873 7213 0000  tched_graphsr...
+00001530: 0072 5200 0000 7233 0000 0072 5800 0000  .rR...r3...rX...
+00001540: 726d 0000 00da 0264 6672 1b00 0000 721b  rm.....dfr....r.
+00001550: 0000 0072 1c00 0000 da0e 6d61 7463 685f  ...r......match_
+00001560: 6665 6174 7572 6573 d200 0000 733a 0000  features....s:..
+00001570: 0000 090a 0204 0104 0104 0202 0108 ff06  ................
+00001580: 0414 010e 0104 0104 0102 0102 0102 0102  ................
+00001590: 0102 0102 fa08 0904 010a ff06 0508 0102  ................
+000015a0: 0102 fd06 0504 0108 020a 017a 1f46 6561  ...........z.Fea
+000015b0: 7475 7265 4576 616c 7561 746f 722e 6d61  tureEvaluator.ma
+000015c0: 7463 685f 6665 6174 7572 6573 6307 0000  tch_featuresc...
+000015d0: 0000 0000 0000 0000 000d 0000 0005 0000  ................
+000015e0: 0043 0000 0073 9000 0000 6700 7d07 6700  .C...s....g.}.g.
+000015f0: 7d08 6700 7d09 7c01 4400 5d38 5c03 7d0a  }.g.}.|.D.]8\.}.
+00001600: 7d0b 7d0c 7c0a 7c07 7601 7326 7c06 7210  }.}.|.|.v.s&|.r.
+00001610: 7c08 a000 7c02 7c0b 1900 a101 0100 7c09  |...|.|.......|.
+00001620: a000 7c0c a101 0100 7c07 a000 7c0a a101  ..|.....|...|...
+00001630: 0100 7110 7c07 736e 7c03 a000 6401 a101  ..q.|.sn|...d...
+00001640: 0100 7c04 a000 6401 a101 0100 7c05 a000  ..|...d.....|...
+00001650: 6401 a101 0100 6e1e 7c03 a000 7c08 a101  d.....n.|...|...
+00001660: 0100 7c04 a000 7c07 a101 0100 7c05 a000  ..|...|.....|...
+00001670: 7c09 a101 0100 6400 5300 a902 4eda 00a9  |.....d.S...N...
+00001680: 0172 6600 0000 290d 721a 0000 0072 5800  .rf...).r....rX.
+00001690: 0000 7251 0000 0072 7400 0000 7275 0000  ..rQ...rt...ru..
+000016a0: 0072 7600 0000 726f 0000 00da 046b 6579  .rv...ro.....key
+000016b0: 735a 0d6d 6174 6368 6564 5f72 756c 6573  sZ.matched_rules
+000016c0: 5a11 6d61 7463 6865 645f 7375 6267 7261  Z.matched_subgra
+000016d0: 7068 7372 5900 0000 7253 0000 0072 6b00  phsrY...rS...rk.
+000016e0: 0000 721b 0000 0072 1b00 0000 721c 0000  ..r....r....r...
+000016f0: 0072 7000 0000 0001 0000 731e 0000 0000  .rp.......s.....
+00001700: 0904 0104 0104 010e 010c 010e 010a 010c  ................
+00001710: 0104 010a 010a 010c 020a 010a 017a 1c46  .............z.F
+00001720: 6561 7475 7265 4576 616c 7561 746f 722e  eatureEvaluator.
+00001730: 6d61 7463 685f 6d75 6c74 6963 0600 0000  match_multic....
+00001740: 0000 0000 0000 0000 0900 0000 0500 0000  ................
+00001750: 4300 0000 7358 0000 007c 0144 005d 305c  C...sX...|.D.]0\
+00001760: 037d 067d 077d 087c 03a0 007c 027c 0719  .}.}.}.|...|.|..
+00001770: 00a1 0101 007c 04a0 007c 06a1 0101 007c  .....|...|.....|
+00001780: 05a0 007c 08a1 0101 0001 0071 5471 047c  ...|.......qTq.|
+00001790: 03a0 0064 01a1 0101 007c 05a0 0064 01a1  ...d.....|...d..
+000017a0: 0101 007c 04a0 0064 01a1 0101 0064 0053  ...|...d.....d.S
+000017b0: 0072 7900 0000 727b 0000 0029 0972 1a00  .ry...r{...).r..
+000017c0: 0000 7258 0000 0072 5100 0000 7274 0000  ..rX...rQ...rt..
+000017d0: 0072 7500 0000 7276 0000 0072 5900 0000  .ru...rv...rY...
+000017e0: 7253 0000 0072 6b00 0000 721b 0000 0072  rS...rk...r....r
+000017f0: 1b00 0000 721c 0000 0072 7100 0000 1a01  ....r....rq.....
+00001800: 0000 7310 0000 0000 010e 010e 010a 010a  ..s.............
+00001810: 0106 020a 010a 017a 2046 6561 7475 7265  .......z Feature
+00001820: 4576 616c 7561 746f 722e 6d61 7463 685f  Evaluator.match_
+00001830: 6e6f 745f 6d75 6c74 6963 0300 0000 0000  not_multic......
+00001840: 0000 0000 0000 0400 0000 0300 0000 0300  ................
+00001850: 0000 732c 0000 007c 0264 0169 0189 007c  ..s,...|.d.i...|
+00001860: 01a0 00a1 007d 0387 0066 0164 0264 0384  .....}...f.d.d..
+00001870: 087c 016a 0144 0083 017c 0364 043c 007c  .|.j.D...|.d.<.|
+00001880: 0353 0029 054e 722e 0000 0063 0100 0000  .S.).Nr....c....
+00001890: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+000018a0: 1300 0000 7320 0000 0067 007c 005d 187d  ....s ...g.|.].}
+000018b0: 017c 0188 0076 0072 1888 007c 0119 006e  .|...v.r...|...n
+000018c0: 0264 0091 0271 0453 0029 0172 0100 0000  .d...q.S.).r....
+000018d0: 721b 0000 0029 02da 022e 30da 0469 7465  r....)....0..ite
+000018e0: 6da9 01da 066d 6170 7065 7272 1b00 0000  m....mapperr....
+000018f0: 721c 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
+00001900: 3e29 0100 0073 0200 0000 0601 7a34 4665  >)...s......z4Fe
+00001910: 6174 7572 6545 7661 6c75 6174 6f72 2e6f  atureEvaluator.o
+00001920: 6e65 5f76 6572 7375 735f 7265 7374 2e3c  ne_versus_rest.<
+00001930: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00001940: 703e da0f 6f6e 655f 7665 7273 7573 5f72  p>..one_versus_r
+00001950: 6573 7429 02da 0463 6f70 79da 056c 6162  est)...copy..lab
+00001960: 656c 2904 721a 0000 0072 7700 0000 7246  el).r....rw...rF
+00001970: 0000 005a 126f 6e65 5f76 6572 7375 735f  ...Z.one_versus_
+00001980: 7265 7374 5f64 6672 1b00 0000 727f 0000  rest_dfr....r...
+00001990: 0072 1c00 0000 7282 0000 0025 0100 0073  .r....r....%...s
+000019a0: 0c00 0000 0001 0802 0801 0a01 04ff 0a04  ................
+000019b0: 7a20 4665 6174 7572 6545 7661 6c75 6174  z FeatureEvaluat
+000019c0: 6f72 2e6f 6e65 5f76 6572 7375 735f 7265  or.one_versus_re
+000019d0: 7374 6305 0000 0000 0000 0000 0000 000b  stc.............
+000019e0: 0000 000c 0000 0003 0000 0073 9800 0000  ...........s....
+000019f0: 7c03 7d05 7c00 a000 7c01 8801 7c05 a103  |.}.|...|...|...
+00001a00: 5c02 8900 7d06 6700 7d07 7401 8801 8301  \...}.g.}.t.....
+00001a10: 4400 5d58 5c02 7d08 7d09 7c07 a002 7c09  D.]X\.}.}.|...|.
+00001a20: 8800 6a03 7c08 1900 6a04 8800 6a03 7c08  ..j.|...j...j.|.
+00001a30: 1900 6a05 8800 6a03 7c08 1900 6a06 8800  ..j...j.|...j...
+00001a40: 6a03 7c08 1900 6a07 7408 8800 6a03 7c08  j.|...j.t...j.|.
+00001a50: 1900 6a09 8301 7408 8800 6a03 7c08 1900  ..j...t...j.|...
+00001a60: 6a0a 8301 6607 a101 0100 7122 8700 8701  j...f.....q"....
+00001a70: 6602 6401 6402 8408 7d0a 740b 7c07 7c0a  f.d.d...}.t.|.|.
+00001a80: 6403 6404 8d03 5300 2905 4e63 0100 0000  d.d...S.).Nc....
+00001a90: 0000 0000 0000 0000 0100 0000 0600 0000  ................
+00001aa0: 1300 0000 731a 0000 0074 0088 006a 0188  ....s....t...j..
+00001ab0: 01a0 027c 0064 0119 00a1 0119 006a 0383  ...|.d.......j..
+00001ac0: 0153 0029 024e 7201 0000 0029 0472 4900  .S.).Nr....).rI.
+00001ad0: 0000 da04 696c 6f63 da05 696e 6465 78da  ....iloc..index.
+00001ae0: 1454 7275 655f 706f 7369 7469 7665 5f67  .True_positive_g
+00001af0: 7261 7068 7329 0172 5300 0000 a902 7277  raphs).rS.....rw
+00001b00: 0000 0072 5100 0000 721b 0000 0072 1c00  ...rQ...r....r..
+00001b10: 0000 da04 7261 6e6b 4701 0000 7302 0000  ....rankG...s...
+00001b20: 0000 017a 2c46 6561 7475 7265 4576 616c  ...z,FeatureEval
+00001b30: 7561 746f 722e 7261 6e6b 5f66 6561 7475  uator.rank_featu
+00001b40: 7265 732e 3c6c 6f63 616c 733e 2e72 616e  res.<locals>.ran
+00001b50: 6b54 2902 7259 0000 00da 0772 6576 6572  kT).rY.....rever
+00001b60: 7365 290c da10 6576 616c 7561 7465 5f66  se)...evaluate_f
+00001b70: 6561 7475 7265 7248 0000 0072 6600 0000  eaturerH...rf...
+00001b80: 7285 0000 00da 0950 7265 6369 7369 6f6e  r......Precision
+00001b90: da06 5265 6361 6c6c da06 4673 636f 7265  ..Recall..Fscore
+00001ba0: da07 5375 7070 6f72 7472 4900 0000 da12  ..SupportrI.....
+00001bb0: 5472 7565 5f70 6f73 6974 6976 655f 7365  True_positive_se
+00001bc0: 6e73 da13 4661 6c73 655f 706f 7369 7469  ns..False_positi
+00001bd0: 7665 5f73 656e 73da 0673 6f72 7465 6429  ve_sens..sorted)
+00001be0: 0b72 1a00 0000 da02 636c 7251 0000 005a  .r......clrQ...Z
+00001bf0: 096f 7269 675f 6461 7461 5a0f 6661 6c73  .orig_dataZ.fals
+00001c00: 655f 6e65 6761 7469 7665 735a 0b73 7562  e_negativesZ.sub
+00001c10: 7365 745f 6461 7461 da08 6163 6375 7261  set_data..accura
+00001c20: 6379 5a0d 6665 6174 7572 6573 5f73 7461  cyZ.features_sta
+00001c30: 7472 5200 0000 7253 0000 0072 8900 0000  trR...rS...r....
+00001c40: 721b 0000 0072 8800 0000 721c 0000 00da  r....r....r.....
+00001c50: 0d72 616e 6b5f 6665 6174 7572 6573 2f01  .rank_features/.
+00001c60: 0000 7320 0000 0000 0604 0112 0204 0210  ..s ............
+00001c70: 0104 0202 010a 010a 010a 010a 010e 010e  ................
+00001c80: f902 ff06 0c0e 037a 1e46 6561 7475 7265  .......z.Feature
+00001c90: 4576 616c 7561 746f 722e 7261 6e6b 5f66  Evaluator.rank_f
+00001ca0: 6561 7475 7265 7363 0500 0000 0000 0000  eaturesc........
+00001cb0: 0000 0000 2100 0000 0e00 0000 4300 0000  ....!.......C...
+00001cc0: 73c0 0200 0074 007c 0267 0167 0067 0067  s....t.|.g.g.g.g
+00001cd0: 0367 0174 017c 006a 0264 018d 037d 057c  .g.t.|.j.d...}.|
+00001ce0: 056a 0364 0219 0064 0219 007d 0674 047c  .j.d...d...}.t.|
+00001cf0: 0664 0219 0074 0583 0272 7074 067c 0664  .d...t...rpt.|.d
+00001d00: 0219 0064 0319 0083 0164 046b 0272 5c7c  ...d.....d.k.r\|
+00001d10: 0664 0219 0064 0319 005c 027d 077d 0871  .d...d...\.}.}.q
+00001d20: 7e7c 0664 0219 0064 0319 005c 037d 097d  ~|.d...d...\.}.}
+00001d30: 077d 086e 0e7c 0664 0219 0064 0002 007d  .}.n.|.d...d...}
+00001d40: 077d 087c 036a 07a0 08a1 007d 0a7c 00a0  .}.|.j.....}.|..
+00001d50: 097c 037c 01a1 026a 09a0 08a1 007d 0b64  .|.|...j.....}.d
+00001d60: 057d 0c67 007d 0d74 0a7c 0c64 0683 0290  .}.g.}.t.|.d....
+00001d70: 018f f67d 0e74 0b7c 0a83 0144 0090 015d  ...}.t.|...D...]
+00001d80: da5c 027d 0f7d 1064 0764 0884 007c 056a  .\.}.}.d.d...|.j
+00001d90: 0c7c 1064 0964 0a8d 0244 0083 017d 117c  .|.d.d...D...}.|
+00001da0: 1144 0090 015d b25c 027d 127d 137c 1344  .D...].\.}.}.|.D
+00001db0: 0090 015d a27d 1467 007d 157c 146a 0d64  ...].}.g.}.|.j.d
+00001dc0: 0964 0b8d 0144 005d 865c 027d 167d 177c  .d...D.].\.}.}.|
+00001dd0: 1590 0173 027c 1764 0c19 007d 187c 1764  ...s.|.d...}.|.d
+00001de0: 0d19 007c 076a 0d76 0090 0172 4a7c 076a  ...|.j.v...rJ|.j
+00001df0: 0d7c 1764 0d19 0019 0064 0c19 0064 0e6b  .|.d.....d...d.k
+00001e00: 0290 0172 4a7c 15a0 0e7c 18a1 0101 007c  ...rJ|...|.....|
+00001e10: 0864 0075 0190 0172 027c 1764 0d19 007c  .d.u...r.|.d...|
+00001e20: 086a 0d76 0090 0172 027c 086a 0d7c 1764  .j.v...r.|.j.|.d
+00001e30: 0d19 0019 0064 0c19 0064 0e6b 0290 0172  .....d...d.k...r
+00001e40: 027c 15a0 0e7c 18a1 0101 0090 0171 027c  .|...|.......q.|
+00001e50: 1590 0273 3a64 0f64 1084 007c 146a 0f64  ...s:d.d...|.j.d
+00001e60: 0964 0b8d 0144 0083 017d 197c 076a 0f64  .d...D...}.|.j.d
+00001e70: 0964 0b8d 0144 005d 3c5c 037d 1a7d 1b7d  .d...D.]<\.}.}.}
+00001e80: 1c7c 1c64 1119 0064 0e6b 0290 0172 b27c  .|.d...d.k...r.|
+00001e90: 10a0 107c 197c 1a19 007c 197c 1b19 00a1  ...|.|...|.|....
+00001ea0: 0264 1119 007d 1d7c 15a0 0e7c 1da1 0101  .d...}.|...|....
+00001eb0: 0090 0171 b27c 086a 0f64 0964 0b8d 0144  ...q.|.j.d.d...D
+00001ec0: 005d 3c5c 037d 1a7d 1b7d 1c7c 1c64 1119  .]<\.}.}.}.|.d..
+00001ed0: 0064 0e6b 0290 0172 fc7c 10a0 107c 197c  .d.k...r.|...|.|
+00001ee0: 1a19 007c 197c 1b19 00a1 0264 1119 007d  ...|.|.....d...}
+00001ef0: 1d7c 15a0 0e7c 1da1 0101 0090 0171 fc64  .|...|.......q.d
+00001f00: 12a0 117c 15a1 017d 1e7c 0b7c 0f19 007d  ...|...}.|.|...}
+00001f10: 1f7c 036a 127c 0f19 006a 137d 207c 0ea0  .|.j.|...j.} |..
+00001f20: 147c 029b 0064 137c 1e9b 0064 137c 209b  .|...d.|...d.| .
+00001f30: 0064 137c 1f9b 0064 149d 08a1 0101 007c  .d.|...d.......|
+00001f40: 0da0 0e7c 027c 1e7c 2074 157c 1f83 0166  ...|.|.| t.|...f
+00001f50: 04a1 0101 0071 ec71 de71 b857 0064 0004  .....q.q.q.W.d..
+00001f60: 0004 0083 0301 006e 1231 0090 0273 ac30  .......n.1...s.0
+00001f70: 0001 0001 0001 0059 0001 007c 00a0 167c  .......Y...|...|
+00001f80: 0da1 0153 0029 154e 2901 723b 0000 0072  ...S.).N).r;...r
+00001f90: 0100 0000 722e 0000 00e9 0200 0000 7a14  ....r.........z.
+00001fa0: 7472 6169 6e65 645f 6665 6174 7572 6573  trained_features
+00001fb0: 2e74 7376 7a02 772b 6301 0000 0000 0000  .tsvz.w+c.......
+00001fc0: 0000 0000 0004 0000 0005 0000 0053 0000  .............S..
+00001fd0: 0073 1a00 0000 6700 7c00 5d12 5c03 7d01  .s....g.|.].\.}.
+00001fe0: 7d02 7d03 7c02 7c03 6602 9102 7104 5300  }.}.|.|.f...q.S.
+00001ff0: 721b 0000 0072 1b00 0000 2904 727d 0000  r....r....).r}..
+00002000: 0072 5900 0000 7252 0000 0072 5f00 0000  .rY...rR...r_...
+00002010: 721b 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+00002020: 8100 0000 6101 0000 7304 0000 0006 0208  ....a...s.......
+00002030: ff7a 3246 6561 7475 7265 4576 616c 7561  .z2FeatureEvalua
+00002040: 746f 722e 7472 6169 6e5f 6665 6174 7572  tor.train_featur
+00002050: 652e 3c6c 6f63 616c 733e 2e3c 6c69 7374  e.<locals>.<list
+00002060: 636f 6d70 3e54 7240 0000 0072 4300 0000  comp>Tr@...rC...
+00002070: 7247 0000 0072 4500 0000 fa02 2e2a 6301  rG...rE......*c.
+00002080: 0000 0000 0000 0000 0000 0004 0000 0005  ................
+00002090: 0000 0053 0000 0073 1800 0000 6900 7c00  ...S...s....i.|.
+000020a0: 5d10 5c03 7d01 7d02 7d03 7c02 7c01 9302  ].\.}.}.}.|.|...
+000020b0: 7104 5300 721b 0000 0072 1b00 0000 2904  q.S.r....r....).
+000020c0: 727d 0000 00da 0175 7262 0000 00da 015f  r}.....urb....._
+000020d0: 721b 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
+000020e0: 0a3c 6469 6374 636f 6d70 3e79 0100 00f3  .<dictcomp>y....
+000020f0: 0000 0000 7a32 4665 6174 7572 6545 7661  ....z2FeatureEva
+00002100: 6c75 6174 6f72 2e74 7261 696e 5f66 6561  luator.train_fea
+00002110: 7475 7265 2e3c 6c6f 6361 6c73 3e2e 3c64  ture.<locals>.<d
+00002120: 6963 7463 6f6d 703e da05 636f 6c6f 72fa  ictcomp>..color.
+00002130: 012c fa01 09da 010a 2917 7205 0000 0072  .,......).r....r
+00002140: 0700 0000 723b 0000 00da 0570 6174 7473  ....r;.....patts
+00002150: da0a 6973 696e 7374 616e 6365 da05 7475  ..isinstance..tu
+00002160: 706c 6572 4900 0000 7250 0000 0072 6500  plerI...rP...re.
+00002170: 0000 7282 0000 00da 046f 7065 6e72 4800  ..r......openrH.
+00002180: 0000 724d 0000 0072 4e00 0000 7266 0000  ..rM...rN...rf..
+00002190: 00da 0565 6467 6573 da0d 6765 745f 6564  ...edges..get_ed
+000021a0: 6765 5f64 6174 6172 0d00 0000 7285 0000  ge_datar....r...
+000021b0: 0072 6700 0000 da05 7772 6974 65da 0373  .rg.....write..s
+000021c0: 7472 da0f 636c 7573 7465 725f 6665 6174  tr..cluster_feat
+000021d0: 7572 6529 2172 1a00 0000 7293 0000 0072  ure)!r....r....r
+000021e0: 5300 0000 7244 0000 0072 3a00 0000 7273  S...rD...r:...rs
+000021f0: 0000 005a 0966 6561 745f 7061 7474 5a05  ...Z.feat_pattZ.
+00002200: 7061 7474 315a 0570 6174 7432 7299 0000  patt1Z.patt2r...
+00002210: 0072 6b00 0000 da06 6c61 6265 6c73 720c  .rk.....labelsr.
+00002220: 0000 00da 1074 7261 696e 6564 5f66 6561  .....trained_fea
+00002230: 7475 7265 73da 0166 7252 0000 0072 3300  tures..frR...r3.
+00002240: 0000 7274 0000 005a 0a70 6174 745f 696e  ..rt...Z.patt_in
+00002250: 6465 7872 4d00 0000 7250 0000 0072 4e00  dexrM...rP...rN.
+00002260: 0000 da0a 6e6f 6465 5f69 6e64 6578 725e  ....node_indexr^
+00002270: 0000 00da 096e 6f64 655f 6e61 6d65 5a08  .....node_nameZ.
+00002280: 6732 5f74 6f5f 6731 7298 0000 0072 6200  g2_to_g1r....rb.
+00002290: 0000 da05 6174 7472 73da 0465 6467 655a  ....attrs..edgeZ
+000022a0: 096e 6f64 6573 5f73 7472 7284 0000 00da  .nodes_strr.....
+000022b0: 0873 656e 7465 6e63 6572 1b00 0000 721b  .sentencer....r.
+000022c0: 0000 0072 1c00 0000 da0d 7472 6169 6e5f  ...r......train_
+000022d0: 6665 6174 7572 654c 0100 0073 7c00 0000  featureL...s|...
+000022e0: 0001 0201 0c01 0201 04fd 0605 0e01 0e01  ................
+000022f0: 1401 1202 1402 0e02 0a01 1201 0401 0401  ................
+00002300: 0e01 1201 0602 0401 04ff 04fe 0606 0e01  ................
+00002310: 0a01 0401 1401 0601 0802 0cff 0402 14fe  ................
+00002320: 0404 0a02 06ff 0402 0cfe 0403 14fd 0405  ................
+00002330: 0e01 0601 1601 1601 0e01 1201 02ff 0403  ................
+00002340: 0e01 1601 0e01 1201 02ff 0403 0e01 0a01  ................
+00002350: 0801 0c01 2201 0401 0eff 2a04 7a1e 4665  ....".....*.z.Fe
+00002360: 6174 7572 6545 7661 6c75 6174 6f72 2e74  atureEvaluator.t
+00002370: 7261 696e 5f66 6561 7475 7265 6302 0000  rain_featurec...
+00002380: 0000 0000 0000 0000 0011 0000 0008 0000  ................
+00002390: 0043 0000 0073 3e01 0000 6900 7d02 7400  .C...s>...i.}.t.
+000023a0: 6a01 a002 6401 a101 7242 7403 6402 8301  j...d...rBt.d...
+000023b0: 8f1a 7d03 7404 a005 7c03 a101 7d02 5700  ..}.t...|...}.W.
+000023c0: 6400 0400 0400 8303 0100 6e10 3100 7338  d.........n.1.s8
+000023d0: 3000 0100 0100 0100 5900 0100 6900 7d04  0.......Y...i.}.
+000023e0: 7c01 4400 5d2c 7d05 7406 7c05 6403 1900  |.D.],}.t.|.d...
+000023f0: 8301 7c04 7c05 6404 1900 6405 1700 7c05  ..|.|.d...d...|.
+00002400: 6403 1900 1700 3c00 7c05 6406 1900 7d06  d.....<.|.d...}.
+00002410: 714a 7407 a008 a100 7d07 7c04 4400 5d7a  qJt.....}.|.D.]z
+00002420: 7d08 7c04 7c08 1900 6404 6b02 729a 6407  }.|.|...d.k.r.d.
+00002430: 7d09 6e04 6408 7d09 7c07 6a09 7c08 7c09  }.n.d.}.|.j.|.|.
+00002440: 6409 8d02 0100 7c08 a00a 6405 a101 6406  d.....|...d...d.
+00002450: 1900 7d0a 7c0a 7c02 7600 7284 7c02 7c0a  ..}.|.|.v.r.|.|.
+00002460: 1900 7d0b 7c0b 4400 5d2e 7d0c 7c0b 7c0c  ..}.|.D.].}.|.|.
+00002470: 1900 7d0d 7c0d 4400 5d1c 7d0e 7c0c 640a  ..}.|.D.].}.|.d.
+00002480: 6b02 72de 7c07 6a0b 7c08 7c0e 7c0c 6409  k.r.|.j.|.|.|.d.
+00002490: 8d03 0100 71de 71ce 7184 7c00 a00c 7c01  ....q.q.q.|...|.
+000024a0: a101 7d0f 6700 7d10 7c0f 9001 7230 7c10  ..}.g.}.|...r0|.
+000024b0: a00d 7c06 a00e 640b 640c a00f 7c0f a101  ..|...d.d...|...
+000024c0: 6404 a103 a101 0100 6e0a 7c10 a00d 7c06  d.......n.|...|.
+000024d0: a101 0100 7c10 5300 290d 4e5a 1a6c 6f6e  ....|.S.).NZ.lon
+000024e0: 676d 616e 5f7a 6572 6f5f 7061 7468 735f  gman_zero_paths_
+000024f0: 6f6e 655f 6578 707a 1f6c 6f6e 676d 616e  one_expz.longman
+00002500: 5f7a 6572 6f5f 7061 7468 735f 6f6e 655f  _zero_paths_one_
+00002510: 6578 702e 6a73 6f6e 723d 0000 0072 2e00  exp.jsonr=...r..
+00002520: 0000 7299 0000 0072 0100 0000 da05 6772  ..r....r......gr
+00002530: 6565 6eda 0372 6564 2901 729c 0000 00da  een..red).r.....
+00002540: 0131 7297 0000 00da 017c 2910 720b 0000  .1r......|).r...
+00002550: 0072 0c00 0000 da06 6973 6669 6c65 72a3  .r......isfiler.
+00002560: 0000 00da 046a 736f 6eda 046c 6f61 64da  .....json..load.
+00002570: 0369 6e74 da02 6e78 da0c 4d75 6c74 6944  .int..nx..MultiD
+00002580: 6947 7261 7068 da08 6164 645f 6e6f 6465  iGraph..add_node
+00002590: da05 7370 6c69 74da 0861 6464 5f65 6467  ..split..add_edg
+000025a0: 65da 0c73 656c 6563 745f 776f 7264 7372  e..select_wordsr
+000025b0: 6600 0000 da07 7265 706c 6163 6572 0d00  f.....replacer..
+000025c0: 0000 2911 721a 0000 0072 aa00 0000 726b  ..).r....r....rk
+000025d0: 0000 0072 ab00 0000 da05 776f 7264 73da  ...r......words.
+000025e0: 0666 6965 6c64 7372 5300 0000 7250 0000  .fieldsrS...rP..
+000025f0: 00da 0477 6f72 6472 9c00 0000 5a0a 776f  ...wordr....Z.wo
+00002600: 7264 5f63 6c65 616e 5a09 6879 7065 726e  rd_cleanZ.hypern
+00002610: 796d 735a 0868 7970 6572 6e79 6d5a 0e68  ymsZ.hypernymZ.h
+00002620: 7970 6572 6e79 6d5f 776f 7264 73da 0177  ypernym_words..w
+00002630: da0e 7365 6c65 6374 6564 5f77 6f72 6473  ..selected_words
+00002640: 5a0d 776f 7264 5f66 6561 7475 7265 7372  Z.word_featuresr
+00002650: 1b00 0000 721b 0000 0072 1c00 0000 72a8  ....r....r....r.
+00002660: 0000 0090 0100 0073 3800 0000 0001 0401  .......s8.......
+00002670: 0c01 0a01 2802 0401 0801 2001 0a01 0802  ....(..... .....
+00002680: 0801 0c01 0602 0401 0e01 0e01 0801 0801  ................
+00002690: 0801 0801 0801 0801 1602 0a02 0402 0601  ................
+000026a0: 1c02 0a02 7a20 4665 6174 7572 6545 7661  ....z FeatureEva
+000026b0: 6c75 6174 6f72 2e63 6c75 7374 6572 5f66  luator.cluster_f
+000026c0: 6561 7475 7265 6302 0000 0000 0000 0000  eaturec.........
+000026d0: 0000 0010 0000 0006 0000 0043 0000 0073  ...........C...s
+000026e0: b001 0000 6700 7d02 6700 7d03 7c01 4400  ....g.}.g.}.|.D.
+000026f0: 5d24 7d04 7c02 a000 7c04 6401 1900 a101  ]$}.|...|.d.....
+00002700: 0100 7c03 a000 7401 7c04 6402 1900 8301  ..|...t.|.d.....
+00002710: a101 0100 710c 6403 6404 8400 7402 7c02  ....q.d.d...t.|.
+00002720: 8301 4400 8301 7d05 7c05 4400 5da6 7d06  ..D...}.|.D.].}.
+00002730: 7403 7c03 8301 4400 5d98 5c02 7d07 7d08  t.|...D.].\.}.}.
+00002740: 7c08 7280 7c02 7c07 1900 7c06 6b02 7280  |.r.|.|...|.k.r.
+00002750: 7c05 7c06 1900 6405 0500 1900 6401 3700  |.|...d.....d.7.
+00002760: 0300 3c00 7c08 72a4 7c02 7c07 1900 7c06  ..<.|.r.|.|...|.
+00002770: 6b03 72a4 7c05 7c06 1900 6406 0500 1900  k.r.|.|...d.....
+00002780: 6401 3700 0300 3c00 7c08 73c8 7c02 7c07  d.7...<.|.s.|.|.
+00002790: 1900 7c06 6b02 72c8 7c05 7c06 1900 6407  ..|.k.r.|.|...d.
+000027a0: 0500 1900 6401 3700 0300 3c00 7c08 7354  ....d.7...<.|.sT
+000027b0: 7c02 7c07 1900 7c06 6b03 7254 7c05 7c06  |.|...|.k.rT|.|.
+000027c0: 1900 6408 0500 1900 6401 3700 0300 3c00  ..d.....d.7...<.
+000027d0: 7154 7148 7c05 4400 5d64 7d06 7c05 7c06  qTqH|.D.]d}.|.|.
+000027e0: 1900 6405 1900 7d09 7c05 7c06 1900 6407  ..d...}.|.|...d.
+000027f0: 1900 7d0a 7c05 7c06 1900 6408 1900 7d0b  ..}.|.|...d...}.
+00002800: 7c05 7c06 1900 6406 1900 7d0c 7c09 7c09  |.|...d...}.|.|.
+00002810: 7c0a 1700 1b00 7d0d 7c09 7c09 7c0c 1700  |.....}.|.|.|...
+00002820: 1b00 7d0e 7c0d 7c05 7c06 1900 6409 3c00  ..}.|.|.|...d.<.
+00002830: 7c0e 7c05 7c06 1900 640a 3c00 71f4 7402  |.|.|...d.<.q.t.
+00002840: 8300 7d0f 7c05 4400 5d46 7d06 7c05 7c06  ..}.|.D.]F}.|.|.
+00002850: 1900 6409 1900 640b 6b04 9001 7264 7c05  ..d...d.k...rd|.
+00002860: 7c06 1900 6405 1900 6401 6b04 9001 739e  |...d...d.k...s.
+00002870: 7c05 7c06 1900 640a 1900 640c 6b04 9001  |.|...d...d.k...
+00002880: 7264 7c0f a004 7c06 a101 0100 9001 7164  rd|...|.......qd
+00002890: 7c0f 5300 290d 4e72 2e00 0000 723d 0000  |.S.).Nr....r=..
+000028a0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+000028b0: 0000 0800 0000 5300 0000 731c 0000 0069  ......S...s....i
+000028c0: 007c 005d 147d 017c 0164 0064 0064 0064  .|.].}.|.d.d.d.d
+000028d0: 0064 019c 0493 0271 0453 0029 0272 0100  .d.....q.S.).r..
+000028e0: 0000 2904 da02 5450 da02 4650 da02 544e  ..)...TP..FP..TN
+000028f0: da02 464e 721b 0000 0029 0272 7d00 0000  ..FNr....).r}...
+00002900: 72c3 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
+00002910: 1c00 0000 729a 0000 00bd 0100 0073 0200  ....r........s..
+00002920: 0000 0601 7a31 4665 6174 7572 6545 7661  ....z1FeatureEva
+00002930: 6c75 6174 6f72 2e73 656c 6563 745f 776f  luator.select_wo
+00002940: 7264 732e 3c6c 6f63 616c 733e 2e3c 6469  rds.<locals>.<di
+00002950: 6374 636f 6d70 3e72 c600 0000 72c9 0000  ctcomp>r....r...
+00002960: 0072 c700 0000 72c8 0000 00da 0970 7265  .r....r......pre
+00002970: 6369 7369 6f6e da06 7265 6361 6c6c 67cd  cision..recallg.
+00002980: cccc cccc ccec 3f67 7b14 ae47 e17a 843f  ......?g{..G.z.?
+00002990: 2905 7266 0000 0072 b900 0000 da03 7365  ).rf...r......se
+000029a0: 7472 4800 0000 da03 6164 6429 1072 1a00  trH.....add).r..
+000029b0: 0000 72aa 0000 0072 5100 0000 72a9 0000  ..r....rQ...r...
+000029c0: 0072 c200 0000 5a11 776f 7264 735f 746f  .r....Z.words_to
+000029d0: 5f6d 6561 7375 7265 7372 c300 0000 7252  _measuresr....rR
+000029e0: 0000 0072 8400 0000 72c6 0000 0072 c700  ...r....r....r..
+000029f0: 0000 72c8 0000 0072 c900 0000 72ca 0000  ..r....r....r...
+00002a00: 0072 cb00 0000 72c5 0000 0072 1b00 0000  .r....r....r....
+00002a10: 721b 0000 0072 1c00 0000 72bf 0000 00b6  r....r....r.....
+00002a20: 0100 0073 4800 0000 0001 0401 0402 0801  ...sH...........
+00002a30: 0e01 1401 0601 06ff 0603 0801 1001 1001  ................
+00002a40: 1401 1001 1401 1001 1401 1001 1802 0801  ................
+00002a50: 0c01 0c01 0c01 0c02 0c01 0c02 0c01 0e02  ................
+00002a60: 0602 0801 1201 0eff 0402 0efe 0404 0e02  ................
+00002a70: 7a1d 4665 6174 7572 6545 7661 6c75 6174  z.FeatureEvaluat
+00002a80: 6f72 2e73 656c 6563 745f 776f 7264 7363  or.select_wordsc
+00002a90: 0600 0000 0000 0000 0000 0000 2300 0000  ............#...
+00002aa0: 0600 0000 4300 0000 7302 0300 0067 007d  ....C...s....g.}
+00002ab0: 067c 036a 00a0 01a1 007d 077c 00a0 027c  .|.j.....}.|...|
+00002ac0: 037c 01a1 026a 02a0 01a1 007d 0867 007d  .|...j.....}.g.}
+00002ad0: 0974 0374 0483 017d 0a67 007d 0b67 007d  .t.t...}.g.}.g.}
+00002ae0: 0c67 007d 0d7c 057c 0274 057c 006a 0664  .g.}.|.|.t.|.j.d
+00002af0: 018d 037d 0e74 077c 0783 0144 005d 965c  ...}.t.|...D.].\
+00002b00: 027d 0f7d 107c 0ea0 087c 10a1 017d 1164  .}.}.|...|...}.d
+00002b10: 027d 127c 1144 005d 225c 027d 137d 147c  .}.|.D.]"\.}.}.|
+00002b20: 0a7c 0f19 00a0 097c 027c 1419 0064 0219  .|.....|.|...d..
+00002b30: 00a1 0101 0064 037d 1271 6a7c 09a0 097c  .....d.}.qj|...|
+00002b40: 12a1 0101 007c 1264 026b 0272 507c 087c  .....|.d.k.rP|.|
+00002b50: 0f19 0064 036b 0272 507c 0ba0 097c 10a1  ...d.k.rP|...|..
+00002b60: 0101 007c 036a 0a7c 0f19 006a 0b7d 157c  ...|.j.|...j.}.|
+00002b70: 036a 0a7c 0f19 006a 0c7d 167c 0ca0 097c  .j.|...j.}.|...|
+00002b80: 157c 1666 02a1 0101 007c 0da0 097c 0fa1  .|.f.....|...|..
+00002b90: 0101 0071 5067 007d 1774 0d7c 087c 0964  ...qPg.}.t.|.|.d
+00002ba0: 0064 048d 0344 005d 2c7d 1874 0e7c 1883  .d...D.],}.t.|..
+00002bb0: 0164 036b 0490 0172 1c7c 17a0 097c 1864  .d.k...r.|...|.d
+00002bc0: 0319 00a1 0101 0071 fa7c 17a0 0964 02a1  .......q.|...d..
+00002bd0: 0101 0071 fa7c 0244 0090 015d b87d 197c  ...q.|.D...].}.|
+00002be0: 1964 0219 0067 017d 1a67 007d 1b67 007d  .d...g.}.g.}.g.}
+00002bf0: 1c67 007d 1d67 007d 1e67 007d 1f67 007d  .g.}.g.}.g.}.g.}
+00002c00: 2067 007d 2174 077c 0783 0144 005d d65c   g.}!t.|...D.].\
+00002c10: 027d 0f7d 107c 0a7c 0f19 007d 117c 1964  .}.}.|.|...}.|.d
+00002c20: 0219 007c 1176 0090 0172 8264 036e 0264  ...|.v...r.d.n.d
+00002c30: 027d 127c 1264 036b 0290 0172 d87c 087c  .}.|.d.k...r.|.|
+00002c40: 0f19 0064 026b 0290 0172 d87c 1ba0 097c  ...d.k...r.|...|
+00002c50: 10a1 0101 007c 036a 0a7c 0f19 006a 0b7d  .....|.j.|...j.}
+00002c60: 157c 036a 0a7c 0f19 006a 0c7d 167c 1ca0  .|.j.|...j.}.|..
+00002c70: 097c 157c 1666 02a1 0101 007c 1da0 097c  .|.|.f.....|...|
+00002c80: 0fa1 0101 007c 1264 036b 0290 0272 2a7c  .....|.d.k...r*|
+00002c90: 087c 0f19 0064 036b 0290 0272 2a7c 1ea0  .|...d.k...r*|..
+00002ca0: 097c 10a1 0101 007c 036a 0a7c 0f19 006a  .|.....|.j.|...j
+00002cb0: 0b7d 157c 036a 0a7c 0f19 006a 0c7d 167c  .}.|.j.|...j.}.|
+00002cc0: 1fa0 097c 157c 1666 02a1 0101 007c 20a0  ...|.|.f.....| .
+00002cd0: 097c 0fa1 0101 007c 21a0 097c 12a1 0101  .|.....|!..|....
+00002ce0: 0090 0171 6074 0d7c 087c 2164 0064 048d  ...q`t.|.|!d.d..
+00002cf0: 0344 005d 2e7d 1874 0e7c 1883 0164 036b  .D.].}.t.|...d.k
+00002d00: 0490 0272 687c 1aa0 097c 1864 0319 00a1  ...rh|...|.d....
+00002d10: 0101 006e 0a7c 1aa0 0964 02a1 0101 0090  ...n.|...d......
+00002d20: 0271 467c 1aa0 097c 1ba1 0101 007c 1aa0  .qF|...|.....|..
+00002d30: 097c 1ca1 0101 007c 1aa0 097c 1da1 0101  .|.....|...|....
+00002d40: 007c 1aa0 097c 1ea1 0101 007c 1aa0 097c  .|...|.....|...|
+00002d50: 1fa1 0101 007c 1aa0 097c 20a1 0101 007c  .....|...| ....|
+00002d60: 1aa0 097c 0ba1 0101 007c 1aa0 097c 0ca1  ...|.....|...|..
+00002d70: 0101 007c 1aa0 097c 0da1 0101 007c 1aa0  ...|...|.....|..
+00002d80: 097c 21a1 0101 007c 06a0 097c 1aa1 0101  .|!....|...|....
+00002d90: 0090 0171 2c74 0f6a 107c 0667 0064 05a2  ...q,t.j.|.g.d..
+00002da0: 0164 068d 027d 227c 227c 1766 0253 0029  .d...}"|"|.f.S.)
+00002db0: 074e 723e 0000 0072 0100 0000 722e 0000  .Nr>...r....r...
+00002dc0: 0029 01da 0761 7665 7261 6765 290f da07  .)...average)...
+00002dd0: 4665 6174 7572 6572 8c00 0000 728d 0000  Featurer....r...
+00002de0: 0072 8e00 0000 728f 0000 00da 1546 616c  .r....r......Fal
+00002df0: 7365 5f70 6f73 6974 6976 655f 6772 6170  se_positive_grap
+00002e00: 6873 7291 0000 00da 1646 616c 7365 5f70  hsr......False_p
+00002e10: 6f73 6974 6976 655f 696e 6469 6365 7372  ositive_indicesr
+00002e20: 8700 0000 7290 0000 00da 1554 7275 655f  ....r......True_
+00002e30: 706f 7369 7469 7665 5f69 6e64 6963 6573  positive_indices
+00002e40: da15 4661 6c73 655f 6e65 6761 7469 7665  ..False_negative
+00002e50: 5f67 7261 7068 73da 1346 616c 7365 5f6e  _graphs..False_n
+00002e60: 6567 6174 6976 655f 7365 6e73 da16 4661  egative_sens..Fa
+00002e70: 6c73 655f 6e65 6761 7469 7665 5f69 6e64  lse_negative_ind
+00002e80: 6963 6573 da09 5072 6564 6963 7465 6429  ices..Predicted)
+00002e90: 01da 0763 6f6c 756d 6e73 2911 7250 0000  ...columns).rP..
+00002ea0: 0072 6500 0000 7282 0000 0072 0200 0000  .re...r....r....
+00002eb0: 7230 0000 0072 0700 0000 723b 0000 0072  r0...r....r;...r
+00002ec0: 4800 0000 724d 0000 0072 6600 0000 7285  H...rM...rf...r.
+00002ed0: 0000 0072 6700 0000 7284 0000 0072 0300  ...rg...r....r..
+00002ee0: 0000 7249 0000 0072 6800 0000 7269 0000  ..rI...rh...ri..
+00002ef0: 0029 2372 1a00 0000 7293 0000 0072 5100  .)#r....r....rQ.
+00002f00: 0000 7244 0000 0072 3a00 0000 7273 0000  ..rD...r:...rs..
+00002f10: 005a 106d 6561 7375 7265 5f66 6561 7475  .Z.measure_featu
+00002f20: 7265 7372 6b00 0000 72a9 0000 005a 0f77  resrk...r....Z.w
+00002f30: 686f 6c65 5f70 7265 6469 6374 6564 5a07  hole_predictedZ.
+00002f40: 6d61 7463 6865 645a 0b66 616c 7365 5f6e  matchedZ.false_n
+00002f50: 6567 5f67 5a0b 6661 6c73 655f 6e65 675f  eg_gZ.false_neg_
+00002f60: 735a 1166 616c 7365 5f6e 6567 5f69 6e64  sZ.false_neg_ind
+00002f70: 6963 6573 7213 0000 0072 5200 0000 7233  icesr....rR...r3
+00002f80: 0000 0072 5800 0000 7284 0000 0072 5900  ...rX...r....rY.
+00002f90: 0000 7253 0000 0072 3200 0000 da03 6c61  ..rS...r2.....la
+00002fa0: 6272 9400 0000 5a03 7063 66da 0466 6561  br....Z.pcf..fea
+00002fb0: 74da 076d 6561 7375 7265 5a0b 6661 6c73  t..measureZ.fals
+00002fc0: 655f 706f 735f 675a 0b66 616c 7365 5f70  e_pos_gZ.false_p
+00002fd0: 6f73 5f73 5a11 6661 6c73 655f 706f 735f  os_sZ.false_pos_
+00002fe0: 696e 6469 6365 735a 0a74 7275 655f 706f  indicesZ.true_po
+00002ff0: 735f 675a 0a74 7275 655f 706f 735f 735a  s_gZ.true_pos_sZ
+00003000: 1074 7275 655f 706f 735f 696e 6469 6365  .true_pos_indice
+00003010: 7372 7500 0000 7277 0000 0072 1b00 0000  sru...rw...r....
+00003020: 721b 0000 0072 1c00 0000 728b 0000 00e2  r....r....r.....
+00003030: 0100 0073 9800 0000 0008 0401 0a01 1202  ...s............
+00003040: 0401 0803 0401 0401 0401 0201 08ff 0603  ................
+00003050: 1001 0a01 0401 0c01 1601 0601 0a02 1401  ................
+00003060: 0a01 0c01 0c01 0e01 0c02 0401 0201 06ff  ................
+00003070: 0a03 0e01 1002 0c02 0a01 0a01 0401 0401  ................
+00003080: 0401 0401 0401 0401 0401 1001 0801 1601  ................
+00003090: 1801 0a01 0c01 0c01 0e01 0a01 1801 0a01  ................
+000030a0: 0c01 0c01 0e01 0a01 0e01 1201 0e01 1002  ................
+000030b0: 0e01 0a01 0a01 0a01 0a01 0a01 0a01 0a01  ................
+000030c0: 0a01 0a01 0a01 0e02 0401 0201 06fe 0615  ................
+000030d0: 7a21 4665 6174 7572 6545 7661 6c75 6174  z!FeatureEvaluat
+000030e0: 6f72 2e65 7661 6c75 6174 655f 6665 6174  or.evaluate_feat
+000030f0: 7572 654e 2902 721e 0000 0046 2901 4629  ureN).r....F).F)
+00003100: 0172 1e00 0000 2910 7236 0000 0072 3700  .r....).r6...r7.
+00003110: 0000 7238 0000 0072 1d00 0000 7263 0000  ..r8...r....rc..
+00003120: 0072 6e00 0000 7205 0000 0072 7800 0000  .rn...r....rx...
+00003130: 7270 0000 0072 7100 0000 7282 0000 0072  rp...rq...r....r
+00003140: 9500 0000 72b1 0000 0072 a800 0000 72bf  ....r....r....r.
+00003150: 0000 0072 8b00 0000 721b 0000 0072 1b00  ...r....r....r..
+00003160: 0000 721b 0000 0072 1c00 0000 7239 0000  ..r....r....r9..
+00003170: 008c 0000 0073 2600 0000 0801 0a06 0831  .....s&........1
+00003180: 0812 0201 0201 0201 02f9 0a35 00f9 0a1a  ...........5....
+00003190: 080b 080a 081d 0a44 0826 0831 0201 02fa  .......D.&.1....
+000031a0: 7239 0000 0029 1572 b700 0000 720b 0000  r9...).r....r...
+000031b0: 00da 0b63 6f6c 6c65 6374 696f 6e73 7202  ...collectionsr.
+000031c0: 0000 00da 086e 6574 776f 726b 7872 ba00  .....networkxr..
+000031d0: 0000 da06 7061 6e64 6173 7268 0000 00da  ....pandasrh....
+000031e0: 0670 656e 6d61 6e72 4a00 0000 5a0f 736b  .penmanrJ...Z.sk
+000031f0: 6c65 6172 6e2e 6d65 7472 6963 7372 0300  learn.metricsr..
+00003200: 0000 7204 0000 00da 1374 7577 5f6e 6c70  ..r......tuw_nlp
+00003210: 2e67 7261 7068 2e75 7469 6c73 7205 0000  .graph.utilsr...
+00003220: 00da 1578 706f 7461 746f 2e64 6174 6173  ...xpotato.datas
+00003230: 6574 2e75 7469 6c73 7206 0000 0072 0700  et.utilsr....r..
+00003240: 0000 7208 0000 0072 0900 0000 7239 0000  ..r....r....r9..
+00003250: 0072 1b00 0000 721b 0000 0072 1b00 0000  .r....r....r....
+00003260: 721c 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00003270: 0000 0073 1600 0000 0801 0801 0c02 0801  ...s............
+00003280: 0801 0801 0c01 0c01 0c02 1403 0e7d       .............}
```

### Comparing `xpotato-0.1.4/xpotato/graph_extractor/__pycache__/graph.cpython-39.pyc` & `xpotato-0.1.5/xpotato/dataset/__pycache__/sample.cpython-37.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Wed Mar  9 10:46:32 2022 UTC, .py size: 468 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,68 @@
-00000000: 610d 0d0a 0000 0000 8885 2862 d401 0000  a.........(b....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
-00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c04 6d05 5a05 0100 4700  ..d.d.l.m.Z...G.
-00000050: 6404 6405 8400 6405 8302 5a06 6401 5300  d.d...d...Z.d.S.
-00000060: 2906 e900 0000 004e 2901 da0b 6772 6170  )......N)...grap
-00000070: 685f 746f 5f70 6e29 01da 1364 6566 6175  h_to_pn)...defau
-00000080: 6c74 5f70 6e5f 746f 5f67 7261 7068 6300  lt_pn_to_graphc.
-00000090: 0000 0000 0000 0000 0000 0000 0000 0005  ................
-000000a0: 0000 0040 0000 0073 3000 0000 6500 5a01  ...@...s0...e.Z.
-000000b0: 6400 5a02 6408 6503 6a04 6505 6401 6402  d.Z.d.e.j.e.d.d.
-000000c0: 9c03 6403 6404 8405 5a06 6505 6405 9c01  ..d.d...Z.e.d...
-000000d0: 6406 6407 8404 5a07 6401 5300 2909 da0b  d.d...Z.d.S.)...
-000000e0: 506f 7461 746f 4772 6170 684e 2903 da05  PotatoGraphN)...
-000000f0: 6772 6170 68da 0967 7261 7068 5f73 7472  graph..graph_str
-00000100: da06 7265 7475 726e 6303 0000 0000 0000  ..returnc.......
-00000110: 0000 0000 0004 0000 0003 0000 0043 0000  .............C..
-00000120: 0073 2a00 0000 7c01 720c 7c01 7c00 5f00  .s*...|.r.|.|._.
-00000130: 6e1a 7c02 7220 7401 7c02 8301 5c02 7c00  n.|.r t.|...\.|.
-00000140: 5f00 7d03 6e06 6400 7c00 5f00 6400 5300  _.}.n.d.|._.d.S.
-00000150: a901 4e29 0272 0500 0000 7203 0000 0029  ..N).r....r....)
-00000160: 04da 0473 656c 6672 0500 0000 7206 0000  ...selfr....r...
-00000170: 00da 015f a900 720b 0000 00fa 3e2f 686f  ..._..r.....>/ho
-00000180: 6d65 2f61 6461 616d 6b6f 2f70 726f 6a65  me/adaamko/proje
-00000190: 6374 732f 504f 5441 544f 2f78 706f 7461  cts/POTATO/xpota
-000001a0: 746f 2f67 7261 7068 5f65 7874 7261 6374  to/graph_extract
-000001b0: 6f72 2f67 7261 7068 2e70 79da 085f 5f69  or/graph.py..__i
-000001c0: 6e69 745f 5f07 0000 0073 0a00 0000 0001  nit__....s......
-000001d0: 0401 0801 0401 1002 7a14 506f 7461 746f  ........z.Potato
-000001e0: 4772 6170 682e 5f5f 696e 6974 5f5f 2901  Graph.__init__).
-000001f0: 7207 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00000200: 0000 0100 0000 0200 0000 4300 0000 730a  ..........C...s.
-00000210: 0000 0074 007c 006a 0183 0153 0072 0800  ...t.|.j...S.r..
-00000220: 0000 2902 7202 0000 0072 0500 0000 2901  ..).r....r....).
-00000230: 7209 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
-00000240: 0c00 0000 da07 5f5f 7374 725f 5f0f 0000  ......__str__...
-00000250: 0073 0200 0000 0001 7a13 506f 7461 746f  .s......z.Potato
-00000260: 4772 6170 682e 5f5f 7374 725f 5f29 024e  Graph.__str__).N
-00000270: 4e29 08da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-00000280: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000290: 6c6e 616d 655f 5fda 026e 78da 0744 6947  lname__..nx..DiG
-000002a0: 7261 7068 da03 7374 7272 0d00 0000 720e  raph..strr....r.
-000002b0: 0000 0072 0b00 0000 720b 0000 0072 0b00  ...r....r....r..
-000002c0: 0000 720c 0000 0072 0400 0000 0600 0000  ..r....r........
-000002d0: 7304 0000 0008 0116 0872 0400 0000 2907  s........r....).
-000002e0: da08 6e65 7477 6f72 6b78 7212 0000 00da  ..networkxr.....
-000002f0: 1374 7577 5f6e 6c70 2e67 7261 7068 2e75  .tuw_nlp.graph.u
-00000300: 7469 6c73 7202 0000 00da 1578 706f 7461  tilsr......xpota
-00000310: 746f 2e64 6174 6173 6574 2e75 7469 6c73  to.dataset.utils
-00000320: 7203 0000 0072 0400 0000 720b 0000 0072  r....r....r....r
-00000330: 0b00 0000 720b 0000 0072 0c00 0000 da08  ....r....r......
-00000340: 3c6d 6f64 756c 653e 0100 0000 7306 0000  <module>....s...
-00000350: 0008 010c 010c 03                        .......
+00000000: 420d 0d0a 0000 0000 6ff7 7d63 e902 0000  B.......o.}c....
+00000010: e300 0000 0000 0000 0000 0000 0003 0000  ................
+00000020: 0040 0000 0073 2e00 0000 6400 6401 6c00  .@...s....d.d.l.
+00000030: 6d01 5a01 6d02 5a02 0100 6400 6402 6c03  m.Z.m.Z...d.d.l.
+00000040: 6d04 5a04 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
+00000050: 8302 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
+00000060: 02da 0444 6963 74da 0554 7570 6c65 2901  ...Dict..Tuple).
+00000070: da0b 506f 7461 746f 4772 6170 6863 0000  ..PotatoGraphc..
+00000080: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
+00000090: 0000 7350 0000 0065 005a 0164 005a 0264  ..sP...e.Z.d.Z.d
+000000a0: 0b65 0365 0465 0466 0219 0065 0565 0664  .e.e.e.f...e.e.d
+000000b0: 0164 029c 0464 0364 0484 055a 0765 0564  .d...d.d...Z.e.d
+000000c0: 0164 059c 0264 0664 0784 045a 0865 0965  .d...d.d...Z.e.e
+000000d0: 0465 0666 0219 0064 089c 0164 0964 0a84  .e.f...d...d.d..
+000000e0: 045a 0a64 0153 0029 0cda 0653 616d 706c  .Z.d.S.)...Sampl
+000000f0: 654e 2904 da07 6578 616d 706c 65da 0c70  eN)...example..p
+00000100: 6f74 6174 6f5f 6772 6170 68da 086c 6162  otato_graph..lab
+00000110: 656c 5f69 64da 0672 6574 7572 6e63 0400  el_id..returnc..
+00000120: 0000 0000 0000 0400 0000 0200 0000 4300  ..............C.
+00000130: 0000 7324 0000 007c 0164 0119 007c 005f  ..s$...|.d...|._
+00000140: 007c 0164 0219 007c 005f 017c 037c 005f  .|.d...|._.|.|._
+00000150: 027c 027c 005f 0364 0053 0029 034e 7201  .|.|._.d.S.).Nr.
+00000160: 0000 00e9 0100 0000 2904 da04 7465 7874  ........)...text
+00000170: da05 6c61 6265 6c72 0800 0000 7207 0000  ..labelr....r...
+00000180: 0029 04da 0473 656c 6672 0600 0000 7207  .)...selfr....r.
+00000190: 0000 0072 0800 0000 a900 720e 0000 00fa  ...r......r.....
+000001a0: 4c2f 5573 6572 732f 6164 616d 6b6f 7661  L/Users/adamkova
+000001b0: 6373 2f70 726f 6a65 6374 732f 6578 702d  cs/projects/exp-
+000001c0: 7265 6c61 7469 6f6e 2d65 7874 7261 6374  relation-extract
+000001d0: 696f 6e2f 7870 6f74 6174 6f2f 6461 7461  ion/xpotato/data
+000001e0: 7365 742f 7361 6d70 6c65 2e70 79da 085f  set/sample.py.._
+000001f0: 5f69 6e69 745f 5f07 0000 0073 0800 0000  _init__....s....
+00000200: 0006 0a01 0a01 0601 7a0f 5361 6d70 6c65  ........z.Sample
+00000210: 2e5f 5f69 6e69 745f 5f29 02da 0567 7261  .__init__)...gra
+00000220: 7068 7209 0000 0063 0200 0000 0000 0000  phr....c........
+00000230: 0200 0000 0200 0000 4300 0000 730a 0000  ........C...s...
+00000240: 007c 017c 005f 0064 0053 0029 014e 2901  .|.|._.d.S.).N).
+00000250: 7207 0000 0029 0272 0d00 0000 7211 0000  r....).r....r...
+00000260: 0072 0e00 0000 720e 0000 0072 0f00 0000  .r....r....r....
+00000270: da09 7365 745f 6772 6170 6812 0000 0073  ..set_graph....s
+00000280: 0200 0000 0001 7a10 5361 6d70 6c65 2e73  ......z.Sample.s
+00000290: 6574 5f67 7261 7068 2901 da0b 6c61 6265  et_graph)...labe
+000002a0: 6c5f 766f 6361 6263 0200 0000 0000 0000  l_vocabc........
+000002b0: 0200 0000 0200 0000 4300 0000 7332 0000  ........C...s2..
+000002c0: 007c 006a 0064 006b 0972 107c 006a 0053  .|.j.d.k.r.|.j.S
+000002d0: 007c 006a 0172 2a7c 006a 017c 016b 0672  .|.j.r*|.j.|.k.r
+000002e0: 2a7c 017c 006a 0119 0053 0064 0053 0064  *|.|.j...S.d.S.d
+000002f0: 0053 0029 014e 2902 7208 0000 0072 0c00  .S.).N).r....r..
+00000300: 0000 2902 720d 0000 0072 1300 0000 720e  ..).r....r....r.
+00000310: 0000 0072 0e00 0000 720f 0000 00da 0c67  ...r....r......g
+00000320: 6574 5f6c 6162 656c 5f69 6415 0000 0073  et_label_id....s
+00000330: 0a00 0000 0001 0a01 0601 1001 0a02 7a13  ..............z.
+00000340: 5361 6d70 6c65 2e67 6574 5f6c 6162 656c  Sample.get_label
+00000350: 5f69 6429 024e 4e29 0bda 085f 5f6e 616d  _id).NN)...__nam
+00000360: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000370: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0300  .__qualname__r..
+00000380: 0000 da03 7374 7272 0400 0000 da03 696e  ....strr......in
+00000390: 7472 1000 0000 7212 0000 0072 0200 0000  tr....r....r....
+000003a0: 7214 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+000003b0: 0e00 0000 720f 0000 0072 0500 0000 0600  ....r....r......
+000003c0: 0000 730a 0000 0008 0400 0110 010e 0610  ..s.............
+000003d0: 0372 0500 0000 4e29 06da 0674 7970 696e  .r....N)...typin
+000003e0: 6772 0200 0000 7203 0000 00da 1d78 706f  gr....r......xpo
+000003f0: 7461 746f 2e67 7261 7068 5f65 7874 7261  tato.graph_extra
+00000400: 6374 6f72 2e67 7261 7068 7204 0000 0072  ctor.graphr....r
+00000410: 0500 0000 720e 0000 0072 0e00 0000 720e  ....r....r....r.
+00000420: 0000 0072 0f00 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000430: 653e 0100 0000 7304 0000 0010 020c 03    e>....s........
```

### Comparing `xpotato-0.1.4/xpotato/graph_extractor/__pycache__/rule.cpython-39.pyc` & `xpotato-0.1.5/xpotato/graph_extractor/__pycache__/rule.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  6 08:59:17 2022 UTC, .py size: 4584 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 65e3 7462 e811 0000  a.......e.tb....
+00000000: 610d 0d0a 0000 0000 6ff7 7d63 e811 0000  a.......o.}c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 0100 4700 6403 6404  m.Z.m.Z...G.d.d.
 00000050: 8400 6404 8302 5a05 4700 6405 6406 8400  ..d...Z.G.d.d...
 00000060: 6406 8302 5a06 6401 5300 2907 e900 0000  d...Z.d.S.).....
 00000070: 004e 2903 da04 4469 6374 da04 4c69 7374  .N)...Dict..List
@@ -23,298 +23,299 @@
 00000160: 4e72 0100 0000 e901 0000 00e9 0200 0000  Nr..............
 00000170: e903 0000 0029 05da 1070 6f73 6974 6976  .....)...positiv
 00000180: 655f 7361 6d70 6c65 73da 106e 6567 6174  e_samples..negat
 00000190: 6976 655f 7361 6d70 6c65 73da 056c 6162  ive_samples..lab
 000001a0: 656c da06 6f70 656e 6965 da0c 6d61 726b  el..openie..mark
 000001b0: 6564 5f6e 6f64 6573 2903 da04 7365 6c66  ed_nodes)...self
 000001c0: da04 7275 6c65 720c 0000 00a9 0072 1000  ..ruler......r..
-000001d0: 0000 fa3d 2f68 6f6d 652f 6164 6161 6d6b  ...=/home/adaamk
-000001e0: 6f2f 7072 6f6a 6563 7473 2f50 4f54 4154  o/projects/POTAT
-000001f0: 4f2f 7870 6f74 6174 6f2f 6772 6170 685f  O/xpotato/graph_
-00000200: 6578 7472 6163 746f 722f 7275 6c65 2e70  extractor/rule.p
-00000210: 79da 085f 5f69 6e69 745f 5f06 0000 0073  y..__init__....s
-00000220: 0e00 0000 0001 0a01 0a01 0a01 0602 0601  ................
-00000230: 0401 7a0d 5275 6c65 2e5f 5f69 6e69 745f  ..z.Rule.__init_
-00000240: 5f29 02da 085f 5275 6c65 5f5f 6fda 0672  _)..._Rule__o..r
-00000250: 6574 7572 6e63 0200 0000 0000 0000 0000  eturnc..........
-00000260: 0000 0200 0000 0400 0000 4300 0000 7346  ..........C...sF
-00000270: 0000 0074 007c 0174 0183 0273 0e64 0153  ...t.|.t...s.d.S
-00000280: 0074 027c 006a 0383 0174 027c 016a 0383  .t.|.j...t.|.j..
-00000290: 016b 026f 4474 027c 006a 0483 0174 027c  .k.oDt.|.j...t.|
-000002a0: 016a 04a0 05a1 0083 016b 026f 447c 006a  .j.......k.oD|.j
-000002b0: 067c 016a 066b 0253 00a9 024e 4629 07da  .|.j.k.S...NF)..
-000002c0: 0a69 7369 6e73 7461 6e63 6572 0500 0000  .isinstancer....
-000002d0: da06 736f 7274 6564 7209 0000 0072 0a00  ..sortedr....r..
-000002e0: 0000 da04 736f 7274 720b 0000 0029 0272  ....sortr....).r
-000002f0: 0e00 0000 7213 0000 0072 1000 0000 7210  ....r....r....r.
-00000300: 0000 0072 1100 0000 da06 5f5f 6571 5f5f  ...r......__eq__
-00000310: 1000 0000 730e 0000 0000 010a 0104 0214  ....s...........
-00000320: 0116 ff02 020a fd7a 0b52 756c 652e 5f5f  .......z.Rule.__
-00000330: 6571 5f5f 4ea9 0172 1400 0000 6301 0000  eq__N..r....c...
-00000340: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00000350: 0043 0000 0073 1800 0000 7c00 6a00 a001  .C...s....|.j...
-00000360: a100 0100 7c00 6a02 a001 a100 0100 6400  ....|.j.......d.
-00000370: 5300 a901 4e29 0372 0900 0000 7218 0000  S...N).r....r...
-00000380: 0072 0a00 0000 a901 720e 0000 0072 1000  .r......r....r..
-00000390: 0000 7210 0000 0072 1100 0000 da09 736f  ..r....r......so
-000003a0: 7274 5f72 756c 6519 0000 0073 0400 0000  rt_rule....s....
-000003b0: 0001 0a01 7a0e 5275 6c65 2e73 6f72 745f  ....z.Rule.sort_
-000003c0: 7275 6c65 6301 0000 0000 0000 0000 0000  rulec...........
-000003d0: 0001 0000 0004 0000 0043 0000 0073 2e00  .........C...s..
-000003e0: 0000 7c00 6a00 6401 6b02 721a 7c00 6a01  ..|.j.d.k.r.|.j.
-000003f0: 7c00 6a02 7c00 6a03 6703 5300 7c00 6a01  |.j.|.j.g.S.|.j.
-00000400: 7c00 6a02 7c00 6a03 7c00 6a04 6704 5300  |.j.|.j.|.j.g.S.
-00000410: 7215 0000 0029 0572 0c00 0000 7209 0000  r....).r....r...
-00000420: 0072 0a00 0000 720b 0000 0072 0d00 0000  .r....r....r....
-00000430: 721c 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
-00000440: 1100 0000 da07 746f 5f6c 6973 741d 0000  ......to_list...
-00000450: 0073 1000 0000 0003 08ff 1203 0401 0401  .s..............
-00000460: 0401 04fc 02fd 7a0c 5275 6c65 2e74 6f5f  ......z.Rule.to_
-00000470: 6c69 7374 2901 4629 0cda 085f 5f6e 616d  list).F)...__nam
-00000480: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000490: 0c5f 5f71 7561 6c6e 616d 655f 5f72 1200  .__qualname__r..
-000004a0: 0000 da06 6f62 6a65 6374 da04 626f 6f6c  ....object..bool
-000004b0: 7219 0000 0072 1d00 0000 7203 0000 0072  r....r....r....r
-000004c0: 0400 0000 da03 7374 7272 1e00 0000 7210  ......strr....r.
-000004d0: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
-000004e0: 0000 7205 0000 0005 0000 0073 0800 0000  ..r........s....
-000004f0: 0801 0a0a 1009 0e04 7205 0000 0063 0000  ........r....c..
-00000500: 0000 0000 0000 0000 0000 0000 0000 0800  ................
-00000510: 0000 4000 0000 730a 0100 0065 005a 0164  ..@...s....e.Z.d
-00000520: 005a 0264 2365 0365 0419 0064 029c 0164  .Z.d#e.e...d...d
-00000530: 0364 0484 055a 0564 0564 0684 005a 0665  .d...Z.d.d...Z.e
-00000540: 0765 0864 079c 0264 0864 0984 045a 0964  .e.d...d.d...Z.d
-00000550: 0164 0a9c 0164 0b64 0c84 045a 0a65 0b64  .d...d.d...Z.e.d
-00000560: 0d9c 0164 0e64 0f84 045a 0c65 0b64 0d9c  ...d.d...Z.e.d..
-00000570: 0164 1064 1184 045a 0d64 2465 0e65 0b65  .d.d...Z.d$e.e.e
-00000580: 0365 0365 0f65 0365 0b19 0065 0b66 0219  .e.e.e.e...e.f..
-00000590: 0019 0019 0066 0219 0065 0864 139c 0264  .....f...e.d...d
-000005a0: 1464 1584 055a 1064 2565 0b65 0864 169c  .d...Z.d%e.e.d..
-000005b0: 0264 1764 1884 055a 1165 0b64 199c 0164  .d.d...Z.e.d...d
-000005c0: 1a64 1b84 045a 1265 0464 1c9c 0164 1d64  .d...Z.e.d...d.d
-000005d0: 1e84 045a 1365 0e65 0b65 0365 0365 0f65  ...Z.e.e.e.e.e.e
-000005e0: 0365 0b19 0065 0b66 0219 0019 0019 0066  .e...e.f.......f
-000005f0: 0219 0064 0a9c 0164 1f64 2084 045a 1465  ...d...d.d ..Z.e
-00000600: 0365 0365 0f65 0365 0b19 0065 0b66 0219  .e.e.e.e...e.f..
-00000610: 0019 0019 0064 0a9c 0164 2164 2284 045a  .....d...d!d"..Z
-00000620: 1564 0153 0029 26da 0752 756c 6553 6574  .d.S.)&..RuleSet
-00000630: 4ea9 01da 0572 756c 6573 6302 0000 0000  N....rulesc.....
-00000640: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
-00000650: 0000 0073 1a00 0000 7c01 6400 7500 7210  ...s....|.d.u.r.
-00000660: 6700 7c00 5f00 6e06 7c01 7c00 5f00 6400  g.|._.n.|.|._.d.
-00000670: 5300 721b 0000 0072 2600 0000 2902 720e  S.r....r&...).r.
-00000680: 0000 0072 2700 0000 7210 0000 0072 1000  ...r'...r....r..
-00000690: 0000 7211 0000 0072 1200 0000 2b00 0000  ..r....r....+...
-000006a0: 7306 0000 0000 0108 0108 027a 1052 756c  s..........z.Rul
-000006b0: 6553 6574 2e5f 5f69 6e69 745f 5f63 0100  eSet.__init__c..
-000006c0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-000006d0: 0000 6300 0000 7316 0000 007c 006a 0044  ..c...s....|.j.D
-000006e0: 005d 0a7d 017c 0156 0001 0071 0664 0053  .].}.|.V...q.d.S
-000006f0: 0072 1b00 0000 7226 0000 00a9 0272 0e00  .r....r&.....r..
-00000700: 0000 720f 0000 0072 1000 0000 7210 0000  ..r....r....r...
-00000710: 0072 1100 0000 da08 5f5f 6974 6572 5f5f  .r......__iter__
-00000720: 3100 0000 7304 0000 0000 010a 017a 1052  1...s........z.R
-00000730: 756c 6553 6574 2e5f 5f69 7465 725f 5f29  uleSet.__iter__)
-00000740: 02da 0b5f 5275 6c65 5365 745f 5f6f 7214  ..._RuleSet__or.
-00000750: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00000760: 0200 0000 0300 0000 4300 0000 731a 0000  ........C...s...
-00000770: 0074 007c 0174 0183 0273 0e64 0153 007c  .t.|.t...s.d.S.|
-00000780: 006a 027c 016a 026b 0253 0072 1500 0000  .j.|.j.k.S.r....
-00000790: 2903 7216 0000 0072 2500 0000 7227 0000  ).r....r%...r'..
-000007a0: 0029 0272 0e00 0000 722a 0000 0072 1000  .).r....r*...r..
-000007b0: 0000 7210 0000 0072 1100 0000 7219 0000  ..r....r....r...
-000007c0: 0035 0000 0073 0600 0000 0001 0a01 0401  .5...s..........
-000007d0: 7a0e 5275 6c65 5365 742e 5f5f 6571 5f5f  z.RuleSet.__eq__
-000007e0: 721a 0000 0063 0100 0000 0000 0000 0000  r....c..........
-000007f0: 0000 0200 0000 0300 0000 4300 0000 732a  ..........C...s*
-00000800: 0000 007c 006a 0044 005d 0c7d 017c 01a0  ...|.j.D.].}.|..
-00000810: 01a1 0001 0071 067c 006a 006a 0264 0164  .....q.|.j.j.d.d
-00000820: 0284 0064 038d 0101 0064 0053 0029 044e  ...d.....d.S.).N
-00000830: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000840: 0005 0000 0053 0000 0073 1c00 0000 7c00  .....S...s....|.
-00000850: 6a00 6401 a001 7c00 6a02 a101 6401 a001  j.d...|.j...d...
-00000860: 7c00 6a03 a101 6603 5300 2902 4efa 013b  |.j...f.S.).N..;
-00000870: 2904 720b 0000 00da 046a 6f69 6e72 0900  ).r......joinr..
-00000880: 0000 720a 0000 00a9 0172 0f00 0000 7210  ..r......r....r.
-00000890: 0000 0072 1000 0000 7211 0000 00da 083c  ...r....r......<
-000008a0: 6c61 6d62 6461 3e3f 0000 0073 0800 0000  lambda>?...s....
-000008b0: 0001 0401 0a01 0afd 7a24 5275 6c65 5365  ........z$RuleSe
-000008c0: 742e 736f 7274 5f72 756c 6573 2e3c 6c6f  t.sort_rules.<lo
-000008d0: 6361 6c73 3e2e 3c6c 616d 6264 613e 2901  cals>.<lambda>).
-000008e0: da03 6b65 7929 0372 2700 0000 721d 0000  ..key).r'...r...
-000008f0: 0072 1800 0000 7228 0000 0072 1000 0000  .r....r(...r....
-00000900: 7210 0000 0072 1100 0000 da0a 736f 7274  r....r......sort
-00000910: 5f72 756c 6573 3a00 0000 730a 0000 0000  _rules:...s.....
-00000920: 010a 010a 0206 0106 ff7a 1252 756c 6553  .........z.RuleS
-00000930: 6574 2e73 6f72 745f 7275 6c65 7329 01da  et.sort_rules)..
-00000940: 0874 7376 5f70 6174 6863 0200 0000 0000  .tsv_pathc......
-00000950: 0000 0000 0000 0900 0000 0800 0000 4300  ..............C.
-00000960: 0000 73a2 0000 007c 00a0 00a1 0001 0074  ..s....|.......t
-00000970: 017c 0164 0183 028f 7c7d 027c 006a 0244  .|.d....|}.|.j.D
-00000980: 005d 647d 0364 02a0 037c 036a 04a1 017d  .]d}.d...|.j...}
-00000990: 0464 02a0 037c 036a 05a1 017d 057c 036a  .d...|.j...}.|.j
-000009a0: 067d 067c 036a 077d 077c 069b 0064 037c  .}.|.j.}.|...d.|
-000009b0: 049b 0064 037c 059b 009d 057d 087c 036a  ...d.|.....}.|.j
-000009c0: 0872 707c 0864 0374 09a0 0a7c 07a1 019b  .rp|.d.t...|....
-000009d0: 009d 0237 007d 087c 02a0 0b7c 0864 0417  ...7.}.|...|.d..
-000009e0: 00a1 0101 0071 1a57 0064 0004 0004 0083  .....q.W.d......
-000009f0: 0301 006e 1031 0073 9430 0001 0001 0001  ...n.1.s.0......
-00000a00: 0059 0001 0064 0053 0029 054e da01 7772  .Y...d.S.).N..wr
-00000a10: 2b00 0000 fa01 09da 010a 290c 7230 0000  +.........).r0..
-00000a20: 00da 046f 7065 6e72 2700 0000 722c 0000  ...openr'...r,..
-00000a30: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
-00000a40: 720d 0000 0072 0c00 0000 da04 6a73 6f6e  r....r......json
-00000a50: da05 6475 6d70 73da 0577 7269 7465 2909  ..dumps..write).
-00000a60: 720e 0000 0072 3100 0000 da01 6672 0f00  r....r1.....fr..
-00000a70: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
-00000a80: 0072 0d00 0000 5a08 7275 6c65 5f73 7472  .r....Z.rule_str
-00000a90: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
-00000aa0: 0674 6f5f 7473 7646 0000 0073 1600 0000  .to_tsvF...s....
-00000ab0: 0001 0801 0c01 0a01 0c01 0c01 0601 0602  ................
-00000ac0: 1402 0601 1401 7a0e 5275 6c65 5365 742e  ......z.RuleSet.
-00000ad0: 746f 5f74 7376 6302 0000 0000 0000 0000  to_tsvc.........
-00000ae0: 0000 0009 0000 0008 0000 0043 0000 0073  ...........C...s
-00000af0: 2601 0000 7400 7c01 6401 8302 9001 8f04  &...t.|.d.......
-00000b00: 7d02 7c02 4400 5dee 7d03 7c03 a001 6402  }.|.D.].}.|...d.
-00000b10: a101 7d03 7c03 a002 6403 a101 7d03 7c03  ..}.|...d...}.|.
-00000b20: 6404 1900 6405 6b02 723a 6700 6e0c 7c03  d...d.k.r:g.n.|.
-00000b30: 6404 1900 a002 6406 a101 7d04 7c03 6407  d.....d...}.|.d.
-00000b40: 1900 6405 6b02 7258 6700 6e0c 7c03 6407  ..d.k.rXg.n.|.d.
-00000b50: 1900 a002 6406 a101 7d05 7c03 6408 1900  ....d...}.|.d...
-00000b60: a001 a100 7d06 6400 7d07 7403 7c03 8301  ....}.d.}.t.|...
-00000b70: 6409 6b02 7296 7404 7c04 7c05 7c06 6703  d.k.r.t.|.|.|.g.
-00000b80: 640a 640b 8d02 7d07 6e4e 7403 7c03 8301  d.d...}.nNt.|...
-00000b90: 640c 6b02 72d6 7c03 6409 1900 6405 6b02  d.k.r.|.d...d.k.
-00000ba0: 72b2 6700 6e0c 7405 a006 7c03 6409 1900  r.g.n.t...|.d...
-00000bb0: a101 7d08 7404 7c04 7c05 7c06 7c08 6704  ..}.t.|.|.|.|.g.
-00000bc0: 640d 640b 8d02 7d07 6e0e 7407 640e 7c03  d.d...}.n.t.d.|.
-00000bd0: 9b00 9d02 8301 8201 7c07 73f6 7407 640f  ........|.s.t.d.
-00000be0: 7c03 9b00 9d02 8301 8201 7c00 a008 7c07  |.........|...|.
-00000bf0: a101 0100 7112 5700 6400 0400 0400 8303  ....q.W.d.......
-00000c00: 0100 6e12 3100 9001 7318 3000 0100 0100  ..n.1...s.0.....
-00000c10: 0100 5900 0100 6400 5300 2910 4eda 0172  ..Y...d.S.).N..r
-00000c20: 7234 0000 0072 3300 0000 7206 0000 00da  r4...r3...r.....
-00000c30: 0072 2b00 0000 7207 0000 0072 0100 0000  .r+...r....r....
-00000c40: 7208 0000 0046 a901 720c 0000 00e9 0400  r....F..r.......
-00000c50: 0000 547a 1a49 6e76 616c 6964 206e 756d  ..Tz.Invalid num
-00000c60: 6265 7220 6f66 2066 6965 6c64 733a 207a  ber of fields: z
-00000c70: 0e49 6e76 616c 6964 2072 756c 653a 2029  .Invalid rule: )
-00000c80: 0972 3500 0000 da05 7374 7269 70da 0573  .r5.....strip..s
-00000c90: 706c 6974 da03 6c65 6e72 0500 0000 7236  plit..lenr....r6
-00000ca0: 0000 00da 056c 6f61 6473 da09 4578 6365  .....loads..Exce
-00000cb0: 7074 696f 6eda 0861 6464 5f72 756c 6529  ption..add_rule)
-00000cc0: 0972 0e00 0000 7231 0000 0072 3900 0000  .r....r1...r9...
-00000cd0: da04 6c69 6e65 7209 0000 0072 0a00 0000  ..liner....r....
-00000ce0: 720b 0000 0072 0f00 0000 720d 0000 0072  r....r....r....r
-00000cf0: 1000 0000 7210 0000 0072 1100 0000 da08  ....r....r......
-00000d00: 6672 6f6d 5f74 7376 5500 0000 732c 0000  from_tsvU...s,..
-00000d10: 0000 010e 0108 010a 010a 021e 011e 010c  ................
-00000d20: 0104 010c 0102 010a ff08 030c 011e 0102  ................
-00000d30: 010a 0102 fe08 050e 0204 010e 017a 1052  .............z.R
-00000d40: 756c 6553 6574 2e66 726f 6d5f 7473 7646  uleSet.from_tsvF
-00000d50: 2902 7227 0000 0072 0c00 0000 6303 0000  ).r'...r....c...
-00000d60: 0000 0000 0000 0000 0006 0000 0008 0000  ................
-00000d70: 0043 0000 0073 3200 0000 7c01 a000 a100  .C...s2...|.....
-00000d80: 4400 5d24 5c02 7d03 7d04 7c04 4400 5d16  D.]$\.}.}.|.D.].
-00000d90: 7d05 7c00 a001 7402 7c05 7c02 6401 8d02  }.|...t.|.|.d...
-00000da0: a101 0100 7114 7108 6400 5300 2902 4e72  ....q.q.d.S.).Nr
-00000db0: 3d00 0000 2903 da05 6974 656d 7372 4400  =...)...itemsrD.
-00000dc0: 0000 7205 0000 0029 0672 0e00 0000 7227  ..r....).r....r'
-00000dd0: 0000 0072 0c00 0000 722f 0000 00da 0576  ...r....r/.....v
-00000de0: 616c 7565 720f 0000 0072 1000 0000 7210  aluer....r....r.
-00000df0: 0000 0072 1100 0000 da09 6672 6f6d 5f64  ...r......from_d
-00000e00: 6963 7470 0000 0073 0600 0000 0003 1001  ictp...s........
-00000e10: 0801 7a11 5275 6c65 5365 742e 6672 6f6d  ..z.RuleSet.from
-00000e20: 5f64 6963 7429 02da 096a 736f 6e5f 7061  _dict)...json_pa
-00000e30: 7468 720c 0000 0063 0300 0000 0000 0000  thr....c........
-00000e40: 0000 0000 0800 0000 0800 0000 4300 0000  ............C...
-00000e50: 7366 0000 0074 007c 0164 0183 028f 1a7d  sf...t.|.d.....}
-00000e60: 0374 01a0 027c 03a1 017d 0457 0064 0004  .t...|...}.W.d..
-00000e70: 0004 0083 0301 006e 1031 0073 2a30 0001  .......n.1.s*0..
-00000e80: 0001 0001 0059 0001 007c 04a0 03a1 0044  .....Y...|.....D
-00000e90: 005d 245c 027d 057d 067c 0644 005d 167d  .]$\.}.}.|.D.].}
-00000ea0: 077c 00a0 0474 057c 077c 0264 028d 02a1  .|...t.|.|.d....
-00000eb0: 0101 0071 4871 3c64 0053 0029 034e 723b  ...qHq<d.S.).Nr;
-00000ec0: 0000 0072 3d00 0000 2906 7235 0000 0072  ...r=...).r5...r
-00000ed0: 3600 0000 da04 6c6f 6164 7247 0000 0072  6.....loadrG...r
-00000ee0: 4400 0000 7205 0000 0029 0872 0e00 0000  D...r....).r....
-00000ef0: 724a 0000 0072 0c00 0000 7239 0000 0072  rJ...r....r9...r
-00000f00: 2700 0000 722f 0000 0072 4800 0000 720f  '...r/...rH...r.
-00000f10: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
-00000f20: 0000 da09 6672 6f6d 5f6a 736f 6e77 0000  ....from_jsonw..
-00000f30: 0073 0a00 0000 0001 0c01 2802 1001 0801  .s........(.....
-00000f40: 7a11 5275 6c65 5365 742e 6672 6f6d 5f6a  z.RuleSet.from_j
-00000f50: 736f 6e29 0172 4a00 0000 6302 0000 0000  son).rJ...c.....
-00000f60: 0000 0000 0000 0003 0000 0008 0000 0043  ...............C
-00000f70: 0000 0073 3e00 0000 7400 7c01 6401 8302  ...s>...t.|.d...
-00000f80: 8f20 7d02 7401 a002 7c00 a003 a100 7c02  . }.t...|.....|.
-00000f90: a102 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
-00000fa0: 6e10 3100 7330 3000 0100 0100 0100 5900  n.1.s00.......Y.
-00000fb0: 0100 6400 5300 2902 4e72 3200 0000 2904  ..d.S.).Nr2...).
-00000fc0: 7235 0000 0072 3600 0000 da04 6475 6d70  r5...r6.....dump
-00000fd0: da07 746f 5f64 6963 7429 0372 0e00 0000  ..to_dict).r....
-00000fe0: 724a 0000 0072 3900 0000 7210 0000 0072  rJ...r9...r....r
-00000ff0: 1000 0000 7211 0000 00da 0774 6f5f 6a73  ....r......to_js
-00001000: 6f6e 7f00 0000 7304 0000 0000 010c 017a  on....s........z
-00001010: 0f52 756c 6553 6574 2e74 6f5f 6a73 6f6e  .RuleSet.to_json
-00001020: 722d 0000 0063 0200 0000 0000 0000 0000  r-...c..........
-00001030: 0000 0200 0000 0300 0000 4300 0000 7310  ..........C...s.
-00001040: 0000 007c 006a 00a0 017c 01a1 0101 0064  ...|.j...|.....d
-00001050: 0053 0072 1b00 0000 2902 7227 0000 00da  .S.r....).r'....
-00001060: 0661 7070 656e 6472 2800 0000 7210 0000  .appendr(...r...
-00001070: 0072 1000 0000 7211 0000 0072 4400 0000  .r....r....rD...
-00001080: 8300 0000 7302 0000 0000 017a 1052 756c  ....s......z.Rul
-00001090: 6553 6574 2e61 6464 5f72 756c 6563 0100  eSet.add_rulec..
-000010a0: 0000 0000 0000 0000 0000 0300 0000 0500  ................
-000010b0: 0000 4300 0000 7334 0000 0064 0164 0284  ..C...s4...d.d..
-000010c0: 007c 006a 0044 0083 017d 017c 006a 0044  .|.j.D...}.|.j.D
-000010d0: 005d 187d 027c 017c 026a 0119 00a0 027c  .].}.|.|.j.....|
-000010e0: 02a0 03a1 00a1 0101 0071 167c 0153 0029  .........q.|.S.)
-000010f0: 034e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
-00001100: 0000 0004 0000 0053 0000 0073 1400 0000  .......S...s....
-00001110: 6900 7c00 5d0c 7d01 7c01 6a00 6700 9302  i.|.].}.|.j.g...
-00001120: 7104 5300 7210 0000 0029 0172 0b00 0000  q.S.r....).r....
-00001130: a902 da02 2e30 720f 0000 0072 1000 0000  .....0r....r....
-00001140: 7210 0000 0072 1100 0000 da0a 3c64 6963  r....r......<dic
-00001150: 7463 6f6d 703e 8700 0000 f300 0000 007a  tcomp>.........z
-00001160: 2352 756c 6553 6574 2e74 6f5f 6469 6374  #RuleSet.to_dict
-00001170: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
-00001180: 6f6d 703e 2904 7227 0000 0072 0b00 0000  omp>).r'...r....
-00001190: 7250 0000 0072 1e00 0000 2903 720e 0000  rP...r....).r...
-000011a0: 005a 0972 756c 655f 6469 6374 720f 0000  .Z.rule_dictr...
-000011b0: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
-000011c0: 724e 0000 0086 0000 0073 0800 0000 0001  rN.......s......
-000011d0: 1002 0a01 1602 7a0f 5275 6c65 5365 742e  ......z.RuleSet.
-000011e0: 746f 5f64 6963 7463 0100 0000 0000 0000  to_dictc........
-000011f0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00001200: 7310 0000 0064 0164 0284 007c 006a 0044  s....d.d...|.j.D
-00001210: 0083 0153 0029 034e 6301 0000 0000 0000  ...S.).Nc.......
-00001220: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
-00001230: 0073 1400 0000 6700 7c00 5d0c 7d01 7c01  .s....g.|.].}.|.
-00001240: a000 a100 9102 7104 5300 7210 0000 0029  ......q.S.r....)
-00001250: 0172 1e00 0000 7251 0000 0072 1000 0000  .r....rQ...r....
-00001260: 7210 0000 0072 1100 0000 da0a 3c6c 6973  r....r......<lis
-00001270: 7463 6f6d 703e 8f00 0000 7254 0000 007a  tcomp>....rT...z
-00001280: 2352 756c 6553 6574 2e74 6f5f 6c69 7374  #RuleSet.to_list
-00001290: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-000012a0: 6f6d 703e 7226 0000 0072 1c00 0000 7210  omp>r&...r....r.
-000012b0: 0000 0072 1000 0000 7211 0000 0072 1e00  ...r....r....r..
-000012c0: 0000 8e00 0000 7302 0000 0000 017a 0f52  ......s......z.R
-000012d0: 756c 6553 6574 2e74 6f5f 6c69 7374 2901  uleSet.to_list).
-000012e0: 4e29 0146 2901 4629 1672 1f00 0000 7220  N).F).F).r....r 
-000012f0: 0000 0072 2100 0000 7203 0000 0072 0500  ...r!...r....r..
-00001300: 0000 7212 0000 0072 2900 0000 7222 0000  ..r....r)...r"..
-00001310: 0072 2300 0000 7219 0000 0072 3000 0000  .r#...r....r0...
-00001320: 7224 0000 0072 3a00 0000 7246 0000 0072  r$...r:...rF...r
-00001330: 0200 0000 7204 0000 0072 4900 0000 724c  ....r....rI...rL
-00001340: 0000 0072 4f00 0000 7244 0000 0072 4e00  ...rO...rD...rN.
-00001350: 0000 721e 0000 0072 1000 0000 7210 0000  ..r....r....r...
-00001360: 0072 1000 0000 7211 0000 0072 2500 0000  .r....r....r%...
-00001370: 2a00 0000 731e 0000 0008 0114 0608 0410  *...s...........
-00001380: 050e 0c0e 0f0e 1c00 ff02 0120 ff0c 0712  ........... ....
-00001390: 080e 040e 032a 0872 2500 0000 2907 7236  .....*.r%...).r6
-000013a0: 0000 00da 0674 7970 696e 6772 0200 0000  .....typingr....
-000013b0: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
-000013c0: 2500 0000 7210 0000 0072 1000 0000 7210  %...r....r....r.
-000013d0: 0000 0072 1100 0000 da08 3c6d 6f64 756c  ...r......<modul
-000013e0: 653e 0100 0000 7306 0000 0008 0114 030e  e>....s.........
-000013f0: 25                                       %
+000001d0: 0000 fa52 2f55 7365 7273 2f61 6461 6d6b  ...R/Users/adamk
+000001e0: 6f76 6163 732f 7072 6f6a 6563 7473 2f65  ovacs/projects/e
+000001f0: 7870 2d72 656c 6174 696f 6e2d 6578 7472  xp-relation-extr
+00000200: 6163 7469 6f6e 2f78 706f 7461 746f 2f67  action/xpotato/g
+00000210: 7261 7068 5f65 7874 7261 6374 6f72 2f72  raph_extractor/r
+00000220: 756c 652e 7079 da08 5f5f 696e 6974 5f5f  ule.py..__init__
+00000230: 0600 0000 730e 0000 0000 010a 010a 010a  ....s...........
+00000240: 0106 0206 0104 017a 0d52 756c 652e 5f5f  .......z.Rule.__
+00000250: 696e 6974 5f5f 2902 da08 5f52 756c 655f  init__)..._Rule_
+00000260: 5f6f da06 7265 7475 726e 6302 0000 0000  _o..returnc.....
+00000270: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00000280: 0000 0073 4600 0000 7400 7c01 7401 8302  ...sF...t.|.t...
+00000290: 730e 6401 5300 7402 7c00 6a03 8301 7402  s.d.S.t.|.j...t.
+000002a0: 7c01 6a03 8301 6b02 6f44 7402 7c00 6a04  |.j...k.oDt.|.j.
+000002b0: 8301 7402 7c01 6a04 a005 a100 8301 6b02  ..t.|.j.......k.
+000002c0: 6f44 7c00 6a06 7c01 6a06 6b02 5300 a902  oD|.j.|.j.k.S...
+000002d0: 4e46 2907 da0a 6973 696e 7374 616e 6365  NF)...isinstance
+000002e0: 7205 0000 00da 0673 6f72 7465 6472 0900  r......sortedr..
+000002f0: 0000 720a 0000 00da 0473 6f72 7472 0b00  ..r......sortr..
+00000300: 0000 2902 720e 0000 0072 1300 0000 7210  ..).r....r....r.
+00000310: 0000 0072 1000 0000 7211 0000 00da 065f  ...r....r......_
+00000320: 5f65 715f 5f10 0000 0073 0e00 0000 0001  _eq__....s......
+00000330: 0a01 0402 1401 16ff 0202 0afd 7a0b 5275  ............z.Ru
+00000340: 6c65 2e5f 5f65 715f 5f4e a901 7214 0000  le.__eq__N..r...
+00000350: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00000360: 0000 0200 0000 4300 0000 7318 0000 007c  ......C...s....|
+00000370: 006a 00a0 01a1 0001 007c 006a 02a0 01a1  .j.......|.j....
+00000380: 0001 0064 0053 00a9 014e 2903 7209 0000  ...d.S...N).r...
+00000390: 0072 1800 0000 720a 0000 00a9 0172 0e00  .r....r......r..
+000003a0: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
+000003b0: 00da 0973 6f72 745f 7275 6c65 1900 0000  ...sort_rule....
+000003c0: 7304 0000 0000 010a 017a 0e52 756c 652e  s........z.Rule.
+000003d0: 736f 7274 5f72 756c 6563 0100 0000 0000  sort_rulec......
+000003e0: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+000003f0: 0000 732e 0000 007c 006a 0064 016b 0272  ..s....|.j.d.k.r
+00000400: 1a7c 006a 017c 006a 027c 006a 0367 0353  .|.j.|.j.|.j.g.S
+00000410: 007c 006a 017c 006a 027c 006a 037c 006a  .|.j.|.j.|.j.|.j
+00000420: 0467 0453 0072 1500 0000 2905 720c 0000  .g.S.r....).r...
+00000430: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000440: 720d 0000 0072 1c00 0000 7210 0000 0072  r....r....r....r
+00000450: 1000 0000 7211 0000 00da 0774 6f5f 6c69  ....r......to_li
+00000460: 7374 1d00 0000 7310 0000 0000 0308 ff12  st....s.........
+00000470: 0304 0104 0104 0104 fc02 fd7a 0c52 756c  ...........z.Rul
+00000480: 652e 746f 5f6c 6973 7429 0146 290c da08  e.to_list).F)...
+00000490: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+000004a0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+000004b0: 5f5f 7212 0000 00da 066f 626a 6563 74da  __r......object.
+000004c0: 0462 6f6f 6c72 1900 0000 721d 0000 0072  .boolr....r....r
+000004d0: 0300 0000 7204 0000 00da 0373 7472 721e  ....r......strr.
+000004e0: 0000 0072 1000 0000 7210 0000 0072 1000  ...r....r....r..
+000004f0: 0000 7211 0000 0072 0500 0000 0500 0000  ..r....r........
+00000500: 7308 0000 0008 010a 0a10 090e 0472 0500  s............r..
+00000510: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000520: 0000 0008 0000 0040 0000 0073 0a01 0000  .......@...s....
+00000530: 6500 5a01 6400 5a02 6423 6503 6504 1900  e.Z.d.Z.d#e.e...
+00000540: 6402 9c01 6403 6404 8405 5a05 6405 6406  d...d.d...Z.d.d.
+00000550: 8400 5a06 6507 6508 6407 9c02 6408 6409  ..Z.e.e.d...d.d.
+00000560: 8404 5a09 6401 640a 9c01 640b 640c 8404  ..Z.d.d...d.d...
+00000570: 5a0a 650b 640d 9c01 640e 640f 8404 5a0c  Z.e.d...d.d...Z.
+00000580: 650b 640d 9c01 6410 6411 8404 5a0d 6424  e.d...d.d...Z.d$
+00000590: 650e 650b 6503 6503 650f 6503 650b 1900  e.e.e.e.e.e.e...
+000005a0: 650b 6602 1900 1900 1900 6602 1900 6508  e.f.......f...e.
+000005b0: 6413 9c02 6414 6415 8405 5a10 6425 650b  d...d.d...Z.d%e.
+000005c0: 6508 6416 9c02 6417 6418 8405 5a11 650b  e.d...d.d...Z.e.
+000005d0: 6419 9c01 641a 641b 8404 5a12 6504 641c  d...d.d...Z.e.d.
+000005e0: 9c01 641d 641e 8404 5a13 650e 650b 6503  ..d.d...Z.e.e.e.
+000005f0: 6503 650f 6503 650b 1900 650b 6602 1900  e.e.e.e...e.f...
+00000600: 1900 1900 6602 1900 640a 9c01 641f 6420  ....f...d...d.d 
+00000610: 8404 5a14 6503 6503 650f 6503 650b 1900  ..Z.e.e.e.e.e...
+00000620: 650b 6602 1900 1900 1900 640a 9c01 6421  e.f.......d...d!
+00000630: 6422 8404 5a15 6401 5300 2926 da07 5275  d"..Z.d.S.)&..Ru
+00000640: 6c65 5365 744e a901 da05 7275 6c65 7363  leSetN....rulesc
+00000650: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000660: 0200 0000 4300 0000 731a 0000 007c 0164  ....C...s....|.d
+00000670: 0075 0072 1067 007c 005f 006e 067c 017c  .u.r.g.|._.n.|.|
+00000680: 005f 0064 0053 0072 1b00 0000 7226 0000  ._.d.S.r....r&..
+00000690: 0029 0272 0e00 0000 7227 0000 0072 1000  .).r....r'...r..
+000006a0: 0000 7210 0000 0072 1100 0000 7212 0000  ..r....r....r...
+000006b0: 002b 0000 0073 0600 0000 0001 0801 0802  .+...s..........
+000006c0: 7a10 5275 6c65 5365 742e 5f5f 696e 6974  z.RuleSet.__init
+000006d0: 5f5f 6301 0000 0000 0000 0000 0000 0002  __c.............
+000006e0: 0000 0002 0000 0063 0000 0073 1600 0000  .......c...s....
+000006f0: 7c00 6a00 4400 5d0a 7d01 7c01 5600 0100  |.j.D.].}.|.V...
+00000700: 7106 6400 5300 721b 0000 0072 2600 0000  q.d.S.r....r&...
+00000710: a902 720e 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00000720: 0072 1000 0000 7211 0000 00da 085f 5f69  .r....r......__i
+00000730: 7465 725f 5f31 0000 0073 0400 0000 0001  ter__1...s......
+00000740: 0a01 7a10 5275 6c65 5365 742e 5f5f 6974  ..z.RuleSet.__it
+00000750: 6572 5f5f 2902 da0b 5f52 756c 6553 6574  er__)..._RuleSet
+00000760: 5f5f 6f72 1400 0000 6302 0000 0000 0000  __or....c.......
+00000770: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
+00000780: 0073 1a00 0000 7400 7c01 7401 8302 730e  .s....t.|.t...s.
+00000790: 6401 5300 7c00 6a02 7c01 6a02 6b02 5300  d.S.|.j.|.j.k.S.
+000007a0: 7215 0000 0029 0372 1600 0000 7225 0000  r....).r....r%..
+000007b0: 0072 2700 0000 2902 720e 0000 0072 2a00  .r'...).r....r*.
+000007c0: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
+000007d0: 0072 1900 0000 3500 0000 7306 0000 0000  .r....5...s.....
+000007e0: 010a 0104 017a 0e52 756c 6553 6574 2e5f  .....z.RuleSet._
+000007f0: 5f65 715f 5f72 1a00 0000 6301 0000 0000  _eq__r....c.....
+00000800: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00000810: 0000 0073 2a00 0000 7c00 6a00 4400 5d0c  ...s*...|.j.D.].
+00000820: 7d01 7c01 a001 a100 0100 7106 7c00 6a00  }.|.......q.|.j.
+00000830: 6a02 6401 6402 8400 6403 8d01 0100 6400  j.d.d...d.....d.
+00000840: 5300 2904 4e63 0100 0000 0000 0000 0000  S.).Nc..........
+00000850: 0000 0100 0000 0500 0000 5300 0000 731c  ..........S...s.
+00000860: 0000 007c 006a 0064 01a0 017c 006a 02a1  ...|.j.d...|.j..
+00000870: 0164 01a0 017c 006a 03a1 0166 0353 0029  .d...|.j...f.S.)
+00000880: 024e fa01 3b29 0472 0b00 0000 da04 6a6f  .N..;).r......jo
+00000890: 696e 7209 0000 0072 0a00 0000 a901 720f  inr....r......r.
+000008a0: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
+000008b0: 0000 da08 3c6c 616d 6264 613e 3f00 0000  ....<lambda>?...
+000008c0: 7308 0000 0000 0104 010a 010a fd7a 2452  s............z$R
+000008d0: 756c 6553 6574 2e73 6f72 745f 7275 6c65  uleSet.sort_rule
+000008e0: 732e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  s.<locals>.<lamb
+000008f0: 6461 3e29 01da 036b 6579 2903 7227 0000  da>)...key).r'..
+00000900: 0072 1d00 0000 7218 0000 0072 2800 0000  .r....r....r(...
+00000910: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
+00000920: 0a73 6f72 745f 7275 6c65 733a 0000 0073  .sort_rules:...s
+00000930: 0a00 0000 0001 0a01 0a02 0601 06ff 7a12  ..............z.
+00000940: 5275 6c65 5365 742e 736f 7274 5f72 756c  RuleSet.sort_rul
+00000950: 6573 2901 da08 7473 765f 7061 7468 6302  es)...tsv_pathc.
+00000960: 0000 0000 0000 0000 0000 0009 0000 0008  ................
+00000970: 0000 0043 0000 0073 a200 0000 7c00 a000  ...C...s....|...
+00000980: a100 0100 7401 7c01 6401 8302 8f7c 7d02  ....t.|.d....|}.
+00000990: 7c00 6a02 4400 5d64 7d03 6402 a003 7c03  |.j.D.]d}.d...|.
+000009a0: 6a04 a101 7d04 6402 a003 7c03 6a05 a101  j...}.d...|.j...
+000009b0: 7d05 7c03 6a06 7d06 7c03 6a07 7d07 7c06  }.|.j.}.|.j.}.|.
+000009c0: 9b00 6403 7c04 9b00 6403 7c05 9b00 9d05  ..d.|...d.|.....
+000009d0: 7d08 7c03 6a08 7270 7c08 6403 7409 a00a  }.|.j.rp|.d.t...
+000009e0: 7c07 a101 9b00 9d02 3700 7d08 7c02 a00b  |.......7.}.|...
+000009f0: 7c08 6404 1700 a101 0100 711a 5700 6400  |.d.......q.W.d.
+00000a00: 0400 0400 8303 0100 6e10 3100 7394 3000  ........n.1.s.0.
+00000a10: 0100 0100 0100 5900 0100 6400 5300 2905  ......Y...d.S.).
+00000a20: 4eda 0177 722b 0000 00fa 0109 da01 0a29  N..wr+.........)
+00000a30: 0c72 3000 0000 da04 6f70 656e 7227 0000  .r0.....openr'..
+00000a40: 0072 2c00 0000 7209 0000 0072 0a00 0000  .r,...r....r....
+00000a50: 720b 0000 0072 0d00 0000 720c 0000 00da  r....r....r.....
+00000a60: 046a 736f 6eda 0564 756d 7073 da05 7772  .json..dumps..wr
+00000a70: 6974 6529 0972 0e00 0000 7231 0000 00da  ite).r....r1....
+00000a80: 0166 720f 0000 0072 0900 0000 720a 0000  .fr....r....r...
+00000a90: 0072 0b00 0000 720d 0000 005a 0872 756c  .r....r....Z.rul
+00000aa0: 655f 7374 7272 1000 0000 7210 0000 0072  e_strr....r....r
+00000ab0: 1100 0000 da06 746f 5f74 7376 4600 0000  ......to_tsvF...
+00000ac0: 7316 0000 0000 0108 010c 010a 010c 010c  s...............
+00000ad0: 0106 0106 0214 0206 0114 017a 0e52 756c  ...........z.Rul
+00000ae0: 6553 6574 2e74 6f5f 7473 7663 0200 0000  eSet.to_tsvc....
+00000af0: 0000 0000 0000 0000 0900 0000 0800 0000  ................
+00000b00: 4300 0000 7326 0100 0074 007c 0164 0183  C...s&...t.|.d..
+00000b10: 0290 018f 047d 027c 0244 005d ee7d 037c  .....}.|.D.].}.|
+00000b20: 03a0 0164 02a1 017d 037c 03a0 0264 03a1  ...d...}.|...d..
+00000b30: 017d 037c 0364 0419 0064 056b 0272 3a67  .}.|.d...d.k.r:g
+00000b40: 006e 0c7c 0364 0419 00a0 0264 06a1 017d  .n.|.d.....d...}
+00000b50: 047c 0364 0719 0064 056b 0272 5867 006e  .|.d...d.k.rXg.n
+00000b60: 0c7c 0364 0719 00a0 0264 06a1 017d 057c  .|.d.....d...}.|
+00000b70: 0364 0819 00a0 01a1 007d 0664 007d 0774  .d.......}.d.}.t
+00000b80: 037c 0383 0164 096b 0272 9674 047c 047c  .|...d.k.r.t.|.|
+00000b90: 057c 0667 0364 0a64 0b8d 027d 076e 4e74  .|.g.d.d...}.nNt
+00000ba0: 037c 0383 0164 0c6b 0272 d67c 0364 0919  .|...d.k.r.|.d..
+00000bb0: 0064 056b 0272 b267 006e 0c74 05a0 067c  .d.k.r.g.n.t...|
+00000bc0: 0364 0919 00a1 017d 0874 047c 047c 057c  .d.....}.t.|.|.|
+00000bd0: 067c 0867 0464 0d64 0b8d 027d 076e 0e74  .|.g.d.d...}.n.t
+00000be0: 0764 0e7c 039b 009d 0283 0182 017c 0773  .d.|.........|.s
+00000bf0: f674 0764 0f7c 039b 009d 0283 0182 017c  .t.d.|.........|
+00000c00: 00a0 087c 07a1 0101 0071 1257 0064 0004  ...|.....q.W.d..
+00000c10: 0004 0083 0301 006e 1231 0090 0173 1830  .......n.1...s.0
+00000c20: 0001 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
+00000c30: 104e da01 7272 3400 0000 7233 0000 0072  .N..rr4...r3...r
+00000c40: 0600 0000 da00 722b 0000 0072 0700 0000  ......r+...r....
+00000c50: 7201 0000 0072 0800 0000 46a9 0172 0c00  r....r....F..r..
+00000c60: 0000 e904 0000 0054 7a1a 496e 7661 6c69  .......Tz.Invali
+00000c70: 6420 6e75 6d62 6572 206f 6620 6669 656c  d number of fiel
+00000c80: 6473 3a20 7a0e 496e 7661 6c69 6420 7275  ds: z.Invalid ru
+00000c90: 6c65 3a20 2909 7235 0000 00da 0573 7472  le: ).r5.....str
+00000ca0: 6970 da05 7370 6c69 74da 036c 656e 7205  ip..split..lenr.
+00000cb0: 0000 0072 3600 0000 da05 6c6f 6164 73da  ...r6.....loads.
+00000cc0: 0945 7863 6570 7469 6f6e da08 6164 645f  .Exception..add_
+00000cd0: 7275 6c65 2909 720e 0000 0072 3100 0000  rule).r....r1...
+00000ce0: 7239 0000 00da 046c 696e 6572 0900 0000  r9.....liner....
+00000cf0: 720a 0000 0072 0b00 0000 720f 0000 0072  r....r....r....r
+00000d00: 0d00 0000 7210 0000 0072 1000 0000 7211  ....r....r....r.
+00000d10: 0000 00da 0866 726f 6d5f 7473 7655 0000  .....from_tsvU..
+00000d20: 0073 2c00 0000 0001 0e01 0801 0a01 0a02  .s,.............
+00000d30: 1e01 1e01 0c01 0401 0c01 0201 0aff 0803  ................
+00000d40: 0c01 1e01 0201 0a01 02fe 0805 0e02 0401  ................
+00000d50: 0e01 7a10 5275 6c65 5365 742e 6672 6f6d  ..z.RuleSet.from
+00000d60: 5f74 7376 4629 0272 2700 0000 720c 0000  _tsvF).r'...r...
+00000d70: 0063 0300 0000 0000 0000 0000 0000 0600  .c..............
+00000d80: 0000 0800 0000 4300 0000 7332 0000 007c  ......C...s2...|
+00000d90: 01a0 00a1 0044 005d 245c 027d 037d 047c  .....D.]$\.}.}.|
+00000da0: 0444 005d 167d 057c 00a0 0174 027c 057c  .D.].}.|...t.|.|
+00000db0: 0264 018d 02a1 0101 0071 1471 0864 0053  .d.......q.q.d.S
+00000dc0: 0029 024e 723d 0000 0029 03da 0569 7465  .).Nr=...)...ite
+00000dd0: 6d73 7244 0000 0072 0500 0000 2906 720e  msrD...r....).r.
+00000de0: 0000 0072 2700 0000 720c 0000 0072 2f00  ...r'...r....r/.
+00000df0: 0000 da05 7661 6c75 6572 0f00 0000 7210  ....valuer....r.
+00000e00: 0000 0072 1000 0000 7211 0000 00da 0966  ...r....r......f
+00000e10: 726f 6d5f 6469 6374 7000 0000 7306 0000  rom_dictp...s...
+00000e20: 0000 0310 0108 017a 1152 756c 6553 6574  .......z.RuleSet
+00000e30: 2e66 726f 6d5f 6469 6374 2902 da09 6a73  .from_dict)...js
+00000e40: 6f6e 5f70 6174 6872 0c00 0000 6303 0000  on_pathr....c...
+00000e50: 0000 0000 0000 0000 0008 0000 0008 0000  ................
+00000e60: 0043 0000 0073 6600 0000 7400 7c01 6401  .C...sf...t.|.d.
+00000e70: 8302 8f1a 7d03 7401 a002 7c03 a101 7d04  ....}.t...|...}.
+00000e80: 5700 6400 0400 0400 8303 0100 6e10 3100  W.d.........n.1.
+00000e90: 732a 3000 0100 0100 0100 5900 0100 7c04  s*0.......Y...|.
+00000ea0: a003 a100 4400 5d24 5c02 7d05 7d06 7c06  ....D.]$\.}.}.|.
+00000eb0: 4400 5d16 7d07 7c00 a004 7405 7c07 7c02  D.].}.|...t.|.|.
+00000ec0: 6402 8d02 a101 0100 7148 713c 6400 5300  d.......qHq<d.S.
+00000ed0: 2903 4e72 3b00 0000 723d 0000 0029 0672  ).Nr;...r=...).r
+00000ee0: 3500 0000 7236 0000 00da 046c 6f61 6472  5...r6.....loadr
+00000ef0: 4700 0000 7244 0000 0072 0500 0000 2908  G...rD...r....).
+00000f00: 720e 0000 0072 4a00 0000 720c 0000 0072  r....rJ...r....r
+00000f10: 3900 0000 7227 0000 0072 2f00 0000 7248  9...r'...r/...rH
+00000f20: 0000 0072 0f00 0000 7210 0000 0072 1000  ...r....r....r..
+00000f30: 0000 7211 0000 00da 0966 726f 6d5f 6a73  ..r......from_js
+00000f40: 6f6e 7700 0000 730a 0000 0000 010c 0128  onw...s........(
+00000f50: 0210 0108 017a 1152 756c 6553 6574 2e66  .....z.RuleSet.f
+00000f60: 726f 6d5f 6a73 6f6e 2901 724a 0000 0063  rom_json).rJ...c
+00000f70: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00000f80: 0800 0000 4300 0000 733e 0000 0074 007c  ....C...s>...t.|
+00000f90: 0164 0183 028f 207d 0274 01a0 027c 00a0  .d.... }.t...|..
+00000fa0: 03a1 007c 02a1 0201 0057 0064 0004 0004  ...|.....W.d....
+00000fb0: 0083 0301 006e 1031 0073 3030 0001 0001  .....n.1.s00....
+00000fc0: 0001 0059 0001 0064 0053 0029 024e 7232  ...Y...d.S.).Nr2
+00000fd0: 0000 0029 0472 3500 0000 7236 0000 00da  ...).r5...r6....
+00000fe0: 0464 756d 70da 0774 6f5f 6469 6374 2903  .dump..to_dict).
+00000ff0: 720e 0000 0072 4a00 0000 7239 0000 0072  r....rJ...r9...r
+00001000: 1000 0000 7210 0000 0072 1100 0000 da07  ....r....r......
+00001010: 746f 5f6a 736f 6e7f 0000 0073 0400 0000  to_json....s....
+00001020: 0001 0c01 7a0f 5275 6c65 5365 742e 746f  ....z.RuleSet.to
+00001030: 5f6a 736f 6e72 2d00 0000 6302 0000 0000  _jsonr-...c.....
+00001040: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00001050: 0000 0073 1000 0000 7c00 6a00 a001 7c01  ...s....|.j...|.
+00001060: a101 0100 6400 5300 721b 0000 0029 0272  ....d.S.r....).r
+00001070: 2700 0000 da06 6170 7065 6e64 7228 0000  '.....appendr(..
+00001080: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
+00001090: 7244 0000 0083 0000 0073 0200 0000 0001  rD.......s......
+000010a0: 7a10 5275 6c65 5365 742e 6164 645f 7275  z.RuleSet.add_ru
+000010b0: 6c65 6301 0000 0000 0000 0000 0000 0003  lec.............
+000010c0: 0000 0005 0000 0043 0000 0073 3400 0000  .......C...s4...
+000010d0: 6401 6402 8400 7c00 6a00 4400 8301 7d01  d.d...|.j.D...}.
+000010e0: 7c00 6a00 4400 5d18 7d02 7c01 7c02 6a01  |.j.D.].}.|.|.j.
+000010f0: 1900 a002 7c02 a003 a100 a101 0100 7116  ....|.........q.
+00001100: 7c01 5300 2903 4e63 0100 0000 0000 0000  |.S.).Nc........
+00001110: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
+00001120: 7314 0000 0069 007c 005d 0c7d 017c 016a  s....i.|.].}.|.j
+00001130: 0067 0093 0271 0453 0072 1000 0000 2901  .g...q.S.r....).
+00001140: 720b 0000 00a9 02da 022e 3072 0f00 0000  r.........0r....
+00001150: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
+00001160: 0a3c 6469 6374 636f 6d70 3e87 0000 00f3  .<dictcomp>.....
+00001170: 0000 0000 7a23 5275 6c65 5365 742e 746f  ....z#RuleSet.to
+00001180: 5f64 6963 742e 3c6c 6f63 616c 733e 2e3c  _dict.<locals>.<
+00001190: 6469 6374 636f 6d70 3e29 0472 2700 0000  dictcomp>).r'...
+000011a0: 720b 0000 0072 5000 0000 721e 0000 0029  r....rP...r....)
+000011b0: 0372 0e00 0000 5a09 7275 6c65 5f64 6963  .r....Z.rule_dic
+000011c0: 7472 0f00 0000 7210 0000 0072 1000 0000  tr....r....r....
+000011d0: 7211 0000 0072 4e00 0000 8600 0000 7308  r....rN.......s.
+000011e0: 0000 0000 0110 020a 0116 027a 0f52 756c  ...........z.Rul
+000011f0: 6553 6574 2e74 6f5f 6469 6374 6301 0000  eSet.to_dictc...
+00001200: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00001210: 0043 0000 0073 1000 0000 6401 6402 8400  .C...s....d.d...
+00001220: 7c00 6a00 4400 8301 5300 2903 4e63 0100  |.j.D...S.).Nc..
+00001230: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00001240: 0000 5300 0000 7314 0000 0067 007c 005d  ..S...s....g.|.]
+00001250: 0c7d 017c 01a0 00a1 0091 0271 0453 0072  .}.|.......q.S.r
+00001260: 1000 0000 2901 721e 0000 0072 5100 0000  ....).r....rQ...
+00001270: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
+00001280: 0a3c 6c69 7374 636f 6d70 3e8f 0000 0072  .<listcomp>....r
+00001290: 5400 0000 7a23 5275 6c65 5365 742e 746f  T...z#RuleSet.to
+000012a0: 5f6c 6973 742e 3c6c 6f63 616c 733e 2e3c  _list.<locals>.<
+000012b0: 6c69 7374 636f 6d70 3e72 2600 0000 721c  listcomp>r&...r.
+000012c0: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
+000012d0: 0000 721e 0000 008e 0000 0073 0200 0000  ..r........s....
+000012e0: 0001 7a0f 5275 6c65 5365 742e 746f 5f6c  ..z.RuleSet.to_l
+000012f0: 6973 7429 014e 2901 4629 0146 2916 721f  ist).N).F).F).r.
+00001300: 0000 0072 2000 0000 7221 0000 0072 0300  ...r ...r!...r..
+00001310: 0000 7205 0000 0072 1200 0000 7229 0000  ..r....r....r)..
+00001320: 0072 2200 0000 7223 0000 0072 1900 0000  .r"...r#...r....
+00001330: 7230 0000 0072 2400 0000 723a 0000 0072  r0...r$...r:...r
+00001340: 4600 0000 7202 0000 0072 0400 0000 7249  F...r....r....rI
+00001350: 0000 0072 4c00 0000 724f 0000 0072 4400  ...rL...rO...rD.
+00001360: 0000 724e 0000 0072 1e00 0000 7210 0000  ..rN...r....r...
+00001370: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
+00001380: 7225 0000 002a 0000 0073 1e00 0000 0801  r%...*...s......
+00001390: 1406 0804 1005 0e0c 0e0f 0e1c 00ff 0201  ................
+000013a0: 20ff 0c07 1208 0e04 0e03 2a08 7225 0000   .........*.r%..
+000013b0: 0029 0772 3600 0000 da06 7479 7069 6e67  .).r6.....typing
+000013c0: 7202 0000 0072 0300 0000 7204 0000 0072  r....r....r....r
+000013d0: 0500 0000 7225 0000 0072 1000 0000 7210  ....r%...r....r.
+000013e0: 0000 0072 1000 0000 7211 0000 00da 083c  ...r....r......<
+000013f0: 6d6f 6475 6c65 3e01 0000 0073 0600 0000  module>....s....
+00001400: 0801 1403 0e25                           .....%
```

### Comparing `xpotato-0.1.4/xpotato/graph_extractor/extract.py` & `xpotato-0.1.5/xpotato/graph_extractor/extract.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,86 +1,144 @@
 import json
 import os
 from collections import defaultdict
 
 import networkx as nx
 import pandas as pd
-import stanza
 import penman as pn
-from networkx.algorithms.isomorphism import DiGraphMatcher
 from sklearn.metrics import precision_recall_fscore_support
 from tqdm import tqdm
-from tuw_nlp.grammar.text_to_4lang import TextTo4lang
-from tuw_nlp.graph.utils import (
-    GraphFormulaMatcher,
-    GraphFormulaPatternMatcher,
-)
-from tuw_nlp.text.pipeline import CachedStanzaPipeline
+from tuw_nlp.graph.utils import GraphFormulaPatternMatcher
 
-from xpotato.dataset.utils import default_pn_to_graph, ud_to_graph, amr_pn_to_graph
+from xpotato.dataset.utils import amr_pn_to_graph, default_pn_to_graph, ud_to_graph
 
 
 class GraphExtractor:
     def __init__(self, cache_dir=None, cache_fn=None, lang=None):
         if cache_dir is None:
             cache_dir = os.path.join(os.path.dirname(__file__), "cache")
         if cache_fn is None:
             cache_fn = os.path.join(cache_dir, f"{lang}_nlp_cache.json")
         self.cache_dir = cache_dir
         self.cache_fn = cache_fn
         self.lang = lang
-        self.nlp = None
         self.matcher = None
-        self.amr_stog = None
 
-    def init_amr(self):
-        if self.amr_stog == None:
-            import amrlib
-
-            self.amr_stog = amrlib.load_stog_model()
-
-    def init_nlp(self):
-        if self.nlp == None:
-            if self.lang == "en_bio":
-                nlp = stanza.Pipeline("en", package="craft")
-            else:
-                nlp = stanza.Pipeline(self.lang)
-            self.nlp = CachedStanzaPipeline(nlp, self.cache_fn)
+        self.ud_parser = None
+        self.fl_parser = None
+        self.amr_parser = None
+        self.ucca_parser = None
+        self.sdp_parser = None
+        self.drs_parser = None
+
+    def init_resources(self, graph_type):
+        if graph_type == "ud":
+            if self.ud_parser == None:
+                from tuw_nlp.grammar.text_to_ud import TextToUD
+
+                self.ud_parser = TextToUD(
+                    lang=self.lang, nlp_cache=self.cache_fn, cache_dir=self.cache_dir
+                )
+
+        elif graph_type == "fourlang":
+            if self.fl_parser == None:
+                from tuw_nlp.grammar.text_to_4lang import TextTo4lang
+
+                self.fl_parser = TextTo4lang(
+                    lang=self.lang, nlp_cache=self.cache_fn, cache_dir=self.cache_dir
+                )
+
+        elif graph_type == "amr":
+            if self.amr_parser == None:
+                if self.lang != "en":
+                    raise ValueError(
+                        f"Currently only english AMR is supported: {self.lang}"
+                    )
+                from tuw_nlp.grammar.text_to_amr import TextToAMR
+
+                self.amr_parser = TextToAMR()
+
+        elif graph_type == "ucca":
+            if self.ucca_parser == None:
+                if self.lang != "en":
+                    raise ValueError(
+                        f"Currently only english UCCA is supported: {self.lang}"
+                    )
+                from tuw_nlp.grammar.text_to_ucca import TextToUCCA
+
+                self.ucca_parser = TextToUCCA()
+
+        elif graph_type == "sdp":
+            if self.sdp_parser == None:
+                if self.lang != "en":
+                    raise ValueError(
+                        f"Currently only english SDP is supported: {self.lang}"
+                    )
+                from tuw_nlp.grammar.text_to_sdp import TextToSDP
+
+                self.sdp_parser = TextToSDP(lang=self.lang)
+        elif graph_type == "drs":
+            if self.drs_parser == None:
+                if self.lang != "en":
+                    raise ValueError(
+                        f"Currently only english DRS is supported: {self.lang}"
+                    )
+                from tuw_nlp.grammar.text_to_drs import TextToDRS
+
+                self.drs_parser = TextToDRS(lang=self.lang)
+
+        else:
+            raise ValueError(f"Currently not supported: {graph_type}")
 
     def parse_iterable(self, iterable, graph_type="fourlang", lang=None):
         if lang:
             self.lang = lang
+        self.init_resources(graph_type)
         if graph_type == "fourlang":
-            with TextTo4lang(
-                lang=self.lang, nlp_cache=self.cache_fn, cache_dir=self.cache_dir
-            ) as tfl:
+            with self.fl_parser as tfl:
                 for sen in tqdm(iterable):
                     fl_graphs = list(tfl(sen, ssplit=False))
                     g = fl_graphs[0]
                     for n in fl_graphs[1:]:
                         raise ValueError(f"sentence should not be split up: {sen}!")
-                        g = nx.compose(g, n)
                     yield g
 
         elif graph_type == "ud":
-            self.init_nlp()
             for sen in tqdm(iterable):
-                doc = self.nlp(sen)
-                g, _ = ud_to_graph(doc.sentences[0])
-                for doc_sen in doc.sentences[1:]:
-                    n, _ = ud_to_graph(doc_sen)
-                    g = nx.compose(g, n)
+                ud_graphs = list(self.ud_parser(sen, ssplit=False))
+                g = ud_graphs[0]
+                for n in ud_graphs[1:]:
+                    raise ValueError(f"sentence should not be split up: {sen}!")
                 yield g
 
         elif graph_type == "amr":
-            self.init_amr()
             for sen in tqdm(iterable):
-                graphs = self.amr_stog.parse_sents([sen])
-                g, _ = amr_pn_to_graph(graphs[0])
-                yield g
+                g = self.amr_parser(sen)
+
+                yield list(g)[0]
+
+        elif graph_type == "ucca":
+            for sen in tqdm(iterable):
+                g = self.ucca_parser(sen)
+
+                yield list(g)[0]
+
+        elif graph_type == "sdp":
+            for sen in tqdm(iterable):
+                g = self.sdp_parser(sen)
+
+                yield list(g)[0]
+
+        elif graph_type == "drs":
+            for sen in tqdm(iterable):
+                g = self.drs_parser(sen)
+
+                yield list(g)[0]
+        else:
+            raise ValueError(f"Currrently not supported: {graph_type}")
 
 
 class FeatureEvaluator:
     def __init__(self, graph_format="ud", case_sensitive=False):
         self.graph_format = graph_format
         self.case_sensitive = case_sensitive
 
@@ -106,15 +164,15 @@
                 p = pn.decode(negative)
                 first = p.triples[0][0]
                 assert first == "u_0", f"The IDs must start from 0, not {first}"
 
             feature_to_marked_nodes[i] = feature[3]
             features[i] = feature[:3]
 
-        matcher = GraphFormulaMatcher(
+        matcher = GraphFormulaPatternMatcher(
             features, converter=default_pn_to_graph, case_sensitive=self.case_sensitive
         )
         feats = matcher.match(graph, return_subgraphs=True)
 
         for key, i, subgraphs in feats:
             triplet = {"relation": key}
             marked_nodes = feature_to_marked_nodes[i]
@@ -268,15 +326,19 @@
 
         def rank(feature):
             return len(df.iloc[features.index(feature[0])].True_positive_graphs)
 
         return sorted(features_stat, key=rank, reverse=True)
 
     def train_feature(self, cl, feature, data, graph_format="ud"):
-        graph_matcher = GraphFormulaPatternMatcher([[[feature], [], []]], default_pn_to_graph, case_sensitive=self.case_sensitive)
+        graph_matcher = GraphFormulaPatternMatcher(
+            [[[feature], [], []]],
+            default_pn_to_graph,
+            case_sensitive=self.case_sensitive,
+        )
         feat_patt = graph_matcher.patts[0][0]
         if isinstance(feat_patt[0], tuple):
             if len(feat_patt[0][1]) == 2:
                 patt1, patt2 = feat_patt[0][1]
             else:
                 _, patt1, patt2 = feat_patt[0][1]
         else:
@@ -284,24 +346,36 @@
 
         graphs = data.graph.tolist()
         labels = self.one_versus_rest(data, cl).one_versus_rest.tolist()
         path = "trained_features.tsv"
         trained_features = []
         with open(path, "w+") as f:
             for i, g in enumerate(graphs):
-                matches = [(i, subgraph) for (key, i, subgraph) in graph_matcher.match(g, return_subgraphs=True)]
+                matches = [
+                    (i, subgraph)
+                    for (key, i, subgraph) in graph_matcher.match(
+                        g, return_subgraphs=True
+                    )
+                ]
                 for patt_index, match in matches:
                     for graph in match:
                         nodes = []
                         for node_index, node in graph.nodes(data=True):
                             if not nodes:
-                                node_name = node['name']
-                                if node['mapping'] in patt1.nodes and patt1.nodes[node['mapping']]["name"] == ".*":
+                                node_name = node["name"]
+                                if (
+                                    node["mapping"] in patt1.nodes
+                                    and patt1.nodes[node["mapping"]]["name"] == ".*"
+                                ):
                                     nodes.append(node_name)
-                                if patt2 is not None and node['mapping'] in patt2.nodes and patt2.nodes[node['mapping']]["name"] == ".*":
+                                if (
+                                    patt2 is not None
+                                    and node["mapping"] in patt2.nodes
+                                    and patt2.nodes[node["mapping"]]["name"] == ".*"
+                                ):
                                     nodes.append(node_name)
                         if not nodes:
                             g2_to_g1 = {v: u for (u, v, _) in graph.edges(data=True)}
                             for u, v, attrs in patt1.edges(data=True):
                                 if attrs["color"] == ".*":
                                     edge = g.get_edge_data(g2_to_g1[u], g2_to_g1[v])[
                                         "color"
```

### Comparing `xpotato-0.1.4/xpotato/graph_extractor/rule.py` & `xpotato-0.1.5/xpotato/graph_extractor/rule.py`

 * *Files identical despite different names*

### Comparing `xpotato-0.1.4/xpotato/models/__pycache__/model.cpython-39.pyc` & `xpotato-0.1.5/xpotato/models/__pycache__/model.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Dec 17 11:31:02 2021 UTC, .py size: 3395 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-00000000: 610d 0d0a 0000 0000 f674 bc61 430d 0000  a........t.aC...
+00000000: 610d 0d0a 0000 0000 b86f 9763 450d 0000  a........o.cE...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
-00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
+00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
+00000040: 5a03 6400 6403 6c04 6d05 5a05 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6400 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6407 6408 8400 6408 8302 5a0c  ..G.d.d...d...Z.
-00000080: 6401 5300 2909 e900 0000 004e 2901 da0b  d.S.)......N)...
-00000090: 6465 6661 756c 7464 6963 7429 01da 0a56  defaultdict)...V
+00000080: 6402 5300 2909 e900 0000 0029 01da 0b64  d.S.)......)...d
+00000090: 6566 6175 6c74 6469 6374 4e29 01da 0a56  efaultdictN)...V
 000000a0: 6f63 6162 756c 6172 7929 01da 094c 6578  ocabulary)...Lex
 000000b0: 4772 6170 6873 a901 da0b 6772 6170 685f  Graphs....graph_
 000000c0: 746f 5f70 6e29 01da 0c74 7265 655f 746f  to_pn)...tree_to
 000000d0: 5f63 6f64 6563 0000 0000 0000 0000 0000  _codec..........
 000000e0: 0000 0000 0000 0300 0000 4000 0000 7358  ..........@...sX
 000000f0: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
 00000100: 005a 0364 0364 0484 005a 0464 0564 0684  .Z.d.d...Z.d.d..
@@ -32,240 +32,241 @@
 000001f0: da0b 6c61 6265 6c5f 766f 6361 62da 066c  ..label_vocab..l
 00000200: 6162 656c 73da 0c66 6561 7473 5f62 795f  abels..feats_by_
 00000210: 7365 6eda 0773 656e 5f69 6473 da0a 766f  sen..sen_ids..vo
 00000220: 6361 625f 7369 7a65 da0c 7265 6c61 6265  cab_size..relabe
 00000230: 6c5f 6469 6374 da0f 696e 7665 7273 655f  l_dict..inverse_
 00000240: 7265 6c61 6265 6cda 0c72 616e 646f 6d5f  relabel..random_
 00000250: 7374 6174 65a9 01da 0473 656c 66a9 0072  state....self..r
-00000260: 1500 0000 fa35 2f68 6f6d 652f 6164 6161  .....5/home/adaa
-00000270: 6d6b 6f2f 7072 6f6a 6563 7473 2f50 4f54  mko/projects/POT
-00000280: 4154 4f2f 7870 6f74 6174 6f2f 6d6f 6465  ATO/xpotato/mode
-00000290: 6c73 2f6d 6f64 656c 2e70 79da 085f 5f69  ls/model.py..__i
-000002a0: 6e69 745f 5f0a 0000 0073 1400 0000 0001  nit__....s......
-000002b0: 0801 0801 0801 0601 0601 0601 0601 0601  ................
-000002c0: 0601 7a13 4772 6170 684d 6f64 656c 2e5f  ..z.GraphModel._
-000002d0: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-000002e0: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
-000002f0: 7312 0000 0064 0164 0284 007c 00a0 00a1  s....d.d...|....
-00000300: 0044 0083 0153 0029 034e 6301 0000 0000  .D...S.).Nc.....
-00000310: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-00000320: 0000 0073 1400 0000 6700 7c00 5d0c 7d01  ...s....g.|.].}.
-00000330: 7400 7c01 8301 9102 7104 5300 7215 0000  t.|.....q.S.r...
-00000340: 0072 0500 0000 2902 da02 2e30 da01 4772  .r....)....0..Gr
-00000350: 1500 0000 7215 0000 0072 1600 0000 da0a  ....r....r......
-00000360: 3c6c 6973 7463 6f6d 703e 1700 0000 f300  <listcomp>......
-00000370: 0000 007a 3847 7261 7068 4d6f 6465 6c2e  ...z8GraphModel.
-00000380: 6765 745f 6665 6174 7572 655f 6772 6170  get_feature_grap
-00000390: 685f 7374 7269 6e67 732e 3c6c 6f63 616c  h_strings.<local
-000003a0: 733e 2e3c 6c69 7374 636f 6d70 3e29 01da  s>.<listcomp>)..
-000003b0: 1267 6574 5f66 6561 7475 7265 5f67 7261  .get_feature_gra
-000003c0: 7068 7372 1300 0000 7215 0000 0072 1500  phsr....r....r..
-000003d0: 0000 7216 0000 00da 1967 6574 5f66 6561  ..r......get_fea
-000003e0: 7475 7265 5f67 7261 7068 5f73 7472 696e  ture_graph_strin
-000003f0: 6773 1600 0000 7302 0000 0000 017a 2447  gs....s......z$G
-00000400: 7261 7068 4d6f 6465 6c2e 6765 745f 6665  raphModel.get_fe
-00000410: 6174 7572 655f 6772 6170 685f 7374 7269  ature_graph_stri
-00000420: 6e67 7363 0100 0000 0000 0000 0000 0000  ngsc............
-00000430: 0100 0000 0300 0000 0300 0000 7316 0000  ............s...
-00000440: 0087 0066 0164 0164 0284 0888 00a0 00a1  ...f.d.d........
-00000450: 0044 0083 0153 0029 034e 6301 0000 0000  .D...S.).Nc.....
-00000460: 0000 0000 0000 0002 0000 0005 0000 0013  ................
-00000470: 0000 0073 1800 0000 6700 7c00 5d10 7d01  ...s....g.|.].}.
-00000480: 8800 6a00 a001 7c01 a101 9102 7104 5300  ..j...|.....q.S.
-00000490: 7215 0000 0029 0272 0900 0000 da0a 6672  r....).r......fr
-000004a0: 6f6d 5f74 7570 6c65 2902 7218 0000 00da  om_tuple).r.....
-000004b0: 0154 7213 0000 0072 1500 0000 7216 0000  .Tr....r....r...
-000004c0: 0072 1a00 0000 1a00 0000 721b 0000 007a  .r........r....z
-000004d0: 3147 7261 7068 4d6f 6465 6c2e 6765 745f  1GraphModel.get_
-000004e0: 6665 6174 7572 655f 6772 6170 6873 2e3c  feature_graphs.<
-000004f0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00000500: 703e 2901 da11 6765 745f 6665 6174 7572  p>)...get_featur
-00000510: 655f 6e61 6d65 7372 1300 0000 7215 0000  e_namesr....r...
-00000520: 0072 1300 0000 7216 0000 0072 1c00 0000  .r....r....r....
-00000530: 1900 0000 7302 0000 0000 017a 1d47 7261  ....s......z.Gra
-00000540: 7068 4d6f 6465 6c2e 6765 745f 6665 6174  phModel.get_feat
-00000550: 7572 655f 6772 6170 6873 6301 0000 0000  ure_graphsc.....
-00000560: 0000 0000 0000 0001 0000 0004 0000 0003  ................
-00000570: 0000 0073 1c00 0000 8700 6601 6401 6402  ...s......f.d.d.
-00000580: 8408 7400 7401 8800 6a02 8301 8301 4400  ..t.t...j.....D.
-00000590: 8301 5300 2903 4e63 0100 0000 0000 0000  ..S.).Nc........
-000005a0: 0000 0000 0200 0000 0500 0000 1300 0000  ................
-000005b0: 7318 0000 0067 007c 005d 107d 0188 006a  s....g.|.].}...j
-000005c0: 00a0 017c 01a1 0191 0271 0453 0072 1500  ...|.....q.S.r..
-000005d0: 0000 2902 720a 0000 00da 0867 6574 5f77  ..).r......get_w
-000005e0: 6f72 64a9 0272 1800 0000 da01 6972 1300  ord..r......ir..
-000005f0: 0000 7215 0000 0072 1600 0000 721a 0000  ..r....r....r...
-00000600: 001d 0000 0072 1b00 0000 7a30 4772 6170  .....r....z0Grap
-00000610: 684d 6f64 656c 2e67 6574 5f66 6561 7475  hModel.get_featu
-00000620: 7265 5f6e 616d 6573 2e3c 6c6f 6361 6c73  re_names.<locals
-00000630: 3e2e 3c6c 6973 7463 6f6d 703e 2903 da05  >.<listcomp>)...
-00000640: 7261 6e67 65da 036c 656e 720a 0000 0072  range..lenr....r
-00000650: 1300 0000 7215 0000 0072 1300 0000 7216  ....r....r....r.
-00000660: 0000 0072 2000 0000 1c00 0000 7302 0000  ...r .......s...
-00000670: 0000 017a 1c47 7261 7068 4d6f 6465 6c2e  ...z.GraphModel.
-00000680: 6765 745f 6665 6174 7572 655f 6e61 6d65  get_feature_name
-00000690: 7363 0300 0000 0000 0000 0000 0000 0800  sc..............
-000006a0: 0000 0800 0000 4300 0000 737a 0000 0074  ......C...sz...t
-000006b0: 0074 0183 017d 0374 027c 016a 0383 0144  .t...}.t.|.j...D
-000006c0: 005d 625c 027d 047d 0564 0164 0284 0074  .]b\.}.}.d.d...t
-000006d0: 0174 047c 057c 027c 006a 0583 0383 0144  .t.|.|.|.j.....D
-000006e0: 0083 017d 067c 0644 005d 387d 077c 0374  ...}.|.D.]8}.|.t
-000006f0: 017c 006a 066a 07a0 08a1 0083 017c 0419  .|.j.j.......|..
-00000700: 0019 00a0 097c 0764 0319 007c 0764 0419  .....|.d...|.d..
-00000710: 007c 006a 066a 0a7c 0419 0066 03a1 0101  .|.j.j.|...f....
-00000720: 0071 3a71 127c 0353 0029 054e 6301 0000  .q:q.|.S.).Nc...
-00000730: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000740: 0053 0000 0073 1800 0000 6700 7c00 5d10  .S...s....g.|.].
-00000750: 7d01 7c01 6400 1900 7204 7c01 9102 7104  }.|.d...r.|...q.
-00000760: 5300 2901 e902 0000 0072 1500 0000 7222  S.)......r....r"
-00000770: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-00000780: 0000 721a 0000 0023 0000 0073 0600 0000  ..r....#...s....
-00000790: 0602 0203 08fc 7a37 4772 6170 684d 6f64  ......z7GraphMod
-000007a0: 656c 2e63 6f6e 7665 7274 5f74 7265 655f  el.convert_tree_
-000007b0: 746f 5f66 6561 7475 7265 732e 3c6c 6f63  to_features.<loc
-000007c0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e72  als>.<listcomp>r
-000007d0: 0100 0000 e901 0000 0029 0b72 0200 0000  .........).r....
-000007e0: da04 6c69 7374 da09 656e 756d 6572 6174  ..list..enumerat
-000007f0: 65da 0b65 7374 696d 6174 6f72 735f 7207  e..estimators_r.
-00000800: 0000 0072 1100 0000 720b 0000 00da 0a77  ...r....r......w
-00000810: 6f72 645f 746f 5f69 64da 046b 6579 73da  ord_to_id..keys.
-00000820: 0661 7070 656e 64da 0a69 645f 746f 5f77  .append..id_to_w
-00000830: 6f72 6429 0872 1400 0000 da03 636c 66da  ord).r......clf.
-00000840: 1566 6561 7475 7265 5f67 7261 7068 5f73  .feature_graph_s
-00000850: 7472 696e 6773 da08 6665 6174 7572 6573  trings..features
-00000860: da01 6ada 0365 7374 da05 7061 7468 73da  ..j..est..paths.
-00000870: 0470 6174 6872 1500 0000 7215 0000 0072  .pathr....r....r
-00000880: 1600 0000 da18 636f 6e76 6572 745f 7472  ......convert_tr
-00000890: 6565 5f74 6f5f 6665 6174 7572 6573 1f00  ee_to_features..
-000008a0: 0000 7318 0000 0000 0108 0212 0106 0202  ..s.............
-000008b0: 010c ff02 fe06 0708 0118 0118 ff08 047a  ...............z
-000008c0: 2347 7261 7068 4d6f 6465 6c2e 636f 6e76  #GraphModel.conv
-000008d0: 6572 745f 7472 6565 5f74 6f5f 6665 6174  ert_tree_to_feat
-000008e0: 7572 6573 7227 0000 0063 0500 0000 0000  uresr'...c......
-000008f0: 0000 0000 0000 0800 0000 0700 0000 4300  ..............C.
-00000900: 0000 7364 0000 0074 0083 007d 057c 006a  ..sd...t...}.|.j
-00000910: 01a0 027c 01a1 0101 007c 006a 03a0 047c  ...|.....|.j...|
-00000920: 027c 04a1 0244 005d 1e5c 027d 067d 077c  .|...D.].\.}.}.|
-00000930: 05a0 057c 006a 066a 077c 0664 0164 028d  ...|.j.j.|.d.d..
-00000940: 02a1 0101 0071 207c 057c 006a 087c 013c  .....q |.|.j.|.<
-00000950: 007c 037c 006a 097c 013c 0074 0a7c 006a  .|.|.j.|.<.t.|.j
-00000960: 0683 017c 005f 0b64 0053 0029 034e 54a9  ...|._.d.S.).NT.
-00000970: 01da 0961 6c6c 6f77 5f6e 6577 290c da03  ...allow_new)...
-00000980: 7365 7472 0e00 0000 722d 0000 0072 0900  setr....r-...r..
-00000990: 0000 da11 6765 6e5f 6c65 785f 7375 6267  ....gen_lex_subg
-000009a0: 7261 7068 73da 0361 6464 720a 0000 00da  raphs..addr.....
-000009b0: 0667 6574 5f69 6472 0d00 0000 720c 0000  .get_idr....r...
-000009c0: 0072 2500 0000 720f 0000 0029 0872 1400  .r%...r....).r..
-000009d0: 0000 da06 7365 6e5f 6964 da05 6772 6170  ....sen_id..grap
-000009e0: 68da 0461 7474 72da 086d 6178 5f65 6467  h..attr..max_edg
-000009f0: 65da 0566 6561 7473 5a08 7367 5f74 7570  e..featsZ.sg_tup
-00000a00: 6c65 da02 7367 7215 0000 0072 1500 0000  le..sgr....r....
-00000a10: 7216 0000 00da 1366 6561 7475 7269 7a65  r......featurize
-00000a20: 5f73 656e 5f67 7261 7068 3100 0000 730e  _sen_graph1...s.
-00000a30: 0000 0000 0106 010c 0116 0118 020a 020a  ................
-00000a40: 017a 1e47 7261 7068 4d6f 6465 6c2e 6665  .z.GraphModel.fe
-00000a50: 6174 7572 697a 655f 7365 6e5f 6772 6170  aturize_sen_grap
-00000a60: 6863 0200 0000 0000 0000 0000 0000 0300  hc..............
-00000a70: 0000 0300 0000 0300 0000 7334 0000 007c  ..........s4...|
-00000a80: 006a 00a0 017c 01a1 015c 0289 007d 027c  .j...|...\...}.|
-00000a90: 027c 005f 0288 007c 005f 0387 0066 0164  .|._...|._...f.d
-00000aa0: 0164 0284 0888 0044 0083 017c 005f 0464  .d.....D...|._.d
-00000ab0: 0053 0029 034e 6301 0000 0000 0000 0000  .S.).Nc.........
-00000ac0: 0000 0002 0000 0004 0000 0013 0000 0073  ...............s
-00000ad0: 1600 0000 6900 7c00 5d0e 7d01 8800 7c01  ....i.|.].}...|.
-00000ae0: 1900 7c01 9302 7104 5300 7215 0000 0072  ..|...q.S.r....r
-00000af0: 1500 0000 a902 7218 0000 00da 016b a901  ......r......k..
-00000b00: 7210 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
-00000b10: 0a3c 6469 6374 636f 6d70 3e40 0000 0072  .<dictcomp>@...r
-00000b20: 1b00 0000 7a2c 4772 6170 684d 6f64 656c  ....z,GraphModel
-00000b30: 2e73 656c 6563 745f 6e5f 6265 7374 2e3c  .select_n_best.<
-00000b40: 6c6f 6361 6c73 3e2e 3c64 6963 7463 6f6d  locals>.<dictcom
-00000b50: 703e 2905 720a 0000 00da 0d73 656c 6563  p>).r......selec
-00000b60: 745f 6e5f 6265 7374 720f 0000 0072 1000  t_n_bestr....r..
-00000b70: 0000 7211 0000 0029 0372 1400 0000 da0c  ..r....).r......
-00000b80: 6d61 785f 6665 6174 7572 6573 da0b 6665  max_features..fe
-00000b90: 6174 7572 655f 6e75 6d72 1500 0000 7246  ature_numr....rF
-00000ba0: 0000 0072 1600 0000 7248 0000 003c 0000  ...r....rH...<..
-00000bb0: 0073 0800 0000 0001 1001 0601 0601 7a18  .s............z.
-00000bc0: 4772 6170 684d 6f64 656c 2e73 656c 6563  GraphModel.selec
-00000bd0: 745f 6e5f 6265 7374 6303 0000 0000 0000  t_n_bestc.......
-00000be0: 0000 0000 0007 0000 0006 0000 0003 0000  ................
-00000bf0: 0073 6e00 0000 7400 7401 8301 7d03 7402  .sn...t.t...}.t.
-00000c00: 7c02 8301 4400 5d22 5c02 7d04 7d05 7c03  |...D.]"\.}.}.|.
-00000c10: 7403 7c05 6a04 6401 6402 8d01 8301 1900  t.|.j.d.d.......
-00000c20: a005 7c04 a101 0100 7110 7c00 6a06 6a07  ..|.....q.|.j.j.
-00000c30: 7c01 7c03 6403 6404 8d03 5c02 8900 7d06  |.|.d.d...\...}.
-00000c40: 7c06 7c00 5f08 8800 7c00 5f09 8700 6601  |.|._...|._...f.
-00000c50: 6405 6406 8408 8800 4400 8301 7c00 5f0a  d.d.....D...|._.
-00000c60: 6400 5300 2907 4e54 2901 da04 6461 7461  d.S.).NT)...data
-00000c70: e903 0000 0029 01da 0575 705f 746f 6301  .....)...up_toc.
-00000c80: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000c90: 0000 0013 0000 0073 1600 0000 6900 7c00  .......s....i.|.
-00000ca0: 5d0e 7d01 8800 7c01 1900 7c01 9302 7104  ].}...|...|...q.
-00000cb0: 5300 7215 0000 0072 1500 0000 7244 0000  S.r....r....rD..
-00000cc0: 0072 4600 0000 7215 0000 0072 1600 0000  .rF...r....r....
-00000cd0: 7247 0000 004c 0000 0072 1b00 0000 7a3c  rG...L...r....z<
-00000ce0: 4772 6170 684d 6f64 656c 2e73 656c 6563  GraphModel.selec
-00000cf0: 745f 6e5f 6265 7374 5f66 726f 6d5f 6561  t_n_best_from_ea
-00000d00: 6368 5f63 6c61 7373 2e3c 6c6f 6361 6c73  ch_class.<locals
-00000d10: 3e2e 3c64 6963 7463 6f6d 703e 290b 7202  >.<dictcomp>).r.
-00000d20: 0000 0072 2800 0000 7229 0000 0072 2500  ...r(...r)...r%.
-00000d30: 0000 da05 6564 6765 7372 2d00 0000 720a  ....edgesr-...r.
-00000d40: 0000 00da 1d73 656c 6563 745f 6e5f 6265  .....select_n_be
-00000d50: 7374 5f66 726f 6d5f 6561 6368 5f63 6c61  st_from_each_cla
-00000d60: 7373 720f 0000 0072 1000 0000 7211 0000  ssr....r....r...
-00000d70: 0029 0772 1400 0000 7249 0000 00da 0e66  .).r....rI.....f
-00000d80: 6561 7475 7265 5f67 7261 7068 735a 0b65  eature_graphsZ.e
-00000d90: 6467 655f 746f 5f69 6e64 7223 0000 0072  dge_to_indr#...r
-00000da0: 3e00 0000 724a 0000 0072 1500 0000 7246  >...rJ...r....rF
-00000db0: 0000 0072 1600 0000 724f 0000 0042 0000  ...r....rO...B..
-00000dc0: 0073 1200 0000 0001 0801 1001 1c02 0601  .s..............
-00000dd0: 06ff 0a03 0601 0601 7a28 4772 6170 684d  ........z(GraphM
-00000de0: 6f64 656c 2e73 656c 6563 745f 6e5f 6265  odel.select_n_be
-00000df0: 7374 5f66 726f 6d5f 6561 6368 5f63 6c61  st_from_each_cla
-00000e00: 7373 4e63 0300 0000 0000 0000 0000 0000  ssNc............
-00000e10: 0800 0000 0600 0000 4300 0000 73aa 0000  ........C...s...
-00000e20: 0074 00a0 0174 027c 006a 0383 017c 006a  .t...t.|.j...|.j
-00000e30: 0466 02a1 017d 0374 00a0 0174 027c 006a  .f...}.t...t.|.j
-00000e40: 0383 01a1 017d 0474 057c 006a 0383 0144  .....}.t.|.j...D
-00000e50: 005d 705c 027d 057d 067c 006a 067c 0619  .]p\.}.}.|.j.|..
-00000e60: 0044 005d 347d 077c 006a 0772 6a7c 077c  .D.]4}.|.j.rj|.|
-00000e70: 006a 0776 0072 7664 017c 037c 0519 007c  .j.v.rvd.|.|...|
-00000e80: 006a 077c 0719 003c 0071 4264 017c 037c  .j.|...<.qBd.|.|
-00000e90: 0519 007c 073c 0071 427c 0272 887c 027c  ...|.<.qB|.r.|.|
-00000ea0: 017c 0519 0019 006e 127c 006a 086a 097c  .|.....n.|.j.j.|
-00000eb0: 017c 0519 0064 0264 038d 027c 047c 053c  .|...d.d...|.|.<
-00000ec0: 0071 307c 037c 0466 0253 0029 044e 7227  .q0|.|.f.S.).Nr'
-00000ed0: 0000 0054 7237 0000 0029 0ada 026e 70da  ...Tr7...)...np.
-00000ee0: 057a 6572 6f73 7225 0000 0072 0e00 0000  .zerosr%...r....
-00000ef0: 720f 0000 0072 2900 0000 720d 0000 0072  r....r)...r....r
-00000f00: 1000 0000 720b 0000 0072 3c00 0000 2908  ....r....r<...).
-00000f10: 7214 0000 0072 3f00 0000 720b 0000 00da  r....r?...r.....
-00000f20: 0158 da01 7972 2300 0000 723d 0000 0072  .X..yr#...r=...r
-00000f30: 3200 0000 7215 0000 0072 1500 0000 7216  2...r....r....r.
-00000f40: 0000 00da 0767 6574 5f78 5f79 4e00 0000  .....get_x_yN...
-00000f50: 731a 0000 0000 0116 0110 0112 010e 0106  s...............
-00000f60: 010a 0114 020e 0302 ff0e 0212 fd08 067a  ...............z
-00000f70: 1247 7261 7068 4d6f 6465 6c2e 6765 745f  .GraphModel.get_
-00000f80: 785f 7929 0172 2700 0000 2901 4e29 0cda  x_y).r'...).N)..
-00000f90: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000fa0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000fb0: 655f 5f72 1700 0000 721d 0000 0072 1c00  e__r....r....r..
-00000fc0: 0000 7220 0000 0072 3600 0000 7243 0000  ..r ...r6...rC..
-00000fd0: 0072 4800 0000 724f 0000 0072 5500 0000  .rH...rO...rU...
-00000fe0: 7215 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
-00000ff0: 1600 0000 7208 0000 0009 0000 0073 1200  ....r........s..
-00001000: 0000 0801 080c 0803 0803 0803 0812 0a0b  ................
-00001010: 0806 080c 7208 0000 0029 0dda 056e 756d  ....r....)...num
-00001020: 7079 7251 0000 00da 0b63 6f6c 6c65 6374  pyrQ.....collect
-00001030: 696f 6e73 7202 0000 00da 1974 7577 5f6e  ionsr......tuw_n
-00001040: 6c70 2e63 6f6d 6d6f 6e2e 766f 6361 6275  lp.common.vocabu
-00001050: 6c61 7279 7203 0000 00da 1574 7577 5f6e  laryr......tuw_n
-00001060: 6c70 2e67 7261 7068 2e6c 6578 6963 616c  lp.graph.lexical
-00001070: 7204 0000 00da 1374 7577 5f6e 6c70 2e67  r......tuw_nlp.g
-00001080: 7261 7068 2e75 7469 6c73 7206 0000 005a  raph.utilsr....Z
-00001090: 1478 706f 7461 746f 2e6d 6f64 656c 732e  .xpotato.models.
-000010a0: 7574 696c 7372 0700 0000 7208 0000 0072  utilsr....r....r
-000010b0: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
-000010c0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000010d0: 0073 0c00 0000 0801 0c01 0c01 0c01 0c01  .s..............
-000010e0: 0c03                                     ..
+00000260: 1500 0000 fa4a 2f55 7365 7273 2f61 6461  .....J/Users/ada
+00000270: 6d6b 6f76 6163 732f 7072 6f6a 6563 7473  mkovacs/projects
+00000280: 2f65 7870 2d72 656c 6174 696f 6e2d 6578  /exp-relation-ex
+00000290: 7472 6163 7469 6f6e 2f78 706f 7461 746f  traction/xpotato
+000002a0: 2f6d 6f64 656c 732f 6d6f 6465 6c2e 7079  /models/model.py
+000002b0: da08 5f5f 696e 6974 5f5f 0c00 0000 7314  ..__init__....s.
+000002c0: 0000 0000 0108 0108 0108 0106 0106 0106  ................
+000002d0: 0106 0106 0106 017a 1347 7261 7068 4d6f  .......z.GraphMo
+000002e0: 6465 6c2e 5f5f 696e 6974 5f5f 6301 0000  del.__init__c...
+000002f0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00000300: 0043 0000 0073 1200 0000 6401 6402 8400  .C...s....d.d...
+00000310: 7c00 a000 a100 4400 8301 5300 2903 4e63  |.....D...S.).Nc
+00000320: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000330: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
+00000340: 005d 0c7d 0174 007c 0183 0191 0271 0453  .].}.t.|.....q.S
+00000350: 0072 1500 0000 7205 0000 0029 02da 022e  .r....r....)....
+00000360: 30da 0147 7215 0000 0072 1500 0000 7216  0..Gr....r....r.
+00000370: 0000 00da 0a3c 6c69 7374 636f 6d70 3e19  .....<listcomp>.
+00000380: 0000 00f3 0000 0000 7a38 4772 6170 684d  ........z8GraphM
+00000390: 6f64 656c 2e67 6574 5f66 6561 7475 7265  odel.get_feature
+000003a0: 5f67 7261 7068 5f73 7472 696e 6773 2e3c  _graph_strings.<
+000003b0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+000003c0: 703e 2901 da12 6765 745f 6665 6174 7572  p>)...get_featur
+000003d0: 655f 6772 6170 6873 7213 0000 0072 1500  e_graphsr....r..
+000003e0: 0000 7215 0000 0072 1600 0000 da19 6765  ..r....r......ge
+000003f0: 745f 6665 6174 7572 655f 6772 6170 685f  t_feature_graph_
+00000400: 7374 7269 6e67 7318 0000 0073 0200 0000  strings....s....
+00000410: 0001 7a24 4772 6170 684d 6f64 656c 2e67  ..z$GraphModel.g
+00000420: 6574 5f66 6561 7475 7265 5f67 7261 7068  et_feature_graph
+00000430: 5f73 7472 696e 6773 6301 0000 0000 0000  _stringsc.......
+00000440: 0000 0000 0001 0000 0003 0000 0003 0000  ................
+00000450: 0073 1600 0000 8700 6601 6401 6402 8408  .s......f.d.d...
+00000460: 8800 a000 a100 4400 8301 5300 2903 4e63  ......D...S.).Nc
+00000470: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000480: 0500 0000 1300 0000 7318 0000 0067 007c  ........s....g.|
+00000490: 005d 107d 0188 006a 00a0 017c 01a1 0191  .].}...j...|....
+000004a0: 0271 0453 0072 1500 0000 2902 7209 0000  .q.S.r....).r...
+000004b0: 005a 0a66 726f 6d5f 7475 706c 6529 0272  .Z.from_tuple).r
+000004c0: 1800 0000 da01 5472 1300 0000 7215 0000  ......Tr....r...
+000004d0: 0072 1600 0000 721a 0000 001c 0000 0072  .r....r........r
+000004e0: 1b00 0000 7a31 4772 6170 684d 6f64 656c  ....z1GraphModel
+000004f0: 2e67 6574 5f66 6561 7475 7265 5f67 7261  .get_feature_gra
+00000500: 7068 732e 3c6c 6f63 616c 733e 2e3c 6c69  phs.<locals>.<li
+00000510: 7374 636f 6d70 3e29 01da 1167 6574 5f66  stcomp>)...get_f
+00000520: 6561 7475 7265 5f6e 616d 6573 7213 0000  eature_namesr...
+00000530: 0072 1500 0000 7213 0000 0072 1600 0000  .r....r....r....
+00000540: 721c 0000 001b 0000 0073 0200 0000 0001  r........s......
+00000550: 7a1d 4772 6170 684d 6f64 656c 2e67 6574  z.GraphModel.get
+00000560: 5f66 6561 7475 7265 5f67 7261 7068 7363  _feature_graphsc
+00000570: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000580: 0400 0000 0300 0000 731c 0000 0087 0066  ........s......f
+00000590: 0164 0164 0284 0874 0074 0188 006a 0283  .d.d...t.t...j..
+000005a0: 0183 0144 0083 0153 0029 034e 6301 0000  ...D...S.).Nc...
+000005b0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+000005c0: 0013 0000 0073 1800 0000 6700 7c00 5d10  .....s....g.|.].
+000005d0: 7d01 8800 6a00 a001 7c01 a101 9102 7104  }...j...|.....q.
+000005e0: 5300 7215 0000 0029 0272 0a00 0000 da08  S.r....).r......
+000005f0: 6765 745f 776f 7264 a902 7218 0000 00da  get_word..r.....
+00000600: 0169 7213 0000 0072 1500 0000 7216 0000  .ir....r....r...
+00000610: 0072 1a00 0000 1f00 0000 721b 0000 007a  .r........r....z
+00000620: 3047 7261 7068 4d6f 6465 6c2e 6765 745f  0GraphModel.get_
+00000630: 6665 6174 7572 655f 6e61 6d65 732e 3c6c  feature_names.<l
+00000640: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00000650: 3e29 03da 0572 616e 6765 da03 6c65 6e72  >)...range..lenr
+00000660: 0a00 0000 7213 0000 0072 1500 0000 7213  ....r....r....r.
+00000670: 0000 0072 1600 0000 721f 0000 001e 0000  ...r....r.......
+00000680: 0073 0200 0000 0001 7a1c 4772 6170 684d  .s......z.GraphM
+00000690: 6f64 656c 2e67 6574 5f66 6561 7475 7265  odel.get_feature
+000006a0: 5f6e 616d 6573 6303 0000 0000 0000 0000  _namesc.........
+000006b0: 0000 0008 0000 0008 0000 0043 0000 0073  ...........C...s
+000006c0: 7a00 0000 7400 7401 8301 7d03 7402 7c01  z...t.t...}.t.|.
+000006d0: 6a03 8301 4400 5d62 5c02 7d04 7d05 6401  j...D.]b\.}.}.d.
+000006e0: 6402 8400 7401 7404 7c05 7c02 7c00 6a05  d...t.t.|.|.|.j.
+000006f0: 8303 8301 4400 8301 7d06 7c06 4400 5d38  ....D...}.|.D.]8
+00000700: 7d07 7c03 7401 7c00 6a06 6a07 a008 a100  }.|.t.|.j.j.....
+00000710: 8301 7c04 1900 1900 a009 7c07 6403 1900  ..|.......|.d...
+00000720: 7c07 6404 1900 7c00 6a06 6a0a 7c04 1900  |.d...|.j.j.|...
+00000730: 6603 a101 0100 713a 7112 7c03 5300 2905  f.....q:q.|.S.).
+00000740: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
+00000750: 0000 0400 0000 5300 0000 7318 0000 0067  ......S...s....g
+00000760: 007c 005d 107d 017c 0164 0019 0072 047c  .|.].}.|.d...r.|
+00000770: 0191 0271 0453 0029 01e9 0200 0000 7215  ...q.S.)......r.
+00000780: 0000 0072 2100 0000 7215 0000 0072 1500  ...r!...r....r..
+00000790: 0000 7216 0000 0072 1a00 0000 2500 0000  ..r....r....%...
+000007a0: 7306 0000 0006 0202 0308 fc7a 3747 7261  s..........z7Gra
+000007b0: 7068 4d6f 6465 6c2e 636f 6e76 6572 745f  phModel.convert_
+000007c0: 7472 6565 5f74 6f5f 6665 6174 7572 6573  tree_to_features
+000007d0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+000007e0: 6f6d 703e 7201 0000 00e9 0100 0000 290b  omp>r.........).
+000007f0: 7202 0000 00da 046c 6973 74da 0965 6e75  r......list..enu
+00000800: 6d65 7261 7465 da0b 6573 7469 6d61 746f  merate..estimato
+00000810: 7273 5f72 0700 0000 7211 0000 0072 0b00  rs_r....r....r..
+00000820: 0000 5a0a 776f 7264 5f74 6f5f 6964 da04  ..Z.word_to_id..
+00000830: 6b65 7973 da06 6170 7065 6e64 da0a 6964  keys..append..id
+00000840: 5f74 6f5f 776f 7264 2908 7214 0000 00da  _to_word).r.....
+00000850: 0363 6c66 da15 6665 6174 7572 655f 6772  .clf..feature_gr
+00000860: 6170 685f 7374 7269 6e67 73da 0866 6561  aph_strings..fea
+00000870: 7475 7265 73da 016a da03 6573 74da 0570  tures..j..est..p
+00000880: 6174 6873 da04 7061 7468 7215 0000 0072  aths..pathr....r
+00000890: 1500 0000 7216 0000 00da 1863 6f6e 7665  ....r......conve
+000008a0: 7274 5f74 7265 655f 746f 5f66 6561 7475  rt_tree_to_featu
+000008b0: 7265 7321 0000 0073 1800 0000 0001 0802  res!...s........
+000008c0: 1201 0602 0201 0cff 02fe 0607 0801 1801  ................
+000008d0: 18ff 0804 7a23 4772 6170 684d 6f64 656c  ....z#GraphModel
+000008e0: 2e63 6f6e 7665 7274 5f74 7265 655f 746f  .convert_tree_to
+000008f0: 5f66 6561 7475 7265 7372 2600 0000 6305  _featuresr&...c.
+00000900: 0000 0000 0000 0000 0000 0008 0000 0007  ................
+00000910: 0000 0043 0000 0073 6400 0000 7400 8300  ...C...sd...t...
+00000920: 7d05 7c00 6a01 a002 7c01 a101 0100 7c00  }.|.j...|.....|.
+00000930: 6a03 a004 7c02 7c04 a102 4400 5d1e 5c02  j...|.|...D.].\.
+00000940: 7d06 7d07 7c05 a005 7c00 6a06 6a07 7c06  }.}.|...|.j.j.|.
+00000950: 6401 6402 8d02 a101 0100 7120 7c05 7c00  d.d.......q |.|.
+00000960: 6a08 7c01 3c00 7c03 7c00 6a09 7c01 3c00  j.|.<.|.|.j.|.<.
+00000970: 740a 7c00 6a06 8301 7c00 5f0b 6400 5300  t.|.j...|._.d.S.
+00000980: 2903 4e54 a901 5a09 616c 6c6f 775f 6e65  ).NT..Z.allow_ne
+00000990: 7729 0cda 0373 6574 720e 0000 0072 2b00  w)...setr....r+.
+000009a0: 0000 7209 0000 005a 1167 656e 5f6c 6578  ..r....Z.gen_lex
+000009b0: 5f73 7562 6772 6170 6873 da03 6164 6472  _subgraphs..addr
+000009c0: 0a00 0000 da06 6765 745f 6964 720d 0000  ......get_idr...
+000009d0: 0072 0c00 0000 7224 0000 0072 0f00 0000  .r....r$...r....
+000009e0: 2908 7214 0000 00da 0673 656e 5f69 64da  ).r......sen_id.
+000009f0: 0567 7261 7068 da04 6174 7472 da08 6d61  .graph..attr..ma
+00000a00: 785f 6564 6765 da05 6665 6174 735a 0873  x_edge..featsZ.s
+00000a10: 675f 7475 706c 65da 0273 6772 1500 0000  g_tuple..sgr....
+00000a20: 7215 0000 0072 1600 0000 da13 6665 6174  r....r......feat
+00000a30: 7572 697a 655f 7365 6e5f 6772 6170 6833  urize_sen_graph3
+00000a40: 0000 0073 0e00 0000 0001 0601 0c01 1601  ...s............
+00000a50: 1802 0a02 0a01 7a1e 4772 6170 684d 6f64  ......z.GraphMod
+00000a60: 656c 2e66 6561 7475 7269 7a65 5f73 656e  el.featurize_sen
+00000a70: 5f67 7261 7068 6302 0000 0000 0000 0000  _graphc.........
+00000a80: 0000 0003 0000 0003 0000 0003 0000 0073  ...............s
+00000a90: 3400 0000 7c00 6a00 a001 7c01 a101 5c02  4...|.j...|...\.
+00000aa0: 8900 7d02 7c02 7c00 5f02 8800 7c00 5f03  ..}.|.|._...|._.
+00000ab0: 8700 6601 6401 6402 8408 8800 4400 8301  ..f.d.d.....D...
+00000ac0: 7c00 5f04 6400 5300 2903 4e63 0100 0000  |._.d.S.).Nc....
+00000ad0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000ae0: 1300 0000 7316 0000 0069 007c 005d 0e7d  ....s....i.|.].}
+00000af0: 0188 007c 0119 007c 0193 0271 0453 0072  ...|...|...q.S.r
+00000b00: 1500 0000 7215 0000 00a9 0272 1800 0000  ....r......r....
+00000b10: da01 6ba9 0172 1000 0000 7215 0000 0072  ..k..r....r....r
+00000b20: 1600 0000 da0a 3c64 6963 7463 6f6d 703e  ......<dictcomp>
+00000b30: 4200 0000 721b 0000 007a 2c47 7261 7068  B...r....z,Graph
+00000b40: 4d6f 6465 6c2e 7365 6c65 6374 5f6e 5f62  Model.select_n_b
+00000b50: 6573 742e 3c6c 6f63 616c 733e 2e3c 6469  est.<locals>.<di
+00000b60: 6374 636f 6d70 3e29 0572 0a00 0000 da0d  ctcomp>).r......
+00000b70: 7365 6c65 6374 5f6e 5f62 6573 7472 0f00  select_n_bestr..
+00000b80: 0000 7210 0000 0072 1100 0000 2903 7214  ..r....r....).r.
+00000b90: 0000 00da 0c6d 6178 5f66 6561 7475 7265  .....max_feature
+00000ba0: 73da 0b66 6561 7475 7265 5f6e 756d 7215  s..feature_numr.
+00000bb0: 0000 0072 4200 0000 7216 0000 0072 4400  ...rB...r....rD.
+00000bc0: 0000 3e00 0000 7308 0000 0000 0110 0106  ..>...s.........
+00000bd0: 0106 017a 1847 7261 7068 4d6f 6465 6c2e  ...z.GraphModel.
+00000be0: 7365 6c65 6374 5f6e 5f62 6573 7463 0300  select_n_bestc..
+00000bf0: 0000 0000 0000 0000 0000 0700 0000 0600  ................
+00000c00: 0000 0300 0000 736e 0000 0074 0074 0183  ......sn...t.t..
+00000c10: 017d 0374 027c 0283 0144 005d 225c 027d  .}.t.|...D.]"\.}
+00000c20: 047d 057c 0374 037c 056a 0464 0164 028d  .}.|.t.|.j.d.d..
+00000c30: 0183 0119 00a0 057c 04a1 0101 0071 107c  .......|.....q.|
+00000c40: 006a 066a 077c 017c 0364 0364 048d 035c  .j.j.|.|.d.d...\
+00000c50: 0289 007d 067c 067c 005f 0888 007c 005f  ...}.|.|._...|._
+00000c60: 0987 0066 0164 0564 0684 0888 0044 0083  ...f.d.d.....D..
+00000c70: 017c 005f 0a64 0053 0029 074e 5429 01da  .|._.d.S.).NT)..
+00000c80: 0464 6174 61e9 0300 0000 2901 5a05 7570  .data.....).Z.up
+00000c90: 5f74 6f63 0100 0000 0000 0000 0000 0000  _toc............
+00000ca0: 0200 0000 0400 0000 1300 0000 7316 0000  ............s...
+00000cb0: 0069 007c 005d 0e7d 0188 007c 0119 007c  .i.|.].}...|...|
+00000cc0: 0193 0271 0453 0072 1500 0000 7215 0000  ...q.S.r....r...
+00000cd0: 0072 4000 0000 7242 0000 0072 1500 0000  .r@...rB...r....
+00000ce0: 7216 0000 0072 4300 0000 4e00 0000 721b  r....rC...N...r.
+00000cf0: 0000 007a 3c47 7261 7068 4d6f 6465 6c2e  ...z<GraphModel.
+00000d00: 7365 6c65 6374 5f6e 5f62 6573 745f 6672  select_n_best_fr
+00000d10: 6f6d 5f65 6163 685f 636c 6173 732e 3c6c  om_each_class.<l
+00000d20: 6f63 616c 733e 2e3c 6469 6374 636f 6d70  ocals>.<dictcomp
+00000d30: 3e29 0b72 0200 0000 7227 0000 0072 2800  >).r....r'...r(.
+00000d40: 0000 7224 0000 00da 0565 6467 6573 722b  ..r$.....edgesr+
+00000d50: 0000 0072 0a00 0000 da1d 7365 6c65 6374  ...r......select
+00000d60: 5f6e 5f62 6573 745f 6672 6f6d 5f65 6163  _n_best_from_eac
+00000d70: 685f 636c 6173 7372 0f00 0000 7210 0000  h_classr....r...
+00000d80: 0072 1100 0000 2907 7214 0000 0072 4500  .r....).r....rE.
+00000d90: 0000 da0e 6665 6174 7572 655f 6772 6170  ....feature_grap
+00000da0: 6873 5a0b 6564 6765 5f74 6f5f 696e 6472  hsZ.edge_to_indr
+00000db0: 2200 0000 723a 0000 0072 4600 0000 7215  "...r:...rF...r.
+00000dc0: 0000 0072 4200 0000 7216 0000 0072 4a00  ...rB...r....rJ.
+00000dd0: 0000 4400 0000 7312 0000 0000 0108 0110  ..D...s.........
+00000de0: 011c 0206 0106 ff0a 0306 0106 017a 2847  .............z(G
+00000df0: 7261 7068 4d6f 6465 6c2e 7365 6c65 6374  raphModel.select
+00000e00: 5f6e 5f62 6573 745f 6672 6f6d 5f65 6163  _n_best_from_eac
+00000e10: 685f 636c 6173 734e 6303 0000 0000 0000  h_classNc.......
+00000e20: 0000 0000 0008 0000 0006 0000 0043 0000  .............C..
+00000e30: 0073 aa00 0000 7400 a001 7402 7c00 6a03  .s....t...t.|.j.
+00000e40: 8301 7c00 6a04 6602 a101 7d03 7400 a001  ..|.j.f...}.t...
+00000e50: 7402 7c00 6a03 8301 a101 7d04 7405 7c00  t.|.j.....}.t.|.
+00000e60: 6a03 8301 4400 5d70 5c02 7d05 7d06 7c00  j...D.]p\.}.}.|.
+00000e70: 6a06 7c06 1900 4400 5d34 7d07 7c00 6a07  j.|...D.]4}.|.j.
+00000e80: 726a 7c07 7c00 6a07 7600 7276 6401 7c03  rj|.|.j.v.rvd.|.
+00000e90: 7c05 1900 7c00 6a07 7c07 1900 3c00 7142  |...|.j.|...<.qB
+00000ea0: 6401 7c03 7c05 1900 7c07 3c00 7142 7c02  d.|.|...|.<.qB|.
+00000eb0: 7288 7c02 7c01 7c05 1900 1900 6e12 7c00  r.|.|.|.....n.|.
+00000ec0: 6a08 6a09 7c01 7c05 1900 6402 6403 8d02  j.j.|.|...d.d...
+00000ed0: 7c04 7c05 3c00 7130 7c03 7c04 6602 5300  |.|.<.q0|.|.f.S.
+00000ee0: 2904 4e72 2600 0000 5472 3500 0000 290a  ).Nr&...Tr5...).
+00000ef0: da02 6e70 da05 7a65 726f 7372 2400 0000  ..np..zerosr$...
+00000f00: 720e 0000 0072 0f00 0000 7228 0000 0072  r....r....r(...r
+00000f10: 0d00 0000 7210 0000 0072 0b00 0000 7238  ....r....r....r8
+00000f20: 0000 0029 0872 1400 0000 723b 0000 0072  ...).r....r;...r
+00000f30: 0b00 0000 da01 58da 0179 7222 0000 0072  ......X..yr"...r
+00000f40: 3900 0000 7230 0000 0072 1500 0000 7215  9...r0...r....r.
+00000f50: 0000 0072 1600 0000 da07 6765 745f 785f  ...r......get_x_
+00000f60: 7950 0000 0073 1a00 0000 0001 1601 1001  yP...s..........
+00000f70: 1201 0e01 0601 0a01 1402 0e03 02ff 0e02  ................
+00000f80: 12fd 0806 7a12 4772 6170 684d 6f64 656c  ....z.GraphModel
+00000f90: 2e67 6574 5f78 5f79 2901 7226 0000 0029  .get_x_y).r&...)
+00000fa0: 014e 290c da08 5f5f 6e61 6d65 5f5f da0a  .N)...__name__..
+00000fb0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000fc0: 616c 6e61 6d65 5f5f 7217 0000 0072 1d00  alname__r....r..
+00000fd0: 0000 721c 0000 0072 1f00 0000 7234 0000  ..r....r....r4..
+00000fe0: 0072 3f00 0000 7244 0000 0072 4a00 0000  .r?...rD...rJ...
+00000ff0: 7250 0000 0072 1500 0000 7215 0000 0072  rP...r....r....r
+00001000: 1500 0000 7216 0000 0072 0800 0000 0b00  ....r....r......
+00001010: 0000 7312 0000 0008 0108 0c08 0308 0308  ..s.............
+00001020: 0308 120a 0b08 0608 0c72 0800 0000 290d  .........r....).
+00001030: da0b 636f 6c6c 6563 7469 6f6e 7372 0200  ..collectionsr..
+00001040: 0000 da05 6e75 6d70 7972 4c00 0000 5a19  ....numpyrL...Z.
+00001050: 7475 775f 6e6c 702e 636f 6d6d 6f6e 2e76  tuw_nlp.common.v
+00001060: 6f63 6162 756c 6172 7972 0300 0000 5a15  ocabularyr....Z.
+00001070: 7475 775f 6e6c 702e 6772 6170 682e 6c65  tuw_nlp.graph.le
+00001080: 7869 6361 6c72 0400 0000 da13 7475 775f  xicalr......tuw_
+00001090: 6e6c 702e 6772 6170 682e 7574 696c 7372  nlp.graph.utilsr
+000010a0: 0600 0000 5a14 7870 6f74 6174 6f2e 6d6f  ....Z.xpotato.mo
+000010b0: 6465 6c73 2e75 7469 6c73 7207 0000 0072  dels.utilsr....r
+000010c0: 0800 0000 7215 0000 0072 1500 0000 7215  ....r....r....r.
+000010d0: 0000 0072 1600 0000 da08 3c6d 6f64 756c  ...r......<modul
+000010e0: 653e 0100 0000 730c 0000 000c 0208 010c  e>....s.........
+000010f0: 010c 010c 020c 03                        .......
```

### Comparing `xpotato-0.1.4/xpotato/models/__pycache__/trainer.cpython-39.pyc` & `xpotato-0.1.5/xpotato/models/__pycache__/trainer.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Feb  7 12:34:26 2022 UTC, .py size: 5796 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,363 +1,364 @@
-00000000: 610d 0d0a 0000 0000 d211 0162 a416 0000  a..........b....
+00000000: 610d 0d0a 0000 0000 b86f 9763 9216 0000  a........o.c....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 ca00 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 c200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c02  m.Z.m.Z...d.d.l.
-00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 6d08 5a08 0100 6400 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000070: 0100 6400 6406 6c0b 5a0b 6400 6406 6c0c  ..d.d.l.Z.d.d.l.
-00000080: 5a0d 6400 6407 6c0e 6d0f 5a0f 6d10 5a10  Z.d.d.l.m.Z.m.Z.
-00000090: 0100 6400 6408 6c11 6d12 5a12 0100 6400  ..d.d.l.m.Z...d.
-000000a0: 6409 6c13 6d14 5a14 0100 6400 640a 6c15  d.l.m.Z...d.d.l.
-000000b0: 6d15 5a15 0100 6400 6406 6c16 5a17 6400  m.Z...d.d.l.Z.d.
-000000c0: 640b 6c18 6d19 5a19 0100 6400 640c 6c1a  d.l.m.Z...d.d.l.
-000000d0: 6d1b 5a1b 0100 6400 640d 6c1c 6d1d 5a1d  m.Z...d.d.l.m.Z.
-000000e0: 6d1e 5a1e 0100 4700 640e 640f 8400 640f  m.Z...G.d.d...d.
-000000f0: 8302 5a1f 6406 5300 2910 e900 0000 0029  ..Z.d.S.)......)
-00000100: 01da 0b64 6566 6175 6c74 6469 6374 2902  ...defaultdict).
-00000110: da04 4469 6374 da04 4c69 7374 2901 da05  ..Dict..List)...
-00000120: 556e 696f 6e29 02da 046c 6f67 32da 0473  Union)...log2..s
-00000130: 7172 7429 01da 0942 4d32 354f 6b61 7069  qrt)...BM25Okapi
-00000140: 4e29 02da 0e47 7261 7068 4578 7472 6163  N)...GraphExtrac
-00000150: 746f 72da 1046 6561 7475 7265 4576 616c  tor..FeatureEval
-00000160: 7561 746f 7229 01da 0a47 7261 7068 4d6f  uator)...GraphMo
-00000170: 6465 6c29 01da 124c 6f67 6973 7469 6352  del)...LogisticR
-00000180: 6567 7265 7373 696f 6e29 01da 0474 7164  egression)...tqd
-00000190: 6d29 01da 0673 696d 706c 6529 01da 066d  m)...simple)...m
-000001a0: 6b70 6970 6529 02da 1169 6e76 6572 745f  kpipe)...invert_
-000001b0: 6f62 6a65 6374 6976 6573 da07 7363 616c  objectives..scal
-000001c0: 6572 7363 0000 0000 0000 0000 0000 0000  ersc............
-000001d0: 0000 0000 0a00 0000 4000 0000 73fa 0000  ........@...s...
-000001e0: 0065 005a 0164 005a 0264 1b65 036a 0465  .e.Z.d.Z.d.e.j.e
-000001f0: 0565 0665 0664 0464 059c 0564 0664 0784  .e.e.d.d...d.d..
-00000200: 055a 0764 1c65 0565 036a 0465 0665 0565  .Z.d.e.e.j.e.e.e
-00000210: 0865 0519 0064 0a9c 0564 0b64 0c84 055a  .e...d...d.d...Z
-00000220: 0964 1d65 0665 0a65 0b65 0565 0865 0865  .d.e.e.e.e.e.e.e
-00000230: 0c65 0865 0519 0065 0566 0219 0019 0019  .e.e...e.f......
-00000240: 0066 0219 0064 0f9c 0364 1064 1184 055a  .f...d...d.d...Z
-00000250: 0d64 0464 129c 0164 1364 1484 045a 0e65  .d.d...d.d...Z.e
-00000260: 0b65 0565 0865 0865 0c65 0865 0519 0065  .e.e.e.e.e.e...e
-00000270: 0566 0219 0019 0019 0066 0219 0065 0b65  .f.......f...e.e
-00000280: 0565 0865 0865 0c65 0865 0519 0065 0566  .e.e.e.e.e...e.f
-00000290: 0219 0019 0019 0066 0219 0064 159c 0264  .......f...d...d
-000002a0: 1664 1784 045a 0f64 1e65 0665 0a65 0b65  .d...Z.d.e.e.e.e
-000002b0: 0565 0865 0865 0c65 0865 0519 0065 0566  .e.e.e.e.e...e.f
-000002c0: 0219 0019 0019 0066 0219 0064 0f9c 0364  .......f...d...d
-000002d0: 1964 1a84 055a 1064 0453 0029 1fda 0c47  .d...Z.d.S.)...G
-000002e0: 7261 7068 5472 6169 6e65 72da 0265 6ee9  raphTrainer..en.
-000002f0: 0200 0000 e9d0 0700 004e 2905 da07 6461  .........N)...da
-00000300: 7461 7365 74da 046c 616e 67da 086d 6178  taset..lang..max
-00000310: 5f65 6467 65da 0c6d 6178 5f66 6561 7475  _edge..max_featu
-00000320: 7265 73da 0672 6574 7572 6e63 0500 0000  res..returnc....
-00000330: 0000 0000 0000 0000 0500 0000 0400 0000  ................
-00000340: 4300 0000 7348 0000 0074 0064 0183 0101  C...sH...t.d....
-00000350: 007c 017c 005f 0174 027c 0264 0264 038d  .|.|._.t.|.d.d..
-00000360: 027c 005f 0374 0483 007c 005f 0574 0683  .|._.t...|._.t..
-00000370: 007c 005f 077c 037c 005f 087c 047c 005f  .|._.|.|._.|.|._
-00000380: 0974 0a64 0464 058d 017c 005f 0b64 0053  .t.d.d...|._.d.S
-00000390: 0029 064e 7a1e 496e 6974 6961 6c69 7a69  .).Nz.Initializi
-000003a0: 6e67 2074 7261 696e 6572 206f 626a 6563  ng trainer objec
-000003b0: 742e 2e2e 5a0c 656e 5f6e 6c70 5f63 6163  t...Z.en_nlp_cac
-000003c0: 6865 2902 7217 0000 00da 0863 6163 6865  he).r......cache
-000003d0: 5f66 6e72 0100 0000 2901 da0c 7261 6e64  _fnr....)...rand
-000003e0: 6f6d 5f73 7461 7465 290c da05 7072 696e  om_state)...prin
-000003f0: 7472 1600 0000 7209 0000 00da 0965 7874  tr....r......ext
-00000400: 7261 6374 6f72 720a 0000 00da 0965 7661  ractorr......eva
-00000410: 6c75 6174 6f72 720b 0000 00da 0b67 7261  luatorr......gra
-00000420: 7068 5f6d 6f64 656c 7218 0000 0072 1900  ph_modelr....r..
-00000430: 0000 720c 0000 00da 056d 6f64 656c 2905  ..r......model).
-00000440: da04 7365 6c66 7216 0000 0072 1700 0000  ..selfr....r....
-00000450: 7218 0000 0072 1900 0000 a900 7223 0000  r....r......r#..
-00000460: 00fa 372f 686f 6d65 2f61 6461 616d 6b6f  ..7/home/adaamko
-00000470: 2f70 726f 6a65 6374 732f 504f 5441 544f  /projects/POTATO
-00000480: 2f78 706f 7461 746f 2f6d 6f64 656c 732f  /xpotato/models/
-00000490: 7472 6169 6e65 722e 7079 da08 5f5f 696e  trainer.py..__in
-000004a0: 6974 5f5f 1500 0000 7310 0000 0000 0708  it__....s.......
-000004b0: 0106 010e 0108 0108 0106 0106 017a 1547  .............z.G
-000004c0: 7261 7068 5472 6169 6e65 722e 5f5f 696e  raphTrainer.__in
-000004d0: 6974 5f5f e90a 0000 00da 0462 6d32 3529  it__.......bm25)
-000004e0: 05da 0673 616d 706c 6572 1600 0000 da01  ...sampler......
-000004f0: 6eda 0961 6c67 6f72 6974 686d 721a 0000  n..algorithmr...
-00000500: 0063 0500 0000 0000 0000 0000 0000 0a00  .c..............
-00000510: 0000 0500 0000 4300 0000 735a 0000 007c  ......C...sZ...|
-00000520: 0273 107c 006a 006a 01a0 02a1 006e 027c  .s.|.j.j.....n.|
-00000530: 027d 057c 0464 016b 0272 4e64 0264 0384  .}.|.d.k.rNd.d..
-00000540: 007c 0544 0083 017d 0674 037c 0683 017d  .|.D...}.t.|...}
-00000550: 077c 01a0 04a1 007d 087c 076a 057c 087c  .|.....}.|.j.|.|
-00000560: 057c 0364 048d 037d 097c 0953 007c 0564  .|.d...}.|.S.|.d
-00000570: 0564 0685 0219 0053 0029 074e 7227 0000  .d.....S.).Nr'..
-00000580: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00000590: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
-000005a0: 007c 005d 0c7d 017c 01a0 00a1 0091 0271  .|.].}.|.......q
-000005b0: 0453 0072 2300 0000 2901 da05 7370 6c69  .S.r#...)...spli
-000005c0: 7429 02da 022e 30da 0364 6f63 7223 0000  t)....0..docr#..
-000005d0: 0072 2300 0000 7224 0000 00da 0a3c 6c69  .r#...r$.....<li
-000005e0: 7374 636f 6d70 3e2e 0000 00f3 0000 0000  stcomp>.........
-000005f0: 7a33 4772 6170 6854 7261 696e 6572 2e67  z3GraphTrainer.g
-00000600: 6574 5f6e 5f6d 6f73 745f 7369 6d69 6c61  et_n_most_simila
-00000610: 722e 3c6c 6f63 616c 733e 2e3c 6c69 7374  r.<locals>.<list
-00000620: 636f 6d70 3e29 0172 2900 0000 7201 0000  comp>).r)...r...
-00000630: 0072 2600 0000 2906 7216 0000 00da 0474  .r&...).r......t
-00000640: 6578 74da 0674 6f6c 6973 7472 0800 0000  ext..tolistr....
-00000650: 722b 0000 005a 0967 6574 5f74 6f70 5f6e  r+...Z.get_top_n
-00000660: 290a 7222 0000 0072 2800 0000 7216 0000  ).r"...r(...r...
-00000670: 0072 2900 0000 722a 0000 00da 0663 6f72  .r)...r*.....cor
-00000680: 7075 735a 1074 6f6b 656e 697a 6564 5f63  pusZ.tokenized_c
-00000690: 6f72 7075 7372 2700 0000 da05 7175 6572  orpusr'.....quer
-000006a0: 795a 0574 6f70 5f6e 7223 0000 0072 2300  yZ.top_nr#...r#.
-000006b0: 0000 7224 0000 00da 1267 6574 5f6e 5f6d  ..r$.....get_n_m
-000006c0: 6f73 745f 7369 6d69 6c61 7225 0000 0073  ost_similar%...s
-000006d0: 1000 0000 0007 1401 0801 0e01 0802 0801  ................
-000006e0: 1002 0402 7a1f 4772 6170 6854 7261 696e  ....z.GraphTrain
-000006f0: 6572 2e67 6574 5f6e 5f6d 6f73 745f 7369  er.get_n_most_si
-00000700: 6d69 6c61 7272 0100 0000 4629 03da 086d  milarr....F)...m
-00000710: 696e 5f65 6467 65da 0472 616e 6b72 1a00  in_edge..rankr..
-00000720: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
-00000730: 0000 0004 0000 0043 0000 0073 1600 0000  .......C...s....
-00000740: 7c00 a000 a100 0100 7c00 6a01 7c01 7c02  |.......|.j.|.|.
-00000750: 6401 8d02 5300 2902 4e29 0272 3500 0000  d...S.).N).r5...
-00000760: 7236 0000 0029 02da 0770 7265 7061 7265  r6...)...prepare
-00000770: da05 7472 6169 6e29 0372 2200 0000 7235  ..train).r"...r5
-00000780: 0000 0072 3600 0000 7223 0000 0072 2300  ...r6...r#...r#.
-00000790: 0000 7224 0000 00da 1170 7265 7061 7265  ..r$.....prepare
-000007a0: 5f61 6e64 5f74 7261 696e 3800 0000 7304  _and_train8...s.
-000007b0: 0000 0000 0308 017a 1e47 7261 7068 5472  .......z.GraphTr
-000007c0: 6169 6e65 722e 7072 6570 6172 655f 616e  ainer.prepare_an
-000007d0: 645f 7472 6169 6e29 0172 1a00 0000 6301  d_train).r....c.
-000007e0: 0000 0000 0000 0000 0000 0009 0000 0007  ................
-000007f0: 0000 0043 0000 0073 ea00 0000 7400 a001  ...C...s....t...
-00000800: 7c00 6a02 6a03 a101 a004 a100 7d01 7c00  |.j.j.......}.|.
-00000810: 6a02 6a05 a004 a100 7d02 7c00 6a02 6a06  j.j.....}.|.j.j.
-00000820: a004 a100 7d03 7c00 6a02 6a07 a004 a100  ....}.|.j.j.....
-00000830: 7d04 7408 6401 7c00 6a09 9b00 6402 9d03  }.t.d.|.j...d...
-00000840: 8301 0100 740a 740b 7c01 7c04 7c03 8303  ....t.t.|.|.|...
-00000850: 8301 4400 5d1e 5c03 7d05 7d06 7d07 7c00  ..D.].\.}.}.}.|.
-00000860: 6a0c a00d 7c05 7c06 7c07 7c00 6a09 a104  j...|.|.|.|.j...
-00000870: 0100 7158 7408 6403 8301 0100 7c00 6a0c  ..qXt.d.....|.j.
-00000880: a00e a100 7c00 5f0f 7c00 6a0c a010 a100  ....|._.|.j.....
-00000890: 7c00 5f11 7408 6404 8301 0100 7c00 6a12  |._.t.d.....|.j.
-000008a0: 7413 7c04 8301 6b04 72d8 7414 7415 7413  t.|...k.r.t.t.t.
-000008b0: 7c04 8301 8301 7416 7413 7c04 8301 8301  |.....t.t.|.....
-000008c0: 1400 8301 7d08 7c00 6a0c a017 7c08 a101  ....}.|.j...|...
-000008d0: 0100 6e0e 7c00 6a0c a017 7c00 6a12 a101  ..n.|.j...|.j...
-000008e0: 0100 6400 5300 2905 4e7a 3146 6561 7475  ..d.S.).Nz1Featu
-000008f0: 7269 7a69 6e67 2067 7261 7068 7320 6279  rizing graphs by
-00000900: 2067 656e 6572 6174 696e 6720 7375 6267   generating subg
-00000910: 7261 7068 7320 7570 2074 6f20 7a03 2e2e  raphs up to z...
-00000920: 2e7a 1947 6574 7469 6e67 2066 6561 7475  .z.Getting featu
-00000930: 7265 2067 7261 7068 732e 2e2e 7a1e 5365  re graphs...z.Se
-00000940: 6c65 6374 696e 6720 7468 6520 6265 7374  lecting the best
-00000950: 2066 6561 7475 7265 732e 2e2e 2918 da02   features...)...
-00000960: 7064 da0a 746f 5f6e 756d 6572 6963 7216  pd..to_numericr.
-00000970: 0000 00da 0569 6e64 6578 7231 0000 0072  .....indexr1...r
-00000980: 3000 0000 da08 6c61 6265 6c5f 6964 da05  0.....label_id..
-00000990: 6772 6170 6872 1d00 0000 7218 0000 0072  graphr....r....r
-000009a0: 0d00 0000 da03 7a69 7072 2000 0000 5a13  ......zipr ...Z.
-000009b0: 6665 6174 7572 697a 655f 7365 6e5f 6772  featurize_sen_gr
-000009c0: 6170 685a 1267 6574 5f66 6561 7475 7265  aphZ.get_feature
-000009d0: 5f67 7261 7068 73da 0e66 6561 7475 7265  _graphs..feature
-000009e0: 5f67 7261 7068 735a 1967 6574 5f66 6561  _graphsZ.get_fea
-000009f0: 7475 7265 5f67 7261 7068 5f73 7472 696e  ture_graph_strin
-00000a00: 6773 da15 6665 6174 7572 655f 6772 6170  gs..feature_grap
-00000a10: 685f 7374 7269 6e67 7372 1900 0000 da03  h_stringsr......
-00000a20: 6c65 6eda 0369 6e74 7206 0000 0072 0700  len..intr....r..
-00000a30: 0000 da0d 7365 6c65 6374 5f6e 5f62 6573  ....select_n_bes
-00000a40: 7429 0972 2200 0000 da03 6964 73da 0973  t).r".....ids..s
-00000a50: 656e 7465 6e63 6573 da06 6c61 6265 6c73  entences..labels
-00000a60: da06 6772 6170 6873 da03 696e 6472 3e00  ..graphs..indr>.
-00000a70: 0000 da05 6c61 6265 6cda 066e 5f62 6573  ....label..n_bes
-00000a80: 7472 2300 0000 7223 0000 0072 2400 0000  tr#...r#...r$...
-00000a90: 7237 0000 003e 0000 0073 1e00 0000 0001  r7...>...s......
-00000aa0: 1201 0c01 0c01 0c02 1201 1a01 1602 0801  ................
-00000ab0: 0c01 0c02 0801 0e01 1c01 0e02 7a14 4772  ............z.Gr
-00000ac0: 6170 6854 7261 696e 6572 2e70 7265 7061  aphTrainer.prepa
-00000ad0: 7265 2902 da08 6665 6174 7572 6573 721a  re)...featuresr.
-00000ae0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00000af0: 0c00 0000 0800 0000 4300 0000 73c4 0000  ........C...s...
-00000b00: 0069 007d 027c 01a0 00a1 0044 005d b25c  .i.}.|.....D.].\
-00000b10: 027d 037d 047c 006a 01a0 027c 037c 047c  .}.}.|.j...|.|.|
-00000b20: 006a 03a1 035c 027d 057d 0674 04a0 057c  .j...\.}.}.t...|
-00000b30: 056a 06a0 0764 0164 0284 00a1 017c 056a  .j...d.d.....|.j
-00000b40: 08a0 0764 0364 0284 00a1 0164 049c 02a1  ...d.d.....d....
-00000b50: 017d 0774 096a 0a7c 0774 0b74 0c67 027c  .}.t.j.|.t.t.g.|
-00000b60: 076a 0d64 0564 0667 0264 078d 047d 0874  .j.d.d.g.d...}.t
-00000b70: 0e74 0fa0 10a1 0074 116a 1264 0864 098d  .t.....t.j.d.d..
-00000b80: 0174 13a0 14a1 0083 037d 097c 09a0 157c  .t.......}.|...|
-00000b90: 08a1 017d 0a64 0a64 0b84 0074 1674 177c  ...}.d.d...t.t.|
-00000ba0: 0a6a 187c 0483 0264 0c64 0284 0064 0d8d  .j.|...d.d...d..
-00000bb0: 0244 0083 017d 0b7c 0b7c 027c 033c 0071  .D...}.|.|.|.<.q
-00000bc0: 0c7c 0253 0029 0e4e 6301 0000 0000 0000  .|.S.).Nc.......
-00000bd0: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
-00000be0: 0073 0800 0000 7400 7c00 8301 5300 a901  .s....t.|...S...
-00000bf0: 4ea9 0172 4200 0000 a901 da01 7872 2300  N..rB.......xr#.
-00000c00: 0000 7223 0000 0072 2400 0000 da08 3c6c  ..r#...r$.....<l
-00000c10: 616d 6264 613e 5d00 0000 722f 0000 007a  ambda>]...r/...z
-00000c20: 2347 7261 7068 5472 6169 6e65 722e 7261  #GraphTrainer.ra
-00000c30: 6e6b 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  nk.<locals>.<lam
-00000c40: 6264 613e 6301 0000 0000 0000 0000 0000  bda>c...........
-00000c50: 0001 0000 0002 0000 0053 0000 0073 0800  .........S...s..
-00000c60: 0000 7400 7c00 8301 5300 724d 0000 0072  ..t.|...S.rM...r
-00000c70: 4e00 0000 724f 0000 0072 2300 0000 7223  N...rO...r#...r#
-00000c80: 0000 0072 2400 0000 7251 0000 005e 0000  ...r$...rQ...^..
-00000c90: 0072 2f00 0000 2902 5a0f 6661 6c73 655f  .r/...).Z.false_
-00000ca0: 706f 7369 7469 7665 735a 0e74 7275 655f  positivesZ.true_
-00000cb0: 706f 7369 7469 7665 73e9 1e00 0000 e946  positives......F
-00000cc0: 0000 0029 04da 066d 6174 7269 785a 0a6f  ...)...matrixZ.o
-00000cd0: 626a 6563 7469 7665 735a 0863 7269 7465  bjectivesZ.crite
-00000ce0: 7269 61da 0777 6569 6768 7473 da04 626f  ria..weights..bo
-00000cf0: 7468 2901 da06 7461 7267 6574 6301 0000  th)...targetc...
-00000d00: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00000d10: 0053 0000 0073 1400 0000 6700 7c00 5d0c  .S...s....g.|.].
-00000d20: 5c02 7d01 7d02 7c02 9102 7104 5300 7223  \.}.}.|...q.S.r#
-00000d30: 0000 0072 2300 0000 2903 722c 0000 00da  ...r#...).r,....
-00000d40: 015f 7250 0000 0072 2300 0000 7223 0000  ._rP...r#...r#..
-00000d50: 0072 2400 0000 722e 0000 0071 0000 0073  .r$...r....q...s
-00000d60: 0200 0000 0601 7a25 4772 6170 6854 7261  ......z%GraphTra
-00000d70: 696e 6572 2e72 616e 6b2e 3c6c 6f63 616c  iner.rank.<local
-00000d80: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
-00000d90: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00000da0: 0000 5300 0000 7308 0000 007c 0064 0119  ..S...s....|.d..
-00000db0: 0053 0029 024e 7201 0000 0072 2300 0000  .S.).Nr....r#...
-00000dc0: 2901 da04 7061 6972 7223 0000 0072 2300  )...pairr#...r#.
-00000dd0: 0000 7224 0000 0072 5100 0000 7200 0000  ..r$...rQ...r...
-00000de0: 722f 0000 0029 01da 036b 6579 2919 da05  r/...)...key)...
-00000df0: 6974 656d 7372 1f00 0000 da10 6576 616c  itemsr......eval
-00000e00: 7561 7465 5f66 6561 7475 7265 7216 0000  uate_featurer...
-00000e10: 0072 3a00 0000 da09 4461 7461 4672 616d  .r:.....DataFram
-00000e20: 65da 1346 616c 7365 5f70 6f73 6974 6976  e..False_positiv
-00000e30: 655f 7365 6e73 da05 6170 706c 79da 1254  e_sens..apply..T
-00000e40: 7275 655f 706f 7369 7469 7665 5f73 656e  rue_positive_sen
-00000e50: 73da 0373 6b63 5a04 6d6b 646d da03 6d69  s..skcZ.mkdm..mi
-00000e60: 6eda 036d 6178 da07 636f 6c75 6d6e 7372  n..max..columnsr
-00000e70: 0f00 0000 7210 0000 005a 124d 696e 696d  ....r....Z.Minim
-00000e80: 697a 6554 6f4d 6178 696d 697a 6572 1100  izeToMaximizer..
-00000e90: 0000 5a09 5375 6d53 6361 6c65 7272 0e00  ..Z.SumScalerr..
-00000ea0: 0000 5a10 5765 6967 6874 6564 5375 6d4d  ..Z.WeightedSumM
-00000eb0: 6f64 656c da08 6576 616c 7561 7465 da06  odel..evaluate..
-00000ec0: 736f 7274 6564 723f 0000 00da 0572 616e  sortedr?.....ran
-00000ed0: 6b5f 290c 7222 0000 0072 4c00 0000 5a0f  k_).r"...rL...Z.
-00000ee0: 7261 6e6b 6564 5f66 6561 7475 7265 7372  ranked_featuresr
-00000ef0: 5a00 0000 da03 7661 6cda 0473 7461 74da  Z.....val..stat.
-00000f00: 0361 6363 5a08 7374 6174 5f6f 7074 5a0d  .accZ.stat_optZ.
-00000f10: 6372 6974 6572 6961 5f64 6174 61da 0264  criteria_data..d
-00000f20: 6dda 0364 6563 5a0c 736f 7274 6564 5f66  m..decZ.sorted_f
-00000f30: 6561 7473 7223 0000 0072 2300 0000 7224  eatsr#...r#...r$
-00000f40: 0000 0072 3600 0000 5300 0000 7332 0000  ...r6...S...s2..
-00000f50: 0000 0404 0210 0116 0104 020e 010e fe04  ................
-00000f60: ff04 0704 0102 0106 0104 0106 fc06 0702  ................
-00000f70: 0106 010a 0106 fd04 060a 0206 0116 ff06  ................
-00000f80: 030a 027a 1147 7261 7068 5472 6169 6e65  ...z.GraphTraine
-00000f90: 722e 7261 6e6b e901 0000 0063 0300 0000  r.rank.....c....
-00000fa0: 0000 0000 0000 0000 1100 0000 0900 0000  ................
-00000fb0: 4300 0000 7386 0100 0069 007d 037c 006a  C...s....i.}.|.j
-00000fc0: 006a 01a0 02a1 0044 005d 227d 047c 006a  .j.....D.]"}.|.j
-00000fd0: 007c 006a 006a 017c 046b 0219 006a 0364  .|.j.j.|.k...j.d
-00000fe0: 0119 006a 047c 037c 043c 0071 1064 0264  ...j.|.|.<.q.d.d
-00000ff0: 0384 007c 03a0 05a1 0044 0083 017d 0574  ...|.....D...}.t
-00001000: 0664 0483 0101 007c 006a 076a 087c 006a  .d.....|.j.j.|.j
-00001010: 006a 01a0 09a1 007c 0364 058d 025c 027d  .j.....|.d...\.}
-00001020: 067d 0774 0664 0683 0101 007c 006a 0aa0  .}.t.d.....|.j..
-00001030: 0b7c 067c 07a1 0201 0074 0ca0 0d7c 006a  .|.|.....t...|.j
-00001040: 0aa1 017d 0874 0e74 0f83 017d 0974 0664  ...}.t.t...}.t.d
-00001050: 0783 0101 007c 086a 10a0 02a1 0044 005d  .....|.j.....D.]
-00001060: c27d 0a7c 087c 086a 107c 0a6b 0219 007d  .}.|.|.j.|.k...}
-00001070: 0b67 007d 0c74 117c 0b6a 12a0 09a1 0083  .g.}.t.|.j......
-00001080: 0144 005d 285c 027d 0d7d 0e7c 0e64 086b  .D.](\.}.}.|.d.k
-00001090: 0472 ca7c 0ca0 137c 0b6a 037c 0d19 006a  .r.|...|.j.|...j
-000010a0: 14a0 1564 09a1 01a1 0101 0071 ca7c 0c44  ...d.......q.|.D
-000010b0: 005d 6e7d 0d7c 0d64 0a6b 0372 f87c 006a  .]n}.|.d.k.r.|.j
-000010c0: 167c 006a 076a 1774 187c 0d83 0119 0019  .|.j.j.t.|......
-000010d0: 007d 0f7c 006a 197c 006a 076a 1774 187c  .}.|.j.|.j.j.t.|
-000010e0: 0d83 0119 0019 007d 1074 1a7c 0fa0 1ba1  .......}.t.|....
-000010f0: 0083 017c 016b 0572 f87c 097c 0574 187c  ...|.k.r.|.|.t.|
-00001100: 0a83 0119 0019 00a0 137c 1067 0167 007c  .........|.g.g.|
-00001110: 0574 187c 0a83 0119 0066 03a1 0101 0071  .t.|.....f.....q
-00001120: f871 a67c 0290 0172 8274 0664 0b83 0101  .q.|...r.t.d....
-00001130: 007c 00a0 1c7c 09a1 017d 097c 0953 0029  .|...|...}.|.S.)
-00001140: 0c4e 7201 0000 0063 0100 0000 0000 0000  .Nr....c........
-00001150: 0000 0000 0300 0000 0400 0000 5300 0000  ............S...
-00001160: 7316 0000 0069 007c 005d 0e5c 027d 017d  s....i.|.].\.}.}
-00001170: 027c 027c 0193 0271 0453 0072 2300 0000  .|.|...q.S.r#...
-00001180: 7223 0000 0029 0372 2c00 0000 da01 6bda  r#...).r,.....k.
-00001190: 0176 7223 0000 0072 2300 0000 7224 0000  .vr#...r#...r$..
-000011a0: 00da 0a3c 6469 6374 636f 6d70 3e81 0000  ...<dictcomp>...
-000011b0: 0072 2f00 0000 7a26 4772 6170 6854 7261  .r/...z&GraphTra
-000011c0: 696e 6572 2e74 7261 696e 2e3c 6c6f 6361  iner.train.<loca
-000011d0: 6c73 3e2e 3c64 6963 7463 6f6d 703e 7a1b  ls>.<dictcomp>z.
-000011e0: 4765 6e65 7261 7469 6e67 2074 7261 696e  Generating train
-000011f0: 696e 6720 6461 7461 2e2e 2e29 01da 0b6c  ing data...)...l
-00001200: 6162 656c 5f76 6f63 6162 7a0b 5472 6169  abel_vocabz.Trai
-00001210: 6e69 6e67 2e2e 2e7a 1347 6574 7469 6e67  ning...z.Getting
-00001220: 2066 6561 7475 7265 732e 2e2e 677b 14ae   features...g{..
-00001230: 47e1 7a84 3f72 5000 0000 7a06 3c42 4941  G.z.?rP...z.<BIA
-00001240: 533e 7a25 5261 6e6b 696e 6720 6665 6174  S>z%Ranking feat
-00001250: 7572 6573 2062 6173 6564 206f 6e20 6163  ures based on ac
-00001260: 6375 7261 6379 2e2e 2e29 1d72 1600 0000  curacy...).r....
-00001270: 724a 0000 00da 0675 6e69 7175 65da 0469  rJ.....unique..i
-00001280: 6c6f 6372 3d00 0000 725b 0000 0072 1d00  locr=...r[...r..
-00001290: 0000 7220 0000 005a 0767 6574 5f78 5f79  ..r ...Z.get_x_y
-000012a0: 7231 0000 0072 2100 0000 da03 6669 74da  r1...r!.....fit.
-000012b0: 0465 6c69 355a 1265 7870 6c61 696e 5f77  .eli5Z.explain_w
-000012c0: 6569 6768 7473 5f64 6672 0200 0000 da04  eights_dfr......
-000012d0: 6c69 7374 7257 0000 00da 0965 6e75 6d65  listrW.....enume
-000012e0: 7261 7465 da06 7765 6967 6874 da06 6170  rate..weight..ap
-000012f0: 7065 6e64 da07 6665 6174 7572 65da 0573  pend..feature..s
-00001300: 7472 6970 7240 0000 005a 0f69 6e76 6572  tripr@...Z.inver
-00001310: 7365 5f72 656c 6162 656c 7243 0000 0072  se_relabelrC...r
-00001320: 4100 0000 7242 0000 00da 0565 6467 6573  A...rB.....edges
-00001330: 7236 0000 0029 1172 2200 0000 7235 0000  r6...).r"...r5..
-00001340: 0072 3600 0000 7271 0000 0072 4a00 0000  .r6...rq...rJ...
-00001350: 5a09 696e 765f 766f 6361 625a 0774 7261  Z.inv_vocabZ.tra
-00001360: 696e 5f58 5a07 7472 6169 6e5f 595a 0a77  in_XZ.train_YZ.w
-00001370: 6569 6768 7473 5f64 6672 4c00 0000 7257  eights_dfrL...rW
-00001380: 0000 005a 0b74 6172 6765 7465 645f 6466  ...Z.targeted_df
-00001390: 5a16 6d6f 7374 5f69 6d70 6f72 7461 6e74  Z.most_important
-000013a0: 5f77 6569 6768 7473 da01 69da 0177 5a04  _weights..i..wZ.
-000013b0: 675f 6e78 da01 6772 2300 0000 7223 0000  g_nx..gr#...r#..
-000013c0: 0072 2400 0000 7238 0000 0078 0000 0073  .r$...r8...x...s
-000013d0: 4800 0000 0003 0401 1002 18ff 0804 1202  H...............
-000013e0: 0801 0601 0cff 0a04 0801 0e01 0c01 0802  ................
-000013f0: 0801 0e01 0e01 0402 1601 0801 0401 10ff  ................
-00001400: 0604 0801 0801 1601 0401 0eff 0403 1001  ................
-00001410: 1001 12ff 0804 0601 0801 0a02 7a12 4772  ............z.Gr
-00001420: 6170 6854 7261 696e 6572 2e74 7261 696e  aphTrainer.train
-00001430: 2903 7213 0000 0072 1400 0000 7215 0000  ).r....r....r...
-00001440: 0029 034e 7226 0000 0072 2700 0000 2902  .).Nr&...r'...).
-00001450: 7201 0000 0046 2902 726d 0000 0046 2911  r....F).rm...F).
-00001460: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00001470: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00001480: 6d65 5f5f 723a 0000 0072 5d00 0000 da03  me__r:...r].....
-00001490: 7374 7272 4300 0000 7225 0000 0072 0400  strrC...r%...r..
-000014a0: 0000 7234 0000 00da 0462 6f6f 6c72 0300  ..r4.....boolr..
-000014b0: 0000 7205 0000 0072 3900 0000 7237 0000  ..r....r9...r7..
-000014c0: 0072 3600 0000 7238 0000 0072 2300 0000  .r6...r8...r#...
-000014d0: 7223 0000 0072 2300 0000 7224 0000 0072  r#...r#...r$...r
-000014e0: 1200 0000 1400 0000 7344 0000 0008 0400  ........sD......
-000014f0: 0100 0100 fb02 0204 0102 0102 0102 0102  ................
-00001500: fa0c 1300 0100 0100 fb02 0202 0104 0102  ................
-00001510: 0102 0106 fa0c 1400 ff02 0104 011e fe0c  ................
-00001520: 060e 161e 011e fe0c 2600 ff02 0104 011e  ........&.......
-00001530: fe72 1200 0000 2920 da0b 636f 6c6c 6563  .r....) ..collec
-00001540: 7469 6f6e 7372 0200 0000 da06 7479 7069  tionsr......typi
-00001550: 6e67 7203 0000 0072 0400 0000 7205 0000  ngr....r....r...
-00001560: 00da 046d 6174 6872 0600 0000 7207 0000  ...mathr....r...
-00001570: 005a 0972 616e 6b5f 626d 3235 7208 0000  .Z.rank_bm25r...
-00001580: 0072 7500 0000 da06 7061 6e64 6173 723a  .ru.....pandasr:
-00001590: 0000 00da 1f78 706f 7461 746f 2e67 7261  .....xpotato.gra
-000015a0: 7068 5f65 7874 7261 6374 6f72 2e65 7874  ph_extractor.ext
-000015b0: 7261 6374 7209 0000 0072 0a00 0000 5a14  ractr....r....Z.
-000015c0: 7870 6f74 6174 6f2e 6d6f 6465 6c73 2e6d  xpotato.models.m
-000015d0: 6f64 656c 720b 0000 005a 1473 6b6c 6561  odelr....Z.sklea
-000015e0: 726e 2e6c 696e 6561 725f 6d6f 6465 6c72  rn.linear_modelr
-000015f0: 0c00 0000 720d 0000 005a 0a73 6b63 7269  ....r....Z.skcri
-00001600: 7465 7269 6172 6100 0000 5a0f 736b 6372  teriara...Z.skcr
-00001610: 6974 6572 6961 2e6d 6164 6d72 0e00 0000  iteria.madmr....
-00001620: 5a13 736b 6372 6974 6572 6961 2e70 6970  Z.skcriteria.pip
-00001630: 656c 696e 6572 0f00 0000 5a18 736b 6372  eliner....Z.skcr
-00001640: 6974 6572 6961 2e70 7265 7072 6f63 6573  iteria.preproces
-00001650: 7369 6e67 7210 0000 0072 1100 0000 7212  singr....r....r.
-00001660: 0000 0072 2300 0000 7223 0000 0072 2300  ...r#...r#...r#.
-00001670: 0000 7224 0000 00da 083c 6d6f 6475 6c65  ..r$.....<module
-00001680: 3e01 0000 0073 1e00 0000 0c01 1001 0c01  >....s..........
-00001690: 1001 0c02 0801 0801 1001 0c01 0c01 0c02  ................
-000016a0: 0801 0c01 0c01 1003                      ........
+00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
+00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6400  m.Z.m.Z.m.Z...d.
+00000060: 6404 6c09 5a09 6400 6404 6c0a 5a0b 6400  d.l.Z.d.d.l.Z.d.
+00000070: 6404 6c0c 5a0d 6400 6405 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
+00000080: 0100 6400 6406 6c10 6d11 5a11 0100 6400  ..d.d.l.m.Z...d.
+00000090: 6407 6c12 6d13 5a13 0100 6400 6408 6c14  d.l.m.Z...d.d.l.
+000000a0: 6d15 5a15 6d16 5a16 0100 6400 6409 6c17  m.Z.m.Z...d.d.l.
+000000b0: 6d18 5a18 0100 6400 640a 6c19 6d19 5a19  m.Z...d.d.l.m.Z.
+000000c0: 0100 6400 640b 6c1a 6d1b 5a1b 6d1c 5a1c  ..d.d.l.m.Z.m.Z.
+000000d0: 0100 6400 640c 6c1d 6d1e 5a1e 0100 4700  ..d.d.l.m.Z...G.
+000000e0: 640d 640e 8400 640e 8302 5a1f 6404 5300  d.d...d...Z.d.S.
+000000f0: 290f e900 0000 0029 01da 0b64 6566 6175  )......)...defau
+00000100: 6c74 6469 6374 2902 da04 6c6f 6732 da04  ltdict)...log2..
+00000110: 7371 7274 2903 da04 4469 6374 da04 4c69  sqrt)...Dict..Li
+00000120: 7374 da05 556e 696f 6e4e 2901 da09 424d  st..UnionN)...BM
+00000130: 3235 4f6b 6170 6929 01da 0673 696d 706c  25Okapi)...simpl
+00000140: 6529 01da 066d 6b70 6970 6529 02da 1169  e)...mkpipe)...i
+00000150: 6e76 6572 745f 6f62 6a65 6374 6976 6573  nvert_objectives
+00000160: da07 7363 616c 6572 7329 01da 124c 6f67  ..scalers)...Log
+00000170: 6973 7469 6352 6567 7265 7373 696f 6e29  isticRegression)
+00000180: 01da 0474 7164 6d29 02da 1046 6561 7475  ...tqdm)...Featu
+00000190: 7265 4576 616c 7561 746f 72da 0e47 7261  reEvaluator..Gra
+000001a0: 7068 4578 7472 6163 746f 7229 01da 0a47  phExtractor)...G
+000001b0: 7261 7068 4d6f 6465 6c63 0000 0000 0000  raphModelc......
+000001c0: 0000 0000 0000 0000 0000 0a00 0000 4000  ..............@.
+000001d0: 0000 73fa 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+000001e0: 1b65 036a 0465 0565 0665 0664 0464 059c  .e.j.e.e.e.d.d..
+000001f0: 0564 0664 0784 055a 0764 1c65 0565 036a  .d.d...Z.d.e.e.j
+00000200: 0465 0665 0565 0865 0519 0064 0a9c 0564  .e.e.e.e...d...d
+00000210: 0b64 0c84 055a 0964 1d65 0665 0a65 0b65  .d...Z.d.e.e.e.e
+00000220: 0565 0865 0865 0c65 0865 0519 0065 0566  .e.e.e.e.e...e.f
+00000230: 0219 0019 0019 0066 0219 0064 0f9c 0364  .......f...d...d
+00000240: 1064 1184 055a 0d64 0464 129c 0164 1364  .d...Z.d.d...d.d
+00000250: 1484 045a 0e65 0b65 0565 0865 0865 0c65  ...Z.e.e.e.e.e.e
+00000260: 0865 0519 0065 0566 0219 0019 0019 0066  .e...e.f.......f
+00000270: 0219 0065 0b65 0565 0865 0865 0c65 0865  ...e.e.e.e.e.e.e
+00000280: 0519 0065 0566 0219 0019 0019 0066 0219  ...e.f.......f..
+00000290: 0064 159c 0264 1664 1784 045a 0f64 1e65  .d...d.d...Z.d.e
+000002a0: 0665 0a65 0b65 0565 0865 0865 0c65 0865  .e.e.e.e.e.e.e.e
+000002b0: 0519 0065 0566 0219 0019 0019 0066 0219  ...e.f.......f..
+000002c0: 0064 0f9c 0364 1964 1a84 055a 1064 0453  .d...d.d...Z.d.S
+000002d0: 0029 1fda 0c47 7261 7068 5472 6169 6e65  .)...GraphTraine
+000002e0: 72da 0265 6ee9 0200 0000 e9d0 0700 004e  r..en..........N
+000002f0: 2905 da07 6461 7461 7365 74da 046c 616e  )...dataset..lan
+00000300: 67da 086d 6178 5f65 6467 65da 0c6d 6178  g..max_edge..max
+00000310: 5f66 6561 7475 7265 73da 0672 6574 7572  _features..retur
+00000320: 6e63 0500 0000 0000 0000 0000 0000 0500  nc..............
+00000330: 0000 0400 0000 4300 0000 7348 0000 0074  ......C...sH...t
+00000340: 0064 0183 0101 007c 017c 005f 0174 027c  .d.....|.|._.t.|
+00000350: 0264 0264 038d 027c 005f 0374 0483 007c  .d.d...|._.t...|
+00000360: 005f 0574 0683 007c 005f 077c 037c 005f  ._.t...|._.|.|._
+00000370: 087c 047c 005f 0974 0a64 0464 058d 017c  .|.|._.t.d.d...|
+00000380: 005f 0b64 0053 0029 064e 7a1e 496e 6974  ._.d.S.).Nz.Init
+00000390: 6961 6c69 7a69 6e67 2074 7261 696e 6572  ializing trainer
+000003a0: 206f 626a 6563 742e 2e2e 5a0c 656e 5f6e   object...Z.en_n
+000003b0: 6c70 5f63 6163 6865 2902 7217 0000 00da  lp_cache).r.....
+000003c0: 0863 6163 6865 5f66 6e72 0100 0000 2901  .cache_fnr....).
+000003d0: da0c 7261 6e64 6f6d 5f73 7461 7465 290c  ..random_state).
+000003e0: da05 7072 696e 7472 1600 0000 7210 0000  ..printr....r...
+000003f0: 00da 0965 7874 7261 6374 6f72 720f 0000  ...extractorr...
+00000400: 00da 0965 7661 6c75 6174 6f72 7211 0000  ...evaluatorr...
+00000410: 00da 0b67 7261 7068 5f6d 6f64 656c 7218  ...graph_modelr.
+00000420: 0000 0072 1900 0000 720d 0000 00da 056d  ...r....r......m
+00000430: 6f64 656c 2905 da04 7365 6c66 7216 0000  odel)...selfr...
+00000440: 0072 1700 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000450: a900 7223 0000 00fa 4c2f 5573 6572 732f  ..r#....L/Users/
+00000460: 6164 616d 6b6f 7661 6373 2f70 726f 6a65  adamkovacs/proje
+00000470: 6374 732f 6578 702d 7265 6c61 7469 6f6e  cts/exp-relation
+00000480: 2d65 7874 7261 6374 696f 6e2f 7870 6f74  -extraction/xpot
+00000490: 6174 6f2f 6d6f 6465 6c73 2f74 7261 696e  ato/models/train
+000004a0: 6572 2e70 79da 085f 5f69 6e69 745f 5f14  er.py..__init__.
+000004b0: 0000 0073 1000 0000 0007 0801 0601 0e01  ...s............
+000004c0: 0801 0801 0601 0601 7a15 4772 6170 6854  ........z.GraphT
+000004d0: 7261 696e 6572 2e5f 5f69 6e69 745f 5fe9  rainer.__init__.
+000004e0: 0a00 0000 da04 626d 3235 2905 da06 7361  ......bm25)...sa
+000004f0: 6d70 6c65 7216 0000 00da 016e da09 616c  mpler......n..al
+00000500: 676f 7269 7468 6d72 1a00 0000 6305 0000  gorithmr....c...
+00000510: 0000 0000 0000 0000 000a 0000 0005 0000  ................
+00000520: 0043 0000 0073 5a00 0000 7c02 7310 7c00  .C...sZ...|.s.|.
+00000530: 6a00 6a01 a002 a100 6e02 7c02 7d05 7c04  j.j.....n.|.}.|.
+00000540: 6401 6b02 724e 6402 6403 8400 7c05 4400  d.k.rNd.d...|.D.
+00000550: 8301 7d06 7403 7c06 8301 7d07 7c01 a004  ..}.t.|...}.|...
+00000560: a100 7d08 7c07 6a05 7c08 7c05 7c03 6404  ..}.|.j.|.|.|.d.
+00000570: 8d03 7d09 7c09 5300 7c05 6405 6406 8502  ..}.|.S.|.d.d...
+00000580: 1900 5300 2907 4e72 2700 0000 6301 0000  ..S.).Nr'...c...
+00000590: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+000005a0: 0053 0000 0073 1400 0000 6700 7c00 5d0c  .S...s....g.|.].
+000005b0: 7d01 7c01 a000 a100 9102 7104 5300 7223  }.|.......q.S.r#
+000005c0: 0000 0029 01da 0573 706c 6974 2902 da02  ...)...split)...
+000005d0: 2e30 da03 646f 6372 2300 0000 7223 0000  .0..docr#...r#..
+000005e0: 0072 2400 0000 da0a 3c6c 6973 7463 6f6d  .r$.....<listcom
+000005f0: 703e 2d00 0000 f300 0000 007a 3347 7261  p>-........z3Gra
+00000600: 7068 5472 6169 6e65 722e 6765 745f 6e5f  phTrainer.get_n_
+00000610: 6d6f 7374 5f73 696d 696c 6172 2e3c 6c6f  most_similar.<lo
+00000620: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00000630: 2901 7229 0000 0072 0100 0000 7226 0000  ).r)...r....r&..
+00000640: 0029 0672 1600 0000 da04 7465 7874 da06  .).r......text..
+00000650: 746f 6c69 7374 7208 0000 0072 2b00 0000  tolistr....r+...
+00000660: 5a09 6765 745f 746f 705f 6e29 0a72 2200  Z.get_top_n).r".
+00000670: 0000 7228 0000 0072 1600 0000 7229 0000  ..r(...r....r)..
+00000680: 0072 2a00 0000 da06 636f 7270 7573 5a10  .r*.....corpusZ.
+00000690: 746f 6b65 6e69 7a65 645f 636f 7270 7573  tokenized_corpus
+000006a0: 7227 0000 00da 0571 7565 7279 5a05 746f  r'.....queryZ.to
+000006b0: 705f 6e72 2300 0000 7223 0000 0072 2400  p_nr#...r#...r$.
+000006c0: 0000 da12 6765 745f 6e5f 6d6f 7374 5f73  ....get_n_most_s
+000006d0: 696d 696c 6172 2400 0000 7310 0000 0000  imilar$...s.....
+000006e0: 0714 0108 010e 0108 0208 0110 0204 027a  ...............z
+000006f0: 1f47 7261 7068 5472 6169 6e65 722e 6765  .GraphTrainer.ge
+00000700: 745f 6e5f 6d6f 7374 5f73 696d 696c 6172  t_n_most_similar
+00000710: 7201 0000 0046 2903 da08 6d69 6e5f 6564  r....F)...min_ed
+00000720: 6765 da04 7261 6e6b 721a 0000 0063 0300  ge..rankr....c..
+00000730: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00000740: 0000 4300 0000 7316 0000 007c 00a0 00a1  ..C...s....|....
+00000750: 0001 007c 006a 017c 017c 0264 018d 0253  ...|.j.|.|.d...S
+00000760: 0029 024e 2902 7235 0000 0072 3600 0000  .).N).r5...r6...
+00000770: 2902 da07 7072 6570 6172 65da 0574 7261  )...prepare..tra
+00000780: 696e 2903 7222 0000 0072 3500 0000 7236  in).r"...r5...r6
+00000790: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
+000007a0: 0000 da11 7072 6570 6172 655f 616e 645f  ....prepare_and_
+000007b0: 7472 6169 6e37 0000 0073 0400 0000 0003  train7...s......
+000007c0: 0801 7a1e 4772 6170 6854 7261 696e 6572  ..z.GraphTrainer
+000007d0: 2e70 7265 7061 7265 5f61 6e64 5f74 7261  .prepare_and_tra
+000007e0: 696e 2901 721a 0000 0063 0100 0000 0000  in).r....c......
+000007f0: 0000 0000 0000 0900 0000 0700 0000 4300  ..............C.
+00000800: 0000 73ea 0000 0074 00a0 017c 006a 026a  ..s....t...|.j.j
+00000810: 03a1 01a0 04a1 007d 017c 006a 026a 05a0  .......}.|.j.j..
+00000820: 04a1 007d 027c 006a 026a 06a0 04a1 007d  ...}.|.j.j.....}
+00000830: 037c 006a 026a 07a0 04a1 007d 0474 0864  .|.j.j.....}.t.d
+00000840: 017c 006a 099b 0064 029d 0383 0101 0074  .|.j...d.......t
+00000850: 0a74 0b7c 017c 047c 0383 0383 0144 005d  .t.|.|.|.....D.]
+00000860: 1e5c 037d 057d 067d 077c 006a 0ca0 0d7c  .\.}.}.}.|.j...|
+00000870: 057c 067c 077c 006a 09a1 0401 0071 5874  .|.|.|.j.....qXt
+00000880: 0864 0383 0101 007c 006a 0ca0 0ea1 007c  .d.....|.j.....|
+00000890: 005f 0f7c 006a 0ca0 10a1 007c 005f 1174  ._.|.j.....|._.t
+000008a0: 0864 0483 0101 007c 006a 1274 137c 0483  .d.....|.j.t.|..
+000008b0: 016b 0472 d874 1474 1574 137c 0483 0183  .k.r.t.t.t.|....
+000008c0: 0174 1674 137c 0483 0183 0114 0083 017d  .t.t.|.........}
+000008d0: 087c 006a 0ca0 177c 08a1 0101 006e 0e7c  .|.j...|.....n.|
+000008e0: 006a 0ca0 177c 006a 12a1 0101 0064 0053  .j...|.j.....d.S
+000008f0: 0029 054e 7a31 4665 6174 7572 697a 696e  .).Nz1Featurizin
+00000900: 6720 6772 6170 6873 2062 7920 6765 6e65  g graphs by gene
+00000910: 7261 7469 6e67 2073 7562 6772 6170 6873  rating subgraphs
+00000920: 2075 7020 746f 207a 032e 2e2e 7a19 4765   up to z....z.Ge
+00000930: 7474 696e 6720 6665 6174 7572 6520 6772  tting feature gr
+00000940: 6170 6873 2e2e 2e7a 1e53 656c 6563 7469  aphs...z.Selecti
+00000950: 6e67 2074 6865 2062 6573 7420 6665 6174  ng the best feat
+00000960: 7572 6573 2e2e 2e29 18da 0270 64da 0a74  ures...)...pd..t
+00000970: 6f5f 6e75 6d65 7269 6372 1600 0000 da05  o_numericr......
+00000980: 696e 6465 7872 3100 0000 7230 0000 00da  indexr1...r0....
+00000990: 086c 6162 656c 5f69 64da 0567 7261 7068  .label_id..graph
+000009a0: 721d 0000 0072 1800 0000 720e 0000 00da  r....r....r.....
+000009b0: 037a 6970 7220 0000 005a 1366 6561 7475  .zipr ...Z.featu
+000009c0: 7269 7a65 5f73 656e 5f67 7261 7068 5a12  rize_sen_graphZ.
+000009d0: 6765 745f 6665 6174 7572 655f 6772 6170  get_feature_grap
+000009e0: 6873 da0e 6665 6174 7572 655f 6772 6170  hs..feature_grap
+000009f0: 6873 5a19 6765 745f 6665 6174 7572 655f  hsZ.get_feature_
+00000a00: 6772 6170 685f 7374 7269 6e67 73da 1566  graph_strings..f
+00000a10: 6561 7475 7265 5f67 7261 7068 5f73 7472  eature_graph_str
+00000a20: 696e 6773 7219 0000 00da 036c 656e da03  ingsr......len..
+00000a30: 696e 7472 0300 0000 7204 0000 005a 0d73  intr....r....Z.s
+00000a40: 656c 6563 745f 6e5f 6265 7374 2909 7222  elect_n_best).r"
+00000a50: 0000 00da 0369 6473 da09 7365 6e74 656e  .....ids..senten
+00000a60: 6365 73da 066c 6162 656c 73da 0667 7261  ces..labels..gra
+00000a70: 7068 73da 0369 6e64 723e 0000 00da 056c  phs..indr>.....l
+00000a80: 6162 656c 5a06 6e5f 6265 7374 7223 0000  abelZ.n_bestr#..
+00000a90: 0072 2300 0000 7224 0000 0072 3700 0000  .r#...r$...r7...
+00000aa0: 3d00 0000 731e 0000 0000 0112 010c 010c  =...s...........
+00000ab0: 010c 0212 011a 0116 0208 010c 010c 0208  ................
+00000ac0: 010e 011c 010e 027a 1447 7261 7068 5472  .......z.GraphTr
+00000ad0: 6169 6e65 722e 7072 6570 6172 6529 02da  ainer.prepare)..
+00000ae0: 0866 6561 7475 7265 7372 1a00 0000 6302  .featuresr....c.
+00000af0: 0000 0000 0000 0000 0000 000c 0000 0008  ................
+00000b00: 0000 0043 0000 0073 c400 0000 6900 7d02  ...C...s....i.}.
+00000b10: 7c01 a000 a100 4400 5db2 5c02 7d03 7d04  |.....D.].\.}.}.
+00000b20: 7c00 6a01 a002 7c03 7c04 7c00 6a03 a103  |.j...|.|.|.j...
+00000b30: 5c02 7d05 7d06 7404 a005 7c05 6a06 a007  \.}.}.t...|.j...
+00000b40: 6401 6402 8400 a101 7c05 6a08 a007 6403  d.d.....|.j...d.
+00000b50: 6402 8400 a101 6404 9c02 a101 7d07 7409  d.....d.....}.t.
+00000b60: 6a0a 7c07 740b 740c 6702 7c07 6a0d 6405  j.|.t.t.g.|.j.d.
+00000b70: 6406 6702 6407 8d04 7d08 740e 740f a010  d.g.d...}.t.t...
+00000b80: a100 7411 6a12 6408 6409 8d01 7413 a014  ..t.j.d.d...t...
+00000b90: a100 8303 7d09 7c09 a015 7c08 a101 7d0a  ....}.|...|...}.
+00000ba0: 640a 640b 8400 7416 7417 7c0a 6a18 7c04  d.d...t.t.|.j.|.
+00000bb0: 8302 640c 6402 8400 640d 8d02 4400 8301  ..d.d...d...D...
+00000bc0: 7d0b 7c0b 7c02 7c03 3c00 710c 7c02 5300  }.|.|.|.<.q.|.S.
+00000bd0: 290e 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
+00000be0: 0100 0000 0200 0000 5300 0000 7308 0000  ........S...s...
+00000bf0: 0074 007c 0083 0153 00a9 014e a901 7242  .t.|...S...N..rB
+00000c00: 0000 00a9 01da 0178 7223 0000 0072 2300  .......xr#...r#.
+00000c10: 0000 7224 0000 00da 083c 6c61 6d62 6461  ..r$.....<lambda
+00000c20: 3e5c 0000 0072 2f00 0000 7a23 4772 6170  >\...r/...z#Grap
+00000c30: 6854 7261 696e 6572 2e72 616e 6b2e 3c6c  hTrainer.rank.<l
+00000c40: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e63  ocals>.<lambda>c
+00000c50: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000c60: 0200 0000 5300 0000 7308 0000 0074 007c  ....S...s....t.|
+00000c70: 0083 0153 0072 4b00 0000 724c 0000 0072  ...S.rK...rL...r
+00000c80: 4d00 0000 7223 0000 0072 2300 0000 7224  M...r#...r#...r$
+00000c90: 0000 0072 4f00 0000 5d00 0000 722f 0000  ...rO...]...r/..
+00000ca0: 0029 025a 0f66 616c 7365 5f70 6f73 6974  .).Z.false_posit
+00000cb0: 6976 6573 5a0e 7472 7565 5f70 6f73 6974  ivesZ.true_posit
+00000cc0: 6976 6573 e91e 0000 00e9 4600 0000 2904  ives......F...).
+00000cd0: da06 6d61 7472 6978 5a0a 6f62 6a65 6374  ..matrixZ.object
+00000ce0: 6976 6573 5a08 6372 6974 6572 6961 da07  ivesZ.criteria..
+00000cf0: 7765 6967 6874 73da 0462 6f74 6829 01da  weights..both)..
+00000d00: 0674 6172 6765 7463 0100 0000 0000 0000  .targetc........
+00000d10: 0000 0000 0300 0000 0400 0000 5300 0000  ............S...
+00000d20: 7314 0000 0067 007c 005d 0c5c 027d 017d  s....g.|.].\.}.}
+00000d30: 027c 0291 0271 0453 0072 2300 0000 7223  .|...q.S.r#...r#
+00000d40: 0000 0029 0372 2c00 0000 da01 5f72 4e00  ...).r,....._rN.
+00000d50: 0000 7223 0000 0072 2300 0000 7224 0000  ..r#...r#...r$..
+00000d60: 0072 2e00 0000 7000 0000 7302 0000 0006  .r....p...s.....
+00000d70: 017a 2547 7261 7068 5472 6169 6e65 722e  .z%GraphTrainer.
+00000d80: 7261 6e6b 2e3c 6c6f 6361 6c73 3e2e 3c6c  rank.<locals>.<l
+00000d90: 6973 7463 6f6d 703e 6301 0000 0000 0000  istcomp>c.......
+00000da0: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
+00000db0: 0073 0800 0000 7c00 6401 1900 5300 2902  .s....|.d...S.).
+00000dc0: 4e72 0100 0000 7223 0000 0029 01da 0470  Nr....r#...)...p
+00000dd0: 6169 7272 2300 0000 7223 0000 0072 2400  airr#...r#...r$.
+00000de0: 0000 724f 0000 0071 0000 0072 2f00 0000  ..rO...q...r/...
+00000df0: 2901 da03 6b65 7929 19da 0569 7465 6d73  )...key)...items
+00000e00: 721f 0000 00da 1065 7661 6c75 6174 655f  r......evaluate_
+00000e10: 6665 6174 7572 6572 1600 0000 723a 0000  featurer....r:..
+00000e20: 00da 0944 6174 6146 7261 6d65 da13 4661  ...DataFrame..Fa
+00000e30: 6c73 655f 706f 7369 7469 7665 5f73 656e  lse_positive_sen
+00000e40: 73da 0561 7070 6c79 da12 5472 7565 5f70  s..apply..True_p
+00000e50: 6f73 6974 6976 655f 7365 6e73 da03 736b  ositive_sens..sk
+00000e60: 635a 046d 6b64 6dda 036d 696e da03 6d61  cZ.mkdm..min..ma
+00000e70: 78da 0763 6f6c 756d 6e73 720a 0000 0072  x..columnsr....r
+00000e80: 0b00 0000 5a12 4d69 6e69 6d69 7a65 546f  ....Z.MinimizeTo
+00000e90: 4d61 7869 6d69 7a65 720c 0000 005a 0953  Maximizer....Z.S
+00000ea0: 756d 5363 616c 6572 7209 0000 005a 1057  umScalerr....Z.W
+00000eb0: 6569 6768 7465 6453 756d 4d6f 6465 6cda  eightedSumModel.
+00000ec0: 0865 7661 6c75 6174 65da 0673 6f72 7465  .evaluate..sorte
+00000ed0: 6472 3f00 0000 5a05 7261 6e6b 5f29 0c72  dr?...Z.rank_).r
+00000ee0: 2200 0000 724a 0000 005a 0f72 616e 6b65  "...rJ...Z.ranke
+00000ef0: 645f 6665 6174 7572 6573 7258 0000 00da  d_featuresrX....
+00000f00: 0376 616c da04 7374 6174 da03 6163 635a  .val..stat..accZ
+00000f10: 0873 7461 745f 6f70 745a 0d63 7269 7465  .stat_optZ.crite
+00000f20: 7269 615f 6461 7461 da02 646d da03 6465  ria_data..dm..de
+00000f30: 635a 0c73 6f72 7465 645f 6665 6174 7372  cZ.sorted_featsr
+00000f40: 2300 0000 7223 0000 0072 2400 0000 7236  #...r#...r$...r6
+00000f50: 0000 0052 0000 0073 3200 0000 0004 0402  ...R...s2.......
+00000f60: 1001 1601 0402 0e01 0efe 04ff 0407 0401  ................
+00000f70: 0201 0601 0401 06fc 0607 0201 0601 0a01  ................
+00000f80: 06fd 0406 0a02 0601 16ff 0603 0a02 7a11  ..............z.
+00000f90: 4772 6170 6854 7261 696e 6572 2e72 616e  GraphTrainer.ran
+00000fa0: 6be9 0100 0000 6303 0000 0000 0000 0000  k.....c.........
+00000fb0: 0000 0011 0000 0009 0000 0043 0000 0073  ...........C...s
+00000fc0: 8601 0000 6900 7d03 7c00 6a00 6a01 a002  ....i.}.|.j.j...
+00000fd0: a100 4400 5d22 7d04 7c00 6a00 7c00 6a00  ..D.]"}.|.j.|.j.
+00000fe0: 6a01 7c04 6b02 1900 6a03 6401 1900 6a04  j.|.k...j.d...j.
+00000ff0: 7c03 7c04 3c00 7110 6402 6403 8400 7c03  |.|.<.q.d.d...|.
+00001000: a005 a100 4400 8301 7d05 7406 6404 8301  ....D...}.t.d...
+00001010: 0100 7c00 6a07 6a08 7c00 6a00 6a01 a009  ..|.j.j.|.j.j...
+00001020: a100 7c03 6405 8d02 5c02 7d06 7d07 7406  ..|.d...\.}.}.t.
+00001030: 6406 8301 0100 7c00 6a0a a00b 7c06 7c07  d.....|.j...|.|.
+00001040: a102 0100 740c a00d 7c00 6a0a a101 7d08  ....t...|.j...}.
+00001050: 740e 740f 8301 7d09 7406 6407 8301 0100  t.t...}.t.d.....
+00001060: 7c08 6a10 a002 a100 4400 5dc2 7d0a 7c08  |.j.....D.].}.|.
+00001070: 7c08 6a10 7c0a 6b02 1900 7d0b 6700 7d0c  |.j.|.k...}.g.}.
+00001080: 7411 7c0b 6a12 a009 a100 8301 4400 5d28  t.|.j.......D.](
+00001090: 5c02 7d0d 7d0e 7c0e 6408 6b04 72ca 7c0c  \.}.}.|.d.k.r.|.
+000010a0: a013 7c0b 6a03 7c0d 1900 6a14 a015 6409  ..|.j.|...j...d.
+000010b0: a101 a101 0100 71ca 7c0c 4400 5d6e 7d0d  ......q.|.D.]n}.
+000010c0: 7c0d 640a 6b03 72f8 7c00 6a16 7c00 6a07  |.d.k.r.|.j.|.j.
+000010d0: 6a17 7418 7c0d 8301 1900 1900 7d0f 7c00  j.t.|.......}.|.
+000010e0: 6a19 7c00 6a07 6a17 7418 7c0d 8301 1900  j.|.j.j.t.|.....
+000010f0: 1900 7d10 741a 7c0f a01b a100 8301 7c01  ..}.t.|.......|.
+00001100: 6b05 72f8 7c09 7c05 7418 7c0a 8301 1900  k.r.|.|.t.|.....
+00001110: 1900 a013 7c10 6701 6700 7c05 7418 7c0a  ....|.g.g.|.t.|.
+00001120: 8301 1900 6603 a101 0100 71f8 71a6 7c02  ....f.....q.q.|.
+00001130: 9001 7282 7406 640b 8301 0100 7c00 a01c  ..r.t.d.....|...
+00001140: 7c09 a101 7d09 7c09 5300 290c 4e72 0100  |...}.|.S.).Nr..
+00001150: 0000 6301 0000 0000 0000 0000 0000 0003  ..c.............
+00001160: 0000 0004 0000 0053 0000 0073 1600 0000  .......S...s....
+00001170: 6900 7c00 5d0e 5c02 7d01 7d02 7c02 7c01  i.|.].\.}.}.|.|.
+00001180: 9302 7104 5300 7223 0000 0072 2300 0000  ..q.S.r#...r#...
+00001190: 2903 722c 0000 00da 016b da01 7672 2300  ).r,.....k..vr#.
+000011a0: 0000 7223 0000 0072 2400 0000 da0a 3c64  ..r#...r$.....<d
+000011b0: 6963 7463 6f6d 703e 8000 0000 722f 0000  ictcomp>....r/..
+000011c0: 007a 2647 7261 7068 5472 6169 6e65 722e  .z&GraphTrainer.
+000011d0: 7472 6169 6e2e 3c6c 6f63 616c 733e 2e3c  train.<locals>.<
+000011e0: 6469 6374 636f 6d70 3e7a 1b47 656e 6572  dictcomp>z.Gener
+000011f0: 6174 696e 6720 7472 6169 6e69 6e67 2064  ating training d
+00001200: 6174 612e 2e2e 2901 da0b 6c61 6265 6c5f  ata...)...label_
+00001210: 766f 6361 627a 0b54 7261 696e 696e 672e  vocabz.Training.
+00001220: 2e2e 7a13 4765 7474 696e 6720 6665 6174  ..z.Getting feat
+00001230: 7572 6573 2e2e 2e67 7b14 ae47 e17a 843f  ures...g{..G.z.?
+00001240: 724e 0000 007a 063c 4249 4153 3e7a 2552  rN...z.<BIAS>z%R
+00001250: 616e 6b69 6e67 2066 6561 7475 7265 7320  anking features 
+00001260: 6261 7365 6420 6f6e 2061 6363 7572 6163  based on accurac
+00001270: 792e 2e2e 291d 7216 0000 0072 4900 0000  y...).r....rI...
+00001280: da06 756e 6971 7565 da04 696c 6f63 723d  ..unique..ilocr=
+00001290: 0000 0072 5900 0000 721d 0000 0072 2000  ...rY...r....r .
+000012a0: 0000 5a07 6765 745f 785f 7972 3100 0000  ..Z.get_x_yr1...
+000012b0: 7221 0000 00da 0366 6974 da04 656c 6935  r!.....fit..eli5
+000012c0: 5a12 6578 706c 6169 6e5f 7765 6967 6874  Z.explain_weight
+000012d0: 735f 6466 7202 0000 00da 046c 6973 7472  s_dfr......listr
+000012e0: 5500 0000 da09 656e 756d 6572 6174 65da  U.....enumerate.
+000012f0: 0677 6569 6768 74da 0661 7070 656e 64da  .weight..append.
+00001300: 0766 6561 7475 7265 da05 7374 7269 7072  .feature..stripr
+00001310: 4000 0000 5a0f 696e 7665 7273 655f 7265  @...Z.inverse_re
+00001320: 6c61 6265 6c72 4300 0000 7241 0000 0072  labelrC...rA...r
+00001330: 4200 0000 da05 6564 6765 7372 3600 0000  B.....edgesr6...
+00001340: 2911 7222 0000 0072 3500 0000 7236 0000  ).r"...r5...r6..
+00001350: 0072 6e00 0000 7249 0000 005a 0969 6e76  .rn...rI...Z.inv
+00001360: 5f76 6f63 6162 5a07 7472 6169 6e5f 585a  _vocabZ.train_XZ
+00001370: 0774 7261 696e 5f59 5a0a 7765 6967 6874  .train_YZ.weight
+00001380: 735f 6466 724a 0000 0072 5500 0000 5a0b  s_dfrJ...rU...Z.
+00001390: 7461 7267 6574 6564 5f64 665a 166d 6f73  targeted_dfZ.mos
+000013a0: 745f 696d 706f 7274 616e 745f 7765 6967  t_important_weig
+000013b0: 6874 73da 0169 da01 775a 0467 5f6e 78da  hts..i..wZ.g_nx.
+000013c0: 0167 7223 0000 0072 2300 0000 7224 0000  .gr#...r#...r$..
+000013d0: 0072 3800 0000 7700 0000 7348 0000 0000  .r8...w...sH....
+000013e0: 0304 0110 0218 ff08 0412 0208 0106 010c  ................
+000013f0: ff0a 0408 010e 010c 0108 0208 010e 010e  ................
+00001400: 0104 0216 0108 0104 0110 ff06 0408 0108  ................
+00001410: 0116 0104 010e ff04 0310 0110 0112 ff08  ................
+00001420: 0406 0108 010a 027a 1247 7261 7068 5472  .......z.GraphTr
+00001430: 6169 6e65 722e 7472 6169 6e29 0372 1300  ainer.train).r..
+00001440: 0000 7214 0000 0072 1500 0000 2903 4e72  ..r....r....).Nr
+00001450: 2600 0000 7227 0000 0029 0272 0100 0000  &...r'...).r....
+00001460: 4629 0272 6a00 0000 4629 11da 085f 5f6e  F).rj...F)...__n
+00001470: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00001480: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
+00001490: 3a00 0000 725b 0000 00da 0373 7472 7243  :...r[.....strrC
+000014a0: 0000 0072 2500 0000 7206 0000 0072 3400  ...r%...r....r4.
+000014b0: 0000 da04 626f 6f6c 7205 0000 0072 0700  ....boolr....r..
+000014c0: 0000 7239 0000 0072 3700 0000 7236 0000  ..r9...r7...r6..
+000014d0: 0072 3800 0000 7223 0000 0072 2300 0000  .r8...r#...r#...
+000014e0: 7223 0000 0072 2400 0000 7212 0000 0013  r#...r$...r.....
+000014f0: 0000 0073 4400 0000 0804 0001 0001 00fb  ...sD...........
+00001500: 0202 0401 0201 0201 0201 02fa 0c13 0001  ................
+00001510: 0001 00fb 0202 0201 0401 0201 0201 06fa  ................
+00001520: 0c14 00ff 0201 0401 1efe 0c06 0e16 1e01  ................
+00001530: 1efe 0c26 00ff 0201 0401 1efe 7212 0000  ...&........r...
+00001540: 0029 20da 0b63 6f6c 6c65 6374 696f 6e73  .) ..collections
+00001550: 7202 0000 00da 046d 6174 6872 0300 0000  r......mathr....
+00001560: 7204 0000 00da 0674 7970 696e 6772 0500  r......typingr..
+00001570: 0000 7206 0000 0072 0700 0000 7272 0000  ..r....r....rr..
+00001580: 00da 0670 616e 6461 7372 3a00 0000 5a0a  ...pandasr:...Z.
+00001590: 736b 6372 6974 6572 6961 725f 0000 005a  skcriteriar_...Z
+000015a0: 0972 616e 6b5f 626d 3235 7208 0000 005a  .rank_bm25r....Z
+000015b0: 0f73 6b63 7269 7465 7269 612e 6d61 646d  .skcriteria.madm
+000015c0: 7209 0000 005a 1373 6b63 7269 7465 7269  r....Z.skcriteri
+000015d0: 612e 7069 7065 6c69 6e65 720a 0000 005a  a.pipeliner....Z
+000015e0: 1873 6b63 7269 7465 7269 612e 7072 6570  .skcriteria.prep
+000015f0: 726f 6365 7373 696e 6772 0b00 0000 720c  rocessingr....r.
+00001600: 0000 005a 1473 6b6c 6561 726e 2e6c 696e  ...Z.sklearn.lin
+00001610: 6561 725f 6d6f 6465 6c72 0d00 0000 720e  ear_modelr....r.
+00001620: 0000 00da 1f78 706f 7461 746f 2e67 7261  .....xpotato.gra
+00001630: 7068 5f65 7874 7261 6374 6f72 2e65 7874  ph_extractor.ext
+00001640: 7261 6374 720f 0000 0072 1000 0000 5a14  ractr....r....Z.
+00001650: 7870 6f74 6174 6f2e 6d6f 6465 6c73 2e6d  xpotato.models.m
+00001660: 6f64 656c 7211 0000 0072 1200 0000 7223  odelr....r....r#
+00001670: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
+00001680: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00001690: 731c 0000 000c 0110 0114 0208 0108 0108  s...............
+000016a0: 010c 010c 010c 0110 010c 010c 0210 010c  ................
+000016b0: 03                                       .
```

### Comparing `xpotato-0.1.4/xpotato/models/__pycache__/utils.cpython-39.pyc` & `xpotato-0.1.5/xpotato/models/__pycache__/utils.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  6 08:16:22 2022 UTC, .py size: 7248 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 56d9 7462 501c 0000  a.......V.tbP...
+00000000: 610d 0d0a 0000 0000 6ff7 7d63 501c 0000  a.......o.}cP...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6403 6404 8400  d.l.m.Z...d.d...
 00000050: 5a05 6405 6406 8400 5a06 6507 8300 6407  Z.d.d...Z.e...d.
 00000060: 6602 6408 6409 8401 5a08 6507 8300 6407  f.d.d...Z.e...d.
 00000070: 6602 640a 640b 8401 5a09 6401 5300 290c  f.d.d...Z.d.S.).
@@ -18,257 +18,258 @@
 00000110: 6a01 6b03 7222 8800 8801 7402 7c01 8301  j.k.r"....t.|...
 00000120: 1900 1900 6e02 6400 9102 7104 5300 2901  ....n.d...q.S.).
 00000130: 7a0a 756e 6465 6669 6e65 6421 2903 7202  z.undefined!).r.
 00000140: 0000 00da 0e54 5245 455f 554e 4445 4649  .....TREE_UNDEFI
 00000150: 4e45 44da 0369 6e74 2902 da02 2e30 da01  NED..int)....0..
 00000160: 6929 02da 1566 6561 7475 7265 5f67 7261  i)...feature_gra
 00000170: 7068 5f73 7472 696e 6773 da0f 696e 7665  ph_strings..inve
-00000180: 7273 655f 7265 6c61 6265 6ca9 00fa 352f  rse_relabel...5/
-00000190: 686f 6d65 2f61 6461 616d 6b6f 2f70 726f  home/adaamko/pro
-000001a0: 6a65 6374 732f 504f 5441 544f 2f78 706f  jects/POTATO/xpo
-000001b0: 7461 746f 2f6d 6f64 656c 732f 7574 696c  tato/models/util
-000001c0: 732e 7079 da0a 3c6c 6973 7463 6f6d 703e  s.py..<listcomp>
-000001d0: 0900 0000 7308 0000 0006 0402 fe08 ff12  ....s...........
-000001e0: 027a 2074 7265 655f 746f 5f63 6f64 652e  .z tree_to_code.
-000001f0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00000200: 6d70 3e63 0200 0000 0000 0000 0000 0000  mp>c............
-00000210: 0600 0000 0800 0000 3300 0000 73f8 0000  ........3...s...
-00000220: 0064 017c 0114 007d 0288 026a 007c 0019  .d.|...}...j.|..
-00000230: 0074 016a 026b 0372 c088 007c 0019 007d  .t.j.k.r...|...}
-00000240: 0388 026a 037c 0019 007d 0474 0464 02a0  ...j.|...}.t.d..
-00000250: 057c 027c 037c 04a1 0383 0101 0088 0188  .|.|.|..........
-00000260: 026a 067c 0019 007c 0164 0317 0083 0244  .j.|...|.d.....D
-00000270: 005d 227d 057c 0564 0419 007c 0564 0319  .]"}.|.d...|.d..
-00000280: 007c 0367 0117 007c 0564 0519 0067 0356  .|.g...|.d...g.V
-00000290: 0001 0071 5074 0464 06a0 057c 027c 037c  ...qPt.d...|.|.|
-000002a0: 04a1 0383 0101 0088 0188 026a 077c 0019  ...........j.|..
-000002b0: 007c 0164 0317 0083 0244 005d 227d 057c  .|.d.....D.]"}.|
-000002c0: 0564 0419 007c 0367 0117 007c 0564 0319  .d...|.g...|.d..
-000002d0: 007c 0564 0519 0067 0356 0001 0071 9a6e  .|.d...g.V...q.n
-000002e0: 3467 0067 0074 08a0 0988 026a 0a7c 0019  4g.g.t.....j.|..
-000002f0: 00a1 0167 0356 0001 0074 0464 07a0 057c  ...g.V...t.d...|
-00000300: 0274 08a0 0988 026a 0a7c 0019 00a1 01a1  .t.....j.|......
-00000310: 0283 0101 0064 0053 0029 084e 7a02 2020  .....d.S.).Nz.  
-00000320: 7a0e 7b7d 6966 207b 7d20 3c3d 207b 7d3a  z.{}if {} <= {}:
-00000330: e901 0000 0072 0100 0000 e902 0000 007a  .....r.........z
-00000340: 157b 7d65 6c73 653a 2020 2320 6966 207b  .{}else:  # if {
-00000350: 7d20 3e20 7b7d 7a0b 7b7d 7265 7475 726e  } > {}z.{}return
-00000360: 207b 7d29 0bda 0766 6561 7475 7265 7202   {})...featurer.
-00000370: 0000 0072 0300 0000 da09 7468 7265 7368  ...r......thresh
-00000380: 6f6c 64da 0570 7269 6e74 da06 666f 726d  old..print..form
-00000390: 6174 da0d 6368 696c 6472 656e 5f6c 6566  at..children_lef
-000003a0: 74da 0e63 6869 6c64 7265 6e5f 7269 6768  t..children_righ
-000003b0: 74da 026e 70da 0661 7267 6d61 78da 0576  t..np..argmax..v
-000003c0: 616c 7565 2906 da04 6e6f 6465 da05 6465  alue)...node..de
-000003d0: 7074 68da 0669 6e64 656e 74da 046e 616d  pth..indent..nam
-000003e0: 6572 0f00 0000 da04 7061 7468 2903 da0c  er......path)...
-000003f0: 6665 6174 7572 655f 6e61 6d65 da07 7265  feature_name..re
-00000400: 6375 7273 65da 0574 7265 655f 7209 0000  curse..tree_r...
-00000410: 0072 0a00 0000 721d 0000 0010 0000 0073  .r....r........s
-00000420: 1800 0000 0001 0801 1001 0801 0a01 1201  ................
-00000430: 1801 2001 1201 1801 2202 1801 7a1d 7472  .. ....."...z.tr
-00000440: 6565 5f74 6f5f 636f 6465 2e3c 6c6f 6361  ee_to_code.<loca
-00000450: 6c73 3e2e 7265 6375 7273 6572 0100 0000  ls>.recurser....
-00000460: 720c 0000 0029 0272 1e00 0000 720e 0000  r....).r....r...
-00000470: 0029 03da 0474 7265 6572 0700 0000 7208  .)...treer....r.
-00000480: 0000 0072 0900 0000 2905 7207 0000 0072  ...r....).r....r
-00000490: 1c00 0000 7208 0000 0072 1d00 0000 721e  ....r....r....r.
-000004a0: 0000 0072 0a00 0000 da0c 7472 6565 5f74  ...r......tree_t
-000004b0: 6f5f 636f 6465 0700 0000 730c 0000 0000  o_code....s.....
-000004c0: 0106 010c 0404 fc06 0710 0f72 2000 0000  ...........r ...
-000004d0: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
-000004e0: 0005 0000 0043 0000 0073 7a00 0000 7c00  .....C...sz...|.
-000004f0: 7d01 6401 4400 5d10 7d02 7c01 a000 7c02  }.d.D.].}.|...|.
-00000500: 6402 a102 7d01 7108 7c01 a000 6403 6404  d...}.q.|...d.d.
-00000510: a102 7d01 7c01 a000 6405 6406 a102 7d01  ..}.|...d.d...}.
-00000520: 7c01 a000 6407 6408 a102 7d01 7c01 a000  |...d.d...}.|...
-00000530: 6409 6408 a102 7d01 7c01 640a 6b02 7256  d.d...}.|.d.k.rV
-00000540: 640b 7d01 640c 7d03 7401 a002 640d 7c01  d.}.d.}.t...d.|.
-00000550: a102 736e 7c01 7c03 7600 7276 640e 7c01  ..sn|.|.v.rvd.|.
-00000560: 1700 7d01 7c01 5300 290f 4e7a 175c 3d40  ..}.|.S.).Nz.\=@
-00000570: 2d2c 2722 2e21 3a3b 3c3e 2f7b 7d5b 5d28  -,'".!:;<>/{}[](
-00000580: 2923 5e3f da01 5ffa 0124 da08 5f64 6f6c  )#^?.._..$.._dol
-00000590: 6c61 7273 fa01 25da 085f 7065 7263 656e  lars..%.._percen
-000005a0: 74fa 017c fa01 20da 012a fa01 23da 075f  t..|.. ..*..#.._
-000005b0: 6e75 6d62 6572 2904 da05 6772 6170 6872  number)...graphr
-000005c0: 1700 0000 da06 7374 7269 6374 da04 6564  ......strict..ed
-000005d0: 6765 7a06 5e5b 302d 395d da01 5829 03da  gez.^[0-9]..X)..
-000005e0: 0772 6570 6c61 6365 da02 7265 da05 6d61  .replace..re..ma
-000005f0: 7463 6829 04da 0673 7472 696e 67da 0173  tch)...string..s
-00000600: da01 63da 086b 6579 776f 7264 7372 0900  ..c..keywordsr..
-00000610: 0000 7209 0000 0072 0a00 0000 da07 645f  ..r....r......d_
-00000620: 636c 6561 6e22 0000 0073 1a00 0000 0001  clean"...s......
-00000630: 0401 0801 0e01 0c01 0c01 0c01 0c01 0801  ................
-00000640: 0401 0401 1401 0801 7236 0000 0046 6303  ........r6...Fc.
-00000650: 0000 0000 0000 0000 0000 0014 0000 000a  ................
-00000660: 0000 0043 0000 0073 f801 0000 6401 6402  ...C...s....d.d.
-00000670: 6702 7d03 7400 7c00 8301 4400 9001 5dd0  g.}.t.|...D...].
-00000680: 5c02 7d04 7d05 6403 7401 7402 6404 8301  \.}.}.d.t.t.d...
-00000690: 7c04 1700 6405 1700 8301 1700 6406 1700  |...d.......d...
-000006a0: 7d06 6700 7d07 7c07 a003 7c06 a101 0100  }.g.}.|...|.....
-000006b0: 6900 7d08 7c05 6a04 6407 6408 8d01 4400  i.}.|.j.d.d...D.
-000006c0: 9001 5d18 5c02 7d09 7d0a 7c02 7270 7405  ..].\.}.}.|.rpt.
-000006d0: 7406 7c09 8301 8301 7d0b 6e0c 7405 7c0a  t.|.....}.n.t.|.
-000006e0: 6409 1900 8301 7d0b 7c0b 7d0c 7c0c 7c08  d.....}.|.}.|.|.
-000006f0: 7c09 3c00 640a 7c0a 7600 72b6 7c0a 640a  |.<.d.|.v.r.|.d.
-00000700: 1900 72b6 7c0c 7c01 7600 72b6 640b a007  ..r.|.|.v.r.d...
-00000710: 7c0b 7c0c a102 a008 640c 640d a102 7d0d  |.|.....d.d...}.
-00000720: 6eae 640a 7c0a 7600 72dc 7c0a 640a 1900  n.d.|.v.r.|.d...
-00000730: 72dc 640e a007 7c0b 7c0c a102 a008 640c  r.d...|.|.....d.
-00000740: 640d a102 7d0d 6e88 640f 7c0a 7600 9001  d...}.n.d.|.v...
-00000750: 7206 7c0a 640f 1900 9001 7206 6410 a007  r.|.d.....r.d...
-00000760: 7c0b 7c0c a102 a008 640c 640d a102 7d0d  |.|.....d.d...}.
-00000770: 6e5e 6411 7c0a 7600 9001 7230 7c0a 6411  n^d.|.v...r0|.d.
-00000780: 1900 9001 7230 640e a007 7c0b 7c0c a102  ....r0d...|.|...
-00000790: a008 640c 640d a102 7d0d 6e34 7c0c 7c01  ..d.d...}.n4|.|.
-000007a0: 7600 9001 7250 6412 a007 7c0b 7c0c a102  v...rPd...|.|...
-000007b0: a008 640c 640d a102 7d0d 6e14 6413 a007  ..d.d...}.n.d...
-000007c0: 7c0b 7c0c a102 a008 640c 640d a102 7d0d  |.|.....d.d...}.
-000007d0: 7c07 a003 7c0d a101 0100 7154 7c03 7409  |...|.....qT|.t.
-000007e0: 7c07 8301 3700 7d03 6700 7d0e 7c05 6a0a  |...7.}.g.}.|.j.
-000007f0: 6407 6408 8d01 4400 5d3e 5c03 7d0f 7d10  d.d...D.]>\.}.}.
-00000800: 7d11 6414 7c11 7600 9001 728c 7c08 7c0f  }.d.|.v...r.|.|.
-00000810: 1900 7d12 7c08 7c10 1900 7d13 7c0e a003  ..}.|.|...}.|...
-00000820: 6415 a007 7c12 7c13 7c11 6414 1900 a103  d...|.|.|.d.....
-00000830: a101 0100 9001 718c 7c03 7409 7c0e 8301  ......q.|.t.|...
-00000840: 3700 7d03 7c03 a003 6416 a101 0100 7110  7.}.|...d.....q.
-00000850: 7c03 a003 6416 a101 0100 6417 a00b 7c03  |...d.....d...|.
-00000860: a101 5300 2918 4efa 1e64 6967 7261 7068  ..S.).N..digraph
-00000870: 2066 696e 6974 655f 7374 6174 655f 6d61   finite_state_ma
-00000880: 6368 696e 6520 7bfa 0809 6470 693d 3730  chine {...dpi=70
-00000890: 3b7a 1173 7562 6772 6170 6820 636c 7573  ;z.subgraph clus
-000008a0: 7465 725f fa01 4072 0c00 0000 7a02 207b  ter_..@r....z. {
-000008b0: 54a9 01da 0464 6174 6172 1a00 0000 da08  T....datar......
-000008c0: 6578 7061 6e64 6564 7a5d 097b 307d 205b  expandedz].{0} [
-000008d0: 7368 6170 6520 3d20 6369 7263 6c65 2c20  shape = circle, 
-000008e0: 6c61 6265 6c20 3d20 227b 317d 222c 2020  label = "{1}",  
-000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000900: 2020 2020 2020 2073 7479 6c65 3d66 696c         style=fil
-00000910: 6c65 642c 2066 696c 6c63 6f6c 6f72 3d70  led, fillcolor=p
-00000920: 7572 706c 655d 3bfa 012d 7221 0000 007a  urple];..-r!...z
-00000930: 4d09 7b30 7d20 5b73 6861 7065 203d 2063  M.{0} [shape = c
-00000940: 6972 636c 652c 206c 6162 656c 203d 2022  ircle, label = "
-00000950: 7b31 7d22 2c20 2020 2020 2020 2020 2020  {1}",           
-00000960: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00000970: 796c 653d 2266 696c 6c65 6422 5d3b da08  yle="filled"];..
-00000980: 666f 7572 6c61 6e67 7a5c 097b 307d 205b  fourlangz\.{0} [
-00000990: 7368 6170 6520 3d20 6369 7263 6c65 2c20  shape = circle, 
-000009a0: 6c61 6265 6c20 3d20 227b 317d 222c 2020  label = "{1}",  
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009c0: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-000009d0: 6c6c 6564 222c 2066 696c 6c63 6f6c 6f72  lled", fillcolor
-000009e0: 3d72 6564 5d3b da0b 7375 6273 7469 7475  =red];..substitu
-000009f0: 7465 64fa 4809 7b30 7d20 5b73 6861 7065  ted.H.{0} [shape
-00000a00: 203d 2063 6972 636c 652c 206c 6162 656c   = circle, label
-00000a10: 203d 2022 7b31 7d22 2c20 7374 796c 653d   = "{1}", style=
-00000a20: 6669 6c6c 6564 2c20 6669 6c6c 636f 6c6f  filled, fillcolo
-00000a30: 723d 6c69 6768 7462 6c75 655d 3bfa 2509  r=lightblue];.%.
-00000a40: 7b30 7d20 5b73 6861 7065 203d 2063 6972  {0} [shape = cir
-00000a50: 636c 652c 206c 6162 656c 203d 2022 7b31  cle, label = "{1
-00000a60: 7d22 5d3b da05 636f 6c6f 72fa 1e09 7b30  }"];..color...{0
-00000a70: 7d20 2d3e 207b 317d 205b 206c 6162 656c  } -> {1} [ label
-00000a80: 203d 2022 7b32 7d22 205d 3bda 017d da01   = "{2}" ];..}..
-00000a90: 0a29 0cda 0965 6e75 6d65 7261 7465 da03  .)...enumerate..
-00000aa0: 6368 72da 036f 7264 da06 6170 7065 6e64  chr..ord..append
-00000ab0: da05 6e6f 6465 7372 3600 0000 da03 7374  ..nodesr6.....st
-00000ac0: 7272 1100 0000 722f 0000 00da 0673 6f72  rr....r/.....sor
-00000ad0: 7465 64da 0565 6467 6573 da04 6a6f 696e  ted..edges..join
-00000ae0: 2914 da06 6772 6170 6873 da0c 6d61 726b  )...graphs..mark
-00000af0: 6564 5f6e 6f64 6573 da05 696e 7465 67da  ed_nodes..integ.
-00000b00: 056c 696e 6573 7206 0000 0072 2b00 0000  .linesr....r+...
-00000b10: 7233 0000 00da 0a6e 6f64 655f 6c69 6e65  r3.....node_line
-00000b20: 73da 0c6e 6f64 655f 746f 5f6e 616d 6572  s..node_to_namer
-00000b30: 1700 0000 da06 6e5f 6461 7461 da06 645f  ......n_data..d_
-00000b40: 6e6f 6465 da09 7072 696e 746e 616d 65da  node..printname.
-00000b50: 096e 6f64 655f 6c69 6e65 da0a 6564 6765  .node_line..edge
-00000b60: 5f6c 696e 6573 da01 75da 0176 da05 6564  _lines..u..v..ed
-00000b70: 6174 61da 0764 5f6e 6f64 6531 da07 645f  ata..d_node1..d_
-00000b80: 6e6f 6465 3272 0900 0000 7209 0000 0072  node2r....r....r
-00000b90: 0a00 0000 da07 746f 5f64 6f74 7332 0000  ......to_dots2..
-00000ba0: 0073 8800 0000 0001 0803 1201 1c01 0402  .s..............
-00000bb0: 0a01 0401 1601 0401 0e02 0c01 0401 0802  ................
-00000bc0: 06ff 0202 06fe 0203 06fd 0205 0402 04fe  ................
-00000bd0: 0404 04fc 0606 1001 0402 04fe 0404 04fc  ................
-00000be0: 0606 1401 0402 04fe 0404 04fc 0606 1401  ................
-00000bf0: 0402 04fe 0404 04fc 0606 0a01 0401 04ff  ................
-00000c00: 0403 04fd 0606 0401 04ff 0402 04fe 0403  ................
-00000c10: 0c01 0c02 0401 1601 0a01 0801 0801 0401  ................
-00000c20: 0401 0aff 02ff 0806 0c01 0c01 0a01 725f  ..............r_
-00000c30: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-00000c40: 1100 0000 0900 0000 4300 0000 73d8 0100  ........C...s...
-00000c50: 0064 0164 0267 027d 0367 007d 0469 007d  .d.d.g.}.g.}.i.}
-00000c60: 057c 006a 0064 0364 048d 0144 0090 015d  .|.j.d.d...D...]
-00000c70: 145c 027d 067d 077c 0272 3474 017c 0683  .\.}.}.|.r4t.|..
-00000c80: 017d 086e 0c74 027c 0764 0519 0083 017d  .}.n.t.|.d.....}
-00000c90: 0874 027c 0764 0519 0083 017d 097c 097c  .t.|.d.....}.|.|
-00000ca0: 057c 063c 0064 067c 0776 0072 827c 0764  .|.<.d.|.v.r.|.d
-00000cb0: 0619 0072 827c 097c 0176 0072 8264 07a0  ...r.|.|.v.r.d..
-00000cc0: 037c 087c 09a1 02a0 0464 0864 09a1 027d  .|.|.....d.d...}
-00000cd0: 0a6e a664 067c 0776 0072 a87c 0764 0619  .n.d.|.v.r.|.d..
-00000ce0: 0072 a864 0aa0 037c 087c 09a1 02a0 0464  .r.d...|.|.....d
-00000cf0: 0864 09a1 027d 0a6e 8064 0b7c 0776 0072  .d...}.n.d.|.v.r
-00000d00: ce7c 0764 0b19 0072 ce64 0ca0 037c 087c  .|.d...r.d...|.|
-00000d10: 09a1 02a0 0464 0864 09a1 027d 0a6e 5a64  .....d.d...}.nZd
-00000d20: 0d7c 0776 0072 f47c 0764 0d19 0072 f464  .|.v.r.|.d...r.d
-00000d30: 0aa0 037c 087c 09a1 02a0 0464 0864 09a1  ...|.|.....d.d..
-00000d40: 027d 0a6e 347c 097c 0176 0090 0172 1464  .}.n4|.|.v...r.d
-00000d50: 0ea0 037c 087c 09a1 02a0 0464 0864 09a1  ...|.|.....d.d..
-00000d60: 027d 0a6e 1464 0fa0 037c 087c 09a1 02a0  .}.n.d...|.|....
-00000d70: 0464 0864 09a1 027d 0a7c 04a0 057c 0aa1  .d.d...}.|...|..
-00000d80: 0101 0071 1c7c 0374 067c 0483 0137 007d  ...q.|.t.|...7.}
-00000d90: 0367 007d 0b7c 006a 0764 0364 048d 0144  .g.}.|.j.d.d...D
-00000da0: 005d 665c 037d 0c7d 0d7d 0e64 107c 0e76  .]f\.}.}.}.d.|.v
-00000db0: 0090 0172 507c 057c 0c19 007d 0f7c 057c  ...rP|.|...}.|.|
-00000dc0: 0d19 007d 107c 0290 0172 9c7c 0ba0 0564  ...}.|...r.|...d
-00000dd0: 11a0 0374 017c 0c83 0174 017c 0d83 017c  ...t.|...t.|...|
-00000de0: 0e64 1019 00a1 03a1 0101 006e 187c 0ba0  .d.........n.|..
-00000df0: 0564 11a0 037c 0f7c 107c 0e64 1019 00a1  .d...|.|.|.d....
-00000e00: 03a1 0101 0090 0171 507c 0374 067c 0b83  .......qP|.t.|..
-00000e10: 0137 007d 037c 03a0 0564 12a1 0101 0064  .7.}.|...d.....d
-00000e20: 13a0 087c 03a1 0153 0029 144e 7237 0000  ...|...S.).Nr7..
-00000e30: 0072 3800 0000 5472 3a00 0000 721a 0000  .r8...Tr:...r...
-00000e40: 0072 3c00 0000 7a59 097b 307d 205b 7368  .r<...zY.{0} [sh
-00000e50: 6170 6520 3d20 6369 7263 6c65 2c20 6c61  ape = circle, la
-00000e60: 6265 6c20 3d20 227b 317d 222c 2020 2020  bel = "{1}",    
-00000e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e80: 2073 7479 6c65 3d66 696c 6c65 642c 2066   style=filled, f
-00000e90: 696c 6c63 6f6c 6f72 3d70 7572 706c 655d  illcolor=purple]
-00000ea0: 3b72 3d00 0000 7221 0000 007a 4909 7b30  ;r=...r!...zI.{0
-00000eb0: 7d20 5b73 6861 7065 203d 2063 6972 636c  } [shape = circl
-00000ec0: 652c 206c 6162 656c 203d 2022 7b31 7d22  e, label = "{1}"
-00000ed0: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
-00000ee0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-00000ef0: 6c65 6422 5d3b 723e 0000 007a 5809 7b30  led"];r>...zX.{0
-00000f00: 7d20 5b73 6861 7065 203d 2063 6972 636c  } [shape = circl
-00000f10: 652c 206c 6162 656c 203d 2022 7b31 7d22  e, label = "{1}"
-00000f20: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
-00000f30: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-00000f40: 6c65 6422 2c20 6669 6c6c 636f 6c6f 723d  led", fillcolor=
-00000f50: 7265 645d 3b72 3f00 0000 7240 0000 0072  red];r?...r@...r
-00000f60: 4100 0000 7242 0000 0072 4300 0000 7244  A...rB...rC...rD
-00000f70: 0000 0072 4500 0000 2909 724a 0000 0072  ...rE...).rJ...r
-00000f80: 4b00 0000 7236 0000 0072 1100 0000 722f  K...r6...r....r/
-00000f90: 0000 0072 4900 0000 724c 0000 0072 4d00  ...rI...rL...rM.
-00000fa0: 0000 724e 0000 0029 1172 2b00 0000 7250  ..rN...).r+...rP
-00000fb0: 0000 0072 5100 0000 7252 0000 0072 5300  ...rQ...rR...rS.
-00000fc0: 0000 7254 0000 0072 1700 0000 7255 0000  ..rT...r....rU..
-00000fd0: 0072 5600 0000 7257 0000 0072 5800 0000  .rV...rW...rX...
-00000fe0: 7259 0000 0072 5a00 0000 725b 0000 0072  rY...rZ...r[...r
-00000ff0: 5c00 0000 725d 0000 0072 5e00 0000 7209  \...r]...r^...r.
-00001000: 0000 0072 0900 0000 720a 0000 00da 0674  ...r....r......t
-00001010: 6f5f 646f 7481 0000 0073 8200 0000 0001  o_dot....s......
-00001020: 0803 0401 0401 1601 0401 0a02 0c01 0c01  ................
-00001030: 0801 1801 0402 04fe 0404 04fc 0606 1001  ................
-00001040: 0402 04fe 0404 04fc 0606 1001 0402 04fe  ................
-00001050: 0404 04fc 0606 1001 0402 04fe 0404 04fc  ................
-00001060: 0606 0a01 0401 04ff 0403 04fd 0606 0401  ................
-00001070: 04ff 0402 04fe 0403 0c01 0c02 0401 1601  ................
-00001080: 0a01 0801 0802 0601 0401 0401 12ff 02ff  ................
-00001090: 0607 0401 0401 0aff 02ff 0806 0c01 0a01  ................
-000010a0: 7260 0000 0029 0a72 3000 0000 da05 6e75  r`...).r0.....nu
-000010b0: 6d70 7972 1400 0000 5a0c 736b 6c65 6172  mpyr....Z.sklear
-000010c0: 6e2e 7472 6565 7202 0000 0072 2000 0000  n.treer....r ...
-000010d0: 7236 0000 00da 0373 6574 725f 0000 0072  r6.....setr_...r
-000010e0: 6000 0000 7209 0000 0072 0900 0000 7209  `...r....r....r.
-000010f0: 0000 0072 0a00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00001100: 653e 0100 0000 730c 0000 0008 0208 010c  e>....s.........
-00001110: 0308 1b08 1010 4f                        ......O
+00000180: 7273 655f 7265 6c61 6265 6ca9 00fa 4a2f  rse_relabel...J/
+00000190: 5573 6572 732f 6164 616d 6b6f 7661 6373  Users/adamkovacs
+000001a0: 2f70 726f 6a65 6374 732f 6578 702d 7265  /projects/exp-re
+000001b0: 6c61 7469 6f6e 2d65 7874 7261 6374 696f  lation-extractio
+000001c0: 6e2f 7870 6f74 6174 6f2f 6d6f 6465 6c73  n/xpotato/models
+000001d0: 2f75 7469 6c73 2e70 79da 0a3c 6c69 7374  /utils.py..<list
+000001e0: 636f 6d70 3e09 0000 0073 0800 0000 0604  comp>....s......
+000001f0: 02fe 08ff 1202 7a20 7472 6565 5f74 6f5f  ......z tree_to_
+00000200: 636f 6465 2e3c 6c6f 6361 6c73 3e2e 3c6c  code.<locals>.<l
+00000210: 6973 7463 6f6d 703e 6302 0000 0000 0000  istcomp>c.......
+00000220: 0000 0000 0006 0000 0008 0000 0033 0000  .............3..
+00000230: 0073 f800 0000 6401 7c01 1400 7d02 8802  .s....d.|...}...
+00000240: 6a00 7c00 1900 7401 6a02 6b03 72c0 8800  j.|...t.j.k.r...
+00000250: 7c00 1900 7d03 8802 6a03 7c00 1900 7d04  |...}...j.|...}.
+00000260: 7404 6402 a005 7c02 7c03 7c04 a103 8301  t.d...|.|.|.....
+00000270: 0100 8801 8802 6a06 7c00 1900 7c01 6403  ......j.|...|.d.
+00000280: 1700 8302 4400 5d22 7d05 7c05 6404 1900  ....D.]"}.|.d...
+00000290: 7c05 6403 1900 7c03 6701 1700 7c05 6405  |.d...|.g...|.d.
+000002a0: 1900 6703 5600 0100 7150 7404 6406 a005  ..g.V...qPt.d...
+000002b0: 7c02 7c03 7c04 a103 8301 0100 8801 8802  |.|.|...........
+000002c0: 6a07 7c00 1900 7c01 6403 1700 8302 4400  j.|...|.d.....D.
+000002d0: 5d22 7d05 7c05 6404 1900 7c03 6701 1700  ]"}.|.d...|.g...
+000002e0: 7c05 6403 1900 7c05 6405 1900 6703 5600  |.d...|.d...g.V.
+000002f0: 0100 719a 6e34 6700 6700 7408 a009 8802  ..q.n4g.g.t.....
+00000300: 6a0a 7c00 1900 a101 6703 5600 0100 7404  j.|.....g.V...t.
+00000310: 6407 a005 7c02 7408 a009 8802 6a0a 7c00  d...|.t.....j.|.
+00000320: 1900 a101 a102 8301 0100 6400 5300 2908  ..........d.S.).
+00000330: 4e7a 0220 207a 0e7b 7d69 6620 7b7d 203c  Nz.  z.{}if {} <
+00000340: 3d20 7b7d 3ae9 0100 0000 7201 0000 00e9  = {}:.....r.....
+00000350: 0200 0000 7a15 7b7d 656c 7365 3a20 2023  ....z.{}else:  #
+00000360: 2069 6620 7b7d 203e 207b 7d7a 0b7b 7d72   if {} > {}z.{}r
+00000370: 6574 7572 6e20 7b7d 290b da07 6665 6174  eturn {})...feat
+00000380: 7572 6572 0200 0000 7203 0000 00da 0974  urer....r......t
+00000390: 6872 6573 686f 6c64 da05 7072 696e 74da  hreshold..print.
+000003a0: 0666 6f72 6d61 74da 0d63 6869 6c64 7265  .format..childre
+000003b0: 6e5f 6c65 6674 da0e 6368 696c 6472 656e  n_left..children
+000003c0: 5f72 6967 6874 da02 6e70 da06 6172 676d  _right..np..argm
+000003d0: 6178 da05 7661 6c75 6529 06da 046e 6f64  ax..value)...nod
+000003e0: 65da 0564 6570 7468 da06 696e 6465 6e74  e..depth..indent
+000003f0: da04 6e61 6d65 720f 0000 00da 0470 6174  ..namer......pat
+00000400: 6829 03da 0c66 6561 7475 7265 5f6e 616d  h)...feature_nam
+00000410: 65da 0772 6563 7572 7365 da05 7472 6565  e..recurse..tree
+00000420: 5f72 0900 0000 720a 0000 0072 1d00 0000  _r....r....r....
+00000430: 1000 0000 7318 0000 0000 0108 0110 0108  ....s...........
+00000440: 010a 0112 0118 0120 0112 0118 0122 0218  ....... ....."..
+00000450: 017a 1d74 7265 655f 746f 5f63 6f64 652e  .z.tree_to_code.
+00000460: 3c6c 6f63 616c 733e 2e72 6563 7572 7365  <locals>.recurse
+00000470: 7201 0000 0072 0c00 0000 2902 721e 0000  r....r....).r...
+00000480: 0072 0e00 0000 2903 da04 7472 6565 7207  .r....)...treer.
+00000490: 0000 0072 0800 0000 7209 0000 0029 0572  ...r....r....).r
+000004a0: 0700 0000 721c 0000 0072 0800 0000 721d  ....r....r....r.
+000004b0: 0000 0072 1e00 0000 720a 0000 00da 0c74  ...r....r......t
+000004c0: 7265 655f 746f 5f63 6f64 6507 0000 0073  ree_to_code....s
+000004d0: 0c00 0000 0001 0601 0c04 04fc 0607 100f  ................
+000004e0: 7220 0000 0063 0100 0000 0000 0000 0000  r ...c..........
+000004f0: 0000 0400 0000 0500 0000 4300 0000 737a  ..........C...sz
+00000500: 0000 007c 007d 0164 0144 005d 107d 027c  ...|.}.d.D.].}.|
+00000510: 01a0 007c 0264 02a1 027d 0171 087c 01a0  ...|.d...}.q.|..
+00000520: 0064 0364 04a1 027d 017c 01a0 0064 0564  .d.d...}.|...d.d
+00000530: 06a1 027d 017c 01a0 0064 0764 08a1 027d  ...}.|...d.d...}
+00000540: 017c 01a0 0064 0964 08a1 027d 017c 0164  .|...d.d...}.|.d
+00000550: 0a6b 0272 5664 0b7d 0164 0c7d 0374 01a0  .k.rVd.}.d.}.t..
+00000560: 0264 0d7c 01a1 0273 6e7c 017c 0376 0072  .d.|...sn|.|.v.r
+00000570: 7664 0e7c 0117 007d 017c 0153 0029 0f4e  vd.|...}.|.S.).N
+00000580: 7a17 5c3d 402d 2c27 222e 213a 3b3c 3e2f  z.\=@-,'".!:;<>/
+00000590: 7b7d 5b5d 2829 235e 3fda 015f fa01 24da  {}[]()#^?.._..$.
+000005a0: 085f 646f 6c6c 6172 73fa 0125 da08 5f70  ._dollars..%.._p
+000005b0: 6572 6365 6e74 fa01 7cfa 0120 da01 2afa  ercent..|.. ..*.
+000005c0: 0123 da07 5f6e 756d 6265 7229 04da 0567  .#.._number)...g
+000005d0: 7261 7068 7217 0000 00da 0673 7472 6963  raphr......stric
+000005e0: 74da 0465 6467 657a 065e 5b30 2d39 5dda  t..edgez.^[0-9].
+000005f0: 0158 2903 da07 7265 706c 6163 65da 0272  .X)...replace..r
+00000600: 65da 056d 6174 6368 2904 da06 7374 7269  e..match)...stri
+00000610: 6e67 da01 73da 0163 da08 6b65 7977 6f72  ng..s..c..keywor
+00000620: 6473 7209 0000 0072 0900 0000 720a 0000  dsr....r....r...
+00000630: 00da 0764 5f63 6c65 616e 2200 0000 731a  ...d_clean"...s.
+00000640: 0000 0000 0104 0108 010e 010c 010c 010c  ................
+00000650: 010c 0108 0104 0104 0114 0108 0172 3600  .............r6.
+00000660: 0000 4663 0300 0000 0000 0000 0000 0000  ..Fc............
+00000670: 1400 0000 0a00 0000 4300 0000 73f8 0100  ........C...s...
+00000680: 0064 0164 0267 027d 0374 007c 0083 0144  .d.d.g.}.t.|...D
+00000690: 0090 015d d05c 027d 047d 0564 0374 0174  ...].\.}.}.d.t.t
+000006a0: 0264 0483 017c 0417 0064 0517 0083 0117  .d...|...d......
+000006b0: 0064 0617 007d 0667 007d 077c 07a0 037c  .d...}.g.}.|...|
+000006c0: 06a1 0101 0069 007d 087c 056a 0464 0764  .....i.}.|.j.d.d
+000006d0: 088d 0144 0090 015d 185c 027d 097d 0a7c  ...D...].\.}.}.|
+000006e0: 0272 7074 0574 067c 0983 0183 017d 0b6e  .rpt.t.|.....}.n
+000006f0: 0c74 057c 0a64 0919 0083 017d 0b7c 0b7d  .t.|.d.....}.|.}
+00000700: 0c7c 0c7c 087c 093c 0064 0a7c 0a76 0072  .|.|.|.<.d.|.v.r
+00000710: b67c 0a64 0a19 0072 b67c 0c7c 0176 0072  .|.d...r.|.|.v.r
+00000720: b664 0ba0 077c 0b7c 0ca1 02a0 0864 0c64  .d...|.|.....d.d
+00000730: 0da1 027d 0d6e ae64 0a7c 0a76 0072 dc7c  ...}.n.d.|.v.r.|
+00000740: 0a64 0a19 0072 dc64 0ea0 077c 0b7c 0ca1  .d...r.d...|.|..
+00000750: 02a0 0864 0c64 0da1 027d 0d6e 8864 0f7c  ...d.d...}.n.d.|
+00000760: 0a76 0090 0172 067c 0a64 0f19 0090 0172  .v...r.|.d.....r
+00000770: 0664 10a0 077c 0b7c 0ca1 02a0 0864 0c64  .d...|.|.....d.d
+00000780: 0da1 027d 0d6e 5e64 117c 0a76 0090 0172  ...}.n^d.|.v...r
+00000790: 307c 0a64 1119 0090 0172 3064 0ea0 077c  0|.d.....r0d...|
+000007a0: 0b7c 0ca1 02a0 0864 0c64 0da1 027d 0d6e  .|.....d.d...}.n
+000007b0: 347c 0c7c 0176 0090 0172 5064 12a0 077c  4|.|.v...rPd...|
+000007c0: 0b7c 0ca1 02a0 0864 0c64 0da1 027d 0d6e  .|.....d.d...}.n
+000007d0: 1464 13a0 077c 0b7c 0ca1 02a0 0864 0c64  .d...|.|.....d.d
+000007e0: 0da1 027d 0d7c 07a0 037c 0da1 0101 0071  ...}.|...|.....q
+000007f0: 547c 0374 097c 0783 0137 007d 0367 007d  T|.t.|...7.}.g.}
+00000800: 0e7c 056a 0a64 0764 088d 0144 005d 3e5c  .|.j.d.d...D.]>\
+00000810: 037d 0f7d 107d 1164 147c 1176 0090 0172  .}.}.}.d.|.v...r
+00000820: 8c7c 087c 0f19 007d 127c 087c 1019 007d  .|.|...}.|.|...}
+00000830: 137c 0ea0 0364 15a0 077c 127c 137c 1164  .|...d...|.|.|.d
+00000840: 1419 00a1 03a1 0101 0090 0171 8c7c 0374  ...........q.|.t
+00000850: 097c 0e83 0137 007d 037c 03a0 0364 16a1  .|...7.}.|...d..
+00000860: 0101 0071 107c 03a0 0364 16a1 0101 0064  ...q.|...d.....d
+00000870: 17a0 0b7c 03a1 0153 0029 184e fa1e 6469  ...|...S.).N..di
+00000880: 6772 6170 6820 6669 6e69 7465 5f73 7461  graph finite_sta
+00000890: 7465 5f6d 6163 6869 6e65 207b fa08 0964  te_machine {...d
+000008a0: 7069 3d37 303b 7a11 7375 6267 7261 7068  pi=70;z.subgraph
+000008b0: 2063 6c75 7374 6572 5ffa 0140 720c 0000   cluster_..@r...
+000008c0: 007a 0220 7b54 a901 da04 6461 7461 721a  .z. {T....datar.
+000008d0: 0000 00da 0865 7870 616e 6465 647a 5d09  .....expandedz].
+000008e0: 7b30 7d20 5b73 6861 7065 203d 2063 6972  {0} [shape = cir
+000008f0: 636c 652c 206c 6162 656c 203d 2022 7b31  cle, label = "{1
+00000900: 7d22 2c20 2020 2020 2020 2020 2020 2020  }",             
+00000910: 2020 2020 2020 2020 2020 2020 7374 796c              styl
+00000920: 653d 6669 6c6c 6564 2c20 6669 6c6c 636f  e=filled, fillco
+00000930: 6c6f 723d 7075 7270 6c65 5d3b fa01 2d72  lor=purple];..-r
+00000940: 2100 0000 7a4d 097b 307d 205b 7368 6170  !...zM.{0} [shap
+00000950: 6520 3d20 6369 7263 6c65 2c20 6c61 6265  e = circle, labe
+00000960: 6c20 3d20 227b 317d 222c 2020 2020 2020  l = "{1}",      
+00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000980: 2020 2073 7479 6c65 3d22 6669 6c6c 6564     style="filled
+00000990: 225d 3bda 0866 6f75 726c 616e 677a 5c09  "];..fourlangz\.
+000009a0: 7b30 7d20 5b73 6861 7065 203d 2063 6972  {0} [shape = cir
+000009b0: 636c 652c 206c 6162 656c 203d 2022 7b31  cle, label = "{1
+000009c0: 7d22 2c20 2020 2020 2020 2020 2020 2020  }",             
+000009d0: 2020 2020 2020 2020 2020 2020 7374 796c              styl
+000009e0: 653d 2266 696c 6c65 6422 2c20 6669 6c6c  e="filled", fill
+000009f0: 636f 6c6f 723d 7265 645d 3bda 0b73 7562  color=red];..sub
+00000a00: 7374 6974 7574 6564 fa48 097b 307d 205b  stituted.H.{0} [
+00000a10: 7368 6170 6520 3d20 6369 7263 6c65 2c20  shape = circle, 
+00000a20: 6c61 6265 6c20 3d20 227b 317d 222c 2073  label = "{1}", s
+00000a30: 7479 6c65 3d66 696c 6c65 642c 2066 696c  tyle=filled, fil
+00000a40: 6c63 6f6c 6f72 3d6c 6967 6874 626c 7565  lcolor=lightblue
+00000a50: 5d3b fa25 097b 307d 205b 7368 6170 6520  ];.%.{0} [shape 
+00000a60: 3d20 6369 7263 6c65 2c20 6c61 6265 6c20  = circle, label 
+00000a70: 3d20 227b 317d 225d 3bda 0563 6f6c 6f72  = "{1}"];..color
+00000a80: fa1e 097b 307d 202d 3e20 7b31 7d20 5b20  ...{0} -> {1} [ 
+00000a90: 6c61 6265 6c20 3d20 227b 327d 2220 5d3b  label = "{2}" ];
+00000aa0: da01 7dda 010a 290c da09 656e 756d 6572  ..}...)...enumer
+00000ab0: 6174 65da 0363 6872 da03 6f72 64da 0661  ate..chr..ord..a
+00000ac0: 7070 656e 64da 056e 6f64 6573 7236 0000  ppend..nodesr6..
+00000ad0: 00da 0373 7472 7211 0000 0072 2f00 0000  ...strr....r/...
+00000ae0: da06 736f 7274 6564 da05 6564 6765 73da  ..sorted..edges.
+00000af0: 046a 6f69 6e29 14da 0667 7261 7068 73da  .join)...graphs.
+00000b00: 0c6d 6172 6b65 645f 6e6f 6465 73da 0569  .marked_nodes..i
+00000b10: 6e74 6567 da05 6c69 6e65 7372 0600 0000  nteg..linesr....
+00000b20: 722b 0000 0072 3300 0000 da0a 6e6f 6465  r+...r3.....node
+00000b30: 5f6c 696e 6573 da0c 6e6f 6465 5f74 6f5f  _lines..node_to_
+00000b40: 6e61 6d65 7217 0000 00da 066e 5f64 6174  namer......n_dat
+00000b50: 61da 0664 5f6e 6f64 65da 0970 7269 6e74  a..d_node..print
+00000b60: 6e61 6d65 da09 6e6f 6465 5f6c 696e 65da  name..node_line.
+00000b70: 0a65 6467 655f 6c69 6e65 73da 0175 da01  .edge_lines..u..
+00000b80: 76da 0565 6461 7461 da07 645f 6e6f 6465  v..edata..d_node
+00000b90: 31da 0764 5f6e 6f64 6532 7209 0000 0072  1..d_node2r....r
+00000ba0: 0900 0000 720a 0000 00da 0774 6f5f 646f  ....r......to_do
+00000bb0: 7473 3200 0000 7388 0000 0000 0108 0312  ts2...s.........
+00000bc0: 011c 0104 020a 0104 0116 0104 010e 020c  ................
+00000bd0: 0104 0108 0206 ff02 0206 fe02 0306 fd02  ................
+00000be0: 0504 0204 fe04 0404 fc06 0610 0104 0204  ................
+00000bf0: fe04 0404 fc06 0614 0104 0204 fe04 0404  ................
+00000c00: fc06 0614 0104 0204 fe04 0404 fc06 060a  ................
+00000c10: 0104 0104 ff04 0304 fd06 0604 0104 ff04  ................
+00000c20: 0204 fe04 030c 010c 0204 0116 010a 0108  ................
+00000c30: 0108 0104 0104 010a ff02 ff08 060c 010c  ................
+00000c40: 010a 0172 5f00 0000 6303 0000 0000 0000  ...r_...c.......
+00000c50: 0000 0000 0011 0000 0009 0000 0043 0000  .............C..
+00000c60: 0073 d801 0000 6401 6402 6702 7d03 6700  .s....d.d.g.}.g.
+00000c70: 7d04 6900 7d05 7c00 6a00 6403 6404 8d01  }.i.}.|.j.d.d...
+00000c80: 4400 9001 5d14 5c02 7d06 7d07 7c02 7234  D...].\.}.}.|.r4
+00000c90: 7401 7c06 8301 7d08 6e0c 7402 7c07 6405  t.|...}.n.t.|.d.
+00000ca0: 1900 8301 7d08 7402 7c07 6405 1900 8301  ....}.t.|.d.....
+00000cb0: 7d09 7c09 7c05 7c06 3c00 6406 7c07 7600  }.|.|.|.<.d.|.v.
+00000cc0: 7282 7c07 6406 1900 7282 7c09 7c01 7600  r.|.d...r.|.|.v.
+00000cd0: 7282 6407 a003 7c08 7c09 a102 a004 6408  r.d...|.|.....d.
+00000ce0: 6409 a102 7d0a 6ea6 6406 7c07 7600 72a8  d...}.n.d.|.v.r.
+00000cf0: 7c07 6406 1900 72a8 640a a003 7c08 7c09  |.d...r.d...|.|.
+00000d00: a102 a004 6408 6409 a102 7d0a 6e80 640b  ....d.d...}.n.d.
+00000d10: 7c07 7600 72ce 7c07 640b 1900 72ce 640c  |.v.r.|.d...r.d.
+00000d20: a003 7c08 7c09 a102 a004 6408 6409 a102  ..|.|.....d.d...
+00000d30: 7d0a 6e5a 640d 7c07 7600 72f4 7c07 640d  }.nZd.|.v.r.|.d.
+00000d40: 1900 72f4 640a a003 7c08 7c09 a102 a004  ..r.d...|.|.....
+00000d50: 6408 6409 a102 7d0a 6e34 7c09 7c01 7600  d.d...}.n4|.|.v.
+00000d60: 9001 7214 640e a003 7c08 7c09 a102 a004  ..r.d...|.|.....
+00000d70: 6408 6409 a102 7d0a 6e14 640f a003 7c08  d.d...}.n.d...|.
+00000d80: 7c09 a102 a004 6408 6409 a102 7d0a 7c04  |.....d.d...}.|.
+00000d90: a005 7c0a a101 0100 711c 7c03 7406 7c04  ..|.....q.|.t.|.
+00000da0: 8301 3700 7d03 6700 7d0b 7c00 6a07 6403  ..7.}.g.}.|.j.d.
+00000db0: 6404 8d01 4400 5d66 5c03 7d0c 7d0d 7d0e  d...D.]f\.}.}.}.
+00000dc0: 6410 7c0e 7600 9001 7250 7c05 7c0c 1900  d.|.v...rP|.|...
+00000dd0: 7d0f 7c05 7c0d 1900 7d10 7c02 9001 729c  }.|.|...}.|...r.
+00000de0: 7c0b a005 6411 a003 7401 7c0c 8301 7401  |...d...t.|...t.
+00000df0: 7c0d 8301 7c0e 6410 1900 a103 a101 0100  |...|.d.........
+00000e00: 6e18 7c0b a005 6411 a003 7c0f 7c10 7c0e  n.|...d...|.|.|.
+00000e10: 6410 1900 a103 a101 0100 9001 7150 7c03  d...........qP|.
+00000e20: 7406 7c0b 8301 3700 7d03 7c03 a005 6412  t.|...7.}.|...d.
+00000e30: a101 0100 6413 a008 7c03 a101 5300 2914  ....d...|...S.).
+00000e40: 4e72 3700 0000 7238 0000 0054 723a 0000  Nr7...r8...Tr:..
+00000e50: 0072 1a00 0000 723c 0000 007a 5909 7b30  .r....r<...zY.{0
+00000e60: 7d20 5b73 6861 7065 203d 2063 6972 636c  } [shape = circl
+00000e70: 652c 206c 6162 656c 203d 2022 7b31 7d22  e, label = "{1}"
+00000e80: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
+00000e90: 2020 2020 2020 7374 796c 653d 6669 6c6c        style=fill
+00000ea0: 6564 2c20 6669 6c6c 636f 6c6f 723d 7075  ed, fillcolor=pu
+00000eb0: 7270 6c65 5d3b 723d 0000 0072 2100 0000  rple];r=...r!...
+00000ec0: 7a49 097b 307d 205b 7368 6170 6520 3d20  zI.{0} [shape = 
+00000ed0: 6369 7263 6c65 2c20 6c61 6265 6c20 3d20  circle, label = 
+00000ee0: 227b 317d 222c 2020 2020 2020 2020 2020  "{1}",          
+00000ef0: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+00000f00: 3d22 6669 6c6c 6564 225d 3b72 3e00 0000  ="filled"];r>...
+00000f10: 7a58 097b 307d 205b 7368 6170 6520 3d20  zX.{0} [shape = 
+00000f20: 6369 7263 6c65 2c20 6c61 6265 6c20 3d20  circle, label = 
+00000f30: 227b 317d 222c 2020 2020 2020 2020 2020  "{1}",          
+00000f40: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+00000f50: 3d22 6669 6c6c 6564 222c 2066 696c 6c63  ="filled", fillc
+00000f60: 6f6c 6f72 3d72 6564 5d3b 723f 0000 0072  olor=red];r?...r
+00000f70: 4000 0000 7241 0000 0072 4200 0000 7243  @...rA...rB...rC
+00000f80: 0000 0072 4400 0000 7245 0000 0029 0972  ...rD...rE...).r
+00000f90: 4a00 0000 724b 0000 0072 3600 0000 7211  J...rK...r6...r.
+00000fa0: 0000 0072 2f00 0000 7249 0000 0072 4c00  ...r/...rI...rL.
+00000fb0: 0000 724d 0000 0072 4e00 0000 2911 722b  ..rM...rN...).r+
+00000fc0: 0000 0072 5000 0000 7251 0000 0072 5200  ...rP...rQ...rR.
+00000fd0: 0000 7253 0000 0072 5400 0000 7217 0000  ..rS...rT...r...
+00000fe0: 0072 5500 0000 7256 0000 0072 5700 0000  .rU...rV...rW...
+00000ff0: 7258 0000 0072 5900 0000 725a 0000 0072  rX...rY...rZ...r
+00001000: 5b00 0000 725c 0000 0072 5d00 0000 725e  [...r\...r]...r^
+00001010: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
+00001020: 0000 da06 746f 5f64 6f74 8100 0000 7382  ....to_dot....s.
+00001030: 0000 0000 0108 0304 0104 0116 0104 010a  ................
+00001040: 020c 010c 0108 0118 0104 0204 fe04 0404  ................
+00001050: fc06 0610 0104 0204 fe04 0404 fc06 0610  ................
+00001060: 0104 0204 fe04 0404 fc06 0610 0104 0204  ................
+00001070: fe04 0404 fc06 060a 0104 0104 ff04 0304  ................
+00001080: fd06 0604 0104 ff04 0204 fe04 030c 010c  ................
+00001090: 0204 0116 010a 0108 0108 0206 0104 0104  ................
+000010a0: 0112 ff02 ff06 0704 0104 010a ff02 ff08  ................
+000010b0: 060c 010a 0172 6000 0000 290a 7230 0000  .....r`...).r0..
+000010c0: 00da 056e 756d 7079 7214 0000 005a 0c73  ...numpyr....Z.s
+000010d0: 6b6c 6561 726e 2e74 7265 6572 0200 0000  klearn.treer....
+000010e0: 7220 0000 0072 3600 0000 da03 7365 7472  r ...r6.....setr
+000010f0: 5f00 0000 7260 0000 0072 0900 0000 7209  _...r`...r....r.
+00001100: 0000 0072 0900 0000 720a 0000 00da 083c  ...r....r......<
+00001110: 6d6f 6475 6c65 3e01 0000 0073 0c00 0000  module>....s....
+00001120: 0802 0801 0c03 081b 0810 104f            ...........O
```

### Comparing `xpotato-0.1.4/xpotato/models/model.py` & `xpotato-0.1.5/xpotato/models/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-import numpy as np
 from collections import defaultdict
+
+import numpy as np
 from tuw_nlp.common.vocabulary import Vocabulary
 from tuw_nlp.graph.lexical import LexGraphs
 from tuw_nlp.graph.utils import graph_to_pn
+
 from xpotato.models.utils import tree_to_code
 
 
 class GraphModel:
     def __init__(self):
         self.lexgraphs = LexGraphs()
         self.feature_vocab = Vocabulary()
```

### Comparing `xpotato-0.1.4/xpotato/models/trainer.py` & `xpotato-0.1.5/xpotato/models/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from collections import defaultdict
-from typing import Dict, List
-from typing import Union
 from math import log2, sqrt
-from rank_bm25 import BM25Okapi
+from typing import Dict, List, Union
 
 import eli5
 import pandas as pd
-from xpotato.graph_extractor.extract import GraphExtractor, FeatureEvaluator
-from xpotato.models.model import GraphModel
-from sklearn.linear_model import LogisticRegression
-from tqdm import tqdm
-
 import skcriteria as skc
+from rank_bm25 import BM25Okapi
 from skcriteria.madm import simple
 from skcriteria.pipeline import mkpipe
 from skcriteria.preprocessing import invert_objectives, scalers
+from sklearn.linear_model import LogisticRegression
+from tqdm import tqdm
+
+from xpotato.graph_extractor.extract import FeatureEvaluator, GraphExtractor
+from xpotato.models.model import GraphModel
 
 
 class GraphTrainer:
     def __init__(
         self,
         dataset: pd.DataFrame,
         lang: str = "en",
```

### Comparing `xpotato-0.1.4/xpotato/models/utils.py` & `xpotato-0.1.5/xpotato/models/utils.py`

 * *Files identical despite different names*

### Comparing `xpotato-0.1.4/xpotato.egg-info/PKG-INFO` & `xpotato-0.1.5/xpotato.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,434 +1,447 @@
 Metadata-Version: 2.1
 Name: xpotato
-Version: 0.1.4
+Version: 0.1.5
 Summary: XAI human-in-the-loop information extraction framework
 Home-page: https://github.com/adaamko/POTATO
 Author: Adam Kovacs, Gabor Recski
 Author-email: adam.kovacs@tuwien.ac.at, gabor.recski@tuwien.ac.at
 License: MIT
-Description: <p align="center">
-          <img src="https://raw.githubusercontent.com/adaamko/POTATO/dev/files/potato_logo.png" />
-        </p>
-        
-        # POTATO: exPlainable infOrmation exTrAcTion framewOrk
-        POTATO is a human-in-the-loop XAI framework for extracting and evaluating interpretable graph features for any classification problem in Natural Language Processing.
-        
-        ## Built systems
-        
-        To get started with rule-systems we provide rule-based features prebuilt with POTATO on different datasets (e.g. our paper _Offensive text detection on English Twitter with deep learning models and rule-based systems_ for the HASOC2021 shared task). If you are interested in that, you can go under _features/_ for more info!
-        
-        ## Install and Quick Start
-        Check out our quick demonstration (~2 min) video about the tool:
-        https://youtu.be/PkQ71wUSeNU
-        
-        There is a longer version with a detailed method description and presented background research (~1 hour): https://youtu.be/6R_V1WfIjsU
-        
-        ### Setup
-        The tool is heavily dependent upon the [tuw-nlp](https://github.com/recski/tuw-nlp) repository. You can install tuw-nlp with pip:
-        
-        ```
-        pip install tuw-nlp
-        ```
-        Then follow the [instructions](https://github.com/recski/tuw-nlp) to setup the package.
-        
-        
-        Then install POTATO from pip:
-        
-        ```
-        pip install xpotato
-        ```
-        
-        Or you can install it from source:
-        
-        ```
-        pip install -e .
-        ```
-        
-        ### Usage
-        
-        - POTATO is an IE tool that works on graphs, currently we support three types of graphs: AMR, UD and [Fourlang](https://github.com/kornai/4lang). 
-        
-        - In the README we provide examples with fourlang semantic graphs. Make sure to follow the instructions in the [tuw_nlp](https://github.com/recski/tuw-nlp) repo to be able to build fourlang graphs. 
-        
-        - If you are interested in AMR graphs, you can go to the [hasoc](https://github.com/adaamko/POTATO/tree/main/features/hasoc) folder To get started with rule-systems prebuilt with POTATO on the HASOC dataset (we also presented a paper named _Offensive text detection on English Twitter with deep learning models and rule-based systems_ for the HASOC2021 shared task). 
-        
-        - We also provide experiments on the [CrowdTruth](https://github.com/CrowdTruth/Medical-Relation-Extraction) medical relation extraction datasets with UD graphs, go to the [crowdtruth](https://github.com/adaamko/POTATO/tree/main/features/crowdtruth) folder for more info!
-        
-        - POTATO can also handle unlabeled, or partially labeled data, see [advanced](###advanced-mode) mode to get to know more.
-        
-        __To see complete working examples go under the _notebooks/_ folder to see experiments on HASOC and on the Semeval relation extraction dataset.__
-        
-        First import packages from potato:
-        ```python
-        from xpotato.dataset.dataset import Dataset
-        from xpotato.models.trainer import GraphTrainer
-        ```
-        
-        First we demonstrate POTATO's capabilities with a few sentences manually picked from the dataset.
-        
-        __Note that we replaced the two entitites in question with _XXX_ and _YYY_.__
-        
-        ```python
-        sentences = [("Governments and industries in nations around the world are pouring XXX into YYY.", "Entity-Destination(e1,e2)"),
-                    ("The scientists poured XXX into pint YYY.", "Entity-Destination(e1,e2)"),
-                    ("The suspect pushed the XXX into a deep YYY.", "Entity-Destination(e1,e2)"),
-                    ("The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.", "Other"),
-                    ("The entity1 to buy papers is pushed into the next entity2.", "Entity-Destination(e1,e2)"),
-                    ("An unnamed XXX was pushed into the YYY.", "Entity-Destination(e1,e2)"),
-                    ("Since then, numerous independent feature XXX have journeyed into YYY.", "Other"),
-                    ("For some reason, the XXX was blinded from his own YYY about the incommensurability of time.", "Other"),
-                    ("Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.", "Other"),
-                    ("Olympics have already poured one XXX into the YYY.", "Entity-Destination(e1,e2)"),
-                    ("After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.", "Entity-Destination(e1,e2)"),
-                    ("I placed the XXX in a natural YYY, at the base of a part of the fallen arch.", "Entity-Destination(e1,e2)"),
-                    ("The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.", "Other"),
-                    ("The XXX leaked from every conceivable YYY.", "Other"),
-                    ("The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse.", "Entity-Destination(e1,e2)"),
-                    ("The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.", "Other"),
-                    ("Gaza XXX recover from three YYY of war.", "Other"),
-                    ("This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.", "Other")]
-        ```
-        
-        Initialize the dataset and also provide a label encoding. Then parse the sentences into graphs. Currently we provide three types of graphs: _ud_, _fourlang_, _amr_. Also provide the language you want to parse, currently we support English (en) and German (de).
-        
-        ```python
-        dataset = Dataset(sentences, label_vocab={"Other":0, "Entity-Destination(e1,e2)": 1}, lang="en")
-        dataset.set_graphs(dataset.parse_graphs(graph_format="ud"))
-        ```
-        
-        Check the dataset:
-        ```python
-        df = dataset.to_dataframe()
-        ```
-        
-        We can also check any of the graphs:
-        ### Check any of the graphs parsed
-        
-        ```python
-        from xpotato.models.utils import to_dot
-        from graphviz import Source
-        
-        Source(to_dot(df.iloc[0].graph))
-        ```
-        ![graph](https://raw.githubusercontent.com/adaamko/POTATO/main/files/re_example.svg)
-        
-        ### Rules
-        
-        If the dataset is prepared and the graphs are parsed, we can write rules to match labels. We can write rules either manually or extract
-        them automatically (POTATO also provides a frontend that tries to do both).
-        
-        The simplest rule would be just a node in the graph:
-        ```python
-        # The syntax of the rules is List[List[rules that we want to match], List[rules that shouldn't be in the matched graphs], Label of the rule]
-        rule_to_match = [[["(u_1 / into)"], [], "Entity-Destination(e1,e2)"]]
-        ```
-        
-        Init the rule matcher:
-        ```python
-        from xpotato.graph_extractor.extract import FeatureEvaluator
-        evaluator = FeatureEvaluator()
-        ```
-        
-        Match the rules in the dataset:
-        ```python
-        #match single feature
-        df = dataset.to_dataframe()
-        evaluator.match_features(df, rule_to_match)
-        ```
-        
-        |    | Sentence                                                                                                                        | Predicted label           | Matched rule                                        |
-        |---:|:--------------------------------------------------------------------------------------------------------------------------------|:--------------------------|:----------------------------------------------------|
-        |  0 | Governments and industries in nations around the world are pouring XXX into YYY.                                                | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        |  1 | The scientists poured XXX into pint YYY.                                                                                        | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        |  2 | The suspect pushed the XXX into a deep YYY.                                                                                     | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        |  3 | The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.                                  | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        |  4 | The entity1 to buy papers is pushed into the next entity2.                                                                      | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        |  5 | An unnamed XXX was pushed into the YYY.                                                                                         | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        |  6 | Since then, numerous independent feature XXX have journeyed into YYY.                                                           | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        |  7 | For some reason, the XXX was blinded from his own YYY about the incommensurability of time.                                     |                           |                                                     |
-        |  8 | Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.           |                           |                                                     |
-        |  9 | Olympics have already poured one XXX into the YYY.                                                                              | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        | 10 | After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.                            |                           |                                                     |
-        | 11 | I placed the XXX in a natural YYY, at the base of a part of the fallen arch.                                                    |                           |                                                     |
-        | 12 | The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.            |                           |                                                     |
-        | 13 | The XXX leaked from every conceivable YYY.                                                                                      |                           |                                                     |
-        | 14 | The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse. | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
-        | 15 | The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.                   |                           |                                                     |
-        | 16 | Gaza XXX recover from three YYY of war.                                                                                         |                           |                                                     |
-        | 17 | This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.  |                           |                                                     |
-        
-        
-        
-        You can see in the dataset that the rules only matched the instances where the "into" node was present.
-        
-        One of the core features of our tool is that we are also able to match subgraphs. To describe a graph, we use the [PENMAN](https://github.com/goodmami/penman) notation. 
-        
-        E.g. the string _(u_1 / into :1 (u_3 / pour))_ would describe a graph with two nodes ("into" and "pour") and a single directed edge with the label "1" between them.
-        ```python
-        #match a simple graph feature
-        evaluator.match_features(df, [[["(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))"], [], "Entity-Destination(e1,e2)"]])
-        ```
-        
-        Describing a subgraph with the string "(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))" will return only three examples instead of 9 (when we only had a single node as a feature)
-        |    | Sentence                                                                                                                        | Predicted label           | Matched rule                                                                       |
-        |---:|:--------------------------------------------------------------------------------------------------------------------------------|:--------------------------|:-----------------------------------------------------------------------------------|
-        |  0 | Governments and industries in nations around the world are pouring XXX into YYY.                                                | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        |  1 | The scientists poured XXX into pint YYY.                                                                                        | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        |  2 | The suspect pushed the XXX into a deep YYY.                                                                                     |                           |                                                                                    |
-        |  3 | The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.                                  |                           |                                                                                    |
-        |  4 | The entity1 to buy papers is pushed into the next entity2.                                                                      |                           |                                                                                    |
-        |  5 | An unnamed XXX was pushed into the YYY.                                                                                         |                           |                                                                                    |
-        |  6 | Since then, numerous independent feature XXX have journeyed into YYY.                                                           |                           |                                                                                    |
-        |  7 | For some reason, the XXX was blinded from his own YYY about the incommensurability of time.                                     |                           |                                                                                    |
-        |  8 | Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.           |                           |                                                                                    |
-        |  9 | Olympics have already poured one XXX into the YYY.                                                                              | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        | 10 | After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.                            |                           |                                                                                    |
-        | 11 | I placed the XXX in a natural YYY, at the base of a part of the fallen arch.                                                    |                           |                                                                                    |
-        | 12 | The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.            |                           |                                                                                    |
-        | 13 | The XXX leaked from every conceivable YYY.                                                                                      |                           |                                                                                    |
-        | 14 | The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse. |                           |                                                                                    |
-        | 15 | The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.                   |                           |                                                                                    |
-        | 16 | Gaza XXX recover from three YYY of war.                                                                                         |                           |                                                                                    |
-        | 17 | This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.  |                           |                                                                                    |
-        
-        
-        We can also add negated features that we don't want to match (e.g. this won't match the first row where 'pour' is present):
-        ```python
-        #match a simple graph feature
-        evaluator.match_features(df, [[["(u_1 / into :2 (u_3 / YYY))"], ["(u_2 / pour)"], "Entity-Destination(e1,e2)"]])
-        ```
-        
-        |    | Sentence                                                                                                                        | Predicted label           | Matched rule                                                                     |
-        |---:|:--------------------------------------------------------------------------------------------------------------------------------|:--------------------------|:---------------------------------------------------------------------------------|
-        |  0 | Governments and industries in nations around the world are pouring XXX into YYY.                                                |                           |                                                                                  |
-        |  1 | The scientists poured XXX into pint YYY.                                                                                        |                           |                                                                                  |
-        |  2 | The suspect pushed the XXX into a deep YYY.                                                                                     | Entity-Destination(e1,e2) | [['(u_1 / into :2 (u_3 / YYY))'], ['(u_2 / pour)'], 'Entity-Destination(e1,e2)'] |
-        |  3 | The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.                                  | Entity-Destination(e1,e2) | [['(u_1 / into :2 (u_3 / YYY))'], ['(u_2 / pour)'], 'Entity-Destination(e1,e2)'] |
-        |  4 | The entity1 to buy papers is pushed into the next entity2.                                                                      |                           |                                                                                  |
-        |  5 | An unnamed XXX was pushed into the YYY.                                                                                         | Entity-Destination(e1,e2) | [['(u_1 / into :2 (u_3 / YYY))'], ['(u_2 / pour)'], 'Entity-Destination(e1,e2)'] |
-        |  6 | Since then, numerous independent feature XXX have journeyed into YYY.                                                           | Entity-Destination(e1,e2) | [['(u_1 / into :2 (u_3 / YYY))'], ['(u_2 / pour)'], 'Entity-Destination(e1,e2)'] |
-        |  7 | For some reason, the XXX was blinded from his own YYY about the incommensurability of time.                                     |                           |                                                                                  |
-        |  8 | Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.           |                           |                                                                                  |
-        |  9 | Olympics have already poured one XXX into the YYY.                                                                              |                           |                                                                                  |
-        | 10 | After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.                            |                           |                                                                                  |
-        | 11 | I placed the XXX in a natural YYY, at the base of a part of the fallen arch.                                                    |                           |                                                                                  |
-        | 12 | The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.            |                           |                                                                                  |
-        | 13 | The XXX leaked from every conceivable YYY.                                                                                      |                           |                                                                                  |
-        | 14 | The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse. |                           |                                                                                  |
-        | 15 | The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.                   |                           |                                                                                  |
-        | 16 | Gaza XXX recover from three YYY of war.                                                                                         |                           |                                                                                  |
-        | 17 | This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.  |                           |                                                                                  |
-        
-        If we don't want to specify nodes, regex can also be used in place of the node and edge-names:
-        
-        ```python
-        #regex can be used to match any node (this will match instances where 'into' is connected to any node with '1' edge)
-        evaluator.match_features(df, [[["(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))"], [], "Entity-Destination(e1,e2)"]])
-        ```
-        
-        |    | Sentence                                                                                                                        | Predicted label           | Matched rule                                                                     |
-        |---:|:--------------------------------------------------------------------------------------------------------------------------------|:--------------------------|:---------------------------------------------------------------------------------|
-        |  0 | Governments and industries in nations around the world are pouring XXX into YYY.                                                | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        |  1 | The scientists poured XXX into pint YYY.                                                                                        | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        |  2 | The suspect pushed the XXX into a deep YYY.                                                                                     | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        |  3 | The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.                                  | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        |  4 | The entity1 to buy papers is pushed into the next entity2.                                                                      |                           |                                                                                  |
-        |  5 | An unnamed XXX was pushed into the YYY.                                                                                         | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        |  6 | Since then, numerous independent feature XXX have journeyed into YYY.                                                           | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        |  7 | For some reason, the XXX was blinded from his own YYY about the incommensurability of time.                                     |                           |                                                                                  |
-        |  8 | Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.           |                           |                                                                                  |
-        |  9 | Olympics have already poured one XXX into the YYY.                                                                              | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
-        | 10 | After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.                            |                           |                                                                                  |
-        | 11 | I placed the XXX in a natural YYY, at the base of a part of the fallen arch.                                                    |                           |                                                                                  |
-        | 12 | The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.            |                           |                                                                                  |
-        | 13 | The XXX leaked from every conceivable YYY.                                                                                      |                           |                                                                                  |
-        | 14 | The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse. |                           |                                                                                  |
-        | 15 | The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.                   |                           |                                                                                  |
-        | 16 | Gaza XXX recover from three YYY of war.                                                                                         |                           |                                                                                  |
-        | 17 | This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.  |                           |                                                                                  |
-        
-        We can also train regex rules from a training data, this will automatically replace regex '.*' with nodes that are 
-        'good enough' statistically based on the provided dataframe.
-        
-        ```python
-        evaluator.train_feature("Entity-Destination(e1,e2)", "(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))", df)
-        ```
-        
-        This returns '(u_1 / into :1 (u_2 / push|pour) :2 (u_3 / YYY))' (replaced '.*' with _push_ and _pour_)
-        
-        ### Learning rules
-        
-        To extract rules automatically, train the dataset with graph features and rank them based on relevancy:
-        
-        ```python
-        df = dataset.to_dataframe()
-        trainer = GraphTrainer(df)
-        #extract features
-        features = trainer.prepare_and_train()
-        
-        from xpotato.dataset.utils import save_dataframe
-        from sklearn.model_selection import train_test_split
-        
-        train, val = train_test_split(df, test_size=0.2, random_state=1234)
-        
-        #save train and validation, this is important for the frontend to work
-        save_dataframe(train, 'train.tsv')
-        save_dataframe(val, 'val.tsv')
-        
-        import json
-        
-        #also save the ranked features
-        with open("features.json", "w+") as f:
-            json.dump(features, f)
-        
-        ```
-        
-        You can also save the parsed graphs for evaluation or for caching:
-        
-        ```python
-        import pickle
-        with open("graphs.pickle", "wb") as f:
-            pickle.dump(val.graph, f)
-        ```
-        
-        ## Frontend
-        
-        If the DataFrame is ready with the parsed graphs, the UI can be started to inspect the extracted rules and modify them. The frontend is a streamlit app, the simplest way of starting it is (the training and the validation dataset must be provided):
-        
-        ```
-        streamlit run frontend/app.py -- -t notebooks/train.tsv -v notebooks/val.tsv -g ud
-        ```
-        
-        it can be also started with the extracted features:
-        
-        ```
-        streamlit run frontend/app.py -- -t notebooks/train.tsv -v notebooks/val.tsv -g ud -sr notebooks/features.json
-        ```
-        
-        if you already used the UI and extracted the features manually and you want to load it, you can run:
-        ```
-        streamlit run frontend/app.py -- -t notebooks/train.tsv -v notebooks/val.tsv -g ud -sr notebooks/features.json -hr notebooks/manual_features.json
-        ```
-        
-        ### Advanced mode
-        
-        If labels are not or just partially provided, the frontend can be started also in _advanced_ mode, where the user can _annotate_ a few examples at the start, then the system gradually offers rules based on the provided examples. 
-        
-        
-        Dataset without labels can be initialized with:
-        ```python
-        sentences = [("Governments and industries in nations around the world are pouring XXX into YYY.", ""),
-                    ("The scientists poured XXX into pint YYY.", ""),
-                    ("The suspect pushed the XXX into a deep YYY.", ""),
-                    ("The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.", ""),
-                    ("The entity1 to buy papers is pushed into the next entity2.", ""),
-                    ("An unnamed XXX was pushed into the YYY.", ""),
-                    ("Since then, numerous independent feature XXX have journeyed into YYY.", ""),
-                    ("For some reason, the XXX was blinded from his own YYY about the incommensurability of time.", ""),
-                    ("Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.", ""),
-                    ("Olympics have already poured one XXX into the YYY.", ""),
-                    ("After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.", ""),
-                    ("I placed the XXX in a natural YYY, at the base of a part of the fallen arch.", ""),
-                    ("The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.", ""),
-                    ("The XXX leaked from every conceivable YYY.", ""),
-                    ("The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse.", ""),
-                    ("The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.", ""),
-                    ("Gaza XXX recover from three YYY of war.", ""),
-                    ("This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.", "")]
-        ```
-        
-        
-        Then, the frontend can be started:
-        ```
-        streamlit run frontend/app.py -- -t notebooks/unsupervised_dataset.tsv -g ud -m advanced
-        ```
-        
-        Once the frontend starts up and you define the labels, you are faced with the annotation interface. You can search elements by clicking on the appropriate column name and applying the desired filter. You can annotate instances by checking the checkbox at the beginning of the line. You can check multiple checkboxs at a time. Once you've selected the utterances you want to annotate, click on the _Annotate_ button. The annotated samples will appear in the lower table. You can clear the annotation of certain elements by selecting them in the second table and clicking _Clear annotation_.
-        
-        Once you have some annotated data, you can train rules by clicking the _Train!_ button. It is recommended to set the _Rank features based on accuracy_ to True, if you have just a few samples. You will get a similar interface as in supervised mode, you can generate rule suggestions, and write your own rules as usual. Once you are satisfied with the rules, select each of them and click _annotate based on selected_. This process might take a while if you are working with large data. You should get all the rule matches marked in the first and the second tables. You can order the tables by each column, so it's easier to check. You will have to manually accept the annotations generated this way for them to appear in the second table.
-        
-        - You can read about the use of the advanced mode in the [docs](https://github.com/adaamko/POTATO/tree/main/docs/README_advanced_mode.md)
-        
-        
-        ## Evaluate
-        If you have the features ready and you want to evaluate them on a test set, you can run:
-        
-        ```python
-        python scripts/evaluate.py -t ud -f notebooks/features.json -d notebooks/val.tsv
-        ```
-        
-        The result will be a _csv_ file with the labels and the matched rules.
-        
-        ## Service
-        If you are ready with the extracted features and want to use our package in production for inference (generating predictions for sentences), we also provide a REST API built on POTATO (based on [fastapi](https://github.com/tiangolo/fastapi)).
-        
-        First install FastAPI and [Uvicorn](https://www.uvicorn.org/)
-        ```bash
-        pip install fastapi
-        pip install "uvicorn[standard]"
-        ```
-        
-        To start the service, you should set _language_, _graph\_type_ and the _features_  for the service. This can be done through enviroment variables.
-        
-        Example:
-        ```bash
-        export FEATURE_PATH=/home/adaamko/projects/POTATO/features/semeval/test_features.json
-        export GRAPH_FORMAT=ud
-        export LANG=en
-        ```
-        
-        Then, start the REST API:
-        ```python
-        python services/main.py
-        ```
-        
-        It will start a service running on _localhost_ on port _8000_ (it will also initialize the correct models).
-        
-        Then you can use any client to make post requests:
-        ```bash
-        curl -X POST localhost:8000 -H 'Content-Type: application/json' -d '{"text":"The suspect pushed the XXX into a deep YYY.\nSparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week."}'
-        ```
-        
-        The answer will be a list with the predicted labels (if none of the rules match, it will return "NONE"):
-        ```bash
-        ["Entity-Destination(e1,e2)","NONE"]
-        ```
-        
-        The streamlit frontend also has an inference mode, where the implemented rule-system can be used for inference. It can be started with:
-        
-        ```bash
-        streamlit run frontend/app.py -- -hr features/semeval/test_features.json -m inference
-        ```
-        
-        ## Contributing
-        
-        We welcome all contributions! Please fork this repository and create a branch for your modifications. We suggest getting in touch with us first, by opening an issue or by writing an email to Adam Kovacs or Gabor Recski at firstname.lastname@tuwien.ac.at
-        
-        ## Citing
-        
-        If you use the library, please cite our [paper](https://arxiv.org/abs/2201.13230)
-        
-        ```bib
-        @article{Kovacs:2022,
-          title={{POTATO: exPlainable infOrmation exTrAcTion framewOrk}},
-          author={Kov{\'a}cs, {\'A}d{\'a}m and G{\'e}mes, Kinga and Ikl{\'o}di, Eszter and Recski, G{\'a}bor},
-          journal={arXiv preprint arXiv:2201.13230},
-          year={2022}
-        }
-        ```
-        
-        ## License 
-        
-        MIT license
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/adaamko/POTATO/dev/files/potato_logo.png" />
+</p>
+
+# POTATO: exPlainable infOrmation exTrAcTion framewOrk
+POTATO is a human-in-the-loop XAI framework for extracting and evaluating interpretable graph features for any classification problem in Natural Language Processing.
+
+## Built systems
+
+To get started with rule-systems we provide rule-based features prebuilt with POTATO on different datasets (e.g. our paper _Offensive text detection on English Twitter with deep learning models and rule-based systems_ for the HASOC2021 shared task). If you are interested in that, you can go under _features/_ for more info!
+
+## Install and Quick Start
+Check out our quick demonstration (~2 min) video about the tool:
+https://youtu.be/PkQ71wUSeNU
+
+There is a longer version with a detailed method description and presented background research (~1 hour): https://youtu.be/6R_V1WfIjsU
+
+### Setup
+The tool is heavily dependent upon the [tuw-nlp](https://github.com/recski/tuw-nlp) repository. You can install tuw-nlp with pip:
+
+```
+pip install tuw-nlp
+```
+Then follow the [instructions](https://github.com/recski/tuw-nlp) to setup the package.
+
+
+Then install POTATO from pip:
+
+```
+pip install xpotato
+```
+
+Or you can install it from source:
+
+```
+pip install -e .
+```
+
+### Usage
+
+- POTATO is an IE tool that works on graphs, currently we support three types of graphs: AMR, UD and [Fourlang](https://github.com/kornai/4lang). 
+
+- In the README we provide examples with fourlang semantic graphs. Make sure to follow the instructions in the [tuw_nlp](https://github.com/recski/tuw-nlp) repo to be able to build fourlang graphs. 
+
+- If you are interested in AMR graphs, you can go to the [hasoc](https://github.com/adaamko/POTATO/tree/main/features/hasoc) folder To get started with rule-systems prebuilt with POTATO on the HASOC dataset (we also presented a paper named _Offensive text detection on English Twitter with deep learning models and rule-based systems_ for the HASOC2021 shared task). 
+
+- We also provide experiments on the [CrowdTruth](https://github.com/CrowdTruth/Medical-Relation-Extraction) medical relation extraction datasets with UD graphs, go to the [crowdtruth](https://github.com/adaamko/POTATO/tree/main/features/crowdtruth) folder for more info!
+
+- POTATO can also handle unlabeled, or partially labeled data, see [advanced](###advanced-mode) mode to get to know more.
+
+__To see complete working examples go under the _notebooks/_ folder to see experiments on HASOC and on the Semeval relation extraction dataset.__
+
+First import packages from potato:
+```python
+from xpotato.dataset.dataset import Dataset
+from xpotato.models.trainer import GraphTrainer
+```
+
+First we demonstrate POTATO's capabilities with a few sentences manually picked from the dataset.
+
+__Note that we replaced the two entitites in question with _XXX_ and _YYY_.__
+
+```python
+sentences = [("Governments and industries in nations around the world are pouring XXX into YYY.", "Entity-Destination(e1,e2)"),
+            ("The scientists poured XXX into pint YYY.", "Entity-Destination(e1,e2)"),
+            ("The suspect pushed the XXX into a deep YYY.", "Entity-Destination(e1,e2)"),
+            ("The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.", "Other"),
+            ("The entity1 to buy papers is pushed into the next entity2.", "Entity-Destination(e1,e2)"),
+            ("An unnamed XXX was pushed into the YYY.", "Entity-Destination(e1,e2)"),
+            ("Since then, numerous independent feature XXX have journeyed into YYY.", "Other"),
+            ("For some reason, the XXX was blinded from his own YYY about the incommensurability of time.", "Other"),
+            ("Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.", "Other"),
+            ("Olympics have already poured one XXX into the YYY.", "Entity-Destination(e1,e2)"),
+            ("After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.", "Entity-Destination(e1,e2)"),
+            ("I placed the XXX in a natural YYY, at the base of a part of the fallen arch.", "Entity-Destination(e1,e2)"),
+            ("The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.", "Other"),
+            ("The XXX leaked from every conceivable YYY.", "Other"),
+            ("The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse.", "Entity-Destination(e1,e2)"),
+            ("The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.", "Other"),
+            ("Gaza XXX recover from three YYY of war.", "Other"),
+            ("This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.", "Other")]
+```
+
+Initialize the dataset and also provide a label encoding. Then parse the sentences into graphs. Currently we provide three types of graphs: _ud_, _fourlang_, _amr_. Also provide the language you want to parse, currently we support English (en) and German (de).
+
+```python
+dataset = Dataset(sentences, label_vocab={"Other":0, "Entity-Destination(e1,e2)": 1}, lang="en")
+dataset.set_graphs(dataset.parse_graphs(graph_format="ud"))
+```
+
+Check the dataset:
+```python
+df = dataset.to_dataframe()
+```
+
+We can also check any of the graphs:
+### Check any of the graphs parsed
+
+```python
+from xpotato.models.utils import to_dot
+from graphviz import Source
+
+Source(to_dot(df.iloc[0].graph))
+```
+![graph](https://raw.githubusercontent.com/adaamko/POTATO/main/files/re_example.svg)
+
+### Rules
+
+If the dataset is prepared and the graphs are parsed, we can write rules to match labels. We can write rules either manually or extract
+them automatically (POTATO also provides a frontend that tries to do both).
+
+The simplest rule would be just a node in the graph:
+```python
+# The syntax of the rules is List[List[rules that we want to match], List[rules that shouldn't be in the matched graphs], Label of the rule]
+rule_to_match = [[["(u_1 / into)"], [], "Entity-Destination(e1,e2)"]]
+```
+
+Init the rule matcher:
+```python
+from xpotato.graph_extractor.extract import FeatureEvaluator
+evaluator = FeatureEvaluator()
+```
+
+Match the rules in the dataset:
+```python
+#match single feature
+df = dataset.to_dataframe()
+evaluator.match_features(df, rule_to_match)
+```
+
+|    | Sentence                                                                                                                        | Predicted label           | Matched rule                                        |
+|---:|:--------------------------------------------------------------------------------------------------------------------------------|:--------------------------|:----------------------------------------------------|
+|  0 | Governments and industries in nations around the world are pouring XXX into YYY.                                                | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+|  1 | The scientists poured XXX into pint YYY.                                                                                        | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+|  2 | The suspect pushed the XXX into a deep YYY.                                                                                     | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+|  3 | The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.                                  | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+|  4 | The entity1 to buy papers is pushed into the next entity2.                                                                      | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+|  5 | An unnamed XXX was pushed into the YYY.                                                                                         | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+|  6 | Since then, numerous independent feature XXX have journeyed into YYY.                                                           | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+|  7 | For some reason, the XXX was blinded from his own YYY about the incommensurability of time.                                     |                           |                                                     |
+|  8 | Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.           |                           |                                                     |
+|  9 | Olympics have already poured one XXX into the YYY.                                                                              | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+| 10 | After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.                            |                           |                                                     |
+| 11 | I placed the XXX in a natural YYY, at the base of a part of the fallen arch.                                                    |                           |                                                     |
+| 12 | The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.            |                           |                                                     |
+| 13 | The XXX leaked from every conceivable YYY.                                                                                      |                           |                                                     |
+| 14 | The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse. | Entity-Destination(e1,e2) | [['(u_1 / into)'], [], 'Entity-Destination(e1,e2)'] |
+| 15 | The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.                   |                           |                                                     |
+| 16 | Gaza XXX recover from three YYY of war.                                                                                         |                           |                                                     |
+| 17 | This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.  |                           |                                                     |
+
+
+
+You can see in the dataset that the rules only matched the instances where the "into" node was present.
+
+One of the core features of our tool is that we are also able to match subgraphs. To describe a graph, we use the [PENMAN](https://github.com/goodmami/penman) notation. 
+
+E.g. the string _(u_1 / into :1 (u_3 / pour))_ would describe a graph with two nodes ("into" and "pour") and a single directed edge with the label "1" between them.
+```python
+#match a simple graph feature
+evaluator.match_features(df, [[["(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))"], [], "Entity-Destination(e1,e2)"]])
+```
+
+Describing a subgraph with the string "(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))" will return only three examples instead of 9 (when we only had a single node as a feature)
+|    | Sentence                                                                                                                        | Predicted label           | Matched rule                                                                       |
+|---:|:--------------------------------------------------------------------------------------------------------------------------------|:--------------------------|:-----------------------------------------------------------------------------------|
+|  0 | Governments and industries in nations around the world are pouring XXX into YYY.                                                | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+|  1 | The scientists poured XXX into pint YYY.                                                                                        | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+|  2 | The suspect pushed the XXX into a deep YYY.                                                                                     |                           |                                                                                    |
+|  3 | The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.                                  |                           |                                                                                    |
+|  4 | The entity1 to buy papers is pushed into the next entity2.                                                                      |                           |                                                                                    |
+|  5 | An unnamed XXX was pushed into the YYY.                                                                                         |                           |                                                                                    |
+|  6 | Since then, numerous independent feature XXX have journeyed into YYY.                                                           |                           |                                                                                    |
+|  7 | For some reason, the XXX was blinded from his own YYY about the incommensurability of time.                                     |                           |                                                                                    |
+|  8 | Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.           |                           |                                                                                    |
+|  9 | Olympics have already poured one XXX into the YYY.                                                                              | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / pour) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+| 10 | After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.                            |                           |                                                                                    |
+| 11 | I placed the XXX in a natural YYY, at the base of a part of the fallen arch.                                                    |                           |                                                                                    |
+| 12 | The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.            |                           |                                                                                    |
+| 13 | The XXX leaked from every conceivable YYY.                                                                                      |                           |                                                                                    |
+| 14 | The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse. |                           |                                                                                    |
+| 15 | The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.                   |                           |                                                                                    |
+| 16 | Gaza XXX recover from three YYY of war.                                                                                         |                           |                                                                                    |
+| 17 | This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.  |                           |                                                                                    |
+
+
+We can also add negated features that we don't want to match (e.g. this won't match the first row where 'pour' is present):
+```python
+#match a simple graph feature
+evaluator.match_features(df, [[["(u_1 / into :2 (u_3 / YYY))"], ["(u_2 / pour)"], "Entity-Destination(e1,e2)"]])
+```
+
+|    | Sentence                                                                                                                        | Predicted label           | Matched rule                                                                     |
+|---:|:--------------------------------------------------------------------------------------------------------------------------------|:--------------------------|:---------------------------------------------------------------------------------|
+|  0 | Governments and industries in nations around the world are pouring XXX into YYY.                                                |                           |                                                                                  |
+|  1 | The scientists poured XXX into pint YYY.                                                                                        |                           |                                                                                  |
+|  2 | The suspect pushed the XXX into a deep YYY.                                                                                     | Entity-Destination(e1,e2) | [['(u_1 / into :2 (u_3 / YYY))'], ['(u_2 / pour)'], 'Entity-Destination(e1,e2)'] |
+|  3 | The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.                                  | Entity-Destination(e1,e2) | [['(u_1 / into :2 (u_3 / YYY))'], ['(u_2 / pour)'], 'Entity-Destination(e1,e2)'] |
+|  4 | The entity1 to buy papers is pushed into the next entity2.                                                                      |                           |                                                                                  |
+|  5 | An unnamed XXX was pushed into the YYY.                                                                                         | Entity-Destination(e1,e2) | [['(u_1 / into :2 (u_3 / YYY))'], ['(u_2 / pour)'], 'Entity-Destination(e1,e2)'] |
+|  6 | Since then, numerous independent feature XXX have journeyed into YYY.                                                           | Entity-Destination(e1,e2) | [['(u_1 / into :2 (u_3 / YYY))'], ['(u_2 / pour)'], 'Entity-Destination(e1,e2)'] |
+|  7 | For some reason, the XXX was blinded from his own YYY about the incommensurability of time.                                     |                           |                                                                                  |
+|  8 | Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.           |                           |                                                                                  |
+|  9 | Olympics have already poured one XXX into the YYY.                                                                              |                           |                                                                                  |
+| 10 | After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.                            |                           |                                                                                  |
+| 11 | I placed the XXX in a natural YYY, at the base of a part of the fallen arch.                                                    |                           |                                                                                  |
+| 12 | The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.            |                           |                                                                                  |
+| 13 | The XXX leaked from every conceivable YYY.                                                                                      |                           |                                                                                  |
+| 14 | The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse. |                           |                                                                                  |
+| 15 | The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.                   |                           |                                                                                  |
+| 16 | Gaza XXX recover from three YYY of war.                                                                                         |                           |                                                                                  |
+| 17 | This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.  |                           |                                                                                  |
+
+If we don't want to specify nodes, regex can also be used in place of the node and edge-names:
+
+```python
+#regex can be used to match any node (this will match instances where 'into' is connected to any node with '1' edge)
+evaluator.match_features(df, [[["(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))"], [], "Entity-Destination(e1,e2)"]])
+```
+
+|    | Sentence                                                                                                                        | Predicted label           | Matched rule                                                                     |
+|---:|:--------------------------------------------------------------------------------------------------------------------------------|:--------------------------|:---------------------------------------------------------------------------------|
+|  0 | Governments and industries in nations around the world are pouring XXX into YYY.                                                | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+|  1 | The scientists poured XXX into pint YYY.                                                                                        | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+|  2 | The suspect pushed the XXX into a deep YYY.                                                                                     | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+|  3 | The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.                                  | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+|  4 | The entity1 to buy papers is pushed into the next entity2.                                                                      |                           |                                                                                  |
+|  5 | An unnamed XXX was pushed into the YYY.                                                                                         | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+|  6 | Since then, numerous independent feature XXX have journeyed into YYY.                                                           | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+|  7 | For some reason, the XXX was blinded from his own YYY about the incommensurability of time.                                     |                           |                                                                                  |
+|  8 | Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.           |                           |                                                                                  |
+|  9 | Olympics have already poured one XXX into the YYY.                                                                              | Entity-Destination(e1,e2) | [['(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))'], [], 'Entity-Destination(e1,e2)'] |
+| 10 | After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.                            |                           |                                                                                  |
+| 11 | I placed the XXX in a natural YYY, at the base of a part of the fallen arch.                                                    |                           |                                                                                  |
+| 12 | The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.            |                           |                                                                                  |
+| 13 | The XXX leaked from every conceivable YYY.                                                                                      |                           |                                                                                  |
+| 14 | The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse. |                           |                                                                                  |
+| 15 | The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.                   |                           |                                                                                  |
+| 16 | Gaza XXX recover from three YYY of war.                                                                                         |                           |                                                                                  |
+| 17 | This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.  |                           |                                                                                  |
+
+We can also train regex rules from a training data, this will automatically replace regex '.*' with nodes that are 
+'good enough' statistically based on the provided dataframe.
+
+```python
+evaluator.train_feature("Entity-Destination(e1,e2)", "(u_1 / into :1 (u_2 / .*) :2 (u_3 / YYY))", df)
+```
+
+This returns '(u_1 / into :1 (u_2 / push|pour) :2 (u_3 / YYY))' (replaced '.*' with _push_ and _pour_)
+
+### Learning rules
+
+To extract rules automatically, train the dataset with graph features and rank them based on relevancy:
+
+```python
+df = dataset.to_dataframe()
+trainer = GraphTrainer(df)
+#extract features
+features = trainer.prepare_and_train()
+
+from xpotato.dataset.utils import save_dataframe
+from sklearn.model_selection import train_test_split
+
+train, val = train_test_split(df, test_size=0.2, random_state=1234)
+
+#save train and validation, this is important for the frontend to work
+save_dataframe(train, 'train.tsv')
+save_dataframe(val, 'val.tsv')
+
+import json
+
+#also save the ranked features
+with open("features.json", "w+") as f:
+    json.dump(features, f)
+
+```
+
+You can also save the parsed graphs for evaluation or for caching:
+
+```python
+import pickle
+with open("graphs.pickle", "wb") as f:
+    pickle.dump(val.graph, f)
+```
+
+## Frontend
+
+If the DataFrame is ready with the parsed graphs, the UI can be started to inspect the extracted rules and modify them. The frontend is a streamlit app, the simplest way of starting it is (the training and the validation dataset must be provided):
+
+```
+streamlit run frontend/app.py -- -t notebooks/train.tsv -v notebooks/val.tsv -g ud
+```
+
+it can be also started with the extracted features:
+
+```
+streamlit run frontend/app.py -- -t notebooks/train.tsv -v notebooks/val.tsv -g ud -sr notebooks/features.json
+```
+
+if you already used the UI and extracted the features manually and you want to load it, you can run:
+```
+streamlit run frontend/app.py -- -t notebooks/train.tsv -v notebooks/val.tsv -g ud -sr notebooks/features.json -hr notebooks/manual_features.json
+```
+
+### Advanced mode
+
+If labels are not or just partially provided, the frontend can be started also in _advanced_ mode, where the user can _annotate_ a few examples at the start, then the system gradually offers rules based on the provided examples. 
+
+
+Dataset without labels can be initialized with:
+```python
+sentences = [("Governments and industries in nations around the world are pouring XXX into YYY.", ""),
+            ("The scientists poured XXX into pint YYY.", ""),
+            ("The suspect pushed the XXX into a deep YYY.", ""),
+            ("The Nepalese government sets up a XXX to inquire into the alleged YYY of diplomatic passports.", ""),
+            ("The entity1 to buy papers is pushed into the next entity2.", ""),
+            ("An unnamed XXX was pushed into the YYY.", ""),
+            ("Since then, numerous independent feature XXX have journeyed into YYY.", ""),
+            ("For some reason, the XXX was blinded from his own YYY about the incommensurability of time.", ""),
+            ("Sparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week.", ""),
+            ("Olympics have already poured one XXX into the YYY.", ""),
+            ("After wrapping him in a light blanket, they placed the XXX in the YYY his father had carved for him.", ""),
+            ("I placed the XXX in a natural YYY, at the base of a part of the fallen arch.", ""),
+            ("The XXX was delivered from the YYY of Lincoln Memorial on August 28, 1963 as part of his famous March on Washington.", ""),
+            ("The XXX leaked from every conceivable YYY.", ""),
+            ("The scientists placed the XXX in a tiny YYY which gets channelled into cancer cells, and is then unpacked with a laser impulse.", ""),
+            ("The level surface closest to the MSS, known as the XXX, departs from an YYY by about 100 m in each direction.", ""),
+            ("Gaza XXX recover from three YYY of war.", ""),
+            ("This latest XXX from the animation YYY at Pixar is beautiful, masterly, inspired - and delivers a powerful ecological message.", "")]
+```
+
+
+Then, the frontend can be started:
+```
+streamlit run frontend/app.py -- -t notebooks/unsupervised_dataset.tsv -g ud -m advanced
+```
+
+Once the frontend starts up and you define the labels, you are faced with the annotation interface. You can search elements by clicking on the appropriate column name and applying the desired filter. You can annotate instances by checking the checkbox at the beginning of the line. You can check multiple checkboxs at a time. Once you've selected the utterances you want to annotate, click on the _Annotate_ button. The annotated samples will appear in the lower table. You can clear the annotation of certain elements by selecting them in the second table and clicking _Clear annotation_.
+
+Once you have some annotated data, you can train rules by clicking the _Train!_ button. It is recommended to set the _Rank features based on accuracy_ to True, if you have just a few samples. You will get a similar interface as in supervised mode, you can generate rule suggestions, and write your own rules as usual. Once you are satisfied with the rules, select each of them and click _annotate based on selected_. This process might take a while if you are working with large data. You should get all the rule matches marked in the first and the second tables. You can order the tables by each column, so it's easier to check. You will have to manually accept the annotations generated this way for them to appear in the second table.
+
+- You can read about the use of the advanced mode in the [docs](https://github.com/adaamko/POTATO/tree/main/docs/README_advanced_mode.md)
+
+
+## Evaluate
+If you have the features ready and you want to evaluate them on a test set, you can run:
+
+```python
+python scripts/evaluate.py -t ud -f notebooks/features.json -d notebooks/val.tsv
+```
+
+The result will be a _csv_ file with the labels and the matched rules.
+
+## Service
+If you are ready with the extracted features and want to use our package in production for inference (generating predictions for sentences), we also provide a REST API built on POTATO (based on [fastapi](https://github.com/tiangolo/fastapi)).
+
+First install FastAPI and [Uvicorn](https://www.uvicorn.org/)
+```bash
+pip install fastapi
+pip install "uvicorn[standard]"
+```
+
+To start the service, you should set _language_, _graph\_type_ and the _features_  for the service. This can be done through enviroment variables.
+
+Example:
+```bash
+export FEATURE_PATH=/home/adaamko/projects/POTATO/features/semeval/test_features.json
+export GRAPH_FORMAT=ud
+export LANG=en
+```
+
+Then, start the REST API:
+```python
+python services/main.py
+```
+
+It will start a service running on _localhost_ on port _8000_ (it will also initialize the correct models).
+
+Then you can use any client to make post requests:
+```bash
+curl -X POST localhost:8000 -H 'Content-Type: application/json' -d '{"text":"The suspect pushed the XXX into a deep YYY.\nSparky Anderson is making progress in his XXX from YYY and could return to managing the Detroit Tigers within a week."}'
+```
+
+The answer will be a list with the predicted labels (if none of the rules match, it will return "NONE"):
+```bash
+["Entity-Destination(e1,e2)","NONE"]
+```
+
+The streamlit frontend also has an inference mode, where the implemented rule-system can be used for inference. It can be started with:
+
+```bash
+streamlit run frontend/app.py -- -hr features/semeval/test_features.json -m inference
+```
+
+## Contributing
+
+We welcome all contributions! Please fork this repository and create a branch for your modifications. We suggest getting in touch with us first, by opening an issue or by writing an email to Adam Kovacs or Gabor Recski at firstname.lastname@tuwien.ac.at
+
+## Citing
+
+If you use the library, please cite our [paper](https://dl.acm.org/doi/abs/10.1145/3511808.3557196) published in CIKM 2022:
+
+```bib
+@inproceedings{Kovacs:2022,
+author = {Kov\'{a}cs, \'{A}d\'{a}m and G\'{e}mes, Kinga and Ikl\'{o}di, Eszter and Recski, G\'{a}bor},
+title = {POTATO: ExPlainable InfOrmation ExTrAcTion FramewOrk},
+year = {2022},
+isbn = {9781450392365},
+publisher = {Association for Computing Machinery},
+address = {New York, NY, USA},
+url = {https://doi.org/10.1145/3511808.3557196},
+doi = {10.1145/3511808.3557196},
+booktitle = {Proceedings of the 31st ACM International Conference on Information & Knowledge Management},
+pages = {4897–4901},
+numpages = {5},
+keywords = {explainability, explainable, hitl},
+location = {Atlanta, GA, USA},
+series = {CIKM '22}
+}
+```
+
+## License 
+
+MIT license
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

