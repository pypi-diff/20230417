# Comparing `tmp/returnn-1.20230417.170727.tar.gz` & `tmp/returnn-1.20230417.173710.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230417.170727.tar", last modified: Mon Apr 17 15:28:43 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230417.173710.tar", last modified: Mon Apr 17 15:54:43 2023, max compression
```

## Comparing `returnn-1.20230417.170727.tar` & `returnn-1.20230417.173710.tar`

### file list

```diff
@@ -1,423 +1,423 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 15:28:15.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-17 15:28:19.000000 returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/extern/graph_editor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97348 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   155421 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tensor/tensor_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   151440 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28259 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    69697 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20104 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   588393 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   292981 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40895 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144922 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   187471 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:28:43.000000 returnn-1.20230417.170727/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-17 15:28:13.000000 returnn-1.20230417.170727/tools/tf_inspect_summary_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 15:54:24.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-17 15:54:26.000000 returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/extern/graph_editor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32926 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97348 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155421 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tensor/tensor_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151440 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69697 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20104 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   588416 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   292981 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41966 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144922 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187471 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:43.000000 returnn-1.20230417.173710/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-17 15:54:23.000000 returnn-1.20230417.173710/tools/tf_inspect_summary_log.py
```

### Comparing `returnn-1.20230417.170727/.gitignore` & `returnn-1.20230417.173710/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/.gitmodules` & `returnn-1.20230417.173710/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/CHANGELOG.md` & `returnn-1.20230417.173710/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/CODEOWNERS` & `returnn-1.20230417.173710/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/CONTRIBUTING.md` & `returnn-1.20230417.173710/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/LICENSE` & `returnn-1.20230417.173710/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/MANIFEST.in` & `returnn-1.20230417.173710/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/PKG-INFO` & `returnn-1.20230417.173710/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230417.170727
+Version: 1.20230417.173710
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230417.170727/README.rst` & `returnn-1.20230417.173710/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/__init__.py` & `returnn-1.20230417.173710/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/12AX.cluster_map` & `returnn-1.20230417.173710/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-fwd.config` & `returnn-1.20230417.173710/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-horovod-mpi.py` & `returnn-1.20230417.173710/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230417.173710/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-hyper-param-tuning.config` & `returnn-1.20230417.173710/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-iter-dataset.py` & `returnn-1.20230417.173710/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-list-devices.py` & `returnn-1.20230417.173710/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-lua-torch-layer.config` & `returnn-1.20230417.173710/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230417.173710/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-returnn-as-framework.py` & `returnn-1.20230417.173710/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-rf.config` & `returnn-1.20230417.173710/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-rhn-enwik8.config` & `returnn-1.20230417.173710/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-sprint-interface.py` & `returnn-1.20230417.173710/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-att-copy.config` & `returnn-1.20230417.173710/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-attention.config` & `returnn-1.20230417.173710/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230417.173710/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230417.173710/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-enc-dec.config` & `returnn-1.20230417.173710/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230417.173710/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230417.173710/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230417.173710/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230417.173710/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230417.173710/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230417.173710/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230417.173710/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230417.173710/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230417.173710/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230417.173710/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-rec-self-att.config` & `returnn-1.20230417.173710/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230417.173710/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230417.173710/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230417.173710/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-torch.config` & `returnn-1.20230417.173710/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230417.173710/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/demo.sh` & `returnn-1.20230417.173710/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230417.173710/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230417.173710/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230417.173710/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/IAM/README.txt` & `returnn-1.20230417.173710/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/IAM/config_demo` & `returnn-1.20230417.173710/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230417.173710/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/IAM/config_real` & `returnn-1.20230417.173710/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230417.173710/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/IAM/decode.py` & `returnn-1.20230417.173710/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230417.173710/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230417.173710/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230417.173710/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230417.173710/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230417.173710/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230417.173710/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230417.173710/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230417.173710/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230417.173710/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230417.173710/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/__init__.py` & `returnn-1.20230417.173710/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/__main__.py` & `returnn-1.20230417.173710/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/__old_mod_loader__.py` & `returnn-1.20230417.173710/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/__setup__.py` & `returnn-1.20230417.173710/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/config.py` & `returnn-1.20230417.173710/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/audio.py` & `returnn-1.20230417.173710/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/basic.py` & `returnn-1.20230417.173710/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/bundle_file.py` & `returnn-1.20230417.173710/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/cached.py` & `returnn-1.20230417.173710/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/cached2.py` & `returnn-1.20230417.173710/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/generating.py` & `returnn-1.20230417.173710/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/hdf.py` & `returnn-1.20230417.173710/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/lm.py` & `returnn-1.20230417.173710/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/map.py` & `returnn-1.20230417.173710/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/meta.py` & `returnn-1.20230417.173710/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/multi_proc.py` & `returnn-1.20230417.173710/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/normalization_data.py` & `returnn-1.20230417.173710/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/numpy_dump.py` & `returnn-1.20230417.173710/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/raw_wav.py` & `returnn-1.20230417.173710/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/sprint.py` & `returnn-1.20230417.173710/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/stereo.py` & `returnn-1.20230417.173710/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230417.173710/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/datasets/util/vocabulary.py` & `returnn-1.20230417.173710/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/engine/base.py` & `returnn-1.20230417.173710/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/engine/batch.py` & `returnn-1.20230417.173710/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230417.173710/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230417.173710/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230417.173710/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230417.173710/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/graph_editor/edit.py` & `returnn-1.20230417.173710/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230417.173710/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/graph_editor/select.py` & `returnn-1.20230417.173710/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230417.173710/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/graph_editor/transform.py` & `returnn-1.20230417.173710/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/extern/graph_editor/util.py` & `returnn-1.20230417.173710/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/__init__.py` & `returnn-1.20230417.173710/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/_backend.py` & `returnn-1.20230417.173710/returnn/frontend/_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,14 +313,23 @@
         :param out_dims: list of dims where sum(out_dims) == axis
         :return: tuple of tensors, same amount as out_dims,
             with the same shape as source, but with the specified axis replaced by the out_dims
         """
         raise NotImplementedError
 
     @staticmethod
+    def expand_dim(source: Tensor, dim: Dim) -> Tensor:
+        """
+        :param source:
+        :param dim:
+        :return: source with dim added
+        """
+        raise NotImplementedError
+
+    @staticmethod
     def pad(
         source: Tensor,
         *,
         axes: Sequence[Dim],
         padding: Sequence[Tuple[Union[Dim, int], Union[Dim, int]]],
         out_dims: Sequence[Dim],
         mode: str = "constant",
```

### Comparing `returnn-1.20230417.170727/returnn/frontend/_numpy_backend.py` & `returnn-1.20230417.173710/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/_utils.py` & `returnn-1.20230417.173710/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/array_.py` & `returnn-1.20230417.173710/returnn/frontend/array_.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 __all__ = [
     "convert_to_tensor",
     "constant",
     "cast",
     "merge_dims",
     "split_dims",
     "split",
+    "expand_dim",
     "pad",
     "cum_concat_step",
     "masked_select",
     "pack",
     "gather",
 ]
 
@@ -177,14 +178,27 @@
     :return: tuple of tensors, same amount as out_dims,
         with the same shape as source, but with the specified axis replaced by the out_dims
     """
     # noinspection PyProtectedMember
     return source._raw_backend.split(source, axis=axis, out_dims=out_dims)
 
 
+def expand_dim(source: Tensor, dim: Dim) -> Tensor:
+    """
+    Expand the source by the given dimension.
+
+    Note that this is *never* needed for broadcasting.
+    All broadcasting should always happen automatically.
+
+    This might be needed for convolution or concatenation.
+    """
+    # noinspection PyProtectedMember
+    return source._raw_backend.expand_dim(source, dim=dim)
+
+
 def pad(
     source: Tensor,
     *,
     axes: Sequence[Dim],
     padding: Sequence[Tuple[Union[Dim, int], Union[Dim, int]]],
     out_dims: Optional[Sequence[Dim]] = None,
     mode: str = "constant",
```

### Comparing `returnn-1.20230417.170727/returnn/frontend/attention.py` & `returnn-1.20230417.173710/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/cond.py` & `returnn-1.20230417.173710/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/const.py` & `returnn-1.20230417.173710/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/container.py` & `returnn-1.20230417.173710/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/conv.py` & `returnn-1.20230417.173710/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/dims.py` & `returnn-1.20230417.173710/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/dropout.py` & `returnn-1.20230417.173710/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/dtype.py` & `returnn-1.20230417.173710/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/init.py` & `returnn-1.20230417.173710/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/linear.py` & `returnn-1.20230417.173710/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/loss.py` & `returnn-1.20230417.173710/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/math_.py` & `returnn-1.20230417.173710/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/matmul.py` & `returnn-1.20230417.173710/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/module.py` & `returnn-1.20230417.173710/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/normalization.py` & `returnn-1.20230417.173710/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/parameter.py` & `returnn-1.20230417.173710/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/rand.py` & `returnn-1.20230417.173710/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/reduce.py` & `returnn-1.20230417.173710/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/run_ctx.py` & `returnn-1.20230417.173710/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/state.py` & `returnn-1.20230417.173710/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/frontend/types.py` & `returnn-1.20230417.173710/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/import_/common.py` & `returnn-1.20230417.173710/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/import_/git.py` & `returnn-1.20230417.173710/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/import_/import_.py` & `returnn-1.20230417.173710/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/learning_rate_control.py` & `returnn-1.20230417.173710/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/log.py` & `returnn-1.20230417.173710/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/native_op.cpp` & `returnn-1.20230417.173710/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/native_op.py` & `returnn-1.20230417.173710/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/pretrain.py` & `returnn-1.20230417.173710/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/sprint/cache.py` & `returnn-1.20230417.173710/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/sprint/control.py` & `returnn-1.20230417.173710/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/sprint/error_signals.py` & `returnn-1.20230417.173710/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/sprint/extern_interface.py` & `returnn-1.20230417.173710/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/sprint/interface.py` & `returnn-1.20230417.173710/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tensor/_dim_extra.py` & `returnn-1.20230417.173710/returnn/tensor/_dim_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tensor/_tensor_extra.py` & `returnn-1.20230417.173710/returnn/tensor/_tensor_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230417.173710/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230417.173710/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230417.173710/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tensor/dim.py` & `returnn-1.20230417.173710/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tensor/marked_dim.py` & `returnn-1.20230417.173710/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tensor/tensor.py` & `returnn-1.20230417.173710/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tensor/tensor_dict.py` & `returnn-1.20230417.173710/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/compat.py` & `returnn-1.20230417.173710/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/data_pipeline.py` & `returnn-1.20230417.173710/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/distributed.py` & `returnn-1.20230417.173710/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/engine.py` & `returnn-1.20230417.173710/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230417.173710/returnn/tf/frontend_layers/_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,26 @@
                     axis=src_axis_int, new_dim_tag=dim, name=f"{source.name}/split:{i}:{dim.description}"
                 ),
             )
             for i, dim in enumerate(out_dims)
         )
 
     @staticmethod
+    def expand_dim(source: Tensor, dim: Dim) -> Tensor:
+        """expand dim"""
+        # Some heuristic on the kind, which just determines where RETURNN puts the new axis.
+        if source.have_feature_axis():
+            axis = "spatial"
+        elif dim.is_static():
+            axis = "feature"
+        else:
+            axis = "spatial"
+        return rfl.make_layer({"class": "expand_dims", "from": source, "axis": axis, "dim": dim}, name="expand_dims")
+
+    @staticmethod
     def pad(
         source: Tensor,
         *,
         axes: Sequence[Dim],
         padding: Sequence[Tuple[Union[Dim, int], Union[Dim, int]]],
         out_dims: Sequence[Dim],
         mode: str = "constant",
```

### Comparing `returnn-1.20230417.170727/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230417.173710/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230417.173710/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230417.173710/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230417.173710/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230417.173710/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230417.173710/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230417.173710/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230417.173710/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/horovod.py` & `returnn-1.20230417.173710/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230417.173710/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/layers/base.py` & `returnn-1.20230417.173710/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/layers/basic.py` & `returnn-1.20230417.173710/returnn/tf/layers/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -5103,16 +5103,17 @@
         """
         if isinstance(axis, int):
             return axis
         assert isinstance(axis, str)
         axis = axis.lower()
         if axis in ["f", "feature"]:
             assert not data.sparse
-            assert data.feature_dim_axis_or_unspecified is NotSpecified
-            return data.batch_ndim
+            if data.feature_dim_axis is None:
+                return data.batch_ndim
+            return data.feature_dim_axis + 1
         elif axis in ["spatial", "time", "t"]:
             if data.sparse:
                 return data.batch_ndim
             else:
                 return data.batch_ndim - 1
         else:
             raise Exception("invalid axis %r" % axis)
```

### Comparing `returnn-1.20230417.170727/returnn/tf/layers/rec.py` & `returnn-1.20230417.173710/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/layers/segmental_model.py` & `returnn-1.20230417.173710/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/layers/signal_processing.py` & `returnn-1.20230417.173710/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/native_op.py` & `returnn-1.20230417.173710/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/network.py` & `returnn-1.20230417.173710/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/sprint.py` & `returnn-1.20230417.173710/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/updater.py` & `returnn-1.20230417.173710/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/util/basic.py` & `returnn-1.20230417.173710/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/util/data.py` & `returnn-1.20230417.173710/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/util/ken_lm.py` & `returnn-1.20230417.173710/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/tf/util/open_fst.py` & `returnn-1.20230417.173710/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/torch/data/pipeline.py` & `returnn-1.20230417.173710/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230417.173710/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/torch/data/tensor_utils.py` & `returnn-1.20230417.173710/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/torch/engine.py` & `returnn-1.20230417.173710/returnn/torch/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/torch/frontend/_backend.py` & `returnn-1.20230417.173710/returnn/torch/frontend/_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,40 @@
             for i, dim in enumerate(out_dims)
         )
         for i, out in enumerate(out_tuple):
             out.raw_tensor = out_raw_list[i]
         return out_tuple
 
     @staticmethod
+    def expand_dim(source: Tensor, dim: Dim) -> Tensor:
+        """expand dim"""
+        assert dim not in source.dims
+        # Some heuristic where to put the new dim.
+        axis = len(source.dims)  # default: at the end
+        if dim.is_static():
+            if source.have_feature_axis():
+                axis = source.feature_dim_axis
+        if dim.is_dynamic():
+            for i, d in reversed(enumerate(source.dims)):
+                assert isinstance(d, Dim)
+                if d.is_dynamic():
+                    axis = i + 1
+                    break
+        new_dim_tags = list(source.dims)
+        new_dim_tags.insert(axis, dim)
+        out = source.copy_template_new_dim_tags(new_dim_tags)
+        if source.feature_dim:
+            out.feature_dim = source.feature_dim
+        out_raw = torch.unsqueeze(source.raw_tensor, axis)
+        if dim.is_dynamic() or dim.dimension != 1:
+            out_raw = torch.tile(out_raw, [dim.get_dim_value() if d == dim else 1 for d in out.dims])
+        out.raw_tensor = out_raw
+        return out
+
+    @staticmethod
     def pad(
         source: Tensor,
         *,
         axes: Sequence[Dim],
         padding: Sequence[Tuple[Union[Dim, int], Union[Dim, int]]],
         out_dims: Sequence[Dim],
         mode: str = "constant",
```

### Comparing `returnn-1.20230417.170727/returnn/torch/frontend/_rand.py` & `returnn-1.20230417.173710/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/torch/frontend/bridge.py` & `returnn-1.20230417.173710/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/torch/updater.py` & `returnn-1.20230417.173710/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/util/basic.py` & `returnn-1.20230417.173710/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/util/better_exchook.py` & `returnn-1.20230417.173710/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/util/bpe.py` & `returnn-1.20230417.173710/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/util/debug.py` & `returnn-1.20230417.173710/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/util/debug_helpers.py` & `returnn-1.20230417.173710/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/util/fsa.py` & `returnn-1.20230417.173710/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230417.173710/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/util/pprint.py` & `returnn-1.20230417.173710/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/util/py-to-pickle.cpp` & `returnn-1.20230417.173710/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/util/sig_proc.py` & `returnn-1.20230417.173710/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn/util/task_system.py` & `returnn-1.20230417.173710/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/returnn.egg-info/PKG-INFO` & `returnn-1.20230417.173710/returnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230417.170727
+Version: 1.20230417.173710
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230417.170727/returnn.egg-info/SOURCES.txt` & `returnn-1.20230417.173710/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/setup.py` & `returnn-1.20230417.173710/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/DummySprintExec.py` & `returnn-1.20230417.173710/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230417.173710/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230417.173710/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230417.173710/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/_set_num_threads1.py` & `returnn-1.20230417.173710/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/_setup_test_env.py` & `returnn-1.20230417.173710/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/bpe-unicode-demo.codes` & `returnn-1.20230417.173710/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/bpe-unicode-demo.vocab` & `returnn-1.20230417.173710/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/lexicon_opt.isyms` & `returnn-1.20230417.173710/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/lexicon_opt.jpg` & `returnn-1.20230417.173710/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/lint_common.py` & `returnn-1.20230417.173710/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/pycharm-inspect.py` & `returnn-1.20230417.173710/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/pylint.py` & `returnn-1.20230417.173710/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/returnn-as-framework.py` & `returnn-1.20230417.173710/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/rf_utils.py` & `returnn-1.20230417.173710/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/spelling.dic` & `returnn-1.20230417.173710/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_Config.py` & `returnn-1.20230417.173710/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_Dataset.py` & `returnn-1.20230417.173710/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_Fsa.py` & `returnn-1.20230417.173710/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_GeneratingDataset.py` & `returnn-1.20230417.173710/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_HDFDataset.py` & `returnn-1.20230417.173710/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_LearningRateControl.py` & `returnn-1.20230417.173710/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_Log.py` & `returnn-1.20230417.173710/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_MultiProcDataset.py` & `returnn-1.20230417.173710/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_PTDataset.py` & `returnn-1.20230417.173710/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_Pretrain.py` & `returnn-1.20230417.173710/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_ResNet.py` & `returnn-1.20230417.173710/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_SprintDataset.py` & `returnn-1.20230417.173710/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_SprintInterface.py` & `returnn-1.20230417.173710/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_TFEngine.py` & `returnn-1.20230417.173710/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_TFNativeOp.py` & `returnn-1.20230417.173710/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_TFNetworkLayer.py` & `returnn-1.20230417.173710/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230417.173710/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230417.173710/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_TFUpdater.py` & `returnn-1.20230417.173710/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_TFUtil.py` & `returnn-1.20230417.173710/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_TF_determinism.py` & `returnn-1.20230417.173710/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_TaskSystem.py` & `returnn-1.20230417.173710/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230417.173710/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_TranslationDataset.py` & `returnn-1.20230417.173710/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_Util.py` & `returnn-1.20230417.173710/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_demos.py` & `returnn-1.20230417.173710/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_fork_exec.py` & `returnn-1.20230417.173710/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_hdf_dump.py` & `returnn-1.20230417.173710/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_rf_array.py` & `returnn-1.20230417.173710/tests/test_rf_array.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,36 @@
     def _forward_step(*, model: _Net, extern_data: TensorDict):
         out, pack_dim = model(extern_data["data"])
         out.mark_as_default_output(shape=(pack_dim, in_dim))
 
     run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
 
 
+def test_expand_dim():
+    time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
+    in_dim = Dim(7, name="in")
+    expand_dim = Dim(3, name="expand")
+    extern_data = TensorDict(
+        {
+            "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
+        }
+    )
+
+    class _Net(rf.Module):
+        def __call__(self, x: Tensor) -> Tensor:
+            return rf.expand_dim(x, expand_dim)
+
+    # noinspection PyShadowingNames
+    def _forward_step(*, model: _Net, extern_data: TensorDict):
+        out = model(extern_data["data"])
+        out.mark_as_default_output(shape=(batch_dim, time_dim, expand_dim, in_dim))
+
+    run_model(extern_data, lambda *, epoch, step: _Net(), _forward_step)
+
+
 def test_pad():
     time_dim = Dim(Tensor("time", [batch_dim], dtype="int32"))
     in_dim = Dim(7, name="in")
     extern_data = TensorDict(
         {
             "data": Tensor("data", [batch_dim, time_dim, in_dim], dtype="float32"),
         }
```

### Comparing `returnn-1.20230417.170727/tests/test_rf_attention.py` & `returnn-1.20230417.173710/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_rf_base.py` & `returnn-1.20230417.173710/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_rf_container.py` & `returnn-1.20230417.173710/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_rf_conv.py` & `returnn-1.20230417.173710/tests/test_rf_conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_rf_normalization.py` & `returnn-1.20230417.173710/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_tensor.py` & `returnn-1.20230417.173710/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_tools.py` & `returnn-1.20230417.173710/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_torch_frontend.py` & `returnn-1.20230417.173710/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tests/test_torch_internal_frontend.py` & `returnn-1.20230417.173710/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/analyze-dataset-batches.py` & `returnn-1.20230417.173710/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/bliss-collect-seq-lens.py` & `returnn-1.20230417.173710/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/bliss-dump-text.py` & `returnn-1.20230417.173710/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/bliss-get-segment-names.py` & `returnn-1.20230417.173710/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/bliss-to-ogg-zip.py` & `returnn-1.20230417.173710/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/bpe-create-lexicon.py` & `returnn-1.20230417.173710/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/calculate-word-error-rate.py` & `returnn-1.20230417.173710/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/cleanup-old-models.py` & `returnn-1.20230417.173710/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/collect-orth-symbols.py` & `returnn-1.20230417.173710/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/collect-words.py` & `returnn-1.20230417.173710/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/compile_native_op.py` & `returnn-1.20230417.173710/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/compile_tf_graph.py` & `returnn-1.20230417.173710/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/debug-dump-search-scores.py` & `returnn-1.20230417.173710/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/debug-plot-search-scores.py` & `returnn-1.20230417.173710/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/dump-dataset-raw-strings.py` & `returnn-1.20230417.173710/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/dump-dataset.py` & `returnn-1.20230417.173710/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/dump-forward-stats.py` & `returnn-1.20230417.173710/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/dump-forward.py` & `returnn-1.20230417.173710/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/dump-network-json.py` & `returnn-1.20230417.173710/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/dump-pickle.py` & `returnn-1.20230417.173710/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230417.173710/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/get-attention-weights.py` & `returnn-1.20230417.173710/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/get-best-model-epoch.py` & `returnn-1.20230417.173710/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/hdf_dump.py` & `returnn-1.20230417.173710/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230417.173710/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/import-blocks-mt-model.py` & `returnn-1.20230417.173710/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/import-t2t-mt-model.py` & `returnn-1.20230417.173710/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/lattice_rescorer/Makefile` & `returnn-1.20230417.173710/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/lattice_rescorer/README.md` & `returnn-1.20230417.173710/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/lattice_rescorer/example/README.md` & `returnn-1.20230417.173710/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230417.173710/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230417.173710/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230417.173710/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/lattice_rescorer/file.h` & `returnn-1.20230417.173710/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230417.173710/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230417.173710/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/lattice_rescorer/main.cc` & `returnn-1.20230417.173710/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230417.173710/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230417.173710/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230417.173710/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/tf_avg_checkpoints.py` & `returnn-1.20230417.173710/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/tf_inspect_checkpoint.py` & `returnn-1.20230417.173710/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230417.170727/tools/tf_inspect_summary_log.py` & `returnn-1.20230417.173710/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

