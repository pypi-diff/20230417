# Comparing `tmp/ml-starter-0.0.17.tar.gz` & `tmp/ml-starter-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.17.tar", last modified: Fri Apr 14 01:50:32 2023, max compression
+gzip compressed data, was "ml-starter-0.0.18.tar", last modified: Mon Apr 17 03:08:11 2023, max compression
```

## Comparing `ml-starter-0.0.17.tar` & `ml-starter-0.0.18.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.267999 ml-starter-0.0.17/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 01:50:19.000000 ml-starter-0.0.17/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-14 01:50:32.267999 ml-starter-0.0.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-14 01:50:19.000000 ml-starter-0.0.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.219998 ml-starter-0.0.17/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/__version__.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.219998 ml-starter-0.0.17/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    21504 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.223998 ml-starter-0.0.17/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.227998 ml-starter-0.0.17/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.227998 ml-starter-0.0.17/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.231998 ml-starter-0.0.17/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.231998 ml-starter-0.0.17/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.235998 ml-starter-0.0.17/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/scripts/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/scripts/mp_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.235998 ml-starter-0.0.17/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17564 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.243998 ml-starter-0.0.17/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.247999 ml-starter-0.0.17/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.247999 ml-starter-0.0.17/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.247999 ml-starter-0.0.17/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.247999 ml-starter-0.0.17/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.251999 ml-starter-0.0.17/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19149 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/ddp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.255998 ml-starter-0.0.17/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.263999 ml-starter-0.0.17/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.267999 ml-starter-0.0.17/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.267999 ml-starter-0.0.17/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-14 01:50:32.000000 ml-starter-0.0.17/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-14 01:50:32.000000 ml-starter-0.0.17/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 01:50:32.000000 ml-starter-0.0.17/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 01:50:32.000000 ml-starter-0.0.17/ml_starter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 01:50:32.000000 ml-starter-0.0.17/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-14 01:50:32.000000 ml-starter-0.0.17/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-14 01:50:19.000000 ml-starter-0.0.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 01:50:19.000000 ml-starter-0.0.17/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 01:50:19.000000 ml-starter-0.0.17/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 01:50:32.271999 ml-starter-0.0.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 01:50:19.000000 ml-starter-0.0.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.731754 ml-starter-0.0.18/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-17 03:07:54.000000 ml-starter-0.0.18/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-17 03:08:11.731754 ml-starter-0.0.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-17 03:07:54.000000 ml-starter-0.0.18/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.715754 ml-starter-0.0.18/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/__version__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.715754 ml-starter-0.0.18/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21504 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.719754 ml-starter-0.0.18/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.719754 ml-starter-0.0.18/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.719754 ml-starter-0.0.18/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.719754 ml-starter-0.0.18/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.719754 ml-starter-0.0.18/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.723754 ml-starter-0.0.18/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/scripts/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/scripts/mp_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.723754 ml-starter-0.0.18/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17564 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.723754 ml-starter-0.0.18/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.723754 ml-starter-0.0.18/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.723754 ml-starter-0.0.18/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.723754 ml-starter-0.0.18/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.723754 ml-starter-0.0.18/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.727754 ml-starter-0.0.18/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19149 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/trainers/ddp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.727754 ml-starter-0.0.18/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/trainers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.727754 ml-starter-0.0.18/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.731754 ml-starter-0.0.18/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-04-17 03:07:54.000000 ml-starter-0.0.18/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:08:11.731754 ml-starter-0.0.18/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-17 03:08:11.000000 ml-starter-0.0.18/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-17 03:08:11.000000 ml-starter-0.0.18/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 03:08:11.000000 ml-starter-0.0.18/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-17 03:08:11.000000 ml-starter-0.0.18/ml_starter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-17 03:08:11.000000 ml-starter-0.0.18/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-17 03:08:11.000000 ml-starter-0.0.18/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-17 03:07:54.000000 ml-starter-0.0.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-17 03:07:54.000000 ml-starter-0.0.18/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-17 03:07:54.000000 ml-starter-0.0.18/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-17 03:08:11.731754 ml-starter-0.0.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-17 03:07:54.000000 ml-starter-0.0.18/setup.py
```

### Comparing `ml-starter-0.0.17/PKG-INFO` & `ml-starter-0.0.18/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.17
+Version: 0.0.18
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.17/README.md` & `ml-starter-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/api.py` & `ml-starter-0.0.18/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/core/config.py` & `ml-starter-0.0.18/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/core/env.py` & `ml-starter-0.0.18/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/core/registry.py` & `ml-starter-0.0.18/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/core/state.py` & `ml-starter-0.0.18/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/loggers/base.py` & `ml-starter-0.0.18/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/loggers/meter.py` & `ml-starter-0.0.18/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/loggers/multi.py` & `ml-starter-0.0.18/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/loggers/stdout.py` & `ml-starter-0.0.18/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/loggers/tensorboard.py` & `ml-starter-0.0.18/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/lr_schedulers/base.py` & `ml-starter-0.0.18/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.18/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.18/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/lr_schedulers/linear.py` & `ml-starter-0.0.18/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.18/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.18/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/models/activations.py` & `ml-starter-0.0.18/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/models/base.py` & `ml-starter-0.0.18/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/models/embeddings.py` & `ml-starter-0.0.18/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/models/init.py` & `ml-starter-0.0.18/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/models/norms.py` & `ml-starter-0.0.18/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/optimizers/adam.py` & `ml-starter-0.0.18/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/optimizers/adamw.py` & `ml-starter-0.0.18/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/optimizers/adan.py` & `ml-starter-0.0.18/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/optimizers/base.py` & `ml-starter-0.0.18/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/optimizers/sgd.py` & `ml-starter-0.0.18/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/optimizers/shampoo.py` & `ml-starter-0.0.18/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/scripts/cli.py` & `ml-starter-0.0.18/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/scripts/compiler.py` & `ml-starter-0.0.18/ml/scripts/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/scripts/stage.py` & `ml-starter-0.0.18/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/scripts/train.py` & `ml-starter-0.0.18/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/base.py` & `ml-starter-0.0.18/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.18/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.18/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/datasets/collate.py` & `ml-starter-0.0.18/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.18/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.18/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.18/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.18/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.18/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/datasets/utils.py` & `ml-starter-0.0.18/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.18/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/environments/base.py` & `ml-starter-0.0.18/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/environments/utils.py` & `ml-starter-0.0.18/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/environments/worker.py` & `ml-starter-0.0.18/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/losses/reduce.py` & `ml-starter-0.0.18/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/rl/base.py` & `ml-starter-0.0.18/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/rl/replay.py` & `ml-starter-0.0.18/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/tasks/sl/base.py` & `ml-starter-0.0.18/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/trainers/base.py` & `ml-starter-0.0.18/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/trainers/ddp.py` & `ml-starter-0.0.18/ml/trainers/ddp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.18/ml/trainers/mixins/cpu_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
             ),
         )
         self._cpu_stats: CPUStatsInfo | None = None
 
         self._proc = mp.Process(
             target=worker,
             args=(ping_interval, self._cpu_stats_smem, self._event, os.getpid()),
-            daemon=True,
+            daemon=False,
         )
         self._proc.start()
         atexit.register(self.stop)
 
     def get_if_set(self) -> CPUStatsInfo | None:
         if self._event.is_set():
             self._event.clear()
```

### Comparing `ml-starter-0.0.17/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.18/ml/trainers/mixins/gpu_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             for i in range(num_gpus)
         ]
         self._gpu_stats: dict[int, GPUStatsInfo] = {}
 
         self._proc = mp.Process(
             target=worker,
             args=(ping_interval, self._smems, self._main_event, self._events),
-            daemon=True,
+            daemon=False,
         )
         self._proc.start()
         atexit.register(self.stop)
 
     def get_if_set(self) -> dict[int, GPUStatsInfo]:
         gpu_stats: dict[int, GPUStatsInfo] = {}
         if self._main_event.is_set():
```

### Comparing `ml-starter-0.0.17/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.18/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.18/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.18/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.18/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.18/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/trainers/rl.py` & `ml-starter-0.0.18/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/trainers/sl.py` & `ml-starter-0.0.18/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/trainers/slurm.py` & `ml-starter-0.0.18/ml/trainers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/trainers/vanilla.py` & `ml-starter-0.0.18/ml/trainers/vanilla.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 )
 from ml.trainers.mixins.mixed_precision import (
     MixedPrecisionTrainerConfig,
     MixedPrecisionTrainerMixin,
 )
 from ml.trainers.mixins.profiler import ProfilerTrainerConfig, ProfilerTrainerMixin
 from ml.utils.device.base import Prefetcher
-from ml.utils.distributed import is_master
 from ml.utils.timer import Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class TrainingFinishedException(Exception):
     pass
@@ -223,28 +222,27 @@
         self.save_checkpoint(state, task, model, optim, lr_scheduler)
         self.remove_lock_file("running", missing_ok=True)
 
     def set_signal_handler(self, handler: Callable[[int, FrameType | None], None]) -> None:
         pass
 
     def _init_environment(self) -> None:
-        if is_master():
-            self.add_lock_file("running", exists_ok=True)
-
         # Sets up environment.
         if self.config.deterministic:
             torch.use_deterministic_algorithms(True)
         if self.config.use_tf32 and torch.cuda.is_available():
             torch.backends.cuda.matmul.allow_tf32 = True
 
         # Saves the config at the start of training.
         with Timer("saving config"):
             self.save_config()
             self.log_run_config()
 
+        self.add_lock_file("running", exists_ok=True)
+
         # Enables anomaly detection.
         if self.config.detect_anomaly:
             torch.autograd.set_detect_anomaly(True, check_nan=self.config.detect_anomaly_check_nan)
 
     def _compile_model(self, model: ModelT) -> ModelT:
         if self.config.torch_compile.enabled:
             backend: str | Callable = self.config.torch_compile.backend
```

### Comparing `ml-starter-0.0.17/ml/utils/argparse.py` & `ml-starter-0.0.18/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/atomic.py` & `ml-starter-0.0.18/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/augmentation.py` & `ml-starter-0.0.18/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/caching.py` & `ml-starter-0.0.18/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/call_train.py` & `ml-starter-0.0.18/ml/utils/call_train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/cli.py` & `ml-starter-0.0.18/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/colors.py` & `ml-starter-0.0.18/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/compiler.py` & `ml-starter-0.0.18/ml/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/data.py` & `ml-starter-0.0.18/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/datetime.py` & `ml-starter-0.0.18/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/device/auto.py` & `ml-starter-0.0.18/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/device/base.py` & `ml-starter-0.0.18/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/device/cpu.py` & `ml-starter-0.0.18/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/device/gpu.py` & `ml-starter-0.0.18/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/device/metal.py` & `ml-starter-0.0.18/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/distributed.py` & `ml-starter-0.0.18/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/io.py` & `ml-starter-0.0.18/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/large_models.py` & `ml-starter-0.0.18/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/logging.py` & `ml-starter-0.0.18/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/meter.py` & `ml-starter-0.0.18/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/staging.py` & `ml-starter-0.0.18/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/timer.py` & `ml-starter-0.0.18/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml/utils/video.py` & `ml-starter-0.0.18/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.18/ml_starter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.17
+Version: 0.0.18
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.17/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.18/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/pyproject.toml` & `ml-starter-0.0.18/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.17/setup.py` & `ml-starter-0.0.18/setup.py`

 * *Files identical despite different names*

