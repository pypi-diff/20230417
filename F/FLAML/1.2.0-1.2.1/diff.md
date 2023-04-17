# Comparing `tmp/FLAML-1.2.0.tar.gz` & `tmp/FLAML-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLAML-1.2.0.tar", last modified: Sat Apr  8 18:29:51 2023, max compression
+gzip compressed data, was "FLAML-1.2.1.tar", last modified: Mon Apr 17 17:43:38 2023, max compression
```

## Comparing `FLAML-1.2.0.tar` & `FLAML-1.2.1.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.755425 FLAML-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.743425 FLAML-1.2.0/FLAML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-04-08 18:29:51.000000 FLAML-1.2.0/FLAML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-08 18:29:51.000000 FLAML-1.2.0/FLAML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:29:51.000000 FLAML-1.2.0/FLAML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-08 18:29:51.000000 FLAML-1.2.0/FLAML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 18:29:51.000000 FLAML-1.2.0/FLAML.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-08 18:28:47.000000 FLAML-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-04-08 18:28:47.000000 FLAML-1.2.0/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-04-08 18:29:51.755425 FLAML-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-04-08 18:28:47.000000 FLAML-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.747425 FLAML-1.2.0/flaml/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.747425 FLAML-1.2.0/flaml/autogen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/autogen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/autogen/code_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/autogen/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.747425 FLAML-1.2.0/flaml/autogen/oai/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/autogen/oai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37455 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/autogen/oai/completion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.747425 FLAML-1.2.0/flaml/automl/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   132360 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/automl.py
--rw-r--r--   0 runner    (1001) docker     (123)    18770 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23603 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)   107198 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.747425 FLAML-1.2.0/flaml/automl/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.747425 FLAML-1.2.0/flaml/automl/nlp/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/nlp/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/nlp/huggingface/data_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/nlp/huggingface/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/nlp/huggingface/training_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    16867 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/nlp/huggingface/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/nlp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.747425 FLAML-1.2.0/flaml/automl/spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/spark/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/spark/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10334 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/spark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17491 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/automl/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/task/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    46906 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/task/generic_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/training_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/automl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/default/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/default/all/
--rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/all/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/all/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/all/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/default/extra_tree/
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/extra_tree/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/extra_tree/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/extra_tree/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/greedy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/default/lgbm/
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/lgbm/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/lgbm/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/lgbm/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/regret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/default/rf/
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/rf/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/rf/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/rf/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/suggest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/default/xgb_limitdepth/
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/xgb_limitdepth/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/xgb_limitdepth/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/xgb_limitdepth/regression.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/default/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/xgboost/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/xgboost/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/default/xgboost/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.751425 FLAML-1.2.0/flaml/onlineml/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/onlineml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/onlineml/autovw.py
--rw-r--r--   0 runner    (1001) docker     (123)    16943 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/onlineml/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    25274 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/onlineml/trial_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.755425 FLAML-1.2.0/flaml/tune/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    22600 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.755425 FLAML-1.2.0/flaml/tune/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/scheduler/online_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/scheduler/trial_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.755425 FLAML-1.2.0/flaml/tune/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/searcher/blendsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/searcher/cfo_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)    32116 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/searcher/flow2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18779 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/searcher/online_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/searcher/search_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    32267 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/searcher/suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/searcher/variant_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.755425 FLAML-1.2.0/flaml/tune/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/spark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/trial_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    38230 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/tune.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/tune/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-08 18:28:47.000000 FLAML-1.2.0/flaml/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 18:29:51.755425 FLAML-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-08 18:28:47.000000 FLAML-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:51.755425 FLAML-1.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    15518 2023-04-08 18:28:47.000000 FLAML-1.2.0/test/test_autovw.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-08 18:28:47.000000 FLAML-1.2.0/test/test_conda_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-08 18:28:47.000000 FLAML-1.2.0/test/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-08 18:28:47.000000 FLAML-1.2.0/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-08 18:28:47.000000 FLAML-1.2.0/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.746997 FLAML-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.734997 FLAML-1.2.1/FLAML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-04-17 17:43:38.000000 FLAML-1.2.1/FLAML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-17 17:43:38.000000 FLAML-1.2.1/FLAML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:43:38.000000 FLAML-1.2.1/FLAML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-17 17:43:38.000000 FLAML-1.2.1/FLAML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 17:43:38.000000 FLAML-1.2.1/FLAML.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-17 17:42:30.000000 FLAML-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-04-17 17:42:30.000000 FLAML-1.2.1/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-04-17 17:43:38.746997 FLAML-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-04-17 17:42:30.000000 FLAML-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.734997 FLAML-1.2.1/flaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.734997 FLAML-1.2.1/flaml/autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/autogen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/autogen/code_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/autogen/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.734997 FLAML-1.2.1/flaml/autogen/oai/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/autogen/oai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37202 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/autogen/oai/completion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129453 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23042 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105105 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/automl/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/automl/nlp/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/nlp/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/nlp/huggingface/data_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/nlp/huggingface/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/nlp/huggingface/training_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16457 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/nlp/huggingface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/nlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/automl/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/spark/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/spark/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/spark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/automl/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/task/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44736 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/task/generic_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/training_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/automl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/default/all/
+-rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/all/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/all/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/all/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/default/extra_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/extra_tree/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/extra_tree/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/extra_tree/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/greedy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/default/lgbm/
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/lgbm/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/lgbm/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/lgbm/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/regret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.738997 FLAML-1.2.1/flaml/default/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/rf/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/rf/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/rf/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/suggest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.742997 FLAML-1.2.1/flaml/default/xgb_limitdepth/
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/xgb_limitdepth/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/xgb_limitdepth/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/xgb_limitdepth/regression.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.742997 FLAML-1.2.1/flaml/default/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/xgboost/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/xgboost/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/default/xgboost/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.742997 FLAML-1.2.1/flaml/onlineml/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/onlineml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/onlineml/autovw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/onlineml/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/onlineml/trial_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.742997 FLAML-1.2.1/flaml/tune/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22060 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.742997 FLAML-1.2.1/flaml/tune/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/scheduler/online_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/scheduler/trial_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.742997 FLAML-1.2.1/flaml/tune/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50302 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/searcher/blendsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/searcher/cfo_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30648 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/searcher/flow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/searcher/online_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/searcher/search_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31123 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/searcher/suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/searcher/variant_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22364 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.742997 FLAML-1.2.1/flaml/tune/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/spark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/trial_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37129 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/tune/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 17:42:30.000000 FLAML-1.2.1/flaml/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:43:38.746997 FLAML-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-17 17:42:30.000000 FLAML-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:43:38.746997 FLAML-1.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-04-17 17:42:30.000000 FLAML-1.2.1/test/test_autovw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-17 17:42:30.000000 FLAML-1.2.1/test/test_conda_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-17 17:42:30.000000 FLAML-1.2.1/test/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-17 17:42:30.000000 FLAML-1.2.1/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-17 17:42:30.000000 FLAML-1.2.1/test/test_version.py
```

### Comparing `FLAML-1.2.0/FLAML.egg-info/PKG-INFO` & `FLAML-1.2.1/FLAML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLAML
-Version: 1.2.0
+Version: 1.2.1
 Summary: A fast library for automated machine learning and tuning
 Home-page: https://github.com/microsoft/FLAML
 Author: Microsoft Corporation
 Author-email: hpo@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,15 +41,15 @@
 # A Fast Library for Automated Machine Learning & Tuning
 
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p>
 
-:fire: OpenAI GPT-3 models support in v1.1.3. ChatGPT and GPT-4 support will be added in v1.2.0.
+:fire: v1.2.0 is released with support for ChatGPT and GPT-4.
 
 :fire: A [lab forum](https://github.com/microsoft/FLAML/tree/tutorial-aaai23/tutorial) on FLAML at AAAI 2023.
 
 :fire: A [hands-on tutorial](https://github.com/microsoft/FLAML/tree/tutorial/tutorial) on FLAML presented at KDD 2022
 
 ## What is FLAML
 FLAML is a lightweight Python library that finds accurate machine
```

### Comparing `FLAML-1.2.0/FLAML.egg-info/SOURCES.txt` & `FLAML-1.2.1/FLAML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/FLAML.egg-info/requires.txt` & `FLAML-1.2.1/FLAML.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 catboost>=0.26
 rgf-python
 optuna==2.8.0
 openml==0.10.2
 statsmodels>=0.12.2
 psutil==5.8.0
 dataclasses
-transformers[torch]
+transformers[torch]==4.26
 datasets
 nltk
 rouge_score
 hcrystalball==0.1.10
 seqeval
 pytorch-forecasting<=0.10.1,>=0.9.0
 mlflow
```

### Comparing `FLAML-1.2.0/LICENSE` & `FLAML-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/NOTICE.md` & `FLAML-1.2.1/NOTICE.md`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/PKG-INFO` & `FLAML-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLAML
-Version: 1.2.0
+Version: 1.2.1
 Summary: A fast library for automated machine learning and tuning
 Home-page: https://github.com/microsoft/FLAML
 Author: Microsoft Corporation
 Author-email: hpo@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,15 +41,15 @@
 # A Fast Library for Automated Machine Learning & Tuning
 
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p>
 
-:fire: OpenAI GPT-3 models support in v1.1.3. ChatGPT and GPT-4 support will be added in v1.2.0.
+:fire: v1.2.0 is released with support for ChatGPT and GPT-4.
 
 :fire: A [lab forum](https://github.com/microsoft/FLAML/tree/tutorial-aaai23/tutorial) on FLAML at AAAI 2023.
 
 :fire: A [hands-on tutorial](https://github.com/microsoft/FLAML/tree/tutorial/tutorial) on FLAML presented at KDD 2022
 
 ## What is FLAML
 FLAML is a lightweight Python library that finds accurate machine
```

### Comparing `FLAML-1.2.0/README.md` & `FLAML-1.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # A Fast Library for Automated Machine Learning & Tuning
 
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p>
 
-:fire: OpenAI GPT-3 models support in v1.1.3. ChatGPT and GPT-4 support will be added in v1.2.0.
+:fire: v1.2.0 is released with support for ChatGPT and GPT-4.
 
 :fire: A [lab forum](https://github.com/microsoft/FLAML/tree/tutorial-aaai23/tutorial) on FLAML at AAAI 2023.
 
 :fire: A [hands-on tutorial](https://github.com/microsoft/FLAML/tree/tutorial/tutorial) on FLAML presented at KDD 2022
 
 ## What is FLAML
 FLAML is a lightweight Python library that finds accurate machine
```

### Comparing `FLAML-1.2.0/flaml/autogen/code_utils.py` & `FLAML-1.2.1/flaml/autogen/code_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,15 @@
         )
         signal.alarm(0)
     except TimeoutError:
         return 0
     return int(result.returncode == 0)
 
 
-def generate_assertions(
-    definition: str, model: Optional[str] = "gpt-3.5-turbo"
-) -> Tuple[str, float]:
+def generate_assertions(definition: str, model: Optional[str] = "gpt-3.5-turbo") -> Tuple[str, float]:
     """Generate assertions for a function.
 
     Args:
         definition (str): The function definition, including the signature and docstr.
         model (str): The model used for generation.
 
     Returns:
@@ -108,17 +106,15 @@
         assertions, gen_cost = assertions(definition)
     else:
         gen_cost = 0
     if n > 1 or test is None:
         for i in range(n):
             response = responses[i] = _remove_check(responses[i])
             code = (
-                f"{response}\n{assertions}"
-                if response.startswith("def")
-                else f"{definition}{response}\n{assertions}"
+                f"{response}\n{assertions}" if response.startswith("def") else f"{definition}{response}\n{assertions}"
             )
             succeed_assertions = execute_code(code)
             if succeed_assertions:
                 break
     else:
         # just test, no need to check assertions
         succeed_assertions = False
@@ -145,17 +141,15 @@
         "assertions": assertions,
     }
 
 
 def implement(
     definition: str,
     configs: List[Dict],
-    assertions: Optional[
-        Union[str, Callable[[str], Tuple[str, float]]]
-    ] = generate_assertions,
+    assertions: Optional[Union[str, Callable[[str], Tuple[str, float]]]] = generate_assertions,
 ) -> Tuple[str, float]:
     """Implement a function from a definition.
 
     Args:
         definition (str): The function definition, including the signature and docstr.
         configs (list): The list of configurations for completion.
         assertions (Optional, str or Callable): The assertion code which serves as a filter of the responses, or an assertion generator.
@@ -168,14 +162,12 @@
     cost = 0
     if len(configs) > 1 and callable(assertions):
         assertions, cost = assertions(definition)
     for i, config in enumerate(configs):
         response = oai.Completion.create({"definition": definition}, **config)
         cost += oai.Completion.cost(config["model"], response)
         responses = oai.Completion.extract_text(response)
-        metrics = eval_function_completions(
-            responses, definition, assertions=assertions
-        )
+        metrics = eval_function_completions(responses, definition, assertions=assertions)
         assertions = metrics["assertions"]
         cost += metrics["gen_cost"]
         if metrics["succeed_assertions"] or i == len(configs) - 1:
             return responses[metrics["index_selected"]], cost, i
```

### Comparing `FLAML-1.2.0/flaml/autogen/math_utils.py` & `FLAML-1.2.1/flaml/autogen/math_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -286,16 +286,24 @@
     Args:
         responses (list): The list of responses.
         solution (str): The canonical solution.
 
     Returns:
         dict: The success metrics.
     """
-    success_list = []
     n = len(responses)
+    if not n:
+        return {
+            "expected_success": 0,
+            "success": False,
+            "success_vote": 0,
+            "voted_answer": None,
+            "votes": 0,
+        }
+    success_list = []
     if solution is not None:
         for i in range(n):
             response = responses[i]
             succeed = is_equiv_chain_of_thought(response, solution)
             success_list.append(succeed)
     # voting
     answers = voting_counts(responses)
```

### Comparing `FLAML-1.2.0/flaml/autogen/oai/completion.py` & `FLAML-1.2.1/flaml/autogen/oai/completion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from time import sleep
 import logging
 import numpy as np
 import time
-from typing import List
+from typing import List, Optional, Dict
 import sys
 from flaml import tune, BlendSearch
 from flaml.automl.logger import logger_formatter
 
 try:
     import openai
     from openai.error import (
@@ -17,17 +17,15 @@
         APIConnectionError,
         Timeout,
     )
     import diskcache
 
     ERROR = None
 except ImportError:
-    ERROR = ImportError(
-        "please install flaml[openai] option to use the flaml.oai subpackage."
-    )
+    ERROR = ImportError("please install flaml[openai] option to use the flaml.oai subpackage.")
 logger = logging.getLogger(__name__)
 if not logger.handlers:
     # Add the console handler.
     _ch = logging.StreamHandler(stream=sys.stdout)
     _ch.setFormatter(logger_formatter)
     logger.addHandler(_ch)
 
@@ -138,83 +136,76 @@
         """
         key = get_key(config)
         if use_cache:
             response = cls._cache.get(key, None)
             if response is not None and (response != -1 or not eval_only):
                 # print("using cached response")
                 return response
-        openai_completion = (
-            openai.ChatCompletion
-            if config["model"] in cls.chat_models
-            else openai.Completion
-        )
+        openai_completion = openai.ChatCompletion if config["model"] in cls.chat_models else openai.Completion
         start_time = time.time()
+        request_timeout = cls.request_timeout
         while True:
             try:
-                response = openai_completion.create(
-                    request_timeout=cls.request_timeout, **config
-                )
+                response = openai_completion.create(request_timeout=request_timeout, **config)
                 cls._cache.set(key, response)
                 return response
             except (
                 ServiceUnavailableError,
                 APIError,
                 APIConnectionError,
             ):
                 # transient error
                 logger.warning(f"retrying in {cls.retry_time} seconds...", exc_info=1)
                 sleep(cls.retry_time)
-            except (RateLimitError, Timeout):
-                # retry after retry_time seconds
-                if time.time() - start_time + cls.retry_time < cls.retry_timeout:
+            except (RateLimitError, Timeout) as e:
+                time_left = cls.retry_timeout - (time.time() - start_time + cls.retry_time)
+                if (
+                    time_left > 0
+                    and isinstance(e, RateLimitError)
+                    or time_left > request_timeout
+                    and isinstance(e, Timeout)
+                ):
                     logger.info(f"retrying in {cls.retry_time} seconds...", exc_info=1)
                 elif eval_only:
                     raise
                 else:
                     break
+                if isinstance(e, Timeout):
+                    request_timeout <<= 1
+                request_timeout = min(request_timeout, time_left)
                 sleep(cls.retry_time)
             except InvalidRequestError:
                 if "azure" == openai.api_type and "model" in config:
                     # azure api uses "engine" instead of "model"
                     config = config.copy()
-                    config["engine"] = config.pop("model").replace(
-                        "gpt-3.5-turbo", "gpt-35-turbo"
-                    )
+                    config["engine"] = config.pop("model").replace("gpt-3.5-turbo", "gpt-35-turbo")
                 else:
                     raise
         logger.warning(
             f"Failed to get response from openai api due to getting RateLimitError or Timeout for {cls.retry_timeout} seconds."
         )
         response = -1
         cls._cache.set(key, response)
         return response
 
     @classmethod
     def _get_max_valid_n(cls, key, max_tokens):
         # find the max value in max_valid_n_per_max_tokens
         # whose key is equal or larger than max_tokens
         return max(
-            (
-                value
-                for k, value in cls._max_valid_n_per_max_tokens.get(key, {}).items()
-                if k >= max_tokens
-            ),
+            (value for k, value in cls._max_valid_n_per_max_tokens.get(key, {}).items() if k >= max_tokens),
             default=1,
         )
 
     @classmethod
     def _get_min_invalid_n(cls, key, max_tokens):
         # find the min value in min_invalid_n_per_max_tokens
         # whose key is equal or smaller than max_tokens
         return min(
-            (
-                value
-                for k, value in cls._min_invalid_n_per_max_tokens.get(key, {}).items()
-                if k <= max_tokens
-            ),
+            (value for k, value in cls._min_invalid_n_per_max_tokens.get(key, {}).items() if k <= max_tokens),
             default=None,
         )
 
     @classmethod
     def _get_region_key(cls, config):
         # get a key for the valid/invalid region corresponding to the given config
         return (
@@ -223,20 +214,18 @@
             config.get("stop"),
         )
 
     @classmethod
     def _update_invalid_n(cls, prune, region_key, max_tokens, num_completions):
         if prune:
             # update invalid n and prune this config
-            cls._min_invalid_n_per_max_tokens[
-                region_key
-            ] = invalid_n = cls._min_invalid_n_per_max_tokens.get(region_key, {})
-            invalid_n[max_tokens] = min(
-                num_completions, invalid_n.get(max_tokens, np.inf)
+            cls._min_invalid_n_per_max_tokens[region_key] = invalid_n = cls._min_invalid_n_per_max_tokens.get(
+                region_key, {}
             )
+            invalid_n[max_tokens] = min(num_completions, invalid_n.get(max_tokens, np.inf))
 
     @classmethod
     def _pop_subspace(cls, config):
         if "subspace" in config:
             config = config.copy()
             config.update(config.pop("subspace"))
         return config
@@ -276,37 +265,31 @@
         """
         cost = 0
         data = cls.data
         config = cls._pop_subspace(config)
         model = config["model"]
         data_length = len(data)
         price = cls.price1K.get(model)
-        price_input, price_output = (
-            price if isinstance(price, tuple) else (price, price)
-        )
+        price_input, price_output = price if isinstance(price, tuple) else (price, price)
         inference_budget = getattr(cls, "inference_budget", None)
         prune_hp = getattr(cls, "_prune_hp", "n")
         metric = cls._metric
         config_n = config.get(prune_hp, 1)  # default value in OpenAI is 1
-        max_tokens = config.get(
-            "max_tokens", np.inf if model in cls.chat_models else 16
-        )
+        max_tokens = config.get("max_tokens", np.inf if model in cls.chat_models else 16)
         prompt, messages = cls._get_prompt_messages_from_config(model, config)
         stop = cls._stops and cls._stops[config["stop"]]
         target_output_tokens = None
         if not cls.avg_input_tokens:
             input_tokens = [None] * data_length
         prune = prune and inference_budget and not eval_only
         if prune:
             region_key = cls._get_region_key(config)
             max_valid_n = cls._get_max_valid_n(region_key, max_tokens)
             if cls.avg_input_tokens:
-                target_output_tokens = (
-                    inference_budget * 1000 - cls.avg_input_tokens * price_input
-                ) / price_output
+                target_output_tokens = (inference_budget * 1000 - cls.avg_input_tokens * price_input) / price_output
                 # max_tokens bounds the maximum tokens
                 # so using it we can calculate a valid n according to the avg # input tokens
                 max_valid_n = max(
                     max_valid_n,
                     int(target_output_tokens // max_tokens),
                 )
             if config_n <= max_valid_n:
@@ -336,45 +319,35 @@
             params[prune_hp] = num_completions - previous_num_completions
             data_limit = 1 if prune else data_length
             prev_data_limit = 0
             data_early_stop = False  # whether data early stop happens for this n
             while True:  # data_limit <= data_length
                 # limit the number of data points to avoid rate limit
                 for i in range(prev_data_limit, data_limit):
-                    logger.debug(
-                        f"num_completions={num_completions}, data instance={i}"
-                    )
+                    logger.debug(f"num_completions={num_completions}, data instance={i}")
                     data_i = data[i]
                     params = cls._construct_params(data_i, params, prompt, messages)
                     response = cls._get_response(params, eval_only)
                     if response == -1:  # rate limit error, treat as invalid
-                        cls._update_invalid_n(
-                            prune, region_key, max_tokens, num_completions
-                        )
+                        cls._update_invalid_n(prune, region_key, max_tokens, num_completions)
                         result[metric] = 0
                         result["cost"] = cost
                         return result
                     # evaluate the quality of the responses
                     responses = cls.extract_text(response)
                     usage = response["usage"]
                     n_input_tokens = usage["prompt_tokens"]
                     n_output_tokens = usage.get("completion_tokens", 0)
                     if not cls.avg_input_tokens and not input_tokens[i]:
                         # store the # input tokens
                         input_tokens[i] = n_input_tokens
-                    query_cost = (
-                        price_input * n_input_tokens + price_output * n_output_tokens
-                    ) / 1000
+                    query_cost = (price_input * n_input_tokens + price_output * n_output_tokens) / 1000
                     cls._total_cost += query_cost
                     cost += query_cost
-                    if (
-                        cls.optimization_budget
-                        and cls._total_cost >= cls.optimization_budget
-                        and not eval_only
-                    ):
+                    if cls.optimization_budget and cls._total_cost >= cls.optimization_budget and not eval_only:
                         # limit the total tuning cost
                         return {
                             metric: 0,
                             "total_cost": cls._total_cost,
                             "cost": cost,
                         }
                     if previous_num_completions:
@@ -389,43 +362,31 @@
                 rho = (
                     (1 - data_limit / data_length) * (1 + 1 / data_limit)
                     if data_limit << 1 > data_length
                     else (1 - (data_limit - 1) / data_length)
                 )
                 # Hoeffding-Serfling bound
                 ratio = 0.1 * np.sqrt(rho / data_limit)
-                if (
-                    target_output_tokens
-                    and avg_n_tokens > target_output_tokens * (1 + ratio)
-                    and not eval_only
-                ):
-                    cls._update_invalid_n(
-                        prune, region_key, max_tokens, num_completions
-                    )
+                if target_output_tokens and avg_n_tokens > target_output_tokens * (1 + ratio) and not eval_only:
+                    cls._update_invalid_n(prune, region_key, max_tokens, num_completions)
                     result[metric] = 0
                     result["total_cost"] = cls._total_cost
                     result["cost"] = cost
                     return result
                 if (
                     prune
                     and target_output_tokens
                     and avg_n_tokens <= target_output_tokens * (1 - ratio)
-                    and (
-                        num_completions < config_n
-                        or num_completions == config_n
-                        and data_limit == data_length
-                    )
+                    and (num_completions < config_n or num_completions == config_n and data_limit == data_length)
                 ):
                     # update valid n
-                    cls._max_valid_n_per_max_tokens[
-                        region_key
-                    ] = valid_n = cls._max_valid_n_per_max_tokens.get(region_key, {})
-                    valid_n[max_tokens] = max(
-                        num_completions, valid_n.get(max_tokens, 0)
+                    cls._max_valid_n_per_max_tokens[region_key] = valid_n = cls._max_valid_n_per_max_tokens.get(
+                        region_key, {}
                     )
+                    valid_n[max_tokens] = max(num_completions, valid_n.get(max_tokens, 0))
                     if num_completions < config_n:
                         # valid already, skip the rest of the data
                         data_limit = data_length
                         data_early_stop = True
                         break
                 prev_data_limit = data_limit
                 if data_limit < data_length:
@@ -451,17 +412,15 @@
                 result["cost"] = cost
                 if not cls.avg_input_tokens:
                     cls.avg_input_tokens = np.mean(input_tokens)
                     if prune:
                         target_output_tokens = (
                             inference_budget * 1000 - cls.avg_input_tokens * price_input
                         ) / price_output
-                result["inference_cost"] = (
-                    avg_n_tokens * price_output + cls.avg_input_tokens * price_input
-                ) / 1000
+                result["inference_cost"] = (avg_n_tokens * price_output + cls.avg_input_tokens * price_input) / 1000
                 break
             else:
                 if data_early_stop:
                     previous_num_completions = 0
                     n_tokens_list.clear()
                     responses_list.clear()
                 else:
@@ -518,22 +477,22 @@
                 -1 means no hard restriction in the number of trials
                 and the actual number is decided by optimization_budget. Defaults to 1.
             logging_level (optional): logging level. Defaults to logging.WARNING.
             **config (dict): The search space to update over the default search.
                 For prompt, please provide a string/Callable or a list of strings/Callables.
                     - If prompt is provided for chat models, it will be converted to messages under role "user".
                     - Do not provide both prompt and messages for chat models, but provide either of them.
-                    - A string `prompt` template will be used to generate a prompt for each data instance
+                    - A string template will be used to generate a prompt for each data instance
                       using `prompt.format(**data)`.
-                    - A callable `prompt` template will be used to generate a prompt for each data instance
+                    - A callable template will be used to generate a prompt for each data instance
                       using `prompt(data)`.
                 For stop, please provide a string, a list of strings, or a list of lists of strings.
                 For messages (chat models only), please provide a list of messages (for a single chat prefix)
                 or a list of lists of messages (for multiple choices of chat prefix to choose from).
-                Each message should be a dict with keys "role" and "content".
+                Each message should be a dict with keys "role" and "content". The value of "content" can be a string/Callable template.
 
         Returns:
             dict: The optimized hyperparameter setting.
             tune.ExperimentAnalysis: The tuning results.
         """
         if ERROR:
             raise ERROR
@@ -548,37 +507,31 @@
                 space["temperature_or_top_p"] = {"temperature": temperature}
             elif temperature is None and top_p is not None:
                 space["temperature_or_top_p"] = {"top_p": top_p}
             elif temperature is not None and top_p is not None:
                 space.pop("temperature_or_top_p")
                 space["temperature"] = temperature
                 space["top_p"] = top_p
-                logger.warning(
-                    "temperature and top_p are not recommended to vary together."
-                )
+                logger.warning("temperature and top_p are not recommended to vary together.")
         cls._max_valid_n_per_max_tokens, cls._min_invalid_n_per_max_tokens = {}, {}
         cls.optimization_budget = optimization_budget
         cls.inference_budget = inference_budget
         cls._prune_hp = "best_of" if space.get("best_of", 1) != 1 else "n"
         cls._prompts = space.get("prompt")
         if cls._prompts is None:
             cls._messages = space.get("messages")
             assert isinstance(cls._messages, list) and isinstance(
                 cls._messages[0], (dict, list)
             ), "messages must be a list of dicts or a list of lists."
             if isinstance(cls._messages[0], dict):
                 cls._messages = [cls._messages]
             space["messages"] = tune.choice(list(range(len(cls._messages))))
         else:
-            assert (
-                space.get("messages") is None
-            ), "messages and prompt cannot be provided at the same time."
-            assert isinstance(
-                cls._prompts, (str, list)
-            ), "prompt must be a string or a list of strings."
+            assert space.get("messages") is None, "messages and prompt cannot be provided at the same time."
+            assert isinstance(cls._prompts, (str, list)), "prompt must be a string or a list of strings."
             if isinstance(cls._prompts, str):
                 cls._prompts = [cls._prompts]
             space["prompt"] = tune.choice(list(range(len(cls._prompts))))
         cls._stops = space.get("stop")
         if cls._stops:
             assert isinstance(
                 cls._stops, (str, list)
@@ -662,25 +615,29 @@
         temperature_or_top_p = params.pop("temperature_or_top_p", None)
         if temperature_or_top_p:
             params.update(temperature_or_top_p)
         logger.setLevel(old_level)
         return params, analysis
 
     @classmethod
-    def create(cls, context, use_cache=True, **config):
+    def create(cls, context: Optional[Dict] = None, use_cache: Optional[bool] = True, **config):
         """Make a completion for a given context.
 
         Args:
-            context (dict): The context to instantiate the prompt.
+            context (dict, Optional): The context to instantiate the prompt.
                 It needs to contain keys that are used by the prompt template.
                 E.g., `prompt="Complete the following sentence: {prefix}"`.
                 `context={"prefix": "Today I feel"}`.
                 The actual prompt sent to OpenAI will be:
                 "Complete the following sentence: Today I feel".
             use_cache (bool, Optional): Whether to use cached responses.
+            **config: Configuration for the completion.
+                Besides the parameters for the openai API call, it can also contain a seed (int) for the cache.
+                This is useful when implementing "controlled randomness" for the completion.
+                Also, the "prompt" or "messages" parameter can contain a template (str or Callable) which will be instantiated with the context.
 
         Returns:
             Responses from OpenAI API.
         """
         if ERROR:
             raise ERROR
         params = cls._construct_params(context, config)
@@ -690,57 +647,55 @@
         if "seed" in params:
             cls.set_cache(params.pop("seed"))
         with diskcache.Cache(cls.cache_path) as cls._cache:
             cls.set_cache(seed)
             return cls._get_response(params, eval_only=True)
 
     @classmethod
+    def _instantiate(cls, template: str, context: Optional[Dict] = None):
+        if not context:
+            return template
+        if isinstance(template, str):
+            return template.format(**context)
+        return template(context)
+
+    @classmethod
     def _construct_params(cls, data_instance, config, prompt=None, messages=None):
         params = config.copy()
         model = config["model"]
         prompt = config.get("prompt") if prompt is None else prompt
         messages = config.get("messages") if messages is None else messages
         # either "prompt" should be in config (for being compatible with non-chat models)
         # or "messages" should be in config (for tuning chat models only)
         if prompt is None and model in cls.chat_models:
             if messages is None:
-                raise ValueError(
-                    "Either prompt or messages should be in config for chat models."
-                )
+                raise ValueError("Either prompt or messages should be in config for chat models.")
         if prompt is None:
-            params["messages"] = [
-                {
-                    "role": m["role"],
-                    "content": m["content"].format(**data_instance)
-                    if isinstance(m["content"], str)
-                    else m["content"](data_instance),
-                }
-                for m in messages
-            ]
+            params["messages"] = (
+                [
+                    {
+                        "role": m["role"],
+                        "content": cls._instantiate(m["content"], data_instance),
+                    }
+                    for m in messages
+                ]
+                if data_instance
+                else messages
+            )
         elif model in cls.chat_models:
             # convert prompt to messages
-            if isinstance(prompt, str):
-                prompt_msg = prompt.format(**data_instance)
-            else:
-                prompt_msg = prompt(data_instance)
             params["messages"] = [
                 {
                     "role": "user",
-                    "content": prompt_msg
-                    if isinstance(prompt, str)
-                    else prompt(data_instance),
+                    "content": cls._instantiate(prompt, data_instance),
                 },
             ]
             params.pop("prompt", None)
         else:
-            params["prompt"] = (
-                prompt.format(**data_instance)
-                if isinstance(prompt, str)
-                else prompt(data_instance)
-            )
+            params["prompt"] = cls._instantiate(prompt, data_instance)
         return params
 
     @classmethod
     def test(
         cls,
         data,
         config,
@@ -851,17 +806,15 @@
                 )
         elif callable(agg_method):
             for key in metric_keys:
                 result_agg[key] = agg_method([r[key] for r in result_list])
         elif isinstance(agg_method, dict):
             for key in metric_keys:
                 metric_agg_method = agg_method[key]
-                assert callable(
-                    metric_agg_method
-                ), "please provide a callable for each metric"
+                assert callable(metric_agg_method), "please provide a callable for each metric"
                 result_agg[key] = metric_agg_method([r[key] for r in result_list])
         else:
             raise ValueError(
                 "agg_method needs to be a string ('avg' or 'median'),\
                 or a callable, or a dictionary of callable."
             )
         logger.setLevel(old_level)
@@ -873,15 +826,15 @@
         if return_responses_and_per_instance_result:
             return result_agg, result_list, responses_list
         else:
             return result_agg
 
     @classmethod
     def cost(cls, model: str, response: dict):
-        """Compute the cost of a completion.
+        """Compute the cost of an API call.
 
         Args:
             model (str): The model name.
             response (dict): The response from OpenAI API.
 
         Returns:
             The cost in USD.
@@ -894,26 +847,26 @@
         price1K = cls.price1K[model]
         if isinstance(price1K, tuple):
             return (price1K[0] * n_input_tokens + price1K[1] * n_output_tokens) / 1000
         return price1K * (n_input_tokens + n_output_tokens) / 1000
 
     @classmethod
     def extract_text(cls, response: dict) -> List[str]:
-        """Extract the text from a completion response.
+        """Extract the text from a completion or chat response.
 
         Args:
             response (dict): The response from OpenAI API.
 
         Returns:
             A list of text in the responses.
         """
         choices = response["choices"]
         if "text" in choices[0]:
             return [choice["text"] for choice in choices]
-        return [choice["message"]["content"] for choice in choices]
+        return [choice["message"].get("content", "") for choice in choices]
 
 
 class ChatCompletion(Completion):
     """A class for OpenAI API ChatCompletion."""
 
     default_search_space = Completion.default_search_space.copy()
     default_search_space["model"] = tune.choice(["gpt-3.5-turbo", "gpt-4"])
```

### Comparing `FLAML-1.2.0/flaml/automl/automl.py` & `FLAML-1.2.1/flaml/automl/automl.py`

 * *Files 3% similar despite different names*

```diff
@@ -383,23 +383,19 @@
         settings["use_ray"] = settings.get("use_ray", False)
         settings["use_spark"] = settings.get("use_spark", False)
         if settings["use_ray"] is not False and settings["use_spark"] is not False:
             raise ValueError("use_ray and use_spark cannot be both True.")
         settings["free_mem_ratio"] = settings.get("free_mem_ratio", 0)
         settings["metric_constraints"] = settings.get("metric_constraints", [])
         settings["cv_score_agg_func"] = settings.get("cv_score_agg_func", None)
-        settings["fit_kwargs_by_estimator"] = settings.get(
-            "fit_kwargs_by_estimator", {}
-        )
+        settings["fit_kwargs_by_estimator"] = settings.get("fit_kwargs_by_estimator", {})
         settings["custom_hp"] = settings.get("custom_hp", {})
         settings["skip_transform"] = settings.get("skip_transform", False)
 
-        self._estimator_type = (
-            "classifier" if settings["task"] in CLASSIFICATION else "regressor"
-        )
+        self._estimator_type = "classifier" if settings["task"] in CLASSIFICATION else "regressor"
 
     def get_params(self, deep: bool = False) -> dict:
         return self._settings.copy()
 
     @property
     def config_history(self) -> dict:
         """A dictionary of iter->(estimator, config, time),
@@ -448,26 +444,22 @@
         config = state and getattr(state, "best_config", None)
         return config and AutoMLState.sanitize(config)
 
     @property
     def best_config_per_estimator(self):
         """A dictionary of all estimators' best configuration."""
         return {
-            e: e_search_state.best_config
-            and AutoMLState.sanitize(e_search_state.best_config)
+            e: e_search_state.best_config and AutoMLState.sanitize(e_search_state.best_config)
             for e, e_search_state in self._search_states.items()
         }
 
     @property
     def best_loss_per_estimator(self):
         """A dictionary of all estimators' best loss."""
-        return {
-            e: e_search_state.best_loss
-            for e, e_search_state in self._search_states.items()
-        }
+        return {e: e_search_state.best_loss for e, e_search_state in self._search_states.items()}
 
     @property
     def best_loss(self):
         """A float of the best loss found."""
         return self._state.best_loss
 
     @property
@@ -478,35 +470,41 @@
 
     @property
     def metrics_for_best_config(self):
         """Returns a float of the best loss, and a dictionary of the auxiliary metrics to log
         associated with the best config. These two objects correspond to the returned
         objects by the customized metric function for the config with the best loss."""
         state = self._search_states.get(self._best_estimator)
-        return self._state.best_loss, state and getattr(state, "best_result", {}).get(
-            "metric_for_logging"
-        )
+        return self._state.best_loss, state and getattr(state, "best_result", {}).get("metric_for_logging")
 
     @property
     def best_config_train_time(self):
         """A float of the seconds taken by training the best config."""
-        return getattr(
-            self._search_states[self._best_estimator], "best_config_train_time", None
-        )
+        return getattr(self._search_states[self._best_estimator], "best_config_train_time", None)
 
     def save_best_config(self, filename):
         best = {
             "class": self.best_estimator,
             "hyperparameters": self.best_config,
         }
         os.makedirs(os.path.dirname(filename), exist_ok=True)
         with open(filename, "w") as f:
             json.dump(best, f)
 
     @property
+    def feature_transformer(self):
+        """Returns AutoML Transformer"""
+        return getattr(self, "_transformer", None)
+
+    @property
+    def label_transformer(self):
+        """Returns AutoML label transformer"""
+        return getattr(self, "_label_transformer", None)
+
+    @property
     def classes_(self):
         """A numpy array of shape (n_classes,) for class labels."""
         attr = getattr(self, "_label_transformer", None)
         if attr:
             return attr.classes_
         attr = getattr(self, "_trained_estimator", None)
         if attr:
@@ -540,17 +538,15 @@
         self,
         X: Union[pd.DataFrame, psDataFrame],
         y: Union[pd.Series, psSeries],
         **kwargs,
     ):
         estimator = getattr(self, "_trained_estimator", None)
         if estimator is None:
-            logger.warning(
-                "No estimator is trained. Please run fit with enough budget."
-            )
+            logger.warning("No estimator is trained. Please run fit with enough budget.")
             return None
         X = self._state.task.preprocess(X, self._transformer)
         if self._label_transformer:
             y = self._label_transformer.transform(y)
         return estimator.score(X, y, **kwargs)
 
     def predict(
@@ -584,30 +580,23 @@
 
         Returns:
             A array-like of shape n * 1: each element is a predicted
             label for an instance.
         """
         estimator = getattr(self, "_trained_estimator", None)
         if estimator is None:
-            logger.warning(
-                "No estimator is trained. Please run fit with enough budget."
-            )
+            logger.warning("No estimator is trained. Please run fit with enough budget.")
             return None
         X = self._state.task.preprocess(X, self._transformer)
         y_pred = estimator.predict(X, **pred_kwargs)
-        if (
-            isinstance(y_pred, np.ndarray)
-            and y_pred.ndim > 1
-            and isinstance(y_pred, np.ndarray)
-        ):
+
+        if isinstance(y_pred, np.ndarray) and y_pred.ndim > 1 and isinstance(y_pred, np.ndarray):
             y_pred = y_pred.flatten()
         if self._label_transformer:
-            return self._label_transformer.inverse_transform(
-                pd.Series(y_pred.astype(int))
-            )
+            return self._label_transformer.inverse_transform(pd.Series(y_pred.astype(int)))
         else:
             return y_pred
 
     def predict_proba(self, X, **pred_kwargs):
         """Predict the probability of each class from features, only works for
         classification problems.
 
@@ -618,34 +607,30 @@
 
         Returns:
             A numpy array of shape n * c. c is the  # classes. Each element at
             (i, j) is the probability for instance i to be in class j.
         """
         estimator = getattr(self, "_trained_estimator", None)
         if estimator is None:
-            logger.warning(
-                "No estimator is trained. Please run fit with enough budget."
-            )
+            logger.warning("No estimator is trained. Please run fit with enough budget.")
             return None
         X = self._state.task.preprocess(X, self._transformer)
         proba = self._trained_estimator.predict_proba(X, **pred_kwargs)
         return proba
 
     def add_learner(self, learner_name, learner_class):
         """Add a customized learner.
 
         Args:
             learner_name: A string of the learner's name.
             learner_class: A subclass of flaml.model.BaseEstimator.
         """
         self._state.learner_classes[learner_name] = learner_class
 
-    def get_estimator_from_log(
-        self, log_file_name: str, record_id: int, task: Union[str, Task]
-    ):
+    def get_estimator_from_log(self, log_file_name: str, record_id: int, task: Union[str, Task]):
         """Get the estimator from log file.
 
         Args:
             log_file_name: A string of the log file name.
             record_id: An integer of the record ID in the file,
                 0 corresponds to the first trial.
             task: A string of the task type,
@@ -815,38 +800,26 @@
         if isinstance(task, str):
             task = task_factory(task)
 
         eval_method = eval_method or self._settings.get("eval_method")
         split_ratio = split_ratio or self._settings.get("split_ratio")
         n_splits = n_splits or self._settings.get("n_splits")
         split_type = split_type or self._settings.get("split_type")
-        auto_augment = (
-            self._settings.get("auto_augment") if auto_augment is None else auto_augment
-        )
+        auto_augment = self._settings.get("auto_augment") if auto_augment is None else auto_augment
         self._state.task = task
         self._estimator_type = "classifier" if task.is_classification() else "regressor"
 
         self._state.fit_kwargs = fit_kwargs
         self._state.custom_hp = custom_hp or self._settings.get("custom_hp")
-        self._skip_transform = (
-            self._settings.get("skip_transform")
-            if skip_transform is None
-            else skip_transform
-        )
-        self._state.fit_kwargs_by_estimator = (
-            fit_kwargs_by_estimator or self._settings.get("fit_kwargs_by_estimator")
-        )
+        self._skip_transform = self._settings.get("skip_transform") if skip_transform is None else skip_transform
+        self._state.fit_kwargs_by_estimator = fit_kwargs_by_estimator or self._settings.get("fit_kwargs_by_estimator")
         self.preserve_checkpoint = (
-            self._settings.get("preserve_checkpoint")
-            if preserve_checkpoint is None
-            else preserve_checkpoint
-        )
-        task.validate_data(
-            self, self._state, X_train, y_train, dataframe, label, groups=groups
+            self._settings.get("preserve_checkpoint") if preserve_checkpoint is None else preserve_checkpoint
         )
+        task.validate_data(self, self._state, X_train, y_train, dataframe, label, groups=groups)
 
         logger.info("log file name {}".format(log_file_name))
 
         best_config = None
         best_val_loss = float("+inf")
         best_estimator = None
         sample_size = None
@@ -872,17 +845,15 @@
                                 sample_size = size
                         else:
                             best = record
                             size = record.sample_size
                             best_val_loss = val_loss
                             sample_size = size
                 if not training_duration:
-                    logger.warning(
-                        f"No estimator found within time_budget={time_budget}"
-                    )
+                    logger.warning(f"No estimator found within time_budget={time_budget}")
                     from .model import BaseEstimator as Estimator
 
                     self._trained_estimator = Estimator()
                     return training_duration
         if not best:
             return
         best_estimator = best.learner
@@ -896,17 +867,15 @@
             )  # make another shallow copy of the value (a dict obj), so user's fit_kwargs_by_estimator won't be updated
             this_estimator_kwargs.update(self._state.fit_kwargs)
             self._state.fit_kwargs_by_estimator[best_estimator] = this_estimator_kwargs
         else:
             self._state.fit_kwargs_by_estimator[best_estimator] = self._state.fit_kwargs
 
         logger.info(
-            "estimator = {}, config = {}, #training instances = {}".format(
-                best_estimator, best_config, sample_size
-            )
+            "estimator = {}, config = {}, #training instances = {}".format(best_estimator, best_config, sample_size)
         )
         # Partially copied from fit() function
         # Initilize some attributes required for retrain_from_log
         self._split_type = task.decide_split_type(
             split_type,
             self._y_train_all,
             self._state.fit_kwargs,
@@ -939,17 +908,15 @@
 
     def _decide_eval_method(self, eval_method, time_budget):
         if not isinstance(self._split_type, str):
             assert eval_method in [
                 "auto",
                 "cv",
             ], "eval_method must be 'auto' or 'cv' for custom data splitter."
-            assert (
-                self._state.X_val is None
-            ), "custom splitter and custom validation data can't be used together."
+            assert self._state.X_val is None, "custom splitter and custom validation data can't be used together."
             return "cv"
         if self._state.X_val is not None:
             assert eval_method in [
                 "auto",
                 "holdout",
             ], "eval_method must be 'auto' or 'holdout' for custom validation data."
             return "holdout"
@@ -1046,18 +1013,15 @@
             return c
         else:
             configs = []
             for estimator in self.estimator_list:
                 c = self._search_states[estimator].cat_hp_cost
                 configs.append(c)
             configs.append(
-                [
-                    self._state.learner_classes.get(estimator).cost_relative2lgbm()
-                    for estimator in self.estimator_list
-                ]
+                [self._state.learner_classes.get(estimator).cost_relative2lgbm() for estimator in self.estimator_list]
             )
             config = {"ml": configs}
         return config
 
     @property
     def points_to_evaluate(self) -> dict:
         """Initial points to evaluate.
@@ -1107,17 +1071,15 @@
     def pickle(self, output_file_name):
         import pickle
 
         estimator_to_training_function = {}
         for estimator in self.estimator_list:
             search_state = self._search_states[estimator]
             if hasattr(search_state, "training_function"):
-                estimator_to_training_function[
-                    estimator
-                ] = search_state.training_function
+                estimator_to_training_function[estimator] = search_state.training_function
                 del search_state.training_function
 
         with open(output_file_name, "wb") as f:
             pickle.dump(self, f, pickle.HIGHEST_PROTOCOL)
 
     @property
     def trainable(self) -> Callable[[dict], Optional[float]]:
@@ -1572,82 +1534,52 @@
         self._estimator_type = "classifier" if task.is_classification() else "regressor"
         time_budget = time_budget or self._settings.get("time_budget")
         n_jobs = n_jobs or self._settings.get("n_jobs")
         gpu_per_trial = fit_kwargs.get("gpu_per_trial", 0)
         eval_method = eval_method or self._settings.get("eval_method")
         split_ratio = split_ratio or self._settings.get("split_ratio")
         n_splits = n_splits or self._settings.get("n_splits")
-        auto_augment = (
-            self._settings.get("auto_augment") if auto_augment is None else auto_augment
-        )
+        auto_augment = self._settings.get("auto_augment") if auto_augment is None else auto_augment
         metric = metric or self._settings.get("metric")
         estimator_list = estimator_list or self._settings.get("estimator_list")
-        log_file_name = (
-            self._settings.get("log_file_name")
-            if log_file_name is None
-            else log_file_name
-        )
+        log_file_name = self._settings.get("log_file_name") if log_file_name is None else log_file_name
         max_iter = self._settings.get("max_iter") if max_iter is None else max_iter
         sample_is_none = sample is None
         if sample_is_none:
             sample = self._settings.get("sample")
         ensemble = self._settings.get("ensemble") if ensemble is None else ensemble
         log_type = log_type or self._settings.get("log_type")
-        model_history = (
-            self._settings.get("model_history")
-            if model_history is None
-            else model_history
-        )
+        model_history = self._settings.get("model_history") if model_history is None else model_history
         log_training_metric = (
-            self._settings.get("log_training_metric")
-            if log_training_metric is None
-            else log_training_metric
+            self._settings.get("log_training_metric") if log_training_metric is None else log_training_metric
         )
         mem_thres = mem_thres or self._settings.get("mem_thres")
         pred_time_limit = pred_time_limit or self._settings.get("pred_time_limit")
         train_time_limit = train_time_limit or self._settings.get("train_time_limit")
-        self._metric_constraints = metric_constraints or self._settings.get(
-            "metric_constraints"
-        )
+        self._metric_constraints = metric_constraints or self._settings.get("metric_constraints")
         if np.isfinite(pred_time_limit):
             self._metric_constraints.append(("pred_time", "<=", pred_time_limit))
         verbose = self._settings.get("verbose") if verbose is None else verbose
-        retrain_full = (
-            self._settings.get("retrain_full") if retrain_full is None else retrain_full
-        )
+        retrain_full = self._settings.get("retrain_full") if retrain_full is None else retrain_full
         split_type = split_type or self._settings.get("split_type")
         hpo_method = hpo_method or self._settings.get("hpo_method")
         learner_selector = learner_selector or self._settings.get("learner_selector")
         no_starting_points = starting_points is None
         if no_starting_points:
             starting_points = self._settings.get("starting_points")
-        n_concurrent_trials = n_concurrent_trials or self._settings.get(
-            "n_concurrent_trials"
-        )
-        keep_search_state = (
-            self._settings.get("keep_search_state")
-            if keep_search_state is None
-            else keep_search_state
-        )
+        n_concurrent_trials = n_concurrent_trials or self._settings.get("n_concurrent_trials")
+        keep_search_state = self._settings.get("keep_search_state") if keep_search_state is None else keep_search_state
         self.preserve_checkpoint = (
-            self._settings.get("preserve_checkpoint")
-            if preserve_checkpoint is None
-            else preserve_checkpoint
-        )
-        early_stop = (
-            self._settings.get("early_stop") if early_stop is None else early_stop
-        )
-        force_cancel = (
-            self._settings.get("force_cancel") if force_cancel is None else force_cancel
+            self._settings.get("preserve_checkpoint") if preserve_checkpoint is None else preserve_checkpoint
         )
+        early_stop = self._settings.get("early_stop") if early_stop is None else early_stop
+        force_cancel = self._settings.get("force_cancel") if force_cancel is None else force_cancel
         # no search budget is provided?
         no_budget = time_budget < 0 and max_iter is None and not early_stop
-        append_log = (
-            self._settings.get("append_log") if append_log is None else append_log
-        )
+        append_log = self._settings.get("append_log") if append_log is None else append_log
         min_sample_size = min_sample_size or self._settings.get("min_sample_size")
         use_ray = self._settings.get("use_ray") if use_ray is None else use_ray
         use_spark = self._settings.get("use_spark") if use_spark is None else use_spark
         if use_spark and use_ray is not False:
             raise ValueError("use_spark and use_ray cannot be both True.")
         elif use_spark:
             spark_available, spark_error_msg = check_spark()
@@ -1693,19 +1625,15 @@
         self._use_ray = use_ray
         # use the following condition if we have an estimation of average_trial_time and average_trial_overhead
         # self._use_ray = use_ray or n_concurrent_trials > ( average_trial_time + average_trial_overhead) / (average_trial_time)
 
         if self._use_ray is not False:
             import ray
 
-            n_cpus = (
-                ray.is_initialized()
-                and ray.available_resources()["CPU"]
-                or os.cpu_count()
-            )
+            n_cpus = ray.is_initialized() and ray.available_resources()["CPU"] or os.cpu_count()
 
             self._state.resources_per_trial = (
                 # when using gpu, default cpu is 1 per job; otherwise, default cpu is n_cpus / n_concurrent_trials
                 (
                     {
                         "cpu": max(int((n_cpus - 2) / 2 / n_concurrent_trials), 1),
                         "gpu": gpu_per_trial,
@@ -1719,38 +1647,24 @@
 
             if isinstance(X_train, ray.ObjectRef):
                 X_train = ray.get(X_train)
             elif isinstance(dataframe, ray.ObjectRef):
                 dataframe = ray.get(dataframe)
         else:
             # TODO: Integrate with Spark
-            self._state.resources_per_trial = (
-                {"cpu": n_jobs} if n_jobs > 0 else {"cpu": 1}
-            )
-        self._state.free_mem_ratio = (
-            self._settings.get("free_mem_ratio")
-            if free_mem_ratio is None
-            else free_mem_ratio
-        )
+            self._state.resources_per_trial = {"cpu": n_jobs} if n_jobs > 0 else {"cpu": 1}
+        self._state.free_mem_ratio = self._settings.get("free_mem_ratio") if free_mem_ratio is None else free_mem_ratio
         self._state.task = task
         self._state.log_training_metric = log_training_metric
 
         self._state.fit_kwargs = fit_kwargs
         custom_hp = custom_hp or self._settings.get("custom_hp")
-        self._skip_transform = (
-            self._settings.get("skip_transform")
-            if skip_transform is None
-            else skip_transform
-        )
-        fit_kwargs_by_estimator = fit_kwargs_by_estimator or self._settings.get(
-            "fit_kwargs_by_estimator"
-        )
-        self._state.fit_kwargs_by_estimator = (
-            fit_kwargs_by_estimator.copy()
-        )  # shallow copy of fit_kwargs_by_estimator
+        self._skip_transform = self._settings.get("skip_transform") if skip_transform is None else skip_transform
+        fit_kwargs_by_estimator = fit_kwargs_by_estimator or self._settings.get("fit_kwargs_by_estimator")
+        self._state.fit_kwargs_by_estimator = fit_kwargs_by_estimator.copy()  # shallow copy of fit_kwargs_by_estimator
         self._state.weight_val = sample_weight_val
 
         task.validate_data(
             self,
             self._state,
             X_train,
             y_train,
@@ -1772,21 +1686,17 @@
             self._state.fit_kwargs,
             self._state.groups,
         )
         logger.info(f"Data split method: {self._split_type}")
         eval_method = self._decide_eval_method(eval_method, time_budget)
         self._state.eval_method = eval_method
         logger.info("Evaluation method: {}".format(eval_method))
-        self._state.cv_score_agg_func = cv_score_agg_func or self._settings.get(
-            "cv_score_agg_func"
-        )
+        self._state.cv_score_agg_func = cv_score_agg_func or self._settings.get("cv_score_agg_func")
 
-        self._retrain_in_budget = retrain_full == "budget" and (
-            eval_method == "holdout" and self._state.X_val is None
-        )
+        self._retrain_in_budget = retrain_full == "budget" and (eval_method == "holdout" and self._state.X_val is None)
         self._auto_augment = auto_augment
 
         _sample_size_from_starting_points = {}
         if isinstance(starting_points, dict):
             for _estimator, _point_per_estimator in starting_points.items():
                 sample_size = (
                     _point_per_estimator
@@ -1800,17 +1710,15 @@
                         [
                             config["FLAML_sample_size"]
                             for config in _point_per_estimator
                             if "FLAML_sample_size" in config
                         ]
                     )
                     if _sample_size_set:
-                        _sample_size_from_starting_points[_estimator] = min(
-                            _sample_size_set
-                        )
+                        _sample_size_from_starting_points[_estimator] = min(_sample_size_set)
                     if len(_sample_size_set) > 1:
                         logger.warning(
                             "Using the min FLAML_sample_size of all the provided starting points for estimator {}. (Provided FLAML_sample_size are: {})".format(
                                 _estimator, _sample_size_set
                             )
                         )
 
@@ -1826,30 +1734,24 @@
         if isinstance(self._min_sample_size, dict):
             self._sample = {
                 (
                     k,
                     sample
                     and not task.is_rank()
                     and eval_method != "cv"
-                    and (
-                        self._min_sample_size[k] * SAMPLE_MULTIPLY_FACTOR
-                        < self._state.data_size[0]
-                    ),
+                    and (self._min_sample_size[k] * SAMPLE_MULTIPLY_FACTOR < self._state.data_size[0]),
                 )
                 for k in self._min_sample_size.keys()
             }
         else:
             self._sample = (
                 sample
                 and not task.is_rank()
                 and eval_method != "cv"
-                and (
-                    self._min_sample_size * SAMPLE_MULTIPLY_FACTOR
-                    < self._state.data_size[0]
-                )
+                and (self._min_sample_size * SAMPLE_MULTIPLY_FACTOR < self._state.data_size[0])
             )
 
         metric = task.default_metric(metric)
         self._state.metric = metric
 
         # TODO pull this to task
         def is_to_reverse_metric(metric, task):
@@ -1869,34 +1771,29 @@
                 "micro_f1",
                 "macro_f1",
             ]:
                 return True, f"1-{metric}"
             if task.is_nlp():
                 from flaml.automl.ml import huggingface_metric_to_mode
 
-                if (
-                    metric in huggingface_metric_to_mode
-                    and huggingface_metric_to_mode[metric] == "max"
-                ):
+                if metric in huggingface_metric_to_mode and huggingface_metric_to_mode[metric] == "max":
                     return True, f"-{metric}"
             return False, None
 
         if isinstance(metric, str):
             is_reverse, reverse_metric = is_to_reverse_metric(metric, task)
             if is_reverse:
                 error_metric = reverse_metric
             else:
                 error_metric = metric
         else:
             error_metric = "customized metric"
         logger.info(f"Minimizing error metric: {error_metric}")
 
-        is_spark_dataframe = isinstance(X_train, psDataFrame) or isinstance(
-            dataframe, psDataFrame
-        )
+        is_spark_dataframe = isinstance(X_train, psDataFrame) or isinstance(dataframe, psDataFrame)
         estimator_list = task.default_estimator_list(estimator_list, is_spark_dataframe)
 
         if is_spark_dataframe and self._use_spark:
             # For spark dataframe, use_spark must be False because spark models are trained in parallel themselves
             self._use_spark = False
             logger.warning(
                 "Spark dataframes support only spark.ml type models, which will be trained "
@@ -1949,17 +1846,15 @@
                         self._state.task,
                         self._X_train_all,
                         self._y_train_all,
                         estimator_name,
                         location,
                         k=1,
                     )
-                    starting_points[estimator_name] = [
-                        x["hyperparameters"] for x in configs
-                    ]
+                    starting_points[estimator_name] = [x["hyperparameters"] for x in configs]
                 except FileNotFoundError:
                     pass
             try:
                 learner = suggest_learner(
                     self._state.task,
                     self._X_train_all,
                     self._y_train_all,
@@ -1973,43 +1868,37 @@
                 pass
 
         self._state.time_budget = time_budget
         starting_points = {} if starting_points == "static" else starting_points
         for estimator_name in estimator_list:
             estimator_class = self._state.learner_classes[estimator_name]
             estimator_class.init()
-            this_estimator_kwargs = self._state.fit_kwargs_by_estimator.get(
-                estimator_name
-            )
+            this_estimator_kwargs = self._state.fit_kwargs_by_estimator.get(estimator_name)
             if this_estimator_kwargs:
                 # make another shallow copy of the value (a dict obj), so user's fit_kwargs_by_estimator won't be updated
                 this_estimator_kwargs = this_estimator_kwargs.copy()
                 this_estimator_kwargs.update(
                     self._state.fit_kwargs
                 )  # update the shallow copy of fit_kwargs to fit_kwargs_by_estimator
                 self._state.fit_kwargs_by_estimator[
                     estimator_name
                 ] = this_estimator_kwargs  # set self._state.fit_kwargs_by_estimator[estimator_name] to the update, so only self._state.fit_kwargs_by_estimator will be updated
             else:
-                self._state.fit_kwargs_by_estimator[
-                    estimator_name
-                ] = self._state.fit_kwargs
+                self._state.fit_kwargs_by_estimator[estimator_name] = self._state.fit_kwargs
 
             self._search_states[estimator_name] = SearchState(
                 learner_class=estimator_class,
                 data_size=self._state.data_size,
                 task=self._state.task,
                 starting_point=starting_points.get(estimator_name),
                 period=self._state.fit_kwargs.get(
                     "period"
                 ),  # NOTE: this is after kwargs is updated to fit_kwargs_by_estimator
                 custom_hp=custom_hp and custom_hp.get(estimator_name),
-                max_iter=max_iter / len(estimator_list)
-                if self._learner_selector == "roundrobin"
-                else max_iter,
+                max_iter=max_iter / len(estimator_list) if self._learner_selector == "roundrobin" else max_iter,
                 budget=self._state.time_budget,
             )
         logger.info("List of ML learners in AutoML Run: {}".format(estimator_list))
         self.estimator_list = estimator_list
         self._active_estimators = estimator_list.copy()
         self._ensemble = ensemble
         self._max_iter = max_iter
@@ -2035,17 +1924,15 @@
                 self._training_log = save_helper
                 self._search()
         else:
             self._training_log = None
             self._search()
         if self._best_estimator:
             logger.info("fit succeeded")
-            logger.info(
-                f"Time taken to find the best model: {self._time_taken_best_iter}"
-            )
+            logger.info(f"Time taken to find the best model: {self._time_taken_best_iter}")
             if (
                 self._hpo_method in ("cfo", "bs")
                 and self._state.time_budget > 0
                 and (self._time_taken_best_iter >= self._state.time_budget * 0.7)
                 and not all(
                     state.search_alg and state.search_alg.searcher.is_ls_ever_converged
                     for state in self._search_states.values()
@@ -2080,18 +1967,15 @@
                 assert ray_version >= "1.10.0"
                 if ray_version.startswith("1."):
                     from ray.tune.suggest import ConcurrencyLimiter
                 else:
                     from ray.tune.search import ConcurrencyLimiter
                 import ray
             except (ImportError, AssertionError):
-                raise ImportError(
-                    "use_ray=True requires installation of ray. "
-                    "Please run pip install flaml[ray]"
-                )
+                raise ImportError("use_ray=True requires installation of ray. " "Please run pip install flaml[ray]")
         else:
             from flaml.tune.searcher.suggestion import ConcurrencyLimiter
 
         if self._hpo_method in ("cfo", "grid"):
             from flaml import CFO as SearchAlgo
         elif "bs" == self._hpo_method:
             from flaml import BlendSearch as SearchAlgo
@@ -2111,24 +1995,19 @@
                     from flaml.tune.searcher.suggestion import (
                         OptunaSearch as SearchAlgo,
                     )
             else:
                 from flaml.tune.searcher.suggestion import OptunaSearch as SearchAlgo
         else:
             raise NotImplementedError(
-                f"hpo_method={self._hpo_method} is not recognized. "
-                "'auto', 'cfo' and 'bs' are supported."
+                f"hpo_method={self._hpo_method} is not recognized. " "'auto', 'cfo' and 'bs' are supported."
             )
         space = self.search_space
         self._state.time_from_start = time.time() - self._start_time_flag
-        time_budget_s = (
-            self._state.time_budget - self._state.time_from_start
-            if self._state.time_budget >= 0
-            else None
-        )
+        time_budget_s = self._state.time_budget - self._state.time_from_start if self._state.time_budget >= 0 else None
         if self._hpo_method != "optuna":
             min_resource = self.min_resource
             if isinstance(min_resource, dict):
                 _min_resource_set = set(min_resource.values())
                 min_resource_all_estimator = min(_min_resource_set)
                 if len(_min_resource_set) > 1:
                     logger.warning(
@@ -2141,17 +2020,15 @@
                 space=space,
                 low_cost_partial_config=self.low_cost_partial_config,
                 points_to_evaluate=self.points_to_evaluate,
                 cat_hp_cost=self.cat_hp_cost,
                 resource_attr=self.resource_attr,
                 min_resource=min_resource_all_estimator,
                 max_resource=self.max_resource,
-                config_constraints=[
-                    (partial(size, self._state.learner_classes), "<=", self._mem_thres)
-                ],
+                config_constraints=[(partial(size, self._state.learner_classes), "<=", self._mem_thres)],
                 metric_constraints=self.metric_constraints,
                 seed=self._seed,
                 time_budget_s=time_budget_s,
                 num_samples=self._max_iter,
                 allow_empty_config=True,
             )
         else:
@@ -2166,17 +2043,15 @@
                 for each_key in removed_keys:
                     r.pop(each_key)
                 new_points_to_evaluate.append(r)
 
             search_alg = SearchAlgo(
                 metric="val_loss",
                 mode="min",
-                points_to_evaluate=[
-                    p for p in new_points_to_evaluate if len(p) == len(converted_space)
-                ],
+                points_to_evaluate=[p for p in new_points_to_evaluate if len(p) == len(converted_space)],
             )
         search_alg = ConcurrencyLimiter(search_alg, self._n_concurrent_trials)
         resources_per_trial = self._state.resources_per_trial
 
         if self._use_spark:
             # use spark as parallel backend
             analysis = tune.run(
@@ -2213,16 +2088,15 @@
                 **self._use_ray if isinstance(self._use_ray, dict) else {},
             )
         # logger.info([trial.last_result for trial in analysis.trials])
         trials = sorted(
             (
                 trial
                 for trial in analysis.trials
-                if trial.last_result
-                and trial.last_result.get("wall_clock_time") is not None
+                if trial.last_result and trial.last_result.get("wall_clock_time") is not None
             ),
             key=lambda x: x.last_result["wall_clock_time"],
         )
         for self._track_iter, trial in enumerate(trials):
             result = trial.last_result
             better = False
             if result:
@@ -2267,22 +2141,18 @@
             )
         if mlflow is not None and mlflow.active_run():
             with mlflow.start_run(nested=True):
                 mlflow.log_metric("iter_counter", self._track_iter)
                 if (search_state.metric_for_logging is not None) and (
                     "intermediate_results" in search_state.metric_for_logging
                 ):
-                    for each_entry in search_state.metric_for_logging[
-                        "intermediate_results"
-                    ]:
+                    for each_entry in search_state.metric_for_logging["intermediate_results"]:
                         with mlflow.start_run(nested=True):
                             mlflow.log_metrics(each_entry)
-                            mlflow.log_metric(
-                                "iter_counter", self._iter_per_learner[estimator]
-                            )
+                            mlflow.log_metric("iter_counter", self._iter_per_learner[estimator])
                     del search_state.metric_for_logging["intermediate_results"]
                 if search_state.metric_for_logging:
                     mlflow.log_metrics(search_state.metric_for_logging)
                 mlflow.log_metric("trial_time", search_state.trial_time)
                 mlflow.log_metric("wall_clock_time", self._state.time_from_start)
                 mlflow.log_metric("validation_loss", search_state.val_loss)
                 mlflow.log_params(search_state.config)
@@ -2320,16 +2190,15 @@
             from flaml import BlendSearch as SearchAlgo
         elif "random" == self._hpo_method:
             from flaml.tune.searcher import RandomSearch as SearchAlgo
         elif "cfocat" == self._hpo_method:
             from flaml.tune.searcher.cfo_cat import CFOCat as SearchAlgo
         else:
             raise NotImplementedError(
-                f"hpo_method={self._hpo_method} is not recognized. "
-                "'cfo' and 'bs' are supported."
+                f"hpo_method={self._hpo_method} is not recognized. " "'cfo' and 'bs' are supported."
             )
 
         est_retrain_time = next_trial_time = 0
         best_config_sig = None
         better = True  # whether we find a better model in one trial
         for self._track_iter in range(self._max_iter):
             if self._estimator_index is None:
@@ -2343,31 +2212,29 @@
             self._state.time_from_start = time.time() - self._start_time_flag
             time_left = self._state.time_budget - self._state.time_from_start
             budget_left = (
                 time_left
                 if not self._retrain_in_budget
                 or better
                 or (not self.best_estimator)
-                or self._search_states[self.best_estimator].sample_size
-                < self._state.data_size[0]
+                or self._search_states[self.best_estimator].sample_size < self._state.data_size[0]
                 else time_left - est_retrain_time
             )
             if not search_state.search_alg:
                 search_state.training_function = partial(
                     AutoMLState._compute_with_config_base,
                     state=self._state,
                     estimator=estimator,
                 )
                 search_space = search_state.search_space
                 if self._sample:
                     resource_attr = "FLAML_sample_size"
                     min_resource = (
                         self._min_sample_size[estimator]
-                        if isinstance(self._min_sample_size, dict)
-                        and estimator in self._min_sample_size
+                        if isinstance(self._min_sample_size, dict) and estimator in self._min_sample_size
                         else self._min_sample_size_input
                     )
                     max_resource = self._state.data_size[0]
                 else:
                     resource_attr = min_resource = max_resource = None
                 learner_class = self._state.learner_classes.get(estimator)
                 if "grid" == self._hpo_method:  # for synthetic exp only
@@ -2386,60 +2253,52 @@
                     self._max_iter_per_learner = len(points_to_evaluate)
                     low_cost_partial_config = None
                 else:
                     points_to_evaluate = search_state.init_config.copy()
 
                     low_cost_partial_config = search_state.low_cost_partial_config
                 time_budget_s = (
-                    min(budget_left, self._state.train_time_limit or np.inf)
-                    if self._state.time_budget >= 0
-                    else None
+                    min(budget_left, self._state.train_time_limit or np.inf) if self._state.time_budget >= 0 else None
                 )
                 if self._hpo_method in ("bs", "cfo", "grid", "cfocat", "random"):
                     algo = SearchAlgo(
                         metric="val_loss",
                         mode="min",
                         space=search_space,
                         points_to_evaluate=points_to_evaluate,
                         low_cost_partial_config=low_cost_partial_config,
                         cat_hp_cost=search_state.cat_hp_cost,
                         resource_attr=resource_attr,
                         min_resource=min_resource,
                         max_resource=max_resource,
-                        config_constraints=[
-                            (learner_class.size, "<=", self._mem_thres)
-                        ],
+                        config_constraints=[(learner_class.size, "<=", self._mem_thres)],
                         metric_constraints=self.metric_constraints,
                         seed=self._seed,
                         allow_empty_config=True,
                         time_budget_s=time_budget_s,
                         num_samples=self._max_iter,
                     )
                 else:
                     # if self._hpo_method is optuna, sometimes the search space and the initial config dimension do not match
                     # need to remove the extra keys from the search space to be consistent with the initial config
                     converted_space = SearchAlgo.convert_search_space(search_space)
-                    removed_keys = set(search_space.keys()).difference(
-                        converted_space.keys()
-                    )
+                    removed_keys = set(search_space.keys()).difference(converted_space.keys())
                     new_points_to_evaluate = []
                     for idx in range(len(points_to_evaluate)):
                         r = points_to_evaluate[idx].copy()
                         for each_key in removed_keys:
                             r.pop(each_key)
                         new_points_to_evaluate.append(r)
                     points_to_evaluate = new_points_to_evaluate
 
                     algo = SearchAlgo(
                         metric="val_loss",
                         mode="min",
                         space=search_space,
-                        points_to_evaluate=[
-                            p for p in points_to_evaluate if len(p) == len(search_space)
-                        ],
+                        points_to_evaluate=[p for p in points_to_evaluate if len(p) == len(search_space)],
                     )
                 search_state.search_alg = ConcurrencyLimiter(algo, max_concurrent=1)
                 # search_state.search_alg = algo
             else:
                 search_space = None
                 if self._hpo_method in ("bs", "cfo", "cfocat"):
                     search_state.search_alg.searcher.set_search_properties(
@@ -2462,17 +2321,15 @@
                 result = analysis.trials[-1].last_result
                 search_state.update(result, time_used=time_used)
                 if self._estimator_index is None:
                     # update init eci estimate
                     eci_base = search_state.init_eci
                     self._eci.append(search_state.estimated_cost4improvement)
                     for e in self.estimator_list[1:]:
-                        self._eci.append(
-                            self._search_states[e].init_eci / eci_base * self._eci[0]
-                        )
+                        self._eci.append(self._search_states[e].init_eci / eci_base * self._eci[0])
                     self._estimator_index = 0
                     min_budget = max(10 * self._eci[0], sum(self._eci))
                     max_budget = 10000 * self._eci[0]
                     if search_state.sample_size:
                         ratio = search_state.data_size[0] / search_state.sample_size
                         min_budget *= ratio
                         max_budget *= ratio
@@ -2531,22 +2388,18 @@
                         self._best_estimator,
                         self._state.best_loss,
                     )
                 )
                 if (
                     self._hpo_method in ("cfo", "bs")
                     and all(
-                        state.search_alg
-                        and state.search_alg.searcher.is_ls_ever_converged
+                        state.search_alg and state.search_alg.searcher.is_ls_ever_converged
                         for state in self._search_states.values()
                     )
-                    and (
-                        self._state.time_from_start
-                        > self._warn_threshold * self._time_taken_best_iter
-                    )
+                    and (self._state.time_from_start > self._warn_threshold * self._time_taken_best_iter)
                 ):
                     logger.warning(
                         "All estimator hyperparameters local search has "
                         "converged at least once, and the total search time "
                         f"exceeds {self._warn_threshold} times the time taken "
                         "to find the best model."
                     )
@@ -2561,40 +2414,32 @@
                     self._estimator_index -= 1
                 search_state.search_alg.searcher._is_ls_ever_converged = True
             if (
                 self._retrain_in_budget
                 and best_config_sig
                 and est_retrain_time
                 and not better
-                and self._search_states[self._best_estimator].sample_size
-                == self._state.data_size[0]
+                and self._search_states[self._best_estimator].sample_size == self._state.data_size[0]
                 and (
                     est_retrain_time
                     <= self._state.time_budget - self._state.time_from_start
                     <= est_retrain_time + next_trial_time
                 )
             ):
                 state = self._search_states[self._best_estimator]
                 self._trained_estimator, retrain_time = self._state._train_with_config(
                     self._best_estimator,
                     state.best_config,
                     self.data_size_full,
                 )
-                logger.info(
-                    "retrain {} for {:.1f}s".format(self._best_estimator, retrain_time)
-                )
-                self._retrained_config[
-                    best_config_sig
-                ] = state.best_config_train_time = retrain_time
+                logger.info("retrain {} for {:.1f}s".format(self._best_estimator, retrain_time))
+                self._retrained_config[best_config_sig] = state.best_config_train_time = retrain_time
                 est_retrain_time = 0
             self._state.time_from_start = time.time() - self._start_time_flag
-            if (
-                self._state.time_from_start >= self._state.time_budget >= 0
-                or not self._active_estimators
-            ):
+            if self._state.time_from_start >= self._state.time_budget >= 0 or not self._active_estimators:
                 break
             if self._ensemble and self._best_estimator:
                 time_left = self._state.time_budget - self._state.time_from_start
                 time_ensemble = self._search_states[self._best_estimator].time2eval_best
                 if time_left < time_ensemble < 2 * time_left:
                     break
 
@@ -2631,28 +2476,24 @@
             self._search_parallel()
         # Add a checkpoint for the current best config to the log.
         if self._training_log:
             self._training_log.checkpoint()
         self._state.time_from_start = time.time() - self._start_time_flag
         if self._best_estimator:
             self._selected = self._search_states[self._best_estimator]
-            self.modelcount = sum(
-                search_state.total_iter for search_state in self._search_states.values()
-            )
+            self.modelcount = sum(search_state.total_iter for search_state in self._search_states.values())
             if self._trained_estimator:
                 logger.info(f"selected model: {self._trained_estimator.model}")
             estimators = []
             if self._ensemble and self._state.task in (
                 "binary",
                 "multiclass",
                 "regression",
             ):
-                search_states = list(
-                    x for x in self._search_states.items() if x[1].best_config
-                )
+                search_states = list(x for x in self._search_states.items() if x[1].best_config)
                 search_states.sort(key=lambda x: x[1].best_loss)
                 estimators = [
                     (
                         x[0],
                         x[1].learner_class(
                             task=self._state.task,
                             n_jobs=self._state.n_jobs,
@@ -2669,62 +2510,51 @@
                             n_jobs=self._state.n_jobs,
                             **AutoMLState.sanitize(x[1].best_config),
                         ),
                     )
                     for x in search_states[2:]
                     if x[1].best_loss < 4 * self._selected.best_loss
                 ]
-                logger.info(
-                    [(estimator[0], estimator[1].params) for estimator in estimators]
-                )
+                logger.info([(estimator[0], estimator[1].params) for estimator in estimators])
             if len(estimators) > 1:
                 if self._state.task.is_classification():
                     from sklearn.ensemble import StackingClassifier as Stacker
                 else:
                     from sklearn.ensemble import StackingRegressor as Stacker
                 if self._use_ray is not False:
                     import ray
 
-                    n_cpus = (
-                        ray.is_initialized()
-                        and ray.available_resources()["CPU"]
-                        or os.cpu_count()
-                    )
+                    n_cpus = ray.is_initialized() and ray.available_resources()["CPU"] or os.cpu_count()
                 elif self._use_spark:
                     from flaml.tune.spark.utils import get_n_cpus
 
                     n_cpus = get_n_cpus()
                 else:
                     n_cpus = os.cpu_count()
                 ensemble_n_jobs = (
                     -self._state.n_jobs  # maximize total parallelization degree
-                    if abs(self._state.n_jobs)
-                    == 1  # 1 and -1 correspond to min/max parallelization
+                    if abs(self._state.n_jobs) == 1  # 1 and -1 correspond to min/max parallelization
                     else max(1, int(n_cpus / 2 / self._state.n_jobs))
                     # the total degree of parallelization = parallelization degree per estimator * parallelization degree of ensemble
                 )
                 if isinstance(self._ensemble, dict):
-                    final_estimator = self._ensemble.get(
-                        "final_estimator", self._trained_estimator
-                    )
+                    final_estimator = self._ensemble.get("final_estimator", self._trained_estimator)
                     passthrough = self._ensemble.get("passthrough", True)
                     ensemble_n_jobs = self._ensemble.get("n_jobs", ensemble_n_jobs)
                 else:
                     final_estimator = self._trained_estimator
                     passthrough = True
                 stacker = Stacker(
                     estimators,
                     final_estimator,
                     n_jobs=ensemble_n_jobs,
                     passthrough=passthrough,
                 )
                 sample_weight_dict = (
-                    (self._sample_weight_full is not None)
-                    and {"sample_weight": self._sample_weight_full}
-                    or {}
+                    (self._sample_weight_full is not None) and {"sample_weight": self._sample_weight_full} or {}
                 )
                 for e in estimators:
                     e[1].__class__.init()
                 import joblib
 
                 try:
                     logger.info("Building ensemble with tuned estimators")
@@ -2771,31 +2601,26 @@
                     or self._trained_estimator is None
                     or self._trained_estimator.model is None
                     or (
                         self._state.time_budget < 0
                         or self._state.time_budget - self._state.time_from_start
                         > self._selected.est_retrain_time(self.data_size_full)
                     )
-                    and self._selected.best_config_sample_size
-                    == self._state.data_size[0]
+                    and self._selected.best_config_sample_size == self._state.data_size[0]
                 ):
                     state = self._search_states[self._best_estimator]
                     (
                         self._trained_estimator,
                         retrain_time,
                     ) = self._state._train_with_config(
                         self._best_estimator,
                         state.best_config,
                         self.data_size_full,
                     )
-                    logger.info(
-                        "retrain {} for {:.1f}s".format(
-                            self._best_estimator, retrain_time
-                        )
-                    )
+                    logger.info("retrain {} for {:.1f}s".format(self._best_estimator, retrain_time))
                     state.best_config_train_time = retrain_time
                     if self._trained_estimator:
                         logger.info(f"retrained model: {self._trained_estimator.model}")
                 else:
                     logger.info("not retraining because the time budget is too small.")
 
     def __del__(self):
@@ -2822,40 +2647,32 @@
                 self._search_states[estimator].sample_size
             ):  # sample_size=None meaning no result
                 search_state = self._search_states[estimator]
                 if (
                     self._state.time_budget >= 0
                     and self._search_states[estimator].time2eval_best
                     > self._state.time_budget - self._state.time_from_start
-                    or self._iter_per_learner_fullsize[estimator]
-                    >= self._max_iter_per_learner
+                    or self._iter_per_learner_fullsize[estimator] >= self._max_iter_per_learner
                 ):
                     inv.append(0)
                     continue
                 estimated_cost = search_state.estimated_cost4improvement
-                if (
-                    search_state.sample_size < self._state.data_size[0]
-                    and self._state.time_budget >= 0
-                ):
+                if search_state.sample_size < self._state.data_size[0] and self._state.time_budget >= 0:
                     estimated_cost = min(
                         estimated_cost,
                         search_state.time2eval_best
                         * min(
                             SAMPLE_MULTIPLY_FACTOR,
                             self._state.data_size[0] / search_state.sample_size,
                         ),
                     )
                 gap = search_state.best_loss - self._state.best_loss
                 if gap > 0 and not self._ensemble:
-                    delta_loss = (
-                        search_state.best_loss_old - search_state.best_loss
-                    ) or search_state.best_loss
-                    delta_time = (
-                        search_state.total_time_used - search_state.time_best_found_old
-                    ) or 1e-10
+                    delta_loss = (search_state.best_loss_old - search_state.best_loss) or search_state.best_loss
+                    delta_time = (search_state.total_time_used - search_state.time_best_found_old) or 1e-10
                     speed = delta_loss / delta_time
                     if speed:
                         estimated_cost = max(2 * gap / speed, estimated_cost)
                 estimated_cost = estimated_cost or 1e-9
                 inv.append(1 / estimated_cost)
             else:
                 estimated_cost = self._eci[i]
```

### Comparing `FLAML-1.2.0/flaml/automl/data.py` & `FLAML-1.2.1/flaml/automl/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,15 @@
 if TYPE_CHECKING:
     from flaml.automl.task import Task
 
 TS_TIMESTAMP_COL = "ds"
 TS_VALUE_COL = "y"
 
 
-def load_openml_dataset(
-    dataset_id, data_dir=None, random_state=0, dataset_format="dataframe"
-):
+def load_openml_dataset(dataset_id, data_dir=None, random_state=0, dataset_format="dataframe"):
     """Load dataset from open ML.
 
     If the file is not cached locally, download it from open ML.
 
     Args:
         dataset_id: An integer of the dataset id in openml.
         data_dir: A string of the path to store and load the data.
@@ -73,17 +71,15 @@
         dataset = openml.datasets.get_dataset(dataset_id)
         if not os.path.exists(data_dir):
             os.makedirs(data_dir)
         with open(filepath, "wb") as f:
             pickle.dump(dataset, f, pickle.HIGHEST_PROTOCOL)
     print("Dataset name:", dataset.name)
     try:
-        X, y, *__ = dataset.get_data(
-            target=dataset.default_target_attribute, dataset_format=dataset_format
-        )
+        X, y, *__ = dataset.get_data(target=dataset.default_target_attribute, dataset_format=dataset_format)
     except ValueError:
         from sklearn.datasets import fetch_openml
 
         X, y = fetch_openml(data_id=dataset_id, return_X_y=True)
     X_train, X_test, y_train, y_test = train_test_split(X, y, random_state=random_state)
     print(
         "X_train.shape: {}, y_train.shape: {};\nX_test.shape: {}, y_test.shape: {}".format(
@@ -263,17 +259,15 @@
         X["time_idx"] = X["time_idx"].astype("int")
     return X
 
 
 class DataTransformer:
     """Transform input training data."""
 
-    def fit_transform(
-        self, X: Union[DataFrame, np.ndarray], y, task: Union[str, "Task"]
-    ):
+    def fit_transform(self, X: Union[DataFrame, np.ndarray], y, task: Union[str, "Task"]):
         """Fit transformer and process the input training data according to the task type.
 
         Args:
             X: A numpy array or a pandas dataframe of training data.
             y: A numpy array or a pandas series of labels.
             task: An instance of type Task, or a str such as 'classification', 'regression'.
 
@@ -308,29 +302,21 @@
                         X = add_time_idx_col(X)
                 ds_col = X.pop(TS_TIMESTAMP_COL)
                 if isinstance(y, Series):
                     y = y.rename(TS_VALUE_COL)
             for column in X.columns:
                 # sklearn\utils\validation.py needs int/float values
                 if X[column].dtype.name in ("object", "category"):
-                    if (
-                        X[column].nunique() == 1
-                        or X[column].nunique(dropna=True)
-                        == n - X[column].isnull().sum()
-                    ):
+                    if X[column].nunique() == 1 or X[column].nunique(dropna=True) == n - X[column].isnull().sum():
                         X.drop(columns=column, inplace=True)
                         drop = True
                     elif X[column].dtype.name == "category":
                         current_categories = X[column].cat.categories
                         if "__NAN__" not in current_categories:
-                            X[column] = (
-                                X[column]
-                                .cat.add_categories("__NAN__")
-                                .fillna("__NAN__")
-                            )
+                            X[column] = X[column].cat.add_categories("__NAN__").fillna("__NAN__")
                         cat_columns.append(column)
                     else:
                         X[column] = X[column].fillna("__NAN__")
                         cat_columns.append(column)
                 elif X[column].nunique(dropna=True) < 2:
                     X.drop(columns=column, inplace=True)
                     drop = True
@@ -345,18 +331,15 @@
                             f"minute_{column}": tmp_dt.minute,
                             f"second_{column}": tmp_dt.second,
                             f"dayofweek_{column}": tmp_dt.dayofweek,
                             f"dayofyear_{column}": tmp_dt.dayofyear,
                             f"quarter_{column}": tmp_dt.quarter,
                         }
                         for key, value in new_columns_dict.items():
-                            if (
-                                key not in X.columns
-                                and value.nunique(dropna=False) >= 2
-                            ):
+                            if key not in X.columns and value.nunique(dropna=False) >= 2:
                                 X[key] = value
                                 num_columns.append(key)
                         X[column] = X[column].map(datetime.toordinal)
                         datetime_columns.append(column)
                         del tmp_dt
                     X[column] = X[column].fillna(np.nan)
                     num_columns.append(column)
@@ -364,17 +347,15 @@
             if task.is_ts_forecast():
                 X.insert(0, TS_TIMESTAMP_COL, ds_col)
             if cat_columns:
                 X[cat_columns] = X[cat_columns].astype("category")
             if num_columns:
                 X_num = X[num_columns]
                 if np.issubdtype(X_num.columns.dtype, np.integer) and (
-                    drop
-                    or min(X_num.columns) != 0
-                    or max(X_num.columns) != X_num.shape[1] - 1
+                    drop or min(X_num.columns) != 0 or max(X_num.columns) != X_num.shape[1] - 1
                 ):
                     X_num.columns = range(X_num.shape[1])
                     drop = True
                 else:
                     drop = False
                 from sklearn.impute import SimpleImputer
                 from sklearn.compose import ColumnTransformer
@@ -391,19 +372,15 @@
                 X[num_columns] = self.transformer.fit_transform(X_num)
             self._cat_columns, self._num_columns, self._datetime_columns = (
                 cat_columns,
                 num_columns,
                 datetime_columns,
             )
             self._drop = drop
-        if (
-            task.is_classification()
-            or not pd.api.types.is_numeric_dtype(y)
-            and not task.is_nlg()
-        ):
+        if task.is_classification() or not pd.api.types.is_numeric_dtype(y) and not task.is_nlg():
             if not task.is_token_classification():
                 from sklearn.preprocessing import LabelEncoder
 
                 self.label_transformer = LabelEncoder()
             else:
                 from flaml.automl.nlp.utils import LabelEncoderforTokenClassification
 
@@ -462,17 +439,15 @@
                 X.insert(0, TS_TIMESTAMP_COL, ds_col)
             for column in cat_columns:
                 if X[column].dtype.name == "object":
                     X[column] = X[column].fillna("__NAN__")
                 elif X[column].dtype.name == "category":
                     current_categories = X[column].cat.categories
                     if "__NAN__" not in current_categories:
-                        X[column] = (
-                            X[column].cat.add_categories("__NAN__").fillna("__NAN__")
-                        )
+                        X[column] = X[column].cat.add_categories("__NAN__").fillna("__NAN__")
             if cat_columns:
                 X[cat_columns] = X[cat_columns].astype("category")
             if num_columns:
                 X_num = X[num_columns].fillna(np.nan)
                 if self._drop:
                     X_num.columns = range(X_num.shape[1])
                 X[num_columns] = self.transformer.transform(X_num)
```

### Comparing `FLAML-1.2.0/flaml/automl/ml.py` & `FLAML-1.2.1/flaml/automl/ml.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,17 +128,15 @@
     NOTE: See why the return type is declarad by using TypeVar here on the mypy doc
     https://mypy.readthedocs.io/en/stable/kinds_of_types.html#the-type-of-class-objects
     """
     # when adding a new learner, need to add an elif branch
     if "xgboost" == estimator_name:
         estimator_class = XGBoost_TS if task in TS_FORECAST else XGBoostSklearnEstimator
     elif "xgb_limitdepth" == estimator_name:
-        estimator_class = (
-            XGBoostLimitDepth_TS if task in TS_FORECAST else XGBoostLimitDepthEstimator
-        )
+        estimator_class = XGBoostLimitDepth_TS if task in TS_FORECAST else XGBoostLimitDepthEstimator
     elif "rf" == estimator_name:
         estimator_class = RF_TS if task in TS_FORECAST else RandomForestEstimator
     elif "lgbm" == estimator_name:
         estimator_class = LGBM_TS if task in TS_FORECAST else LGBMEstimator
     elif "lgbm_spark" == estimator_name:
         estimator_class = SparkLGBMEstimator
     elif "lrl1" == estimator_name:
@@ -199,48 +197,35 @@
             sample_weight,
             groups,
         )
     else:
         try:
             import datasets
 
-            datasets_metric_name = huggingface_submetric_to_metric.get(
-                metric_name, metric_name.split(":")[0]
-            )
+            datasets_metric_name = huggingface_submetric_to_metric.get(metric_name, metric_name.split(":")[0])
             metric = datasets.load_metric(datasets_metric_name)
             metric_mode = huggingface_metric_to_mode[datasets_metric_name]
 
             if metric_name.startswith("seqeval"):
-                y_processed_true = [
-                    [labels[tr] for tr in each_list] for each_list in y_processed_true
-                ]
+                y_processed_true = [[labels[tr] for tr in each_list] for each_list in y_processed_true]
             elif metric in ("pearsonr", "spearmanr"):
                 y_processed_true = (
-                    y_processed_true.to_list()
-                    if isinstance(y_processed_true, pd.Series)
-                    else list(y_processed_true)
+                    y_processed_true.to_list() if isinstance(y_processed_true, pd.Series) else list(y_processed_true)
                 )
-            score_dict = metric.compute(
-                predictions=y_processed_predict, references=y_processed_true
-            )
+            score_dict = metric.compute(predictions=y_processed_predict, references=y_processed_true)
             if "rouge" in metric_name:
                 score = score_dict[metric_name].mid.fmeasure
             elif metric_name.startswith("seqeval"):
                 metric_submetric_names = metric_name.split(":")
-                score = score_dict[
-                    metric_submetric_names[1]
-                    if len(metric_submetric_names) > 1
-                    else "overall_accuracy"
-                ]
+                score = score_dict[metric_submetric_names[1] if len(metric_submetric_names) > 1 else "overall_accuracy"]
             else:
                 score = score_dict[metric_name]
         except ImportError:
             raise ValueError(
-                metric_name
-                + " is not an built-in sklearn metric and [hf] is not installed. "
+                metric_name + " is not an built-in sklearn metric and [hf] is not installed. "
                 "Currently built-in sklearn metrics are: "
                 "r2, rmse, mae, mse, accuracy, roc_auc, roc_auc_ovr, roc_auc_ovo,"
                 "log_loss, mape, f1, micro_f1, macro_f1, ap. "
                 "If the metric is a huggingface metric, please pip install flaml[hf] ",
                 "or pass a customized metric function to AutoML.fit(metric=func)",
             )
         # If the metric is not found from huggingface dataset metric list (i.e., FileNotFoundError)
@@ -299,37 +284,29 @@
         score: A float number of the loss, the lower the better.
     """
     metric_name = metric_name.lower()
 
     if "r2" == metric_name:
         score = 1.0 - r2_score(y_true, y_predict, sample_weight=sample_weight)
     elif metric_name == "rmse":
-        score = np.sqrt(
-            mean_squared_error(y_true, y_predict, sample_weight=sample_weight)
-        )
+        score = np.sqrt(mean_squared_error(y_true, y_predict, sample_weight=sample_weight))
     elif metric_name == "mae":
         score = mean_absolute_error(y_true, y_predict, sample_weight=sample_weight)
     elif metric_name == "mse":
         score = mean_squared_error(y_true, y_predict, sample_weight=sample_weight)
     elif metric_name == "accuracy":
         score = 1.0 - accuracy_score(y_true, y_predict, sample_weight=sample_weight)
     elif metric_name == "roc_auc":
         score = 1.0 - roc_auc_score(y_true, y_predict, sample_weight=sample_weight)
     elif metric_name == "roc_auc_ovr":
-        score = 1.0 - roc_auc_score(
-            y_true, y_predict, sample_weight=sample_weight, multi_class="ovr"
-        )
+        score = 1.0 - roc_auc_score(y_true, y_predict, sample_weight=sample_weight, multi_class="ovr")
     elif metric_name == "roc_auc_ovo":
-        score = 1.0 - roc_auc_score(
-            y_true, y_predict, sample_weight=sample_weight, multi_class="ovo"
-        )
+        score = 1.0 - roc_auc_score(y_true, y_predict, sample_weight=sample_weight, multi_class="ovo")
     elif metric_name == "roc_auc_weighted":
-        score = 1.0 - roc_auc_score(
-            y_true, y_predict, sample_weight=sample_weight, average="weighted"
-        )
+        score = 1.0 - roc_auc_score(y_true, y_predict, sample_weight=sample_weight, average="weighted")
     elif metric_name == "roc_auc_ovo_weighted":
         score = 1.0 - roc_auc_score(
             y_true,
             y_predict,
             sample_weight=sample_weight,
             average="weighted",
             multi_class="ovo",
@@ -346,27 +323,21 @@
         score = log_loss(y_true, y_predict, labels=labels, sample_weight=sample_weight)
     elif "mape" == metric_name:
         try:
             score = mean_absolute_percentage_error(y_true, y_predict)
         except ValueError:
             return np.inf
     elif "micro_f1" == metric_name:
-        score = 1 - f1_score(
-            y_true, y_predict, sample_weight=sample_weight, average="micro"
-        )
+        score = 1 - f1_score(y_true, y_predict, sample_weight=sample_weight, average="micro")
     elif "macro_f1" == metric_name:
-        score = 1 - f1_score(
-            y_true, y_predict, sample_weight=sample_weight, average="macro"
-        )
+        score = 1 - f1_score(y_true, y_predict, sample_weight=sample_weight, average="macro")
     elif "f1" == metric_name:
         score = 1 - f1_score(y_true, y_predict, sample_weight=sample_weight)
     elif "ap" == metric_name:
-        score = 1 - average_precision_score(
-            y_true, y_predict, sample_weight=sample_weight
-        )
+        score = 1 - average_precision_score(y_true, y_predict, sample_weight=sample_weight)
     elif "ndcg" in metric_name:
         if "@" in metric_name:
             k = int(metric_name.split("@", 1)[-1])
             counts = group_counts(groups)
             score = 0
             psum = 0
             for c in counts:
@@ -520,17 +491,15 @@
         elif isinstance(metrics_to_log, dict):
             metrics_to_log = {k: metrics_to_log[k] + v for k, v in single_fold.items()}
         else:
             metrics_to_log += single_fold
     if metrics_to_log:
         n = len(val_loss_folds)
         metrics_to_log = (
-            {k: v / n for k, v in metrics_to_log.items()}
-            if isinstance(metrics_to_log, dict)
-            else metrics_to_log / n
+            {k: v / n for k, v in metrics_to_log.items()} if isinstance(metrics_to_log, dict) else metrics_to_log / n
         )
     return metric_to_minimize, metrics_to_log
 
 
 def compute_estimator(
     X_train,
     y_train,
@@ -542,17 +511,15 @@
     kf,
     config_dic: dict,
     task: str,
     estimator_name: str,
     eval_method: str,
     eval_metric: Union[str, Callable],
     best_val_loss=np.Inf,
-    n_jobs: Optional[
-        int
-    ] = 1,  # some estimators of EstimatorSubclass don't accept n_jobs. Should be None in that case.
+    n_jobs: Optional[int] = 1,  # some estimators of EstimatorSubclass don't accept n_jobs. Should be None in that case.
     estimator_class: Optional[EstimatorSubclass] = None,
     cv_score_agg_func: Optional[callable] = None,
     log_training_metric: Optional[bool] = False,
     fit_kwargs: Optional[dict] = None,
     free_mem_ratio=0,
 ):
     if fit_kwargs is None:
@@ -579,17 +546,15 @@
             y_train,
             X_val,
             y_val,
             weight_val,
             groups_val,
             eval_metric,
             task,
-            labels=fit_kwargs.get(
-                "label_list"
-            ),  # pass the label list on to compute the evaluation metric
+            labels=fit_kwargs.get("label_list"),  # pass the label list on to compute the evaluation metric
             budget=budget,
             log_training_metric=log_training_metric,
             fit_kwargs=fit_kwargs,
             free_mem_ratio=0,
         )
     else:
         val_loss, metric_for_logging, train_time, pred_time = task.evaluate_model_CV(
@@ -615,17 +580,15 @@
 
 def train_estimator(
     config_dic: dict,
     X_train,
     y_train,
     task: str,
     estimator_name: str,
-    n_jobs: Optional[
-        int
-    ] = 1,  # some estimators of EstimatorSubclass don't accept n_jobs. Should be None in that case.
+    n_jobs: Optional[int] = 1,  # some estimators of EstimatorSubclass don't accept n_jobs. Should be None in that case.
     estimator_class: Optional[EstimatorSubclass] = None,
     budget=None,
     fit_kwargs: Optional[dict] = None,
     eval_metric=None,
     free_mem_ratio=0,
 ) -> Tuple[EstimatorSubclass, float]:
     start_time = time.time()
@@ -638,26 +601,22 @@
     if fit_kwargs is None:
         fit_kwargs = {}
 
     if isinstance(estimator, TransformersEstimator):
         fit_kwargs["metric"] = eval_metric
 
     if X_train is not None:
-        train_time = estimator.fit(
-            X_train, y_train, budget, free_mem_ratio, **fit_kwargs
-        )
+        train_time = estimator.fit(X_train, y_train, budget, free_mem_ratio, **fit_kwargs)
     else:
         estimator = estimator.estimator_class(**estimator.params)
     train_time = time.time() - start_time
     return estimator, train_time
 
 
-def norm_confusion_matrix(
-    y_true: Union[np.array, pd.Series], y_pred: Union[np.array, pd.Series]
-):
+def norm_confusion_matrix(y_true: Union[np.array, pd.Series], y_pred: Union[np.array, pd.Series]):
     """normalized confusion matrix.
 
     Args:
         estimator: A multi-class classification estimator.
         y_true: A numpy array or a pandas series of true labels.
         y_pred: A numpy array or a pandas series of predicted labels.
```

### Comparing `FLAML-1.2.0/flaml/automl/model.py` & `FLAML-1.2.1/flaml/automl/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,17 +135,15 @@
         """
         self._task = task
         self.params = self.config2params(config)
         self.estimator_class = self._model = None
         if "_estimator_type" in config:
             self._estimator_type = self.params.pop("_estimator_type")
         else:
-            self._estimator_type = (
-                "classifier" if task in CLASSIFICATION else "regressor"
-            )
+            self._estimator_type = "classifier" if task in CLASSIFICATION else "regressor"
 
     def get_params(self, deep=False):
         params = self.params.copy()
         params["task"] = self._task
         if hasattr(self, "_estimator_type"):
             params["_estimator_type"] = self._estimator_type
         return params
@@ -251,16 +249,15 @@
             and resource is not None
             and (budget is not None or psutil is not None)
         ):
             start_time = time.time()
             mem = psutil.virtual_memory() if psutil is not None else None
             try:
                 with limit_resource(
-                    mem.available * (1 - free_mem_ratio)
-                    + psutil.Process(os.getpid()).memory_info().rss
+                    mem.available * (1 - free_mem_ratio) + psutil.Process(os.getpid()).memory_info().rss
                     if mem is not None
                     else -1,
                     budget,
                 ):
                     train_time = self._fit(X_train, y_train, **kwargs)
             except (MemoryError, TimeoutError) as e:
                 logger.warning(f"{e.__class__} {e}")
@@ -286,17 +283,15 @@
             A numpy array of shape n*1.
             Each element is the label for a instance.
         """
         if self._model is not None:
             X = self._preprocess(X)
             return self._model.predict(X, **kwargs)
         else:
-            logger.warning(
-                "Estimator is not fit yet. Please run fit() before predict()."
-            )
+            logger.warning("Estimator is not fit yet. Please run fit() before predict().")
             return np.ones(X.shape[0])
 
     def predict_proba(self, X, **kwargs):
         """Predict the probability of each class from features.
 
         Only works for classification problems
 
@@ -337,32 +332,28 @@
             The evaluation score on the validation dataset.
         """
         from .ml import metric_loss_score
         from .ml import is_min_metric
 
         if self._model is not None:
             if self._task == "rank":
-                raise NotImplementedError(
-                    "AutoML.score() is not implemented for ranking"
-                )
+                raise NotImplementedError("AutoML.score() is not implemented for ranking")
             else:
                 X_val = self._preprocess(X_val)
                 metric = kwargs.pop("metric", None)
                 if metric:
                     y_pred = self.predict(X_val, **kwargs)
                     if is_min_metric(metric):
                         return metric_loss_score(metric, y_pred, y_val)
                     else:
                         return 1.0 - metric_loss_score(metric, y_pred, y_val)
                 else:
                     return self._model.score(X_val, y_val, **kwargs)
         else:
-            logger.warning(
-                "Estimator is not fit yet. Please run fit() before predict()."
-            )
+            logger.warning("Estimator is not fit yet. Please run fit() before predict().")
             return 0.0
 
     def cleanup(self):
         del self._model
         self._model = None
 
     @classmethod
@@ -421,17 +412,15 @@
 
 
 class SparkEstimator(BaseEstimator):
     """The base class for fine-tuning spark models, using pyspark.ml and SynapseML API."""
 
     def __init__(self, task="binary", **config):
         if not _have_spark:
-            raise ImportError(
-                "pyspark is not installed. Try `pip install flaml[spark]`."
-            )
+            raise ImportError("pyspark is not installed. Try `pip install flaml[spark]`.")
         super().__init__(task, **config)
         self.df_train = None
 
     def _preprocess(
         self,
         X_train: Union[psDataFrame, sparkDataFrame],
         y_train: psSeries = None,
@@ -469,17 +458,15 @@
         train_time = self._fit(df_train, **kwargs)
         return train_time
 
     def _fit(self, df_train: sparkDataFrame, **kwargs):
         current_time = time.time()
         pipeline_model = self.estimator_class(**self.params, **kwargs)
         if logger.level == logging.DEBUG:
-            logger.debug(
-                f"flaml.model - {pipeline_model} fit started with params {self.params}"
-            )
+            logger.debug(f"flaml.model - {pipeline_model} fit started with params {self.params}")
         pipeline_model.fit(df_train)
         if logger.level == logging.DEBUG:
             logger.debug(f"flaml.model - {pipeline_model} fit finished")
         train_time = time.time() - current_time
         self._model = pipeline_model
         return train_time
 
@@ -490,27 +477,23 @@
             index_col: A str of the index column name. Default to "tmp_index_col".
             return_all: A bool of whether to return all the prediction results. Default to False.
         Returns:
             A pyspark.pandas series of shape n*1 if return_all is False. Otherwise, a pyspark.pandas dataframe.
         """
         if self._model is not None:
             X = self._preprocess(X, index_col=index_col)
-            predictions = to_pandas_on_spark(
-                self._model.transform(X), index_col=index_col
-            )
+            predictions = to_pandas_on_spark(self._model.transform(X), index_col=index_col)
             predictions.index.name = None
             pred_y = predictions["prediction"]
             if return_all:
                 return predictions
             else:
                 return pred_y
         else:
-            logger.warning(
-                "Estimator is not fit yet. Please run fit() before predict()."
-            )
+            logger.warning("Estimator is not fit yet. Please run fit() before predict().")
             return np.ones(X.shape[0])
 
     def predict_proba(self, X, index_col="tmp_index_col", return_all=False, **kwargs):
         """Predict the probability of each class from features.
         Only works for classification problems
         Args:
             X: A pyspark or pyspark.pandas dataframe of featurized instances, shape n*m.
@@ -520,28 +503,24 @@
             A pyspark.pandas dataframe of shape n*c. c is the # classes.
             Each element at (i,j) is the probability for instance i to be in
                 class j.
         """
         assert self._task in CLASSIFICATION, "predict_proba() only for classification."
         if self._model is not None:
             X = self._preprocess(X, index_col=index_col)
-            predictions = to_pandas_on_spark(
-                self._model.transform(X), index_col=index_col
-            )
+            predictions = to_pandas_on_spark(self._model.transform(X), index_col=index_col)
             predictions.index.name = None
             pred_y = predictions["probability"]
 
             if return_all:
                 return predictions
             else:
                 return pred_y
         else:
-            logger.warning(
-                "Estimator is not fit yet. Please run fit() before predict()."
-            )
+            logger.warning("Estimator is not fit yet. Please run fit() before predict().")
             return np.ones(X.shape[0])
 
 
 class SparkLGBMEstimator(SparkEstimator):
     """The class for fine-tuning spark version lightgbm models, using SynapseML API."""
 
     """The class for tuning LGBM, using sklearn API."""
@@ -596,17 +575,15 @@
             params.pop("n_jobs")
         if "log_max_bin" in params:
             params["maxBin"] = (1 << params.pop("log_max_bin")) - 1
         return params
 
     @classmethod
     def size(cls, config):
-        num_leaves = int(
-            round(config.get("numLeaves") or 1 << config.get("maxDepth", 16))
-        )
+        num_leaves = int(round(config.get("numLeaves") or 1 << config.get("maxDepth", 16)))
         n_estimators = int(round(config["numIterations"]))
         return (num_leaves * 3 + (num_leaves - 1) * 4 + 1.0) * n_estimators * 8
 
     def __init__(self, task="binary", **config):
         super().__init__(task, **config)
         err_msg = (
             "SynapseML is not installed. Please refer to [SynapseML]"
@@ -649,31 +626,25 @@
         budget=None,
         free_mem_ratio=0,
         index_col="tmp_index_col",
         **kwargs,
     ):
         start_time = time.time()
         if self.model_n_classes_ is None and self._task not in ["regression", "rank"]:
-            self.model_n_classes_, self.model_classes_ = len_labels(
-                y_train, return_labels=True
-            )
+            self.model_n_classes_, self.model_classes_ = len_labels(y_train, return_labels=True)
         df_train = self._preprocess(X_train, y_train, index_col=index_col)
         # n_iter = self.params.get(self.ITER_HP, self.DEFAULT_ITER)
         # trained = False
         # mem0 = psutil.virtual_memory().available if psutil is not None else 1
         _kwargs = kwargs.copy()
         if self._task not in ["regression", "rank"] and "objective" not in _kwargs:
-            _kwargs["objective"] = (
-                "binary" if self.model_n_classes_ == 2 else "multiclass"
-            )
+            _kwargs["objective"] = "binary" if self.model_n_classes_ == 2 else "multiclass"
         for k in list(_kwargs.keys()):
             if k not in self.estimator_params:
-                logger.warning(
-                    f"[SparkLGBMEstimator] [Warning] Ignored unknown parameter: {k}"
-                )
+                logger.warning(f"[SparkLGBMEstimator] [Warning] Ignored unknown parameter: {k}")
                 _kwargs.pop(k)
         # TODO: find a better estimation of early stopping
         # if (
         #     (not self._time_per_iter or abs(self._train_size - df_train.count()) > 4)
         #     and budget is not None
         #     or self._mem_per_iter < 0
         #     and psutil is not None
@@ -799,17 +770,15 @@
 
         for key, val in kwargs.items():
             assert key not in self.params, (
                 "Since {} is in the search space, it cannot exist in 'custom_fit_kwargs' at the same time."
                 "If you need to fix the value of {} to {}, the only way is to add a single-value domain in the search "
                 "space by adding:\n '{}': {{ 'domain': {} }} to 'custom_hp'. For example:"
                 'automl_settings["custom_hp"] = {{ "transformer": {{ "model_path": {{ "domain" : '
-                '"google/electra-small-discriminator" }} }} }}'.format(
-                    key, key, val, key, val
-                )
+                '"google/electra-small-discriminator" }} }} }}'.format(key, key, val, key, val)
             )
 
         """
             If use has specified any custom args for TrainingArguments, update these arguments
         """
         self._training_args = self._TrainingArguments(**kwargs)
 
@@ -819,33 +788,26 @@
         for key, val in self.params.items():
             if hasattr(self._training_args, key):
                 setattr(self._training_args, key, val)
 
         """
             Update the attributes in TrainingArguments that depends on the values of self.params
         """
-        local_dir = os.path.join(
-            self._training_args.output_dir, "train_{}".format(date_str())
-        )
+        local_dir = os.path.join(self._training_args.output_dir, "train_{}".format(date_str()))
         if self._use_ray is True:
             import ray
 
             self._training_args.output_dir = ray.tune.get_trial_dir()
         else:
-            self._training_args.output_dir = Counter.get_trial_fold_name(
-                local_dir, self.params, self.trial_id
-            )
+            self._training_args.output_dir = Counter.get_trial_fold_name(local_dir, self.params, self.trial_id)
 
         self._training_args.fp16 = self.fp16
         self._training_args.no_cuda = self.no_cuda
 
-        if (
-            self._task == TOKENCLASSIFICATION
-            and self._training_args.max_seq_length is not None
-        ):
+        if self._task == TOKENCLASSIFICATION and self._training_args.max_seq_length is not None:
             logger.warning(
                 "For token classification task, FLAML currently does not support customizing the max_seq_length, max_seq_length will be reset to None."
             )
             setattr(self._training_args, "max_seq_length", None)
 
     def _tokenize_text(self, X, y=None, **kwargs):
         from .nlp.huggingface.utils import tokenize_text
@@ -934,18 +896,15 @@
                 "label_pad_token_id": -100,  # pad with token id -100
                 "pad_to_multiple_of": 8,
                 # pad to multiple of 8 because quote Transformers: "This is especially useful to enable the use of Tensor Cores on NVIDIA hardware with compute capability >= 7.5 (Volta)"
                 "tokenizer": self.tokenizer,
             }
 
             for key in list(kwargs.keys()):
-                if (
-                    key not in data_collator_class.__dict__.keys()
-                    and key != "tokenizer"
-                ):
+                if key not in data_collator_class.__dict__.keys() and key != "tokenizer":
                     del kwargs[key]
             return data_collator_class(**kwargs)
         else:
             return None
 
     def fit(
         self,
@@ -980,17 +939,15 @@
         self._X_train, self._y_train = X_train, y_train
         self._set_training_args(**kwargs)
         self._add_prefix_space = (
             "roberta" in self._training_args.model_path
         )  # If using roberta model, must set add_prefix_space to True to avoid the assertion error at
         # https://github.com/huggingface/transformers/blob/main/src/transformers/models/roberta/tokenization_roberta_fast.py#L249
 
-        train_dataset, self._X_train, self._y_train = self._preprocess_data(
-            X_train, y_train
-        )
+        train_dataset, self._X_train, self._y_train = self._preprocess_data(X_train, y_train)
         if X_val is not None:
             eval_dataset, self._X_val, self._y_val = self._preprocess_data(X_val, y_val)
         else:
             eval_dataset, self._X_val, self._y_val = None, None, None
 
         set_seed(self.params.get("seed", self._training_args.seed))
         self._metric = metric
@@ -1003,30 +960,24 @@
                 self.step_begin_time = time.time()
 
             def on_step_end(self, args, state, control, **callback_kwargs):
                 if state.global_step == 1:
                     self.time_per_iter = time.time() - self.step_begin_time
                 if (
                     budget
-                    and (
-                        time.time() + self.time_per_iter
-                        > self.train_begin_time + budget
-                    )
+                    and (time.time() + self.time_per_iter > self.train_begin_time + budget)
                     or state.global_step >= this_params[TransformersEstimator.ITER_HP]
                 ):
                     control.should_training_stop = True
                     control.should_save = True
                     control.should_evaluate = True
                 return control
 
             def on_epoch_end(self, args, state, control, **callback_kwargs):
-                if (
-                    control.should_training_stop
-                    or state.epoch + 1 >= args.num_train_epochs
-                ):
+                if control.should_training_stop or state.epoch + 1 >= args.num_train_epochs:
                     control.should_save = True
                     control.should_evaluate = True
 
         self._trainer = TrainerForAuto(
             args=self._training_args,
             model_init=self._model_init,
             train_dataset=train_dataset,
@@ -1047,17 +998,15 @@
         if gpu_per_trial is not None:
             tmp_cuda_visible_devices = os.environ.get("CUDA_VISIBLE_DEVICES", "")
             self._trainer.args._n_gpu = gpu_per_trial
 
             # if gpu_per_trial == 0:
             #     os.environ["CUDA_VISIBLE_DEVICES"] = ""
             if tmp_cuda_visible_devices.count(",") != math.ceil(gpu_per_trial) - 1:
-                os.environ["CUDA_VISIBLE_DEVICES"] = ",".join(
-                    [str(x) for x in range(math.ceil(gpu_per_trial))]
-                )
+                os.environ["CUDA_VISIBLE_DEVICES"] = ",".join([str(x) for x in range(math.ceil(gpu_per_trial))])
 
         import time
 
         start_time = time.time()
         self._trainer.train()
 
         if gpu_per_trial is not None:
@@ -1066,18 +1015,15 @@
         self.params[self.ITER_HP] = self._trainer.state.global_step
 
         self._checkpoint_path = self._select_checkpoint(self._trainer)
         self._ckpt_remains = list(self._trainer.ckpt_to_metric.keys())
 
         if hasattr(self._trainer, "intermediate_results"):
             self.intermediate_results = [
-                x[1]
-                for x in sorted(
-                    self._trainer.intermediate_results.items(), key=lambda x: x[0]
-                )
+                x[1] for x in sorted(self._trainer.intermediate_results.items(), key=lambda x: x[0])
             ]
         self._trainer = None
 
         return time.time() - start_time
 
     def _delete_one_ckpt(self, ckpt_location):
         if self._use_ray is False:
@@ -1090,17 +1036,15 @@
             for each_ckpt in self._ckpt_remains:
                 self._delete_one_ckpt(each_ckpt)
 
     def _select_checkpoint(self, trainer):
         from transformers.trainer_utils import PREFIX_CHECKPOINT_DIR
 
         if trainer.ckpt_to_metric:
-            best_ckpt, _ = min(
-                trainer.ckpt_to_metric.items(), key=lambda x: x[1]["eval_automl_metric"]
-            )
+            best_ckpt, _ = min(trainer.ckpt_to_metric.items(), key=lambda x: x[1]["eval_automl_metric"])
             best_ckpt_global_step = trainer.ckpt_to_global_step[best_ckpt]
             for each_ckpt in list(trainer.ckpt_to_metric):
                 if each_ckpt != best_ckpt:
                     del trainer.ckpt_to_metric[each_ckpt]
                     del trainer.ckpt_to_global_step[each_ckpt]
                     self._delete_one_ckpt(each_ckpt)
         else:
@@ -1154,17 +1098,15 @@
     def _init_model_for_predict(self):
         from .nlp.huggingface.trainer import TrainerForAuto
 
         """
             Need to reinit training_args because of a bug in deepspeed: if not reinit, the deepspeed config will be inconsistent
             with HF config https://github.com/huggingface/transformers/blob/main/src/transformers/training_args.py#L947
         """
-        training_args = self._TrainingArguments(
-            local_rank=-1, model_path=self._checkpoint_path, fp16=self.fp16
-        )
+        training_args = self._TrainingArguments(local_rank=-1, model_path=self._checkpoint_path, fp16=self.fp16)
         for key, val in self._training_args.__dict__.items():
             if key not in ("local_rank", "model_path", "fp16"):
                 setattr(training_args, key, val)
         self._training_args = training_args
 
         new_trainer = TrainerForAuto(
             model=self._model_init(),
@@ -1179,24 +1121,27 @@
     def predict_proba(self, X, **pred_kwargs):
         from datasets import Dataset
 
         if pred_kwargs:
             for key, val in pred_kwargs.items():
                 setattr(self._training_args, key, val)
 
-        assert (
-            self._task in CLASSIFICATION
-        ), "predict_proba() only for classification tasks."
+        assert self._task in CLASSIFICATION, "predict_proba() only for classification tasks."
 
         X_test, _ = self._tokenize_text(X, **self._kwargs)
         test_dataset = Dataset.from_pandas(X_test)
 
         new_trainer = self._init_model_for_predict()
-        predictions = new_trainer.predict(test_dataset)
-        return predictions.predictions
+        try:
+            predictions = new_trainer.predict(test_dataset).predictions
+        except ZeroDivisionError:
+            logger.warning("Zero division error appeared in HuggingFace Transformers.")
+            predictions = np.array([-0.05] * len(test_dataset))
+        else:
+            return predictions
 
     def score(self, X_val: DataFrame, y_val: Series, **kwargs):
         import transformers
 
         transformers.logging.set_verbosity_error()
 
         self._metric = kwargs["metric"]
@@ -1218,47 +1163,43 @@
                 setattr(self._training_args, key, val)
 
         X_test, _ = self._tokenize_text(X, **self._kwargs)
         test_dataset = Dataset.from_pandas(X_test)
 
         new_trainer = self._init_model_for_predict()
 
-        if self._task not in NLG_TASKS:
-            predictions = new_trainer.predict(test_dataset)
-        else:
-            predictions = new_trainer.predict(
-                test_dataset,
-                metric_key_prefix="predict",
-            )
+        kwargs = {} if self._task not in NLG_TASKS else {"metric_key_prefix": "predict"}
+        try:
+            predictions = new_trainer.predict(test_dataset, **kwargs)
+        except ZeroDivisionError:
+            logger.warning("Zero division error appeared in HuggingFace Transformers.")
+            predictions = np.array([0] * len(test_dataset))
+
         post_y_pred, _ = postprocess_prediction_and_true(
             task=self._task,
             y_pred=predictions.predictions,
             tokenizer=self.tokenizer,
             hf_args=self._training_args,
             X=X,
         )
         return post_y_pred
 
     def config2params(self, config: dict) -> dict:
         params = super().config2params(config)
-        params[TransformersEstimator.ITER_HP] = params.get(
-            TransformersEstimator.ITER_HP, sys.maxsize
-        )
+        params[TransformersEstimator.ITER_HP] = params.get(TransformersEstimator.ITER_HP, sys.maxsize)
         return params
 
 
 class TransformersEstimatorModelSelection(TransformersEstimator):
     def __init__(self, task="seq-classification", **config):
         super().__init__(task, **config)
 
     @classmethod
     def search_space(cls, data_size, task, **params):
-        search_space_dict = TransformersEstimator.search_space(
-            data_size, task, **params
-        )
+        search_space_dict = TransformersEstimator.search_space(data_size, task, **params)
 
         """
             For model selection, use the same search space regardless of memory constraint
             If OOM, user should change the search space themselves
         """
 
         search_space_dict["model_path"] = {
@@ -1359,19 +1300,15 @@
         if "log_max_bin" in params:
             params["max_bin"] = (1 << params.pop("log_max_bin")) - 1
         return params
 
     @classmethod
     def size(cls, config):
         num_leaves = int(
-            round(
-                config.get("num_leaves")
-                or config.get("max_leaves")
-                or 1 << config.get("max_depth", 16)
-            )
+            round(config.get("num_leaves") or config.get("max_leaves") or 1 << config.get("max_depth", 16))
         )
         n_estimators = int(round(config["n_estimators"]))
         return (num_leaves * 3 + (num_leaves - 1) * 4 + 1.0) * n_estimators * 8
 
     def __init__(self, task="binary", **config):
         super().__init__(task, **config)
         if "verbose" not in self.params:
@@ -1390,19 +1327,15 @@
             self.estimator_class = LGBMClassifier
         self._time_per_iter = None
         self._train_size = 0
         self._mem_per_iter = -1
         self.HAS_CALLBACK = self.HAS_CALLBACK and self._callbacks(0, 0, 0) is not None
 
     def _preprocess(self, X):
-        if (
-            not isinstance(X, DataFrame)
-            and issparse(X)
-            and np.issubdtype(X.dtype, np.integer)
-        ):
+        if not isinstance(X, DataFrame) and issparse(X) and np.issubdtype(X.dtype, np.integer):
             X = X.astype(float)
         elif isinstance(X, np.ndarray) and X.dtype.kind not in "buif":
             # numpy array is not of numeric dtype
             X = DataFrame(X)
             for col in X.columns:
                 if isinstance(X[col][0], str):
                     X[col] = X[col].astype("category").cat.codes
@@ -1413,18 +1346,15 @@
         start_time = time.time()
         deadline = start_time + budget if budget else np.inf
         n_iter = self.params.get(self.ITER_HP, self.DEFAULT_ITER)
         trained = False
         if not self.HAS_CALLBACK:
             mem0 = psutil.virtual_memory().available if psutil is not None else 1
             if (
-                (
-                    not self._time_per_iter
-                    or abs(self._train_size - X_train.shape[0]) > 4
-                )
+                (not self._time_per_iter or abs(self._train_size - X_train.shape[0]) > 4)
                 and budget is not None
                 or self._mem_per_iter < 0
                 and psutil is not None
             ) and n_iter > 1:
                 self.params[self.ITER_HP] = 1
                 self._t1 = self._fit(X_train, y_train, **kwargs)
                 if budget is not None and self._t1 >= budget or n_iter == 1:
@@ -1436,61 +1366,49 @@
                 mem2 = psutil.virtual_memory().available if psutil is not None else 1
                 self._mem2 = max(mem0 - mem2, self._mem1)
                 # if self._mem1 <= 0:
                 #     self._mem_per_iter = self._mem2 / (self.params[self.ITER_HP] + 1)
                 # elif self._mem2 <= 0:
                 #     self._mem_per_iter = self._mem1
                 # else:
-                self._mem_per_iter = min(
-                    self._mem1, self._mem2 / self.params[self.ITER_HP]
-                )
+                self._mem_per_iter = min(self._mem1, self._mem2 / self.params[self.ITER_HP])
                 # if self._mem_per_iter <= 1 and psutil is not None:
                 #     n_iter = self.params[self.ITER_HP]
                 self._time_per_iter = (
                     (self._t2 - self._t1) / (self.params[self.ITER_HP] - 1)
                     if self._t2 > self._t1
                     else self._t1
                     if self._t1
                     else 0.001
                 )
                 self._train_size = X_train.shape[0]
-                if (
-                    budget is not None
-                    and self._t1 + self._t2 >= budget
-                    or n_iter == self.params[self.ITER_HP]
-                ):
+                if budget is not None and self._t1 + self._t2 >= budget or n_iter == self.params[self.ITER_HP]:
                     # self.params[self.ITER_HP] = n_iter
                     return time.time() - start_time
                 trained = True
             # logger.debug(mem0)
             # logger.debug(self._mem_per_iter)
             if n_iter > 1:
                 max_iter = min(
                     n_iter,
-                    int(
-                        (budget - time.time() + start_time - self._t1)
-                        / self._time_per_iter
-                        + 1
-                    )
+                    int((budget - time.time() + start_time - self._t1) / self._time_per_iter + 1)
                     if budget is not None
                     else n_iter,
                     int((1 - free_mem_ratio) * mem0 / self._mem_per_iter)
                     if psutil is not None and self._mem_per_iter > 0
                     else n_iter,
                 )
                 if trained and max_iter <= self.params[self.ITER_HP]:
                     return time.time() - start_time
                 # when not trained, train at least one iter
                 self.params[self.ITER_HP] = max(max_iter, 1)
         if self.HAS_CALLBACK:
             kwargs_callbacks = kwargs.get("callbacks")
             if kwargs_callbacks:
-                callbacks = kwargs_callbacks + self._callbacks(
-                    start_time, deadline, free_mem_ratio
-                )
+                callbacks = kwargs_callbacks + self._callbacks(start_time, deadline, free_mem_ratio)
                 kwargs.pop("callbacks")
             else:
                 callbacks = self._callbacks(start_time, deadline, free_mem_ratio)
             if isinstance(self, XGBoostSklearnEstimator):
                 from xgboost import __version__
 
                 if __version__ >= "1.6.0":
@@ -1807,17 +1725,15 @@
     @classmethod
     def cost_relative2lgbm(cls):
         return 2
 
     def config2params(self, config: dict) -> dict:
         params = super().config2params(config)
         if "max_leaves" in params:
-            params["max_leaf_nodes"] = params.get(
-                "max_leaf_nodes", params.pop("max_leaves")
-            )
+            params["max_leaf_nodes"] = params.get("max_leaf_nodes", params.pop("max_leaves"))
         if self._task not in CLASSIFICATION and "criterion" in config:
             params.pop("criterion")
         if "random_state" not in params:
             params["random_state"] = 12032022
         return params
 
     def __init__(
@@ -1943,20 +1859,15 @@
 
     def _preprocess(self, X):
         if isinstance(X, DataFrame):
             cat_columns = X.select_dtypes(include=["category"]).columns
             if not cat_columns.empty:
                 X = X.copy()
                 X[cat_columns] = X[cat_columns].apply(
-                    lambda x: x.cat.rename_categories(
-                        [
-                            str(c) if isinstance(c, float) else c
-                            for c in x.cat.categories
-                        ]
-                    )
+                    lambda x: x.cat.rename_categories([str(c) if isinstance(c, float) else c for c in x.cat.categories])
                 )
         elif isinstance(X, np.ndarray) and X.dtype.kind not in "buif":
             # numpy array is not of numeric dtype
             X = DataFrame(X)
             for col in X.columns:
                 if isinstance(X[col][0], str):
                     X[col] = X[col].astype("category").cat.codes
@@ -1996,27 +1907,19 @@
         train_dir = f"catboost_{str(start_time)}"
         X_train = self._preprocess(X_train)
         if isinstance(X_train, DataFrame):
             cat_features = list(X_train.select_dtypes(include="category").columns)
         else:
             cat_features = []
         use_best_model = kwargs.get("use_best_model", True)
-        n = (
-            max(int(len(y_train) * 0.9), len(y_train) - 1000)
-            if use_best_model
-            else len(y_train)
-        )
+        n = max(int(len(y_train) * 0.9), len(y_train) - 1000) if use_best_model else len(y_train)
         X_tr, y_tr = X_train[:n], y_train[:n]
         from catboost import Pool, __version__
 
-        eval_set = (
-            Pool(data=X_train[n:], label=y_train[n:], cat_features=cat_features)
-            if use_best_model
-            else None
-        )
+        eval_set = Pool(data=X_train[n:], label=y_train[n:], cat_features=cat_features) if use_best_model else None
         if "sample_weight" in kwargs:
             weight = kwargs["sample_weight"]
             if weight is not None:
                 kwargs["sample_weight"] = weight[:n]
         else:
             weight = None
 
@@ -2181,17 +2084,15 @@
                 " the timestamp values."
             )
         if self._model is not None:
             X = self._preprocess(X)
             forecast = self._model.predict(X, **kwargs)
             return forecast["yhat"]
         else:
-            logger.warning(
-                "Estimator is not fit yet. Please run fit() before predict()."
-            )
+            logger.warning("Estimator is not fit yet. Please run fit() before predict().")
             return np.ones(X.shape[0])
 
     def score(self, X_val: DataFrame, y_val: Series, **kwargs):
         from sklearn.metrics import r2_score
         from .ml import metric_loss_score
 
         y_pred = self.predict(X_val, **kwargs)
@@ -2270,17 +2171,15 @@
                 forecast = self._model.forecast(steps=X)
             elif isinstance(X, DataFrame):
                 start = X[TS_TIMESTAMP_COL].iloc[0]
                 end = X[TS_TIMESTAMP_COL].iloc[-1]
                 if len(X.columns) > 1:
                     X = self._preprocess(X.drop(columns=TS_TIMESTAMP_COL))
                     regressors = list(X)
-                    forecast = self._model.predict(
-                        start=start, end=end, exog=X[regressors], **kwargs
-                    )
+                    forecast = self._model.predict(start=start, end=end, exog=X[regressors], **kwargs)
                 else:
                     forecast = self._model.predict(start=start, end=end, **kwargs)
             else:
                 raise ValueError(
                     "X needs to be either a pandas Dataframe with dates as the first column"
                     " or an int number of periods for predict()."
                 )
@@ -2389,17 +2288,15 @@
             "trend": {"domain": tune.choice(["add", "mul", None]), "init_value": "add"},
             "seasonal": {
                 "domain": tune.choice(["add", "mul", None]),
                 "init_value": "add",
             },
             "use_boxcox": {"domain": tune.choice([False, True]), "init_value": False},
             "seasonal_periods": {  # statsmodels casts this to None if "seasonal" is None
-                "domain": tune.choice(
-                    [7, 12, 4, 52, 6]
-                ),  # weekly, yearly, quarterly, weekly w yearly data
+                "domain": tune.choice([7, 12, 4, 52, 6]),  # weekly, yearly, quarterly, weekly w yearly data
                 "init_value": 7,
             },
         }
         return space
 
     def fit(self, X_train, y_train, budget=None, free_mem_ratio=0, **kwargs):
         import warnings
@@ -2477,29 +2374,25 @@
             {
                 "optimize_for_horizon": {
                     "domain": tune.choice([True, False]),
                     "init_value": False,
                     "low_cost_init_value": False,
                 },
                 "lags": {
-                    "domain": tune.randint(
-                        lower=1, upper=max(2, int(np.sqrt(data_size[0])))
-                    ),
+                    "domain": tune.randint(lower=1, upper=max(2, int(np.sqrt(data_size[0])))),
                     "init_value": 3,
                 },
             }
         )
         return space
 
     def __init__(self, task="ts_forecast", **params):
         super().__init__(task, **params)
         self.hcrystaball_model = None
-        self.ts_task = (
-            "regression" if task in TS_FORECASTREGRESSION else "classification"
-        )
+        self.ts_task = "regression" if task in TS_FORECASTREGRESSION else "classification"
 
     def transform_X(self, X):
         cols = list(X)
         if len(cols) == 1:
             ds_col = cols[0]
             X = DataFrame(index=X[ds_col])
         elif len(cols) > 1:
@@ -2523,28 +2416,24 @@
         if optimize_for_horizon:
             # Direct Multi-step Forecast Strategy - fit a seperate model for each horizon
             model_list = []
             for i in range(1, kwargs["period"] + 1):
                 (
                     X_fit,
                     y_fit,
-                ) = self.hcrystaball_model._transform_data_to_tsmodel_input_format(
-                    X_train, y_train, i
-                )
+                ) = self.hcrystaball_model._transform_data_to_tsmodel_input_format(X_train, y_train, i)
                 self.hcrystaball_model.model.set_params(**estimator.params)
                 model = self.hcrystaball_model.model.fit(X_fit, y_fit)
                 model_list.append(model)
             self._model = model_list
         else:
             (
                 X_fit,
                 y_fit,
-            ) = self.hcrystaball_model._transform_data_to_tsmodel_input_format(
-                X_train, y_train, kwargs["period"]
-            )
+            ) = self.hcrystaball_model._transform_data_to_tsmodel_input_format(X_train, y_train, kwargs["period"])
             self.hcrystaball_model.model.set_params(**estimator.params)
             model = self.hcrystaball_model.model.fit(X_fit, y_fit)
             self._model = model
 
     def fit(self, X_train, y_train, budget=None, free_mem_ratio=0, **kwargs):
         current_time = time.time()
         self._fit(X_train, y_train, budget=budget, **kwargs)
@@ -2560,30 +2449,26 @@
                     X
                 ), "Model is optimized for horizon, length of X must be equal to `period`."
                 preds = []
                 for i in range(1, len(self._model) + 1):
                     (
                         X_pred,
                         _,
-                    ) = self.hcrystaball_model._transform_data_to_tsmodel_input_format(
-                        X.iloc[:i, :]
-                    )
+                    ) = self.hcrystaball_model._transform_data_to_tsmodel_input_format(X.iloc[:i, :])
                     preds.append(self._model[i - 1].predict(X_pred, **kwargs)[-1])
                 forecast = Series(preds)
             else:
                 (
                     X_pred,
                     _,
                 ) = self.hcrystaball_model._transform_data_to_tsmodel_input_format(X)
                 forecast = self._model.predict(X_pred, **kwargs)
             return forecast
         else:
-            logger.warning(
-                "Estimator is not fit yet. Please run fit() before predict()."
-            )
+            logger.warning("Estimator is not fit yet. Please run fit() before predict().")
             return np.ones(X.shape[0])
 
 
 class LGBM_TS(TS_SKLearn):
     """The class for tuning LGBM Regressor for time-series forecasting"""
 
     base_class = LGBMEstimator
@@ -2672,21 +2557,17 @@
                 "min_encoder_length", self.max_encoder_length // 2
             ),  # keep encoder length long (as it is in the validation set)
             max_encoder_length=self.max_encoder_length,
             min_prediction_length=1,
             max_prediction_length=max_prediction_length,
             static_categoricals=kwargs.get("static_categoricals", []),
             static_reals=kwargs.get("static_reals", []),
-            time_varying_known_categoricals=kwargs.get(
-                "time_varying_known_categoricals", []
-            ),
+            time_varying_known_categoricals=kwargs.get("time_varying_known_categoricals", []),
             time_varying_known_reals=kwargs.get("time_varying_known_reals", []),
-            time_varying_unknown_categoricals=kwargs.get(
-                "time_varying_unknown_categoricals", []
-            ),
+            time_varying_unknown_categoricals=kwargs.get("time_varying_unknown_categoricals", []),
             time_varying_unknown_reals=kwargs.get("time_varying_unknown_reals", []),
             variable_groups=kwargs.get(
                 "variable_groups", {}
             ),  # group of categorical variables can be treated as one variable
             lags=kwargs.get("lags", {}),
             target_normalizer=GroupNormalizer(
                 groups=kwargs["group_ids"], transformation="softplus"
@@ -2694,60 +2575,46 @@
             add_relative_time_idx=True,
             add_target_scales=True,
             add_encoder_length=True,
         )
 
         # create validation set (predict=True) which means to predict the last max_prediction_length points in time
         # for each series
-        validation = TimeSeriesDataSet.from_dataset(
-            training, self.data, predict=True, stop_randomization=True
-        )
+        validation = TimeSeriesDataSet.from_dataset(training, self.data, predict=True, stop_randomization=True)
 
         # create dataloaders for model
         batch_size = kwargs.get("batch_size", 64)
-        train_dataloader = training.to_dataloader(
-            train=True, batch_size=batch_size, num_workers=0
-        )
-        val_dataloader = validation.to_dataloader(
-            train=False, batch_size=batch_size * 10, num_workers=0
-        )
+        train_dataloader = training.to_dataloader(train=True, batch_size=batch_size, num_workers=0)
+        val_dataloader = validation.to_dataloader(train=False, batch_size=batch_size * 10, num_workers=0)
 
         return training, train_dataloader, val_dataloader
 
     def fit(self, X_train, y_train, budget=None, free_mem_ratio=0, **kwargs):
         import warnings
         import pytorch_lightning as pl
         from pytorch_lightning.callbacks import EarlyStopping, LearningRateMonitor
         import torch
         from pytorch_forecasting import TemporalFusionTransformer
         from pytorch_forecasting.metrics import QuantileLoss
 
         warnings.filterwarnings("ignore")
         current_time = time.time()
-        training, train_dataloader, val_dataloader = self.transform_ds(
-            X_train, y_train, **kwargs
-        )
+        training, train_dataloader, val_dataloader = self.transform_ds(X_train, y_train, **kwargs)
         params = self.params.copy()
         gradient_clip_val = params.pop("gradient_clip_val")
         params.pop("n_jobs")
         max_epochs = kwargs.get("max_epochs", 20)
-        early_stop_callback = EarlyStopping(
-            monitor="val_loss", min_delta=1e-4, patience=10, verbose=False, mode="min"
-        )
+        early_stop_callback = EarlyStopping(monitor="val_loss", min_delta=1e-4, patience=10, verbose=False, mode="min")
 
         def _fit(log):
             default_trainer_kwargs = dict(
-                gpus=kwargs.get("gpu_per_trial", [0])
-                if torch.cuda.is_available()
-                else None,
+                gpus=kwargs.get("gpu_per_trial", [0]) if torch.cuda.is_available() else None,
                 max_epochs=max_epochs,
                 gradient_clip_val=gradient_clip_val,
-                callbacks=[LearningRateMonitor(), early_stop_callback]
-                if log
-                else [early_stop_callback],
+                callbacks=[LearningRateMonitor(), early_stop_callback] if log else [early_stop_callback],
                 logger=log,
             )
             trainer = pl.Trainer(
                 **default_trainer_kwargs,
             )
             tft = TemporalFusionTransformer.from_dataset(
                 training,
@@ -2785,27 +2652,23 @@
         return train_time
 
     def predict(self, X):
         import pandas as pd
 
         ids = self.group_ids.copy()
         ids.append(TS_TIMESTAMP_COL)
-        encoder_data = self.data[
-            lambda x: x.time_idx > x.time_idx.max() - self.max_encoder_length
-        ]
+        encoder_data = self.data[lambda x: x.time_idx > x.time_idx.max() - self.max_encoder_length]
         # following pytorchforecasting example, make all target values equal to the last data
         last_data_cols = self.group_ids.copy()
         last_data_cols.append(TS_VALUE_COL)
         last_data = self.data[lambda x: x.time_idx == x.time_idx.max()][last_data_cols]
         decoder_data = X
         if "time_idx" not in decoder_data:
             decoder_data = add_time_idx_col(decoder_data)
-        decoder_data["time_idx"] += (
-            encoder_data["time_idx"].max() + 1 - decoder_data["time_idx"].min()
-        )
+        decoder_data["time_idx"] += encoder_data["time_idx"].max() + 1 - decoder_data["time_idx"].min()
         # decoder_data[TS_VALUE_COL] = 0
         decoder_data = decoder_data.merge(last_data, how="inner", on=self.group_ids)
         decoder_data = decoder_data.sort_values(ids)
         new_prediction_data = pd.concat([encoder_data, decoder_data], ignore_index=True)
         new_prediction_data["time_idx"] = new_prediction_data["time_idx"].astype("int")
         new_raw_predictions = self._model.predict(new_prediction_data)
         index = [decoder_data[idx].to_numpy() for idx in ids]
```

### Comparing `FLAML-1.2.0/flaml/automl/nlp/huggingface/data_collator.py` & `FLAML-1.2.1/flaml/automl/nlp/huggingface/data_collator.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,30 +18,23 @@
 @dataclass
 class DataCollatorForMultipleChoiceClassification(DataCollatorWithPadding):
     def __call__(self, features):
         from itertools import chain
         import torch
 
         label_name = "label" if "label" in features[0].keys() else "labels"
-        labels = (
-            [feature.pop(label_name) for feature in features]
-            if label_name in features[0]
-            else None
-        )
+        labels = [feature.pop(label_name) for feature in features] if label_name in features[0] else None
 
         batch_size = len(features)
         num_choices = len(features[0]["input_ids"])
         flattened_features = [
-            [{k: v[i] for k, v in feature.items()} for i in range(num_choices)]
-            for feature in features
+            [{k: v[i] for k, v in feature.items()} for i in range(num_choices)] for feature in features
         ]
         flattened_features = list(chain(*flattened_features))
-        batch = super(DataCollatorForMultipleChoiceClassification, self).__call__(
-            flattened_features
-        )
+        batch = super(DataCollatorForMultipleChoiceClassification, self).__call__(flattened_features)
         # Un-flatten
         batch = {k: v.view(batch_size, num_choices, -1) for k, v in batch.items()}
         # Add back labels
         if labels:
             batch["labels"] = torch.tensor(labels, dtype=torch.int64)
         return batch
```

### Comparing `FLAML-1.2.0/flaml/automl/nlp/huggingface/trainer.py` & `FLAML-1.2.1/flaml/automl/nlp/huggingface/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,33 +20,27 @@
                 test_dataset,
                 ignore_keys,
                 metric_key_prefix=metric_key_prefix,
                 max_length=max_length,
                 num_beams=num_beams,
             )
         else:
-            return super(Seq2SeqTrainer, self).predict(
-                test_dataset, ignore_keys, metric_key_prefix
-            )
+            return super(Seq2SeqTrainer, self).predict(test_dataset, ignore_keys, metric_key_prefix)
 
     def prediction_step(
         self,
         model,
         inputs,
         prediction_loss_only,
         ignore_keys,
     ):
         if getattr(self, "_is_seq2seq", None):
-            return super().prediction_step(
-                model, inputs, prediction_loss_only, ignore_keys
-            )
+            return super().prediction_step(model, inputs, prediction_loss_only, ignore_keys)
         else:
-            return super(Seq2SeqTrainer, self).prediction_step(
-                model, inputs, prediction_loss_only, ignore_keys
-            )
+            return super(Seq2SeqTrainer, self).prediction_step(model, inputs, prediction_loss_only, ignore_keys)
 
     def log(self, logs) -> None:
         if getattr(self, "_is_seq2seq", None):
             super().log(logs)
         else:
             super(Seq2SeqTrainer, self).log(logs)
         if not hasattr(self, "intermediate_results"):
@@ -62,17 +56,15 @@
         eval_dataset=None,
         ignore_keys=None,
         metric_key_prefix="eval",
     ):
         """Overriding transformers.Trainer.evaluate by saving metrics and checkpoint path."""
         from transformers.trainer_utils import PREFIX_CHECKPOINT_DIR
 
-        ckpt_dir = os.path.join(
-            self.args.output_dir, f"{PREFIX_CHECKPOINT_DIR}-{self.state.global_step}"
-        )
+        ckpt_dir = os.path.join(self.args.output_dir, f"{PREFIX_CHECKPOINT_DIR}-{self.state.global_step}")
         eval_dataset = eval_dataset if eval_dataset is not None else self.eval_dataset
 
         # TODO: if your task is seq2seq (i.e., SUMMARIZATION), uncomment the code below (add indentation before metrics = eval_dataset...
 
         if getattr(self, "_is_seq2seq", None):
             metrics = eval_dataset and super().evaluate(
                 eval_dataset,
```

### Comparing `FLAML-1.2.0/flaml/automl/nlp/huggingface/training_args.py` & `FLAML-1.2.1/flaml/automl/nlp/huggingface/training_args.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,70 +65,52 @@
     )
 
     per_device_eval_batch_size: int = field(
         default=1,
         metadata={"help": "per gpu evaluation batch size"},
     )
 
-    label_list: Optional[List[str]] = field(
-        default=None, metadata={"help": "The string list of the label names. "}
-    )
+    label_list: Optional[List[str]] = field(default=None, metadata={"help": "The string list of the label names. "})
 
-    eval_steps: int = field(
-        default=500, metadata={"help": "Run an evaluation every X steps."}
-    )
+    eval_steps: int = field(default=500, metadata={"help": "Run an evaluation every X steps."})
 
-    save_steps: int = field(
-        default=500, metadata={"help": "Save checkpoint every X updates steps."}
-    )
+    save_steps: int = field(default=500, metadata={"help": "Save checkpoint every X updates steps."})
 
-    logging_steps: int = field(
-        default=500, metadata={"help": "Log every X updates steps."}
-    )
+    logging_steps: int = field(default=500, metadata={"help": "Log every X updates steps."})
 
     @staticmethod
     def load_args_from_console():
         from dataclasses import fields
 
         arg_parser = argparse.ArgumentParser()
         for each_field in fields(TrainingArgumentsForAuto):
             print(each_field)
             arg_parser.add_argument(
                 "--" + each_field.name,
                 type=each_field.type,
                 help=each_field.metadata["help"],
-                required=each_field.metadata["required"]
-                if "required" in each_field.metadata
-                else False,
-                choices=each_field.metadata["choices"]
-                if "choices" in each_field.metadata
-                else None,
+                required=each_field.metadata["required"] if "required" in each_field.metadata else False,
+                choices=each_field.metadata["choices"] if "choices" in each_field.metadata else None,
                 default=each_field.default,
             )
         console_args, unknown = arg_parser.parse_known_args()
         return console_args
 
 
 @dataclass
 class Seq2SeqTrainingArgumentsForAuto(TrainingArgumentsForAuto):
     model_path: str = field(
         default="t5-small",
-        metadata={
-            "help": "model path for HPO natural language generation tasks, default is set to t5-small"
-        },
+        metadata={"help": "model path for HPO natural language generation tasks, default is set to t5-small"},
     )
 
-    sortish_sampler: bool = field(
-        default=False, metadata={"help": "Whether to use SortishSampler or not."}
-    )
+    sortish_sampler: bool = field(default=False, metadata={"help": "Whether to use SortishSampler or not."})
     predict_with_generate: bool = field(
         default=True,
-        metadata={
-            "help": "Whether to use generate to calculate generative metrics (ROUGE, BLEU)."
-        },
+        metadata={"help": "Whether to use generate to calculate generative metrics (ROUGE, BLEU)."},
     )
     generation_max_length: Optional[int] = field(
         default=None,
         metadata={
             "help": "The `max_length` to use on each evaluation loop when `predict_with_generate=True`. Will default "
             "to the `max_length` value of the model configuration."
         },
```

### Comparing `FLAML-1.2.0/flaml/automl/nlp/huggingface/utils.py` & `FLAML-1.2.1/flaml/automl/nlp/huggingface/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,24 +34,20 @@
             task=task,
             hf_args=hf_args,
             prefix_str="",
         )
         Y_tokenized = Y
         label_col_name = ["label"]
     elif task == TOKENCLASSIFICATION:
-        X_tokenized, Y_tokenized = tokenize_text_tokclassification(
-            X, Y, tokenizer=tokenizer, hf_args=hf_args
-        )
+        X_tokenized, Y_tokenized = tokenize_text_tokclassification(X, Y, tokenizer=tokenizer, hf_args=hf_args)
         label_col_name = ["labels"]
     elif task in NLG_TASKS:
         return tokenize_seq2seq(X, Y, tokenizer=tokenizer, task=task, hf_args=hf_args)
     elif task == MULTICHOICECLASSIFICATION:
-        X_tokenized = tokenize_text_multiplechoice(
-            X, tokenizer=tokenizer, hf_args=hf_args
-        )
+        X_tokenized = tokenize_text_multiplechoice(X, tokenizer=tokenizer, hf_args=hf_args)
         label_col_name = ["label"]
         Y_tokenized = Y
     Y_tokenized = todf(X_tokenized, Y_tokenized, label_col_name)
     return X_tokenized, Y_tokenized
 
 
 def tokenize_seq2seq(X, Y, tokenizer, task=None, hf_args=None):
@@ -71,17 +67,15 @@
             hf_args=hf_args,
             prefix_str="",
         )
         model_outputs["labels"] = [
             [(each_l if each_l != tokenizer.pad_token_id else -100) for each_l in label]
             for label in model_outputs["input_ids"]
         ]
-        model_outputs = model_outputs.drop(
-            columns=["attention_mask", "input_ids", "decoder_input_ids"]
-        )
+        model_outputs = model_outputs.drop(columns=["attention_mask", "input_ids", "decoder_input_ids"])
     return model_inputs, model_outputs
 
 
 def tokenize_and_align_labels(
     examples,
     tokenizer,
     label_to_id,
@@ -112,17 +106,15 @@
                 label_ids.append(label_to_id[examples[Y_sent_key][word_idx]])
             # For the other tokens in a word, we set the label to either the current label or -100, depending on
             # the label_all_tokens flag.
             else:
                 # Use the label_all_tokens to control whether to copy the label to all subtokens or to pad the additional tokens as -100
                 if hf_args.label_all_tokens:
                     # If the B- word is converted into multiple subtokens, map the additional subtokens to I-
-                    label_ids.append(
-                        b_to_i_label[label_to_id[examples[Y_sent_key][word_idx]]]
-                    )
+                    label_ids.append(b_to_i_label[label_to_id[examples[Y_sent_key][word_idx]]])
                 else:
                     label_ids.append(-100)
             previous_word_idx = word_idx
         tokenized_inputs["labels"] = label_ids
     tmp_column_names = sorted(tokenized_inputs.keys())
     tokenized_input_and_labels = [tokenized_inputs[x] for x in tmp_column_names]
     for key_idx, each_key in enumerate(tmp_column_names):
@@ -169,17 +161,15 @@
                 label_to_id=label_to_id,
                 b_to_i_label=b_to_i_label,
             ),
             axis=1,
             result_type="expand",
         )
         label_idx = tokenized_column_names.index("labels")
-        other_indices = sorted(
-            set(range(len(tokenized_column_names))).difference({label_idx})
-        )
+        other_indices = sorted(set(range(len(tokenized_column_names))).difference({label_idx}))
         other_column_names = [tokenized_column_names[x] for x in other_indices]
         d = X_and_Y_tokenized.iloc[:, other_indices]
         y_tokenized = X_and_Y_tokenized.iloc[:, label_idx]
     else:
         X_key = list(X.keys())[0]
 
         _, tokenized_column_names = tokenize_and_align_labels(
@@ -294,18 +284,15 @@
 
 
 def tokenize_swag(this_row, tokenizer, hf_args=None, return_column_name=False):
     first_sentences = [[this_row["sent1"]] * 4]
     # get each 1st sentence, multiply to 4 sentences
     question_headers = this_row["sent2"]
     # sent2 are the noun part of 2nd line
-    second_sentences = [
-        question_headers + " " + this_row[key]
-        for key in ["ending0", "ending1", "ending2", "ending3"]
-    ]
+    second_sentences = [question_headers + " " + this_row[key] for key in ["ending0", "ending1", "ending2", "ending3"]]
     # now the 2nd-sentences are formed by combing the noun part and 4 ending parts
 
     # Flatten out
     # From 2 dimension to 1 dimension array
     first_sentences = list(chain(*first_sentences))
 
     tokenized_example = tokenizer(
@@ -318,26 +305,22 @@
 
     if return_column_name:
         return [tokenized_example[x] for x in tmp_column_names], tmp_column_names
     else:
         return [tokenized_example[x] for x in tmp_column_names]
 
 
-def postprocess_prediction_and_true(
-    task, y_pred, tokenizer, hf_args, y_true=None, X=None
-):
+def postprocess_prediction_and_true(task, y_pred, tokenizer, hf_args, y_true=None, X=None):
     # postprocess the matrix prediction y_pred and ground truth y_true into user readable format, e.g., for summarization, decode into text
     if task == SEQCLASSIFICATION:
         return np.argmax(y_pred, axis=1), y_true
     elif task == SEQREGRESSION:
         return np.squeeze(y_pred), y_true  # predictions.reshape((len(predictions),))
     elif task == TOKENCLASSIFICATION:
-        assert (y_true is not None) or (
-            X is not None
-        ), "One of y_true and X must not be None"
+        assert (y_true is not None) or (X is not None), "One of y_true and X must not be None"
         ## If y_true is not None, we use y_true to remove the -100 in the prediction (postprocessing), and return the postprocessed y_true and prediction
         # If y_true is None, we use X to compute y_is_pad (i.e., whether y_true is -100 in that position), and use y_is_pad to remove the -100 in the prediction, and return the postprocessed prediction (not the y_true)
         y_predict = pd.Series(np.argmax(y_pred, axis=2).tolist())
         if y_true is None:
             _, y_is_pad_df = tokenize_text(
                 X,
                 y_predict,
@@ -350,25 +333,20 @@
             y_is_pad = y_true
         label_len = len(hf_args.label_list)
         zip_pred_ispad = [
             [(p, ispd) for (p, ispd) in zip(each_pred, each_is_pad) if ispd != -100]
             for (each_pred, each_is_pad) in zip(y_predict, y_is_pad)
         ]
         y_pred_label = [
-            [
-                hf_args.label_list[p] if 0 <= p < label_len else -1
-                for (p, ispd) in each_list
-            ]
+            [hf_args.label_list[p] if 0 <= p < label_len else -1 for (p, ispd) in each_list]
             for each_list in zip_pred_ispad
         ]  # To compute precision and recall, y_pred and y_true must be converted to string labels
         # (B-PER, I-PER, etc.), so that the category-based precision/recall (i.e., PER, LOC, etc.) scores can be computed
         if y_true is not None:
-            y_true_label = [
-                [tr for (p, tr) in each_list] for each_list in zip_pred_ispad
-            ]
+            y_true_label = [[tr for (p, tr) in each_list] for each_list in zip_pred_ispad]
         else:
             y_true_label = None
         return y_pred_label, y_true_label
     elif task == SUMMARIZATION:
         if isinstance(y_pred, tuple):
             y_pred = np.argmax(y_pred[0], axis=2)
         decoded_preds = tokenizer.batch_decode(y_pred, skip_special_tokens=True)
@@ -377,21 +355,17 @@
 
         nltk.download("punkt")
         decoded_preds = [pred.strip() for pred in decoded_preds]
         decoded_preds = ["\n".join(nltk.sent_tokenize(pred)) for pred in decoded_preds]
 
         if y_true is not None:
             y_true_labels = np.where(y_true != -100, y_true, tokenizer.pad_token_id)
-            decoded_y_true_labels = tokenizer.batch_decode(
-                y_true_labels, skip_special_tokens=True
-            )
+            decoded_y_true_labels = tokenizer.batch_decode(y_true_labels, skip_special_tokens=True)
             decoded_y_true_labels = [label.strip() for label in decoded_y_true_labels]
-            decoded_y_true_labels = [
-                "\n".join(nltk.sent_tokenize(label)) for label in decoded_y_true_labels
-            ]
+            decoded_y_true_labels = ["\n".join(nltk.sent_tokenize(label)) for label in decoded_y_true_labels]
         else:
             decoded_y_true_labels = None
 
         return decoded_preds, decoded_y_true_labels
     elif task == MULTICHOICECLASSIFICATION:
         return np.argmax(y_pred, axis=1), y_true
 
@@ -415,25 +389,19 @@
         from transformers import AutoModelForTokenClassification
 
         if task in (SEQCLASSIFICATION, SEQREGRESSION):
             return AutoModelForSequenceClassification.from_pretrained(
                 checkpoint_path, config=model_config, ignore_mismatched_sizes=True
             )
         elif task == TOKENCLASSIFICATION:
-            return AutoModelForTokenClassification.from_pretrained(
-                checkpoint_path, config=model_config
-            )
+            return AutoModelForTokenClassification.from_pretrained(checkpoint_path, config=model_config)
         elif task in NLG_TASKS:
-            return AutoModelForSeq2SeqLM.from_pretrained(
-                checkpoint_path, config=model_config
-            )
+            return AutoModelForSeq2SeqLM.from_pretrained(checkpoint_path, config=model_config)
         elif task == MULTICHOICECLASSIFICATION:
-            return AutoModelForMultipleChoice.from_pretrained(
-                checkpoint_path, config=model_config
-            )
+            return AutoModelForMultipleChoice.from_pretrained(checkpoint_path, config=model_config)
 
     def _set_model_config(checkpoint_path):
         if task in (SEQCLASSIFICATION, SEQREGRESSION, TOKENCLASSIFICATION):
             model_config = AutoConfig.from_pretrained(
                 checkpoint_path,
                 num_labels=model_config_num_labels,
             )
```

### Comparing `FLAML-1.2.0/flaml/automl/nlp/utils.py` & `FLAML-1.2.1/flaml/automl/nlp/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -81,36 +81,28 @@
 
 class Counter:
     counter = 0
 
     @staticmethod
     def get_trial_fold_name(local_dir, trial_config, trial_id):
         Counter.counter += 1
-        experiment_tag = "{0}_{1}".format(
-            str(Counter.counter), format_vars(trial_config)
-        )
-        logdir = get_logdir_name(
-            _generate_dirname(experiment_tag, trial_id=trial_id), local_dir
-        )
+        experiment_tag = "{0}_{1}".format(str(Counter.counter), format_vars(trial_config))
+        logdir = get_logdir_name(_generate_dirname(experiment_tag, trial_id=trial_id), local_dir)
         return logdir
 
 
 class LabelEncoderforTokenClassification:
     def fit_transform(self, y):
         # if the labels are tokens, convert them to ids
         if any(isinstance(id, str) for id in y[0]):
             self.label_list = sorted(list(set().union(*y)))
-            self._tokenlabel_to_id = {
-                self.label_list[id]: id for id in range(len(self.label_list))
-            }
+            self._tokenlabel_to_id = {self.label_list[id]: id for id in range(len(self.label_list))}
             y = y.apply(lambda sent: [self._tokenlabel_to_id[token] for token in sent])
         # if the labels are not tokens, they must be ids
         else:
-            assert all(
-                isinstance(id, (int, np.integer)) for id in y[0]
-            ), "The labels must either be tokens or ids"
+            assert all(isinstance(id, (int, np.integer)) for id in y[0]), "The labels must either be tokens or ids"
         return y
 
     def transform(self, y):
         if hasattr(self, "_tokenlabel_to_id"):
             y = y.apply(lambda sent: [self._tokenlabel_to_id[token] for token in sent])
         return y
```

### Comparing `FLAML-1.2.0/flaml/automl/spark/configs.py` & `FLAML-1.2.1/flaml/automl/spark/configs.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/automl/spark/metrics.py` & `FLAML-1.2.1/flaml/automl/spark/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,15 @@
     df = df.withColumn(prediction_col, F.array([df[prediction_col]]))
     return df
 
 
 def _compute_label_from_probability(df, probability_col, prediction_col):
     # array_max finds the maximum value in the 'probability' array
     # array_position finds the index of the maximum value in the 'probability' array
-    max_index_expr = F.expr(
-        f"array_position({probability_col}, array_max({probability_col}))-1"
-    )
+    max_index_expr = F.expr(f"array_position({probability_col}, array_max({probability_col}))-1")
     # Create a new column 'prediction' based on the maximum probability value
     df = df.withColumn(prediction_col, max_index_expr.cast("double"))
     return df
 
 
 def spark_metric_loss_score(
     metric_name: str,
@@ -139,17 +137,15 @@
             metricName="accuracy",
             labelCol=label_col,
             predictionCol=prediction_col,
             **kwargs,
         )
     elif metric_name == "log_loss":
         # For log_loss, prediction_col should be probability, and we need to convert it to label
-        df = _compute_label_from_probability(
-            df, prediction_col, prediction_col + "_label"
-        )
+        df = _compute_label_from_probability(df, prediction_col, prediction_col + "_label")
         evaluator = MulticlassClassificationEvaluator(
             metricName="logLoss",
             labelCol=label_col,
             predictionCol=prediction_col + "_label",
             probabilityCol=prediction_col,
             **kwargs,
         )
@@ -210,21 +206,15 @@
                         k=k,
                     )
                     score -= evaluator.evaluate(df)
                     psum += c
                 score /= len(counts)
                 score += 1
         else:
-            evaluator = RankingEvaluator(
-                metricName="ndcgAtK", labelCol=label_col, predictionCol=prediction_col
-            )
+            evaluator = RankingEvaluator(metricName="ndcgAtK", labelCol=label_col, predictionCol=prediction_col)
             df = _process_df(df, label_col, prediction_col)
             score = 1 - evaluator.evaluate(df)
         return score
     else:
         raise ValueError(f"Unknown metric name: {metric_name} for spark models.")
 
-    return (
-        evaluator.evaluate(df)
-        if metric_name in min_mode_metrics
-        else 1 - evaluator.evaluate(df)
-    )
+    return evaluator.evaluate(df) if metric_name in min_mode_metrics else 1 - evaluator.evaluate(df)
```

### Comparing `FLAML-1.2.0/flaml/automl/spark/utils.py` & `FLAML-1.2.1/flaml/automl/spark/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,17 +69,15 @@
         if _spark_major_minor_version[0] == 3 and _spark_major_minor_version[1] < 3:
             return df.to_pandas_on_spark(index_col=index_col)
         else:
             return df.pandas_api(index_col=index_col)
     elif isinstance(df, (ps.DataFrame, ps.Series)):
         return df
     else:
-        raise TypeError(
-            f"{type(df)} is not one of pandas.DataFrame, pandas.Series and pyspark.sql.DataFrame"
-        )
+        raise TypeError(f"{type(df)} is not one of pandas.DataFrame, pandas.Series and pyspark.sql.DataFrame")
 
 
 def train_test_split_pyspark(
     df: Union[DataFrame, ps.DataFrame],
     stratify_column: Optional[str] = None,
     test_fraction: Optional[float] = 0.2,
     seed: Optional[int] = 1234,
@@ -102,18 +100,15 @@
     """
     if isinstance(df, ps.DataFrame):
         df = df.to_spark(index_col=index_col)
 
     if stratify_column:
         # Test data
         test_fraction_dict = (
-            df.select(stratify_column)
-            .distinct()
-            .withColumn("fraction", F.lit(test_fraction))
-            .rdd.collectAsMap()
+            df.select(stratify_column).distinct().withColumn("fraction", F.lit(test_fraction)).rdd.collectAsMap()
         )
         df_test = df.stat.sampleBy(stratify_column, test_fraction_dict, seed)
         # Train data
         df_train = df.subtract(df_test)
     else:
         df_train, df_test = df.randomSplit([1 - test_fraction, test_fraction], seed)
 
@@ -124,42 +119,36 @@
         df_test.index.name = None
     elif index_col == "tmp_index_col":
         df_train = df_train.drop(index_col)
         df_test = df_test.drop(index_col)
     return [df_train, df_test]
 
 
-def unique_pandas_on_spark(
-    psds: Union[ps.Series, ps.DataFrame]
-) -> Tuple[np.ndarray, np.ndarray]:
+def unique_pandas_on_spark(psds: Union[ps.Series, ps.DataFrame]) -> Tuple[np.ndarray, np.ndarray]:
     """Get the unique values and counts of a pandas_on_spark series."""
     if isinstance(psds, ps.DataFrame):
         psds = psds.iloc[:, 0]
     _tmp = psds.value_counts().to_pandas()
     label_set = _tmp.index.values
     counts = _tmp.values
     return label_set, counts
 
 
-def len_labels(
-    y: Union[ps.Series, np.ndarray], return_labels=False
-) -> Union[int, Optional[np.ndarray]]:
+def len_labels(y: Union[ps.Series, np.ndarray], return_labels=False) -> Union[int, Optional[np.ndarray]]:
     """Get the number of unique labels in y."""
     if not isinstance(y, (ps.DataFrame, ps.Series)):
         labels = np.unique(y)
     else:
         labels = y.unique() if isinstance(y, ps.Series) else y.iloc[:, 0].unique()
     if return_labels:
         return len(labels), labels
     return len(labels)
 
 
-def unique_value_first_index(
-    y: Union[pd.Series, ps.Series, np.ndarray]
-) -> Tuple[np.ndarray, np.ndarray]:
+def unique_value_first_index(y: Union[pd.Series, ps.Series, np.ndarray]) -> Tuple[np.ndarray, np.ndarray]:
     """Get the unique values and indices of a pandas series,
     pandas_on_spark series or numpy array."""
     if isinstance(y, ps.Series):
         y_unique = y.drop_duplicates().sort_index()
         label_set = y_unique.values
         first_index = y_unique.index.values
     else:
@@ -192,17 +181,15 @@
         psdfiloc = to_pandas_on_spark(sdfiloc)
         if isinstance(psdf, ps.Series):
             psdfiloc = psdfiloc[psdfiloc.columns.drop(index_col)[0]]
         elif index_col not in psdf.columns:
             psdfiloc = psdfiloc.drop(columns=[index_col])
         return psdfiloc
     else:
-        raise TypeError(
-            f"{type(index)} is not one of int, slice and list for pandas_on_spark iloc"
-        )
+        raise TypeError(f"{type(index)} is not one of int, slice and list for pandas_on_spark iloc")
 
 
 def spark_kFold(
     dataset: Union[DataFrame, ps.DataFrame],
     nFolds: int = 3,
     foldCol: str = "",
     seed: int = 42,
@@ -237,17 +224,15 @@
         df = dataset.select("*", F.rand(seed).alias(randCol))
         for i in range(nFolds):
             validateLB = i * h
             validateUB = (i + 1) * h
             condition = (df[randCol] >= validateLB) & (df[randCol] < validateUB)
             validation = to_pandas_on_spark(df.filter(condition), index_col=index_col)
             train = to_pandas_on_spark(df.filter(~condition), index_col=index_col)
-            datasets.append(
-                (train.drop(columns=[randCol]), validation.drop(columns=[randCol]))
-            )
+            datasets.append((train.drop(columns=[randCol]), validation.drop(columns=[randCol])))
     else:
         # Use user-specified fold column
         def get_fold_num(foldNum: int) -> int:
             return int(foldNum % nFolds)
 
         get_fold_num_udf = F.UserDefinedFunction(get_fold_num, T.IntegerType())
         for i in range(nFolds):
```

### Comparing `FLAML-1.2.0/flaml/automl/state.py` & `FLAML-1.2.1/flaml/automl/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,17 +59,15 @@
             For each hp in the starting point, check the following 3 conditions:
             (1) If the type of the starting point does not match the required type in search space, return false
             (2) If the starting point is not in the required search space, return false
             (3) If the search space is a value instead of domain, and the value is not equal to the starting point
             Notice (2) include the case starting point not in user specified search space custom_hp
         """
         if isinstance(domain_one_dim, sample.Domain):
-            renamed_type = list(
-                inspect.signature(domain_one_dim.is_valid).parameters.values()
-            )[0].annotation
+            renamed_type = list(inspect.signature(domain_one_dim.is_valid).parameters.values())[0].annotation
             type_match = (
                 renamed_type == Any
                 or isinstance(value_one_dim, renamed_type)
                 or isinstance(value_one_dim, int)
                 and renamed_type is float
             )
             if not (type_match and domain_one_dim.is_valid(value_one_dim)):
@@ -102,80 +100,63 @@
         self.low_cost_partial_config = {}
         self.cat_hp_cost = {}
         self.data_size = data_size
         self.ls_ever_converged = False
         self.learner_class = learner_class
         self._budget = budget
         if task in TS_FORECAST:
-            search_space = learner_class.search_space(
-                data_size=data_size, task=task, pred_horizon=period
-            )
+            search_space = learner_class.search_space(data_size=data_size, task=task, pred_horizon=period)
         else:
             search_space = learner_class.search_space(data_size=data_size, task=task)
 
         if custom_hp is not None:
             search_space.update(custom_hp)
 
         if isinstance(starting_point, dict):
             starting_point = AutoMLState.sanitize(starting_point)
-            if max_iter > 1 and not self.valid_starting_point(
-                starting_point, search_space
-            ):
+            if max_iter > 1 and not self.valid_starting_point(starting_point, search_space):
                 # If the number of iterations is larger than 1, remove invalid point
                 logger.warning(
-                    "Starting point {} removed because it is outside of the search space".format(
-                        starting_point
-                    )
+                    "Starting point {} removed because it is outside of the search space".format(starting_point)
                 )
                 starting_point = None
         elif isinstance(starting_point, list):
             starting_point = [AutoMLState.sanitize(x) for x in starting_point]
             if max_iter > len(starting_point):
                 # If the number of starting points is no smaller than max iter, avoid the checking
                 starting_point_len = len(starting_point)
-                starting_point = [
-                    x
-                    for x in starting_point
-                    if self.valid_starting_point(x, search_space)
-                ]
+                starting_point = [x for x in starting_point if self.valid_starting_point(x, search_space)]
                 if starting_point_len > len(starting_point):
                     logger.warning(
                         "Starting points outside of the search space are removed. "
                         f"Remaining starting points for {learner_class}: {starting_point}"
                     )
                 starting_point = starting_point or None
 
         for name, space in search_space.items():
-            assert (
-                "domain" in space
-            ), f"{name}'s domain is missing in the search space spec {space}"
+            assert "domain" in space, f"{name}'s domain is missing in the search space spec {space}"
             if space["domain"] is None:
                 # don't search this hp
                 continue
             self._search_space_domain[name] = space["domain"]
 
             if "low_cost_init_value" in space:
                 self.low_cost_partial_config[name] = space["low_cost_init_value"]
             if "cat_hp_cost" in space:
                 self.cat_hp_cost[name] = space["cat_hp_cost"]
             # if a starting point is provided, set the init config to be
             # the starting point provided
-            if (
-                isinstance(starting_point, dict)
-                and starting_point.get(name) is not None
-            ):
+            if isinstance(starting_point, dict) and starting_point.get(name) is not None:
                 if self.init_config is None:
                     self.init_config = {}
                 self.init_config[name] = starting_point[name]
             elif (
                 not isinstance(starting_point, list)
                 and "init_value" in space
-                and self.valid_starting_point_one_dim(
-                    space["init_value"], space["domain"]
-                )
+                and self.valid_starting_point_one_dim(space["init_value"], space["domain"])
             ):
                 if self.init_config is None:
                     self.init_config = {}
                 self.init_config[name] = space["init_value"]
 
         if isinstance(starting_point, list):
             self.init_config = starting_point
@@ -237,36 +218,30 @@
             self.iter_best_found = self.total_iter
             self.best_config = config
             self.best_config_sample_size = self.sample_size
             self.best_config_train_time = time_used
             if time2eval:
                 self.time2eval_best_old = self.time2eval_best
                 self.time2eval_best = time2eval
-            if (
-                self.trained_estimator
-                and trained_estimator
-                and self.trained_estimator != trained_estimator
-            ):
+            if self.trained_estimator and trained_estimator and self.trained_estimator != trained_estimator:
                 self.trained_estimator.cleanup()
             if trained_estimator:
                 self.trained_estimator = trained_estimator
         elif trained_estimator:
             trained_estimator.cleanup()
         self.metric_for_logging = metric_for_logging
         self.val_loss, self.config = obj, config
 
     def get_hist_config_sig(self, sample_size, config):
         config_values = tuple([config[k] for k in self._hp_names if k in config])
         config_sig = str(sample_size) + "_" + str(config_values)
         return config_sig
 
     def est_retrain_time(self, retrain_sample_size):
-        assert (
-            self.best_config_sample_size is not None
-        ), "need to first get best_config_sample_size"
+        assert self.best_config_sample_size is not None, "need to first get best_config_sample_size"
         return self.time2eval_best * retrain_sample_size / self.best_config_sample_size
 
 
 class AutoMLState:
     def _prepare_sample_train_data(self, sample_size: int):
         sampled_weight = groups = None
         if sample_size <= self.data_size[0]:
@@ -279,17 +254,15 @@
             else:
                 sampled_y_train = self.y_train[:sample_size]
             weight = self.fit_kwargs.get(
                 "sample_weight"
             )  # NOTE: _prepare_sample_train_data is before kwargs is updated to fit_kwargs_by_estimator
             if weight is not None:
                 sampled_weight = (
-                    weight.iloc[:sample_size]
-                    if isinstance(weight, (pd.Series, psSeries))
-                    else weight[:sample_size]
+                    weight.iloc[:sample_size] if isinstance(weight, (pd.Series, psSeries)) else weight[:sample_size]
                 )
             if self.groups is not None:
                 groups = (
                     self.groups.iloc[:sample_size]
                     if isinstance(self.groups, (pd.Series, psSeries))
                     else self.groups[:sample_size]
                 )
@@ -334,18 +307,15 @@
         if "FLAML_sample_size" in config:
             del config["FLAML_sample_size"]
         budget = (
             None
             if state.time_budget < 0
             else state.time_budget - state.time_from_start
             if sample_size == state.data_size[0]
-            else (state.time_budget - state.time_from_start)
-            / 2
-            * sample_size
-            / state.data_size[0]
+            else (state.time_budget - state.time_from_start) / 2 * sample_size / state.data_size[0]
         )
 
         (
             trained_estimator,
             val_loss,
             metric_for_logging,
             _,
@@ -353,17 +323,15 @@
         ) = compute_estimator(
             sampled_X_train,
             sampled_y_train,
             state.X_val,
             state.y_val,
             state.weight_val,
             state.groups_val,
-            state.train_time_limit
-            if budget is None
-            else min(budget, state.train_time_limit or np.inf),
+            state.train_time_limit if budget is None else min(budget, state.train_time_limit or np.inf),
             state.kf,
             config,
             state.task,
             estimator,
             state.eval_method,
             state.metric,
             state.best_loss,
@@ -402,17 +370,15 @@
     def _train_with_config(
         self,
         estimator: str,
         config_w_resource: dict,
         sample_size: Optional[int] = None,
     ):
         if not sample_size:
-            sample_size = config_w_resource.get(
-                "FLAML_sample_size", len(self.y_train_all)
-            )
+            sample_size = config_w_resource.get("FLAML_sample_size", len(self.y_train_all))
         config = AutoMLState.sanitize(config_w_resource)
 
         this_estimator_kwargs = self.fit_kwargs_by_estimator.get(
             estimator
         ).copy()  # NOTE: _train_with_config is after kwargs is updated to fit_kwargs_by_estimator
         (
             sampled_X_train,
@@ -428,17 +394,15 @@
                 "sample_weight"
             ] = sampled_weight  # NOTE: _train_with_config is after kwargs is updated to fit_kwargs_by_estimator
         if groups is not None:
             this_estimator_kwargs[
                 "groups"
             ] = groups  # NOTE: _train_with_config is after kwargs is updated to fit_kwargs_by_estimator
 
-        budget = (
-            None if self.time_budget < 0 else self.time_budget - self.time_from_start
-        )
+        budget = None if self.time_budget < 0 else self.time_budget - self.time_from_start
 
         estimator, train_time = train_estimator(
             X_train=sampled_X_train,
             y_train=sampled_y_train,
             config_dic=config,
             task=self.task,
             estimator_name=estimator,
```

### Comparing `FLAML-1.2.0/flaml/automl/task/generic_task.py` & `FLAML-1.2.1/flaml/automl/task/generic_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,64 +104,46 @@
         label,
         X_val=None,
         y_val=None,
         groups_val=None,
         groups=None,
     ):
         if X_train_all is not None and y_train_all is not None:
-            assert isinstance(
-                X_train_all, (np.ndarray, pd.DataFrame, psDataFrame)
-            ) or issparse(X_train_all), (
+            assert isinstance(X_train_all, (np.ndarray, pd.DataFrame, psDataFrame)) or issparse(X_train_all), (
                 "X_train_all must be a numpy array, a pandas dataframe, "
                 "a Scipy sparse matrix or a pyspark.pandas dataframe."
             )
             assert isinstance(
                 y_train_all, (np.ndarray, pd.Series, psSeries)
             ), "y_train_all must be a numpy array, a pandas series or a pyspark.pandas series."
-            assert (
-                X_train_all.size != 0 and y_train_all.size != 0
-            ), "Input data must not be empty."
+            assert X_train_all.size != 0 and y_train_all.size != 0, "Input data must not be empty."
             if isinstance(X_train_all, np.ndarray) and len(X_train_all.shape) == 1:
                 X_train_all = np.reshape(X_train_all, (X_train_all.size, 1))
             if isinstance(y_train_all, np.ndarray):
                 y_train_all = y_train_all.flatten()
-            assert (
-                X_train_all.shape[0] == y_train_all.shape[0]
-            ), "# rows in X_train must match length of y_train."
+            assert X_train_all.shape[0] == y_train_all.shape[0], "# rows in X_train must match length of y_train."
             if isinstance(X_train_all, psDataFrame):
-                X_train_all = (
-                    X_train_all.spark.cache()
-                )  # cache data to improve compute speed
+                X_train_all = X_train_all.spark.cache()  # cache data to improve compute speed
                 y_train_all = y_train_all.to_frame().spark.cache()[y_train_all.name]
-                logger.debug(
-                    f"X_train_all and y_train_all cached, shape of X_train_all: {X_train_all.shape}"
-                )
+                logger.debug(f"X_train_all and y_train_all cached, shape of X_train_all: {X_train_all.shape}")
             automl._df = isinstance(X_train_all, (pd.DataFrame, psDataFrame))
             automl._nrow, automl._ndim = X_train_all.shape
             if self.is_ts_forecast():
-                X_train_all = (
-                    pd.DataFrame(X_train_all)
-                    if isinstance(X_train_all, np.ndarray)
-                    else X_train_all
-                )
-                X_train_all, y_train_all = self._validate_ts_data(
-                    X_train_all, y_train_all
-                )
+                X_train_all = pd.DataFrame(X_train_all) if isinstance(X_train_all, np.ndarray) else X_train_all
+                X_train_all, y_train_all = self._validate_ts_data(X_train_all, y_train_all)
             X, y = X_train_all, y_train_all
         elif dataframe is not None and label is not None:
             assert isinstance(
                 dataframe, (pd.DataFrame, psDataFrame)
             ), "dataframe must be a pandas DataFrame or a pyspark.pandas DataFrame."
             assert (
                 label in dataframe.columns
             ), f"The provided label column name `{label}` doesn't exist in the provided dataframe."
             if isinstance(dataframe, psDataFrame):
-                dataframe = (
-                    dataframe.spark.cache()
-                )  # cache data to improve compute speed
+                dataframe = dataframe.spark.cache()  # cache data to improve compute speed
                 logger.debug(f"dataframe cached, shape of dataframe: {dataframe.shape}")
             automl._df = True
             if self.is_ts_forecast():
                 dataframe = self._validate_ts_data(dataframe)
             # TODO: to support pyspark.sql.DataFrame and pure dataframe mode
             X = dataframe.drop(columns=label)
             automl._nrow, automl._ndim = X.shape
@@ -179,17 +161,15 @@
                 assert X[column].dtype.name in (
                     "object",
                     "string",
                 ), "If the task is an NLP task, X can only contain text columns"
                 for _, each_cell in X[column].items():
                     if each_cell is not None:
                         is_str = isinstance(each_cell, str)
-                        is_list_of_int = isinstance(each_cell, list) and all(
-                            isinstance(x, int) for x in each_cell
-                        )
+                        is_list_of_int = isinstance(each_cell, list) and all(isinstance(x, int) for x in each_cell)
                         is_list_of_str = is_a_list_of_str(each_cell)
                         if self.is_token_classification():
                             assert is_list_of_str, (
                                 "For the token-classification task, the input column needs to be a list of string,"
                                 "instead of string, e.g., ['EU', 'rejects','German', 'call','to','boycott','British','lamb','.',].",
                                 "For more examples, please refer to test/nlp/test_autohf_tokenclassification.py",
                             )
@@ -218,52 +198,42 @@
             (
                 automl._X_train_all,
                 automl._y_train_all,
             ) = automl._transformer.fit_transform(X, y, self)
             automl._label_transformer = automl._transformer.label_transformer
             if self.is_token_classification():
                 if hasattr(automl._label_transformer, "label_list"):
-                    state.fit_kwargs.update(
-                        {"label_list": automl._label_transformer.label_list}
-                    )
+                    state.fit_kwargs.update({"label_list": automl._label_transformer.label_list})
                 elif "label_list" not in state.fit_kwargs:
                     for each_fit_kwargs in state.fit_kwargs_by_estimator.values():
                         assert (
                             "label_list" in each_fit_kwargs
                         ), "For the token-classification task, you must either (1) pass token labels; or (2) pass id labels and the label list. "
                         "Please refer to the documentation for more details: https://microsoft.github.io/FLAML/docs/Examples/AutoML-NLP#a-simple-token-classification-example"
             automl._feature_names_in_ = (
-                automl._X_train_all.columns.to_list()
-                if hasattr(automl._X_train_all, "columns")
-                else None
+                automl._X_train_all.columns.to_list() if hasattr(automl._X_train_all, "columns") else None
             )
 
         automl._sample_weight_full = state.fit_kwargs.get(
             "sample_weight"
         )  # NOTE: _validate_data is before kwargs is updated to fit_kwargs_by_estimator
         if X_val is not None and y_val is not None:
-            assert isinstance(
-                X_val, (np.ndarray, pd.DataFrame, psDataFrame)
-            ) or issparse(X_train_all), (
+            assert isinstance(X_val, (np.ndarray, pd.DataFrame, psDataFrame)) or issparse(X_train_all), (
                 "X_val must be None, a numpy array, a pandas dataframe, "
                 "a Scipy sparse matrix or a pyspark.pandas dataframe."
             )
             assert isinstance(y_val, (np.ndarray, pd.Series, psSeries)), (
-                "y_val must be None, a numpy array, a pandas series "
-                "or a pyspark.pandas series."
+                "y_val must be None, a numpy array, a pandas series " "or a pyspark.pandas series."
             )
             assert X_val.size != 0 and y_val.size != 0, (
-                "Validation data are expected to be nonempty. "
-                "Use None for X_val and y_val if no validation data."
+                "Validation data are expected to be nonempty. " "Use None for X_val and y_val if no validation data."
             )
             if isinstance(y_val, np.ndarray):
                 y_val = y_val.flatten()
-            assert (
-                X_val.shape[0] == y_val.shape[0]
-            ), "# rows in X_val must match length of y_val."
+            assert X_val.shape[0] == y_val.shape[0], "# rows in X_val must match length of y_val."
             if automl._transformer:
                 state.X_val = automl._transformer.transform(X_val)
             else:
                 state.X_val = X_val
             # If it's NLG_TASKS, y_val is a pandas series containing the output sequence tokens,
             # so we cannot use label_transformer.transform to process it
             if automl._label_transformer:
@@ -272,21 +242,17 @@
                 state.y_val = y_val
         else:
             state.X_val = state.y_val = None
 
         if groups is not None and len(groups) != automl._nrow:
             # groups is given as group counts
             state.groups = np.concatenate([[i] * c for i, c in enumerate(groups)])
-            assert (
-                len(state.groups) == automl._nrow
-            ), "the sum of group counts must match the number of examples"
+            assert len(state.groups) == automl._nrow, "the sum of group counts must match the number of examples"
             state.groups_val = (
-                np.concatenate([[i] * c for i, c in enumerate(groups_val)])
-                if groups_val is not None
-                else None
+                np.concatenate([[i] * c for i, c in enumerate(groups_val)]) if groups_val is not None else None
             )
         else:
             state.groups_val = groups_val
             state.groups = groups
 
     @staticmethod
     def _validate_ts_data(
@@ -341,19 +307,15 @@
     @staticmethod
     def _split_pyspark(state, X_train_all, y_train_all, split_ratio, stratify=None):
         # TODO: optimize this
         set_option("compute.ops_on_diff_frames", True)
         if not isinstance(y_train_all, (psDataFrame, psSeries)):
             raise ValueError("y_train_all must be a pyspark.pandas dataframe or series")
         df_all_in_one = X_train_all.join(y_train_all)
-        stratify_column = (
-            y_train_all.name
-            if isinstance(y_train_all, psSeries)
-            else y_train_all.columns[0]
-        )
+        stratify_column = y_train_all.name if isinstance(y_train_all, psSeries) else y_train_all.columns[0]
         ret_sample_weight = False
         if (
             "sample_weight" in state.fit_kwargs
         ):  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
             # fit_kwargs["sample_weight"] is an numpy array
             ps_sample_weight = ps.DataFrame(
                 state.fit_kwargs["sample_weight"],
@@ -363,17 +325,15 @@
             ret_sample_weight = True
         df_all_train, df_all_val = train_test_split_pyspark(
             df_all_in_one,
             None if stratify is None else stratify_column,
             test_fraction=split_ratio,
             seed=RANDOM_SEED,
         )
-        columns_to_drop = [
-            c for c in df_all_train.columns if c in [stratify_column, "sample_weight"]
-        ]
+        columns_to_drop = [c for c in df_all_train.columns if c in [stratify_column, "sample_weight"]]
         X_train = df_all_train.drop(columns_to_drop)
         X_val = df_all_val.drop(columns_to_drop)
         y_train = df_all_train[stratify_column]
         y_val = df_all_val[stratify_column]
 
         if ret_sample_weight:
             return (
@@ -383,25 +343,21 @@
                 y_val,
                 df_all_train["sample_weight"],
                 df_all_val["sample_weight"],
             )
         return X_train, X_val, y_train, y_val
 
     @staticmethod
-    def _train_test_split(
-        state, X, y, first=None, rest=None, split_ratio=0.2, stratify=None
-    ):
+    def _train_test_split(state, X, y, first=None, rest=None, split_ratio=0.2, stratify=None):
         condition_type = isinstance(X, (psDataFrame, psSeries))
         # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
         condition_param = "sample_weight" in state.fit_kwargs
         if not condition_type and condition_param:
             sample_weight = (
-                state.fit_kwargs["sample_weight"]
-                if rest is None
-                else state.fit_kwargs["sample_weight"][rest]
+                state.fit_kwargs["sample_weight"] if rest is None else state.fit_kwargs["sample_weight"][rest]
             )
             (
                 X_train,
                 X_val,
                 y_train,
                 y_val,
                 weight_train,
@@ -444,17 +400,15 @@
                 weight1 = state.fit_kwargs["sample_weight"][first]
                 state.weight_val = concat(weight1, weight_val)
                 state.fit_kwargs["sample_weight"] = concat(weight1, weight_train)
             else:
                 state.weight_val = weight_val
                 state.fit_kwargs["sample_weight"] = weight_train
         else:
-            X_train, X_val, y_train, y_val = GenericTask._split_pyspark(
-                state, X, y, split_ratio, stratify
-            )
+            X_train, X_val, y_train, y_val = GenericTask._split_pyspark(state, X, y, split_ratio, stratify)
         return X_train, X_val, y_train, y_val
 
     def prepare_data(
         self,
         state,
         X_train_all,
         y_train_all,
@@ -494,29 +448,21 @@
             rare_label, rare_counts = label_set[rare], counts[rare]
             for i, label in enumerate(rare_label.tolist()):
                 count = rare_count = rare_counts[i]
                 rare_index = y_train_all == label
                 n = len(y_train_all)
                 while count < rare_threshld:
                     if data_is_df:
-                        X_train_all = concat(
-                            X_train_all, X_train_all.iloc[:n].loc[rare_index]
-                        )
+                        X_train_all = concat(X_train_all, X_train_all.iloc[:n].loc[rare_index])
                     else:
-                        X_train_all = concat(
-                            X_train_all, X_train_all[:n][rare_index, :]
-                        )
+                        X_train_all = concat(X_train_all, X_train_all[:n][rare_index, :])
                     if isinstance(y_train_all, (pd.Series, psSeries)):
-                        y_train_all = concat(
-                            y_train_all, y_train_all.iloc[:n].loc[rare_index]
-                        )
+                        y_train_all = concat(y_train_all, y_train_all.iloc[:n].loc[rare_index])
                     else:
-                        y_train_all = np.concatenate(
-                            [y_train_all, y_train_all[:n][rare_index]]
-                        )
+                        y_train_all = np.concatenate([y_train_all, y_train_all[:n][rare_index]])
                     count += rare_count
                 logger.info(f"class {label} augmented from {rare_count} to {count}")
         SHUFFLE_SPLIT_TYPES = ["uniform", "stratified"]
         if is_spark_dataframe:
             # no need to shuffle pyspark dataframe
             pass
         elif split_type in SHUFFLE_SPLIT_TYPES:
@@ -531,17 +477,15 @@
                     "sample_weight"
                 ] = (
                     state.sample_weight_all
                 )  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
                 if isinstance(state.sample_weight_all, pd.Series):
                     state.sample_weight_all.reset_index(drop=True, inplace=True)
             else:
-                X_train_all, y_train_all = shuffle(
-                    X_train_all, y_train_all, random_state=RANDOM_SEED
-                )
+                X_train_all, y_train_all = shuffle(X_train_all, y_train_all, random_state=RANDOM_SEED)
             if data_is_df:
                 X_train_all.reset_index(drop=True, inplace=True)
             if isinstance(y_train_all, pd.Series):
                 y_train_all.reset_index(drop=True, inplace=True)
 
         X_train, y_train = X_train_all, y_train_all
         state.groups_all = state.groups
@@ -565,29 +509,21 @@
                             if isinstance(y_train_all, psSeries)
                             else y_train_all
                         )
                         y_train_all[ids] = X_train_all[ids]
                         X_train_all = X_train_all.sort_values(ids)
                         y_train_all = y_train_all.sort_values(ids)
                         training_cutoff = X_train_all["time_idx"].max() - period
-                        X_train = X_train_all[
-                            X_train_all["time_idx"] <= training_cutoff
-                        ]
-                        y_train = y_train_all[
-                            y_train_all["time_idx"] <= training_cutoff
-                        ].drop(columns=ids)
+                        X_train = X_train_all[X_train_all["time_idx"] <= training_cutoff]
+                        y_train = y_train_all[y_train_all["time_idx"] <= training_cutoff].drop(columns=ids)
                         X_val = X_train_all[X_train_all["time_idx"] > training_cutoff]
-                        y_val = y_train_all[
-                            y_train_all["time_idx"] > training_cutoff
-                        ].drop(columns=ids)
+                        y_val = y_train_all[y_train_all["time_idx"] > training_cutoff].drop(columns=ids)
                     else:
                         num_samples = X_train_all.shape[0]
-                        assert (
-                            period < num_samples
-                        ), f"period={period}>#examples={num_samples}"
+                        assert period < num_samples, f"period={period}>#examples={num_samples}"
                         split_idx = num_samples - period
                         X_train = X_train_all[:split_idx]
                         y_train = y_train_all[:split_idx]
                         X_val = X_train_all[split_idx:]
                         y_val = y_train_all[split_idx:]
                 else:
                     is_sample_weight = "sample_weight" in state.fit_kwargs
@@ -623,28 +559,22 @@
                             X_val,
                             y_train,
                             y_val,
                             state.fit_kwargs[
                                 "sample_weight"
                             ],  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
                             state.weight_val,
-                        ) = self._split_pyspark(
-                            state, X_train_all, y_train_all, split_ratio
-                        )
+                        ) = self._split_pyspark(state, X_train_all, y_train_all, split_ratio)
                     else:
                         X_train, X_val, y_train, y_val = self._split_pyspark(
                             state, X_train_all, y_train_all, split_ratio
                         )
             elif split_type == "group":
-                gss = GroupShuffleSplit(
-                    n_splits=1, test_size=split_ratio, random_state=RANDOM_SEED
-                )
-                for train_idx, val_idx in gss.split(
-                    X_train_all, y_train_all, state.groups_all
-                ):
+                gss = GroupShuffleSplit(n_splits=1, test_size=split_ratio, random_state=RANDOM_SEED)
+                for train_idx, val_idx in gss.split(X_train_all, y_train_all, state.groups_all):
                     if data_is_df:
                         X_train = X_train_all.iloc[train_idx]
                         X_val = X_train_all.iloc[val_idx]
                     else:
                         X_train, X_val = X_train_all[train_idx], X_train_all[val_idx]
                     y_train, y_val = y_train_all[train_idx], y_train_all[val_idx]
                     state.groups = state.groups_all[train_idx]
@@ -670,25 +600,17 @@
                     else y_train_all.iloc[rest]
                 )
                 stratify = y_rest if split_type == "stratified" else None
                 X_train, X_val, y_train, y_val = self._train_test_split(
                     state, X_rest, y_rest, first, rest, split_ratio, stratify
                 )
                 X_train = concat(X_first, X_train)
-                y_train = (
-                    concat(label_set, y_train)
-                    if data_is_df
-                    else np.concatenate([label_set, y_train])
-                )
+                y_train = concat(label_set, y_train) if data_is_df else np.concatenate([label_set, y_train])
                 X_val = concat(X_first, X_val)
-                y_val = (
-                    concat(label_set, y_val)
-                    if data_is_df
-                    else np.concatenate([label_set, y_val])
-                )
+                y_val = concat(label_set, y_val) if data_is_df else np.concatenate([label_set, y_val])
             elif self.is_regression():
                 X_train, X_val, y_train, y_val = self._train_test_split(
                     state, X_train_all, y_train_all, split_ratio=split_ratio
                 )
         state.data_size = X_train.shape
         state.X_train, state.y_train = X_train, y_train
         state.X_val, state.y_val = X_val, y_val
@@ -696,34 +618,29 @@
         state.y_train_all = y_train_all
         y_train_all_size = y_train_all.size
         if eval_method == "holdout":
             state.kf = None
             return
         if split_type == "group":
             # logger.info("Using GroupKFold")
-            assert (
-                len(state.groups_all) == y_train_all_size
-            ), "the length of groups must match the number of examples"
+            assert len(state.groups_all) == y_train_all_size, "the length of groups must match the number of examples"
             assert (
                 len_labels(state.groups_all) >= n_splits
             ), "the number of groups must be equal or larger than n_splits"
             state.kf = GroupKFold(n_splits)
         elif split_type == "stratified":
             # logger.info("Using StratifiedKFold")
             assert y_train_all_size >= n_splits, (
-                f"{n_splits}-fold cross validation"
-                f" requires input data with at least {n_splits} examples."
+                f"{n_splits}-fold cross validation" f" requires input data with at least {n_splits} examples."
             )
             assert y_train_all_size >= 2 * n_splits, (
                 f"{n_splits}-fold cross validation with metric=r2 "
                 f"requires input data with at least {n_splits*2} examples."
             )
-            state.kf = RepeatedStratifiedKFold(
-                n_splits=n_splits, n_repeats=1, random_state=RANDOM_SEED
-            )
+            state.kf = RepeatedStratifiedKFold(n_splits=n_splits, n_repeats=1, random_state=RANDOM_SEED)
         elif split_type == "time":
             # logger.info("Using TimeSeriesSplit")
             if self.is_ts_forecast() and not self.is_ts_forecastpanel():
                 period = state.fit_kwargs[
                     "period"
                 ]  # NOTE: _prepare_data is before kwargs is updated to fit_kwargs_by_estimator
                 if period * (n_splits + 1) > y_train_all_size:
@@ -731,28 +648,22 @@
                     assert n_splits >= 2, (
                         f"cross validation for forecasting period={period}"
                         f" requires input data with at least {3 * period} examples."
                     )
                     logger.info(f"Using nsplits={n_splits} due to data size limit.")
                 state.kf = TimeSeriesSplit(n_splits=n_splits, test_size=period)
             elif self.is_ts_forecastpanel():
-                n_groups = len(
-                    X_train.groupby(state.fit_kwargs.get("group_ids")).size()
-                )
+                n_groups = len(X_train.groupby(state.fit_kwargs.get("group_ids")).size())
                 period = state.fit_kwargs.get("period")
-                state.kf = TimeSeriesSplit(
-                    n_splits=n_splits, test_size=period * n_groups
-                )
+                state.kf = TimeSeriesSplit(n_splits=n_splits, test_size=period * n_groups)
             else:
                 state.kf = TimeSeriesSplit(n_splits=n_splits)
         elif isinstance(split_type, str):
             # logger.info("Using RepeatedKFold")
-            state.kf = RepeatedKFold(
-                n_splits=n_splits, n_repeats=1, random_state=RANDOM_SEED
-            )
+            state.kf = RepeatedKFold(n_splits=n_splits, n_repeats=1, random_state=RANDOM_SEED)
         else:
             # logger.info("Using splitter object")
             state.kf = split_type
         if isinstance(state.kf, (GroupKFold, StratifiedGroupKFold)):
             # self._split_type is either "group", a GroupKFold object, or a StratifiedGroupKFold object
             state.kf.groups = state.groups_all
 
@@ -786,19 +697,15 @@
                 assert isinstance(
                     fit_kwargs.get("group_ids"), list
                 ), f"missing a required List[str] 'group_ids' for '{TS_FORECASTPANEL}' task."
             return "time"
 
         elif self.is_classification():
             assert split_type in ["auto", "stratified", "uniform", "time", "group"]
-            return (
-                split_type
-                if split_type != "auto"
-                else groups is None and "stratified" or "group"
-            )
+            return split_type if split_type != "auto" else groups is None and "stratified" or "group"
 
         elif self.is_regression():
             assert split_type in ["auto", "uniform", "time", "group"]
             return split_type if split_type != "auto" else "uniform"
 
         elif self.is_rank():
             assert groups is not None, "groups must be specified for ranking task."
@@ -821,17 +728,15 @@
                             if isinstance(X[0], List)
                             else (transformer._str_columns[idx], [X[idx]])
                             for idx in range(len(X))
                         ]
                     )
                 )
             except IndexError:
-                raise IndexError(
-                    "Test data contains more columns than training data, exiting"
-                )
+                raise IndexError("Test data contains more columns than training data, exiting")
         elif isinstance(X, int):
             return X
         elif isinstance(X, psDataFrame):
             return X
         elif issparse(X):
             X = X.tocsr()
         if self.is_ts_forecast():
@@ -868,34 +773,30 @@
         n = kf.get_n_splits()
         rng = np.random.RandomState(2020)
         budget_per_train = budget and budget / n
         groups = None
         if self.is_classification():
             labels = _, labels = len_labels(y_train_all, return_labels=True)
         else:
-            labels = fit_kwargs.get(
-                "label_list"
-            )  # pass the label list on to compute the evaluation metric
+            labels = fit_kwargs.get("label_list")  # pass the label list on to compute the evaluation metric
         if "sample_weight" in fit_kwargs:
             weight = fit_kwargs["sample_weight"]
             weight_val = None
         else:
             weight = weight_val = None
 
         is_spark_dataframe = isinstance(X_train_all, (psDataFrame, psSeries))
         if is_spark_dataframe:
             dataframe = X_train_all.join(y_train_all)
             if weight is not None:
                 dataframe = dataframe.join(weight)
             if isinstance(kf, (GroupKFold, StratifiedGroupKFold)):
                 groups = kf.groups
                 dataframe = dataframe.join(groups)
-            kf = spark_kFold(
-                dataframe, nFolds=n, foldCol=groups.name if groups is not None else ""
-            )
+            kf = spark_kFold(dataframe, nFolds=n, foldCol=groups.name if groups is not None else "")
             shuffle = False
         else:
             X_train_split, y_train_split = X_train_all, y_train_all
             shuffle = getattr(kf, "shuffle", not self.is_ts_forecast())
             if isinstance(kf, RepeatedStratifiedKFold):
                 kf = kf.split(X_train_split, y_train_split)
             elif isinstance(kf, (GroupKFold, StratifiedGroupKFold)):
@@ -930,23 +831,17 @@
                 if weight is not None:
                     fit_kwargs["sample_weight"], weight_val = (
                         weight[train_index],
                         weight[val_index],
                     )
                 if groups is not None:
                     fit_kwargs["groups"] = (
-                        groups[train_index]
-                        if isinstance(groups, np.ndarray)
-                        else groups.iloc[train_index]
-                    )
-                    groups_val = (
-                        groups[val_index]
-                        if isinstance(groups, np.ndarray)
-                        else groups.iloc[val_index]
+                        groups[train_index] if isinstance(groups, np.ndarray) else groups.iloc[train_index]
                     )
+                    groups_val = groups[val_index] if isinstance(groups, np.ndarray) else groups.iloc[val_index]
                 else:
                     groups_val = None
 
             estimator.cleanup()
             val_loss_i, metric_i, train_time_i, pred_time_i = get_val_loss(
                 config,
                 estimator,
@@ -979,39 +874,33 @@
             if budget and time.time() - start_time >= budget:
                 break
         val_loss, metric = cv_score_agg_func(val_loss_folds, log_metric_folds)
         n = total_fold_num
         pred_time /= n
         return val_loss, metric, train_time, pred_time
 
-    def default_estimator_list(
-        self, estimator_list: List[str], is_spark_dataframe: bool = False
-    ) -> List[str]:
+    def default_estimator_list(self, estimator_list: List[str], is_spark_dataframe: bool = False) -> List[str]:
         if "auto" != estimator_list:
             n_estimators = len(estimator_list)
             if is_spark_dataframe:
                 # For spark dataframe, only estimators ending with '_spark' are supported
-                estimator_list = [
-                    est for est in estimator_list if est.endswith("_spark")
-                ]
+                estimator_list = [est for est in estimator_list if est.endswith("_spark")]
                 if len(estimator_list) == 0:
                     raise ValueError(
                         "Spark dataframes only support estimator names ending with `_spark`. Non-supported "
                         "estimators are removed. No estimator is left."
                     )
                 elif n_estimators != len(estimator_list):
                     logger.warning(
                         "Spark dataframes only support estimator names ending with `_spark`. Non-supported "
                         "estimators are removed."
                     )
             else:
                 # For non-spark dataframe, only estimators not ending with '_spark' are supported
-                estimator_list = [
-                    est for est in estimator_list if not est.endswith("_spark")
-                ]
+                estimator_list = [est for est in estimator_list if not est.endswith("_spark")]
                 if len(estimator_list) == 0:
                     raise ValueError(
                         "Non-spark dataframes only support estimator names not ending with `_spark`. Non-supported "
                         "estimators are removed. No estimator is left."
                     )
                 elif n_estimators != len(estimator_list):
                     logger.warning(
@@ -1065,19 +954,15 @@
                         estimator_list += ["arima", "sarimax", "holt-winters"]
             elif not self.is_regression():
                 estimator_list += ["lrl1"]
 
         estimator_list = [
             est
             for est in estimator_list
-            if (
-                est.endswith("_spark")
-                if is_spark_dataframe
-                else not est.endswith("_spark")
-            )
+            if (est.endswith("_spark") if is_spark_dataframe else not est.endswith("_spark"))
         ]
         return estimator_list
 
     def default_metric(self, metric: str) -> str:
         if "auto" != metric:
             return metric
```

### Comparing `FLAML-1.2.0/flaml/automl/task/task.py` & `FLAML-1.2.1/flaml/automl/task/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,17 +329,15 @@
         return self.name in REGRESSION
 
     def __eq__(self, other: str) -> bool:
         """For backward compatibility with all the string comparisons to task"""
         return self.name == other
 
     @classmethod
-    def estimator_class_from_str(
-        cls, estimator_name: str
-    ) -> "flaml.automl.ml.BaseEstimator":
+    def estimator_class_from_str(cls, estimator_name: str) -> "flaml.automl.ml.BaseEstimator":
         """Determine the estimator class corresponding to the provided name.
 
         Args:
             estimator_name: Name of the desired estimator.
 
         Returns:
             The estimator class corresponding to the provided name.
```

### Comparing `FLAML-1.2.0/flaml/automl/training_log.py` & `FLAML-1.2.1/flaml/automl/training_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,17 +107,15 @@
         self.file.write("\n")
         self.file.flush()
 
     def checkpoint(self):
         if self.file is None:
             raise IOError("Call open() to open the output file first.")
         if self.current_best_loss_record_id is None:
-            logger.warning(
-                "flaml.training_log: checkpoint() called before any record is written, skipped."
-            )
+            logger.warning("flaml.training_log: checkpoint() called before any record is written, skipped.")
             return
         record = TrainingLogCheckPoint(self.current_best_loss_record_id)
         record.dump(self.file)
         self.file.write("\n")
         self.file.flush()
 
     def close(self):
```

### Comparing `FLAML-1.2.0/flaml/automl/utils.py` & `FLAML-1.2.1/flaml/automl/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/all/binary.json` & `FLAML-1.2.1/flaml/default/all/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/all/multiclass.json` & `FLAML-1.2.1/flaml/default/all/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/all/regression.json` & `FLAML-1.2.1/flaml/default/all/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/estimator.py` & `FLAML-1.2.1/flaml/default/estimator.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,39 +71,32 @@
             if alternatives:
                 for alternative in alternatives:
                     if self._params.get(alternative[0]) == alternative[1]:
                         estimator_name = alternative[2]
                         break
             estimator_name = (
                 "choose_xgb"
-                if (
-                    estimator_name == "xgb_limitdepth"
-                    and "max_depth" not in self._params
-                )
+                if (estimator_name == "xgb_limitdepth" and "max_depth" not in self._params)
                 else estimator_name
             )
             (
                 hyperparams,
                 estimator_class,
                 X_transformed,
                 y_transformed,
                 self._feature_transformer,
                 self._label_transformer,
-            ) = preprocess_and_suggest_hyperparams(
-                task, X, y, estimator_name, self._default_location
-            )
+            ) = preprocess_and_suggest_hyperparams(task, X, y, estimator_name, self._default_location)
             assert estimator_class == super_class
             hyperparams.update(self._params)
             return hyperparams, estimator_name, X_transformed, y_transformed
 
         @wraps(super_class.fit)
         def fit(self, X, y, *args, **params):
-            hyperparams, estimator_name, X, y_transformed = self.suggest_hyperparams(
-                X, y
-            )
+            hyperparams, estimator_name, X, y_transformed = self.suggest_hyperparams(X, y)
             self.set_params(**hyperparams)
             if self._label_transformer and estimator_name in [
                 "rf",
                 "extra_tree",
                 "xgboost",
                 "xgb_limitdepth",
                 "choose_xgb",
@@ -146,34 +139,24 @@
                 return y_pred
 
     EstimatorClass.__doc__ += " " + super_class.__doc__
     EstimatorClass.__name__ = super_class.__name__
     return EstimatorClass
 
 
-RandomForestRegressor = flamlize_estimator(
-    ensemble.RandomForestRegressor, "rf", "regression"
-)
-RandomForestClassifier = flamlize_estimator(
-    ensemble.RandomForestClassifier, "rf", "classification"
-)
-ExtraTreesRegressor = flamlize_estimator(
-    ensemble.ExtraTreesRegressor, "extra_tree", "regression"
-)
-ExtraTreesClassifier = flamlize_estimator(
-    ensemble.ExtraTreesClassifier, "extra_tree", "classification"
-)
+RandomForestRegressor = flamlize_estimator(ensemble.RandomForestRegressor, "rf", "regression")
+RandomForestClassifier = flamlize_estimator(ensemble.RandomForestClassifier, "rf", "classification")
+ExtraTreesRegressor = flamlize_estimator(ensemble.ExtraTreesRegressor, "extra_tree", "regression")
+ExtraTreesClassifier = flamlize_estimator(ensemble.ExtraTreesClassifier, "extra_tree", "classification")
 
 try:
     import lightgbm
 
     LGBMRegressor = flamlize_estimator(lightgbm.LGBMRegressor, "lgbm", "regression")
-    LGBMClassifier = flamlize_estimator(
-        lightgbm.LGBMClassifier, "lgbm", "classification"
-    )
+    LGBMClassifier = flamlize_estimator(lightgbm.LGBMClassifier, "lgbm", "classification")
 except ImportError:
     pass
 
 try:
     import xgboost
 
     XGBRegressor = flamlize_estimator(
```

### Comparing `FLAML-1.2.0/flaml/default/extra_tree/binary.json` & `FLAML-1.2.1/flaml/default/extra_tree/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/extra_tree/multiclass.json` & `FLAML-1.2.1/flaml/default/extra_tree/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/extra_tree/regression.json` & `FLAML-1.2.1/flaml/default/extra_tree/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/greedy.py` & `FLAML-1.2.1/flaml/default/greedy.py`

 * *Files 16% similar despite different names*

```diff
@@ -67,31 +67,24 @@
     eps = 1e-5
     while True:
         candidates = [configs + [d] for d in all_configs.difference(configs)]
         losses, avg_regret = tuple(zip(*(loss(x) for x in candidates)))
         sorted_losses = np.sort(losses)
         if sorted_losses[1] - sorted_losses[0] < eps:
             minloss = np.nanmin(losses)
-            print(
-                f"tie detected at loss = {sorted_losses[0]}, using alternative metric."
-            )
+            print(f"tie detected at loss = {sorted_losses[0]}, using alternative metric.")
             tied = np.flatnonzero(losses - minloss < eps)
             losses = [(avg_regret[i], i) for i in tied]
             minloss, ind = min(losses)
             if minloss > prev - eps:
-                print(
-                    f"May be overfitting at k = {i + 1}, current = {minloss:.5f}, "
-                    f"prev = {prev:.5f}. Stopping."
-                )
+                print(f"May be overfitting at k = {i + 1}, current = {minloss:.5f}, " f"prev = {prev:.5f}. Stopping.")
                 break
             configs = candidates[ind]
             prev = minloss
         else:
             configs = candidates[np.nanargmin(losses)]
         i += 1
         if sorted_losses[0] <= eps:
-            print(
-                f"Reached target regret bound of {regret_bound}! k = {i}. Declining to pick further!"
-            )
+            print(f"Reached target regret bound of {regret_bound}! k = {i}. Declining to pick further!")
             break
 
     return configs
```

### Comparing `FLAML-1.2.0/flaml/default/lgbm/binary.json` & `FLAML-1.2.1/flaml/default/lgbm/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/lgbm/multiclass.json` & `FLAML-1.2.1/flaml/default/lgbm/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/lgbm/regression.json` & `FLAML-1.2.1/flaml/default/lgbm/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/portfolio.py` & `FLAML-1.2.1/flaml/default/portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,30 +105,26 @@
     output_file = Path(output_file)
     # delete if exists
     try:
         output_file.unlink()
     except FileNotFoundError:
         pass
 
-    meta_features_norm, preferences, proc = config_predictor_tuple(
-        regret.columns, configs, meta_features, regret
-    )
+    meta_features_norm, preferences, proc = config_predictor_tuple(regret.columns, configs, meta_features, regret)
     portfolio = [load_json(config_path.joinpath(m + ".json")) for m in configs]
     regret = regret.loc[configs]
 
     meta_predictor = {
         "version": __version__,
         "meta_feature_names": list(meta_features.columns),
         "portfolio": portfolio,
         "preprocessing": proc,
         "neighbors": [
             {"features": tuple(x), "choice": _filter(preferences[y], regret[y])}
-            for x, y in zip(
-                meta_features_norm.to_records(index=False), preferences.columns
-            )
+            for x, y in zip(meta_features_norm.to_records(index=False), preferences.columns)
         ],
         "configsource": list(configs),
     }
 
     with open(output_file, "w+") as f:
         json.dump(meta_predictor, f, indent=4)
     return meta_predictor
@@ -160,17 +156,15 @@
 #     best = regrets.min()
 #     if best > regret_bound:
 #         print(tasks[i], "best_regret", best, "task", regrets.idxmin())
 
 
 def main():
     parser = argparse.ArgumentParser(description="Build a portfolio.")
-    parser.add_argument(
-        "--strategy", help="One of {greedy, greedy-feedback}", default="greedy"
-    )
+    parser.add_argument("--strategy", help="One of {greedy, greedy-feedback}", default="greedy")
     parser.add_argument("--input", help="Input path")
     parser.add_argument("--metafeatures", help="CSV of task metafeatures")
     parser.add_argument("--exclude", help="One task name to exclude (for LOO purposes)")
     parser.add_argument("--output", help="Location to write portfolio JSON")
     parser.add_argument("--task", help="Task to merge portfolios", default="binary")
     parser.add_argument(
         "--estimator",
@@ -184,45 +178,37 @@
     if args.exclude:
         meta_features.drop(args.exclude, inplace=True)
 
     baseline_best = None
     all_results = None
     for estimator in args.estimator:
         # produce regret
-        all, baseline = load_result(
-            f"{args.input}/{estimator}/results.csv", args.task, "result"
-        )
+        all, baseline = load_result(f"{args.input}/{estimator}/results.csv", args.task, "result")
         regret = build_regret(all, baseline)
         regret = regret.replace(np.inf, np.nan).dropna(axis=1, how="all")
 
         if args.exclude:
             regret = regret.loc[[i for i in regret.index if args.exclude not in i]]
             regret = regret[[c for c in regret.columns if args.exclude not in c]]
 
-        print(
-            f"Regret matrix complete: {100 * regret.count().sum() / regret.shape[0] / regret.shape[1]}%"
-        )
+        print(f"Regret matrix complete: {100 * regret.count().sum() / regret.shape[0] / regret.shape[1]}%")
         print(f"Num models considered: {regret.shape[0]}")
 
         configs = build_portfolio(meta_features, regret, args.strategy)
         meta_predictor = serialize(
             configs,
             regret,
             meta_features,
             f"{args.output}/{estimator}/{args.task}.json",
             Path(f"{args.input}/{estimator}"),
         )
         configsource = meta_predictor["configsource"]
         all = all.loc[configsource]
         all.rename({x: f"{estimator}/{x}" for x in regret.index.values}, inplace=True)
-        baseline_best = (
-            baseline
-            if baseline_best is None
-            else pd.DataFrame({0: baseline_best, 1: baseline}).max(1)
-        )
+        baseline_best = baseline if baseline_best is None else pd.DataFrame({0: baseline_best, 1: baseline}).max(1)
         all_results = all if all_results is None else pd.concat([all_results, all])
         # analyze(regret, meta_predictor)
     regrets = build_regret(all_results, baseline_best)
     if len(args.estimator) > 1:
         meta_predictor = serialize(
             regrets.index,
             regrets,
```

### Comparing `FLAML-1.2.0/flaml/default/regret.py` & `FLAML-1.2.1/flaml/default/regret.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,33 +14,25 @@
 
 def load_result(filename, task_type, metric):
     df = pd.read_csv(filename)
     df = df.loc[
         (df[metric].notnull()) & (df.type == task_type),
         ["task", "fold", "params", metric],
     ]
-    df["params"] = df["params"].apply(
-        lambda x: path.splitext(path.basename(eval(x)["_modeljson"]))[0]
-    )
-    baseline = (
-        df.loc[df["task"] == df["params"], ["task", metric]]
-        .groupby("task")
-        .mean()[metric]
-    )
+    df["params"] = df["params"].apply(lambda x: path.splitext(path.basename(eval(x)["_modeljson"]))[0])
+    baseline = df.loc[df["task"] == df["params"], ["task", metric]].groupby("task").mean()[metric]
     df = df.pivot_table(index="params", columns="task", values=metric)
     return df, baseline
 
 
 def main():
     parser = argparse.ArgumentParser(description="Build a regret matrix.")
     parser.add_argument("--result_csv", help="File of experiment results")
     parser.add_argument("--task_type", help="Type of task")
-    parser.add_argument(
-        "--metric", help="Metric for calculating regret", default="result"
-    )
+    parser.add_argument("--metric", help="Metric for calculating regret", default="result")
     parser.add_argument("--output", help="Location to write regret CSV to")
     args = parser.parse_args()
 
     all, baseline = load_result(args.result_csv, args.task_type, args.metric)
     regret = build_regret(all, baseline)
     write_regret(regret, args.output)
```

### Comparing `FLAML-1.2.0/flaml/default/rf/binary.json` & `FLAML-1.2.1/flaml/default/rf/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/rf/multiclass.json` & `FLAML-1.2.1/flaml/default/rf/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/rf/regression.json` & `FLAML-1.2.1/flaml/default/rf/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/suggest.py` & `FLAML-1.2.1/flaml/default/suggest.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,18 +49,15 @@
             this_feature.append(n_feat)
         elif each_feature_name == "NumberOfClasses":
             this_feature.append(len_labels(y_train) if is_classification else 0)
         elif each_feature_name == "PercentageOfNumericFeatures":
             try:
                 # this feature is only supported for dataframe
                 this_feature.append(
-                    X_train.select_dtypes(
-                        include=[np.number, "float", "int", "long"]
-                    ).shape[1]
-                    / n_feat
+                    X_train.select_dtypes(include=[np.number, "float", "int", "long"]).shape[1] / n_feat
                 )
             except AttributeError:
                 # 'numpy.ndarray' object has no attribute 'select_dtypes'
                 this_feature.append(1)  # all features are numeric
         else:
             raise ValueError("Feature {} not implemented. ".format(each_feature_name))
 
@@ -75,17 +72,15 @@
         return predictor
     task = "multiclass" if task == "multi" else task  # TODO: multi -> multiclass?
     try:
         location = location or LOCATION
         with open(f"{location}/{estimator_name}/{task}.json", "r") as f:
             CONFIG_PREDICTORS[key] = predictor = json.load(f)
     except FileNotFoundError:
-        raise FileNotFoundError(
-            f"Portfolio has not been built for {estimator_name} on {task} task."
-        )
+        raise FileNotFoundError(f"Portfolio has not been built for {estimator_name} on {task} task.")
     return predictor
 
 
 def suggest_config(
     task,
     X,
     y,
@@ -95,36 +90,26 @@
     meta_feature_fn=meta_feature,
 ):
     """Suggest a list of configs for the given task and training data.
 
     The returned configs can be used as starting points for AutoML.fit().
     `FLAML_sample_size` is removed from the configs.
     """
-    task = (
-        get_classification_objective(len_labels(y))
-        if task == "classification" and y is not None
-        else task
-    )
+    task = get_classification_objective(len_labels(y)) if task == "classification" and y is not None else task
     predictor = (
         load_config_predictor(estimator_or_predictor, task, location)
         if isinstance(estimator_or_predictor, str)
         else estimator_or_predictor
     )
 
     older_version = "1.0.2"
     # TODO: update older_version when the newer code can no longer handle the older version json file
-    assert (
-        version_parse(__version__)
-        >= version_parse(predictor["version"])
-        >= version_parse(older_version)
-    )
+    assert version_parse(__version__) >= version_parse(predictor["version"]) >= version_parse(older_version)
     prep = predictor["preprocessing"]
-    feature = meta_feature_fn(
-        task, X_train=X, y_train=y, meta_feature_names=predictor["meta_feature_names"]
-    )
+    feature = meta_feature_fn(task, X_train=X, y_train=y, meta_feature_names=predictor["meta_feature_names"])
     feature = (np.array(feature) - np.array(prep["center"])) / np.array(prep["scale"])
     neighbors = predictor["neighbors"]
     nn = NearestNeighbors(n_neighbors=1)
     nn.fit([x["features"] for x in neighbors])
     dist, ind = nn.kneighbors(feature.reshape(1, -1), return_distance=True)
     logger.info(f"metafeature distance: {dist.item()}")
     ind = int(ind.item())
@@ -134,17 +119,15 @@
         if "hyperparameters" in config:
             hyperparams = config["hyperparameters"]
             if hyperparams and "FLAML_sample_size" in hyperparams:
                 hyperparams.pop("FLAML_sample_size")
     return configs
 
 
-def suggest_learner(
-    task, X, y, estimator_or_predictor="all", estimator_list=None, location=None
-):
+def suggest_learner(task, X, y, estimator_or_predictor="all", estimator_list=None, location=None):
     """Suggest best learner within estimator_list."""
     configs = suggest_config(task, X, y, estimator_or_predictor, location)
     if not estimator_list:
         return configs[0]["class"]
     for c in configs:
         if c["class"] in estimator_list:
             return c["class"]
@@ -189,17 +172,15 @@
         location: (Optional) A str of the location containing mined portfolio file.
             Only valid when the portfolio is a str, by default the location is flaml/default.
 
     Returns:
         hyperparams: A dict of the hyperparameter configurations.
         estiamtor_class: A class of the underlying estimator, e.g., lightgbm.LGBMClassifier.
     """
-    config = suggest_config(task, X, y, estimator_or_predictor, location=location, k=1)[
-        0
-    ]
+    config = suggest_config(task, X, y, estimator_or_predictor, location=location, k=1)[0]
     estimator = config["class"]
     model_class = get_estimator_class(task, estimator)
     hyperparams = config["hyperparameters"]
     model = model_class(task=task, **hyperparams)
     estimator_class = model.estimator_class
     hyperparams = hyperparams and model.params
     return hyperparams, estimator_class
@@ -275,17 +256,15 @@
         estimator_or_predictor = suggest_learner(
             task,
             X,
             y,
             estimator_list=["xgb_limitdepth", "xgboost"],
             location=location,
         )
-    config = suggest_config(task, X, y, estimator_or_predictor, location=location, k=1)[
-        0
-    ]
+    config = suggest_config(task, X, y, estimator_or_predictor, location=location, k=1)[0]
     estimator = config["class"]
     model_class = get_estimator_class(task, estimator)
     hyperparams = config["hyperparameters"]
     model = model_class(task=task, **hyperparams)
     if model.estimator_class is None:
         return hyperparams, model_class, X, y, None, None
     else:
```

### Comparing `FLAML-1.2.0/flaml/default/xgb_limitdepth/binary.json` & `FLAML-1.2.1/flaml/default/xgb_limitdepth/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/xgb_limitdepth/multiclass.json` & `FLAML-1.2.1/flaml/default/xgb_limitdepth/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/xgb_limitdepth/regression.json` & `FLAML-1.2.1/flaml/default/xgb_limitdepth/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/xgboost/binary.json` & `FLAML-1.2.1/flaml/default/xgboost/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/xgboost/multiclass.json` & `FLAML-1.2.1/flaml/default/xgboost/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/default/xgboost/regression.json` & `FLAML-1.2.1/flaml/default/xgboost/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/onlineml/autovw.py` & `FLAML-1.2.1/flaml/onlineml/autovw.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,20 +109,16 @@
 
     def _setup_trial_runner(self, vw_example):
         """Set up the _trial_runner based on one vw_example."""
         # setup the default search space for the namespace interaction hyperparameter
         search_space = self._search_space.copy()
         for k, v in self._search_space.items():
             if k == self.VW_INTERACTION_ARG_NAME and v == self.AUTOMATIC:
-                raw_namespaces = self.get_ns_feature_dim_from_vw_example(
-                    vw_example
-                ).keys()
-                search_space[k] = polynomial_expansion_set(
-                    init_monomials=set(raw_namespaces)
-                )
+                raw_namespaces = self.get_ns_feature_dim_from_vw_example(vw_example).keys()
+                search_space[k] = polynomial_expansion_set(init_monomials=set(raw_namespaces))
         # setup the init config based on the input _init_config and search space
         init_config = self._init_config.copy()
         for k, v in search_space.items():
             if k not in init_config.keys():
                 if isinstance(v, PolynomialExpansionSet):
                     init_config[k] = set()
                 elif not isinstance(v, Categorical) and not isinstance(v, Float):
@@ -154,18 +150,15 @@
             data_sample: one data example in vw format.
         """
         if self._trial_runner is None:
             self._setup_trial_runner(data_sample)
         self._best_trial = self._select_best_trial()
         self._y_predict = self._best_trial.predict(data_sample)
         # code for debugging purpose
-        if (
-            self._prediction_trial_id is None
-            or self._prediction_trial_id != self._best_trial.trial_id
-        ):
+        if self._prediction_trial_id is None or self._prediction_trial_id != self._best_trial.trial_id:
             self._prediction_trial_id = self._best_trial.trial_id
             logger.info(
                 "prediction trial id changed to %s at iter %s, resource used: %s",
                 self._prediction_trial_id,
                 self._iter,
                 self._best_trial.result.resource_used,
             )
@@ -179,42 +172,34 @@
                 update the vw model.
         """
         self._iter += 1
         self._trial_runner.step(data_sample, (self._y_predict, self._best_trial))
 
     def _select_best_trial(self):
         """Select a best trial from the running trials according to the _model_select_policy."""
-        best_score = (
-            float("+inf") if self._model_selection_mode == "min" else float("-inf")
-        )
+        best_score = float("+inf") if self._model_selection_mode == "min" else float("-inf")
         new_best_trial = None
         for trial in self._trial_runner.running_trials:
             if trial.result is not None and (
-                "threshold" not in self._model_select_policy
-                or trial.result.resource_used >= self.WARMSTART_NUM
+                "threshold" not in self._model_select_policy or trial.result.resource_used >= self.WARMSTART_NUM
             ):
                 score = trial.result.get_score(self._model_select_policy)
                 if ("min" == self._model_selection_mode and score < best_score) or (
                     "max" == self._model_selection_mode and score > best_score
                 ):
                     best_score = score
                     new_best_trial = trial
         if new_best_trial is not None:
-            logger.debug(
-                "best_trial resource used: %s", new_best_trial.result.resource_used
-            )
+            logger.debug("best_trial resource used: %s", new_best_trial.result.resource_used)
             return new_best_trial
         else:
             # This branch will be triggered when the resource consumption all trials are smaller
             # than the WARMSTART_NUM threshold. In this case, we will select the _best_trial
             # selected in the previous iteration.
-            if (
-                self._best_trial is not None
-                and self._best_trial.status == Trial.RUNNING
-            ):
+            if self._best_trial is not None and self._best_trial.status == Trial.RUNNING:
                 logger.debug("old best trial %s", self._best_trial.trial_id)
                 return self._best_trial
             else:
                 # this will be triggered in the first iteration or in the iteration where we want
                 # to select the trial from the previous iteration but that trial has been paused
                 # (i.e., self._best_trial.status != Trial.RUNNING) by the scheduler.
                 logger.debug(
```

### Comparing `FLAML-1.2.0/flaml/onlineml/trial.py` & `FLAML-1.2.1/flaml/onlineml/trial.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,30 +102,26 @@
         self._loss_avg = self._loss_avg * (
             self.observation_count / (self.observation_count + new_observation_count)
         ) + new_loss / (self.observation_count + new_observation_count)
         self.observation_count += new_observation_count
         self._loss_cb = self._update_loss_cb(bound_of_range, data_dimension)
         self._loss_queue.append(new_loss)
 
-    def _update_loss_cb(
-        self, bound_of_range, data_dim, bound_name="sample_complexity_bound"
-    ):
+    def _update_loss_cb(self, bound_of_range, data_dim, bound_name="sample_complexity_bound"):
         """Calculate the coefficient of the confidence bound."""
         if bound_name == "sample_complexity_bound":
             # set the coefficient in the loss bound
             if "mae" in self.result_type_name:
                 coef = self._cb_coef * bound_of_range
             else:
                 coef = 0.001 * bound_of_range
 
             comp_F = math.sqrt(data_dim)
             n = self.observation_count
-            return (
-                coef * comp_F * math.sqrt((np.log10(n / OnlineResult.prob_delta)) / n)
-            )
+            return coef * comp_F * math.sqrt((np.log10(n / OnlineResult.prob_delta)) / n)
         else:
             raise NotImplementedError
 
     @property
     def result_type_name(self):
         return self._result_type_name
 
@@ -143,19 +139,15 @@
 
     @property
     def loss_ucb(self):
         return min(self._loss_avg + self._loss_cb, OnlineResult.LOSS_MAX)
 
     @property
     def loss_avg_recent(self):
-        return (
-            sum(self._loss_queue) / len(self._loss_queue)
-            if len(self._loss_queue) != 0
-            else self._init_loss
-        )
+        return sum(self._loss_queue) / len(self._loss_queue) if len(self._loss_queue) != 0 else self._init_loss
 
     def get_score(self, score_name, cb_ratio=1):
         if "lcb" in score_name:
             return max(self._loss_avg - cb_ratio * self._loss_cb, OnlineResult.LOSS_MIN)
         elif "ucb" in score_name:
             return min(self._loss_avg + cb_ratio * self._loss_cb, OnlineResult.LOSS_MAX)
         elif "avg" in score_name:
@@ -278,17 +270,15 @@
             is_checked_under_current_champion (bool): indicates whether this trials has
                 been paused under the current champion.
             trial_id (str): id of the trial (if None, it will be generated in the constructor).
         """
         try:
             from vowpalwabbit import pyvw
         except ImportError:
-            raise ImportError(
-                "To use AutoVW, please run pip install flaml[vw] to install vowpalwabbit"
-            )
+            raise ImportError("To use AutoVW, please run pip install flaml[vw] to install vowpalwabbit")
         # attributes
         self.trial_id = self._config_to_id(config) if trial_id is None else trial_id
         logger.info("Create trial with trial_id: %s", self.trial_id)
         super().__init__(
             config,
             min_resource_lease,
             is_champion,
@@ -323,22 +313,18 @@
                 config_id += str(v)
             config_id_full = config_id_full + config_id
         return config_id_full
 
     def _initialize_vw_model(self, vw_example):
         """Initialize a vw model using the trainable_class"""
         self._vw_config = self.config.copy()
-        ns_interactions = self.config.get(
-            VowpalWabbitTrial.interactions_config_key, None
-        )
+        ns_interactions = self.config.get(VowpalWabbitTrial.interactions_config_key, None)
         # ensure the feature interaction config is a list (required by VW)
         if ns_interactions is not None:
-            self._vw_config[VowpalWabbitTrial.interactions_config_key] = list(
-                ns_interactions
-            )
+            self._vw_config[VowpalWabbitTrial.interactions_config_key] = list(ns_interactions)
         # get the dimensionality of the feature according to the namespace configuration
         namespace_feature_dim = get_ns_feature_dim_from_vw_example(vw_example)
         self._dim = self._get_dim_from_ns(namespace_feature_dim, ns_interactions)
         # construct an instance of vw model using the input config and fixed config
         self.model = self.trainable_class(**self._vw_config)
         self.result = OnlineResult(
             self._metric,
@@ -357,17 +343,15 @@
         self._update_y_range(y)
         if self.model is None:
             # initialize self.model and self.result
             self._initialize_vw_model(data_sample)
         # do one step of learning
         self.model.learn(data_sample)
         # update training related results accordingly
-        new_loss = self._get_loss(
-            y, y_pred, self._metric, self._y_min_observed, self._y_max_observed
-        )
+        new_loss = self._get_loss(y, y_pred, self._metric, self._y_min_observed, self._y_max_observed)
         # udpate sample size, sum of loss, and cost
         data_sample_size = 1
         bound_of_range = self._y_max_observed - self._y_min_observed
         if bound_of_range == 0:
             bound_of_range = 1.0
         self.result.update_result(
             new_loss,
@@ -387,36 +371,30 @@
         """Get instantaneous loss from y_true and y_pred, and loss_func_name
         For mae_clip, we clip y_pred in the observed range of y
         """
         if "mse" in loss_func_name or "squared" in loss_func_name:
             loss_func = mean_squared_error
         elif "mae" in loss_func_name or "absolute" in loss_func_name:
             loss_func = mean_absolute_error
-            if (
-                y_min_observed is not None
-                and y_max_observed is not None
-                and "clip" in loss_func_name
-            ):
+            if y_min_observed is not None and y_max_observed is not None and "clip" in loss_func_name:
                 # clip y_pred in the observed range of y
                 y_pred = min(y_max_observed, max(y_pred, y_min_observed))
         else:
             raise NotImplementedError
         return loss_func([y_true], [y_pred])
 
     def _update_y_range(self, y):
         """Maintain running observed minimum and maximum target value."""
         if self._y_min_observed is None or y < self._y_min_observed:
             self._y_min_observed = y
         if self._y_max_observed is None or y > self._y_max_observed:
             self._y_max_observed = y
 
     @staticmethod
-    def _get_dim_from_ns(
-        namespace_feature_dim: dict, namespace_interactions: Union[set, list]
-    ):
+    def _get_dim_from_ns(namespace_feature_dim: dict, namespace_interactions: Union[set, list]):
         """Get the dimensionality of the corresponding feature of input namespace set."""
         total_dim = sum(namespace_feature_dim.values())
         if namespace_interactions:
             for f in namespace_interactions:
                 ns_dim = 1.0
                 for c in f:
                     ns_dim *= namespace_feature_dim[c]
```

### Comparing `FLAML-1.2.0/flaml/onlineml/trial_runner.py` & `FLAML-1.2.1/flaml/onlineml/trial_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,20 +29,15 @@
     # Status change routine of a trial:
     # Trial.PENDING -> (Trial.RUNNING -> Trial.PAUSED -> Trial.RUNNING -> ...) -> Trial.TERMINATED(optional)
 
     RANDOM_SEED = 123456
     WARMSTART_NUM = 100
 
     def __init__(
-        self,
-        max_live_model_num: int,
-        searcher=None,
-        scheduler=None,
-        champion_test_policy="loss_ucb",
-        **kwargs
+        self, max_live_model_num: int, searcher=None, scheduler=None, champion_test_policy="loss_ucb", **kwargs
     ):
         """Constructor.
 
         Args:
             max_live_model_num: The maximum number of 'live'/running models allowed.
             searcher: A class for generating Trial objects progressively.
                 The ConfigOracle is implemented in the searcher.
@@ -188,17 +183,15 @@
             if trial_to_run is not None:
                 self.run_trial(trial_to_run)
             else:
                 break
 
     def get_top_running_trials(self, top_ratio=None, top_metric="ucb") -> list:
         """Get a list of trial ids, whose performance is among the top running trials."""
-        running_valid_trials = [
-            trial for trial in self._running_trials if trial.result is not None
-        ]
+        running_valid_trials = [trial for trial in self._running_trials if trial.result is not None]
         if not running_valid_trials:
             return
         if top_ratio is None:
             top_number = 0
         elif isinstance(top_ratio, float):
             top_number = math.ceil(len(running_valid_trials) * top_ratio)
         elif isinstance(top_ratio, str) and "best" in top_ratio:
@@ -211,49 +204,36 @@
         elif "avg" in top_metric:
             test_attribute = "loss_avg"
         elif "lcb" in top_metric:
             test_attribute = "loss_lcb"
         else:
             raise NotImplementedError
         top_running_valid_trials = []
-        logger.info(
-            "Running trial ids %s", [trial.trial_id for trial in running_valid_trials]
-        )
+        logger.info("Running trial ids %s", [trial.trial_id for trial in running_valid_trials])
         self._random_state.shuffle(running_valid_trials)
-        results = [
-            trial.result.get_score(test_attribute) for trial in running_valid_trials
-        ]
+        results = [trial.result.get_score(test_attribute) for trial in running_valid_trials]
         # sorted result (small to large) index
         sorted_index = np.argsort(np.array(results))
         for i in range(min(top_number, len(running_valid_trials))):
             top_running_valid_trials.append(running_valid_trials[sorted_index[i]])
-        logger.info(
-            "Top running ids %s", [trial.trial_id for trial in top_running_valid_trials]
-        )
+        logger.info("Top running ids %s", [trial.trial_id for trial in top_running_valid_trials])
         return top_running_valid_trials
 
     def _add_trial_from_searcher(self):
         """Add a new trial to this TrialRunner.
 
         NOTE:
             The new trial is acquired from the input search algorithm, i.e. self._searcher.
             A 'new' trial means the trial is not in self._trial.
         """
         # (optionally) upper bound the number of trials in the OnlineTrialRunner
         if self._bound_trial_num and self._first_challenger_pool_size is not None:
-            active_trial_size = len(
-                [t for t in self._trials if t.status != Trial.TERMINATED]
-            )
+            active_trial_size = len([t for t in self._trials if t.status != Trial.TERMINATED])
             trial_num_upper_bound = (
-                int(
-                    round(
-                        (np.log10(self._total_steps) + 1)
-                        * self._first_challenger_pool_size
-                    )
-                )
+                int(round((np.log10(self._total_steps) + 1) * self._first_challenger_pool_size))
                 if self._first_challenger_pool_size
                 else np.inf
             )
             if active_trial_size > trial_num_upper_bound:
                 logger.info(
                     "Not adding new trials: %s exceeds trial limit %s.",
                     active_trial_size,
@@ -282,35 +262,30 @@
     def _champion_test(self):
         """Perform tests again the latest champion, including bette_than tests and worse_than tests"""
         # for BetterThan test, we only need to compare the best challenger with the champion
         self._get_best_challenger()
         if self._best_challenger_trial is not None:
             assert self._best_challenger_trial.trial_id != self._champion_trial.trial_id
             # test whether a new champion is found and set the trial properties accordingly
-            is_new_champion_found = self._better_than_champion_test(
-                self._best_challenger_trial
-            )
+            is_new_champion_found = self._better_than_champion_test(self._best_challenger_trial)
             if is_new_champion_found:
                 self._set_champion(new_champion_trial=self._best_challenger_trial)
 
         # performs _worse_than_champion_test, which is an optional component in ChaCha
         if self._remove_worse:
             to_stop = []
             for trial_to_test in self._trials:
                 if trial_to_test.status != Trial.TERMINATED:
                     worse_than_champion = self._worse_than_champion_test(
                         self._champion_trial, trial_to_test, self.WARMSTART_NUM
                     )
                     if worse_than_champion:
                         to_stop.append(trial_to_test)
             # we want to ensure there are at least #max_live_model_num of challengers remaining
-            max_to_stop_num = (
-                len([t for t in self._trials if t.status != Trial.TERMINATED])
-                - self._max_live_model_num
-            )
+            max_to_stop_num = len([t for t in self._trials if t.status != Trial.TERMINATED]) - self._max_live_model_num
             for i in range(min(max_to_stop_num, len(to_stop))):
                 self.stop_trial(to_stop[i])
 
     def _get_best_challenger(self):
         """Get the 'best' (in terms of the champion_test_policy) challenger under consideration."""
         if self._champion_test_policy is None:
             return
@@ -327,17 +302,15 @@
                 trial.status != Trial.TERMINATED
                 and trial.trial_id != self._champion_trial.trial_id
                 and trial.result is not None
             )
         ]
         if active_trials:
             self._random_state.shuffle(active_trials)
-            results = [
-                trial.result.get_score(test_attribute) for trial in active_trials
-            ]
+            results = [trial.result.get_score(test_attribute) for trial in active_trials]
             best_index = np.argmin(results)
             self._best_challenger_trial = active_trials[best_index]
 
     def _set_champion(self, new_champion_trial):
         """Set the status of the existing trials once a new champion is found."""
         assert new_champion_trial is not None
         is_init_update = False
@@ -354,17 +327,15 @@
         self._all_new_challengers_added = False
         logger.info("Set the champion as %s", self._champion_trial.trial_id)
         if not is_init_update:
             self._champion_update_times += 1
             # calling set_search_properties of searcher will trigger
             # new challenger generation. we do not do this for init champion
             # as this step is already done when first constructing the searcher
-            self._searcher.set_search_properties(
-                setting={self._searcher.CHAMPION_TRIAL_NAME: self._champion_trial}
-            )
+            self._searcher.set_search_properties(setting={self._searcher.CHAMPION_TRIAL_NAME: self._champion_trial})
         else:
             self._champion_update_times = 0
 
     def get_trials(self) -> list:
         """Return the list of trials managed by this TrialRunner."""
         return self._trials
 
@@ -446,21 +417,17 @@
         is better than the current champion config.
 
         Returns:
             A bool indicating whether a new champion is found.
         """
         if trial_to_test.result is not None and self._champion_trial.result is not None:
             if "ucb" in self._champion_test_policy:
-                return self._test_lcb_ucb(
-                    self._champion_trial, trial_to_test, self.WARMSTART_NUM
-                )
+                return self._test_lcb_ucb(self._champion_trial, trial_to_test, self.WARMSTART_NUM)
             elif "avg" in self._champion_test_policy:
-                return self._test_avg_loss(
-                    self._champion_trial, trial_to_test, self.WARMSTART_NUM
-                )
+                return self._test_avg_loss(self._champion_trial, trial_to_test, self.WARMSTART_NUM)
             elif "martingale" in self._champion_test_policy:
                 return self._test_martingale(self._champion_trial, trial_to_test)
             else:
                 raise NotImplementedError
         else:
             return False
 
@@ -470,17 +437,15 @@
         if trial.result is not None and trial.result.resource_used >= warmstart_num:
             if trial.result.loss_lcb > champion_trial.result.loss_ucb:
                 logger.info(
                     "=========trial %s is worse than champion %s=====",
                     trial.trial_id,
                     champion_trial.trial_id,
                 )
-                logger.info(
-                    "trial %s %s %s", trial.config, trial.result, trial.resource_lease
-                )
+                logger.info("trial %s %s %s", trial.config, trial.result, trial.resource_lease)
                 logger.info(
                     "trial loss_avg:%s, trial loss_cb %s",
                     trial.result.loss_avg,
                     trial.result.loss_cb,
                 )
                 logger.info(
                     "champion loss_avg:%s, champion loss_cb %s",
@@ -504,21 +469,16 @@
     @staticmethod
     def _test_lcb_ucb(champion_trial, trial, warmstart_num=1) -> bool:
         """Comare the challenger(i.e., trial)'s loss upper bound with
         champion_trial's loss lower bound - cb
         """
         assert trial.trial_id != champion_trial.trial_id
         if trial.result.resource_used >= warmstart_num:
-            if (
-                trial.result.loss_ucb
-                < champion_trial.result.loss_lcb - champion_trial.result.loss_cb
-            ):
-                logger.info(
-                    "======new champion condition satisfied: using lcb vs ucb====="
-                )
+            if trial.result.loss_ucb < champion_trial.result.loss_lcb - champion_trial.result.loss_cb:
+                logger.info("======new champion condition satisfied: using lcb vs ucb=====")
                 logger.info(
                     "new champion trial %s %s %s",
                     trial.trial_id,
                     trial.result.resource_used,
                     trial.resource_lease,
                 )
                 logger.info(
```

### Comparing `FLAML-1.2.0/flaml/tune/__init__.py` & `FLAML-1.2.1/flaml/tune/__init__.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/tune/analysis.py` & `FLAML-1.2.1/flaml/tune/analysis.py`

 * *Files 9% similar despite different names*

```diff
@@ -122,17 +122,15 @@
         mode = self._validate_mode(mode)
         if scope not in ["all", "last", "avg", "last-5-avg", "last-10-avg"]:
             raise ValueError(
                 "ExperimentAnalysis: attempting to get best trial for "
                 'metric {} for scope {} not in ["all", "last", "avg", '
                 '"last-5-avg", "last-10-avg"]. '
                 "If you didn't pass a `metric` parameter to `tune.run()`, "
-                "you have to pass one when fetching the best trial.".format(
-                    metric, scope
-                )
+                "you have to pass one when fetching the best trial.".format(metric, scope)
             )
         best_trial = None
         best_metric_score = None
         for trial in self.trials:
             if metric not in trial.metric_analysis:
                 continue
             if scope in ["last", "avg", "last-5-avg", "last-10-avg"]:
@@ -151,18 +149,15 @@
             if (mode == "max") and (best_metric_score < metric_score):
                 best_metric_score = metric_score
                 best_trial = trial
             elif (mode == "min") and (best_metric_score > metric_score):
                 best_metric_score = metric_score
                 best_trial = trial
         if not best_trial:
-            logger.warning(
-                "Could not find best trial. Did you pass the correct `metric` "
-                "parameter?"
-            )
+            logger.warning("Could not find best trial. Did you pass the correct `metric` " "parameter?")
         return best_trial
 
     def get_best_config(
         self,
         metric: Optional[str] = None,
         mode: Optional[str] = None,
         scope: str = "last",
```

### Comparing `FLAML-1.2.0/flaml/tune/result.py` & `FLAML-1.2.1/flaml/tune/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,17 +120,15 @@
 # __stdout_file__/__stderr_file__ are magic keywords used internally
 # to pass log file locations to the Trainable via the constructor.
 STDOUT_FILE = "__stdout_file__"
 STDERR_FILE = "__stderr_file__"
 
 # Where Tune writes result files by default
 DEFAULT_RESULTS_DIR = (
-    os.environ.get("TEST_TMPDIR")
-    or os.environ.get("TUNE_RESULT_DIR")
-    or os.path.expanduser("~/ray_results")
+    os.environ.get("TEST_TMPDIR") or os.environ.get("TUNE_RESULT_DIR") or os.path.expanduser("~/ray_results")
 )
 
 # Meta file about status under each experiment directory, can be
 # parsed by automlboard if exists.
 JOB_META_FILE = "job_status.json"
 
 # Meta file about status under each trial directory, can be parsed
```

### Comparing `FLAML-1.2.0/flaml/tune/sample.py` & `FLAML-1.2.1/flaml/tune/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,21 +49,17 @@
         new and old numpy randomness generators.
         """
 
         _rng = None
 
         def __init__(
             self,
-            generator_or_seed: Optional[
-                Union["np_random_generator", np.random.RandomState, int]
-            ] = None,
+            generator_or_seed: Optional[Union["np_random_generator", np.random.RandomState, int]] = None,
         ):
-            if generator_or_seed is None or isinstance(
-                generator_or_seed, (np.random.RandomState, np_random_generator)
-            ):
+            if generator_or_seed is None or isinstance(generator_or_seed, (np.random.RandomState, np_random_generator)):
                 self._rng = generator_or_seed
             elif LEGACY_RNG:
                 self._rng = np.random.RandomState(generator_or_seed)
             else:
                 self._rng = np.random.default_rng(generator_or_seed)
 
         @property
@@ -81,17 +77,15 @@
                 if name == "integers":
                     name = "randint"
                 elif name == "random":
                     name = "rand"
             return getattr(self.rng, name)
 
 
-RandomState = Union[
-    None, _BackwardsCompatibleNumpyRng, np_random_generator, np.random.RandomState, int
-]
+RandomState = Union[None, _BackwardsCompatibleNumpyRng, np_random_generator, np.random.RandomState, int]
 
 
 class Domain:
     """Base class to specify a type and valid range to sample parameters from.
     This base class is implemented by parameter spaces, like float ranges
     (``Float``), integer ranges (``Integer``), or categorical variables
     (``Categorical``). The ``Domain`` object contains information about
@@ -108,17 +102,15 @@
         return value
 
     def set_sampler(self, sampler, allow_override=False):
         if self.sampler and not allow_override:
             raise ValueError(
                 "You can only choose one sampler for parameter "
                 "domains. Existing sampler for parameter {}: "
-                "{}. Tried to add {}".format(
-                    self.__class__.__name__, self.sampler, sampler
-                )
+                "{}. Tried to add {}".format(self.__class__.__name__, self.sampler, sampler)
             )
         self.sampler = sampler
 
     def get_sampler(self):
         sampler = self.sampler
         if not sampler:
             sampler = self.default_sampler_cls()
@@ -227,17 +219,15 @@
             spec: Optional[Union[List[Dict], Dict]] = None,
             size: int = 1,
             random_state: "RandomState" = None,
         ):
             if not isinstance(random_state, _BackwardsCompatibleNumpyRng):
                 random_state = _BackwardsCompatibleNumpyRng(random_state)
             assert domain.lower > 0, "LogUniform needs a lower bound greater than 0"
-            assert (
-                0 < domain.upper < float("inf")
-            ), "LogUniform needs a upper bound greater than 0"
+            assert 0 < domain.upper < float("inf"), "LogUniform needs a upper bound greater than 0"
             logmin = np.log(domain.lower) / np.log(self.base)
             logmax = np.log(domain.upper) / np.log(self.base)
 
             items = self.base ** (random_state.uniform(logmin, logmax, size=size))
             return items if len(items) > 1 else domain.cast(items[0])
 
     class _Normal(Normal):
@@ -267,23 +257,17 @@
         self.upper = upper if upper is not None else float("inf")
 
     def cast(self, value):
         return float(value)
 
     def uniform(self):
         if not self.lower > float("-inf"):
-            raise ValueError(
-                "Uniform requires a lower bound. Make sure to set the "
-                "`lower` parameter of `Float()`."
-            )
+            raise ValueError("Uniform requires a lower bound. Make sure to set the " "`lower` parameter of `Float()`.")
         if not self.upper < float("inf"):
-            raise ValueError(
-                "Uniform requires a upper bound. Make sure to set the "
-                "`upper` parameter of `Float()`."
-            )
+            raise ValueError("Uniform requires a upper bound. Make sure to set the " "`upper` parameter of `Float()`.")
         new = copy(self)
         new.set_sampler(self._Uniform())
         return new
 
     def loguniform(self, base: float = 10):
         if not self.lower > 0:
             raise ValueError(
@@ -305,28 +289,18 @@
 
     def normal(self, mean=0.0, sd=1.0):
         new = copy(self)
         new.set_sampler(self._Normal(mean, sd))
         return new
 
     def quantized(self, q: float):
-        if self.lower > float("-inf") and not isclose(
-            self.lower / q, round(self.lower / q)
-        ):
-            raise ValueError(
-                f"Your lower variable bound {self.lower} is not divisible by "
-                f"quantization factor {q}."
-            )
-        if self.upper < float("inf") and not isclose(
-            self.upper / q, round(self.upper / q)
-        ):
-            raise ValueError(
-                f"Your upper variable bound {self.upper} is not divisible by "
-                f"quantization factor {q}."
-            )
+        if self.lower > float("-inf") and not isclose(self.lower / q, round(self.lower / q)):
+            raise ValueError(f"Your lower variable bound {self.lower} is not divisible by " f"quantization factor {q}.")
+        if self.upper < float("inf") and not isclose(self.upper / q, round(self.upper / q)):
+            raise ValueError(f"Your upper variable bound {self.upper} is not divisible by " f"quantization factor {q}.")
 
         new = copy(self)
         new.set_sampler(Quantized(new.get_sampler(), q), allow_override=True)
         return new
 
     def is_valid(self, value: float):
         return self.lower <= value <= self.upper
@@ -357,17 +331,15 @@
             spec: Optional[Union[List[Dict], Dict]] = None,
             size: int = 1,
             random_state: "RandomState" = None,
         ):
             if not isinstance(random_state, _BackwardsCompatibleNumpyRng):
                 random_state = _BackwardsCompatibleNumpyRng(random_state)
             assert domain.lower > 0, "LogUniform needs a lower bound greater than 0"
-            assert (
-                0 < domain.upper < float("inf")
-            ), "LogUniform needs a upper bound greater than 0"
+            assert 0 < domain.upper < float("inf"), "LogUniform needs a upper bound greater than 0"
             logmin = np.log(domain.lower) / np.log(self.base)
             logmax = np.log(domain.upper) / np.log(self.base)
 
             items = self.base ** (random_state.uniform(logmin, logmax, size=size))
             items = np.floor(items).astype(int)
             return items if len(items) > 1 else domain.cast(items[0])
 
@@ -426,17 +398,15 @@
             size: int = 1,
             random_state: "RandomState" = None,
         ):
             if not isinstance(random_state, _BackwardsCompatibleNumpyRng):
                 random_state = _BackwardsCompatibleNumpyRng(random_state)
             # do not use .choice() directly on domain.categories
             # as that will coerce them to a single dtype
-            indices = random_state.choice(
-                np.arange(0, len(domain.categories)), size=size
-            )
+            indices = random_state.choice(np.arange(0, len(domain.categories)), size=size)
             items = [domain.categories[index] for index in indices]
             return items if len(items) > 1 else domain.cast(items[0])
 
     default_sampler_cls = _Uniform
 
     def __init__(self, categories: Sequence):
         self.categories = list(categories)
@@ -487,17 +457,15 @@
 
         if self.q == 1:
             return self.sampler.sample(domain, spec, size, random_state=random_state)
 
         quantized_domain = copy(domain)
         quantized_domain.lower = np.ceil(domain.lower / self.q) * self.q
         quantized_domain.upper = np.floor(domain.upper / self.q) * self.q
-        values = self.sampler.sample(
-            quantized_domain, spec, size, random_state=random_state
-        )
+        values = self.sampler.sample(quantized_domain, spec, size, random_state=random_state)
         quantized = np.round(np.divide(values, self.q)) * self.q
 
         if not isinstance(quantized, np.ndarray):
             return domain.cast(quantized)
         return list(quantized)
 
 
@@ -505,19 +473,15 @@
     def __init__(
         self,
         init_monomials: set = (),
         highest_poly_order: int = None,
         allow_self_inter: bool = False,
     ):
         self._init_monomials = init_monomials
-        self._highest_poly_order = (
-            highest_poly_order
-            if highest_poly_order is not None
-            else len(self._init_monomials)
-        )
+        self._highest_poly_order = highest_poly_order if highest_poly_order is not None else len(self._init_monomials)
         self._allow_self_inter = allow_self_inter
 
     @property
     def init_monomials(self):
         return self._init_monomials
 
     @property
@@ -640,11 +604,9 @@
         q: Quantization number. The result will be rounded to an
             integer increment of this value.
 
     """
     return Float(None, None).normal(mean, sd).quantized(q)
 
 
-def polynomial_expansion_set(
-    init_monomials: set, highest_poly_order: int = None, allow_self_inter: bool = False
-):
+def polynomial_expansion_set(init_monomials: set, highest_poly_order: int = None, allow_self_inter: bool = False):
     return PolynomialExpansionSet(init_monomials, highest_poly_order, allow_self_inter)
```

### Comparing `FLAML-1.2.0/flaml/tune/scheduler/online_scheduler.py` & `FLAML-1.2.1/flaml/tune/scheduler/online_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,15 @@
         for trial in trial_runner.get_trials():
             if trial.status == Trial.PENDING:
                 return trial
         min_paused_resource = np.inf
         min_paused_resource_trial = None
         for trial in trial_runner.get_trials():
             # if there is a tie, prefer the earlier added ones
-            if (
-                trial.status == Trial.PAUSED
-                and trial.resource_lease < min_paused_resource
-            ):
+            if trial.status == Trial.PAUSED and trial.resource_lease < min_paused_resource:
                 min_paused_resource = trial.resource_lease
                 min_paused_resource_trial = trial
         if min_paused_resource_trial is not None:
             return min_paused_resource_trial
 
 
 class OnlineSuccessiveDoublingScheduler(OnlineScheduler):
@@ -118,12 +115,10 @@
                 logger.debug("champion, %s", trial_runner.champion_trial.trial_id)
                 # this can be inefficient when the # trials is large. TODO: need to improve efficiency.
                 top_trials = trial_runner.get_top_running_trials(
                     self._keep_challenger_ratio, self._keep_challenger_metric
                 )
                 logger.debug("top_learners: %s", top_trials)
                 if trial in top_trials:
-                    logger.debug(
-                        "top runner %s: set from PAUSE to CONTINUE", trial.trial_id
-                    )
+                    logger.debug("top runner %s: set from PAUSE to CONTINUE", trial.trial_id)
                     return TrialScheduler.CONTINUE
         return decision
```

### Comparing `FLAML-1.2.0/flaml/tune/scheduler/trial_scheduler.py` & `FLAML-1.2.1/flaml/tune/scheduler/trial_scheduler.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/tune/searcher/blendsearch.py` & `FLAML-1.2.1/flaml/tune/searcher/blendsearch.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,15 @@
         time_budget_s: Union[int, float] = None,
         num_samples: Optional[int] = None,
         resource_attr: Optional[str] = None,
         min_resource: Optional[float] = None,
         max_resource: Optional[float] = None,
         reduction_factor: Optional[float] = None,
         global_search_alg: Optional[Searcher] = None,
-        config_constraints: Optional[
-            List[Tuple[Callable[[dict], float], str, float]]
-        ] = None,
+        config_constraints: Optional[List[Tuple[Callable[[dict], float], str, float]]] = None,
         metric_constraints: Optional[List[Tuple[str, str, float]]] = None,
         seed: Optional[int] = 20,
         cost_attr: Optional[str] = "auto",
         cost_budget: Optional[float] = None,
         experimental: Optional[bool] = False,
         lexico_objectives: Optional[dict] = None,
         use_incumbent_result_in_evaluation=False,
@@ -192,17 +190,15 @@
             self._points_to_evaluate.extend(new_points_to_evaluate)
         else:
             self._points_to_evaluate = points_to_evaluate or []
             self._evaluated_rewards = evaluated_rewards or []
         self._config_constraints = config_constraints
         self._metric_constraints = metric_constraints
         if metric_constraints:
-            assert all(
-                x[1] in ["<=", ">="] for x in metric_constraints
-            ), "sign of metric constraints must be <= or >=."
+            assert all(x[1] in ["<=", ">="] for x in metric_constraints), "sign of metric constraints must be <= or >=."
             # metric modified by lagrange
             metric += self.lagrange
         self._cat_hp_cost = cat_hp_cost or {}
         if space:
             add_cost_to_space(space, init_config, self._cat_hp_cost)
         self._ls = self.LocalSearch(
             init_config,
@@ -228,17 +224,15 @@
             else:
                 gs_space = space
             gs_seed = seed - 10 if (seed - 10) >= 0 else seed - 11 + (1 << 32)
             self._gs_seed = gs_seed
             if experimental:
                 import optuna as ot
 
-                sampler = ot.samplers.TPESampler(
-                    seed=gs_seed, multivariate=True, group=True
-                )
+                sampler = ot.samplers.TPESampler(seed=gs_seed, multivariate=True, group=True)
             else:
                 sampler = None
             try:
                 assert evaluated_rewards
                 self._gs = GlobalSearch(
                     space=gs_space,
                     metric=metric,
@@ -256,19 +250,15 @@
                     seed=gs_seed,
                     sampler=sampler,
                 )
             self._gs.space = space
         else:
             self._gs = None
         self._experimental = experimental
-        if (
-            getattr(self, "__name__", None) == "CFO"
-            and points_to_evaluate
-            and len(self._points_to_evaluate) > 1
-        ):
+        if getattr(self, "__name__", None) == "CFO" and points_to_evaluate and len(self._points_to_evaluate) > 1:
             # use the best config in points_to_evaluate as the start point
             self._candidate_start_points = {}
             self._started_from_low_cost = not low_cost_partial_config
         else:
             self._candidate_start_points = None
         self._time_budget_s, self._num_samples = time_budget_s, num_samples
         self._allow_empty_config = allow_empty_config
@@ -379,17 +369,15 @@
             recursive=True,
         )
         self._gs_admissible_min = self._ls_bound_min.copy()
         self._gs_admissible_max = self._ls_bound_max.copy()
 
         if self._metric_constraints:
             self._metric_constraint_satisfied = False
-            self._metric_constraint_penalty = [
-                self.penalty for _ in self._metric_constraints
-            ]
+            self._metric_constraint_penalty = [self.penalty for _ in self._metric_constraints]
         else:
             self._metric_constraint_satisfied = True
             self._metric_constraint_penalty = None
         self.best_resource = self._ls.min_resource
         i = 0
         # config_signature: tuple -> result: Dict
         self._result = {}
@@ -420,60 +408,50 @@
     def metric_target(self):
         return self._metric_target
 
     @property
     def is_ls_ever_converged(self):
         return self._is_ls_ever_converged
 
-    def on_trial_complete(
-        self, trial_id: str, result: Optional[Dict] = None, error: bool = False
-    ):
+    def on_trial_complete(self, trial_id: str, result: Optional[Dict] = None, error: bool = False):
         """search thread updater and cleaner."""
         metric_constraint_satisfied = True
         if result and not error and self._metric_constraints:
             # account for metric constraints if any
             objective = result[self._metric]
             for i, constraint in enumerate(self._metric_constraints):
                 metric_constraint, sign, threshold = constraint
                 value = result.get(metric_constraint)
                 if value:
                     sign_op = 1 if sign == "<=" else -1
                     violation = (value - threshold) * sign_op
                     if violation > 0:
                         # add penalty term to the metric
-                        objective += (
-                            self._metric_constraint_penalty[i]
-                            * violation
-                            * self._ls.metric_op
-                        )
+                        objective += self._metric_constraint_penalty[i] * violation * self._ls.metric_op
                         metric_constraint_satisfied = False
                         if self._metric_constraint_penalty[i] < self.penalty:
                             self._metric_constraint_penalty[i] += violation
             result[self._metric + self.lagrange] = objective
             if metric_constraint_satisfied and not self._metric_constraint_satisfied:
                 # found a feasible point
                 self._metric_constraint_penalty = [1 for _ in self._metric_constraints]
             self._metric_constraint_satisfied |= metric_constraint_satisfied
         thread_id = self._trial_proposed_by.get(trial_id)
         if thread_id in self._search_thread_pool:
-            self._search_thread_pool[thread_id].on_trial_complete(
-                trial_id, result, error
-            )
+            self._search_thread_pool[thread_id].on_trial_complete(trial_id, result, error)
             del self._trial_proposed_by[trial_id]
         if result:
             config = result.get("config", {})
             if not config:
                 for key, value in result.items():
                     if key.startswith("config/"):
                         config[key[7:]] = value
             if self._allow_empty_config and not config:
                 return
-            signature = self._ls.config_signature(
-                config, self._subspace.get(trial_id, {})
-            )
+            signature = self._ls.config_signature(config, self._subspace.get(trial_id, {}))
             if error:  # remove from result cache
                 del self._result[signature]
             else:  # add to result cache
                 self._cost_used += result.get(self.cost_attr, 0)
                 self._result[signature] = result
                 # update target metric if improved
                 objective = result[self._ls.metric]
@@ -485,38 +463,29 @@
                     if not self._metric_constraint_satisfied:
                         # no point has been found to satisfy metric constraint
                         self._expand_admissible_region(
                             self._ls_bound_min,
                             self._ls_bound_max,
                             self._subspace.get(trial_id, self._ls.space),
                         )
-                    if (
-                        self._gs is not None
-                        and self._experimental
-                        and (not self._ls.hierarchical)
-                    ):
+                    if self._gs is not None and self._experimental and (not self._ls.hierarchical):
                         self._gs.add_evaluated_point(flatten_dict(config), objective)
                         # TODO: recover when supported
                         # converted = convert_key(config, self._gs.space)
                         # logger.info(converted)
                         # self._gs.add_evaluated_point(converted, objective)
                 elif metric_constraint_satisfied and self._create_condition(result):
                     # thread creator
                     thread_id = self._thread_count
-                    self._started_from_given = (
-                        self._candidate_start_points
-                        and trial_id in self._candidate_start_points
-                    )
+                    self._started_from_given = self._candidate_start_points and trial_id in self._candidate_start_points
                     if self._started_from_given:
                         del self._candidate_start_points[trial_id]
                     else:
                         self._started_from_low_cost = True
-                    self._create_thread(
-                        config, result, self._subspace.get(trial_id, self._ls.space)
-                    )
+                    self._create_thread(config, result, self._subspace.get(trial_id, self._ls.space))
                 # reset admissible region to ls bounding box
                 self._gs_admissible_min.update(self._ls_bound_min)
                 self._gs_admissible_max.update(self._ls_bound_max)
         # cleaner
         if thread_id and thread_id in self._search_thread_pool:
             # local search thread
             self._clean(thread_id)
@@ -591,17 +560,15 @@
                 elif value < admissible_min[key]:
                     admissible_min[key] = value
 
     def _create_condition(self, result: Dict) -> bool:
         """create thread condition"""
         if len(self._search_thread_pool) < 2:
             return True
-        obj_median = np.median(
-            [thread.obj_best1 for id, thread in self._search_thread_pool.items() if id]
-        )
+        obj_median = np.median([thread.obj_best1 for id, thread in self._search_thread_pool.items() if id])
         return result[self._ls.metric] * self._ls.metric_op < obj_median
 
     def _clean(self, thread_id: int):
         """delete thread and increase admissible region if converged,
         merge local threads if they are close
         """
         assert thread_id
@@ -644,43 +611,36 @@
             self._create_thread_from_best_candidate()
 
     def _create_thread_from_best_candidate(self):
         # find the best start point
         best_trial_id = None
         obj_best = None
         for trial_id, r in self._candidate_start_points.items():
-            if r and (
-                best_trial_id is None
-                or r[self._ls.metric] * self._ls.metric_op < obj_best
-            ):
+            if r and (best_trial_id is None or r[self._ls.metric] * self._ls.metric_op < obj_best):
                 best_trial_id = trial_id
                 obj_best = r[self._ls.metric] * self._ls.metric_op
         if best_trial_id:
             # create a new thread
             config = {}
             result = self._candidate_start_points[best_trial_id]
             for key, value in result.items():
                 if key.startswith("config/"):
                     config[key[7:]] = value
             self._started_from_given = True
             del self._candidate_start_points[best_trial_id]
-            self._create_thread(
-                config, result, self._subspace.get(best_trial_id, self._ls.space)
-            )
+            self._create_thread(config, result, self._subspace.get(best_trial_id, self._ls.space))
 
     def _expand_admissible_region(self, lower, upper, space):
         """expand the admissible region for the subspace `space`"""
         for key in upper:
             ub = upper[key]
             if isinstance(ub, list):
                 choice = space[key].get("_choice_")
                 if choice:
-                    self._expand_admissible_region(
-                        lower[key][choice], upper[key][choice], space[key]
-                    )
+                    self._expand_admissible_region(lower[key][choice], upper[key][choice], space[key])
             elif isinstance(ub, dict):
                 self._expand_admissible_region(lower[key], ub, space[key])
             else:
                 upper[key] += self._ls.STEPSIZE
                 lower[key] -= self._ls.STEPSIZE
 
     def _inferior(self, id1: int, id2: int) -> bool:
@@ -748,17 +708,15 @@
                 # LS or valid or no backup choice
                 self._trial_proposed_by[trial_id] = choice
                 self._search_thread_pool[choice].running += use_rs
             else:  # invalid config proposed by GS
                 if choice == backup:
                     # use CFO's init point
                     init_config = self._ls.init_config
-                    config, space = self._ls.complete_config(
-                        init_config, self._ls_bound_min, self._ls_bound_max
-                    )
+                    config, space = self._ls.complete_config(init_config, self._ls_bound_min, self._ls_bound_max)
                     self._trial_proposed_by[trial_id] = choice
                     self._search_thread_pool[choice].running += 1
                 else:
                     thread = self._search_thread_pool[backup]
                     config = thread.suggest(trial_id)
                     space = thread.space
                     skip = self._should_skip(backup, trial_id, config, space)
@@ -797,17 +755,15 @@
                 if self._evaluated_rewards:
                     reward = self._evaluated_rewards.pop(0)
             else:
                 init_config = self._ls.init_config
             if self._allow_empty_config and not init_config:
                 assert reward is None, "Empty config can't have reward."
                 return init_config
-            config, space = self._ls.complete_config(
-                init_config, self._ls_bound_min, self._ls_bound_max
-            )
+            config, space = self._ls.complete_config(init_config, self._ls_bound_min, self._ls_bound_max)
             config_signature = self._ls.config_signature(config, space)
             if reward is None:
                 result = self._result.get(config_signature)
                 if result:  # tried before
                     return
                 elif result is None:  # not tried before
                     if self._violate_config_constriants(config, config_signature):
@@ -823,17 +779,15 @@
             if reward is not None:
                 result = {self._metric: reward, self.cost_attr: 1, "config": config}
                 # result = self._result[config_signature]
                 self.on_trial_complete(trial_id, result)
                 return
         if self._use_incumbent_result_in_evaluation:
             if self._trial_proposed_by[trial_id] > 0:
-                choice_thread = self._search_thread_pool[
-                    self._trial_proposed_by[trial_id]
-                ]
+                choice_thread = self._search_thread_pool[self._trial_proposed_by[trial_id]]
                 config[INCUMBENT_RESULT] = choice_thread.best_result
         return config
 
     def _violate_config_constriants(self, config, config_signature):
         """check if config violates config constraints.
         If so, set the result to worst and return True.
         """
@@ -870,17 +824,15 @@
         if not exists:
             # check constraints
             exists = self._violate_config_constriants(config, config_signature)
         if exists:  # suggested before (including violate constraints)
             if choice >= 0:  # not fallback to rs
                 result = self._result.get(config_signature)
                 if result:  # finished
-                    self._search_thread_pool[choice].on_trial_complete(
-                        trial_id, result, error=False
-                    )
+                    self._search_thread_pool[choice].on_trial_complete(trial_id, result, error=False)
                     if choice:
                         # local search thread
                         self._clean(choice)
                 # else:     # running
                 #     # tell the thread there is an error
                 #     self._search_thread_pool[choice].on_trial_complete(
                 #         trial_id, {}, error=True)
@@ -934,17 +886,15 @@
                     priority1 = priority
                     top_thread_id = thread_id
                 if priority > priority2 or backup_thread_id == 0:
                     priority2 = priority
                     backup_thread_id = thread_id
         return top_thread_id, backup_thread_id
 
-    def _valid(
-        self, config: Dict, space: Dict, subspace: Dict, lower: Dict, upper: Dict
-    ) -> bool:
+    def _valid(self, config: Dict, space: Dict, subspace: Dict, lower: Dict, upper: Dict) -> bool:
         """config validator"""
         normalized_config = normalize(config, subspace, config, {})
         for key, lb in lower.items():
             if key in config:
                 value = normalized_config[key]
                 if isinstance(lb, list):
                     domain = space[key]
@@ -958,18 +908,15 @@
                     ub = upper[key]
                 else:
                     nestedspace = None
                 if nestedspace:
                     valid = self._valid(value, domain, nestedspace, lb, ub)
                     if not valid:
                         return False
-                elif (
-                    value + self._ls.STEPSIZE < lower[key]
-                    or value > upper[key] + self._ls.STEPSIZE
-                ):
+                elif value + self._ls.STEPSIZE < lower[key] or value > upper[key] + self._ls.STEPSIZE:
                     return False
         return True
 
     @property
     def results(self) -> List[Dict]:
         """A list of dicts of results for each evaluated configuration.
 
@@ -1029,17 +976,15 @@
             parameter_id: int.
             parameters: object created by `generate_parameters()`.
             value: final metrics of the trial, including default metric.
         """
         result = {
             "config": parameters,
             self._metric: extract_scalar_reward(value),
-            self.cost_attr: 1
-            if isinstance(value, float)
-            else value.get(self.cost_attr, value.get("sequence", 1))
+            self.cost_attr: 1 if isinstance(value, float) else value.get(self.cost_attr, value.get("sequence", 1))
             # if nni does not report training cost,
             # using sequence as an approximation.
             # if no sequence, using a constant 1
         }
         self.on_trial_complete(str(parameter_id), result)
 
     ...
@@ -1141,29 +1086,23 @@
             # create the first local search thread
             return False
         if len(self._search_thread_pool) == 2:
             return False
         if self._candidate_start_points and self._thread_count == 1:
             # result needs to match or exceed the best candidate start point
             obj_best = min(
-                (
-                    self._ls.metric_op * r[self._ls.metric]
-                    for r in self._candidate_start_points.values()
-                    if r
-                ),
+                (self._ls.metric_op * r[self._ls.metric] for r in self._candidate_start_points.values() if r),
                 default=-np.inf,
             )
 
             return result[self._ls.metric] * self._ls.metric_op <= obj_best
         else:
             return True
 
-    def on_trial_complete(
-        self, trial_id: str, result: Optional[Dict] = None, error: bool = False
-    ):
+    def on_trial_complete(self, trial_id: str, result: Optional[Dict] = None, error: bool = False):
         super().on_trial_complete(trial_id, result, error)
         if self._candidate_start_points and trial_id in self._candidate_start_points:
             # the trial is a candidate start point
             self._candidate_start_points[trial_id] = result
             if len(self._search_thread_pool) < 2 and not self._points_to_evaluate:
                 self._create_thread_from_best_candidate()
 
@@ -1173,14 +1112,12 @@
 
     def suggest(self, trial_id: str) -> Optional[Dict]:
         if self._points_to_evaluate:
             return super().suggest(trial_id)
         config, _ = self._ls.complete_config({})
         return config
 
-    def on_trial_complete(
-        self, trial_id: str, result: Optional[Dict] = None, error: bool = False
-    ):
+    def on_trial_complete(self, trial_id: str, result: Optional[Dict] = None, error: bool = False):
         return
 
     def on_trial_result(self, trial_id: str, result: Dict):
         return
```

### Comparing `FLAML-1.2.0/flaml/tune/searcher/cfo_cat.py` & `FLAML-1.2.1/flaml/tune/searcher/cfo_cat.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/flaml/tune/searcher/flow2.py` & `FLAML-1.2.1/flaml/tune/searcher/flow2.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,29 +120,21 @@
         self.init_config = init_config
         self.best_config = flatten_dict(init_config)
         self.resource_attr = resource_attr
         self.min_resource = min_resource
         self.lexico_objectives = lexico_objectives
         if self.lexico_objectives is not None:
             if "modes" not in self.lexico_objectives.keys():
-                self.lexico_objectives["modes"] = ["min"] * len(
-                    self.lexico_objectives["metrics"]
-                )
-            for t_metric, t_mode in zip(
-                self.lexico_objectives["metrics"], self.lexico_objectives["modes"]
-            ):
+                self.lexico_objectives["modes"] = ["min"] * len(self.lexico_objectives["metrics"])
+            for t_metric, t_mode in zip(self.lexico_objectives["metrics"], self.lexico_objectives["modes"]):
                 if t_metric not in self.lexico_objectives["tolerances"].keys():
                     self.lexico_objectives["tolerances"][t_metric] = 0
                 if t_metric not in self.lexico_objectives["targets"].keys():
-                    self.lexico_objectives["targets"][t_metric] = (
-                        -float("inf") if t_mode == "min" else float("inf")
-                    )
-        self.resource_multiple_factor = (
-            resource_multiple_factor or SAMPLE_MULTIPLY_FACTOR
-        )
+                    self.lexico_objectives["targets"][t_metric] = -float("inf") if t_mode == "min" else float("inf")
+        self.resource_multiple_factor = resource_multiple_factor or SAMPLE_MULTIPLY_FACTOR
         self.cost_attr = cost_attr
         self.max_resource = max_resource
         self._resource = None
         self._f_best = None  # only use for lexico_comapre. It represent the best value achieved by lexico_flow.
         self._step_lb = np.Inf
         self._histories = None  # only use for lexico_comapre. It records the result of historical configurations.
         if space is not None:
@@ -162,39 +154,31 @@
                 sampler = domain.get_sampler()
                 # the step size lower bound for uniform variables doesn't depend
                 # on the current config
                 if isinstance(sampler, sample.Quantized):
                     q = sampler.q
                     sampler = sampler.get_sampler()
                     if str(sampler) == "Uniform":
-                        self._step_lb = min(
-                            self._step_lb, q / (domain.upper - domain.lower + 1)
-                        )
+                        self._step_lb = min(self._step_lb, q / (domain.upper - domain.lower + 1))
                 elif isinstance(domain, sample.Integer) and str(sampler) == "Uniform":
-                    self._step_lb = min(
-                        self._step_lb, 1.0 / (domain.upper - domain.lower)
-                    )
+                    self._step_lb = min(self._step_lb, 1.0 / (domain.upper - domain.lower))
                 if isinstance(domain, sample.Categorical):
                     if not domain.ordered:
                         self._unordered_cat_hp[key] = len(domain.categories)
                     if not hier:
                         for cat in domain.categories:
                             if isinstance(cat, dict):
                                 hier = True
                                 break
                 if str(sampler) != "Normal":
                     self._bounded_keys.append(key)
         if not hier:
             self._space_keys = sorted(self._tunable_keys)
         self.hierarchical = hier
-        if (
-            self.resource_attr
-            and self.resource_attr not in self._space
-            and self.max_resource
-        ):
+        if self.resource_attr and self.resource_attr not in self._space and self.max_resource:
             self.min_resource = self.min_resource or self._min_resource()
             self._resource = self._round(self.min_resource)
             if not hier:
                 self._space_keys.append(self.resource_attr)
         else:
             self._resource = None
         self.incumbent = {}
@@ -240,22 +224,20 @@
             # current config
             if isinstance(sampler, sample.Quantized):
                 q = sampler.q
                 sampler_inner = sampler.get_sampler()
                 if str(sampler_inner) == "LogUniform":
                     step_lb = min(
                         step_lb,
-                        np.log(1.0 + q / self.best_config[key])
-                        / np.log(domain.upper / domain.lower),
+                        np.log(1.0 + q / self.best_config[key]) / np.log(domain.upper / domain.lower),
                     )
             elif isinstance(domain, sample.Integer) and str(sampler) == "LogUniform":
                 step_lb = min(
                     step_lb,
-                    np.log(1.0 + 1.0 / self.best_config[key])
-                    / np.log((domain.upper - 1) / domain.lower),
+                    np.log(1.0 + 1.0 / self.best_config[key]) / np.log((domain.upper - 1) / domain.lower),
                 )
         if np.isinf(step_lb):
             step_lb = self.STEP_LOWER_BOUND
         else:
             step_lb *= self.step_ub
         return step_lb
 
@@ -284,26 +266,22 @@
     ) -> Tuple[Dict, Dict]:
         """Generate a complete config from the partial config input.
 
         Add minimal resource to config if available.
         """
         disturb = self._reset_times and partial_config == self.init_config
         # if not the first time to complete init_config, use random gaussian
-        config, space = complete_config(
-            partial_config, self.space, self, disturb, lower, upper
-        )
+        config, space = complete_config(partial_config, self.space, self, disturb, lower, upper)
         if partial_config == self.init_config:
             self._reset_times += 1
         if self._resource:
             config[self.resource_attr] = self.min_resource
         return config, space
 
-    def create(
-        self, init_config: Dict, obj: float, cost: float, space: Dict
-    ) -> Searcher:
+    def create(self, init_config: Dict, obj: float, cost: float, space: Dict) -> Searcher:
         # space is the subspace where the init_config is located
         flow2 = self.__class__(
             init_config,
             self.metric,
             self.mode,
             space,
             self.resource_attr,
@@ -314,38 +292,29 @@
             self.seed + 1,
             self.lexico_objectives,
         )
         if self.lexico_objectives is not None:
             flow2.best_obj = {}
             for k, v in obj.items():
                 flow2.best_obj[k] = (
-                    -v
-                    if self.lexico_objectives["modes"][
-                        self.lexico_objectives["metrics"].index(k)
-                    ]
-                    == "max"
-                    else v
+                    -v if self.lexico_objectives["modes"][self.lexico_objectives["metrics"].index(k)] == "max" else v
                 )
         else:
             flow2.best_obj = obj * self.metric_op  # minimize internally
         flow2.cost_incumbent = cost
         self.seed += 1
         return flow2
 
     def normalize(self, config, recursive=False) -> Dict:
         """normalize each dimension in config to [0,1]."""
-        return normalize(
-            config, self._space, self.best_config, self.incumbent, recursive
-        )
+        return normalize(config, self._space, self.best_config, self.incumbent, recursive)
 
     def denormalize(self, config):
         """denormalize each dimension in config from [0,1]."""
-        return denormalize(
-            config, self._space, self.best_config, self.incumbent, self._random
-        )
+        return denormalize(config, self._space, self.best_config, self.incumbent, self._random)
 
     def set_search_properties(
         self,
         metric: Optional[str] = None,
         mode: Optional[str] = None,
         config: Optional[Dict] = None,
     ) -> bool:
@@ -370,28 +339,21 @@
         obj_initial = self.lexico_objectives["metrics"][0]
         feasible_index = np.array([*range(len(self._histories[obj_initial]))])
         for k_metric in self.lexico_objectives["metrics"]:
             k_values = np.array(self._histories[k_metric])
             feasible_value = k_values.take(feasible_index)
             self._f_best[k_metric] = np.min(feasible_value)
             if not isinstance(self.lexico_objectives["tolerances"][k_metric], str):
-                tolerance_bound = (
-                    self._f_best[k_metric]
-                    + self.lexico_objectives["tolerances"][k_metric]
-                )
+                tolerance_bound = self._f_best[k_metric] + self.lexico_objectives["tolerances"][k_metric]
             else:
                 assert (
                     self.lexico_objectives["tolerances"][k_metric][-1] == "%"
                 ), "String tolerance of {} should use %% as the suffix".format(k_metric)
                 tolerance_bound = self._f_best[k_metric] * (
-                    1
-                    + 0.01
-                    * float(
-                        self.lexico_objectives["tolerances"][k_metric].replace("%", "")
-                    )
+                    1 + 0.01 * float(self.lexico_objectives["tolerances"][k_metric].replace("%", ""))
                 )
             feasible_index_filter = np.where(
                 feasible_value
                 <= max(
                     tolerance_bound,
                     self.lexico_objectives["targets"][k_metric],
                 )
@@ -405,41 +367,28 @@
                 self._histories[k].append(result[k])
             self.update_fbest()
             return True
         else:
             for k in self.lexico_objectives["metrics"]:
                 self._histories[k].append(result[k])
             self.update_fbest()
-            for k_metric, k_mode in zip(
-                self.lexico_objectives["metrics"], self.lexico_objectives["modes"]
-            ):
+            for k_metric, k_mode in zip(self.lexico_objectives["metrics"], self.lexico_objectives["modes"]):
                 k_target = (
                     self.lexico_objectives["targets"][k_metric]
                     if k_mode == "min"
                     else -self.lexico_objectives["targets"][k_metric]
                 )
                 if not isinstance(self.lexico_objectives["tolerances"][k_metric], str):
-                    tolerance_bound = (
-                        self._f_best[k_metric]
-                        + self.lexico_objectives["tolerances"][k_metric]
-                    )
+                    tolerance_bound = self._f_best[k_metric] + self.lexico_objectives["tolerances"][k_metric]
                 else:
                     assert (
                         self.lexico_objectives["tolerances"][k_metric][-1] == "%"
-                    ), "String tolerance of {} should use %% as the suffix".format(
-                        k_metric
-                    )
+                    ), "String tolerance of {} should use %% as the suffix".format(k_metric)
                     tolerance_bound = self._f_best[k_metric] * (
-                        1
-                        + 0.01
-                        * float(
-                            self.lexico_objectives["tolerances"][k_metric].replace(
-                                "%", ""
-                            )
-                        )
+                        1 + 0.01 * float(self.lexico_objectives["tolerances"][k_metric].replace("%", ""))
                     )
                 if (result[k_metric] < max(tolerance_bound, k_target)) and (
                     self.best_obj[k_metric]
                     < max(
                         tolerance_bound,
                         k_target,
                     )
@@ -453,17 +402,15 @@
                 if result[k_metr] == self.best_obj[k_metr]:
                     continue
                 elif result[k_metr] < self.best_obj[k_metr]:
                     return True
                 else:
                     return False
 
-    def on_trial_complete(
-        self, trial_id: str, result: Optional[Dict] = None, error: bool = False
-    ):
+    def on_trial_complete(self, trial_id: str, result: Optional[Dict] = None, error: bool = False):
         """
         Compare with incumbent.
         If better, move, reset num_complete and num_proposed.
         If not better and num_complete >= 2*dim, num_allowed += 2.
         """
         self.trial_count_complete += 1
         if not error and result:
@@ -508,29 +455,20 @@
                         self._trunc = min(self._trunc + 1, self.dim)
                     return
                 elif self._trunc:
                     self._trunc = max(self._trunc >> 1, 1)
         proposed_by = self._proposed_by.get(trial_id)
         if proposed_by == self.incumbent:
             self._num_complete4incumbent += 1
-            cost = (
-                result.get(self.cost_attr, 1)
-                if result
-                else self._trial_cost.get(trial_id)
-            )
+            cost = result.get(self.cost_attr, 1) if result else self._trial_cost.get(trial_id)
             if cost:
                 self._cost_complete4incumbent += cost
-            if (
-                self._num_complete4incumbent >= 2 * self.dim
-                and self._num_allowed4incumbent == 0
-            ):
+            if self._num_complete4incumbent >= 2 * self.dim and self._num_allowed4incumbent == 0:
                 self._num_allowed4incumbent = 2
-            if self._num_complete4incumbent == self.dir and (
-                not self._resource or self._resource == self.max_resource
-            ):
+            if self._num_complete4incumbent == self.dir and (not self._resource or self._resource == self.max_resource):
                 self._num_complete4incumbent -= 2
                 self._num_allowed4incumbent = max(self._num_allowed4incumbent, 2)
 
     def on_trial_result(self, trial_id: str, result: Dict):
         """Early update of incumbent."""
         if result:
             obj = (
@@ -589,62 +527,49 @@
         # TODO: better decouple FLOW2 config suggestion and stepsize update
         self.trial_count_proposed += 1
         if (
             self._num_complete4incumbent > 0
             and self.cost_incumbent
             and self._resource
             and self._resource < self.max_resource
-            and (
-                self._cost_complete4incumbent
-                >= self.cost_incumbent * self.resource_multiple_factor
-            )
+            and (self._cost_complete4incumbent >= self.cost_incumbent * self.resource_multiple_factor)
         ):
             return self._increase_resource(trial_id)
         self._num_allowed4incumbent -= 1
         move = self.incumbent.copy()
         if self._direction_tried is not None:
             # return negative direction
             for i, key in enumerate(self._tunable_keys):
                 move[key] -= self._direction_tried[i]
             self._direction_tried = None
         else:
             # propose a new direction
-            self._direction_tried = (
-                self.rand_vector_unit_sphere(self.dim, self._trunc) * self.step
-            )
+            self._direction_tried = self.rand_vector_unit_sphere(self.dim, self._trunc) * self.step
             for i, key in enumerate(self._tunable_keys):
                 move[key] += self._direction_tried[i]
         self._project(move)
         config = self.denormalize(move)
         self._proposed_by[trial_id] = self.incumbent
         self._configs[trial_id] = (config, self.step)
         self._num_proposedby_incumbent += 1
         best_config = self.best_config
         if self._init_phase:
             if self._direction_tried is None:
                 if self._same:
-                    same = not any(
-                        key not in best_config or value != best_config[key]
-                        for key, value in config.items()
-                    )
+                    same = not any(key not in best_config or value != best_config[key] for key, value in config.items())
 
                     if same:
                         # increase step size
                         self.step += self.STEPSIZE
                         self.step = min(self.step, self.step_ub)
             else:
-                same = not any(
-                    key not in best_config or value != best_config[key]
-                    for key, value in config.items()
-                )
+                same = not any(key not in best_config or value != best_config[key] for key, value in config.items())
 
                 self._same = same
-        if self._num_proposedby_incumbent == self.dir and (
-            not self._resource or self._resource == self.max_resource
-        ):
+        if self._num_proposedby_incumbent == self.dir and (not self._resource or self._resource == self.max_resource):
             # check stuck condition if using max resource
             self._num_proposedby_incumbent -= 2
             self._init_phase = False
             if self.step < self.step_lower_bound:
                 return None
                 # decrease step size
             self._oldK = self._K or self._iter_best_config
@@ -710,17 +635,15 @@
             value = config[key]
             if key == self.resource_attr:
                 value_list.append(value)
             else:
                 # key must be in space
                 domain = space[key]
                 if self.hierarchical and not (
-                    domain is None
-                    or type(domain) in (str, int, float)
-                    or isinstance(domain, sample.Domain)
+                    domain is None or type(domain) in (str, int, float) or isinstance(domain, sample.Domain)
                 ):
                     # not domain or hashable
                     # get rid of list type for hierarchical search space.
                     continue
                 if isinstance(domain, sample.Integer):
                     value_list.append(int(round(value)))
                 else:
@@ -742,14 +665,9 @@
         if self._resource and config1[self.resource_attr] > config2[self.resource_attr]:
             # resource will not decrease
             return False
         for key in self._unordered_cat_hp:
             # unordered cat choice is hard to reach by chance
             if config1[key] != config2.get(key):
                 return False
-        delta = np.array(
-            [
-                incumbent1[key] - incumbent2.get(key, np.inf)
-                for key in self._tunable_keys
-            ]
-        )
+        delta = np.array([incumbent1[key] - incumbent2.get(key, np.inf) for key in self._tunable_keys])
         return np.linalg.norm(delta) <= self.step
```

### Comparing `FLAML-1.2.0/flaml/tune/searcher/online_searcher.py` & `FLAML-1.2.1/flaml/tune/searcher/online_searcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,17 +124,15 @@
         self._searcher_trialid_to_trialid = {}
 
         # value: trial_id, key: searcher_trial_id
         self._trialid_to_searcher_trial_id = {}
 
         self._challenger_list = []
         # initialize the search in set_search_properties
-        self.set_search_properties(
-            setting={self.CHAMPION_TRIAL_NAME: None}, init_call=True
-        )
+        self.set_search_properties(setting={self.CHAMPION_TRIAL_NAME: None}, init_call=True)
         logger.debug("using random seed %s in config oracle", self._seed)
 
     def set_search_properties(
         self,
         metric: Optional[str] = None,
         mode: Optional[str] = None,
         config: Optional[Dict] = {},
@@ -198,24 +196,20 @@
         hyperparameter_config_groups = []
         searcher_trial_ids_groups = []
         nonpoly_config = {}
         for k, v in seed_config.items():
             config_domain = self._space[k]
             if isinstance(config_domain, PolynomialExpansionSet):
                 # get candidate configs for hyperparameters of the PolynomialExpansionSet type
-                partial_new_configs = self._generate_independent_hp_configs(
-                    k, v, config_domain
-                )
+                partial_new_configs = self._generate_independent_hp_configs(k, v, config_domain)
                 if partial_new_configs:
                     hyperparameter_config_groups.append(partial_new_configs)
                     # does not have searcher_trial_ids
                     searcher_trial_ids_groups.append([])
-            elif isinstance(config_domain, Float) or isinstance(
-                config_domain, Categorical
-            ):
+            elif isinstance(config_domain, Float) or isinstance(config_domain, Categorical):
                 # otherwise we need to deal with them in group
                 nonpoly_config[k] = v
                 if k not in self._space_of_nonpoly_hp:
                     self._space_of_nonpoly_hp[k] = self._space[k]
 
         # -----------generate partial new configs for non-PolynomialExpansionSet hyperparameters
         if nonpoly_config:
@@ -225,57 +219,41 @@
                 if seed_config_trial_id not in self._searcher_for_nonpoly_hp:
                     self._searcher_for_nonpoly_hp[seed_config_trial_id] = CFO(
                         space=self._space_of_nonpoly_hp,
                         points_to_evaluate=[nonpoly_config],
                         metric=self.CFO_SEARCHER_METRIC_NAME,
                     )
                     # initialize the search in set_search_properties
-                    self._searcher_for_nonpoly_hp[
-                        seed_config_trial_id
-                    ].set_search_properties(
+                    self._searcher_for_nonpoly_hp[seed_config_trial_id].set_search_properties(
                         setting={"metric_target": self.CFO_SEARCHER_LARGE_LOSS}
                     )
                     # We need to call this for once, such that the seed config in points_to_evaluate will be called
                     # to be tried
-                    self._searcher_for_nonpoly_hp[seed_config_trial_id].suggest(
-                        seed_config_searcher_trial_id
-                    )
+                    self._searcher_for_nonpoly_hp[seed_config_trial_id].suggest(seed_config_searcher_trial_id)
                 # assuming minimization
-                if (
-                    self._searcher_for_nonpoly_hp[seed_config_trial_id].metric_target
-                    is None
-                ):
+                if self._searcher_for_nonpoly_hp[seed_config_trial_id].metric_target is None:
                     pseudo_loss = self.CFO_SEARCHER_LARGE_LOSS
                 else:
-                    pseudo_loss = (
-                        self._searcher_for_nonpoly_hp[
-                            seed_config_trial_id
-                        ].metric_target
-                        * 0.95
-                    )
+                    pseudo_loss = self._searcher_for_nonpoly_hp[seed_config_trial_id].metric_target * 0.95
                 pseudo_result_to_report = {}
                 for k, v in nonpoly_config.items():
                     pseudo_result_to_report["config/" + str(k)] = v
                 pseudo_result_to_report[self.CFO_SEARCHER_METRIC_NAME] = pseudo_loss
                 pseudo_result_to_report["time_total_s"] = 1
                 self._searcher_for_nonpoly_hp[seed_config_trial_id].on_trial_complete(
                     seed_config_searcher_trial_id, result=pseudo_result_to_report
                 )
                 while len(partial_new_nonpoly_configs) < self.NUMERICAL_NUM:
                     # suggest multiple times
                     new_searcher_trial_id = Trial.generate_id()
                     new_searcher_trial_ids.append(new_searcher_trial_id)
-                    suggestion = self._searcher_for_nonpoly_hp[
-                        seed_config_trial_id
-                    ].suggest(new_searcher_trial_id)
+                    suggestion = self._searcher_for_nonpoly_hp[seed_config_trial_id].suggest(new_searcher_trial_id)
                     if suggestion is not None:
                         partial_new_nonpoly_configs.append(suggestion)
-                logger.info(
-                    "partial_new_nonpoly_configs %s", partial_new_nonpoly_configs
-                )
+                logger.info("partial_new_nonpoly_configs %s", partial_new_nonpoly_configs)
             else:
                 raise NotImplementedError
             if partial_new_nonpoly_configs:
                 hyperparameter_config_groups.append(partial_new_nonpoly_configs)
                 searcher_trial_ids_groups.append(new_searcher_trial_ids)
         # ----------- coordinate generation of new challengers in the case of multiple groups
         new_trials = []
@@ -294,28 +272,22 @@
                 # instead set the searcher_trial_id to be None. When creating a trial from a config,
                 # a searcher_trial_id will be generated if None is provided.
                 # TODO: An alternative option is to generate a searcher_trial_id for each partial config
                 if searcher_trial_ids_groups[i]:
                     new_searcher_trial_id = searcher_trial_ids_groups[i][j]
                 else:
                     new_searcher_trial_id = None
-                new_trial = self._create_trial_from_config(
-                    new_seed_config, new_searcher_trial_id
-                )
+                new_trial = self._create_trial_from_config(new_seed_config, new_searcher_trial_id)
                 new_trials.append(new_trial)
         logger.info("new_configs %s", [t.trial_id for t in new_trials])
         return new_trials
 
-    def _generate_independent_hp_configs(
-        self, hp_name, current_config_value, config_domain
-    ) -> List:
+    def _generate_independent_hp_configs(self, hp_name, current_config_value, config_domain) -> List:
         if isinstance(config_domain, PolynomialExpansionSet):
-            seed_interactions = list(current_config_value) + list(
-                config_domain.init_monomials
-            )
+            seed_interactions = list(current_config_value) + list(config_domain.init_monomials)
             logger.info(
                 "**Important** Seed namespaces (singletons and interactions): %s",
                 seed_interactions,
             )
             logger.info("current_config_value %s", current_config_value)
             configs = self._generate_poly_expansion_sets(
                 seed_interactions,
@@ -336,21 +308,15 @@
         allow_self_inter,
         highest_poly_order,
         interaction_num_to_add,
     ):
         champion_all_combinations = self._generate_all_comb(
             seed_interactions, order, allow_self_inter, highest_poly_order
         )
-        space = sorted(
-            list(
-                itertools.combinations(
-                    champion_all_combinations, interaction_num_to_add
-                )
-            )
-        )
+        space = sorted(list(itertools.combinations(champion_all_combinations, interaction_num_to_add)))
         self._random_state.shuffle(space)
         candidate_configs = [set(seed_interactions) | set(item) for item in space]
         final_candidate_configs = []
         for c in candidate_configs:
             new_c = set([e for e in c if len(e) > 1])
             final_candidate_configs.append(new_c)
         return final_candidate_configs
@@ -409,19 +375,14 @@
             interactions = get_interactions(interactions, seed_interactions)
             seed_interaction_order -= 1
             all_interactions += interactions
         if not allow_self_inter:
             all_interactions_no_self_inter = []
             for s in all_interactions:
                 s_no_inter = strip_self_inter(s)
-                if (
-                    len(s_no_inter) > 1
-                    and s_no_inter not in all_interactions_no_self_inter
-                ):
+                if len(s_no_inter) > 1 and s_no_inter not in all_interactions_no_self_inter:
                     all_interactions_no_self_inter.append(s_no_inter)
             all_interactions = all_interactions_no_self_inter
         if highest_poly_order is not None:
-            all_interactions = [
-                c for c in all_interactions if len(c) <= highest_poly_order
-            ]
+            all_interactions = [c for c in all_interactions if len(c) <= highest_poly_order]
         logger.info("all_combinations %s", all_interactions)
         return all_interactions
```

### Comparing `FLAML-1.2.0/flaml/tune/searcher/search_thread.py` & `FLAML-1.2.1/flaml/tune/searcher/search_thread.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,36 +34,28 @@
         eps: Optional[float] = 1.0,
     ):
         """When search_alg is omitted, use local search FLOW2."""
         self._search_alg = search_alg
         self._is_ls = isinstance(search_alg, FLOW2)
         self._mode = mode
         self._metric_op = 1 if mode == "min" else -1
-        self.cost_best = self.cost_last = self.cost_total = self.cost_best1 = getattr(
-            search_alg, "cost_incumbent", 0
-        )
+        self.cost_best = self.cost_last = self.cost_total = self.cost_best1 = getattr(search_alg, "cost_incumbent", 0)
         self._eps = eps
         self.cost_best2 = 0
-        self.obj_best1 = self.obj_best2 = getattr(
-            search_alg, "best_obj", np.inf
-        )  # inherently minimize
+        self.obj_best1 = self.obj_best2 = getattr(search_alg, "best_obj", np.inf)  # inherently minimize
         self.best_result = None
         # eci: estimated cost for improvement
         self.eci = self.cost_best
         self.priority = self.speed = 0
         self._init_config = True
         self.running = 0  # the number of running trials from the thread
         self.cost_attr = cost_attr
         if search_alg:
             self.space = self._space = search_alg.space  # unflattened space
-            if (
-                self.space
-                and not isinstance(search_alg, FLOW2)
-                and isinstance(search_alg._space, dict)
-            ):
+            if self.space and not isinstance(search_alg, FLOW2) and isinstance(search_alg._space, dict):
                 # remember const config
                 self._const = add_cost_to_space(self.space, {}, {})
 
     def suggest(self, trial_id: str) -> Optional[Dict]:
         """Use the suggest() of the underlying search algorithm."""
         if isinstance(self._search_alg, FLOW2):
             config = self._search_alg.suggest(trial_id)
@@ -72,79 +64,64 @@
                 config = self._search_alg.suggest(trial_id)
                 if isinstance(self._search_alg._space, dict):
                     config.update(self._const)
                 else:
                     # define by run
                     config, self.space = unflatten_hierarchical(config, self._space)
             except FloatingPointError:
-                logger.warning(
-                    "The global search method raises FloatingPointError. "
-                    "Ignoring for this iteration."
-                )
+                logger.warning("The global search method raises FloatingPointError. " "Ignoring for this iteration.")
                 config = None
         if config is not None:
             self.running += 1
         return config
 
     def update_priority(self, eci: Optional[float] = 0):
         # optimistic projection
         self.priority = eci * self.speed - self.obj_best1
 
     def update_eci(self, metric_target: float, max_speed: Optional[float] = np.inf):
         # calculate eci: estimated cost for improvement over metric_target
         best_obj = metric_target * self._metric_op
         if not self.speed:
             self.speed = max_speed
-        self.eci = max(
-            self.cost_total - self.cost_best1, self.cost_best1 - self.cost_best2
-        )
+        self.eci = max(self.cost_total - self.cost_best1, self.cost_best1 - self.cost_best2)
         if self.obj_best1 > best_obj and self.speed > 0:
             self.eci = max(self.eci, 2 * (self.obj_best1 - best_obj) / self.speed)
 
     def _update_speed(self):
         # calculate speed; use 0 for invalid speed temporarily
         if self.obj_best2 > self.obj_best1:
             # discount the speed if there are unfinished trials
             self.speed = (
-                (self.obj_best2 - self.obj_best1)
-                / self.running
-                / (max(self.cost_total - self.cost_best2, self._eps))
+                (self.obj_best2 - self.obj_best1) / self.running / (max(self.cost_total - self.cost_best2, self._eps))
             )
         else:
             self.speed = 0
 
-    def on_trial_complete(
-        self, trial_id: str, result: Optional[Dict] = None, error: bool = False
-    ):
+    def on_trial_complete(self, trial_id: str, result: Optional[Dict] = None, error: bool = False):
         """Update the statistics of the thread."""
         if not self._search_alg:
             return
-        if not hasattr(self._search_alg, "_ot_trials") or (
-            not error and trial_id in self._search_alg._ot_trials
-        ):
+        if not hasattr(self._search_alg, "_ot_trials") or (not error and trial_id in self._search_alg._ot_trials):
             # optuna doesn't handle error
             if self._is_ls or not self._init_config:
                 try:
                     self._search_alg.on_trial_complete(trial_id, result, error)
                 except RuntimeError as e:
                     # rs is used in place of optuna sometimes
-                    if not str(e).endswith(
-                        "has already finished and can not be updated."
-                    ):
+                    if not str(e).endswith("has already finished and can not be updated."):
                         raise e
             else:
                 # init config is not proposed by self._search_alg
                 # under this thread
                 self._init_config = False
         if result:
             self.cost_last = result.get(self.cost_attr, 1)
             self.cost_total += self.cost_last
-            if self._search_alg.metric in result and (
-                getattr(self._search_alg, "lexico_objectives", None) is None
-            ):
+            if self._search_alg.metric in result and (getattr(self._search_alg, "lexico_objectives", None) is None):
                 # TODO: Improve this behavior. When lexico_objectives is provided to CFO,
                 # related variables are not callable.
                 obj = result[self._search_alg.metric] * self._metric_op
                 if obj < self.obj_best1 or self.best_result is None:
                     self.cost_best2 = self.cost_best1
                     self.cost_best1 = self.cost_total
                     self.obj_best2 = obj if np.isinf(self.obj_best1) else self.obj_best1
@@ -158,17 +135,15 @@
         self.running -= 1
         assert self.running >= 0
 
     def on_trial_result(self, trial_id: str, result: Dict):
         # TODO update the statistics of the thread with partial result?
         if not self._search_alg:
             return
-        if not hasattr(self._search_alg, "_ot_trials") or (
-            trial_id in self._search_alg._ot_trials
-        ):
+        if not hasattr(self._search_alg, "_ot_trials") or (trial_id in self._search_alg._ot_trials):
             try:
                 self._search_alg.on_trial_result(trial_id, result)
             except RuntimeError as e:
                 # rs is used in place of optuna sometimes
                 if not str(e).endswith("has already finished and can not be updated."):
                     raise e
         new_cost = result.get(self.cost_attr, 1)
```

### Comparing `FLAML-1.2.0/flaml/tune/searcher/suggestion.py` & `FLAML-1.2.1/flaml/tune/searcher/suggestion.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,30 +108,24 @@
         self._metric = metric
         self._mode = mode
 
         if not mode or not metric:
             # Early return to avoid assertions
             return
 
-        assert isinstance(
-            metric, type(mode)
-        ), "metric and mode must be of the same type"
+        assert isinstance(metric, type(mode)), "metric and mode must be of the same type"
         if isinstance(mode, str):
             assert mode in ["min", "max"], "if `mode` is a str must be 'min' or 'max'!"
         elif isinstance(mode, list):
             assert len(mode) == len(metric), "Metric and mode must be the same length"
-            assert all(
-                mod in ["min", "max", "obs"] for mod in mode
-            ), "All of mode must be 'min' or 'max' or 'obs'!"
+            assert all(mod in ["min", "max", "obs"] for mod in mode), "All of mode must be 'min' or 'max' or 'obs'!"
         else:
             raise ValueError("Mode must either be a list or string")
 
-    def set_search_properties(
-        self, metric: Optional[str], mode: Optional[str], config: Dict
-    ) -> bool:
+    def set_search_properties(self, metric: Optional[str], mode: Optional[str], config: Dict) -> bool:
         """Pass search properties to searcher.
         This method acts as an alternative to instantiating search algorithms
         with their own specific search spaces. Instead they can accept a
         Tune config through this method. A searcher should return ``True``
         if setting the config was successful, or ``False`` if it was
         unsuccessful, e.g. when the search space has already been set.
         Args:
@@ -189,50 +183,41 @@
     def __init__(self, searcher: Searcher, max_concurrent: int, batch: bool = False):
         assert type(max_concurrent) is int and max_concurrent > 0
         self.searcher = searcher
         self.max_concurrent = max_concurrent
         self.batch = batch
         self.live_trials = set()
         self.cached_results = {}
-        super(ConcurrencyLimiter, self).__init__(
-            metric=self.searcher.metric, mode=self.searcher.mode
-        )
+        super(ConcurrencyLimiter, self).__init__(metric=self.searcher.metric, mode=self.searcher.mode)
 
     def suggest(self, trial_id: str) -> Optional[Dict]:
-        assert (
-            trial_id not in self.live_trials
-        ), f"Trial ID {trial_id} must be unique: already found in set."
+        assert trial_id not in self.live_trials, f"Trial ID {trial_id} must be unique: already found in set."
         if len(self.live_trials) >= self.max_concurrent:
             logger.debug(
-                f"Not providing a suggestion for {trial_id} due to "
-                "concurrency limit: %s/%s.",
+                f"Not providing a suggestion for {trial_id} due to " "concurrency limit: %s/%s.",
                 len(self.live_trials),
                 self.max_concurrent,
             )
             return
 
         suggestion = self.searcher.suggest(trial_id)
         if suggestion not in (None, Searcher.FINISHED):
             self.live_trials.add(trial_id)
         return suggestion
 
-    def on_trial_complete(
-        self, trial_id: str, result: Optional[Dict] = None, error: bool = False
-    ):
+    def on_trial_complete(self, trial_id: str, result: Optional[Dict] = None, error: bool = False):
         if trial_id not in self.live_trials:
             return
         elif self.batch:
             self.cached_results[trial_id] = (result, error)
             if len(self.cached_results) == self.max_concurrent:
                 # Update the underlying searcher once the
                 # full batch is completed.
                 for trial_id, (result, error) in self.cached_results.items():
-                    self.searcher.on_trial_complete(
-                        trial_id, result=result, error=error
-                    )
+                    self.searcher.on_trial_complete(trial_id, result=result, error=error)
                     self.live_trials.remove(trial_id)
                 self.cached_results = {}
             else:
                 return
         else:
             self.searcher.on_trial_complete(trial_id, result=result, error=error)
             self.live_trials.remove(trial_id)
@@ -253,17 +238,15 @@
 
     def on_pause(self, trial_id: str):
         self.searcher.on_pause(trial_id)
 
     def on_unpause(self, trial_id: str):
         self.searcher.on_unpause(trial_id)
 
-    def set_search_properties(
-        self, metric: Optional[str], mode: Optional[str], config: Dict
-    ) -> bool:
+    def set_search_properties(self, metric: Optional[str], mode: Optional[str], config: Dict) -> bool:
         return self.searcher.set_search_properties(metric, mode, config)
 
 
 try:
     import optuna as ot
     from optuna.distributions import BaseDistribution as OptunaDistribution
     from optuna.samplers import BaseSampler
@@ -297,40 +280,29 @@
     parameters.
     If ``validate_point_name_lengths`` is False, the equality of lengths
     between ``points_to_evaluate`` and ``parameter_names`` will not be
     validated.
     """
     if points_to_evaluate:
         if not isinstance(points_to_evaluate, list):
-            raise TypeError(
-                "points_to_evaluate expected to be a list, got {}.".format(
-                    type(points_to_evaluate)
-                )
-            )
+            raise TypeError("points_to_evaluate expected to be a list, got {}.".format(type(points_to_evaluate)))
         for point in points_to_evaluate:
             if not isinstance(point, (dict, list)):
-                raise TypeError(
-                    f"points_to_evaluate expected to include list or dict, "
-                    f"got {point}."
-                )
+                raise TypeError(f"points_to_evaluate expected to include list or dict, " f"got {point}.")
 
             if validate_point_name_lengths and (not len(point) == len(parameter_names)):
                 raise ValueError(
                     "Dim of point {}".format(point)
                     + " and parameter_names {}".format(parameter_names)
                     + " do not match."
                 )
 
     if points_to_evaluate and evaluated_rewards:
         if not isinstance(evaluated_rewards, list):
-            raise TypeError(
-                "evaluated_rewards expected to be a list, got {}.".format(
-                    type(evaluated_rewards)
-                )
-            )
+            raise TypeError("evaluated_rewards expected to be a list, got {}.".format(type(evaluated_rewards)))
         if not len(evaluated_rewards) == len(points_to_evaluate):
             raise ValueError(
                 "Dim of evaluated_rewards {}".format(evaluated_rewards)
                 + " and points_to_evaluate {}".format(points_to_evaluate)
                 + " do not match."
             )
 
@@ -457,24 +429,20 @@
         mode: Optional[str] = None,
         points_to_evaluate: Optional[List[Dict]] = None,
         sampler: Optional["BaseSampler"] = None,
         seed: Optional[int] = None,
         evaluated_rewards: Optional[List] = None,
     ):
         assert ot is not None, "Optuna must be installed! Run `pip install optuna`."
-        super(OptunaSearch, self).__init__(
-            metric=metric, mode=mode, max_concurrent=None, use_early_stopped_trials=None
-        )
+        super(OptunaSearch, self).__init__(metric=metric, mode=mode, max_concurrent=None, use_early_stopped_trials=None)
 
         if isinstance(space, dict) and space:
             resolved_vars, domain_vars, grid_vars = parse_spec_vars(space)
             if domain_vars or grid_vars:
-                logger.warning(
-                    UNRESOLVED_SEARCH_SPACE.format(par="space", cls=type(self).__name__)
-                )
+                logger.warning(UNRESOLVED_SEARCH_SPACE.format(par="space", cls=type(self).__name__))
                 space = self.convert_search_space(space)
             else:
                 # Flatten to support nested dicts
                 space = flatten_dict(space, "/")
 
         self._space = space
 
@@ -489,16 +457,15 @@
                 "`seed` parameter has to be passed to the sampler directly "
                 "and will be ignored."
             )
 
         self._sampler = sampler or ot.samplers.TPESampler(seed=seed)
 
         assert isinstance(self._sampler, BaseSampler), (
-            "You can only pass an instance of `optuna.samplers.BaseSampler` "
-            "as a sampler to `OptunaSearcher`."
+            "You can only pass an instance of `optuna.samplers.BaseSampler` " "as a sampler to `OptunaSearcher`."
         )
 
         self._ot_trials = {}
         self._ot_study = None
         if self._space:
             self._setup_study(mode)
 
@@ -523,25 +490,21 @@
             validate_warmstart(
                 self._space,
                 self._points_to_evaluate,
                 self._evaluated_rewards,
                 validate_point_name_lengths=not callable(self._space),
             )
             if self._evaluated_rewards:
-                for point, reward in zip(
-                    self._points_to_evaluate, self._evaluated_rewards
-                ):
+                for point, reward in zip(self._points_to_evaluate, self._evaluated_rewards):
                     self.add_evaluated_point(point, reward)
             else:
                 for point in self._points_to_evaluate:
                     self._ot_study.enqueue_trial(point)
 
-    def set_search_properties(
-        self, metric: Optional[str], mode: Optional[str], config: Dict
-    ) -> bool:
+    def set_search_properties(self, metric: Optional[str], mode: Optional[str], config: Dict) -> bool:
         if self._space:
             return False
         space = self.convert_search_space(config)
         self._space = space
         if metric:
             self._metric = metric
         if mode:
@@ -581,68 +544,56 @@
                     "define-by-run function passed in the `space` argument "
                     "was not a `str`."
                 )
         return {**captor.captured_values, **ret} if ret else captor.captured_values
 
     def suggest(self, trial_id: str) -> Optional[Dict]:
         if not self._space:
-            raise RuntimeError(
-                UNDEFINED_SEARCH_SPACE.format(
-                    cls=self.__class__.__name__, space="space"
-                )
-            )
+            raise RuntimeError(UNDEFINED_SEARCH_SPACE.format(cls=self.__class__.__name__, space="space"))
         if not self._metric or not self._mode:
             raise RuntimeError(
-                UNDEFINED_METRIC_MODE.format(
-                    cls=self.__class__.__name__, metric=self._metric, mode=self._mode
-                )
+                UNDEFINED_METRIC_MODE.format(cls=self.__class__.__name__, metric=self._metric, mode=self._mode)
             )
 
         if isinstance(self._space, list):
             # Keep for backwards compatibility
             # Deprecate: 1.5
             if trial_id not in self._ot_trials:
                 self._ot_trials[trial_id] = self._ot_study.ask()
 
             ot_trial = self._ot_trials[trial_id]
 
             # getattr will fetch the trial.suggest_ function on Optuna trials
             params = {
-                args[0]
-                if len(args) > 0
-                else kwargs["name"]: getattr(ot_trial, fn)(*args, **kwargs)
+                args[0] if len(args) > 0 else kwargs["name"]: getattr(ot_trial, fn)(*args, **kwargs)
                 for (fn, args, kwargs) in self._space
             }
         elif callable(self._space):
             if trial_id not in self._ot_trials:
                 self._ot_trials[trial_id] = self._ot_study.ask()
 
             ot_trial = self._ot_trials[trial_id]
 
             params = self._suggest_from_define_by_run_func(self._space, ot_trial)
         else:
             # Use Optuna ask interface (since version 2.6.0)
             if trial_id not in self._ot_trials:
-                self._ot_trials[trial_id] = self._ot_study.ask(
-                    fixed_distributions=self._space
-                )
+                self._ot_trials[trial_id] = self._ot_study.ask(fixed_distributions=self._space)
             ot_trial = self._ot_trials[trial_id]
             params = ot_trial.params
 
         return unflatten_dict(params)
 
     def on_trial_result(self, trial_id: str, result: Dict):
         metric = result[self.metric]
         step = result[TRAINING_ITERATION]
         ot_trial = self._ot_trials[trial_id]
         ot_trial.report(metric, step)
 
-    def on_trial_complete(
-        self, trial_id: str, result: Optional[Dict] = None, error: bool = False
-    ):
+    def on_trial_complete(self, trial_id: str, result: Optional[Dict] = None, error: bool = False):
         ot_trial = self._ot_trials[trial_id]
 
         val = result.get(self.metric, None) if result else None
         ot_trial_state = OptunaTrialState.COMPLETE
         if val is None:
             if error:
                 ot_trial_state = OptunaTrialState.FAIL
@@ -658,36 +609,28 @@
         parameters: Dict,
         value: float,
         error: bool = False,
         pruned: bool = False,
         intermediate_values: Optional[List[float]] = None,
     ):
         if not self._space:
-            raise RuntimeError(
-                UNDEFINED_SEARCH_SPACE.format(
-                    cls=self.__class__.__name__, space="space"
-                )
-            )
+            raise RuntimeError(UNDEFINED_SEARCH_SPACE.format(cls=self.__class__.__name__, space="space"))
         if not self._metric or not self._mode:
             raise RuntimeError(
-                UNDEFINED_METRIC_MODE.format(
-                    cls=self.__class__.__name__, metric=self._metric, mode=self._mode
-                )
+                UNDEFINED_METRIC_MODE.format(cls=self.__class__.__name__, metric=self._metric, mode=self._mode)
             )
 
         ot_trial_state = OptunaTrialState.COMPLETE
         if error:
             ot_trial_state = OptunaTrialState.FAIL
         elif pruned:
             ot_trial_state = OptunaTrialState.PRUNED
 
         if intermediate_values:
-            intermediate_values_dict = {
-                i: value for i, value in enumerate(intermediate_values)
-            }
+            intermediate_values_dict = {i: value for i, value in enumerate(intermediate_values)}
         else:
             intermediate_values_dict = None
 
         trial = ot.trial.create_trial(
             state=ot_trial_state,
             value=value,
             params=parameters,
@@ -732,18 +675,15 @@
     def convert_search_space(spec: Dict) -> Dict[str, Any]:
         resolved_vars, domain_vars, grid_vars = parse_spec_vars(spec)
 
         if not domain_vars and not grid_vars:
             return {}
 
         if grid_vars:
-            raise ValueError(
-                "Grid search parameters cannot be automatically converted "
-                "to an Optuna search space."
-            )
+            raise ValueError("Grid search parameters cannot be automatically converted " "to an Optuna search space.")
 
         # Flatten and resolve again after checking for grid search.
         spec = flatten_dict(spec, prevent_delimiter=True)
         resolved_vars, domain_vars, grid_vars = parse_spec_vars(spec)
 
         def resolve_value(domain: Domain) -> ot.distributions.BaseDistribution:
             quantize = None
@@ -762,26 +702,20 @@
             if isinstance(domain, Float):
                 if isinstance(sampler, LogUniform):
                     if quantize:
                         logger.warning(
                             "Optuna does not support both quantization and "
                             "sampling from LogUniform. Dropped quantization."
                         )
-                    return ot.distributions.LogUniformDistribution(
-                        domain.lower, domain.upper
-                    )
+                    return ot.distributions.LogUniformDistribution(domain.lower, domain.upper)
 
                 elif isinstance(sampler, Uniform):
                     if quantize:
-                        return ot.distributions.DiscreteUniformDistribution(
-                            domain.lower, domain.upper, quantize
-                        )
-                    return ot.distributions.UniformDistribution(
-                        domain.lower, domain.upper
-                    )
+                        return ot.distributions.DiscreteUniformDistribution(domain.lower, domain.upper, quantize)
+                    return ot.distributions.UniformDistribution(domain.lower, domain.upper)
 
             elif isinstance(domain, Integer):
                 if isinstance(sampler, LogUniform):
                     return ot.distributions.IntLogUniformDistribution(
                         domain.lower, domain.upper - 1, step=quantize or 1
                     )
                 elif isinstance(sampler, Uniform):
@@ -794,16 +728,14 @@
                     )
             elif isinstance(domain, Categorical):
                 if isinstance(sampler, Uniform):
                     return ot.distributions.CategoricalDistribution(domain.categories)
 
             raise ValueError(
                 "Optuna search does not support parameters of type "
-                "`{}` with samplers of type `{}`".format(
-                    type(domain).__name__, type(domain.sampler).__name__
-                )
+                "`{}` with samplers of type `{}`".format(type(domain).__name__, type(domain.sampler).__name__)
             )
 
         # Parameter name is e.g. "a/b/c" for nested dicts
         values = {"/".join(path): resolve_value(domain) for path, domain in domain_vars}
 
         return values
```

### Comparing `FLAML-1.2.0/flaml/tune/searcher/variant_generator.py` & `FLAML-1.2.1/flaml/tune/searcher/variant_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,31 +139,25 @@
             # Not all variables have been resolved, but remove those that have
             # from the `to_resolve` list.
             to_resolve = [(r, d) for r, d in to_resolve if r not in resolved_vars]
     grid_search = _grid_search_generator(spec, grid_vars)
     for resolved_spec in grid_search:
         if not constant_grid_search or not all_resolved:
             # In this path, we sample the remaining random variables
-            _, resolved_vars = _resolve_domain_vars(
-                resolved_spec, to_resolve, random_state=random_state
-            )
+            _, resolved_vars = _resolve_domain_vars(resolved_spec, to_resolve, random_state=random_state)
 
         for resolved, spec in _generate_variants(
             resolved_spec,
             constant_grid_search=constant_grid_search,
             random_state=random_state,
         ):
             for path, value in grid_vars:
                 resolved_vars[path] = _get_value(spec, path)
             for k, v in resolved.items():
-                if (
-                    k in resolved_vars
-                    and v != resolved_vars[k]
-                    and _is_resolved(resolved_vars[k])
-                ):
+                if k in resolved_vars and v != resolved_vars[k] and _is_resolved(resolved_vars[k]):
                     raise ValueError(
                         "The variable `{}` could not be unambiguously "
                         "resolved to a single value. Consider simplifying "
                         "your configuration.".format(k)
                     )
                 resolved_vars[k] = v
             yield resolved_vars, spec
@@ -193,17 +187,15 @@
     while error and num_passes < _MAX_RESOLUTION_PASSES:
         num_passes += 1
         error = False
         for path, domain in domain_vars:
             if path in resolved:
                 continue
             try:
-                value = domain.sample(
-                    _UnresolvedAccessGuard(spec), random_state=random_state
-                )
+                value = domain.sample(_UnresolvedAccessGuard(spec), random_state=random_state)
             except RecursiveDependencyError as e:
                 error = e
             # except Exception:
             #     raise ValueError(
             #         "Failed to evaluate expression: {}: {}".format(path, domain)
             #     )
             else:
@@ -213,17 +205,15 @@
         if not allow_fail:
             raise error
         else:
             return False, resolved
     return True, resolved
 
 
-def _grid_search_generator(
-    unresolved_spec: Dict, grid_vars: List
-) -> Generator[Dict, None, None]:
+def _grid_search_generator(unresolved_spec: Dict, grid_vars: List) -> Generator[Dict, None, None]:
     value_indices = [0] * len(grid_vars)
 
     def increment(i):
         value_indices[i] += 1
         if value_indices[i] >= len(grid_vars[i][1]):
             value_indices[i] = 0
             if i + 1 < len(value_indices):
@@ -256,17 +246,15 @@
     if isinstance(v, (Domain, RayDomain)):
         # Domain to sample from
         return False, v
     elif isinstance(v, dict) and len(v) == 1 and "grid_search" in v:
         # Grid search values
         grid_values = v["grid_search"]
         if not isinstance(grid_values, list):
-            raise TuneError(
-                "Grid search expected list of values, got: {}".format(grid_values)
-            )
+            raise TuneError("Grid search expected list of values, got: {}".format(grid_values))
         return False, Categorical(grid_values).grid()
     return True, v
 
 
 def _split_resolved_unresolved_values(
     spec: Dict,
 ) -> Tuple[Dict[Tuple, Any], Dict[Tuple, Any]]:
@@ -314,17 +302,15 @@
     def __init__(self, *args, **kwds):
         super(_UnresolvedAccessGuard, self).__init__(*args, **kwds)
         self.__dict__ = self
 
     def __getattribute__(self, item):
         value = dict.__getattribute__(self, item)
         if not _is_resolved(value):
-            raise RecursiveDependencyError(
-                "`{}` recursively depends on {}".format(item, value)
-            )
+            raise RecursiveDependencyError("`{}` recursively depends on {}".format(item, value))
         elif isinstance(value, dict):
             return _UnresolvedAccessGuard(value)
         else:
             return value
 
 
 class RecursiveDependencyError(Exception):
```

### Comparing `FLAML-1.2.0/flaml/tune/space.py` & `FLAML-1.2.1/flaml/tune/space.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,23 +66,19 @@
                 if quantize:
                     trial.suggest_float(key, domain.lower, domain.upper, step=quantize)
                 else:
                     trial.suggest_float(key, domain.lower, domain.upper)
             else:
                 raise ValueError(
                     "Optuna search does not support parameters of type "
-                    "`{}` with samplers of type `{}`".format(
-                        type(domain).__name__, type(domain.sampler).__name__
-                    )
+                    "`{}` with samplers of type `{}`".format(type(domain).__name__, type(domain.sampler).__name__)
                 )
         elif isinstance(domain, sample.Integer):
             if isinstance(sampler, sample.LogUniform):
-                trial.suggest_int(
-                    key, domain.lower, domain.upper - int(bool(not quantize)), log=True
-                )
+                trial.suggest_int(key, domain.lower, domain.upper - int(bool(not quantize)), log=True)
             elif isinstance(sampler, sample.Uniform):
                 # Upper bound should be inclusive for quantization and
                 # exclusive otherwise
                 trial.suggest_int(
                     key,
                     domain.lower,
                     domain.upper - int(bool(not quantize)),
@@ -99,17 +95,15 @@
                 if isinstance(choice, dict):
                     key += f":{index}"
                     # the suffix needs to be removed from the final config
                     config.update(define_by_run_func(trial, choice, key))
         else:
             raise ValueError(
                 "Optuna search does not support parameters of type "
-                "`{}` with samplers of type `{}`".format(
-                    type(domain).__name__, type(domain.sampler).__name__
-                )
+                "`{}` with samplers of type `{}`".format(type(domain).__name__, type(domain.sampler).__name__)
             )
     # Return all constants in a dictionary.
     return config
 
 
 # def convert_key(
 #     conf: Dict, space: Dict, path: str = ""
@@ -144,17 +138,15 @@
     for key, value in config.items():
         if "/" in key:
             key = key[key.rfind("/") + 1 :]
         if ":" in key:
             pos = key.rfind(":")
             true_key = key[:pos]
             choice = int(key[pos + 1 :])
-            hier[true_key], subspace[true_key] = unflatten_hierarchical(
-                value, space[true_key][choice]
-            )
+            hier[true_key], subspace[true_key] = unflatten_hierarchical(value, space[true_key][choice])
         else:
             if key.endswith("_choice_"):
                 key = key[:-8]
             domain = space.get(key)
             if domain is not None:
                 if isinstance(domain, dict):
                     value, domain = unflatten_hierarchical(value, domain)
@@ -208,17 +200,15 @@
                         low_cost_dict = low_cost[i]
                     else:
                         low_cost_dict = {}
                     if choice_cost_list:
                         choice_cost_dict = choice_cost_list[i]
                     else:
                         choice_cost_dict = {}
-                    domain.const.append(
-                        add_cost_to_space(cat, low_cost_dict, choice_cost_dict)
-                    )
+                    domain.const.append(add_cost_to_space(cat, low_cost_dict, choice_cost_dict))
                 else:
                     domain.const.append(None)
             if choice_cost_list:
                 if len(choice_cost_list) == len(domain.categories):
                     domain.choice_cost = choice_cost_list
                 else:
                     domain.choice_cost = choice_cost_list[-1]
@@ -229,26 +219,22 @@
                 domain.choice_cost = cost[ind]
                 domain.const = [domain.const[i] for i in ind]
                 domain.ordered = True
             else:
                 ordered = getattr(domain, "ordered", None)
                 if ordered is None:
                     # automatically decide whether to order the choices based on the value type
-                    domain.ordered = ordered = all(
-                        isinstance(x, (int, float)) for x in domain.categories
-                    )
+                    domain.ordered = ordered = all(isinstance(x, (int, float)) for x in domain.categories)
                 if ordered:
                     # sort the choices by value
                     ind = np.argsort(domain.categories)
                     domain.categories = [domain.categories[i] for i in ind]
 
             if low_cost and low_cost not in domain.categories:
-                assert isinstance(
-                    low_cost, list
-                ), f"low cost {low_cost} not in domain {domain.categories}"
+                assert isinstance(low_cost, list), f"low cost {low_cost} not in domain {domain.categories}"
                 if domain.ordered:
                     sorted_points = [low_cost[i] for i in ind]
                     for i, point in enumerate(sorted_points):
                         low_cost[i] = point
                 if len(low_cost) > len(domain.categories):
                     if domain.ordered:
                         low_cost[-1] = int(np.where(ind == low_cost[-1])[0])
@@ -288,19 +274,15 @@
             # value is: a category, a nested dict, or a low_cost_point list
             if value not in domain.categories:
                 # nested
                 if isinstance(value, list):
                     # low_cost_point list
                     norm = []
                     for i, cat in enumerate(domain.categories):
-                        norm.append(
-                            normalize(value[i], cat, reference_config[key][i], {})
-                            if recursive
-                            else value[i]
-                        )
+                        norm.append(normalize(value[i], cat, reference_config[key][i], {}) if recursive else value[i])
                     if len(value) > len(domain.categories):
                         # the low cost index was appended to low_cost_point list
                         index = value[-1]
                         value = domain.categories[index]
                     elif not recursive:
                         # no low cost index. randomly pick one as init point
                         continue
@@ -331,24 +313,18 @@
         if isinstance(sampler, sample.Quantized):
             # sampler is sample.Quantized
             quantize = sampler.q
             sampler = sampler.get_sampler()
         else:
             quantize = None
         if str(sampler) == "LogUniform":
-            upper = domain.upper - (
-                isinstance(domain, sample.Integer) & (quantize is None)
-            )
-            config_norm[key] = np.log(value / domain.lower) / np.log(
-                upper / domain.lower
-            )
+            upper = domain.upper - (isinstance(domain, sample.Integer) & (quantize is None))
+            config_norm[key] = np.log(value / domain.lower) / np.log(upper / domain.lower)
         elif str(sampler) == "Uniform":
-            upper = domain.upper - (
-                isinstance(domain, sample.Integer) & (quantize is None)
-            )
+            upper = domain.upper - (isinstance(domain, sample.Integer) & (quantize is None))
             config_norm[key] = (value - domain.lower) / (upper - domain.lower)
         elif str(sampler) == "Normal":
             # N(mean, sd) -> N(0,1)
             config_norm[key] = (value - sampler.mean) / sampler.sd
         # else:
         #     config_norm[key] = value
     return config_norm
@@ -362,78 +338,62 @@
     random_state,
 ):
     config_denorm = {}
     for key, value in config.items():
         if key in space:
             # domain: sample.Categorical/Integer/Float/Function
             domain = space[key]
-            if isinstance(value, dict) or not callable(
-                getattr(domain, "get_sampler", None)
-            ):
+            if isinstance(value, dict) or not callable(getattr(domain, "get_sampler", None)):
                 config_denorm[key] = value
             else:
                 if isinstance(domain, sample.Categorical):
                     # denormalize categorical
                     n = len(domain.categories)
                     if isinstance(value, list):
                         # denormalize list
-                        choice = min(
-                            n - 1, int(np.floor(value[-1] * n))
-                        )  # max choice is n-1
+                        choice = min(n - 1, int(np.floor(value[-1] * n)))  # max choice is n-1
                         config_denorm[key] = point = value[choice]
                         point["_choice_"] = choice
                         continue
                     if domain.ordered:
-                        config_denorm[key] = domain.categories[
-                            min(n - 1, int(np.floor(value * n)))
-                        ]
+                        config_denorm[key] = domain.categories[min(n - 1, int(np.floor(value * n)))]
                     else:
                         assert key in normalized_reference_config
                         if min(n - 1, np.floor(value * n)) == min(
                             n - 1, np.floor(normalized_reference_config[key] * n)
                         ):
                             config_denorm[key] = reference_config[key]
                         else:  # ****random value each time!****
                             config_denorm[key] = random_state.choice(
-                                [
-                                    x
-                                    for x in domain.categories
-                                    if x != reference_config[key]
-                                ]
+                                [x for x in domain.categories if x != reference_config[key]]
                             )
                     continue
                 # Uniform/LogUniform/Normal/Base
                 sampler = domain.get_sampler()
                 if isinstance(sampler, sample.Quantized):
                     # sampler is sample.Quantized
                     quantize = sampler.q
                     sampler = sampler.get_sampler()
                 else:
                     quantize = None
                 # Handle Log/Uniform
                 if str(sampler) == "LogUniform":
-                    upper = domain.upper - (
-                        isinstance(domain, sample.Integer) & (quantize is None)
-                    )
+                    upper = domain.upper - (isinstance(domain, sample.Integer) & (quantize is None))
                     config_denorm[key] = (upper / domain.lower) ** value * domain.lower
                 elif str(sampler) == "Uniform":
-                    upper = domain.upper - (
-                        isinstance(domain, sample.Integer) & (quantize is None)
-                    )
+                    upper = domain.upper - (isinstance(domain, sample.Integer) & (quantize is None))
                     config_denorm[key] = value * (upper - domain.lower) + domain.lower
                 elif str(sampler) == "Normal":
                     # denormalization for 'Normal'
                     config_denorm[key] = value * sampler.sd + sampler.mean
                 # else:
                 #     config_denorm[key] = value
                 # Handle quantized
                 if quantize is not None:
-                    config_denorm[key] = (
-                        np.round(np.divide(config_denorm[key], quantize)) * quantize
-                    )
+                    config_denorm[key] = np.round(np.divide(config_denorm[key], quantize)) * quantize
                 # Handle int (4.6 -> 5)
                 if isinstance(domain, sample.Integer):
                     config_denorm[key] = int(round(config_denorm[key]))
         else:  # resource_attr
             config_denorm[key] = value
     return config_denorm
 
@@ -521,17 +481,15 @@
             else:
                 normalized[key] = max(low, min(up, value + delta))
     config = denormalize(normalized, space, config, normalized, flow2._random)
     # print("denormalized", config)
     for key, value in space.items():
         if key not in config:
             config[key] = value
-    for _, generated in generate_variants_compatible(
-        {"config": config}, random_state=flow2.rs_random
-    ):
+    for _, generated in generate_variants_compatible({"config": config}, random_state=flow2.rs_random):
         config = generated["config"]
         break
     subspace = {}
     for key, domain in space.items():
         value = config[key]
         if isinstance(value, dict):
             if isinstance(domain, sample.Categorical):
@@ -546,17 +504,15 @@
                     value,
                     domain.categories[index],
                     flow2,
                     disturb,
                     lower and lower.get(key) and lower[key][index],
                     upper and upper.get(key) and upper[key][index],
                 )
-                assert (
-                    "_choice_" not in subspace[key]
-                ), "_choice_ is a reserved key for hierarchical search space"
+                assert "_choice_" not in subspace[key], "_choice_ is a reserved key for hierarchical search space"
                 subspace[key]["_choice_"] = index
             else:
                 config[key], subspace[key] = complete_config(
                     value,
                     space[key],
                     flow2,
                     disturb,
```

### Comparing `FLAML-1.2.0/flaml/tune/spark/utils.py` & `FLAML-1.2.1/flaml/tune/spark/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,19 +65,15 @@
             Default is 'driver'.
 
     Returns:
         An int of the number of CPU cores.
     """
     assert node in ["driver", "executor"]
     try:
-        n_cpus = int(
-            SparkSession.builder.getOrCreate()
-            .sparkContext.getConf()
-            .get(f"spark.{node}.cores")
-        )
+        n_cpus = int(SparkSession.builder.getOrCreate().sparkContext.getConf().get(f"spark.{node}.cores"))
     except (TypeError, RuntimeError):
         n_cpus = os.cpu_count()
     return n_cpus
 
 
 def with_parameters(trainable, **kwargs):
     """Wrapper for trainables to pass arbitrary large data objects.
@@ -109,17 +105,15 @@
     with_parameters_train(config=1)
     train(config={"metric": "accuracy"})
     ```
     """
 
     if not callable(trainable):
         raise ValueError(
-            f"`with_parameters() only works with function trainables`. "
-            f"Got type: "
-            f"{type(trainable)}."
+            f"`with_parameters() only works with function trainables`. " f"Got type: " f"{type(trainable)}."
         )
 
     spark_available, spark_error_msg = check_spark()
     if not spark_available:
         raise spark_error_msg
     spark = SparkSession.builder.getOrCreate()
```

### Comparing `FLAML-1.2.0/flaml/tune/trial.py` & `FLAML-1.2.1/flaml/tune/trial.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,33 +112,27 @@
                     for n in self.n_steps:
                         key = "last-{:d}-avg".format(n)
                         self.metric_analysis[metric][key] = value
                         # Store n as string for correct restore.
                         self.metric_n_steps[metric][str(n)] = deque([value], maxlen=n)
                 else:
                     step = result["training_iteration"] or 1
-                    self.metric_analysis[metric]["max"] = max(
-                        value, self.metric_analysis[metric]["max"]
-                    )
-                    self.metric_analysis[metric]["min"] = min(
-                        value, self.metric_analysis[metric]["min"]
-                    )
+                    self.metric_analysis[metric]["max"] = max(value, self.metric_analysis[metric]["max"])
+                    self.metric_analysis[metric]["min"] = min(value, self.metric_analysis[metric]["min"])
                     self.metric_analysis[metric]["avg"] = (
-                        1
-                        / step
-                        * (value + (step - 1) * self.metric_analysis[metric]["avg"])
+                        1 / step * (value + (step - 1) * self.metric_analysis[metric]["avg"])
                     )
                     self.metric_analysis[metric]["last"] = value
 
                     for n in self.n_steps:
                         key = "last-{:d}-avg".format(n)
                         self.metric_n_steps[metric][str(n)].append(value)
-                        self.metric_analysis[metric][key] = sum(
+                        self.metric_analysis[metric][key] = sum(self.metric_n_steps[metric][str(n)]) / len(
                             self.metric_n_steps[metric][str(n)]
-                        ) / len(self.metric_n_steps[metric][str(n)])
+                        )
 
     def set_status(self, status):
         """Sets the status of the trial."""
         self.status = status
         if status == Trial.RUNNING:
             if self.start_time is None:
                 self.start_time = time.time()
```

### Comparing `FLAML-1.2.0/flaml/tune/trial_runner.py` & `FLAML-1.2.1/flaml/tune/trial_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,25 +92,21 @@
             elif decision == "PAUSE":
                 trial.set_status(Trial.PAUSED)
 
     def stop_trial(self, trial):
         """Stops trial."""
         if trial.status not in [Trial.ERROR, Trial.TERMINATED]:
             if self._scheduler_alg:
-                self._scheduler_alg.on_trial_complete(
-                    self, trial.trial_id, trial.last_result
-                )
+                self._scheduler_alg.on_trial_complete(self, trial.trial_id, trial.last_result)
             self._search_alg.on_trial_complete(trial.trial_id, trial.last_result)
             trial.set_status(Trial.TERMINATED)
         elif self._scheduler_alg:
             self._scheduler_alg.on_trial_remove(self, trial)
             if trial.status == Trial.ERROR:
-                self._search_alg.on_trial_complete(
-                    trial.trial_id, trial.last_result, error=True
-                )
+                self._search_alg.on_trial_complete(trial.trial_id, trial.last_result, error=True)
 
 
 class SequentialTrialRunner(BaseTrialRunner):
     """Implementation of the sequential trial runner."""
 
     def step(self) -> Trial:
         """Runs one step of the trial event loop.
```

### Comparing `FLAML-1.2.0/flaml/tune/tune.py` & `FLAML-1.2.1/flaml/tune/tune.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,63 +61,45 @@
     def best_config(self) -> Dict:
         if self.lexico_objectives is None:
             return super().best_config
         else:
             return self.get_best_config(self.default_metric, self.default_mode)
 
     def lexico_best(self, trials):
-        results = {
-            index: trial.last_result
-            for index, trial in enumerate(trials)
-            if trial.last_result
-        }
+        results = {index: trial.last_result for index, trial in enumerate(trials) if trial.last_result}
         metrics = self.lexico_objectives["metrics"]
         modes = self.lexico_objectives["modes"]
         f_best = {}
         keys = list(results.keys())
         length = len(keys)
         histories = defaultdict(list)
         for time_index in range(length):
             for objective, mode in zip(metrics, modes):
                 histories[objective].append(
-                    results[keys[time_index]][objective]
-                    if mode == "min"
-                    else -results[keys[time_index]][objective]
+                    results[keys[time_index]][objective] if mode == "min" else -results[keys[time_index]][objective]
                 )
         obj_initial = self.lexico_objectives["metrics"][0]
         feasible_index = np.array([*range(len(histories[obj_initial]))])
-        for k_metric, k_mode in zip(
-            self.lexico_objectives["metrics"], self.lexico_objectives["modes"]
-        ):
+        for k_metric, k_mode in zip(self.lexico_objectives["metrics"], self.lexico_objectives["modes"]):
             k_values = np.array(histories[k_metric])
             k_target = (
                 -self.lexico_objectives["targets"][k_metric]
                 if k_mode == "max"
                 else self.lexico_objectives["targets"][k_metric]
             )
             feasible_value = k_values.take(feasible_index)
             f_best[k_metric] = np.min(feasible_value)
 
             feasible_index_filter = np.where(
                 feasible_value
                 <= max(
                     f_best[k_metric] + self.lexico_objectives["tolerances"][k_metric]
-                    if not isinstance(
-                        self.lexico_objectives["tolerances"][k_metric], str
-                    )
+                    if not isinstance(self.lexico_objectives["tolerances"][k_metric], str)
                     else f_best[k_metric]
-                    * (
-                        1
-                        + 0.01
-                        * float(
-                            self.lexico_objectives["tolerances"][k_metric].replace(
-                                "%", ""
-                            )
-                        )
-                    ),
+                    * (1 + 0.01 * float(self.lexico_objectives["tolerances"][k_metric].replace("%", ""))),
                     k_target,
                 )
             )[0]
             feasible_index = feasible_index.take(feasible_index_filter)
         best_trial = trials[feasible_index[-1]]
         return best_trial
 
@@ -233,17 +215,15 @@
     reduction_factor: Optional[float] = None,
     scheduler=None,
     search_alg=None,
     verbose: Optional[int] = 2,
     local_dir: Optional[str] = None,
     num_samples: Optional[int] = 1,
     resources_per_trial: Optional[dict] = None,
-    config_constraints: Optional[
-        List[Tuple[Callable[[dict], float], str, float]]
-    ] = None,
+    config_constraints: Optional[List[Tuple[Callable[[dict], float], str, float]]] = None,
     metric_constraints: Optional[List[Tuple[str, str, float]]] = None,
     max_failure: Optional[int] = 100,
     use_ray: Optional[bool] = False,
     use_spark: Optional[bool] = False,
     use_incumbent_result_in_evaluation: Optional[bool] = None,
     log_file_name: Optional[str] = None,
     lexico_objectives: Optional[dict] = None,
@@ -459,17 +439,15 @@
     old_training_iteration = _training_iteration
     if log_file_name:
         dir_name = os.path.dirname(log_file_name)
         if dir_name:
             os.makedirs(dir_name, exist_ok=True)
     elif local_dir and verbose > 0:
         os.makedirs(local_dir, exist_ok=True)
-        log_file_name = os.path.join(
-            local_dir, "tune_" + str(datetime.datetime.now()).replace(":", "-") + ".log"
-        )
+        log_file_name = os.path.join(local_dir, "tune_" + str(datetime.datetime.now()).replace(":", "-") + ".log")
     if use_ray and use_spark:
         raise ValueError("use_ray and use_spark cannot be both True.")
     if not use_ray:
         _use_ray = False
         _verbose = verbose
         old_handlers = logger.handlers
         old_level = logger.getEffectiveLevel()
@@ -502,17 +480,15 @@
                 logger.setLevel(logging.DEBUG)
         else:
             logger.setLevel(logging.CRITICAL)
 
     from .searcher.blendsearch import BlendSearch, CFO
 
     if lexico_objectives is not None:
-        logger.warning(
-            "If lexico_objectives is not None, search_alg is forced to be CFO"
-        )
+        logger.warning("If lexico_objectives is not None, search_alg is forced to be CFO")
         search_alg = None
     if search_alg is None:
         flaml_scheduler_resource_attr = (
             flaml_scheduler_min_resource
         ) = flaml_scheduler_max_resource = flaml_scheduler_reduction_factor = None
         if scheduler in (None, "flaml"):
             # when scheduler is set 'flaml' or None, we will use a scheduler that is
@@ -525,22 +501,18 @@
             flaml_scheduler_reduction_factor = reduction_factor
             scheduler = None
         if lexico_objectives is None:
             try:
                 import optuna as _
 
                 SearchAlgorithm = BlendSearch
-                logger.info(
-                    "Using search algorithm {}.".format(SearchAlgorithm.__name__)
-                )
+                logger.info("Using search algorithm {}.".format(SearchAlgorithm.__name__))
             except ImportError:
                 SearchAlgorithm = CFO
-                logger.warning(
-                    "Using CFO for search. To use BlendSearch, run: pip install flaml[blendsearch]"
-                )
+                logger.warning("Using CFO for search. To use BlendSearch, run: pip install flaml[blendsearch]")
             metric = metric or DEFAULT_METRIC
         else:
             SearchAlgorithm = CFO
             logger.info("Using search algorithm {}.".format(SearchAlgorithm.__name__))
             metric = lexico_objectives["metrics"][0] or DEFAULT_METRIC
         search_alg = SearchAlgorithm(
             metric=metric,
@@ -577,22 +549,16 @@
             in [
                 "BlendSearch",
                 "CFO",
                 "CFOCat",
             ]
             and use_incumbent_result_in_evaluation is not None
         ):
-            search_alg.use_incumbent_result_in_evaluation = (
-                use_incumbent_result_in_evaluation
-            )
-        searcher = (
-            search_alg.searcher
-            if isinstance(search_alg, ConcurrencyLimiter)
-            else search_alg
-        )
+            search_alg.use_incumbent_result_in_evaluation = use_incumbent_result_in_evaluation
+        searcher = search_alg.searcher if isinstance(search_alg, ConcurrencyLimiter) else search_alg
         if isinstance(searcher, BlendSearch):
             setting = {}
             if time_budget_s:
                 setting["time_budget_s"] = time_budget_s
             if num_samples > 0:
                 setting["num_samples"] = num_samples
             searcher.set_search_properties(metric, mode, config, **setting)
@@ -613,18 +579,15 @@
             from ray.tune.schedulers import ASHAScheduler
 
             scheduler = ASHAScheduler(**params)
     if use_ray:
         try:
             from ray import tune
         except ImportError:
-            raise ImportError(
-                "Failed to import ray tune. "
-                "Please install ray[tune] or set use_ray=False"
-            )
+            raise ImportError("Failed to import ray tune. " "Please install ray[tune] or set use_ray=False")
         _use_ray = True
         try:
             analysis = tune.run(
                 evaluation_function,
                 metric=metric,
                 mode=mode,
                 search_alg=search_alg,
@@ -655,27 +618,22 @@
         if not spark_available:
             raise spark_error_msg
         try:
             from pyspark.sql import SparkSession
             from joblib import Parallel, delayed, parallel_backend
             from joblibspark import register_spark
         except ImportError as e:
-            raise ImportError(
-                f"{e}. Try pip install flaml[spark] or set use_spark=False."
-            )
+            raise ImportError(f"{e}. Try pip install flaml[spark] or set use_spark=False.")
         from flaml.tune.searcher.suggestion import ConcurrencyLimiter
         from .trial_runner import SparkTrialRunner
 
         register_spark()
         spark = SparkSession.builder.getOrCreate()
         sc = spark._jsc.sc()
-        num_executors = (
-            len([executor.host() for executor in sc.statusTracker().getExecutorInfos()])
-            - 1
-        )
+        num_executors = len([executor.host() for executor in sc.statusTracker().getExecutorInfos()]) - 1
         """
         By default, the number of executors is the number of VMs in the cluster. And we can
         launch one trial per executor. However, sometimes we can launch more trials than
         the number of executors (e.g., local mode). In this case, we can set the environment
         variable `FLAML_MAX_CONCURRENT` to override the detected `num_executors`.
 
         `max_concurrent` is the maximum number of concurrent trials defined by `search_alg`,
@@ -704,31 +662,27 @@
         else:
             max_concurrent = max(1, max_spark_parallelism)
         n_concurrent_trials = min(
             n_concurrent_trials if n_concurrent_trials > 0 else num_executors,
             max_concurrent,
         )
         with parallel_backend("spark"):
-            with Parallel(
-                n_jobs=n_concurrent_trials, verbose=max(0, (verbose - 1) * 50)
-            ) as parallel:
+            with Parallel(n_jobs=n_concurrent_trials, verbose=max(0, (verbose - 1) * 50)) as parallel:
                 try:
                     _runner = SparkTrialRunner(
                         search_alg=search_alg,
                         scheduler=scheduler,
                         metric=metric,
                         mode=mode,
                     )
                     num_trials = 0
                     if time_budget_s is None:
                         time_budget_s = np.inf
                     num_failures = 0
-                    upperbound_num_failures = (
-                        len(evaluated_rewards) if evaluated_rewards else 0
-                    ) + max_failure
+                    upperbound_num_failures = (len(evaluated_rewards) if evaluated_rewards else 0) + max_failure
                     while (
                         time.time() - time_start < time_budget_s
                         and (num_samples < 0 or num_trials < num_samples)
                         and num_failures < upperbound_num_failures
                     ):
                         while len(_runner.running_trials) < n_concurrent_trials:
                             # suggest trials for spark
@@ -738,32 +692,27 @@
                             else:
                                 num_failures += 1  # break with upperbound_num_failures consecutive failures
                                 logger.debug(f"consecutive failures is {num_failures}")
                                 if num_failures >= upperbound_num_failures:
                                     break
                         trials_to_run = _runner.running_trials
                         if not trials_to_run:
-                            logger.warning(
-                                f"fail to sample a trial for {max_failure} times in a row, stopping."
-                            )
+                            logger.warning(f"fail to sample a trial for {max_failure} times in a row, stopping.")
                             break
                         logger.info(
                             f"Number of trials: {num_trials}/{num_samples}, {len(_runner.running_trials)} RUNNING,"
                             f" {len(_runner._trials) - len(_runner.running_trials)} TERMINATED"
                         )
                         logger.debug(
                             f"Configs of Trials to run: {[trial_to_run.config for trial_to_run in trials_to_run]}"
                         )
                         results = None
-                        with PySparkOvertimeMonitor(
-                            time_start, time_budget_s, force_cancel, parallel=parallel
-                        ):
+                        with PySparkOvertimeMonitor(time_start, time_budget_s, force_cancel, parallel=parallel):
                             results = parallel(
-                                delayed(evaluation_function)(trial_to_run.config)
-                                for trial_to_run in trials_to_run
+                                delayed(evaluation_function)(trial_to_run.config) for trial_to_run in trials_to_run
                             )
                         # results = [evaluation_function(trial_to_run.config) for trial_to_run in trials_to_run]
                         while results:
                             result = results.pop(0)
                             trial_to_run = trials_to_run[0]
                             _runner.running_trial = trial_to_run
                             if result is not None:
@@ -771,17 +720,15 @@
                                     if result:
                                         logger.info(f"Brief result: {result}")
                                         report(**result)
                                     else:
                                         # When the result returned is an empty dict, set the trial status to error
                                         trial_to_run.set_status(Trial.ERROR)
                                 else:
-                                    logger.info(
-                                        "Brief result: {}".format({metric: result})
-                                    )
+                                    logger.info("Brief result: {}".format({metric: result}))
                                     report(_metric=result)
                             _runner.stop_trial(trial_to_run)
                         num_failures = 0
                     analysis = ExperimentAnalysis(
                         _runner.get_trials(),
                         metric=metric,
                         mode=mode,
@@ -813,17 +760,15 @@
             metric=metric,
             mode=mode,
         )
         num_trials = 0
         if time_budget_s is None:
             time_budget_s = np.inf
         num_failures = 0
-        upperbound_num_failures = (
-            len(evaluated_rewards) if evaluated_rewards else 0
-        ) + max_failure
+        upperbound_num_failures = (len(evaluated_rewards) if evaluated_rewards else 0) + max_failure
         while (
             time.time() - time_start < time_budget_s
             and (num_samples < 0 or num_trials < num_samples)
             and num_failures < upperbound_num_failures
         ):
             trial_to_run = _runner.step()
             if trial_to_run:
@@ -848,17 +793,15 @@
                     # application stops tuning by returning None
                     # TODO document this feature when it is finalized
                     break
             else:
                 # break with upperbound_num_failures consecutive failures
                 num_failures += 1
         if num_failures == upperbound_num_failures:
-            logger.warning(
-                f"fail to sample a trial for {max_failure} times in a row, stopping."
-            )
+            logger.warning(f"fail to sample a trial for {max_failure} times in a row, stopping.")
         analysis = ExperimentAnalysis(
             _runner.get_trials(),
             metric=metric,
             mode=mode,
             lexico_objectives=lexico_objectives,
         )
         return analysis
```

### Comparing `FLAML-1.2.0/flaml/tune/utils.py` & `FLAML-1.2.1/flaml/tune/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,13 +19,9 @@
 
     Args:
         categories (Sequence): Sequence of categories to sample from.
         order (bool): Whether the categories have an order. If None, will be decided autoamtically:
             Numerical categories have an order, while string categories do not.
     """
     domain = sample.Categorical(categories).uniform()
-    domain.ordered = (
-        order
-        if order is not None
-        else all(isinstance(x, (int, float)) for x in categories)
-    )
+    domain.ordered = order if order is not None else all(isinstance(x, (int, float)) for x in categories)
     return domain
```

### Comparing `FLAML-1.2.0/setup.py` & `FLAML-1.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             "catboost>=0.26",
             "rgf-python",
             "optuna==2.8.0",
             "openml==0.10.2",
             "statsmodels>=0.12.2",
             "psutil==5.8.0",
             "dataclasses",
-            "transformers[torch]",
+            "transformers[torch]==4.26",
             "datasets",
             "nltk",
             "rouge_score",
             "hcrystalball==0.1.10",
             "seqeval",
             "pytorch-forecasting>=0.9.0,<=0.10.1",
             "mlflow",
```

### Comparing `FLAML-1.2.0/test/test_autovw.py` & `FLAML-1.2.1/test/test_autovw.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 import pytest
 
 VW_DS_DIR = "test/data/"
 NS_LIST = list(string.ascii_lowercase) + list(string.ascii_uppercase)
 logger = logging.getLogger(__name__)
 
 
-def oml_to_vw_w_grouping(
-    X, y, ds_dir, fname, orginal_dim, group_num, grouping_method="sequential"
-):
+def oml_to_vw_w_grouping(X, y, ds_dir, fname, orginal_dim, group_num, grouping_method="sequential"):
     # split all_indexes into # group_num of groups
     max_size_per_group = int(np.ceil(orginal_dim / float(group_num)))
     # sequential grouping
     if grouping_method == "sequential":
         group_indexes = []  # lists of lists
         for i in range(group_num):
             indexes = [
@@ -45,25 +43,19 @@
         with open(os.path.join(ds_dir, fname), "w") as f:
             if isinstance(X, pd.DataFrame):
                 raise NotImplementedError
             elif isinstance(X, np.ndarray):
                 for i in range(len(X)):
                     NS_content = []
                     for zz in range(len(group_indexes)):
-                        ns_features = " ".join(
-                            "{}:{:.6f}".format(ind, X[i][ind])
-                            for ind in group_indexes[zz]
-                        )
+                        ns_features = " ".join("{}:{:.6f}".format(ind, X[i][ind]) for ind in group_indexes[zz])
                         NS_content.append(ns_features)
                     ns_line = "{} |{}".format(
                         str(y[i]),
-                        "|".join(
-                            "{} {}".format(NS_LIST[j], NS_content[j])
-                            for j in range(len(group_indexes))
-                        ),
+                        "|".join("{} {}".format(NS_LIST[j], NS_content[j]) for j in range(len(group_indexes))),
                     )
                     f.write(ns_line)
                     f.write("\n")
             elif isinstance(X, scipy.sparse.csr_matrix):
                 print("NotImplementedError for sparse data")
                 NotImplementedError
 
@@ -136,18 +128,15 @@
     import os
 
     if is_regression:
         # the second field specifies the largest number of namespaces using.
         fname = "ds_{}_{}_{}.vw".format(did, max_ns_num, 0)
         vw_dataset_file = os.path.join(ds_dir, fname)
         # if file does not exist, generate and save the datasets
-        if (
-            not os.path.exists(vw_dataset_file)
-            or os.stat(vw_dataset_file).st_size < 1000
-        ):
+        if not os.path.exists(vw_dataset_file) or os.stat(vw_dataset_file).st_size < 1000:
             get_oml_to_vw(did, max_ns_num)
         print(ds_dir, vw_dataset_file)
         if not os.path.exists(ds_dir):
             os.makedirs(ds_dir)
         with open(os.path.join(ds_dir, fname), "r") as f:
             vw_content = f.read().splitlines()
             print(type(vw_content), len(vw_content))
@@ -171,17 +160,15 @@
     vw_examples = None
     data_id = int(dataset_id)
     # loading oml dataset
     # data = OpenML2VWData(data_id, max_ns_num, dataset_type)
     # Y = data.Y
     if vw_format:
         # vw_examples = data.vw_examples
-        vw_examples = load_vw_dataset(
-            did=data_id, ds_dir=VW_DS_DIR, is_regression=True, max_ns_num=max_ns_num
-        )
+        vw_examples = load_vw_dataset(did=data_id, ds_dir=VW_DS_DIR, is_regression=True, max_ns_num=max_ns_num)
         Y = []
         for i, e in enumerate(vw_examples):
             Y.append(float(e.split("|")[0]))
     logger.debug("first data %s", vw_examples[0])
     # do data shuffling or log transformation for oml data when needed
     if shuffle:
         random.seed(54321)
@@ -226,17 +213,15 @@
         self._problem_info = {
             "max_iter_num": self.max_iter_num,
             "dataset_id": dataset_id,
             "ns_num": ns_num,
         }
         self._problem_info.update(kwargs)
         self._fixed_hp_config = kwargs.get("fixed_hp_config", {})
-        self.namespace_feature_dim = AutoVW.get_ns_feature_dim_from_vw_example(
-            self.vw_examples[0]
-        )
+        self.namespace_feature_dim = AutoVW.get_ns_feature_dim_from_vw_example(self.vw_examples[0])
         self._raw_namespaces = list(self.namespace_feature_dim.keys())
         self._setup_search()
 
     def _setup_search(self):
         self._search_space = self._fixed_hp_config.copy()
         self._init_config = self._fixed_hp_config.copy()
         search_space = {
@@ -351,21 +336,17 @@
     vw_oml_problem_args = {
         "max_iter_num": online_vw_exp_setting["max_iter_num"],
         "dataset_id": "42183",
         "ns_num": online_vw_exp_setting["ns_num"],
         "fixed_hp_config": online_vw_exp_setting["fixed_hp_config"],
     }
     if tuning_hp == "NamesapceInteraction":
-        vw_online_aml_problem = VowpalWabbitNamesspaceTuningProblem(
-            **vw_oml_problem_args
-        )
+        vw_online_aml_problem = VowpalWabbitNamesspaceTuningProblem(**vw_oml_problem_args)
     elif tuning_hp == "NamesapceInteraction+LearningRate":
-        vw_online_aml_problem = VowpalWabbitNamesspaceLRTuningProblem(
-            **vw_oml_problem_args
-        )
+        vw_online_aml_problem = VowpalWabbitNamesspaceLRTuningProblem(**vw_oml_problem_args)
     else:
         NotImplementedError
 
     return vw_oml_problem_args, vw_online_aml_problem
 
 
 @pytest.mark.skipif(
@@ -378,21 +359,17 @@
 
         vw_oml_problem_args, vw_online_aml_problem = get_vw_tuning_problem()
         vanilla_vw = pyvw.vw(**vw_oml_problem_args["fixed_hp_config"])
         cumulative_loss_list = online_learning_loop(
             vw_online_aml_problem.max_iter_num,
             vw_online_aml_problem.vw_examples,
             vanilla_vw,
-            loss_func=vw_oml_problem_args["fixed_hp_config"].get(
-                "loss_function", "squared"
-            ),
-        )
-        print(
-            "final average loss:", sum(cumulative_loss_list) / len(cumulative_loss_list)
+            loss_func=vw_oml_problem_args["fixed_hp_config"].get("loss_function", "squared"),
         )
+        print("final average loss:", sum(cumulative_loss_list) / len(cumulative_loss_list))
 
     def test_supervised_vw_tune_namespace(self):
         # basic experiment setting
         vw_oml_problem_args, vw_online_aml_problem = get_vw_tuning_problem()
         autovw = AutoVW(
             max_live_model_num=5,
             search_space=vw_online_aml_problem.search_space,
@@ -401,21 +378,17 @@
             random_seed=2345,
         )
 
         cumulative_loss_list = online_learning_loop(
             vw_online_aml_problem.max_iter_num,
             vw_online_aml_problem.vw_examples,
             autovw,
-            loss_func=vw_oml_problem_args["fixed_hp_config"].get(
-                "loss_function", "squared"
-            ),
-        )
-        print(
-            "final average loss:", sum(cumulative_loss_list) / len(cumulative_loss_list)
+            loss_func=vw_oml_problem_args["fixed_hp_config"].get("loss_function", "squared"),
         )
+        print("final average loss:", sum(cumulative_loss_list) / len(cumulative_loss_list))
 
     def test_supervised_vw_tune_namespace_learningrate(self):
         # basic experiment setting
         vw_oml_problem_args, vw_online_aml_problem = get_vw_tuning_problem(
             tuning_hp="NamesapceInteraction+LearningRate"
         )
         autovw = AutoVW(
@@ -426,21 +399,17 @@
             random_seed=2345,
         )
 
         cumulative_loss_list = online_learning_loop(
             vw_online_aml_problem.max_iter_num,
             vw_online_aml_problem.vw_examples,
             autovw,
-            loss_func=vw_oml_problem_args["fixed_hp_config"].get(
-                "loss_function", "squared"
-            ),
-        )
-        print(
-            "final average loss:", sum(cumulative_loss_list) / len(cumulative_loss_list)
+            loss_func=vw_oml_problem_args["fixed_hp_config"].get("loss_function", "squared"),
         )
+        print("final average loss:", sum(cumulative_loss_list) / len(cumulative_loss_list))
 
     def test_bandit_vw_tune_namespace(self):
         pass
 
     def test_bandit_vw_tune_namespace_learningrate(self):
         pass
```

### Comparing `FLAML-1.2.0/test/test_conda_distribution.py` & `FLAML-1.2.1/test/test_conda_distribution.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.0/test/test_gpu.py` & `FLAML-1.2.1/test/test_gpu.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,17 +19,15 @@
             X_train,
             y_train,
             estimator_list=["xgb_limitdepth", "xgboost"],
             time_budget=5,
             gpu_per_trial=1,
         )
 
-        train, label = make_moons(
-            n_samples=300000, shuffle=True, noise=0.3, random_state=None
-        )
+        train, label = make_moons(n_samples=300000, shuffle=True, noise=0.3, random_state=None)
         automl = AutoML()
         automl.fit(
             train,
             label,
             estimator_list=["xgb_limitdepth", "xgboost"],
             time_budget=5,
             gpu_per_trial=1,
@@ -85,26 +83,18 @@
         "transformer": {
             "model_path": "facebook/muppet-roberta-base",
             "output_dir": "test/data/output/",
             "fp16": True,
         }
     }
 
-    automl.fit(
-        X_train=X_train, y_train=y_train, X_val=X_val, y_val=y_val, **automl_settings
-    )
+    automl.fit(X_train=X_train, y_train=y_train, X_val=X_val, y_val=y_val, **automl_settings)
 
     automl = AutoML()
-    automl.retrain_from_log(
-        X_train=X_train,
-        y_train=y_train,
-        train_full=True,
-        record_id=0,
-        **automl_settings
-    )
+    automl.retrain_from_log(X_train=X_train, y_train=y_train, train_full=True, record_id=0, **automl_settings)
     with open("automl.pkl", "wb") as f:
         pickle.dump(automl, f, pickle.HIGHEST_PROTOCOL)
     with open("automl.pkl", "rb") as f:
         automl = pickle.load(f)
     shutil.rmtree("test/data/output/")
     automl.predict(X_test)
     automl.predict(["test test", "test test"])
```

### Comparing `FLAML-1.2.0/test/test_model.py` & `FLAML-1.2.1/test/test_model.py`

 * *Files identical despite different names*

