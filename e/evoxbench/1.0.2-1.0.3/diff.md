# Comparing `tmp/evoxbench-1.0.2.tar.gz` & `tmp/evoxbench-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evoxbench-1.0.2.tar", last modified: Wed Feb  8 11:42:58 2023, max compression
+gzip compressed data, was "evoxbench-1.0.3.tar", last modified: Mon Apr 17 03:20:24 2023, max compression
```

## Comparing `evoxbench-1.0.2.tar` & `evoxbench-1.0.3.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.909992 evoxbench-1.0.2/
--rw-r--r--   0 satan     (1000) satan     (1000)    11357 2023-02-08 11:42:34.000000 evoxbench-1.0.2/LICENSE
--rw-r--r--   0 satan     (1000) satan     (1000)      656 2023-02-08 11:42:34.000000 evoxbench-1.0.2/NOTICE
--rw-r--r--   0 satan     (1000) satan     (1000)     2932 2023-02-08 11:42:58.909992 evoxbench-1.0.2/PKG-INFO
--rw-r--r--   0 satan     (1000) satan     (1000)     1881 2023-02-08 11:42:34.000000 evoxbench-1.0.2/README.md
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.889992 evoxbench-1.0.2/evoxbench/
--rw-r--r--   0 satan     (1000) satan     (1000)       71 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/__init__.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.899992 evoxbench-1.0.2/evoxbench/api/
--rw-r--r--   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/api/__init__.py
--rw-r--r--   0 satan     (1000) satan     (1000)     8195 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/api/rpc.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.899992 evoxbench-1.0.2/evoxbench/benchmarks/
--rw-r--r--   0 satan     (1000) satan     (1000)      201 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/benchmarks/__init__.py
--rw-r--r--   0 satan     (1000) satan     (1000)    15898 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/benchmarks/darts.py
--rw-r--r--   0 satan     (1000) satan     (1000)    23584 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/benchmarks/mnv3.py
--rw-r--r--   0 satan     (1000) satan     (1000)     7058 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/benchmarks/nats.py
--rw-r--r--   0 satan     (1000) satan     (1000)    14937 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/benchmarks/nb101.py
--rw-r--r--   0 satan     (1000) satan     (1000)     9538 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/benchmarks/nb201.py
--rw-r--r--   0 satan     (1000) satan     (1000)    20401 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/benchmarks/resnet.py
--rw-r--r--   0 satan     (1000) satan     (1000)    32145 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/benchmarks/transformer.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.899992 evoxbench-1.0.2/evoxbench/database/
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.899992 evoxbench-1.0.2/evoxbench/database/ORM/
--rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/ORM/__init__.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      383 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/ORM/asgi.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)     3583 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/ORM/settings.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      807 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/ORM/urls.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      383 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/ORM/wsgi.py
--rw-r--r--   0 satan     (1000) satan     (1000)       72 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/__init__.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.899992 evoxbench-1.0.2/evoxbench/database/darts/
--rw-r--r--   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/darts/__init__.py
--rw-r--r--   0 satan     (1000) satan     (1000)      239 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/darts/admin.py
--rw-r--r--   0 satan     (1000) satan     (1000)      148 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/darts/apps.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.899992 evoxbench-1.0.2/evoxbench/database/darts/migrations/
--rw-r--r--   0 satan     (1000) satan     (1000)     1182 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/darts/migrations/0001_initial.py
--rw-r--r--   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/darts/migrations/__init__.py
--rw-r--r--   0 satan     (1000) satan     (1000)      443 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/darts/models.py
--rw-r--r--   0 satan     (1000) satan     (1000)       60 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/darts/tests.py
--rw-r--r--   0 satan     (1000) satan     (1000)       63 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/darts/views.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.899992 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/
--rw-r--r--   0 satan     (1000) satan     (1000)       44 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/__init__.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.899992 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/fbnet_models/
--rw-r--r--   0 satan     (1000) satan     (1000)       37 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/fbnet_models/__init__.py
--rw-r--r--   0 satan     (1000) satan     (1000)    11030 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/fbnet_models/model_infer.py
--rw-r--r--   0 satan     (1000) satan     (1000)    11588 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/hw_nas_bench_api.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.899992 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/
--rw-r--r--   0 satan     (1000) satan     (1000)     3973 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/CifarDenseNet.py
--rw-r--r--   0 satan     (1000) satan     (1000)     6228 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/CifarResNet.py
--rw-r--r--   0 satan     (1000) satan     (1000)     3432 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/CifarWideResNet.py
--rw-r--r--   0 satan     (1000) satan     (1000)     4034 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/ImageNet_MobileNetV2.py
--rw-r--r--   0 satan     (1000) satan     (1000)     6849 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/ImageNet_ResNet.py
--rw-r--r--   0 satan     (1000) satan     (1000)      891 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/SharedUtils.py
--rw-r--r--   0 satan     (1000) satan     (1000)    10992 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/__init__.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.899992 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_infers/
--rw-r--r--   0 satan     (1000) satan     (1000)      240 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_infers/__init__.py
--rw-r--r--   0 satan     (1000) satan     (1000)     4821 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_infers/cells.py
--rw-r--r--   0 satan     (1000) satan     (1000)     3405 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_infers/nasnet_cifar.py
--rw-r--r--   0 satan     (1000) satan     (1000)     2114 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_infers/tiny_network.py
--rw-r--r--   0 satan     (1000) satan     (1000)    16598 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_operations.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.899992 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/
--rw-r--r--   0 satan     (1000) satan     (1000)     1265 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/__init__.py
--rw-r--r--   0 satan     (1000) satan     (1000)      332 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/_test_module.py
--rw-r--r--   0 satan     (1000) satan     (1000)    12923 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/generic_model.py
--rw-r--r--   0 satan     (1000) satan     (1000)     9146 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/genotypes.py
--rw-r--r--   0 satan     (1000) satan     (1000)     8473 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_cells.py
--rw-r--r--   0 satan     (1000) satan     (1000)     4209 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_darts.py
--rw-r--r--   0 satan     (1000) satan     (1000)     5418 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_darts_nasnet.py
--rw-r--r--   0 satan     (1000) satan     (1000)     4168 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_enas.py
--rw-r--r--   0 satan     (1000) satan     (1000)     2548 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_enas_utils.py
--rw-r--r--   0 satan     (1000) satan     (1000)     4933 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_gdas.py
--rw-r--r--   0 satan     (1000) satan     (1000)     5874 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_gdas_frc_nasnet.py
--rw-r--r--   0 satan     (1000) satan     (1000)     6271 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_gdas_nasnet.py
--rw-r--r--   0 satan     (1000) satan     (1000)     3631 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_random.py
--rw-r--r--   0 satan     (1000) satan     (1000)     6711 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_setn.py
--rw-r--r--   0 satan     (1000) satan     (1000)     6854 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_setn_nasnet.py
--rw-r--r--   0 satan     (1000) satan     (1000)     2769 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/clone_weights.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.899992 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/
--rw-r--r--   0 satan     (1000) satan     (1000)      630 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/__init__.py
--rw-r--r--   0 satan     (1000) satan     (1000)     1286 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/attention_args.py
--rw-r--r--   0 satan     (1000) satan     (1000)     1536 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/basic_args.py
--rw-r--r--   0 satan     (1000) satan     (1000)     1208 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/cls_init_args.py
--rw-r--r--   0 satan     (1000) satan     (1000)     1563 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/cls_kd_args.py
--rw-r--r--   0 satan     (1000) satan     (1000)     3934 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/configure_utils.py
--rw-r--r--   0 satan     (1000) satan     (1000)     1786 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/pruning_args.py
--rw-r--r--   0 satan     (1000) satan     (1000)     1604 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/random_baseline.py
--rw-r--r--   0 satan     (1000) satan     (1000)     2182 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/search_args.py
--rw-r--r--   0 satan     (1000) satan     (1000)     2143 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/search_single_args.py
--rw-r--r--   0 satan     (1000) satan     (1000)     1015 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/share_args.py
--rw-r--r--   0 satan     (1000) satan     (1000)      513 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/initialization.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.909992 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/
--rw-r--r--   0 satan     (1000) satan     (1000)     7386 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/InferCifarResNet.py
--rw-r--r--   0 satan     (1000) satan     (1000)     6619 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/InferCifarResNet_depth.py
--rw-r--r--   0 satan     (1000) satan     (1000)     6983 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/InferCifarResNet_width.py
--rw-r--r--   0 satan     (1000) satan     (1000)     7873 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/InferImagenetResNet.py
--rw-r--r--   0 satan     (1000) satan     (1000)     5308 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/InferMobileNetV2.py
--rw-r--r--   0 satan     (1000) satan     (1000)     2449 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/InferTinyCellNet.py
--rw-r--r--   0 satan     (1000) satan     (1000)      475 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/__init__.py
--rw-r--r--   0 satan     (1000) satan     (1000)      178 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/shared_utils.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.909992 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/
--rw-r--r--   0 satan     (1000) satan     (1000)    26869 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchCifarResNet.py
--rw-r--r--   0 satan     (1000) satan     (1000)    16874 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchCifarResNet_depth.py
--rw-r--r--   0 satan     (1000) satan     (1000)    20558 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchCifarResNet_width.py
--rw-r--r--   0 satan     (1000) satan     (1000)    25619 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchImagenetResNet.py
--rw-r--r--   0 satan     (1000) satan     (1000)    15733 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchSimResNet_width.py
--rw-r--r--   0 satan     (1000) satan     (1000)     4173 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SoftSelect.py
--rw-r--r--   0 satan     (1000) satan     (1000)      504 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/__init__.py
--rw-r--r--   0 satan     (1000) satan     (1000)     6480 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/generic_size_tiny_cell_model.py
--rw-r--r--   0 satan     (1000) satan     (1000)      677 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/test.py
--rw-r--r--   0 satan     (1000) satan     (1000)     2252 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/init.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      659 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/manage.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.909992 evoxbench-1.0.2/evoxbench/database/mobilenetv3/
--rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/mobilenetv3/__init__.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)       63 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/mobilenetv3/admin.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      154 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/mobilenetv3/apps.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.909992 evoxbench-1.0.2/evoxbench/database/mobilenetv3/migrations/
--rw-r--r--   0 satan     (1000) satan     (1000)     1000 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/mobilenetv3/migrations/0001_initial.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/mobilenetv3/migrations/__init__.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      293 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/mobilenetv3/models.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)       60 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/mobilenetv3/tests.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)       63 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/mobilenetv3/views.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.909992 evoxbench-1.0.2/evoxbench/database/nasbench101/
--rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench101/__init__.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      245 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench101/admin.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      154 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench101/apps.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.909992 evoxbench-1.0.2/evoxbench/database/nasbench101/migrations/
--rwxr-xr-x   0 satan     (1000) satan     (1000)      990 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench101/migrations/0001_initial.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench101/migrations/__init__.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      594 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench101/models.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)       60 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench101/tests.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)       63 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench101/views.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.909992 evoxbench-1.0.2/evoxbench/database/nasbench201/
--rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench201/__init__.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      262 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench201/admin.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      154 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench201/apps.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.909992 evoxbench-1.0.2/evoxbench/database/nasbench201/migrations/
--rwxr-xr-x   0 satan     (1000) satan     (1000)      860 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench201/migrations/0001_initial.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      547 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench201/migrations/0002_auto_20220320_1447.py
--rw-r--r--   0 satan     (1000) satan     (1000)      398 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench201/migrations/0003_nasbench201result_hw_info.py
--rw-r--r--   0 satan     (1000) satan     (1000)      407 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench201/migrations/0004_nasbench201result_more_info.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench201/migrations/__init__.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      535 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench201/models.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)       60 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench201/tests.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)       63 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbench201/views.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.909992 evoxbench-1.0.2/evoxbench/database/nasbenchbase/
--rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbenchbase/__init__.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbenchbase/admin.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      148 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbenchbase/apps.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)       52 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbenchbase/convert.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      150 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbenchbase/generate.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.909992 evoxbench-1.0.2/evoxbench/database/nasbenchbase/migrations/
--rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbenchbase/migrations/__init__.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      428 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbenchbase/models.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)       60 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbenchbase/tests.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)       63 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/nasbenchbase/views.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.909992 evoxbench-1.0.2/evoxbench/database/natsbenchsss/
--rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/natsbenchsss/__init__.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      266 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/natsbenchsss/admin.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      156 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/natsbenchsss/apps.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.909992 evoxbench-1.0.2/evoxbench/database/natsbenchsss/migrations/
--rw-r--r--   0 satan     (1000) satan     (1000)      917 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/natsbenchsss/migrations/0001_initial.py
--rw-r--r--   0 satan     (1000) satan     (1000)      383 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/natsbenchsss/migrations/0002_natsbenchresult_cost.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/natsbenchsss/migrations/__init__.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      372 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/natsbenchsss/models.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)       60 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/natsbenchsss/tests.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)       63 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/natsbenchsss/views.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.909992 evoxbench-1.0.2/evoxbench/database/resnet50/
--rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/resnet50/__init__.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)       63 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/resnet50/admin.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      148 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/resnet50/apps.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.909992 evoxbench-1.0.2/evoxbench/database/resnet50/migrations/
--rw-r--r--   0 satan     (1000) satan     (1000)      997 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/resnet50/migrations/0001_initial.py
--rw-r--r--   0 satan     (1000) satan     (1000)      326 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/resnet50/migrations/0002_remove_resnet50result_latency.py
--rw-r--r--   0 satan     (1000) satan     (1000)      538 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/resnet50/migrations/0003_rename_test_acc_resnet50result_test_err_and_more.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/resnet50/migrations/__init__.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)      292 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/resnet50/models.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)       60 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/resnet50/tests.py
--rwxr-xr-x   0 satan     (1000) satan     (1000)       63 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/database/resnet50/views.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.909992 evoxbench-1.0.2/evoxbench/modules/
--rw-r--r--   0 satan     (1000) satan     (1000)      109 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/modules/__init__.py
--rw-r--r--   0 satan     (1000) satan     (1000)     4856 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/modules/benchmark.py
--rw-r--r--   0 satan     (1000) satan     (1000)      540 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/modules/evaluator.py
--rw-r--r--   0 satan     (1000) satan     (1000)     1440 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/modules/search_space.py
--rw-r--r--   0 satan     (1000) satan     (1000)     3937 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/modules/surrogate_model.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.909992 evoxbench-1.0.2/evoxbench/test_suites/
--rw-r--r--   0 satan     (1000) satan     (1000)       45 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/test_suites/__init__.py
--rw-r--r--   0 satan     (1000) satan     (1000)     1716 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/test_suites/c10mop.py
--rw-r--r--   0 satan     (1000) satan     (1000)     1355 2023-02-08 11:42:34.000000 evoxbench-1.0.2/evoxbench/test_suites/in1kmop.py
-drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-02-08 11:42:58.899992 evoxbench-1.0.2/evoxbench.egg-info/
--rw-r--r--   0 satan     (1000) satan     (1000)     2932 2023-02-08 11:42:58.000000 evoxbench-1.0.2/evoxbench.egg-info/PKG-INFO
--rw-r--r--   0 satan     (1000) satan     (1000)     8859 2023-02-08 11:42:58.000000 evoxbench-1.0.2/evoxbench.egg-info/SOURCES.txt
--rw-r--r--   0 satan     (1000) satan     (1000)        1 2023-02-08 11:42:58.000000 evoxbench-1.0.2/evoxbench.egg-info/dependency_links.txt
--rw-r--r--   0 satan     (1000) satan     (1000)       56 2023-02-08 11:42:58.000000 evoxbench-1.0.2/evoxbench.egg-info/entry_points.txt
--rw-r--r--   0 satan     (1000) satan     (1000)        1 2023-02-08 11:42:58.000000 evoxbench-1.0.2/evoxbench.egg-info/not-zip-safe
--rw-r--r--   0 satan     (1000) satan     (1000)       39 2023-02-08 11:42:58.000000 evoxbench-1.0.2/evoxbench.egg-info/requires.txt
--rw-r--r--   0 satan     (1000) satan     (1000)       10 2023-02-08 11:42:58.000000 evoxbench-1.0.2/evoxbench.egg-info/top_level.txt
--rw-r--r--   0 satan     (1000) satan     (1000)       38 2023-02-08 11:42:58.909992 evoxbench-1.0.2/setup.cfg
--rw-r--r--   0 satan     (1000) satan     (1000)     4923 2023-02-08 11:42:49.000000 evoxbench-1.0.2/setup.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.344576 evoxbench-1.0.3/
+-rw-r--r--   0 satan     (1000) satan     (1000)    11558 2023-04-17 03:19:59.000000 evoxbench-1.0.3/LICENSE
+-rw-r--r--   0 satan     (1000) satan     (1000)      672 2023-04-17 03:19:59.000000 evoxbench-1.0.3/NOTICE
+-rw-r--r--   0 satan     (1000) satan     (1000)     3909 2023-04-17 03:20:24.344576 evoxbench-1.0.3/PKG-INFO
+-rw-r--r--   0 satan     (1000) satan     (1000)     2959 2023-04-17 03:19:59.000000 evoxbench-1.0.3/README.md
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.324576 evoxbench-1.0.3/evoxbench/
+-rw-r--r--   0 satan     (1000) satan     (1000)       75 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/__init__.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.324576 evoxbench-1.0.3/evoxbench/api/
+-rw-r--r--   0 satan     (1000) satan     (1000)        0 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/api/__init__.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     8449 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/api/rpc.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.324576 evoxbench-1.0.3/evoxbench/benchmarks/
+-rw-r--r--   0 satan     (1000) satan     (1000)      212 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/benchmarks/__init__.py
+-rw-r--r--   0 satan     (1000) satan     (1000)    16372 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/benchmarks/darts.py
+-rw-r--r--   0 satan     (1000) satan     (1000)    24220 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/benchmarks/mnv3.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     7262 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/benchmarks/nats.py
+-rw-r--r--   0 satan     (1000) satan     (1000)    15321 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/benchmarks/nb101.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     9770 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/benchmarks/nb201.py
+-rw-r--r--   0 satan     (1000) satan     (1000)    20931 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/benchmarks/resnet.py
+-rw-r--r--   0 satan     (1000) satan     (1000)    32997 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/benchmarks/transformer.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.324576 evoxbench-1.0.3/evoxbench/database/
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.324576 evoxbench-1.0.3/evoxbench/database/ORM/
+-rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/ORM/__init__.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      399 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/ORM/asgi.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)     3715 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/ORM/settings.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      831 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/ORM/urls.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      399 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/ORM/wsgi.py
+-rw-r--r--   0 satan     (1000) satan     (1000)       77 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/__init__.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.324576 evoxbench-1.0.3/evoxbench/database/darts/
+-rw-r--r--   0 satan     (1000) satan     (1000)        0 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/darts/__init__.py
+-rw-r--r--   0 satan     (1000) satan     (1000)      249 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/darts/admin.py
+-rw-r--r--   0 satan     (1000) satan     (1000)      154 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/darts/apps.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.324576 evoxbench-1.0.3/evoxbench/database/darts/migrations/
+-rw-r--r--   0 satan     (1000) satan     (1000)     1215 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/darts/migrations/0001_initial.py
+-rw-r--r--   0 satan     (1000) satan     (1000)        0 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/darts/migrations/__init__.py
+-rw-r--r--   0 satan     (1000) satan     (1000)      455 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/darts/models.py
+-rw-r--r--   0 satan     (1000) satan     (1000)       63 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/darts/tests.py
+-rw-r--r--   0 satan     (1000) satan     (1000)       66 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/darts/views.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.324576 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/
+-rw-r--r--   0 satan     (1000) satan     (1000)       45 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/__init__.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.324576 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/fbnet_models/
+-rw-r--r--   0 satan     (1000) satan     (1000)       38 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/fbnet_models/__init__.py
+-rw-r--r--   0 satan     (1000) satan     (1000)    11323 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/fbnet_models/model_infer.py
+-rw-r--r--   0 satan     (1000) satan     (1000)    11848 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/hw_nas_bench_api.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/
+-rw-r--r--   0 satan     (1000) satan     (1000)     4081 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/CifarDenseNet.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     6392 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/CifarResNet.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     3526 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/CifarWideResNet.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     4139 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/ImageNet_MobileNetV2.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     7027 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/ImageNet_ResNet.py
+-rw-r--r--   0 satan     (1000) satan     (1000)      926 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/SharedUtils.py
+-rw-r--r--   0 satan     (1000) satan     (1000)    11200 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/__init__.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_infers/
+-rw-r--r--   0 satan     (1000) satan     (1000)      245 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_infers/__init__.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     4943 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_infers/cells.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     3481 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_infers/nasnet_cifar.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     2172 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_infers/tiny_network.py
+-rw-r--r--   0 satan     (1000) satan     (1000)    16954 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_operations.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/
+-rw-r--r--   0 satan     (1000) satan     (1000)     1292 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/__init__.py
+-rw-r--r--   0 satan     (1000) satan     (1000)      346 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/_test_module.py
+-rw-r--r--   0 satan     (1000) satan     (1000)    13235 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/generic_model.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     9360 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/genotypes.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     8677 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_cells.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     4310 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_darts.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     5536 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_darts_nasnet.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     4267 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_enas.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     2603 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_enas_utils.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     5049 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_gdas.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     6009 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_gdas_frc_nasnet.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     6408 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_gdas_nasnet.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     3717 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_random.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     6869 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_setn.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     7003 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_setn_nasnet.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     2835 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/clone_weights.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/
+-rw-r--r--   0 satan     (1000) satan     (1000)      643 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/__init__.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     1311 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/attention_args.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     1564 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/basic_args.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     1231 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/cls_init_args.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     1589 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/cls_kd_args.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     4053 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/configure_utils.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     1815 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/pruning_args.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     1631 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/random_baseline.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     2217 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/search_args.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     2177 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/search_single_args.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     1033 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/share_args.py
+-rw-r--r--   0 satan     (1000) satan     (1000)      529 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/initialization.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/
+-rw-r--r--   0 satan     (1000) satan     (1000)     7568 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/InferCifarResNet.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     6786 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/InferCifarResNet_depth.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     7158 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/InferCifarResNet_width.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     8061 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/InferImagenetResNet.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     5438 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/InferMobileNetV2.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     2510 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/InferTinyCellNet.py
+-rw-r--r--   0 satan     (1000) satan     (1000)      484 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/__init__.py
+-rw-r--r--   0 satan     (1000) satan     (1000)      183 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/shared_utils.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/
+-rw-r--r--   0 satan     (1000) satan     (1000)    27427 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchCifarResNet.py
+-rw-r--r--   0 satan     (1000) satan     (1000)    17246 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchCifarResNet_depth.py
+-rw-r--r--   0 satan     (1000) satan     (1000)    20998 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchCifarResNet_width.py
+-rw-r--r--   0 satan     (1000) satan     (1000)    26157 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchImagenetResNet.py
+-rw-r--r--   0 satan     (1000) satan     (1000)    16080 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchSimResNet_width.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     4294 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SoftSelect.py
+-rw-r--r--   0 satan     (1000) satan     (1000)      513 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/__init__.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     6634 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/generic_size_tiny_cell_model.py
+-rw-r--r--   0 satan     (1000) satan     (1000)      696 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/test.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     2315 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/init.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      681 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/manage.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/mobilenetv3/
+-rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/mobilenetv3/__init__.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)       66 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/mobilenetv3/admin.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      160 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/mobilenetv3/apps.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/mobilenetv3/migrations/
+-rw-r--r--   0 satan     (1000) satan     (1000)     1031 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/mobilenetv3/migrations/0001_initial.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/mobilenetv3/migrations/__init__.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      303 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/mobilenetv3/models.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)       63 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/mobilenetv3/tests.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)       66 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/mobilenetv3/views.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/nasbench101/
+-rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench101/__init__.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      255 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench101/admin.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      160 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench101/apps.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/nasbench101/migrations/
+-rwxr-xr-x   0 satan     (1000) satan     (1000)     1020 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench101/migrations/0001_initial.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench101/migrations/__init__.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      609 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench101/models.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)       63 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench101/tests.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)       66 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench101/views.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/nasbench201/
+-rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench201/__init__.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      272 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench201/admin.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      160 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench201/apps.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/nasbench201/migrations/
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      888 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench201/migrations/0001_initial.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      569 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench201/migrations/0002_auto_20220320_1447.py
+-rw-r--r--   0 satan     (1000) satan     (1000)      415 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench201/migrations/0003_nasbench201result_hw_info.py
+-rw-r--r--   0 satan     (1000) satan     (1000)      424 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench201/migrations/0004_nasbench201result_more_info.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench201/migrations/__init__.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      549 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench201/models.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)       63 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench201/tests.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)       66 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbench201/views.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/nasbenchbase/
+-rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbenchbase/__init__.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbenchbase/admin.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      154 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbenchbase/apps.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)       55 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbenchbase/convert.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      156 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbenchbase/generate.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/nasbenchbase/migrations/
+-rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbenchbase/migrations/__init__.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      443 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbenchbase/models.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)       63 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbenchbase/tests.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)       66 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/nasbenchbase/views.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/natsbenchsss/
+-rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/natsbenchsss/__init__.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      276 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/natsbenchsss/admin.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      162 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/natsbenchsss/apps.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/natsbenchsss/migrations/
+-rw-r--r--   0 satan     (1000) satan     (1000)      947 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/natsbenchsss/migrations/0001_initial.py
+-rw-r--r--   0 satan     (1000) satan     (1000)      400 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/natsbenchsss/migrations/0002_natsbenchresult_cost.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/natsbenchsss/migrations/__init__.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      384 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/natsbenchsss/models.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)       63 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/natsbenchsss/tests.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)       66 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/natsbenchsss/views.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/resnet50/
+-rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/resnet50/__init__.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)       66 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/resnet50/admin.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      154 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/resnet50/apps.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/database/resnet50/migrations/
+-rw-r--r--   0 satan     (1000) satan     (1000)     1028 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/resnet50/migrations/0001_initial.py
+-rw-r--r--   0 satan     (1000) satan     (1000)      342 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/resnet50/migrations/0002_remove_resnet50result_latency.py
+-rw-r--r--   0 satan     (1000) satan     (1000)      560 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/resnet50/migrations/0003_rename_test_acc_resnet50result_test_err_and_more.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/resnet50/migrations/__init__.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)      302 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/resnet50/models.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)       63 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/resnet50/tests.py
+-rwxr-xr-x   0 satan     (1000) satan     (1000)       66 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/database/resnet50/views.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/modules/
+-rw-r--r--   0 satan     (1000) satan     (1000)      113 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/modules/__init__.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     5003 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/modules/benchmark.py
+-rw-r--r--   0 satan     (1000) satan     (1000)      564 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/modules/evaluator.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     1496 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/modules/search_space.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     4070 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/modules/surrogate_model.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.334576 evoxbench-1.0.3/evoxbench/test_suites/
+-rw-r--r--   0 satan     (1000) satan     (1000)       47 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/test_suites/__init__.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     1755 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/test_suites/c10mop.py
+-rw-r--r--   0 satan     (1000) satan     (1000)     1395 2023-04-17 03:19:59.000000 evoxbench-1.0.3/evoxbench/test_suites/in1kmop.py
+drwxr-xr-x   0 satan     (1000) satan     (1000)        0 2023-04-17 03:20:24.324576 evoxbench-1.0.3/evoxbench.egg-info/
+-rw-r--r--   0 satan     (1000) satan     (1000)     3909 2023-04-17 03:20:24.000000 evoxbench-1.0.3/evoxbench.egg-info/PKG-INFO
+-rw-r--r--   0 satan     (1000) satan     (1000)     8859 2023-04-17 03:20:24.000000 evoxbench-1.0.3/evoxbench.egg-info/SOURCES.txt
+-rw-r--r--   0 satan     (1000) satan     (1000)        1 2023-04-17 03:20:24.000000 evoxbench-1.0.3/evoxbench.egg-info/dependency_links.txt
+-rw-r--r--   0 satan     (1000) satan     (1000)       56 2023-04-17 03:20:24.000000 evoxbench-1.0.3/evoxbench.egg-info/entry_points.txt
+-rw-r--r--   0 satan     (1000) satan     (1000)        1 2023-04-17 03:20:24.000000 evoxbench-1.0.3/evoxbench.egg-info/not-zip-safe
+-rw-r--r--   0 satan     (1000) satan     (1000)       39 2023-04-17 03:20:24.000000 evoxbench-1.0.3/evoxbench.egg-info/requires.txt
+-rw-r--r--   0 satan     (1000) satan     (1000)       10 2023-04-17 03:20:24.000000 evoxbench-1.0.3/evoxbench.egg-info/top_level.txt
+-rw-r--r--   0 satan     (1000) satan     (1000)       38 2023-04-17 03:20:24.344576 evoxbench-1.0.3/setup.cfg
+-rw-r--r--   0 satan     (1000) satan     (1000)     5041 2023-04-17 03:19:59.000000 evoxbench-1.0.3/setup.py
```

### Comparing `evoxbench-1.0.2/LICENSE` & `evoxbench-1.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `evoxbench-1.0.2/NOTICE` & `evoxbench-1.0.3/NOTICE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-EvoXBench
-Copyright 2022 EvoXGroup
-
-This product includes software developed at
-EvoXGroup (https://github.com/EvoXGroup/evoxbench/).
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-   http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
+EvoXBench
+Copyright 2022 EvoXGroup
+
+This product includes software developed at
+EvoXGroup (https://github.com/EvoXGroup/evoxbench/).
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+   http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
 limitations under the License.
```

### Comparing `evoxbench-1.0.2/evoxbench/benchmarks/mnv3.py` & `evoxbench-1.0.3/evoxbench/benchmarks/mnv3.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,636 +1,636 @@
-import os
-import copy
-from pathlib import Path
-
-import yaml
-import json
-import random
-import numpy as np
-from collections import OrderedDict
-
-from evoxbench.modules import SearchSpace, Evaluator, Benchmark, MLPPredictor
-
-__all__ = ['MobileNetV3SearchSpace', 'MobileNetV3Evaluator', 'MobileNetV3Benchmark']
-
-IMAGE_SIZE_LIST = (160, 176, 192, 208, 224)
-KERNEL_SIZE_LIST = (3, 5, 7)
-DEPTH_LIST = (2, 3, 4)
-EXPAND_RATIO_LIST = (3, 4, 6)
-WIDTH_MULT = 1.2
-
-
-def get_path(name):
-    return str(Path(os.environ.get("EVOXBENCH_MODEL", os.getcwd())) / "mnv3" / name)
-
-
-# ------------------- Following functions are specific to MobileNetV3 search space ------------------- #
-class MobileNetV3FeatureEncoder(object):
-    def __init__(self):
-
-        self.ks_map = self.construct_maps(keys=KERNEL_SIZE_LIST)
-        self.ex_map = self.construct_maps(keys=EXPAND_RATIO_LIST)
-        self.dp_map = self.construct_maps(keys=DEPTH_LIST)
-
-    # Helper for constructing the one-hot vectors.
-    @staticmethod
-    def construct_maps(keys):
-        d = dict()
-        keys = list(set(keys))
-        for k in keys:
-            if k not in d:
-                d[k] = len(list(d.keys()))
-        return d
-
-    def arch2feature(self, arch):
-        # This function converts a network config to a feature vector (128-D).
-        ks_list = copy.deepcopy(arch["ks"])
-        ex_list = copy.deepcopy(arch["e"])
-        d_list = copy.deepcopy(arch["d"])
-        r = copy.deepcopy(arch["r"])
-
-        start = 0
-        end = 4
-        for d in d_list:
-            for j in range(start + d, end):
-                ks_list[j] = 0
-                ex_list[j] = 0
-            start += 4
-            end += 4
-
-        # convert to onehot
-        ks_onehot = [0 for _ in range(60)]
-        ex_onehot = [0 for _ in range(60)]
-        r_onehot = [0 for _ in range(8)]
-
-        for i in range(20):
-            start = i * 3
-            if ks_list[i] != 0:
-                ks_onehot[start + self.ks_map[ks_list[i]]] = 1
-            if ex_list[i] != 0:
-                ex_onehot[start + self.ex_map[ex_list[i]]] = 1
-
-        r_onehot[(r - 112) // 16] = 1
-        return ks_onehot + ex_onehot + r_onehot
-
-
-class FLOPsPredictor:
-    channel_list = [24, 32, 48, 96, 136, 192]  # WIDTH_MULT = 1.2
-    stride_stages = [2, 2, 2, 1, 2]
-    act_stages = ["relu", "relu", "h_swish", "h_swish", "h_swish"]
-    se_stages = ['false', 'true', 'false', 'true', 'true']
-
-    def __init__(self,
-                 data_file_path=get_path("flops_model.json")):
-        with open(data_file_path, 'r') as f:
-            self.flops_dict = json.load(f)
-
-    def predict_flops(self, sample):
-        input_size = sample.get("r", 224)
-        flops_dict = self.flops_dict[str(input_size)]
-        assert "ks" in sample and "e" in sample and "d" in sample
-        assert len(sample["ks"]) == len(sample["e"]) and len(sample["ks"]) == 20
-        assert len(sample["d"]) == 5
-
-        flops = 0
-        # calculate the dynamic blocks
-        size = input_size // 2
-        for block_id in range(5):
-            for i in range(sample['d'][block_id]):
-                idx = block_id * 4 + i
-                out_channel = self.channel_list[block_id + 1]
-                k = sample['ks'][idx]
-                e = sample['e'][idx]
-                if i == 0:
-                    s = self.stride_stages[block_id]
-                    in_channel = self.channel_list[block_id]
-                else:
-                    s = 1
-                    in_channel = self.channel_list[block_id + 1]
-                act = self.act_stages[block_id]
-                se = self.se_stages[block_id]
-
-                in_channel = str(in_channel)
-                out_channel = str(out_channel)
-                k = str(k)
-                e = str(e)
-                s = str(s)
-                size_str = str(size)
-                # print(in_channel,out_channel,size, k,e,s,act,se)
-                flops = flops + flops_dict['MBConvLayerBlock'][in_channel][out_channel][size_str][k][e][s][act][se]
-                if s == "2":  # stride = 2 means half the HW
-                    size = (size + 1) // 2
-
-        flops += flops_dict["FirstBlockLayer"]
-        flops += flops_dict["LastLayers"]
-        return flops
-
-
-class ParamsPredictor:
-    channel_list = [24, 32, 48, 96, 136, 192]  # WIDTH_MULT = 1.2
-    stride_stages = [2, 2, 2, 1, 2]
-    act_stages = ["relu", "relu", "h_swish", "h_swish", "h_swish"]
-    se_stages = ['false', 'true', 'false', 'true', 'true']
-
-    def __init__(self,
-                 data_file_path=get_path("params_model.json")):
-        with open(data_file_path, 'r') as f:
-            self.params_dict = json.load(f)
-
-    def predict_params(self, sample):
-        assert "ks" in sample and "e" in sample and "d" in sample
-        assert len(sample["ks"]) == len(sample["e"]) and len(sample["ks"]) == 20
-        assert len(sample["d"]) == 5
-
-        params = 0
-        # calculate the dynamic layers
-
-        for block_id in range(5):
-            for i in range(sample['d'][block_id]):
-                idx = block_id * 4 + i
-                # print(idx)
-                out_channel = self.channel_list[block_id + 1]
-                k = sample['ks'][idx]
-                e = sample['e'][idx]
-                if i == 0:
-                    s = self.stride_stages[block_id]
-                    in_channel = self.channel_list[block_id]
-                else:
-                    s = 1
-                    in_channel = self.channel_list[block_id + 1]
-                act = self.act_stages[block_id]
-                se = self.se_stages[block_id]
-                in_channel = str(in_channel)
-                out_channel = str(out_channel)
-                k = str(k)
-                e = str(e)
-                s = str(s)
-                # print(in_channel, out_channel, k, e, s, act, se)
-                params = params + self.params_dict['MBConvLayer'][in_channel][out_channel][k][e][s][act][se]
-        params = params + self.params_dict['OtherLayer']
-
-        return params
-
-
-class LatencyEstimator(object):
-    def __init__(self, yaml_file_path=''):
-
-        with open(yaml_file_path, "r") as fp:
-            self.lut = yaml.load(fp, Loader=yaml.FullLoader)
-
-    @staticmethod
-    def repr_shape(shape):
-        if isinstance(shape, (list, tuple)):
-            return "x".join(str(_) for _ in shape)
-        elif isinstance(shape, str):
-            return shape
-        else:
-            return TypeError
-
-    def query(
-            self,
-            l_type: str,
-            input_shape,
-            output_shape,
-            mid=None,
-            ks=None,
-            stride=None,
-            id_skip=None,
-            se=None,
-            h_swish=None,
-    ):
-        infos = [
-            l_type,
-            "input:%s" % self.repr_shape(input_shape),
-            "output:%s" % self.repr_shape(output_shape),
-        ]
-
-        if l_type in ("expanded_conv",):
-            assert None not in (mid, ks, stride, id_skip, se, h_swish)
-            infos += [
-                "expand:%d" % mid,
-                "kernel:%d" % ks,
-                "stride:%d" % stride,
-                "idskip:%d" % id_skip,
-                "se:%d" % se,
-                "hs:%d" % h_swish,
-            ]
-        key = "-".join(infos)
-        return self.lut[key]["mean"]
-
-    def predict_network_latency(self, net, image_size=224):
-        predicted_latency = 0
-        # first conv
-        predicted_latency += self.query(
-            "Conv",
-            [image_size, image_size, 3],
-            [(image_size + 1) // 2, (image_size + 1) // 2, net.first_conv.out_channels],
-        )
-        # blocks
-        fsize = (image_size + 1) // 2
-        for block in net.blocks:
-            mb_conv = block.mobile_inverted_conv
-            shortcut = block.shortcut
-
-            if mb_conv is None:
-                continue
-            if shortcut is None:
-                idskip = 0
-            else:
-                idskip = 1
-            out_fz = int((fsize - 1) / mb_conv.stride + 1)
-            block_latency = self.query(
-                "expanded_conv",
-                [fsize, fsize, mb_conv.in_channels],
-                [out_fz, out_fz, mb_conv.out_channels],
-                mid=mb_conv.depth_conv.conv.in_channels,
-                ks=mb_conv.kernel_size,
-                stride=mb_conv.stride,
-                id_skip=idskip,
-                se=1 if mb_conv.use_se else 0,
-                h_swish=1 if mb_conv.act_func == "h_swish" else 0,
-            )
-            predicted_latency += block_latency
-            fsize = out_fz
-        # final expand layer
-        predicted_latency += self.query(
-            "Conv_1",
-            [fsize, fsize, net.final_expand_layer.in_channels],
-            [fsize, fsize, net.final_expand_layer.out_channels],
-        )
-        # global average pooling
-        predicted_latency += self.query(
-            "AvgPool2D",
-            [fsize, fsize, net.final_expand_layer.out_channels],
-            [1, 1, net.final_expand_layer.out_channels],
-        )
-        # feature mix layer
-        predicted_latency += self.query(
-            "Conv_2",
-            [1, 1, net.feature_mix_layer.in_channels],
-            [1, 1, net.feature_mix_layer.out_channels],
-        )
-        # classifier
-        predicted_latency += self.query(
-            "Logits", [1, 1, net.classifier.in_features], [net.classifier.out_features]
-        )
-        return predicted_latency
-
-    def predict_network_latency_given_spec(self, spec):
-        image_size = spec["r"]
-        predicted_latency = 0
-        # first conv
-        predicted_latency += self.query(
-            "Conv",
-            [image_size, image_size, 3],
-            [(image_size + 1) // 2, (image_size + 1) // 2, 24],
-        )
-        # blocks
-        fsize = (image_size + 1) // 2
-        # first block
-        predicted_latency += self.query(
-            "expanded_conv",
-            [fsize, fsize, 24],
-            [fsize, fsize, 24],
-            mid=24,
-            ks=3,
-            stride=1,
-            id_skip=1,
-            se=0,
-            h_swish=0,
-        )
-        in_channel = 24
-        stride_stages = [2, 2, 2, 1, 2]
-        width_stages = [32, 48, 96, 136, 192]
-        act_stages = ["relu", "relu", "h_swish", "h_swish", "h_swish"]
-        se_stages = [False, True, False, True, True]
-        for i in range(20):
-            stage = i // 4
-            depth_max = spec["d"][stage]
-            depth = i % 4 + 1
-            if depth > depth_max:
-                continue
-            ks, e = spec["ks"][i], spec["e"][i]
-            if i % 4 == 0:
-                stride = stride_stages[stage]
-                idskip = 0
-            else:
-                stride = 1
-                idskip = 1
-            out_channel = width_stages[stage]
-            out_fz = int((fsize - 1) / stride + 1)
-
-            mid_channel = round(in_channel * e)
-            block_latency = self.query(
-                "expanded_conv",
-                [fsize, fsize, in_channel],
-                [out_fz, out_fz, out_channel],
-                mid=mid_channel,
-                ks=ks,
-                stride=stride,
-                id_skip=idskip,
-                se=1 if se_stages[stage] else 0,
-                h_swish=1 if act_stages[stage] == "h_swish" else 0,
-            )
-            predicted_latency += block_latency
-            fsize = out_fz
-            in_channel = out_channel
-        # final expand layer
-        predicted_latency += self.query(
-            "Conv_1",
-            [fsize, fsize, 192],
-            [fsize, fsize, 1152],
-        )
-        # global average pooling
-        predicted_latency += self.query(
-            "AvgPool2D",
-            [fsize, fsize, 1152],
-            [1, 1, 1152],
-        )
-        # feature mix layer
-        predicted_latency += self.query("Conv_2", [1, 1, 1152], [1, 1, 1536])
-        # classifier
-        predicted_latency += self.query("Logits", [1, 1, 1536], [1000])
-        return predicted_latency
-
-
-class LatencyPredictor:
-    def __init__(self, data_root=get_path("note10"),
-                 resolutions=(160, 176, 192, 208, 224)):
-        self.latency_tables = {}
-        # device = os.path.basename(data_root)
-
-        for image_size in resolutions:
-            self.latency_tables[image_size] = LatencyEstimator(
-                os.path.join(data_root, '{}_lookup_table.yaml'.format(image_size)))
-            # print("Built latency table for image size: %d." % image_size)
-
-    def predict_latency(self, spec: dict):
-        return self.latency_tables[spec["r"]].predict_network_latency_given_spec(
-            spec
-        )
-
-
-class MobileNetV3SearchSpace(SearchSpace):
-
-    def __init__(self,
-                 image_scale=IMAGE_SIZE_LIST,  # (min img size, max img size)
-                 ks_list=KERNEL_SIZE_LIST,  # kernel sizes
-                 depth_list=DEPTH_LIST,  # depth
-                 expand_ratio_list=EXPAND_RATIO_LIST,  # expansion ratio
-                 width_mult=WIDTH_MULT,  # width multiplier
-                 **kwargs):
-
-        super().__init__(**kwargs)
-
-        self.image_scale_list = list(image_scale)
-        self.ks_list = list(ks_list)
-        self.depth_list = list(depth_list)
-        self.expand_ratio_list = list(expand_ratio_list)
-        self.width_mult = width_mult
-
-        # upper and lower bound on the decision variables
-        self.n_var = 21
-        # [image resolution, layer 1, layer 2, ..., layer 20]
-        # image resolution ~ [128, 136, 144, ..., 224]
-        # the last two layers in each stage can be skipped
-        self.lb = [0] + [1, 1, 0, 0] + [1, 1, 0, 0] + [1, 1, 0, 0] + [1, 1, 0, 0] + [1, 1, 0, 0]
-        self.ub = [len(self.image_scale_list) - 1]
-
-        if max(depth_list) == 4:
-            self.ub += [int(len(ks_list) * len(expand_ratio_list))] * 20
-        elif max(depth_list) == 3:
-            self.ub += ([int(len(ks_list) * len(expand_ratio_list))] * 3 + [0]) * 5
-        elif max(depth_list) == 2:
-            self.ub += ([int(len(ks_list) * len(expand_ratio_list))] * 2 + [0, 0]) * 5
-        else:
-            ValueError("max depth has to be greater than 2")
-
-        # create the categories for each variable
-        self.categories = [list(range(a, b + 1)) for a, b in zip(self.lb, self.ub)]
-
-        # assuming maximum 4 layers per stage for 5 stages
-        self.stage_layer_indices = [list(range(1, self.n_var))[i:i + 4]
-                                    for i in range(0, 20, 4)]
-
-        # create the mappings between decision variables (genotype) and subnet architectural string (phenotype)
-        self.str2var_mapping = OrderedDict()
-        self.var2str_mapping = OrderedDict()
-        self.str2var_mapping['skip'] = 0
-        increment = 1
-        for e in self.expand_ratio_list:
-            for ks in self.ks_list:
-                self.str2var_mapping['ks@{}_e@{}'.format(ks, e)] = increment
-                self.var2str_mapping[increment] = (ks, e)
-                increment += 1
-
-    @property
-    def name(self):
-        return 'MobileNetV3SearchSpace'
-
-    def str2var(self, ks, e):
-        return self.str2var_mapping['ks@{}_e@{}'.format(ks, e)]
-
-    def var2str(self, v, ub):
-        if v > 0:
-            return self.var2str_mapping[v]
-        else:
-            return self.var2str_mapping[random.randint(1, max(ub, 1))]
-
-    def _sample(self, phenotype=True):
-
-        # uniform random sampling
-        x = [random.choice(options) for options in self.categories]
-
-        x = np.array(x).astype(int)
-
-        # repair, in case of skipping the third but not the fourth layer in a stage
-        for indices in self.stage_layer_indices:
-            if x[indices[-2]] == 0 and x[indices[-1]] > 0:
-                x[indices[-2]] = x[indices[-1]]
-                x[indices[-1]] = 0
-
-        if phenotype:
-            return self._decode(x)
-        else:
-            return x
-
-    def _encode(self, arch):
-        # a sample subnet string
-        # {'r' : 224,
-        #  'ks': [7, 7, 7, 7, 7, 3, 5, 3, 3, 5, 7, 3, 5, 5, 3, 3, 3, 3, 3, 5],
-        #  'e' : [4, 6, 4, 6, 6, 6, 6, 6, 3, 4, 4, 4, 6, 4, 4, 3, 3, 6, 3, 4],
-        #  'd' : [2, 2, 3, 4, 2]}
-
-        x = [0] * self.n_var
-        x[0] = np.where(arch['r'] == np.array(self.image_scale_list))[0][0]
-
-        for indices, d in zip(self.stage_layer_indices, arch['d']):
-            for i in range(d):
-                idx = indices[i]
-                x[idx] = self.str2var(arch['ks'][idx - 1], arch['e'][idx - 1])
-        return x
-
-    def _decode(self, x):
-        # a sample decision variable vector x corresponding to the above subnet string
-        # [(image scale) 4,
-        #  (layers)      8, 9, 5, 5, 6, 2, 3, 6, 6, 1, 4, 0, 1, 2, 2, 3, 9, 5, 8, 1]
-
-        ks_list, expand_ratio_list, depth_list = [], [], []
-        for indices in self.stage_layer_indices:
-            d = len(indices)
-            for idx in indices:
-                ks, e = self.var2str(x[idx], self.ub[idx])
-                ks_list.append(ks)
-                expand_ratio_list.append(e)
-                if x[idx] < 1:
-                    d -= 1
-            depth_list.append(d)
-
-        return {
-            'r': self.image_scale_list[x[0]],
-            'ks': ks_list, 'e': expand_ratio_list, 'd': depth_list}
-
-    def visualize(self, arch):
-        raise NotImplementedError
-
-
-class MobileNetV3Evaluator(Evaluator):
-    def __init__(self,
-                 valid_acc_model_path=get_path("valid_acc_predictor_checkpoint.json"),
-                 # MNV3 validation acc predictor path
-                 test_acc_model_path=get_path("test_acc_predictor_checkpoint.json"),
-                 # MNV3 test acc predictor path
-                 params_model_path=get_path("params_model.json"),
-                 # path to pretrained Params predictor surrogate model / look-up table
-                 flops_model_path=get_path("flops_model.json"),
-                 # path to pretrained FLOPs predictor surrogate model / look-up table
-                 latency_model_path=get_path("note10"),
-                 # path to pretrained latency predictor surrogate model / look-up table
-                 objs='err&flops&latency',  # objectives to be minimized
-                 ):
-        super().__init__(objs)
-
-        self.feature_encoder = MobileNetV3FeatureEncoder()
-        self.valid_acc_predictor = MLPPredictor(pretrained=valid_acc_model_path)
-        self.test_acc_predictor = MLPPredictor(pretrained=test_acc_model_path)
-
-        self.params_predictor = ParamsPredictor(params_model_path)
-        self.flops_predictor = FLOPsPredictor(flops_model_path)
-        self.latency_predictor = LatencyPredictor(latency_model_path)
-
-    @property
-    def name(self):
-        return 'MobileNetV3Evaluator'
-
-    def evaluate(self, archs, objs=None,
-                 true_eval=False  # query the true (mean over three runs) performance
-                 ):
-
-        if objs is None:
-            objs = self.objs
-
-        features = np.array([self.feature_encoder.arch2feature(arch) for arch in archs])
-
-        batch_stats = []
-
-        if true_eval:
-            top1_accs = self.test_acc_predictor.predict(features)
-        else:
-            top1_accs = self.valid_acc_predictor.predict(features, is_noisy=True)
-
-        for i, (arch, top1) in enumerate(zip(archs, top1_accs)):
-            stats = OrderedDict()
-
-            # todo: add stochastic evaluation method
-            if 'err' in objs:
-                stats['err'] = 1 - top1[0]
-
-            if 'params' in objs:
-                stats['params'] = self.params_predictor.predict_params(arch)
-
-            if 'flops' in objs:
-                stats['flops'] = self.flops_predictor.predict_flops(arch)
-
-            if 'latency' in objs:
-                stats['latency'] = self.latency_predictor.predict_latency(arch)  # in ms
-
-            batch_stats.append(stats)
-        return batch_stats
-
-
-class MobileNetV3Benchmark(Benchmark):
-    def __init__(self,
-                 valid_acc_model_path=get_path("valid_acc_predictor_checkpoint.json"),
-                 # MNV3 validation acc predictor path
-                 test_acc_model_path=get_path("test_acc_predictor_checkpoint.json"),
-                 # MNV3 test acc predictor path
-                 params_model_path=get_path("params_model.json"),
-                 # path to pretrained Params predictor surrogate model / look-up table
-                 flops_model_path=get_path("flops_model.json"),
-                 # path to pretrained FLOPs predictor surrogate model / look-up table
-                 latency_model_path=get_path("note10"),
-                 # path to pretrained latency predictor surrogate model / look-up table
-                 objs='err&flops&latency',  # objectives to be minimized
-                 normalized_objectives=False,  # whether to normalize the objectives
-                 ):
-        search_space = MobileNetV3SearchSpace()
-        evaluator = MobileNetV3Evaluator(valid_acc_model_path, test_acc_model_path,
-                                         params_model_path, flops_model_path, latency_model_path, objs)
-        super().__init__(search_space, evaluator, normalized_objectives)
-
-    @property
-    def name(self):
-        return 'MobileNetV3Benchmark'
-
-    @property
-    def _utopian_point(self):
-        """ estimated from sampled architectures, use w/ caution """
-        return {
-            'err&params': [2.091800e-01, 4.610136e+06],
-            'err&flops': [2.09180000e-01, 2.13223824e+08],
-            'err&latency': [0.20918, 10.35887161],
-            'err&params&flops': [2.09180000e-01, 4.61013600e+06, 2.13223824e+08],
-            'err&params&latency': [2.09180000e-01, 4.61013600e+06, 1.03588716e+01],
-            'err&flops&latency': [2.09180000e-01, 2.13223824e+08, 1.03588716e+01],
-            'err&params&flops&latency': [2.09180000e-01, 4.61013600e+06, 2.13223824e+08, 1.03588716e+01],
-        }[self.evaluator.objs]
-
-    @property
-    def _nadir_point(self):
-        """ estimated from sampled architectures, use w/ caution """
-        return {
-            'err&params': [2.9796000e-01, 1.0197992e+07],
-            'err&flops': [2.97960000e-01, 1.37679763e+09],
-            'err&latency': [0.29796, 70.38058926],
-            'err&params&flops': [2.97960000e-01, 1.01979920e+07, 1.37679763e+09],
-            'err&params&latency': [2.97960000e-01, 1.01979920e+07, 7.03805893e+01],
-            'err&flops&latency': [2.97960000e-01, 1.37679763e+09, 7.03805893e+01],
-            'err&params&flops&latency': [2.97960000e-01, 1.01979920e+07, 1.37679763e+09, 7.03805893e+01],
-        }[self.evaluator.objs]
-
-    def debug(self):
-        archs = self.search_space.sample(10)
-        X = self.search_space.encode(archs)
-        F = self.evaluate(X, true_eval=True)
-        hv = self.calc_perf_indicator(X, 'hv')
-
-        print(archs)
-        print(X)
-        print(F)
-        print(hv)
-
-
-if __name__ == '__main__':
-    benchmark = MobileNetV3Benchmark(
-        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/mnv3/valid_acc_predictor_checkpoint.json",
-        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/mnv3/test_acc_predictor_checkpoint.json",
-        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/mnv3/params_model.json",
-        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/mnv3/flops_model.json",
-        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/mnv3/note10",
-        objs='err&params&flops&latency', normalized_objectives=False,
-    )
-
-    # print(benchmark.search_space.n_var)
-    # exit()
-
-    benchmark.debug()
+import os
+import copy
+from pathlib import Path
+
+import yaml
+import json
+import random
+import numpy as np
+from collections import OrderedDict
+
+from evoxbench.modules import SearchSpace, Evaluator, Benchmark, MLPPredictor
+
+__all__ = ['MobileNetV3SearchSpace', 'MobileNetV3Evaluator', 'MobileNetV3Benchmark']
+
+IMAGE_SIZE_LIST = (160, 176, 192, 208, 224)
+KERNEL_SIZE_LIST = (3, 5, 7)
+DEPTH_LIST = (2, 3, 4)
+EXPAND_RATIO_LIST = (3, 4, 6)
+WIDTH_MULT = 1.2
+
+
+def get_path(name):
+    return str(Path(os.environ.get("EVOXBENCH_MODEL", os.getcwd())) / "mnv3" / name)
+
+
+# ------------------- Following functions are specific to MobileNetV3 search space ------------------- #
+class MobileNetV3FeatureEncoder(object):
+    def __init__(self):
+
+        self.ks_map = self.construct_maps(keys=KERNEL_SIZE_LIST)
+        self.ex_map = self.construct_maps(keys=EXPAND_RATIO_LIST)
+        self.dp_map = self.construct_maps(keys=DEPTH_LIST)
+
+    # Helper for constructing the one-hot vectors.
+    @staticmethod
+    def construct_maps(keys):
+        d = dict()
+        keys = list(set(keys))
+        for k in keys:
+            if k not in d:
+                d[k] = len(list(d.keys()))
+        return d
+
+    def arch2feature(self, arch):
+        # This function converts a network config to a feature vector (128-D).
+        ks_list = copy.deepcopy(arch["ks"])
+        ex_list = copy.deepcopy(arch["e"])
+        d_list = copy.deepcopy(arch["d"])
+        r = copy.deepcopy(arch["r"])
+
+        start = 0
+        end = 4
+        for d in d_list:
+            for j in range(start + d, end):
+                ks_list[j] = 0
+                ex_list[j] = 0
+            start += 4
+            end += 4
+
+        # convert to onehot
+        ks_onehot = [0 for _ in range(60)]
+        ex_onehot = [0 for _ in range(60)]
+        r_onehot = [0 for _ in range(8)]
+
+        for i in range(20):
+            start = i * 3
+            if ks_list[i] != 0:
+                ks_onehot[start + self.ks_map[ks_list[i]]] = 1
+            if ex_list[i] != 0:
+                ex_onehot[start + self.ex_map[ex_list[i]]] = 1
+
+        r_onehot[(r - 112) // 16] = 1
+        return ks_onehot + ex_onehot + r_onehot
+
+
+class FLOPsPredictor:
+    channel_list = [24, 32, 48, 96, 136, 192]  # WIDTH_MULT = 1.2
+    stride_stages = [2, 2, 2, 1, 2]
+    act_stages = ["relu", "relu", "h_swish", "h_swish", "h_swish"]
+    se_stages = ['false', 'true', 'false', 'true', 'true']
+
+    def __init__(self,
+                 data_file_path=get_path("flops_model.json")):
+        with open(data_file_path, 'r') as f:
+            self.flops_dict = json.load(f)
+
+    def predict_flops(self, sample):
+        input_size = sample.get("r", 224)
+        flops_dict = self.flops_dict[str(input_size)]
+        assert "ks" in sample and "e" in sample and "d" in sample
+        assert len(sample["ks"]) == len(sample["e"]) and len(sample["ks"]) == 20
+        assert len(sample["d"]) == 5
+
+        flops = 0
+        # calculate the dynamic blocks
+        size = input_size // 2
+        for block_id in range(5):
+            for i in range(sample['d'][block_id]):
+                idx = block_id * 4 + i
+                out_channel = self.channel_list[block_id + 1]
+                k = sample['ks'][idx]
+                e = sample['e'][idx]
+                if i == 0:
+                    s = self.stride_stages[block_id]
+                    in_channel = self.channel_list[block_id]
+                else:
+                    s = 1
+                    in_channel = self.channel_list[block_id + 1]
+                act = self.act_stages[block_id]
+                se = self.se_stages[block_id]
+
+                in_channel = str(in_channel)
+                out_channel = str(out_channel)
+                k = str(k)
+                e = str(e)
+                s = str(s)
+                size_str = str(size)
+                # print(in_channel,out_channel,size, k,e,s,act,se)
+                flops = flops + flops_dict['MBConvLayerBlock'][in_channel][out_channel][size_str][k][e][s][act][se]
+                if s == "2":  # stride = 2 means half the HW
+                    size = (size + 1) // 2
+
+        flops += flops_dict["FirstBlockLayer"]
+        flops += flops_dict["LastLayers"]
+        return flops
+
+
+class ParamsPredictor:
+    channel_list = [24, 32, 48, 96, 136, 192]  # WIDTH_MULT = 1.2
+    stride_stages = [2, 2, 2, 1, 2]
+    act_stages = ["relu", "relu", "h_swish", "h_swish", "h_swish"]
+    se_stages = ['false', 'true', 'false', 'true', 'true']
+
+    def __init__(self,
+                 data_file_path=get_path("params_model.json")):
+        with open(data_file_path, 'r') as f:
+            self.params_dict = json.load(f)
+
+    def predict_params(self, sample):
+        assert "ks" in sample and "e" in sample and "d" in sample
+        assert len(sample["ks"]) == len(sample["e"]) and len(sample["ks"]) == 20
+        assert len(sample["d"]) == 5
+
+        params = 0
+        # calculate the dynamic layers
+
+        for block_id in range(5):
+            for i in range(sample['d'][block_id]):
+                idx = block_id * 4 + i
+                # print(idx)
+                out_channel = self.channel_list[block_id + 1]
+                k = sample['ks'][idx]
+                e = sample['e'][idx]
+                if i == 0:
+                    s = self.stride_stages[block_id]
+                    in_channel = self.channel_list[block_id]
+                else:
+                    s = 1
+                    in_channel = self.channel_list[block_id + 1]
+                act = self.act_stages[block_id]
+                se = self.se_stages[block_id]
+                in_channel = str(in_channel)
+                out_channel = str(out_channel)
+                k = str(k)
+                e = str(e)
+                s = str(s)
+                # print(in_channel, out_channel, k, e, s, act, se)
+                params = params + self.params_dict['MBConvLayer'][in_channel][out_channel][k][e][s][act][se]
+        params = params + self.params_dict['OtherLayer']
+
+        return params
+
+
+class LatencyEstimator(object):
+    def __init__(self, yaml_file_path=''):
+
+        with open(yaml_file_path, "r") as fp:
+            self.lut = yaml.load(fp, Loader=yaml.FullLoader)
+
+    @staticmethod
+    def repr_shape(shape):
+        if isinstance(shape, (list, tuple)):
+            return "x".join(str(_) for _ in shape)
+        elif isinstance(shape, str):
+            return shape
+        else:
+            return TypeError
+
+    def query(
+            self,
+            l_type: str,
+            input_shape,
+            output_shape,
+            mid=None,
+            ks=None,
+            stride=None,
+            id_skip=None,
+            se=None,
+            h_swish=None,
+    ):
+        infos = [
+            l_type,
+            "input:%s" % self.repr_shape(input_shape),
+            "output:%s" % self.repr_shape(output_shape),
+        ]
+
+        if l_type in ("expanded_conv",):
+            assert None not in (mid, ks, stride, id_skip, se, h_swish)
+            infos += [
+                "expand:%d" % mid,
+                "kernel:%d" % ks,
+                "stride:%d" % stride,
+                "idskip:%d" % id_skip,
+                "se:%d" % se,
+                "hs:%d" % h_swish,
+            ]
+        key = "-".join(infos)
+        return self.lut[key]["mean"]
+
+    def predict_network_latency(self, net, image_size=224):
+        predicted_latency = 0
+        # first conv
+        predicted_latency += self.query(
+            "Conv",
+            [image_size, image_size, 3],
+            [(image_size + 1) // 2, (image_size + 1) // 2, net.first_conv.out_channels],
+        )
+        # blocks
+        fsize = (image_size + 1) // 2
+        for block in net.blocks:
+            mb_conv = block.mobile_inverted_conv
+            shortcut = block.shortcut
+
+            if mb_conv is None:
+                continue
+            if shortcut is None:
+                idskip = 0
+            else:
+                idskip = 1
+            out_fz = int((fsize - 1) / mb_conv.stride + 1)
+            block_latency = self.query(
+                "expanded_conv",
+                [fsize, fsize, mb_conv.in_channels],
+                [out_fz, out_fz, mb_conv.out_channels],
+                mid=mb_conv.depth_conv.conv.in_channels,
+                ks=mb_conv.kernel_size,
+                stride=mb_conv.stride,
+                id_skip=idskip,
+                se=1 if mb_conv.use_se else 0,
+                h_swish=1 if mb_conv.act_func == "h_swish" else 0,
+            )
+            predicted_latency += block_latency
+            fsize = out_fz
+        # final expand layer
+        predicted_latency += self.query(
+            "Conv_1",
+            [fsize, fsize, net.final_expand_layer.in_channels],
+            [fsize, fsize, net.final_expand_layer.out_channels],
+        )
+        # global average pooling
+        predicted_latency += self.query(
+            "AvgPool2D",
+            [fsize, fsize, net.final_expand_layer.out_channels],
+            [1, 1, net.final_expand_layer.out_channels],
+        )
+        # feature mix layer
+        predicted_latency += self.query(
+            "Conv_2",
+            [1, 1, net.feature_mix_layer.in_channels],
+            [1, 1, net.feature_mix_layer.out_channels],
+        )
+        # classifier
+        predicted_latency += self.query(
+            "Logits", [1, 1, net.classifier.in_features], [net.classifier.out_features]
+        )
+        return predicted_latency
+
+    def predict_network_latency_given_spec(self, spec):
+        image_size = spec["r"]
+        predicted_latency = 0
+        # first conv
+        predicted_latency += self.query(
+            "Conv",
+            [image_size, image_size, 3],
+            [(image_size + 1) // 2, (image_size + 1) // 2, 24],
+        )
+        # blocks
+        fsize = (image_size + 1) // 2
+        # first block
+        predicted_latency += self.query(
+            "expanded_conv",
+            [fsize, fsize, 24],
+            [fsize, fsize, 24],
+            mid=24,
+            ks=3,
+            stride=1,
+            id_skip=1,
+            se=0,
+            h_swish=0,
+        )
+        in_channel = 24
+        stride_stages = [2, 2, 2, 1, 2]
+        width_stages = [32, 48, 96, 136, 192]
+        act_stages = ["relu", "relu", "h_swish", "h_swish", "h_swish"]
+        se_stages = [False, True, False, True, True]
+        for i in range(20):
+            stage = i // 4
+            depth_max = spec["d"][stage]
+            depth = i % 4 + 1
+            if depth > depth_max:
+                continue
+            ks, e = spec["ks"][i], spec["e"][i]
+            if i % 4 == 0:
+                stride = stride_stages[stage]
+                idskip = 0
+            else:
+                stride = 1
+                idskip = 1
+            out_channel = width_stages[stage]
+            out_fz = int((fsize - 1) / stride + 1)
+
+            mid_channel = round(in_channel * e)
+            block_latency = self.query(
+                "expanded_conv",
+                [fsize, fsize, in_channel],
+                [out_fz, out_fz, out_channel],
+                mid=mid_channel,
+                ks=ks,
+                stride=stride,
+                id_skip=idskip,
+                se=1 if se_stages[stage] else 0,
+                h_swish=1 if act_stages[stage] == "h_swish" else 0,
+            )
+            predicted_latency += block_latency
+            fsize = out_fz
+            in_channel = out_channel
+        # final expand layer
+        predicted_latency += self.query(
+            "Conv_1",
+            [fsize, fsize, 192],
+            [fsize, fsize, 1152],
+        )
+        # global average pooling
+        predicted_latency += self.query(
+            "AvgPool2D",
+            [fsize, fsize, 1152],
+            [1, 1, 1152],
+        )
+        # feature mix layer
+        predicted_latency += self.query("Conv_2", [1, 1, 1152], [1, 1, 1536])
+        # classifier
+        predicted_latency += self.query("Logits", [1, 1, 1536], [1000])
+        return predicted_latency
+
+
+class LatencyPredictor:
+    def __init__(self, data_root=get_path("note10"),
+                 resolutions=(160, 176, 192, 208, 224)):
+        self.latency_tables = {}
+        # device = os.path.basename(data_root)
+
+        for image_size in resolutions:
+            self.latency_tables[image_size] = LatencyEstimator(
+                os.path.join(data_root, '{}_lookup_table.yaml'.format(image_size)))
+            # print("Built latency table for image size: %d." % image_size)
+
+    def predict_latency(self, spec: dict):
+        return self.latency_tables[spec["r"]].predict_network_latency_given_spec(
+            spec
+        )
+
+
+class MobileNetV3SearchSpace(SearchSpace):
+
+    def __init__(self,
+                 image_scale=IMAGE_SIZE_LIST,  # (min img size, max img size)
+                 ks_list=KERNEL_SIZE_LIST,  # kernel sizes
+                 depth_list=DEPTH_LIST,  # depth
+                 expand_ratio_list=EXPAND_RATIO_LIST,  # expansion ratio
+                 width_mult=WIDTH_MULT,  # width multiplier
+                 **kwargs):
+
+        super().__init__(**kwargs)
+
+        self.image_scale_list = list(image_scale)
+        self.ks_list = list(ks_list)
+        self.depth_list = list(depth_list)
+        self.expand_ratio_list = list(expand_ratio_list)
+        self.width_mult = width_mult
+
+        # upper and lower bound on the decision variables
+        self.n_var = 21
+        # [image resolution, layer 1, layer 2, ..., layer 20]
+        # image resolution ~ [128, 136, 144, ..., 224]
+        # the last two layers in each stage can be skipped
+        self.lb = [0] + [1, 1, 0, 0] + [1, 1, 0, 0] + [1, 1, 0, 0] + [1, 1, 0, 0] + [1, 1, 0, 0]
+        self.ub = [len(self.image_scale_list) - 1]
+
+        if max(depth_list) == 4:
+            self.ub += [int(len(ks_list) * len(expand_ratio_list))] * 20
+        elif max(depth_list) == 3:
+            self.ub += ([int(len(ks_list) * len(expand_ratio_list))] * 3 + [0]) * 5
+        elif max(depth_list) == 2:
+            self.ub += ([int(len(ks_list) * len(expand_ratio_list))] * 2 + [0, 0]) * 5
+        else:
+            ValueError("max depth has to be greater than 2")
+
+        # create the categories for each variable
+        self.categories = [list(range(a, b + 1)) for a, b in zip(self.lb, self.ub)]
+
+        # assuming maximum 4 layers per stage for 5 stages
+        self.stage_layer_indices = [list(range(1, self.n_var))[i:i + 4]
+                                    for i in range(0, 20, 4)]
+
+        # create the mappings between decision variables (genotype) and subnet architectural string (phenotype)
+        self.str2var_mapping = OrderedDict()
+        self.var2str_mapping = OrderedDict()
+        self.str2var_mapping['skip'] = 0
+        increment = 1
+        for e in self.expand_ratio_list:
+            for ks in self.ks_list:
+                self.str2var_mapping['ks@{}_e@{}'.format(ks, e)] = increment
+                self.var2str_mapping[increment] = (ks, e)
+                increment += 1
+
+    @property
+    def name(self):
+        return 'MobileNetV3SearchSpace'
+
+    def str2var(self, ks, e):
+        return self.str2var_mapping['ks@{}_e@{}'.format(ks, e)]
+
+    def var2str(self, v, ub):
+        if v > 0:
+            return self.var2str_mapping[v]
+        else:
+            return self.var2str_mapping[random.randint(1, max(ub, 1))]
+
+    def _sample(self, phenotype=True):
+
+        # uniform random sampling
+        x = [random.choice(options) for options in self.categories]
+
+        x = np.array(x).astype(int)
+
+        # repair, in case of skipping the third but not the fourth layer in a stage
+        for indices in self.stage_layer_indices:
+            if x[indices[-2]] == 0 and x[indices[-1]] > 0:
+                x[indices[-2]] = x[indices[-1]]
+                x[indices[-1]] = 0
+
+        if phenotype:
+            return self._decode(x)
+        else:
+            return x
+
+    def _encode(self, arch):
+        # a sample subnet string
+        # {'r' : 224,
+        #  'ks': [7, 7, 7, 7, 7, 3, 5, 3, 3, 5, 7, 3, 5, 5, 3, 3, 3, 3, 3, 5],
+        #  'e' : [4, 6, 4, 6, 6, 6, 6, 6, 3, 4, 4, 4, 6, 4, 4, 3, 3, 6, 3, 4],
+        #  'd' : [2, 2, 3, 4, 2]}
+
+        x = [0] * self.n_var
+        x[0] = np.where(arch['r'] == np.array(self.image_scale_list))[0][0]
+
+        for indices, d in zip(self.stage_layer_indices, arch['d']):
+            for i in range(d):
+                idx = indices[i]
+                x[idx] = self.str2var(arch['ks'][idx - 1], arch['e'][idx - 1])
+        return x
+
+    def _decode(self, x):
+        # a sample decision variable vector x corresponding to the above subnet string
+        # [(image scale) 4,
+        #  (layers)      8, 9, 5, 5, 6, 2, 3, 6, 6, 1, 4, 0, 1, 2, 2, 3, 9, 5, 8, 1]
+
+        ks_list, expand_ratio_list, depth_list = [], [], []
+        for indices in self.stage_layer_indices:
+            d = len(indices)
+            for idx in indices:
+                ks, e = self.var2str(x[idx], self.ub[idx])
+                ks_list.append(ks)
+                expand_ratio_list.append(e)
+                if x[idx] < 1:
+                    d -= 1
+            depth_list.append(d)
+
+        return {
+            'r': self.image_scale_list[x[0]],
+            'ks': ks_list, 'e': expand_ratio_list, 'd': depth_list}
+
+    def visualize(self, arch):
+        raise NotImplementedError
+
+
+class MobileNetV3Evaluator(Evaluator):
+    def __init__(self,
+                 valid_acc_model_path=get_path("valid_acc_predictor_checkpoint.json"),
+                 # MNV3 validation acc predictor path
+                 test_acc_model_path=get_path("test_acc_predictor_checkpoint.json"),
+                 # MNV3 test acc predictor path
+                 params_model_path=get_path("params_model.json"),
+                 # path to pretrained Params predictor surrogate model / look-up table
+                 flops_model_path=get_path("flops_model.json"),
+                 # path to pretrained FLOPs predictor surrogate model / look-up table
+                 latency_model_path=get_path("note10"),
+                 # path to pretrained latency predictor surrogate model / look-up table
+                 objs='err&flops&latency',  # objectives to be minimized
+                 ):
+        super().__init__(objs)
+
+        self.feature_encoder = MobileNetV3FeatureEncoder()
+        self.valid_acc_predictor = MLPPredictor(pretrained=valid_acc_model_path)
+        self.test_acc_predictor = MLPPredictor(pretrained=test_acc_model_path)
+
+        self.params_predictor = ParamsPredictor(params_model_path)
+        self.flops_predictor = FLOPsPredictor(flops_model_path)
+        self.latency_predictor = LatencyPredictor(latency_model_path)
+
+    @property
+    def name(self):
+        return 'MobileNetV3Evaluator'
+
+    def evaluate(self, archs, objs=None,
+                 true_eval=False  # query the true (mean over three runs) performance
+                 ):
+
+        if objs is None:
+            objs = self.objs
+
+        features = np.array([self.feature_encoder.arch2feature(arch) for arch in archs])
+
+        batch_stats = []
+
+        if true_eval:
+            top1_accs = self.test_acc_predictor.predict(features)
+        else:
+            top1_accs = self.valid_acc_predictor.predict(features, is_noisy=True)
+
+        for i, (arch, top1) in enumerate(zip(archs, top1_accs)):
+            stats = OrderedDict()
+
+            # todo: add stochastic evaluation method
+            if 'err' in objs:
+                stats['err'] = 1 - top1[0]
+
+            if 'params' in objs:
+                stats['params'] = self.params_predictor.predict_params(arch)
+
+            if 'flops' in objs:
+                stats['flops'] = self.flops_predictor.predict_flops(arch)
+
+            if 'latency' in objs:
+                stats['latency'] = self.latency_predictor.predict_latency(arch)  # in ms
+
+            batch_stats.append(stats)
+        return batch_stats
+
+
+class MobileNetV3Benchmark(Benchmark):
+    def __init__(self,
+                 valid_acc_model_path=get_path("valid_acc_predictor_checkpoint.json"),
+                 # MNV3 validation acc predictor path
+                 test_acc_model_path=get_path("test_acc_predictor_checkpoint.json"),
+                 # MNV3 test acc predictor path
+                 params_model_path=get_path("params_model.json"),
+                 # path to pretrained Params predictor surrogate model / look-up table
+                 flops_model_path=get_path("flops_model.json"),
+                 # path to pretrained FLOPs predictor surrogate model / look-up table
+                 latency_model_path=get_path("note10"),
+                 # path to pretrained latency predictor surrogate model / look-up table
+                 objs='err&flops&latency',  # objectives to be minimized
+                 normalized_objectives=False,  # whether to normalize the objectives
+                 ):
+        search_space = MobileNetV3SearchSpace()
+        evaluator = MobileNetV3Evaluator(valid_acc_model_path, test_acc_model_path,
+                                         params_model_path, flops_model_path, latency_model_path, objs)
+        super().__init__(search_space, evaluator, normalized_objectives)
+
+    @property
+    def name(self):
+        return 'MobileNetV3Benchmark'
+
+    @property
+    def _utopian_point(self):
+        """ estimated from sampled architectures, use w/ caution """
+        return {
+            'err&params': [2.091800e-01, 4.610136e+06],
+            'err&flops': [2.09180000e-01, 2.13223824e+08],
+            'err&latency': [0.20918, 10.35887161],
+            'err&params&flops': [2.09180000e-01, 4.61013600e+06, 2.13223824e+08],
+            'err&params&latency': [2.09180000e-01, 4.61013600e+06, 1.03588716e+01],
+            'err&flops&latency': [2.09180000e-01, 2.13223824e+08, 1.03588716e+01],
+            'err&params&flops&latency': [2.09180000e-01, 4.61013600e+06, 2.13223824e+08, 1.03588716e+01],
+        }[self.evaluator.objs]
+
+    @property
+    def _nadir_point(self):
+        """ estimated from sampled architectures, use w/ caution """
+        return {
+            'err&params': [2.9796000e-01, 1.0197992e+07],
+            'err&flops': [2.97960000e-01, 1.37679763e+09],
+            'err&latency': [0.29796, 70.38058926],
+            'err&params&flops': [2.97960000e-01, 1.01979920e+07, 1.37679763e+09],
+            'err&params&latency': [2.97960000e-01, 1.01979920e+07, 7.03805893e+01],
+            'err&flops&latency': [2.97960000e-01, 1.37679763e+09, 7.03805893e+01],
+            'err&params&flops&latency': [2.97960000e-01, 1.01979920e+07, 1.37679763e+09, 7.03805893e+01],
+        }[self.evaluator.objs]
+
+    def debug(self):
+        archs = self.search_space.sample(10)
+        X = self.search_space.encode(archs)
+        F = self.evaluate(X, true_eval=True)
+        hv = self.calc_perf_indicator(X, 'hv')
+
+        print(archs)
+        print(X)
+        print(F)
+        print(hv)
+
+
+if __name__ == '__main__':
+    benchmark = MobileNetV3Benchmark(
+        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/mnv3/valid_acc_predictor_checkpoint.json",
+        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/mnv3/test_acc_predictor_checkpoint.json",
+        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/mnv3/params_model.json",
+        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/mnv3/flops_model.json",
+        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/mnv3/note10",
+        objs='err&params&flops&latency', normalized_objectives=False,
+    )
+
+    # print(benchmark.search_space.n_var)
+    # exit()
+
+    benchmark.debug()
```

### Comparing `evoxbench-1.0.2/evoxbench/benchmarks/nb201.py` & `evoxbench-1.0.3/evoxbench/benchmarks/nb201.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,237 +1,237 @@
-import json
-import os
-from pathlib import Path
-
-import numpy as np
-from typing import List
-from numpy import ndarray
-from collections import OrderedDict
-
-from evoxbench.modules import SearchSpace, Evaluator, Benchmark
-from nasbench201.models import NASBench201Result  # has to be imported after the init method
-
-__all__ = ['NASBench201SearchSpace', 'NASBench201Evaluator', 'NASBench201Benchmark']
-
-
-def get_path(name):
-    return str(Path(os.environ.get("EVOXBENCH_MODEL", os.getcwd())) / "nb201" / name)
-
-
-class NASBench201SearchSpace(SearchSpace):
-    """
-        NASBench201 topology search space
-    """
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.num_vertices: int = 4
-        self.edge_spots: int = self.num_vertices * (self.num_vertices - 1) // 2
-
-        # the operation must be none rather than zeroize
-        self.allowed_ops: List[str] = ['none', 'skip_connect', 'nor_conv_1x1', 'nor_conv_3x3', 'avg_pool_3x3']
-
-        # upper and lower bound on the decision variables
-        self.n_var = self.edge_spots
-        self.lb = [0] * self.n_var
-        self.ub = [4] * self.n_var
-
-        # create the categories for each variable
-        self.categories = [list(range(a, b + 1)) for a, b in zip(self.lb, self.ub)]
-
-    @property
-    def name(self):
-        return 'NASBench201SearchSpace'
-
-    def _sample(self):
-        x = np.random.choice(len(self.allowed_ops), self.edge_spots)
-        return self._decode(x)
-
-    def _encode(self, arch: str):
-        # encode architecture phenotype to genotype
-        # a sample architecture
-        # '|none~0|+|avg_pool_3x3~0|nor_conv_3x3~1|+|nor_conv_1x1~0|nor_conv_3x3~1|nor_conv_1x1~2|'
-        ops = []
-        for node in arch.split('+'):
-            op = [o.split('~')[0] for o in node.split('|') if o]
-            ops.extend(op)
-        x_ops = np.empty(self.edge_spots, dtype=np.int64)
-        for i, op in enumerate(ops):
-            x_ops[i] = (np.array(self.allowed_ops) == op).nonzero()[0][0]
-        return x_ops
-
-    def _decode(self, x: ndarray) -> str:
-        _x = x.tolist()
-        result, index = [], 0
-        for i in range(1, self.num_vertices):
-            tmp = []
-            for j in range(i):
-                tmp.append(f"{self.allowed_ops[_x[index]]}~{j}")
-                index += 1
-            result.append(f"|{'|'.join(tmp)}|")
-        return '+'.join(result)
-
-    def visualize(self, arch):
-        raise NotImplementedError
-
-
-class NASBench201Evaluator(Evaluator):
-    def __init__(self,
-                 fidelity=200,  # options = [1, 12, 90, 200], i.e. acc measured at different training epochs
-                 # objs='err&params&flops',  # objectives to be minimized
-                 objs='err&params&flops&edgegpu_latency&edgegpu_energy&'
-                      'eyeriss_latency&eyeriss_energy&eyeriss_arithmetic_intensity',  # objectives to be minimized
-                 dataset='cifar10',  # ['cifar10', 'cifar100', 'ImageNet16-120']
-                 # hardware='fpga',  # ['edgegpu', 'raspi4', 'edgetpu', 'pixel3', 'eyeriss', 'fpga']
-                 ):
-        super().__init__(objs)
-        self.engine = NASBench201Result
-        # self.hardware = hardware
-        self.fidelity = str(fidelity)
-        self.dataset = dataset
-
-    @property
-    def name(self):
-        return 'NASBench201Evaluator'
-
-    def evaluate(self, archs, objs=None,
-                 true_eval=False  # query the true (mean over multiple runs) performance
-                 ):
-
-        if objs is None:
-            objs = self.objs
-        objs = set(objs.split('&'))
-        batch_stats = []
-        infos = {result.phenotype: result for result in NASBench201Result.objects.filter(phenotype__in=archs)}
-        for arch in archs:
-            info = infos[arch]
-            stats = OrderedDict()
-            fixed = info.cost12[self.dataset] if self.fidelity == '12' else info.cost200[self.dataset]
-            if true_eval:
-                top1 = np.mean([v['test-accuracy'] for v in
-                                info.more_info[self.dataset]['hp{}'.format(self.fidelity)]])  # mean test accuracy
-            else:
-                computed = [v['valid-accuracy'] for v in info.more_info[
-                    'cifar10-valid' if self.dataset == 'cifar10' else self.dataset][
-                    'hp{}'.format(self.fidelity)]]
-                top1 = np.random.choice(computed)  # randomly chosen from trials
-
-            if 'err' in objs:
-                stats['err'] = 100 - top1
-            if 'params' in objs:
-                stats['params'] = fixed['params']  # in M
-            if 'flops' in objs:
-                stats['flops'] = fixed['flops']  # in M
-
-            # the remaining obj in objs should be latency, energy or arithmetic_intensity
-            for obj in objs:
-                if 'latency' in obj:
-                    hardware = obj.split('_')[0]
-                    assert hardware in ['edgegpu', 'eyeriss', 'fpga'], "the requested hardware do not support latency"
-                    stats[obj] = info.hw_info[self.dataset][obj]
-                if 'energy' in obj:
-                    hardware = obj.split('_')[0]
-                    assert hardware in ['edgegpu', 'eyeriss', 'fpga'], "the requested hardware do not support energy"
-                    stats[obj] = info.hw_info[self.dataset][obj]
-                if 'arithmetic_intensity' in obj:
-                    hardware = obj.split('_')[0]
-                    assert hardware in ['eyeriss'], "only Eyeriss support arithmetic intensity"
-                    stats[obj] = info.hw_info[self.dataset][obj]
-                # ms for latency, mJ for energy, OPs/Byte for arithmetic_intensity
-
-            batch_stats.append(stats)
-
-        return batch_stats
-
-
-class NASBench201Benchmark(Benchmark):
-    def __init__(self,
-                 fidelity=200,  # options = [12, 200], i.e. acc measured at different training epochs
-                 objs='err&params&flops',  # objectives to be minimized
-                 dataset='cifar10',  # ['cifar10', 'cifar100', 'ImageNet16-120']
-                 # hardware='fpga',  # ['edgegpu', 'raspi4', 'edgetpu', 'pixel3', 'eyeriss', 'fpga']
-                 pf_file_path=get_path("nb201_pf.json"),  # path to the Pareto front json file
-                 ps_file_path=get_path("nb201_ps.json"),  # path to the Pareto set json file
-                 normalized_objectives=True,  # whether to normalize the objectives
-                 ):
-        search_space = NASBench201SearchSpace()
-        evaluator = NASBench201Evaluator(fidelity, objs, dataset)
-        super().__init__(search_space, evaluator, normalized_objectives)
-
-        # # process objectives w.r.t hardware
-        # if 'latency' in objs:
-        #     objs = objs.replace('latency', '{}_latency'.format(hardware))
-        #
-        # if 'energy' in objs:
-        #     assert hardware in ['edgegpu', 'eyeriss', 'fpga'], \
-        #         "the requested hardware do not support energy"
-        #     objs = objs.replace('energy', '{}_energy'.format(hardware))
-        #
-        # if 'arithmetic_intensity' in objs:
-        #     assert hardware in ['eyeriss'], \
-        #         "only Eyeriss support arithmetic intensity"
-        #     objs = objs.replace('arithmetic_intensity', '{}_arithmetic_intensity'.format(hardware))
-
-        self.pf = np.array(json.load(open(pf_file_path, 'r'))[objs])
-        self.ps = np.array(json.load(open(ps_file_path, 'r'))[objs])
-
-    @property
-    def name(self):
-        return 'NASBench201Benchmark'
-
-    @property
-    def pareto_front(self):
-        return self.pf
-
-    @property
-    def pareto_set(self):
-        return self.ps
-
-    def debug(self):
-        archs = self.search_space.sample(10)
-        X = self.search_space.encode(archs)
-        F = self.evaluate(X, true_eval=False)
-        print(F)
-
-        igd = self.calc_perf_indicator(X, 'igd')
-        hv = self.calc_perf_indicator(X, 'hv')
-        norm_hv = self.calc_perf_indicator(X, 'normalized_hv')
-
-        # ps_X = self.search_space.encode(self.ps)
-        ps_igd = self.calc_perf_indicator(self.pareto_set, 'igd')
-        ps_hv = self.calc_perf_indicator(self.pareto_set, 'hv')
-        ps_norm_hv = self.calc_perf_indicator(self.pareto_set, 'normalized_hv')
-
-        print(archs)
-        print(X)
-        print(F)
-        print(igd)
-        print(hv)
-        print(norm_hv)
-
-        print("PF IGD: {}, this number should be really close to 0".format(ps_igd))
-        print(ps_hv)
-        print("PF normalized HV: {}, this number should be really close to 1".format(ps_norm_hv))
-
-
-# ------------------------ Following functions are specific to NASBench201 ------------------------- #
-
-
-if __name__ == '__main__':
-    nb201_pf = "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/nb201/nb201_pf.json"
-    nb201_ps = "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/nb201/nb201_ps.json"
-
-    benchmark = NASBench201Benchmark(
-        200, objs='err&params&flops&edgegpu_latency&edgegpu_energy&'
-                  'eyeriss_latency&eyeriss_energy&eyeriss_arithmetic_intensity', dataset='cifar10',
-        # hardware='eyeriss',
-        pf_file_path=nb201_pf, ps_file_path=nb201_ps, normalized_objectives=True)
-
-    # print(benchmark.search_space.n_var)
-    # exit()
-
-    # pf = benchmark.normalize(benchmark.pareto_front)
-    # _pf = benchmark.evaluate(benchmark.search_space.encode(benchmark.pareto_set), true_eval=True)
-    #
-    # print(np.sum(np.abs(pf - _pf)))
-    # exit()
-    benchmark.debug()
+import json
+import os
+from pathlib import Path
+
+import numpy as np
+from typing import List
+from numpy import ndarray
+from collections import OrderedDict
+
+from evoxbench.modules import SearchSpace, Evaluator, Benchmark
+from nasbench201.models import NASBench201Result  # has to be imported after the init method
+
+__all__ = ['NASBench201SearchSpace', 'NASBench201Evaluator', 'NASBench201Benchmark']
+
+
+def get_path(name):
+    return str(Path(os.environ.get("EVOXBENCH_MODEL", os.getcwd())) / "nb201" / name)
+
+
+class NASBench201SearchSpace(SearchSpace):
+    """
+        NASBench201 topology search space
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.num_vertices: int = 4
+        self.edge_spots: int = self.num_vertices * (self.num_vertices - 1) // 2
+
+        # the operation must be none rather than zeroize
+        self.allowed_ops: List[str] = ['none', 'skip_connect', 'nor_conv_1x1', 'nor_conv_3x3', 'avg_pool_3x3']
+
+        # upper and lower bound on the decision variables
+        self.n_var = self.edge_spots
+        self.lb = [0] * self.n_var
+        self.ub = [4] * self.n_var
+
+        # create the categories for each variable
+        self.categories = [list(range(a, b + 1)) for a, b in zip(self.lb, self.ub)]
+
+    @property
+    def name(self):
+        return 'NASBench201SearchSpace'
+
+    def _sample(self):
+        x = np.random.choice(len(self.allowed_ops), self.edge_spots)
+        return self._decode(x)
+
+    def _encode(self, arch: str):
+        # encode architecture phenotype to genotype
+        # a sample architecture
+        # '|none~0|+|avg_pool_3x3~0|nor_conv_3x3~1|+|nor_conv_1x1~0|nor_conv_3x3~1|nor_conv_1x1~2|'
+        ops = []
+        for node in arch.split('+'):
+            op = [o.split('~')[0] for o in node.split('|') if o]
+            ops.extend(op)
+        x_ops = np.empty(self.edge_spots, dtype=np.int64)
+        for i, op in enumerate(ops):
+            x_ops[i] = (np.array(self.allowed_ops) == op).nonzero()[0][0]
+        return x_ops
+
+    def _decode(self, x: ndarray) -> str:
+        _x = x.tolist()
+        result, index = [], 0
+        for i in range(1, self.num_vertices):
+            tmp = []
+            for j in range(i):
+                tmp.append(f"{self.allowed_ops[_x[index]]}~{j}")
+                index += 1
+            result.append(f"|{'|'.join(tmp)}|")
+        return '+'.join(result)
+
+    def visualize(self, arch):
+        raise NotImplementedError
+
+
+class NASBench201Evaluator(Evaluator):
+    def __init__(self,
+                 fidelity=200,  # options = [1, 12, 90, 200], i.e. acc measured at different training epochs
+                 # objs='err&params&flops',  # objectives to be minimized
+                 objs='err&params&flops&edgegpu_latency&edgegpu_energy&'
+                      'eyeriss_latency&eyeriss_energy&eyeriss_arithmetic_intensity',  # objectives to be minimized
+                 dataset='cifar10',  # ['cifar10', 'cifar100', 'ImageNet16-120']
+                 # hardware='fpga',  # ['edgegpu', 'raspi4', 'edgetpu', 'pixel3', 'eyeriss', 'fpga']
+                 ):
+        super().__init__(objs)
+        self.engine = NASBench201Result
+        # self.hardware = hardware
+        self.fidelity = str(fidelity)
+        self.dataset = dataset
+
+    @property
+    def name(self):
+        return 'NASBench201Evaluator'
+
+    def evaluate(self, archs, objs=None,
+                 true_eval=False  # query the true (mean over multiple runs) performance
+                 ):
+
+        if objs is None:
+            objs = self.objs
+        objs = objs.split('&')
+        batch_stats = []
+        infos = {result.phenotype: result for result in NASBench201Result.objects.filter(phenotype__in=archs)}
+        for arch in archs:
+            info = infos[arch]
+            stats = OrderedDict()
+            fixed = info.cost12[self.dataset] if self.fidelity == '12' else info.cost200[self.dataset]
+            if true_eval:
+                top1 = np.mean([v['test-accuracy'] for v in
+                                info.more_info[self.dataset]['hp{}'.format(self.fidelity)]])  # mean test accuracy
+            else:
+                computed = [v['valid-accuracy'] for v in info.more_info[
+                    'cifar10-valid' if self.dataset == 'cifar10' else self.dataset][
+                    'hp{}'.format(self.fidelity)]]
+                top1 = np.random.choice(computed)  # randomly chosen from trials
+
+            if 'err' in objs:
+                stats['err'] = 100 - top1
+            if 'params' in objs:
+                stats['params'] = fixed['params']  # in M
+            if 'flops' in objs:
+                stats['flops'] = fixed['flops']  # in M
+
+            # the remaining obj in objs should be latency, energy or arithmetic_intensity
+            for obj in objs:
+                if 'latency' in obj:
+                    hardware = obj.split('_')[0]
+                    assert hardware in ['edgegpu', 'eyeriss', 'fpga'], "the requested hardware do not support latency"
+                    stats[obj] = info.hw_info[self.dataset][obj]
+                if 'energy' in obj:
+                    hardware = obj.split('_')[0]
+                    assert hardware in ['edgegpu', 'eyeriss', 'fpga'], "the requested hardware do not support energy"
+                    stats[obj] = info.hw_info[self.dataset][obj]
+                if 'arithmetic_intensity' in obj:
+                    hardware = obj.split('_')[0]
+                    assert hardware in ['eyeriss'], "only Eyeriss support arithmetic intensity"
+                    stats[obj] = info.hw_info[self.dataset][obj]
+                # ms for latency, mJ for energy, OPs/Byte for arithmetic_intensity
+
+            batch_stats.append(stats)
+
+        return batch_stats
+
+
+class NASBench201Benchmark(Benchmark):
+    def __init__(self,
+                 fidelity=200,  # options = [12, 200], i.e. acc measured at different training epochs
+                 objs='err&params&flops',  # objectives to be minimized
+                 dataset='cifar10',  # ['cifar10', 'cifar100', 'ImageNet16-120']
+                 # hardware='fpga',  # ['edgegpu', 'raspi4', 'edgetpu', 'pixel3', 'eyeriss', 'fpga']
+                 pf_file_path=get_path("nb201_pf.json"),  # path to the Pareto front json file
+                 ps_file_path=get_path("nb201_ps.json"),  # path to the Pareto set json file
+                 normalized_objectives=True,  # whether to normalize the objectives
+                 ):
+        search_space = NASBench201SearchSpace()
+        evaluator = NASBench201Evaluator(fidelity, objs, dataset)
+        super().__init__(search_space, evaluator, normalized_objectives)
+
+        # # process objectives w.r.t hardware
+        # if 'latency' in objs:
+        #     objs = objs.replace('latency', '{}_latency'.format(hardware))
+        #
+        # if 'energy' in objs:
+        #     assert hardware in ['edgegpu', 'eyeriss', 'fpga'], \
+        #         "the requested hardware do not support energy"
+        #     objs = objs.replace('energy', '{}_energy'.format(hardware))
+        #
+        # if 'arithmetic_intensity' in objs:
+        #     assert hardware in ['eyeriss'], \
+        #         "only Eyeriss support arithmetic intensity"
+        #     objs = objs.replace('arithmetic_intensity', '{}_arithmetic_intensity'.format(hardware))
+
+        self.pf = np.array(json.load(open(pf_file_path, 'r'))[objs])
+        self.ps = np.array(json.load(open(ps_file_path, 'r'))[objs])
+
+    @property
+    def name(self):
+        return 'NASBench201Benchmark'
+
+    @property
+    def pareto_front(self):
+        return self.pf
+
+    @property
+    def pareto_set(self):
+        return self.ps
+
+    def debug(self):
+        archs = self.search_space.sample(10)
+        X = self.search_space.encode(archs)
+        F = self.evaluate(X, true_eval=False)
+        print(F)
+
+        igd = self.calc_perf_indicator(X, 'igd')
+        hv = self.calc_perf_indicator(X, 'hv')
+        norm_hv = self.calc_perf_indicator(X, 'normalized_hv')
+
+        # ps_X = self.search_space.encode(self.ps)
+        ps_igd = self.calc_perf_indicator(self.pareto_set, 'igd')
+        ps_hv = self.calc_perf_indicator(self.pareto_set, 'hv')
+        ps_norm_hv = self.calc_perf_indicator(self.pareto_set, 'normalized_hv')
+
+        print(archs)
+        print(X)
+        print(F)
+        print(igd)
+        print(hv)
+        print(norm_hv)
+
+        print("PF IGD: {}, this number should be really close to 0".format(ps_igd))
+        print(ps_hv)
+        print("PF normalized HV: {}, this number should be really close to 1".format(ps_norm_hv))
+
+
+# ------------------------ Following functions are specific to NASBench201 ------------------------- #
+
+
+if __name__ == '__main__':
+    nb201_pf = "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/nb201/nb201_pf.json"
+    nb201_ps = "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/nb201/nb201_ps.json"
+
+    benchmark = NASBench201Benchmark(
+        200, objs='err&params&flops&edgegpu_latency&edgegpu_energy&'
+                  'eyeriss_latency&eyeriss_energy&eyeriss_arithmetic_intensity', dataset='cifar10',
+        # hardware='eyeriss',
+        pf_file_path=nb201_pf, ps_file_path=nb201_ps, normalized_objectives=True)
+
+    # print(benchmark.search_space.n_var)
+    # exit()
+
+    # pf = benchmark.normalize(benchmark.pareto_front)
+    # _pf = benchmark.evaluate(benchmark.search_space.encode(benchmark.pareto_set), true_eval=True)
+    #
+    # print(np.sum(np.abs(pf - _pf)))
+    # exit()
+    benchmark.debug()
```

### Comparing `evoxbench-1.0.2/evoxbench/benchmarks/resnet.py` & `evoxbench-1.0.3/evoxbench/benchmarks/resnet.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,530 +1,530 @@
-import json
-import copy
-import os
-from pathlib import Path
-from collections import OrderedDict
-
-import numpy as np
-
-from evoxbench.modules import SearchSpace, Evaluator, Benchmark, MLPPredictor
-
-__all__ = ['ResNet50DSearchSpace', 'ResNet50DEvaluator', 'ResNet50DBenchmark']
-
-IMAGE_SIZE_LIST = (128, 144, 160, 176, 192, 224, 240, 256)
-DEPTH_LIST = (0, 1, 2)
-EXPAND_RATIO_LIST = (0.2, 0.25, 0.35)
-WIDTH_MULT_LIST = (0.65, 0.8, 1.0)
-BASE_DEPTH_LIST = (2, 2, 4, 2)
-
-
-def get_path(name):
-    return str(Path(os.environ.get("EVOXBENCH_MODEL", os.getcwd())) / "resnet" / name)
-
-
-# ------------------- Following functions are specific to ResNet50D search space ------------------- #
-class ResNet50DFeatureEncoder:
-    def __init__(
-            self,
-            image_size_list=IMAGE_SIZE_LIST,
-            depth_list=DEPTH_LIST,
-            expand_list=EXPAND_RATIO_LIST,
-            width_mult_list=WIDTH_MULT_LIST,
-            base_depth_list=BASE_DEPTH_LIST,
-    ):
-        self.image_size_list = image_size_list
-        self.expand_list = expand_list
-        self.depth_list = depth_list
-        self.width_mult_list = width_mult_list
-        self.base_depth_list = base_depth_list
-
-        """" build info dict """
-        self.n_dim = 0
-        # resolution
-        self.r_info = dict(id2val={}, val2id={}, L=[], R=[])
-        self._build_info_dict(target="r")
-        # input stem skip
-        self.input_stem_d_info = dict(id2val={}, val2id={}, L=[], R=[])
-        self._build_info_dict(target="input_stem_d")
-        # width_mult
-        self.width_mult_info = dict(id2val=[], val2id=[], L=[], R=[])
-        self._build_info_dict(target="width_mult")
-        # expand ratio
-        self.e_info = dict(id2val=[], val2id=[], L=[], R=[])
-        self._build_info_dict(target="e")
-
-    @property
-    def n_stage(self):
-        return len(self.base_depth_list)
-
-    @property
-    def max_n_blocks(self):
-        return sum(self.base_depth_list) + self.n_stage * max(self.depth_list)
-
-    def _build_info_dict(self, target):
-        if target == "r":
-            target_dict = self.r_info
-            target_dict["L"].append(self.n_dim)
-            for img_size in self.image_size_list:
-                target_dict["val2id"][img_size] = self.n_dim
-                target_dict["id2val"][self.n_dim] = img_size
-                self.n_dim += 1
-            target_dict["R"].append(self.n_dim)
-        elif target == "input_stem_d":
-            target_dict = self.input_stem_d_info
-            target_dict["L"].append(self.n_dim)
-            for skip in [0, 1]:
-                target_dict["val2id"][skip] = self.n_dim
-                target_dict["id2val"][self.n_dim] = skip
-                self.n_dim += 1
-            target_dict["R"].append(self.n_dim)
-        elif target == "e":
-            target_dict = self.e_info
-            choices = self.expand_list
-            for i in range(self.max_n_blocks):
-                target_dict["val2id"].append({})
-                target_dict["id2val"].append({})
-                target_dict["L"].append(self.n_dim)
-                for e in choices:
-                    target_dict["val2id"][i][e] = self.n_dim
-                    target_dict["id2val"][i][self.n_dim] = e
-                    self.n_dim += 1
-                target_dict["R"].append(self.n_dim)
-        elif target == "width_mult":
-            target_dict = self.width_mult_info
-            choices = list(range(len(self.width_mult_list)))
-            for i in range(self.n_stage + 2):
-                target_dict["val2id"].append({})
-                target_dict["id2val"].append({})
-                target_dict["L"].append(self.n_dim)
-                for w in choices:
-                    target_dict["val2id"][i][w] = self.n_dim
-                    target_dict["id2val"][i][self.n_dim] = w
-                    self.n_dim += 1
-                target_dict["R"].append(self.n_dim)
-
-    def arch2feature(self, arch_dict):
-        d, e, w, r = (
-            arch_dict["d"],
-            arch_dict["e"],
-            arch_dict["w"],
-            arch_dict["r"],
-        )
-        input_stem_skip = 1 if d[0] > 0 else 0
-        d = d[1:]
-
-        feature = np.zeros(self.n_dim)
-        feature[self.r_info["val2id"][r]] = 1
-        feature[self.input_stem_d_info["val2id"][input_stem_skip]] = 1
-        for i in range(self.n_stage + 2):
-            feature[self.width_mult_info["val2id"][i][w[i]]] = 1
-
-        start_pt = 0
-        for i, base_depth in enumerate(self.base_depth_list):
-            depth = base_depth + d[i]
-            for j in range(start_pt, start_pt + depth):
-                feature[self.e_info["val2id"][j][e[j]]] = 1
-            start_pt += max(self.depth_list) + base_depth
-
-        return feature
-
-    def feature2arch(self, feature):
-        img_sz = self.r_info["id2val"][
-            int(np.argmax(feature[self.r_info["L"][0]: self.r_info["R"][0]]))
-            + self.r_info["L"][0]
-            ]
-        input_stem_skip = (
-                self.input_stem_d_info["id2val"][
-                    int(
-                        np.argmax(
-                            feature[
-                            self.input_stem_d_info["L"][0]: self.input_stem_d_info[
-                                "R"
-                            ][0]
-                            ]
-                        )
-                    )
-                    + self.input_stem_d_info["L"][0]
-                    ]
-                * 2
-        )
-        assert img_sz in self.image_size_list
-        arch_dict = {"d": [input_stem_skip], "e": [], "w": [], "r": img_sz}
-
-        for i in range(self.n_stage + 2):
-            arch_dict["w"].append(
-                self.width_mult_info["id2val"][i][
-                    int(
-                        np.argmax(
-                            feature[
-                            self.width_mult_info["L"][i]: self.width_mult_info[
-                                "R"
-                            ][i]
-                            ]
-                        )
-                    )
-                    + self.width_mult_info["L"][i]
-                    ]
-            )
-
-        d = 0
-        skipped = 0
-        stage_id = 0
-        for i in range(self.max_n_blocks):
-            skip = True
-            for j in range(self.e_info["L"][i], self.e_info["R"][i]):
-                if feature[j] == 1:
-                    arch_dict["e"].append(self.e_info["id2val"][i][j])
-                    skip = False
-                    break
-            if skip:
-                arch_dict["e"].append(0)
-                skipped += 1
-            else:
-                d += 1
-
-            if (
-                    i + 1 == self.max_n_blocks
-                    or (skipped + d)
-                    % (max(self.depth_list) + self.base_depth_list[stage_id])
-                    == 0
-            ):
-                arch_dict["d"].append(d - self.base_depth_list[stage_id])
-                d, skipped = 0, 0
-                stage_id += 1
-        return arch_dict
-
-
-class FLOPsPredictor:
-    channel_list = [[40, 48, 64], [168, 208, 256], [336, 408, 512], [664, 816, 1024], [1328, 1640, 2048]]
-    stride_list = [1, 2, 2, 2]
-    base_depth_list = [2, 2, 4, 2]
-
-    def __init__(self, data_file_path=get_path("flops_model.json")):
-        with open(data_file_path, 'r') as f:
-            self.flops_dict = json.load(f)
-
-    def predict_flops(self, sample):
-        input_size = sample.get("r", 224)
-
-        assert "d" in sample and "e" in sample and "w" in sample
-        assert len(sample["d"]) == 5
-        assert len(sample["e"]) == 18
-        assert len(sample["w"]) == 6
-        assert str(input_size) in self.flops_dict
-        flops_dict = self.flops_dict[str(input_size)]
-
-        flops = 0
-        # calculate the input_stem
-
-        flops = flops + flops_dict["input_stem"][str(sample['w'][0])][str(sample['w'][1])][str(sample['d'][0])]
-        # calculate the  blocks
-        base_depth = 0
-        for block_id in range(4):
-
-            for i in range(self.base_depth_list[block_id] + sample['d'][block_id + 1]):
-                idx = base_depth + i
-
-                if i == 0:
-                    stride = self.stride_list[block_id]
-                    in_channel = self.channel_list[block_id][sample['w'][block_id + 1]]
-                    type = "head"
-                else:
-                    stride = 1
-                    in_channel = self.channel_list[block_id + 1][sample['w'][block_id + 2]]
-                    type = "follow"
-                out_channel = self.channel_list[block_id + 1][sample['w'][block_id + 2]]
-                expand_ratio = sample['e'][idx]
-
-                flops = flops + flops_dict['ResNetBottleneckBlock'][str(block_id)][str(in_channel)][
-                    str(out_channel)][str(stride)][str(expand_ratio)][type]
-
-            base_depth = base_depth + self.base_depth_list[block_id] + 2
-
-        # calculate the linear layer
-        in_channel = self.channel_list[-1][sample['w'][-1]]
-        flops = flops + flops_dict["LinearLayer"][str(in_channel)]
-
-        return flops
-
-
-class ParamsPredictor:
-    channel_list = [[40, 48, 64], [168, 208, 256], [336, 408, 512], [664, 816, 1024], [1328, 1640, 2048]]
-    stride_list = [1, 2, 2, 2]
-    base_depth_list = [2, 2, 4, 2]
-
-    def __init__(self, data_file_path=get_path("params_model.json")):
-        with open(data_file_path, 'r') as f:
-            self.params_dict = json.load(f)
-
-    def predict_params(self, sample):
-        assert "d" in sample and "e" in sample and "w" in sample
-        assert len(sample["d"]) == 5
-        assert len(sample["e"]) == 18
-        assert len(sample["w"]) == 6
-
-        params = 0
-        # calculate the input_stem
-
-        params = params + self.params_dict["input_stem"][str(sample['w'][0])][str(sample['w'][1])][str(sample['d'][0])]
-        # calculate the  blocks
-        base_depth = 0
-        for block_id in range(4):
-
-            for i in range(self.base_depth_list[block_id] + sample['d'][block_id + 1]):
-                idx = base_depth + i
-
-                if i == 0:
-                    stride = self.stride_list[block_id]
-                    in_channel = self.channel_list[block_id][sample['w'][block_id + 1]]
-                else:
-                    stride = 1
-                    in_channel = self.channel_list[block_id + 1][sample['w'][block_id + 2]]
-                out_channel = self.channel_list[block_id + 1][sample['w'][block_id + 2]]
-                expand_ratio = sample['e'][idx]
-
-                params = params + self.params_dict['ResNetBottleneckBlock'][str(block_id)][str(in_channel)][
-                    str(out_channel)][str(stride)][str(expand_ratio)]
-
-            base_depth = base_depth + self.base_depth_list[block_id] + 2
-
-        # calculate the linear layer
-        in_channel = self.channel_list[-1][sample['w'][-1]]
-        params = params + self.params_dict["LinearLayer"][str(in_channel)]
-
-        return params
-
-
-class ResNet50DSearchSpace(SearchSpace):
-
-    def __init__(self,
-                 image_scale=IMAGE_SIZE_LIST,  # (min img size, max img size)
-                 depth_list=DEPTH_LIST,  # depth
-                 expand_ratio_list=EXPAND_RATIO_LIST,  # expansion ratio
-                 width_mult_list=WIDTH_MULT_LIST,  # width multiplier
-                 base_depth_list=BASE_DEPTH_LIST,  # base depth list
-                 **kwargs):
-
-        super().__init__(**kwargs)
-
-        self.image_scale_list = list(image_scale)
-        self.depth_list = list(depth_list)
-        self.expand_ratio_list = list(expand_ratio_list)
-        self.width_mult_list = list(width_mult_list)
-        self.base_depth_list = base_depth_list
-
-        # upper and lower bound on the decision variables
-        self.n_var = 25
-        # [image resolution, stem_width1, stem_width2, layer 1, layer 2, ..., layer 18]
-        # image resolution ~ [128, 136, 144, ..., 256]
-        # the last two layers in each stage can be skipped
-        self.lb = [0] + [0, 0, 1, 1, 1, 1] + [1, 1, 0, 0] + [1, 1, 0, 0] + [1, 1, 1, 1, 0, 0] + [1, 1, 0, 0]
-        self.ub = [len(self.image_scale_list) - 1] + [len(width_mult_list)] * 6 + [len(expand_ratio_list)] * 18
-
-        # create the categories for each variable
-        self.categories = [list(range(a, b + 1)) for a, b in zip(self.lb, self.ub)]
-
-        # assuming maximum 4 layers per stage for 5 stages
-        self.stage_width_indices = [1, 2, 3, 4, 5, 6]
-        self.stage_layer_indices = [[7, 8, 9, 10], [11, 12, 13, 14], [15, 16, 17, 18, 19, 20], [21, 22, 23, 24]]
-
-    @property
-    def name(self):
-        return 'ResNet50DSearchSpace'
-
-    def _sample(self, phenotype=True):
-
-        # uniform random sampling
-        x = np.array([np.random.choice(options) for options in self.categories]).astype(int)
-
-        # repair, in case of skipping the last second but not the last layer in a stage
-        for indices in self.stage_layer_indices:
-            if x[indices[-2]] == 0 and x[indices[-1]] > 0:
-                x[indices[-2]] = x[indices[-1]]
-                x[indices[-1]] = 0
-
-        if phenotype:
-            return self._decode(x)
-        else:
-            return x
-
-    def _encode(self, arch):
-        # a sample subnet string
-        # {'r': 224,
-        #  'w': [0, 0, 1, 0, 0, 1],
-        #  'e': [0.35, 0.2, 0.35, 0.35, 0.25, 0.2, 0.2, 0.2, 0.35, 0.35, 0.2, 0.25, 0.2, 0.25, 0.25, 0.25, 0.2, 0.25],
-        #  'd': [2, 0, 0, 2, 2]}
-
-        x = np.array([0] * self.n_var)
-        x[0] = np.where(arch['r'] == np.array(self.image_scale_list))[0][0]
-
-        x[self.stage_width_indices] = arch['w']
-        x[self.stage_width_indices] += 1
-
-        if arch['d'][0] == 0:
-            x[self.stage_width_indices[0]] = 0
-            x[self.stage_width_indices[1]] = 0
-
-        for i, (indices, d) in enumerate(zip(self.stage_layer_indices, arch['d'][1:])):
-            for j in range(d + self.base_depth_list[i]):
-                idx = indices[j]
-                x[idx] = np.where(arch['e'][idx - 7] == np.array(self.expand_ratio_list))[0][0] + 1
-
-        return x
-
-    def _decode(self, x):
-        # a sample decision variable vector x corresponding to the above subnet string
-        # [(image scale) 3,
-        #  (width mult)  2, 1, 2, 2, 2, 2
-        #  (layer exp)   2, 2, 1, 1, 1, 1, 2, 0, 2, 1, 1, 1, 3, 1, 1, 2, 3, 0]
-        expand_ratio_list, depth_list = [], [2]
-        width_mult_list = copy.deepcopy(x[self.stage_width_indices] - 1).tolist()
-
-        if width_mult_list[0] < 0:
-            width_mult_list[0] = np.random.choice(len(self.width_mult_list))
-            depth_list[0] = 0
-
-        if width_mult_list[1] < 0:
-            width_mult_list[1] = np.random.choice(len(self.width_mult_list))
-            depth_list[0] = 0
-
-        for i, indices in enumerate(self.stage_layer_indices):
-            d = len(indices)
-            for idx in indices:
-                if x[idx] < 1:
-                    d -= 1
-                    e = np.random.choice(self.expand_ratio_list)
-                else:
-                    e = self.expand_ratio_list[x[idx] - 1]
-                expand_ratio_list.append(e)
-            depth_list.append(d - self.base_depth_list[i])
-
-        return {
-            'r': self.image_scale_list[x[0]],
-            'w': width_mult_list, 'e': expand_ratio_list, 'd': depth_list}
-
-    def visualize(self, arch):
-        raise NotImplementedError
-
-
-class ResNet50DEvaluator(Evaluator):
-    def __init__(self,
-                 valid_acc_model_path=get_path("valid_acc_predictor_checkpoint.json"),
-                 # ResNet50 validation acc predictor path
-                 test_acc_model_path=get_path("test_acc_predictor_checkpoint.json"),  # ResNet50 test acc predictor path
-                 params_model_path=get_path("params_model.json"),
-                 # path to pretrained Params predictor surrogate model / look-up table
-                 flops_model_path=get_path("flops_model.json"),
-                 # path to pretrained FLOPs predictor surrogate model / look-up table
-                 objs='err&flops&latency',  # objectives to be minimized
-                 ):
-        super().__init__(objs)
-
-        self.feature_encoder = ResNet50DFeatureEncoder()
-        self.valid_acc_predictor = MLPPredictor(pretrained=valid_acc_model_path)
-        self.test_acc_predictor = MLPPredictor(pretrained=test_acc_model_path)
-
-        self.params_predictor = ParamsPredictor(params_model_path)
-        self.flops_predictor = FLOPsPredictor(flops_model_path)
-
-        # # prepare meta file for calculating statistics
-        # self.pf = np.array(json.load(open(pf_file_path, 'r'))[str(fidelity)][objs])
-
-    @property
-    def name(self):
-        return 'ResNet50DEvaluator'
-
-    def evaluate(self, archs, objs=None,
-                 true_eval=False  # query the true (mean over three runs) performance
-                 ):
-
-        if objs is None:
-            objs = self.objs
-
-        features = np.array([self.feature_encoder.arch2feature(arch) for arch in archs])
-
-        batch_stats = []
-
-        if true_eval:
-            top1_accs = self.test_acc_predictor.predict(features)
-        else:
-            top1_accs = self.valid_acc_predictor.predict(features, is_noisy=True)
-
-        for i, (arch, top1) in enumerate(zip(archs, top1_accs)):
-            stats = OrderedDict()
-
-            # todo: add stochastic evaluation method
-            if 'err' in objs:
-                stats['err'] = 1 - top1[0]
-
-            if 'params' in objs:
-                stats['params'] = self.params_predictor.predict_params(arch)
-
-            if 'flops' in objs:
-                stats['flops'] = self.flops_predictor.predict_flops(arch)
-
-            batch_stats.append(stats)
-
-        return batch_stats
-
-
-class ResNet50DBenchmark(Benchmark):
-    def __init__(self,
-                 valid_acc_model_path=get_path("valid_acc_predictor_checkpoint.json"),
-                 # ResNet50 validation acc predictor path
-                 test_acc_model_path=get_path("test_acc_predictor_checkpoint.json"),  # ResNet50 test acc predictor path
-                 params_model_path=get_path("params_model.json"),
-                 # path to pretrained Params predictor surrogate model / look-up table
-                 flops_model_path=get_path("flops_model.json"),
-                 # path to pretrained FLOPs predictor surrogate model / look-up table
-                 objs='err&flops&latency',  # objectives to be minimized
-                 normalized_objectives=False,  # whether to normalize the objectives
-                 ):
-        search_space = ResNet50DSearchSpace()
-        evaluator = ResNet50DEvaluator(
-            valid_acc_model_path, test_acc_model_path, params_model_path, flops_model_path, objs)
-        super().__init__(search_space, evaluator, normalized_objectives)
-
-    @property
-    def name(self):
-        return 'ResNet50DBenchmark'
-
-    @property
-    def _utopian_point(self):
-        """ estimated from sampled architectures, use w/ caution """
-        return {
-            'err&params': [1.987000e-01, 6.542624e+06],
-            'err&flops': [1.98700000e-01, 6.69461472e+08],
-            'err&params&flops': [1.98700000e-01, 6.54262400e+06, 6.69461472e+08],
-        }[self.evaluator.objs]
-
-    @property
-    def _nadir_point(self):
-        """ estimated from sampled architectures, use w/ caution """
-        return {
-            'err&params': [3.1242000e-01, 4.4114544e+07],
-            'err&flops': [3.12420000e-01, 1.45769615e+10],
-            'err&params&flops': [3.12420000e-01, 4.41145440e+07, 1.45769615e+10],
-        }[self.evaluator.objs]
-
-    def debug(self):
-        archs = self.search_space.sample(10)
-        X = self.search_space.encode(archs)
-        F = self.evaluate(X)
-        hv = self.calc_perf_indicator(X, 'hv')
-
-        print(archs)
-        print(X)
-        print(F)
-        print(hv)
-
-
-if __name__ == '__main__':
-    benchmark = ResNet50DBenchmark(
-        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/resnet/valid_acc_predictor_checkpoint.json",
-        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/resnet/test_acc_predictor_checkpoint.json",
-        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/resnet/params_model.json",
-        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/resnet/flops_model.json",
-        objs='err&params', normalized_objectives=True
-    )
-
-    benchmark.debug()
+import json
+import copy
+import os
+from pathlib import Path
+from collections import OrderedDict
+
+import numpy as np
+
+from evoxbench.modules import SearchSpace, Evaluator, Benchmark, MLPPredictor
+
+__all__ = ['ResNet50DSearchSpace', 'ResNet50DEvaluator', 'ResNet50DBenchmark']
+
+IMAGE_SIZE_LIST = (128, 144, 160, 176, 192, 224, 240, 256)
+DEPTH_LIST = (0, 1, 2)
+EXPAND_RATIO_LIST = (0.2, 0.25, 0.35)
+WIDTH_MULT_LIST = (0.65, 0.8, 1.0)
+BASE_DEPTH_LIST = (2, 2, 4, 2)
+
+
+def get_path(name):
+    return str(Path(os.environ.get("EVOXBENCH_MODEL", os.getcwd())) / "resnet" / name)
+
+
+# ------------------- Following functions are specific to ResNet50D search space ------------------- #
+class ResNet50DFeatureEncoder:
+    def __init__(
+            self,
+            image_size_list=IMAGE_SIZE_LIST,
+            depth_list=DEPTH_LIST,
+            expand_list=EXPAND_RATIO_LIST,
+            width_mult_list=WIDTH_MULT_LIST,
+            base_depth_list=BASE_DEPTH_LIST,
+    ):
+        self.image_size_list = image_size_list
+        self.expand_list = expand_list
+        self.depth_list = depth_list
+        self.width_mult_list = width_mult_list
+        self.base_depth_list = base_depth_list
+
+        """" build info dict """
+        self.n_dim = 0
+        # resolution
+        self.r_info = dict(id2val={}, val2id={}, L=[], R=[])
+        self._build_info_dict(target="r")
+        # input stem skip
+        self.input_stem_d_info = dict(id2val={}, val2id={}, L=[], R=[])
+        self._build_info_dict(target="input_stem_d")
+        # width_mult
+        self.width_mult_info = dict(id2val=[], val2id=[], L=[], R=[])
+        self._build_info_dict(target="width_mult")
+        # expand ratio
+        self.e_info = dict(id2val=[], val2id=[], L=[], R=[])
+        self._build_info_dict(target="e")
+
+    @property
+    def n_stage(self):
+        return len(self.base_depth_list)
+
+    @property
+    def max_n_blocks(self):
+        return sum(self.base_depth_list) + self.n_stage * max(self.depth_list)
+
+    def _build_info_dict(self, target):
+        if target == "r":
+            target_dict = self.r_info
+            target_dict["L"].append(self.n_dim)
+            for img_size in self.image_size_list:
+                target_dict["val2id"][img_size] = self.n_dim
+                target_dict["id2val"][self.n_dim] = img_size
+                self.n_dim += 1
+            target_dict["R"].append(self.n_dim)
+        elif target == "input_stem_d":
+            target_dict = self.input_stem_d_info
+            target_dict["L"].append(self.n_dim)
+            for skip in [0, 1]:
+                target_dict["val2id"][skip] = self.n_dim
+                target_dict["id2val"][self.n_dim] = skip
+                self.n_dim += 1
+            target_dict["R"].append(self.n_dim)
+        elif target == "e":
+            target_dict = self.e_info
+            choices = self.expand_list
+            for i in range(self.max_n_blocks):
+                target_dict["val2id"].append({})
+                target_dict["id2val"].append({})
+                target_dict["L"].append(self.n_dim)
+                for e in choices:
+                    target_dict["val2id"][i][e] = self.n_dim
+                    target_dict["id2val"][i][self.n_dim] = e
+                    self.n_dim += 1
+                target_dict["R"].append(self.n_dim)
+        elif target == "width_mult":
+            target_dict = self.width_mult_info
+            choices = list(range(len(self.width_mult_list)))
+            for i in range(self.n_stage + 2):
+                target_dict["val2id"].append({})
+                target_dict["id2val"].append({})
+                target_dict["L"].append(self.n_dim)
+                for w in choices:
+                    target_dict["val2id"][i][w] = self.n_dim
+                    target_dict["id2val"][i][self.n_dim] = w
+                    self.n_dim += 1
+                target_dict["R"].append(self.n_dim)
+
+    def arch2feature(self, arch_dict):
+        d, e, w, r = (
+            arch_dict["d"],
+            arch_dict["e"],
+            arch_dict["w"],
+            arch_dict["r"],
+        )
+        input_stem_skip = 1 if d[0] > 0 else 0
+        d = d[1:]
+
+        feature = np.zeros(self.n_dim)
+        feature[self.r_info["val2id"][r]] = 1
+        feature[self.input_stem_d_info["val2id"][input_stem_skip]] = 1
+        for i in range(self.n_stage + 2):
+            feature[self.width_mult_info["val2id"][i][w[i]]] = 1
+
+        start_pt = 0
+        for i, base_depth in enumerate(self.base_depth_list):
+            depth = base_depth + d[i]
+            for j in range(start_pt, start_pt + depth):
+                feature[self.e_info["val2id"][j][e[j]]] = 1
+            start_pt += max(self.depth_list) + base_depth
+
+        return feature
+
+    def feature2arch(self, feature):
+        img_sz = self.r_info["id2val"][
+            int(np.argmax(feature[self.r_info["L"][0]: self.r_info["R"][0]]))
+            + self.r_info["L"][0]
+            ]
+        input_stem_skip = (
+                self.input_stem_d_info["id2val"][
+                    int(
+                        np.argmax(
+                            feature[
+                            self.input_stem_d_info["L"][0]: self.input_stem_d_info[
+                                "R"
+                            ][0]
+                            ]
+                        )
+                    )
+                    + self.input_stem_d_info["L"][0]
+                    ]
+                * 2
+        )
+        assert img_sz in self.image_size_list
+        arch_dict = {"d": [input_stem_skip], "e": [], "w": [], "r": img_sz}
+
+        for i in range(self.n_stage + 2):
+            arch_dict["w"].append(
+                self.width_mult_info["id2val"][i][
+                    int(
+                        np.argmax(
+                            feature[
+                            self.width_mult_info["L"][i]: self.width_mult_info[
+                                "R"
+                            ][i]
+                            ]
+                        )
+                    )
+                    + self.width_mult_info["L"][i]
+                    ]
+            )
+
+        d = 0
+        skipped = 0
+        stage_id = 0
+        for i in range(self.max_n_blocks):
+            skip = True
+            for j in range(self.e_info["L"][i], self.e_info["R"][i]):
+                if feature[j] == 1:
+                    arch_dict["e"].append(self.e_info["id2val"][i][j])
+                    skip = False
+                    break
+            if skip:
+                arch_dict["e"].append(0)
+                skipped += 1
+            else:
+                d += 1
+
+            if (
+                    i + 1 == self.max_n_blocks
+                    or (skipped + d)
+                    % (max(self.depth_list) + self.base_depth_list[stage_id])
+                    == 0
+            ):
+                arch_dict["d"].append(d - self.base_depth_list[stage_id])
+                d, skipped = 0, 0
+                stage_id += 1
+        return arch_dict
+
+
+class FLOPsPredictor:
+    channel_list = [[40, 48, 64], [168, 208, 256], [336, 408, 512], [664, 816, 1024], [1328, 1640, 2048]]
+    stride_list = [1, 2, 2, 2]
+    base_depth_list = [2, 2, 4, 2]
+
+    def __init__(self, data_file_path=get_path("flops_model.json")):
+        with open(data_file_path, 'r') as f:
+            self.flops_dict = json.load(f)
+
+    def predict_flops(self, sample):
+        input_size = sample.get("r", 224)
+
+        assert "d" in sample and "e" in sample and "w" in sample
+        assert len(sample["d"]) == 5
+        assert len(sample["e"]) == 18
+        assert len(sample["w"]) == 6
+        assert str(input_size) in self.flops_dict
+        flops_dict = self.flops_dict[str(input_size)]
+
+        flops = 0
+        # calculate the input_stem
+
+        flops = flops + flops_dict["input_stem"][str(sample['w'][0])][str(sample['w'][1])][str(sample['d'][0])]
+        # calculate the  blocks
+        base_depth = 0
+        for block_id in range(4):
+
+            for i in range(self.base_depth_list[block_id] + sample['d'][block_id + 1]):
+                idx = base_depth + i
+
+                if i == 0:
+                    stride = self.stride_list[block_id]
+                    in_channel = self.channel_list[block_id][sample['w'][block_id + 1]]
+                    type = "head"
+                else:
+                    stride = 1
+                    in_channel = self.channel_list[block_id + 1][sample['w'][block_id + 2]]
+                    type = "follow"
+                out_channel = self.channel_list[block_id + 1][sample['w'][block_id + 2]]
+                expand_ratio = sample['e'][idx]
+
+                flops = flops + flops_dict['ResNetBottleneckBlock'][str(block_id)][str(in_channel)][
+                    str(out_channel)][str(stride)][str(expand_ratio)][type]
+
+            base_depth = base_depth + self.base_depth_list[block_id] + 2
+
+        # calculate the linear layer
+        in_channel = self.channel_list[-1][sample['w'][-1]]
+        flops = flops + flops_dict["LinearLayer"][str(in_channel)]
+
+        return flops
+
+
+class ParamsPredictor:
+    channel_list = [[40, 48, 64], [168, 208, 256], [336, 408, 512], [664, 816, 1024], [1328, 1640, 2048]]
+    stride_list = [1, 2, 2, 2]
+    base_depth_list = [2, 2, 4, 2]
+
+    def __init__(self, data_file_path=get_path("params_model.json")):
+        with open(data_file_path, 'r') as f:
+            self.params_dict = json.load(f)
+
+    def predict_params(self, sample):
+        assert "d" in sample and "e" in sample and "w" in sample
+        assert len(sample["d"]) == 5
+        assert len(sample["e"]) == 18
+        assert len(sample["w"]) == 6
+
+        params = 0
+        # calculate the input_stem
+
+        params = params + self.params_dict["input_stem"][str(sample['w'][0])][str(sample['w'][1])][str(sample['d'][0])]
+        # calculate the  blocks
+        base_depth = 0
+        for block_id in range(4):
+
+            for i in range(self.base_depth_list[block_id] + sample['d'][block_id + 1]):
+                idx = base_depth + i
+
+                if i == 0:
+                    stride = self.stride_list[block_id]
+                    in_channel = self.channel_list[block_id][sample['w'][block_id + 1]]
+                else:
+                    stride = 1
+                    in_channel = self.channel_list[block_id + 1][sample['w'][block_id + 2]]
+                out_channel = self.channel_list[block_id + 1][sample['w'][block_id + 2]]
+                expand_ratio = sample['e'][idx]
+
+                params = params + self.params_dict['ResNetBottleneckBlock'][str(block_id)][str(in_channel)][
+                    str(out_channel)][str(stride)][str(expand_ratio)]
+
+            base_depth = base_depth + self.base_depth_list[block_id] + 2
+
+        # calculate the linear layer
+        in_channel = self.channel_list[-1][sample['w'][-1]]
+        params = params + self.params_dict["LinearLayer"][str(in_channel)]
+
+        return params
+
+
+class ResNet50DSearchSpace(SearchSpace):
+
+    def __init__(self,
+                 image_scale=IMAGE_SIZE_LIST,  # (min img size, max img size)
+                 depth_list=DEPTH_LIST,  # depth
+                 expand_ratio_list=EXPAND_RATIO_LIST,  # expansion ratio
+                 width_mult_list=WIDTH_MULT_LIST,  # width multiplier
+                 base_depth_list=BASE_DEPTH_LIST,  # base depth list
+                 **kwargs):
+
+        super().__init__(**kwargs)
+
+        self.image_scale_list = list(image_scale)
+        self.depth_list = list(depth_list)
+        self.expand_ratio_list = list(expand_ratio_list)
+        self.width_mult_list = list(width_mult_list)
+        self.base_depth_list = base_depth_list
+
+        # upper and lower bound on the decision variables
+        self.n_var = 25
+        # [image resolution, stem_width1, stem_width2, layer 1, layer 2, ..., layer 18]
+        # image resolution ~ [128, 136, 144, ..., 256]
+        # the last two layers in each stage can be skipped
+        self.lb = [0] + [0, 0, 1, 1, 1, 1] + [1, 1, 0, 0] + [1, 1, 0, 0] + [1, 1, 1, 1, 0, 0] + [1, 1, 0, 0]
+        self.ub = [len(self.image_scale_list) - 1] + [len(width_mult_list)] * 6 + [len(expand_ratio_list)] * 18
+
+        # create the categories for each variable
+        self.categories = [list(range(a, b + 1)) for a, b in zip(self.lb, self.ub)]
+
+        # assuming maximum 4 layers per stage for 5 stages
+        self.stage_width_indices = [1, 2, 3, 4, 5, 6]
+        self.stage_layer_indices = [[7, 8, 9, 10], [11, 12, 13, 14], [15, 16, 17, 18, 19, 20], [21, 22, 23, 24]]
+
+    @property
+    def name(self):
+        return 'ResNet50DSearchSpace'
+
+    def _sample(self, phenotype=True):
+
+        # uniform random sampling
+        x = np.array([np.random.choice(options) for options in self.categories]).astype(int)
+
+        # repair, in case of skipping the last second but not the last layer in a stage
+        for indices in self.stage_layer_indices:
+            if x[indices[-2]] == 0 and x[indices[-1]] > 0:
+                x[indices[-2]] = x[indices[-1]]
+                x[indices[-1]] = 0
+
+        if phenotype:
+            return self._decode(x)
+        else:
+            return x
+
+    def _encode(self, arch):
+        # a sample subnet string
+        # {'r': 224,
+        #  'w': [0, 0, 1, 0, 0, 1],
+        #  'e': [0.35, 0.2, 0.35, 0.35, 0.25, 0.2, 0.2, 0.2, 0.35, 0.35, 0.2, 0.25, 0.2, 0.25, 0.25, 0.25, 0.2, 0.25],
+        #  'd': [2, 0, 0, 2, 2]}
+
+        x = np.array([0] * self.n_var)
+        x[0] = np.where(arch['r'] == np.array(self.image_scale_list))[0][0]
+
+        x[self.stage_width_indices] = arch['w']
+        x[self.stage_width_indices] += 1
+
+        if arch['d'][0] == 0:
+            x[self.stage_width_indices[0]] = 0
+            x[self.stage_width_indices[1]] = 0
+
+        for i, (indices, d) in enumerate(zip(self.stage_layer_indices, arch['d'][1:])):
+            for j in range(d + self.base_depth_list[i]):
+                idx = indices[j]
+                x[idx] = np.where(arch['e'][idx - 7] == np.array(self.expand_ratio_list))[0][0] + 1
+
+        return x
+
+    def _decode(self, x):
+        # a sample decision variable vector x corresponding to the above subnet string
+        # [(image scale) 3,
+        #  (width mult)  2, 1, 2, 2, 2, 2
+        #  (layer exp)   2, 2, 1, 1, 1, 1, 2, 0, 2, 1, 1, 1, 3, 1, 1, 2, 3, 0]
+        expand_ratio_list, depth_list = [], [2]
+        width_mult_list = copy.deepcopy(x[self.stage_width_indices] - 1).tolist()
+
+        if width_mult_list[0] < 0:
+            width_mult_list[0] = np.random.choice(len(self.width_mult_list))
+            depth_list[0] = 0
+
+        if width_mult_list[1] < 0:
+            width_mult_list[1] = np.random.choice(len(self.width_mult_list))
+            depth_list[0] = 0
+
+        for i, indices in enumerate(self.stage_layer_indices):
+            d = len(indices)
+            for idx in indices:
+                if x[idx] < 1:
+                    d -= 1
+                    e = np.random.choice(self.expand_ratio_list)
+                else:
+                    e = self.expand_ratio_list[x[idx] - 1]
+                expand_ratio_list.append(e)
+            depth_list.append(d - self.base_depth_list[i])
+
+        return {
+            'r': self.image_scale_list[x[0]],
+            'w': width_mult_list, 'e': expand_ratio_list, 'd': depth_list}
+
+    def visualize(self, arch):
+        raise NotImplementedError
+
+
+class ResNet50DEvaluator(Evaluator):
+    def __init__(self,
+                 valid_acc_model_path=get_path("valid_acc_predictor_checkpoint.json"),
+                 # ResNet50 validation acc predictor path
+                 test_acc_model_path=get_path("test_acc_predictor_checkpoint.json"),  # ResNet50 test acc predictor path
+                 params_model_path=get_path("params_model.json"),
+                 # path to pretrained Params predictor surrogate model / look-up table
+                 flops_model_path=get_path("flops_model.json"),
+                 # path to pretrained FLOPs predictor surrogate model / look-up table
+                 objs='err&flops&latency',  # objectives to be minimized
+                 ):
+        super().__init__(objs)
+
+        self.feature_encoder = ResNet50DFeatureEncoder()
+        self.valid_acc_predictor = MLPPredictor(pretrained=valid_acc_model_path)
+        self.test_acc_predictor = MLPPredictor(pretrained=test_acc_model_path)
+
+        self.params_predictor = ParamsPredictor(params_model_path)
+        self.flops_predictor = FLOPsPredictor(flops_model_path)
+
+        # # prepare meta file for calculating statistics
+        # self.pf = np.array(json.load(open(pf_file_path, 'r'))[str(fidelity)][objs])
+
+    @property
+    def name(self):
+        return 'ResNet50DEvaluator'
+
+    def evaluate(self, archs, objs=None,
+                 true_eval=False  # query the true (mean over three runs) performance
+                 ):
+
+        if objs is None:
+            objs = self.objs
+
+        features = np.array([self.feature_encoder.arch2feature(arch) for arch in archs])
+
+        batch_stats = []
+
+        if true_eval:
+            top1_accs = self.test_acc_predictor.predict(features)
+        else:
+            top1_accs = self.valid_acc_predictor.predict(features, is_noisy=True)
+
+        for i, (arch, top1) in enumerate(zip(archs, top1_accs)):
+            stats = OrderedDict()
+
+            # todo: add stochastic evaluation method
+            if 'err' in objs:
+                stats['err'] = 1 - top1[0]
+
+            if 'params' in objs:
+                stats['params'] = self.params_predictor.predict_params(arch)
+
+            if 'flops' in objs:
+                stats['flops'] = self.flops_predictor.predict_flops(arch)
+
+            batch_stats.append(stats)
+
+        return batch_stats
+
+
+class ResNet50DBenchmark(Benchmark):
+    def __init__(self,
+                 valid_acc_model_path=get_path("valid_acc_predictor_checkpoint.json"),
+                 # ResNet50 validation acc predictor path
+                 test_acc_model_path=get_path("test_acc_predictor_checkpoint.json"),  # ResNet50 test acc predictor path
+                 params_model_path=get_path("params_model.json"),
+                 # path to pretrained Params predictor surrogate model / look-up table
+                 flops_model_path=get_path("flops_model.json"),
+                 # path to pretrained FLOPs predictor surrogate model / look-up table
+                 objs='err&flops&latency',  # objectives to be minimized
+                 normalized_objectives=False,  # whether to normalize the objectives
+                 ):
+        search_space = ResNet50DSearchSpace()
+        evaluator = ResNet50DEvaluator(
+            valid_acc_model_path, test_acc_model_path, params_model_path, flops_model_path, objs)
+        super().__init__(search_space, evaluator, normalized_objectives)
+
+    @property
+    def name(self):
+        return 'ResNet50DBenchmark'
+
+    @property
+    def _utopian_point(self):
+        """ estimated from sampled architectures, use w/ caution """
+        return {
+            'err&params': [1.987000e-01, 6.542624e+06],
+            'err&flops': [1.98700000e-01, 6.69461472e+08],
+            'err&params&flops': [1.98700000e-01, 6.54262400e+06, 6.69461472e+08],
+        }[self.evaluator.objs]
+
+    @property
+    def _nadir_point(self):
+        """ estimated from sampled architectures, use w/ caution """
+        return {
+            'err&params': [3.1242000e-01, 4.4114544e+07],
+            'err&flops': [3.12420000e-01, 1.45769615e+10],
+            'err&params&flops': [3.12420000e-01, 4.41145440e+07, 1.45769615e+10],
+        }[self.evaluator.objs]
+
+    def debug(self):
+        archs = self.search_space.sample(10)
+        X = self.search_space.encode(archs)
+        F = self.evaluate(X)
+        hv = self.calc_perf_indicator(X, 'hv')
+
+        print(archs)
+        print(X)
+        print(F)
+        print(hv)
+
+
+if __name__ == '__main__':
+    benchmark = ResNet50DBenchmark(
+        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/resnet/valid_acc_predictor_checkpoint.json",
+        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/resnet/test_acc_predictor_checkpoint.json",
+        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/resnet/params_model.json",
+        "/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/evoxbench/benchmarks/data/resnet/flops_model.json",
+        objs='err&params', normalized_objectives=True
+    )
+
+    benchmark.debug()
```

### Comparing `evoxbench-1.0.2/evoxbench/database/ORM/settings.py` & `evoxbench-1.0.3/evoxbench/database/ORM/settings.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-"""
-Django settings for ORM project.
-
-Generated by 'django-admin startproject' using Django 3.2.12.
-
-For more information on this file, see
-https://docs.djangoproject.com/en/3.2/topics/settings/
-
-For the full list of settings and their values, see
-https://docs.djangoproject.com/en/3.2/ref/settings/
-"""
-import logging.handlers
-import os
-from pathlib import Path
-
-# Build paths inside the project like this: BASE_DIR / 'subdir'.
-BASE_DIR = Path(__file__).resolve().parent.parent
-
-LOGGING = None
-LOGGING_CONFIG = None
-FORCE_SCRIPT_NAME = None
-# Quick-start development settings - unsuitable for production
-# See https://docs.djangoproject.com/en/3.2/howto/deployment/checklist/
-
-# SECURITY WARNING: keep the secret key used in production secret!
-SECRET_KEY = 'django-insecure-rz7_ah$+638!cm7bshjq)tu&)izufg6qhj^*0ge1y@=5+6u!sf'
-
-# SECURITY WARNING: don't run with debug turned on in production!
-DEBUG = True
-
-ALLOWED_HOSTS = ['*', ]
-
-# Application definition
-
-INSTALLED_APPS = [
-    'django.contrib.admin',
-    'django.contrib.auth',
-    'django.contrib.contenttypes',
-    'django.contrib.sessions',
-    'django.contrib.messages',
-    'django.contrib.staticfiles',
-    # "nasbenchbase",
-    # 'python_codes.evoxbench.database.nasbench101',
-    "nasbench101",
-    "nasbench201",
-    "darts",
-    "natsbenchsss",
-    "mobilenetv3",
-    "resnet50"
-]
-
-MIDDLEWARE = [
-    'django.middleware.security.SecurityMiddleware',
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.middleware.common.CommonMiddleware',
-    'django.middleware.csrf.CsrfViewMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware',
-    'django.middleware.clickjacking.XFrameOptionsMiddleware',
-]
-
-ROOT_URLCONF = 'ORM.urls'
-
-TEMPLATES = [
-    {
-        'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'DIRS': [BASE_DIR / 'templates']
-        ,
-        'APP_DIRS': True,
-        'OPTIONS': {
-            'context_processors': [
-                'django.template.context_processors.debug',
-                'django.template.context_processors.request',
-                'django.contrib.auth.context_processors.auth',
-                'django.contrib.messages.context_processors.messages',
-            ],
-        },
-    },
-]
-
-WSGI_APPLICATION = 'ORM.wsgi.application'
-
-# Database
-# https://docs.djangoproject.com/en/3.2/ref/settings/#databases
-
-DATABASES = {
-    'default': {
-        'ENGINE': 'django.db.backends.sqlite3',
-        'NAME': Path(os.environ.get("EVOXBENCH_DATA") or str(BASE_DIR)) / 'db.sqlite3',
-    }
-}
-
-# Password validation
-# https://docs.djangoproject.com/en/3.2/ref/settings/#auth-password-validators
-
-AUTH_PASSWORD_VALIDATORS = [
-    {
-        'NAME': 'django.contrib.auth.password_validation.UserAttributeSimilarityValidator',
-    },
-    {
-        'NAME': 'django.contrib.auth.password_validation.MinimumLengthValidator',
-    },
-    {
-        'NAME': 'django.contrib.auth.password_validation.CommonPasswordValidator',
-    },
-    {
-        'NAME': 'django.contrib.auth.password_validation.NumericPasswordValidator',
-    },
-]
-
-# Internationalization
-# https://docs.djangoproject.com/en/3.2/topics/i18n/
-
-LANGUAGE_CODE = 'en-us'
-
-TIME_ZONE = 'UTC'
-
-USE_I18N = True
-
-USE_L10N = True
-
-USE_TZ = True
-
-# Static files (CSS, JavaScript, Images)
-# https://docs.djangoproject.com/en/3.2/howto/static-files/
-
-STATIC_URL = '/static/'
-
-# Default primary key field type
-# https://docs.djangoproject.com/en/3.2/ref/settings/#default-auto-field
-
-DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'
+"""
+Django settings for ORM project.
+
+Generated by 'django-admin startproject' using Django 3.2.12.
+
+For more information on this file, see
+https://docs.djangoproject.com/en/3.2/topics/settings/
+
+For the full list of settings and their values, see
+https://docs.djangoproject.com/en/3.2/ref/settings/
+"""
+import logging.handlers
+import os
+from pathlib import Path
+
+# Build paths inside the project like this: BASE_DIR / 'subdir'.
+BASE_DIR = Path(__file__).resolve().parent.parent
+
+LOGGING = None
+LOGGING_CONFIG = None
+FORCE_SCRIPT_NAME = None
+# Quick-start development settings - unsuitable for production
+# See https://docs.djangoproject.com/en/3.2/howto/deployment/checklist/
+
+# SECURITY WARNING: keep the secret key used in production secret!
+SECRET_KEY = 'django-insecure-rz7_ah$+638!cm7bshjq)tu&)izufg6qhj^*0ge1y@=5+6u!sf'
+
+# SECURITY WARNING: don't run with debug turned on in production!
+DEBUG = True
+
+ALLOWED_HOSTS = ['*', ]
+
+# Application definition
+
+INSTALLED_APPS = [
+    'django.contrib.admin',
+    'django.contrib.auth',
+    'django.contrib.contenttypes',
+    'django.contrib.sessions',
+    'django.contrib.messages',
+    'django.contrib.staticfiles',
+    # "nasbenchbase",
+    # 'python_codes.evoxbench.database.nasbench101',
+    "nasbench101",
+    "nasbench201",
+    "darts",
+    "natsbenchsss",
+    "mobilenetv3",
+    "resnet50"
+]
+
+MIDDLEWARE = [
+    'django.middleware.security.SecurityMiddleware',
+    'django.contrib.sessions.middleware.SessionMiddleware',
+    'django.middleware.common.CommonMiddleware',
+    'django.middleware.csrf.CsrfViewMiddleware',
+    'django.contrib.auth.middleware.AuthenticationMiddleware',
+    'django.contrib.messages.middleware.MessageMiddleware',
+    'django.middleware.clickjacking.XFrameOptionsMiddleware',
+]
+
+ROOT_URLCONF = 'ORM.urls'
+
+TEMPLATES = [
+    {
+        'BACKEND': 'django.template.backends.django.DjangoTemplates',
+        'DIRS': [BASE_DIR / 'templates']
+        ,
+        'APP_DIRS': True,
+        'OPTIONS': {
+            'context_processors': [
+                'django.template.context_processors.debug',
+                'django.template.context_processors.request',
+                'django.contrib.auth.context_processors.auth',
+                'django.contrib.messages.context_processors.messages',
+            ],
+        },
+    },
+]
+
+WSGI_APPLICATION = 'ORM.wsgi.application'
+
+# Database
+# https://docs.djangoproject.com/en/3.2/ref/settings/#databases
+
+DATABASES = {
+    'default': {
+        'ENGINE': 'django.db.backends.sqlite3',
+        'NAME': Path(os.environ.get("EVOXBENCH_DATA") or str(BASE_DIR)) / 'db.sqlite3',
+    }
+}
+
+# Password validation
+# https://docs.djangoproject.com/en/3.2/ref/settings/#auth-password-validators
+
+AUTH_PASSWORD_VALIDATORS = [
+    {
+        'NAME': 'django.contrib.auth.password_validation.UserAttributeSimilarityValidator',
+    },
+    {
+        'NAME': 'django.contrib.auth.password_validation.MinimumLengthValidator',
+    },
+    {
+        'NAME': 'django.contrib.auth.password_validation.CommonPasswordValidator',
+    },
+    {
+        'NAME': 'django.contrib.auth.password_validation.NumericPasswordValidator',
+    },
+]
+
+# Internationalization
+# https://docs.djangoproject.com/en/3.2/topics/i18n/
+
+LANGUAGE_CODE = 'en-us'
+
+TIME_ZONE = 'UTC'
+
+USE_I18N = True
+
+USE_L10N = True
+
+USE_TZ = True
+
+# Static files (CSS, JavaScript, Images)
+# https://docs.djangoproject.com/en/3.2/howto/static-files/
+
+STATIC_URL = '/static/'
+
+# Default primary key field type
+# https://docs.djangoproject.com/en/3.2/ref/settings/#default-auto-field
+
+DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'
```

### Comparing `evoxbench-1.0.2/evoxbench/database/darts/migrations/0001_initial.py` & `evoxbench-1.0.3/evoxbench/database/darts/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# Generated by Django 3.2.12 on 2022-03-28 03:17
-
-from django.db import migrations, models
-
-
-class Migration(migrations.Migration):
-    initial = True
-
-    dependencies = [
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='NASBench301Result',
-            fields=[
-                ('id', models.BigAutoField(primary_key=True, serialize=False)),
-                ('index', models.TextField(db_index=True, max_length=256, null=True)),
-                ('phenotype', models.JSONField(default=dict)),
-                ('genotype', models.JSONField(default=dict)),
-                ('result', models.JSONField(default=dict)),
-                ('normal', models.CharField(max_length=128)),
-                ('normal_concat', models.CharField(max_length=128)),
-                ('reduce', models.CharField(max_length=128)),
-                ('reduce_concat', models.CharField(max_length=128)),
-                ('epochs', models.IntegerField()),
-                ('dataset_id', models.IntegerField()),
-                ('dataset_path', models.CharField(max_length=256)),
-            ],
-            options={
-                'abstract': False,
-            },
-        ),
-    ]
+# Generated by Django 3.2.12 on 2022-03-28 03:17
+
+from django.db import migrations, models
+
+
+class Migration(migrations.Migration):
+    initial = True
+
+    dependencies = [
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='NASBench301Result',
+            fields=[
+                ('id', models.BigAutoField(primary_key=True, serialize=False)),
+                ('index', models.TextField(db_index=True, max_length=256, null=True)),
+                ('phenotype', models.JSONField(default=dict)),
+                ('genotype', models.JSONField(default=dict)),
+                ('result', models.JSONField(default=dict)),
+                ('normal', models.CharField(max_length=128)),
+                ('normal_concat', models.CharField(max_length=128)),
+                ('reduce', models.CharField(max_length=128)),
+                ('reduce_concat', models.CharField(max_length=128)),
+                ('epochs', models.IntegerField()),
+                ('dataset_id', models.IntegerField()),
+                ('dataset_path', models.CharField(max_length=256)),
+            ],
+            options={
+                'abstract': False,
+            },
+        ),
+    ]
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/fbnet_models/model_infer.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/fbnet_models/model_infer.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,293 +1,293 @@
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-from torch.nn import init
-from torch.autograd import Variable
-import numpy as np
-
-
-class ChannelShuffle(nn.Module):
-    def __init__(self, groups):
-        super(ChannelShuffle, self).__init__()
-        self.groups = groups
-
-    def forward(self, x):
-        """Channel shuffle: [N,C,H,W] -> [N,g,C/g,H,W] -> [N,C/g,g,H,w] -> [N,C,H,W]"""
-        N, C, H, W = x.size()
-        g = self.groups
-        assert (
-                C % g == 0
-        ), "Incompatible group size {} for input channel {}".format(g, C)
-        return (
-            x.view(N, g, int(C / g), H, W)
-            .permute(0, 2, 1, 3, 4)
-            .contiguous()
-            .view(N, C, H, W)
-        )
-
-
-class ConvNorm(nn.Module):
-    '''
-    conv => norm => activation
-    use native Conv2d, not slimmable
-    '''
-
-    def __init__(self, C_in, C_out, kernel_size=3, stride=1, padding=None, dilation=1, groups=1, bias=False):
-        super(ConvNorm, self).__init__()
-        self.C_in = C_in
-        self.C_out = C_out
-
-        self.kernel_size = kernel_size
-        assert stride in [1, 2]
-        self.stride = stride
-        if padding is None:
-            # assume h_out = h_in / s
-            self.padding = int(np.ceil((dilation * (kernel_size - 1) + 1 - stride) / 2.))
-        else:
-            self.padding = padding
-        self.dilation = dilation
-        assert type(groups) == int
-        self.groups = groups
-        self.bias = bias
-
-        self.conv = nn.Conv2d(C_in, C_out, kernel_size=self.kernel_size, stride=self.stride, padding=self.padding,
-                              dilation=self.dilation, groups=self.groups, bias=bias)
-        self.bn = nn.BatchNorm2d(C_out)
-        self.relu = nn.ReLU(inplace=True)
-
-    def forward(self, x):
-        x = self.relu(self.bn(self.conv(x)))
-        return x
-
-
-class ConvBlock(nn.Module):
-    '''
-    conv => norm => activation
-    use native nn.Conv2d, not slimmable
-    '''
-
-    def __init__(self, C_in, C_out, layer_id, expansion=1, kernel_size=3, stride=1, padding=None, dilation=1, groups=1,
-                 bias=False):
-        super(ConvBlock, self).__init__()
-        self.C_in = C_in
-        self.C_out = C_out
-
-        self.layer_id = layer_id
-
-        assert type(expansion) == int
-        self.expansion = expansion
-        self.kernel_size = kernel_size
-        assert stride in [1, 2]
-        self.stride = stride
-        if padding is None:
-            # assume h_out = h_in / s
-            self.padding = int(np.ceil((dilation * (kernel_size - 1) + 1 - stride) / 2.))
-        else:
-            self.padding = padding
-        self.dilation = dilation
-        assert type(groups) == int
-        self.groups = groups
-        self.bias = bias
-
-        if self.groups > 1:
-            self.shuffle = ChannelShuffle(self.groups)
-
-        self.conv1 = nn.Conv2d(C_in, C_in * expansion, kernel_size=1, stride=1, padding=0, dilation=1,
-                               groups=self.groups, bias=bias)
-        self.bn1 = nn.BatchNorm2d(C_in * expansion)
-
-        self.conv2 = nn.Conv2d(C_in * expansion, C_in * expansion, kernel_size=self.kernel_size, stride=self.stride,
-                               padding=self.padding, dilation=1, groups=C_in * expansion, bias=bias)
-        self.bn2 = nn.BatchNorm2d(C_in * expansion)
-
-        self.conv3 = nn.Conv2d(C_in * expansion, C_out, kernel_size=1, stride=1, padding=0, dilation=1,
-                               groups=self.groups, bias=bias)
-        self.bn3 = nn.BatchNorm2d(C_out)
-
-        self.nl = nn.ReLU(inplace=True)
-
-    # beta, mode, act_num, beta_param are for bit-widths search
-    def forward(self, x):
-
-        identity = x
-        x = self.nl(self.bn1(self.conv1(x)))
-
-        if self.groups > 1:
-            x = self.shuffle(x)
-
-        x = self.nl(self.bn2(self.conv2(x)))
-
-        x = self.bn3(self.conv3(x))
-
-        if self.C_in == self.C_out and self.stride == 1:
-            x += identity
-
-        return x
-
-
-class Skip(nn.Module):
-    def __init__(self, C_in, C_out, layer_id, stride=1):
-        super(Skip, self).__init__()
-        assert stride in [1, 2]
-        assert C_out % 2 == 0, 'C_out=%d' % C_out
-        self.C_in = C_in
-        self.C_out = C_out
-        self.stride = stride
-
-        self.layer_id = layer_id
-
-        self.kernel_size = 1
-        self.padding = 0
-
-        if stride == 2 or C_in != C_out:
-            self.conv = nn.Conv2d(C_in, C_out, 1, stride=stride, padding=0, bias=False)
-            self.bn = nn.BatchNorm2d(C_out)
-            self.relu = nn.ReLU(inplace=True)
-
-    def forward(self, x):
-        if hasattr(self, 'conv'):
-            out = self.conv(x)
-            out = self.bn(out)
-            out = self.relu(out)
-        else:
-            out = x
-
-        return out
-
-
-# The 9 blocks in FBNet Space
-PRIMITIVES = [
-    'k3_e1',
-    'k3_e1_g2',
-    'k3_e3',
-    'k3_e6',
-    'k5_e1',
-    'k5_e1_g2',
-    'k5_e3',
-    'k5_e6',
-    'skip'
-]
-
-OPS = {
-    'k3_e1': lambda C_in, C_out, layer_id, stride: ConvBlock(C_in, C_out, layer_id, expansion=1, kernel_size=3,
-                                                             stride=stride, groups=1),
-    'k3_e1_g2': lambda C_in, C_out, layer_id, stride: ConvBlock(C_in, C_out, layer_id, expansion=1, kernel_size=3,
-                                                                stride=stride, groups=2),
-    'k3_e3': lambda C_in, C_out, layer_id, stride: ConvBlock(C_in, C_out, layer_id, expansion=3, kernel_size=3,
-                                                             stride=stride, groups=1),
-    'k3_e6': lambda C_in, C_out, layer_id, stride: ConvBlock(C_in, C_out, layer_id, expansion=6, kernel_size=3,
-                                                             stride=stride, groups=1),
-    'k5_e1': lambda C_in, C_out, layer_id, stride: ConvBlock(C_in, C_out, layer_id, expansion=1, kernel_size=5,
-                                                             stride=stride, groups=1),
-    'k5_e1_g2': lambda C_in, C_out, layer_id, stride: ConvBlock(C_in, C_out, layer_id, expansion=1, kernel_size=5,
-                                                                stride=stride, groups=2),
-    'k5_e3': lambda C_in, C_out, layer_id, stride: ConvBlock(C_in, C_out, layer_id, expansion=3, kernel_size=5,
-                                                             stride=stride, groups=1),
-    'k5_e6': lambda C_in, C_out, layer_id, stride: ConvBlock(C_in, C_out, layer_id, expansion=6, kernel_size=5,
-                                                             stride=stride, groups=1),
-    'skip': lambda C_in, C_out, layer_id, stride: Skip(C_in, C_out, layer_id, stride)
-}
-
-AUX_OPS = {
-    'ConvNorm': lambda C_in, C_out, layer_id, kernel_size, stride: ConvBlock(C_in, C_out, layer_id,
-                                                                             kernel_size=kernel_size, stride=stride),
-    'AvgP': lambda C_in, C_out, layer_id, kernel_size, stride: nn.AdaptiveAvgPool2d(1),
-    'FC': lambda C_in, C_out: nn.Linear(C_in, C_out),
-}
-
-
-class MixedOp(nn.Module):
-    def __init__(self, C_in, C_out, op_idx, layer_id, stride=1):
-        super(MixedOp, self).__init__()
-        self.layer_id = layer_id
-        self._op = OPS[PRIMITIVES[op_idx]](C_in, C_out, layer_id, stride)
-
-    def forward(self, x):
-        return self._op(x)
-
-
-class FBNet_Infer(nn.Module):
-    def __init__(self, config):
-        super(FBNet_Infer, self).__init__()
-
-        self.op_idx_list = config["op_idx_list"]
-        assert len(self.op_idx_list) == 22, (
-            "The length of op_idx_list should be 22, while it is {}".format(len(self.op_idx_list)))
-
-        self.num_classes = config["num_classes"]
-
-        self.num_layer_list = [1, 4, 4, 4, 4, 4, 1]  # FBNetv1 setting
-        self.num_channel_list = [16, 24, 32, 64, 112, 184, 352]  # FBNetv1 setting
-
-        if "cifar" in config["dataset"]:
-            self.stride_list = [1, 1, 2, 2, 1, 2, 1]  # FBNetv1 setting, unoffcial CIFAR-10/100 setting
-        else:
-            self.stride_list = [1, 2, 2, 2, 1, 2, 1]  # FBNetv1 setting, offcial ImageNet setting
-
-        self.stem_channel = 16  # FBNetv1 setting
-
-        if "cifar" in config["dataset"]:
-            self.header_channel = 1504  # FBNetv1 setting
-        else:
-            self.header_channel = 1984  # FBNetv1 setting
-
-        if "cifar" in config["dataset"]:
-            stride_init = 1
-        else:
-            stride_init = 2
-
-        self.stem = ConvNorm(3, self.stem_channel, kernel_size=3, stride=stride_init, padding=1, bias=False)
-
-        self.cells = nn.ModuleList()
-
-        layer_id = 1
-        for stage_id, num_layer in enumerate(self.num_layer_list):
-            for i in range(num_layer):
-                if i == 0:  # first Conv takes the stride into consideration
-                    if stage_id == 0:
-                        # The first block in the first stage will use stem_channel as input channel
-                        op = OPS[PRIMITIVES[self.op_idx_list[layer_id - 1]]](self.stem_channel,
-                                                                             self.num_channel_list[stage_id], layer_id,
-                                                                             self.stride_list[stage_id])
-                    else:
-                        op = OPS[PRIMITIVES[self.op_idx_list[layer_id - 1]]](self.num_channel_list[stage_id - 1],
-                                                                             self.num_channel_list[stage_id], layer_id,
-                                                                             self.stride_list[stage_id])
-                else:
-                    op = OPS[PRIMITIVES[self.op_idx_list[layer_id - 1]]](self.num_channel_list[stage_id],
-                                                                         self.num_channel_list[stage_id], layer_id,
-                                                                         stride=1)
-
-                layer_id += 1
-                self.cells.append(op)
-
-        self.header = ConvNorm(self.num_channel_list[-1], self.header_channel, kernel_size=1)
-
-        self.avgpool = nn.AdaptiveAvgPool2d(1)
-        self.fc = nn.Linear(self.header_channel, self.num_classes)
-        self.init_params()
-
-    def init_params(self):
-        for m in self.modules():
-            if isinstance(m, nn.Conv2d):
-                init.kaiming_normal_(m.weight, mode='fan_out')
-                if m.bias is not None:
-                    init.constant_(m.bias, 0)
-            elif isinstance(m, nn.BatchNorm2d):
-                init.constant_(m.weight, 1)
-                init.constant_(m.bias, 0)
-            elif isinstance(m, nn.Linear):
-                init.normal_(m.weight, std=0.001)
-                if m.bias is not None:
-                    init.constant_(m.bias, 0)
-
-    def forward(self, input):
-
-        out = self.stem(input)
-
-        for i, cell in enumerate(self.cells):
-            out = cell(out)
-
-        out = self.fc(self.avgpool(self.header(out)).view(out.size(0), -1))
-
-        return out
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+from torch.nn import init
+from torch.autograd import Variable
+import numpy as np
+
+
+class ChannelShuffle(nn.Module):
+    def __init__(self, groups):
+        super(ChannelShuffle, self).__init__()
+        self.groups = groups
+
+    def forward(self, x):
+        """Channel shuffle: [N,C,H,W] -> [N,g,C/g,H,W] -> [N,C/g,g,H,w] -> [N,C,H,W]"""
+        N, C, H, W = x.size()
+        g = self.groups
+        assert (
+                C % g == 0
+        ), "Incompatible group size {} for input channel {}".format(g, C)
+        return (
+            x.view(N, g, int(C / g), H, W)
+            .permute(0, 2, 1, 3, 4)
+            .contiguous()
+            .view(N, C, H, W)
+        )
+
+
+class ConvNorm(nn.Module):
+    '''
+    conv => norm => activation
+    use native Conv2d, not slimmable
+    '''
+
+    def __init__(self, C_in, C_out, kernel_size=3, stride=1, padding=None, dilation=1, groups=1, bias=False):
+        super(ConvNorm, self).__init__()
+        self.C_in = C_in
+        self.C_out = C_out
+
+        self.kernel_size = kernel_size
+        assert stride in [1, 2]
+        self.stride = stride
+        if padding is None:
+            # assume h_out = h_in / s
+            self.padding = int(np.ceil((dilation * (kernel_size - 1) + 1 - stride) / 2.))
+        else:
+            self.padding = padding
+        self.dilation = dilation
+        assert type(groups) == int
+        self.groups = groups
+        self.bias = bias
+
+        self.conv = nn.Conv2d(C_in, C_out, kernel_size=self.kernel_size, stride=self.stride, padding=self.padding,
+                              dilation=self.dilation, groups=self.groups, bias=bias)
+        self.bn = nn.BatchNorm2d(C_out)
+        self.relu = nn.ReLU(inplace=True)
+
+    def forward(self, x):
+        x = self.relu(self.bn(self.conv(x)))
+        return x
+
+
+class ConvBlock(nn.Module):
+    '''
+    conv => norm => activation
+    use native nn.Conv2d, not slimmable
+    '''
+
+    def __init__(self, C_in, C_out, layer_id, expansion=1, kernel_size=3, stride=1, padding=None, dilation=1, groups=1,
+                 bias=False):
+        super(ConvBlock, self).__init__()
+        self.C_in = C_in
+        self.C_out = C_out
+
+        self.layer_id = layer_id
+
+        assert type(expansion) == int
+        self.expansion = expansion
+        self.kernel_size = kernel_size
+        assert stride in [1, 2]
+        self.stride = stride
+        if padding is None:
+            # assume h_out = h_in / s
+            self.padding = int(np.ceil((dilation * (kernel_size - 1) + 1 - stride) / 2.))
+        else:
+            self.padding = padding
+        self.dilation = dilation
+        assert type(groups) == int
+        self.groups = groups
+        self.bias = bias
+
+        if self.groups > 1:
+            self.shuffle = ChannelShuffle(self.groups)
+
+        self.conv1 = nn.Conv2d(C_in, C_in * expansion, kernel_size=1, stride=1, padding=0, dilation=1,
+                               groups=self.groups, bias=bias)
+        self.bn1 = nn.BatchNorm2d(C_in * expansion)
+
+        self.conv2 = nn.Conv2d(C_in * expansion, C_in * expansion, kernel_size=self.kernel_size, stride=self.stride,
+                               padding=self.padding, dilation=1, groups=C_in * expansion, bias=bias)
+        self.bn2 = nn.BatchNorm2d(C_in * expansion)
+
+        self.conv3 = nn.Conv2d(C_in * expansion, C_out, kernel_size=1, stride=1, padding=0, dilation=1,
+                               groups=self.groups, bias=bias)
+        self.bn3 = nn.BatchNorm2d(C_out)
+
+        self.nl = nn.ReLU(inplace=True)
+
+    # beta, mode, act_num, beta_param are for bit-widths search
+    def forward(self, x):
+
+        identity = x
+        x = self.nl(self.bn1(self.conv1(x)))
+
+        if self.groups > 1:
+            x = self.shuffle(x)
+
+        x = self.nl(self.bn2(self.conv2(x)))
+
+        x = self.bn3(self.conv3(x))
+
+        if self.C_in == self.C_out and self.stride == 1:
+            x += identity
+
+        return x
+
+
+class Skip(nn.Module):
+    def __init__(self, C_in, C_out, layer_id, stride=1):
+        super(Skip, self).__init__()
+        assert stride in [1, 2]
+        assert C_out % 2 == 0, 'C_out=%d' % C_out
+        self.C_in = C_in
+        self.C_out = C_out
+        self.stride = stride
+
+        self.layer_id = layer_id
+
+        self.kernel_size = 1
+        self.padding = 0
+
+        if stride == 2 or C_in != C_out:
+            self.conv = nn.Conv2d(C_in, C_out, 1, stride=stride, padding=0, bias=False)
+            self.bn = nn.BatchNorm2d(C_out)
+            self.relu = nn.ReLU(inplace=True)
+
+    def forward(self, x):
+        if hasattr(self, 'conv'):
+            out = self.conv(x)
+            out = self.bn(out)
+            out = self.relu(out)
+        else:
+            out = x
+
+        return out
+
+
+# The 9 blocks in FBNet Space
+PRIMITIVES = [
+    'k3_e1',
+    'k3_e1_g2',
+    'k3_e3',
+    'k3_e6',
+    'k5_e1',
+    'k5_e1_g2',
+    'k5_e3',
+    'k5_e6',
+    'skip'
+]
+
+OPS = {
+    'k3_e1': lambda C_in, C_out, layer_id, stride: ConvBlock(C_in, C_out, layer_id, expansion=1, kernel_size=3,
+                                                             stride=stride, groups=1),
+    'k3_e1_g2': lambda C_in, C_out, layer_id, stride: ConvBlock(C_in, C_out, layer_id, expansion=1, kernel_size=3,
+                                                                stride=stride, groups=2),
+    'k3_e3': lambda C_in, C_out, layer_id, stride: ConvBlock(C_in, C_out, layer_id, expansion=3, kernel_size=3,
+                                                             stride=stride, groups=1),
+    'k3_e6': lambda C_in, C_out, layer_id, stride: ConvBlock(C_in, C_out, layer_id, expansion=6, kernel_size=3,
+                                                             stride=stride, groups=1),
+    'k5_e1': lambda C_in, C_out, layer_id, stride: ConvBlock(C_in, C_out, layer_id, expansion=1, kernel_size=5,
+                                                             stride=stride, groups=1),
+    'k5_e1_g2': lambda C_in, C_out, layer_id, stride: ConvBlock(C_in, C_out, layer_id, expansion=1, kernel_size=5,
+                                                                stride=stride, groups=2),
+    'k5_e3': lambda C_in, C_out, layer_id, stride: ConvBlock(C_in, C_out, layer_id, expansion=3, kernel_size=5,
+                                                             stride=stride, groups=1),
+    'k5_e6': lambda C_in, C_out, layer_id, stride: ConvBlock(C_in, C_out, layer_id, expansion=6, kernel_size=5,
+                                                             stride=stride, groups=1),
+    'skip': lambda C_in, C_out, layer_id, stride: Skip(C_in, C_out, layer_id, stride)
+}
+
+AUX_OPS = {
+    'ConvNorm': lambda C_in, C_out, layer_id, kernel_size, stride: ConvBlock(C_in, C_out, layer_id,
+                                                                             kernel_size=kernel_size, stride=stride),
+    'AvgP': lambda C_in, C_out, layer_id, kernel_size, stride: nn.AdaptiveAvgPool2d(1),
+    'FC': lambda C_in, C_out: nn.Linear(C_in, C_out),
+}
+
+
+class MixedOp(nn.Module):
+    def __init__(self, C_in, C_out, op_idx, layer_id, stride=1):
+        super(MixedOp, self).__init__()
+        self.layer_id = layer_id
+        self._op = OPS[PRIMITIVES[op_idx]](C_in, C_out, layer_id, stride)
+
+    def forward(self, x):
+        return self._op(x)
+
+
+class FBNet_Infer(nn.Module):
+    def __init__(self, config):
+        super(FBNet_Infer, self).__init__()
+
+        self.op_idx_list = config["op_idx_list"]
+        assert len(self.op_idx_list) == 22, (
+            "The length of op_idx_list should be 22, while it is {}".format(len(self.op_idx_list)))
+
+        self.num_classes = config["num_classes"]
+
+        self.num_layer_list = [1, 4, 4, 4, 4, 4, 1]  # FBNetv1 setting
+        self.num_channel_list = [16, 24, 32, 64, 112, 184, 352]  # FBNetv1 setting
+
+        if "cifar" in config["dataset"]:
+            self.stride_list = [1, 1, 2, 2, 1, 2, 1]  # FBNetv1 setting, unoffcial CIFAR-10/100 setting
+        else:
+            self.stride_list = [1, 2, 2, 2, 1, 2, 1]  # FBNetv1 setting, offcial ImageNet setting
+
+        self.stem_channel = 16  # FBNetv1 setting
+
+        if "cifar" in config["dataset"]:
+            self.header_channel = 1504  # FBNetv1 setting
+        else:
+            self.header_channel = 1984  # FBNetv1 setting
+
+        if "cifar" in config["dataset"]:
+            stride_init = 1
+        else:
+            stride_init = 2
+
+        self.stem = ConvNorm(3, self.stem_channel, kernel_size=3, stride=stride_init, padding=1, bias=False)
+
+        self.cells = nn.ModuleList()
+
+        layer_id = 1
+        for stage_id, num_layer in enumerate(self.num_layer_list):
+            for i in range(num_layer):
+                if i == 0:  # first Conv takes the stride into consideration
+                    if stage_id == 0:
+                        # The first block in the first stage will use stem_channel as input channel
+                        op = OPS[PRIMITIVES[self.op_idx_list[layer_id - 1]]](self.stem_channel,
+                                                                             self.num_channel_list[stage_id], layer_id,
+                                                                             self.stride_list[stage_id])
+                    else:
+                        op = OPS[PRIMITIVES[self.op_idx_list[layer_id - 1]]](self.num_channel_list[stage_id - 1],
+                                                                             self.num_channel_list[stage_id], layer_id,
+                                                                             self.stride_list[stage_id])
+                else:
+                    op = OPS[PRIMITIVES[self.op_idx_list[layer_id - 1]]](self.num_channel_list[stage_id],
+                                                                         self.num_channel_list[stage_id], layer_id,
+                                                                         stride=1)
+
+                layer_id += 1
+                self.cells.append(op)
+
+        self.header = ConvNorm(self.num_channel_list[-1], self.header_channel, kernel_size=1)
+
+        self.avgpool = nn.AdaptiveAvgPool2d(1)
+        self.fc = nn.Linear(self.header_channel, self.num_classes)
+        self.init_params()
+
+    def init_params(self):
+        for m in self.modules():
+            if isinstance(m, nn.Conv2d):
+                init.kaiming_normal_(m.weight, mode='fan_out')
+                if m.bias is not None:
+                    init.constant_(m.bias, 0)
+            elif isinstance(m, nn.BatchNorm2d):
+                init.constant_(m.weight, 1)
+                init.constant_(m.bias, 0)
+            elif isinstance(m, nn.Linear):
+                init.normal_(m.weight, std=0.001)
+                if m.bias is not None:
+                    init.constant_(m.bias, 0)
+
+    def forward(self, input):
+
+        out = self.stem(input)
+
+        for i, cell in enumerate(self.cells):
+            out = cell(out)
+
+        out = self.fc(self.avgpool(self.header(out)).view(out.size(0), -1))
+
+        return out
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/hw_nas_bench_api.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/hw_nas_bench_api.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,260 +1,260 @@
-import pickle
-
-"""
-This is the class for the API for HW-NAS-Bench
-"""
-
-
-class HWNASBenchAPI():
-    def __init__(self, file_path_or_dict, search_space="nasbench201"):
-        # Load the pickle file containing all the Hardware metrics
-        with open(file_path_or_dict, 'rb') as f:
-            self.HW_metrics = pickle.load(f)
-        self.search_space = search_space
-
-    def query_by_index(self, arch_index, dataname):
-        if self.search_space == "nasbench201":
-            metrics_list = ["edgegpu_latency",
-                            "edgegpu_energy",
-                            "raspi4_latency",
-                            "edgetpu_latency",
-                            "pixel3_latency",
-                            "eyeriss_latency",
-                            "eyeriss_energy",
-                            "eyeriss_arithmetic_intensity",
-                            "fpga_latency",
-                            "fpga_energy",
-                            ]
-            results = {}
-            for metric_name in metrics_list:
-                results[metric_name] = float(self.HW_metrics[self.search_space][dataname][metric_name][arch_index])
-
-            # for 'average_hw_metric'
-            results['average_hw_metric'] = results["edgegpu_latency"] * results["edgegpu_energy"] * results[
-                "raspi4_latency"] * results["edgetpu_latency"] * results["pixel3_latency"] * results[
-                                               "eyeriss_latency"] * results["eyeriss_energy"] * results[
-                                               "fpga_latency"] * results["fpga_energy"]
-
-            return results
-        elif self.search_space == "fbnet":
-            metrics_list = ["edgegpu_latency",
-                            "edgegpu_energy",
-                            "raspi4_latency",
-                            "pixel3_latency",
-                            "eyeriss_latency",
-                            "eyeriss_energy",
-                            "fpga_latency",
-                            "fpga_energy",
-                            ]
-            results = {}
-            for metric_name in metrics_list:
-                lookup_table = self.HW_metrics[self.search_space][metric_name]
-                results[metric_name] = fbnet_get_metrics(arch_index, dataname, lookup_table)
-
-            # for 'average_hw_metric'
-            results['average_hw_metric'] = results["edgegpu_latency"] * results["edgegpu_energy"] * results[
-                "raspi4_latency"] * results["pixel3_latency"] * results["eyeriss_latency"] * results["eyeriss_energy"] * \
-                                           results["fpga_latency"] * results["fpga_energy"]
-
-            return results
-        else:
-            print("Wrong dataset name, expect: {} and {}, while receive: {}",
-                  format("nasbench201", "fbnet", self.search_space))
-
-    def get_net_config(self, arch_index, dataname):
-        if self.search_space == "nasbench201":
-            config = self.HW_metrics[self.search_space][dataname]["config"][arch_index]
-            return config
-        elif self.search_space == "fbnet":
-            ops_str_lookup_table = ["k3_e1", "k3_e1_g2", "k3_e3",
-                                    "k3_e6", "k5_e1", "k5_e1_g2",
-                                    "k5_e3", "k5_e6", "skip"]
-            assert dataname in ["cifar100", "ImageNet"], (
-                "Only {} and {} are allowed to be datasets in FBNet space, while receive {}".format("cifar100",
-                                                                                                    "ImageNet",
-                                                                                                    dataname))
-            if dataname == "cifar100":
-                num_classes = 100
-            else:
-                num_classes = 1000  # ImageNet
-            arch_str = [ops_str_lookup_table[v] for v in arch_index]
-            config = {"dataset": dataname, "num_classes": num_classes, "op_idx_list": arch_index, "arch_str": arch_str}
-            return config
-        else:
-            print("Wrong dataset name, expect: {} and {}, while receive: {}",
-                  format("nasbench201", "fbnet", self.search_space))
-
-    def get_op_lookup_tables(self):
-        if self.search_space == "fbnet":
-            lookup_tables = {}
-            metrics_list = ["edgegpu_latency",
-                            "edgegpu_energy",
-                            "raspi4_latency",
-                            "pixel3_latency",
-                            "eyeriss_latency",
-                            "eyeriss_energy",
-                            "fpga_latency",
-                            "fpga_energy",
-                            ]
-            results = {}
-            for metric_name in metrics_list:
-                lookup_table = self.HW_metrics[self.search_space][metric_name]
-                lookup_tables[metric_name] = lookup_table
-            return lookup_tables
-        else:
-            print("Wrong dataset name, expect: {} and {}, while receive: {}",
-                  format("nasbench201", "fbnet", self.search_space))
-
-
-def fbnet_get_metrics(arch_index, dataname, lookup_table):
-    # Receive arch_index (a list format), dataname ("cifar100", "ImageNet"), and an lookup_table
-    assert type(arch_index) == list, (
-        "The type of arch_index should be a list in FBNet space, while receive {}".format(type(arch_index)))
-    assert len(arch_index) == 22, (
-        "The length of arch_index should be 22 in FBNet space, while receive {}".format(len(arch_index)))
-    assert dataname in ["cifar100", "ImageNet"], (
-        "Only {} and {} are allowed to be datasets in FBNet space, while receive {}".format("cifar100", "ImageNet",
-                                                                                            dataname))
-
-    # Architecture settings in FBNet space
-    op_idx_list = arch_index
-    OP_metrics_dict = lookup_table
-
-    stem_channel = 16
-    num_layer_list = [1, 4, 4, 4, 4, 4, 1]
-    num_channel_list = [16, 24, 32, 64, 112, 184, 352]
-
-    ConvBlock_list = []
-    ConvBlock_list.append({"exp": 1, "kernel": 3, "group": 1})
-    ConvBlock_list.append({"exp": 1, "kernel": 3, "group": 2})
-    ConvBlock_list.append({"exp": 3, "kernel": 3, "group": 1})
-    ConvBlock_list.append({"exp": 6, "kernel": 3, "group": 1})
-    ConvBlock_list.append({"exp": 1, "kernel": 5, "group": 1})
-    ConvBlock_list.append({"exp": 1, "kernel": 5, "group": 2})
-    ConvBlock_list.append({"exp": 3, "kernel": 5, "group": 1})
-    ConvBlock_list.append({"exp": 6, "kernel": 5, "group": 1})
-
-    if dataname == "cifar100":
-        num_classes = 100
-        stride_list = [1, 1, 2, 2, 1, 2, 1]
-        header_channel = 1504  # FBNetv1 setting
-        stride_init = 1
-        H_W = 32
-    else:
-        num_classes = 1000  # ImageNet
-        stride_list = [1, 2, 2, 2, 1, 2, 1]  # FBNetv1 setting, offcial ImageNet setting
-        header_channel = 1984  # FBNetv1 setting
-        stride_init = 2
-        H_W = 224
-
-    metric = 0.0
-
-    # Add STEM cost
-    metric += OP_metrics_dict["ConvNorm_H{}_W{}_Cin{}_Cout{}_kernel{}_stride{}_group{}".format(
-        H_W,
-        H_W,
-        3,
-        stem_channel,
-        3,
-        stride_init,
-        1,
-    )]
-    H_W = H_W // stride_init  # Downsample size due to stride
-    # Add Cells cost
-    layer_id = 0
-    for stage_id, num_layer in enumerate(num_layer_list):
-        for i in range(num_layer):
-            layer_op_idx = op_idx_list[layer_id]
-            if i == 0:  # first Conv takes the stride into consideration
-                if stage_id == 0:
-                    # The first block in the first stage will use stem_channel as input channel
-                    if layer_op_idx < 8:  # ConvBlock
-                        metric += OP_metrics_dict[
-                            "ConvBlock_H{}_W{}_Cin{}_Cout{}_exp{}_kernel{}_stride{}_group{}".format(
-                                H_W,
-                                H_W,
-                                stem_channel,
-                                num_channel_list[stage_id],
-                                ConvBlock_list[layer_op_idx]["exp"],
-                                ConvBlock_list[layer_op_idx]["kernel"],
-                                stride_list[stage_id],
-                                ConvBlock_list[layer_op_idx]["group"],
-                            )]
-                    else:  # Skip connection
-                        metric += OP_metrics_dict["Skip_H{}_W{}_Cin{}_Cout{}_stride{}".format(
-                            H_W,
-                            H_W,
-                            stem_channel,
-                            num_channel_list[stage_id],
-                            stride_list[stage_id]
-                        )]
-                else:
-                    if layer_op_idx < 8:  # ConvBlock
-                        metric += OP_metrics_dict[
-                            "ConvBlock_H{}_W{}_Cin{}_Cout{}_exp{}_kernel{}_stride{}_group{}".format(
-                                H_W,
-                                H_W,
-                                num_channel_list[stage_id - 1],
-                                num_channel_list[stage_id],
-                                ConvBlock_list[layer_op_idx]["exp"],
-                                ConvBlock_list[layer_op_idx]["kernel"],
-                                stride_list[stage_id],
-                                ConvBlock_list[layer_op_idx]["group"],
-                            )]
-                    else:  # Skip connection
-                        metric += OP_metrics_dict["Skip_H{}_W{}_Cin{}_Cout{}_stride{}".format(
-                            H_W,
-                            H_W,
-                            num_channel_list[stage_id - 1],
-                            num_channel_list[stage_id],
-                            stride_list[stage_id]
-                        )]
-                H_W = H_W // stride_list[stage_id]  # Downsample size due to stride
-            else:
-                if layer_op_idx < 8:  # ConvBlock
-                    metric += OP_metrics_dict["ConvBlock_H{}_W{}_Cin{}_Cout{}_exp{}_kernel{}_stride{}_group{}".format(
-                        H_W,
-                        H_W,
-                        num_channel_list[stage_id],
-                        num_channel_list[stage_id],
-                        ConvBlock_list[layer_op_idx]["exp"],
-                        ConvBlock_list[layer_op_idx]["kernel"],
-                        1,
-                        ConvBlock_list[layer_op_idx]["group"],
-                    )]
-                else:  # Skip connection
-                    metric += OP_metrics_dict["Skip_H{}_W{}_Cin{}_Cout{}_stride{}".format(
-                        H_W,
-                        H_W,
-                        num_channel_list[stage_id],
-                        num_channel_list[stage_id],
-                        1
-                    )]
-                # no downsample size because of stride = 1
-            layer_id += 1
-    # Add Header cost
-    metric += OP_metrics_dict["ConvNorm_H{}_W{}_Cin{}_Cout{}_kernel{}_stride{}_group{}".format(
-        H_W,
-        H_W,
-        num_channel_list[-1],
-        header_channel,
-        1,
-        1,
-        1,
-    )]
-    # Add AvgP cost
-    metric += OP_metrics_dict["AvgP_H{}_W{}_Cin{}_Cout{}_kernel{}_stride{}".format(
-        H_W,
-        H_W,
-        header_channel,
-        header_channel,
-        H_W,
-        1,
-    )]
-    # Add FC cost
-    metric += OP_metrics_dict["FC_Cin{}_Cout{}".format(
-        header_channel,
-        num_classes,
-    )]
-
-    return metric
+import pickle
+
+"""
+This is the class for the API for HW-NAS-Bench
+"""
+
+
+class HWNASBenchAPI():
+    def __init__(self, file_path_or_dict, search_space="nasbench201"):
+        # Load the pickle file containing all the Hardware metrics
+        with open(file_path_or_dict, 'rb') as f:
+            self.HW_metrics = pickle.load(f)
+        self.search_space = search_space
+
+    def query_by_index(self, arch_index, dataname):
+        if self.search_space == "nasbench201":
+            metrics_list = ["edgegpu_latency",
+                            "edgegpu_energy",
+                            "raspi4_latency",
+                            "edgetpu_latency",
+                            "pixel3_latency",
+                            "eyeriss_latency",
+                            "eyeriss_energy",
+                            "eyeriss_arithmetic_intensity",
+                            "fpga_latency",
+                            "fpga_energy",
+                            ]
+            results = {}
+            for metric_name in metrics_list:
+                results[metric_name] = float(self.HW_metrics[self.search_space][dataname][metric_name][arch_index])
+
+            # for 'average_hw_metric'
+            results['average_hw_metric'] = results["edgegpu_latency"] * results["edgegpu_energy"] * results[
+                "raspi4_latency"] * results["edgetpu_latency"] * results["pixel3_latency"] * results[
+                                               "eyeriss_latency"] * results["eyeriss_energy"] * results[
+                                               "fpga_latency"] * results["fpga_energy"]
+
+            return results
+        elif self.search_space == "fbnet":
+            metrics_list = ["edgegpu_latency",
+                            "edgegpu_energy",
+                            "raspi4_latency",
+                            "pixel3_latency",
+                            "eyeriss_latency",
+                            "eyeriss_energy",
+                            "fpga_latency",
+                            "fpga_energy",
+                            ]
+            results = {}
+            for metric_name in metrics_list:
+                lookup_table = self.HW_metrics[self.search_space][metric_name]
+                results[metric_name] = fbnet_get_metrics(arch_index, dataname, lookup_table)
+
+            # for 'average_hw_metric'
+            results['average_hw_metric'] = results["edgegpu_latency"] * results["edgegpu_energy"] * results[
+                "raspi4_latency"] * results["pixel3_latency"] * results["eyeriss_latency"] * results["eyeriss_energy"] * \
+                                           results["fpga_latency"] * results["fpga_energy"]
+
+            return results
+        else:
+            print("Wrong dataset name, expect: {} and {}, while receive: {}",
+                  format("nasbench201", "fbnet", self.search_space))
+
+    def get_net_config(self, arch_index, dataname):
+        if self.search_space == "nasbench201":
+            config = self.HW_metrics[self.search_space][dataname]["config"][arch_index]
+            return config
+        elif self.search_space == "fbnet":
+            ops_str_lookup_table = ["k3_e1", "k3_e1_g2", "k3_e3",
+                                    "k3_e6", "k5_e1", "k5_e1_g2",
+                                    "k5_e3", "k5_e6", "skip"]
+            assert dataname in ["cifar100", "ImageNet"], (
+                "Only {} and {} are allowed to be datasets in FBNet space, while receive {}".format("cifar100",
+                                                                                                    "ImageNet",
+                                                                                                    dataname))
+            if dataname == "cifar100":
+                num_classes = 100
+            else:
+                num_classes = 1000  # ImageNet
+            arch_str = [ops_str_lookup_table[v] for v in arch_index]
+            config = {"dataset": dataname, "num_classes": num_classes, "op_idx_list": arch_index, "arch_str": arch_str}
+            return config
+        else:
+            print("Wrong dataset name, expect: {} and {}, while receive: {}",
+                  format("nasbench201", "fbnet", self.search_space))
+
+    def get_op_lookup_tables(self):
+        if self.search_space == "fbnet":
+            lookup_tables = {}
+            metrics_list = ["edgegpu_latency",
+                            "edgegpu_energy",
+                            "raspi4_latency",
+                            "pixel3_latency",
+                            "eyeriss_latency",
+                            "eyeriss_energy",
+                            "fpga_latency",
+                            "fpga_energy",
+                            ]
+            results = {}
+            for metric_name in metrics_list:
+                lookup_table = self.HW_metrics[self.search_space][metric_name]
+                lookup_tables[metric_name] = lookup_table
+            return lookup_tables
+        else:
+            print("Wrong dataset name, expect: {} and {}, while receive: {}",
+                  format("nasbench201", "fbnet", self.search_space))
+
+
+def fbnet_get_metrics(arch_index, dataname, lookup_table):
+    # Receive arch_index (a list format), dataname ("cifar100", "ImageNet"), and an lookup_table
+    assert type(arch_index) == list, (
+        "The type of arch_index should be a list in FBNet space, while receive {}".format(type(arch_index)))
+    assert len(arch_index) == 22, (
+        "The length of arch_index should be 22 in FBNet space, while receive {}".format(len(arch_index)))
+    assert dataname in ["cifar100", "ImageNet"], (
+        "Only {} and {} are allowed to be datasets in FBNet space, while receive {}".format("cifar100", "ImageNet",
+                                                                                            dataname))
+
+    # Architecture settings in FBNet space
+    op_idx_list = arch_index
+    OP_metrics_dict = lookup_table
+
+    stem_channel = 16
+    num_layer_list = [1, 4, 4, 4, 4, 4, 1]
+    num_channel_list = [16, 24, 32, 64, 112, 184, 352]
+
+    ConvBlock_list = []
+    ConvBlock_list.append({"exp": 1, "kernel": 3, "group": 1})
+    ConvBlock_list.append({"exp": 1, "kernel": 3, "group": 2})
+    ConvBlock_list.append({"exp": 3, "kernel": 3, "group": 1})
+    ConvBlock_list.append({"exp": 6, "kernel": 3, "group": 1})
+    ConvBlock_list.append({"exp": 1, "kernel": 5, "group": 1})
+    ConvBlock_list.append({"exp": 1, "kernel": 5, "group": 2})
+    ConvBlock_list.append({"exp": 3, "kernel": 5, "group": 1})
+    ConvBlock_list.append({"exp": 6, "kernel": 5, "group": 1})
+
+    if dataname == "cifar100":
+        num_classes = 100
+        stride_list = [1, 1, 2, 2, 1, 2, 1]
+        header_channel = 1504  # FBNetv1 setting
+        stride_init = 1
+        H_W = 32
+    else:
+        num_classes = 1000  # ImageNet
+        stride_list = [1, 2, 2, 2, 1, 2, 1]  # FBNetv1 setting, offcial ImageNet setting
+        header_channel = 1984  # FBNetv1 setting
+        stride_init = 2
+        H_W = 224
+
+    metric = 0.0
+
+    # Add STEM cost
+    metric += OP_metrics_dict["ConvNorm_H{}_W{}_Cin{}_Cout{}_kernel{}_stride{}_group{}".format(
+        H_W,
+        H_W,
+        3,
+        stem_channel,
+        3,
+        stride_init,
+        1,
+    )]
+    H_W = H_W // stride_init  # Downsample size due to stride
+    # Add Cells cost
+    layer_id = 0
+    for stage_id, num_layer in enumerate(num_layer_list):
+        for i in range(num_layer):
+            layer_op_idx = op_idx_list[layer_id]
+            if i == 0:  # first Conv takes the stride into consideration
+                if stage_id == 0:
+                    # The first block in the first stage will use stem_channel as input channel
+                    if layer_op_idx < 8:  # ConvBlock
+                        metric += OP_metrics_dict[
+                            "ConvBlock_H{}_W{}_Cin{}_Cout{}_exp{}_kernel{}_stride{}_group{}".format(
+                                H_W,
+                                H_W,
+                                stem_channel,
+                                num_channel_list[stage_id],
+                                ConvBlock_list[layer_op_idx]["exp"],
+                                ConvBlock_list[layer_op_idx]["kernel"],
+                                stride_list[stage_id],
+                                ConvBlock_list[layer_op_idx]["group"],
+                            )]
+                    else:  # Skip connection
+                        metric += OP_metrics_dict["Skip_H{}_W{}_Cin{}_Cout{}_stride{}".format(
+                            H_W,
+                            H_W,
+                            stem_channel,
+                            num_channel_list[stage_id],
+                            stride_list[stage_id]
+                        )]
+                else:
+                    if layer_op_idx < 8:  # ConvBlock
+                        metric += OP_metrics_dict[
+                            "ConvBlock_H{}_W{}_Cin{}_Cout{}_exp{}_kernel{}_stride{}_group{}".format(
+                                H_W,
+                                H_W,
+                                num_channel_list[stage_id - 1],
+                                num_channel_list[stage_id],
+                                ConvBlock_list[layer_op_idx]["exp"],
+                                ConvBlock_list[layer_op_idx]["kernel"],
+                                stride_list[stage_id],
+                                ConvBlock_list[layer_op_idx]["group"],
+                            )]
+                    else:  # Skip connection
+                        metric += OP_metrics_dict["Skip_H{}_W{}_Cin{}_Cout{}_stride{}".format(
+                            H_W,
+                            H_W,
+                            num_channel_list[stage_id - 1],
+                            num_channel_list[stage_id],
+                            stride_list[stage_id]
+                        )]
+                H_W = H_W // stride_list[stage_id]  # Downsample size due to stride
+            else:
+                if layer_op_idx < 8:  # ConvBlock
+                    metric += OP_metrics_dict["ConvBlock_H{}_W{}_Cin{}_Cout{}_exp{}_kernel{}_stride{}_group{}".format(
+                        H_W,
+                        H_W,
+                        num_channel_list[stage_id],
+                        num_channel_list[stage_id],
+                        ConvBlock_list[layer_op_idx]["exp"],
+                        ConvBlock_list[layer_op_idx]["kernel"],
+                        1,
+                        ConvBlock_list[layer_op_idx]["group"],
+                    )]
+                else:  # Skip connection
+                    metric += OP_metrics_dict["Skip_H{}_W{}_Cin{}_Cout{}_stride{}".format(
+                        H_W,
+                        H_W,
+                        num_channel_list[stage_id],
+                        num_channel_list[stage_id],
+                        1
+                    )]
+                # no downsample size because of stride = 1
+            layer_id += 1
+    # Add Header cost
+    metric += OP_metrics_dict["ConvNorm_H{}_W{}_Cin{}_Cout{}_kernel{}_stride{}_group{}".format(
+        H_W,
+        H_W,
+        num_channel_list[-1],
+        header_channel,
+        1,
+        1,
+        1,
+    )]
+    # Add AvgP cost
+    metric += OP_metrics_dict["AvgP_H{}_W{}_Cin{}_Cout{}_kernel{}_stride{}".format(
+        H_W,
+        H_W,
+        header_channel,
+        header_channel,
+        H_W,
+        1,
+    )]
+    # Add FC cost
+    metric += OP_metrics_dict["FC_Cin{}_Cout{}".format(
+        header_channel,
+        num_classes,
+    )]
+
+    return metric
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/CifarDenseNet.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/CifarDenseNet.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-##################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
-##################################################
-import math, torch
-import torch.nn as nn
-import torch.nn.functional as F
-from .initialization import initialize_resnet
-
-
-class Bottleneck(nn.Module):
-    def __init__(self, nChannels, growthRate):
-        super(Bottleneck, self).__init__()
-        interChannels = 4 * growthRate
-        self.bn1 = nn.BatchNorm2d(nChannels)
-        self.conv1 = nn.Conv2d(nChannels, interChannels, kernel_size=1, bias=False)
-        self.bn2 = nn.BatchNorm2d(interChannels)
-        self.conv2 = nn.Conv2d(interChannels, growthRate, kernel_size=3, padding=1, bias=False)
-
-    def forward(self, x):
-        out = self.conv1(F.relu(self.bn1(x)))
-        out = self.conv2(F.relu(self.bn2(out)))
-        out = torch.cat((x, out), 1)
-        return out
-
-
-class SingleLayer(nn.Module):
-    def __init__(self, nChannels, growthRate):
-        super(SingleLayer, self).__init__()
-        self.bn1 = nn.BatchNorm2d(nChannels)
-        self.conv1 = nn.Conv2d(nChannels, growthRate, kernel_size=3, padding=1, bias=False)
-
-    def forward(self, x):
-        out = self.conv1(F.relu(self.bn1(x)))
-        out = torch.cat((x, out), 1)
-        return out
-
-
-class Transition(nn.Module):
-    def __init__(self, nChannels, nOutChannels):
-        super(Transition, self).__init__()
-        self.bn1 = nn.BatchNorm2d(nChannels)
-        self.conv1 = nn.Conv2d(nChannels, nOutChannels, kernel_size=1, bias=False)
-
-    def forward(self, x):
-        out = self.conv1(F.relu(self.bn1(x)))
-        out = F.avg_pool2d(out, 2)
-        return out
-
-
-class DenseNet(nn.Module):
-    def __init__(self, growthRate, depth, reduction, nClasses, bottleneck):
-        super(DenseNet, self).__init__()
-
-        if bottleneck:
-            nDenseBlocks = int((depth - 4) / 6)
-        else:
-            nDenseBlocks = int((depth - 4) / 3)
-
-        self.message = 'CifarDenseNet : block : {:}, depth : {:}, reduction : {:}, growth-rate = {:}, class = {:}'.format(
-            'bottleneck' if bottleneck else 'basic', depth, reduction, growthRate, nClasses)
-
-        nChannels = 2 * growthRate
-        self.conv1 = nn.Conv2d(3, nChannels, kernel_size=3, padding=1, bias=False)
-
-        self.dense1 = self._make_dense(nChannels, growthRate, nDenseBlocks, bottleneck)
-        nChannels += nDenseBlocks * growthRate
-        nOutChannels = int(math.floor(nChannels * reduction))
-        self.trans1 = Transition(nChannels, nOutChannels)
-
-        nChannels = nOutChannels
-        self.dense2 = self._make_dense(nChannels, growthRate, nDenseBlocks, bottleneck)
-        nChannels += nDenseBlocks * growthRate
-        nOutChannels = int(math.floor(nChannels * reduction))
-        self.trans2 = Transition(nChannels, nOutChannels)
-
-        nChannels = nOutChannels
-        self.dense3 = self._make_dense(nChannels, growthRate, nDenseBlocks, bottleneck)
-        nChannels += nDenseBlocks * growthRate
-
-        self.act = nn.Sequential(
-            nn.BatchNorm2d(nChannels), nn.ReLU(inplace=True),
-            nn.AvgPool2d(8))
-        self.fc = nn.Linear(nChannels, nClasses)
-
-        self.apply(initialize_resnet)
-
-    def get_message(self):
-        return self.message
-
-    def _make_dense(self, nChannels, growthRate, nDenseBlocks, bottleneck):
-        layers = []
-        for i in range(int(nDenseBlocks)):
-            if bottleneck:
-                layers.append(Bottleneck(nChannels, growthRate))
-            else:
-                layers.append(SingleLayer(nChannels, growthRate))
-            nChannels += growthRate
-        return nn.Sequential(*layers)
-
-    def forward(self, inputs):
-        out = self.conv1(inputs)
-        out = self.trans1(self.dense1(out))
-        out = self.trans2(self.dense2(out))
-        out = self.dense3(out)
-        features = self.act(out)
-        features = features.view(features.size(0), -1)
-        out = self.fc(features)
-        return features, out
+##################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
+##################################################
+import math, torch
+import torch.nn as nn
+import torch.nn.functional as F
+from .initialization import initialize_resnet
+
+
+class Bottleneck(nn.Module):
+    def __init__(self, nChannels, growthRate):
+        super(Bottleneck, self).__init__()
+        interChannels = 4 * growthRate
+        self.bn1 = nn.BatchNorm2d(nChannels)
+        self.conv1 = nn.Conv2d(nChannels, interChannels, kernel_size=1, bias=False)
+        self.bn2 = nn.BatchNorm2d(interChannels)
+        self.conv2 = nn.Conv2d(interChannels, growthRate, kernel_size=3, padding=1, bias=False)
+
+    def forward(self, x):
+        out = self.conv1(F.relu(self.bn1(x)))
+        out = self.conv2(F.relu(self.bn2(out)))
+        out = torch.cat((x, out), 1)
+        return out
+
+
+class SingleLayer(nn.Module):
+    def __init__(self, nChannels, growthRate):
+        super(SingleLayer, self).__init__()
+        self.bn1 = nn.BatchNorm2d(nChannels)
+        self.conv1 = nn.Conv2d(nChannels, growthRate, kernel_size=3, padding=1, bias=False)
+
+    def forward(self, x):
+        out = self.conv1(F.relu(self.bn1(x)))
+        out = torch.cat((x, out), 1)
+        return out
+
+
+class Transition(nn.Module):
+    def __init__(self, nChannels, nOutChannels):
+        super(Transition, self).__init__()
+        self.bn1 = nn.BatchNorm2d(nChannels)
+        self.conv1 = nn.Conv2d(nChannels, nOutChannels, kernel_size=1, bias=False)
+
+    def forward(self, x):
+        out = self.conv1(F.relu(self.bn1(x)))
+        out = F.avg_pool2d(out, 2)
+        return out
+
+
+class DenseNet(nn.Module):
+    def __init__(self, growthRate, depth, reduction, nClasses, bottleneck):
+        super(DenseNet, self).__init__()
+
+        if bottleneck:
+            nDenseBlocks = int((depth - 4) / 6)
+        else:
+            nDenseBlocks = int((depth - 4) / 3)
+
+        self.message = 'CifarDenseNet : block : {:}, depth : {:}, reduction : {:}, growth-rate = {:}, class = {:}'.format(
+            'bottleneck' if bottleneck else 'basic', depth, reduction, growthRate, nClasses)
+
+        nChannels = 2 * growthRate
+        self.conv1 = nn.Conv2d(3, nChannels, kernel_size=3, padding=1, bias=False)
+
+        self.dense1 = self._make_dense(nChannels, growthRate, nDenseBlocks, bottleneck)
+        nChannels += nDenseBlocks * growthRate
+        nOutChannels = int(math.floor(nChannels * reduction))
+        self.trans1 = Transition(nChannels, nOutChannels)
+
+        nChannels = nOutChannels
+        self.dense2 = self._make_dense(nChannels, growthRate, nDenseBlocks, bottleneck)
+        nChannels += nDenseBlocks * growthRate
+        nOutChannels = int(math.floor(nChannels * reduction))
+        self.trans2 = Transition(nChannels, nOutChannels)
+
+        nChannels = nOutChannels
+        self.dense3 = self._make_dense(nChannels, growthRate, nDenseBlocks, bottleneck)
+        nChannels += nDenseBlocks * growthRate
+
+        self.act = nn.Sequential(
+            nn.BatchNorm2d(nChannels), nn.ReLU(inplace=True),
+            nn.AvgPool2d(8))
+        self.fc = nn.Linear(nChannels, nClasses)
+
+        self.apply(initialize_resnet)
+
+    def get_message(self):
+        return self.message
+
+    def _make_dense(self, nChannels, growthRate, nDenseBlocks, bottleneck):
+        layers = []
+        for i in range(int(nDenseBlocks)):
+            if bottleneck:
+                layers.append(Bottleneck(nChannels, growthRate))
+            else:
+                layers.append(SingleLayer(nChannels, growthRate))
+            nChannels += growthRate
+        return nn.Sequential(*layers)
+
+    def forward(self, inputs):
+        out = self.conv1(inputs)
+        out = self.trans1(self.dense1(out))
+        out = self.trans2(self.dense2(out))
+        out = self.dense3(out)
+        features = self.act(out)
+        features = features.view(features.size(0), -1)
+        out = self.fc(features)
+        return features, out
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/CifarResNet.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/CifarResNet.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-from .initialization import initialize_resnet
-from .SharedUtils import additive_func
-
-
-class Downsample(nn.Module):
-
-    def __init__(self, nIn, nOut, stride):
-        super(Downsample, self).__init__()
-        assert stride == 2 and nOut == 2 * nIn, 'stride:{} IO:{},{}'.format(stride, nIn, nOut)
-        self.in_dim = nIn
-        self.out_dim = nOut
-        self.avg = nn.AvgPool2d(kernel_size=2, stride=2, padding=0)
-        self.conv = nn.Conv2d(nIn, nOut, kernel_size=1, stride=1, padding=0, bias=False)
-
-    def forward(self, x):
-        x = self.avg(x)
-        out = self.conv(x)
-        return out
-
-
-class ConvBNReLU(nn.Module):
-
-    def __init__(self, nIn, nOut, kernel, stride, padding, bias, relu):
-        super(ConvBNReLU, self).__init__()
-        self.conv = nn.Conv2d(nIn, nOut, kernel_size=kernel, stride=stride, padding=padding, bias=bias)
-        self.bn = nn.BatchNorm2d(nOut)
-        if relu:
-            self.relu = nn.ReLU(inplace=True)
-        else:
-            self.relu = None
-        self.out_dim = nOut
-        self.num_conv = 1
-
-    def forward(self, x):
-        conv = self.conv(x)
-        bn = self.bn(conv)
-        if self.relu:
-            return self.relu(bn)
-        else:
-            return bn
-
-
-class ResNetBasicblock(nn.Module):
-    expansion = 1
-
-    def __init__(self, inplanes, planes, stride):
-        super(ResNetBasicblock, self).__init__()
-        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
-        self.conv_a = ConvBNReLU(inplanes, planes, 3, stride, 1, False, True)
-        self.conv_b = ConvBNReLU(planes, planes, 3, 1, 1, False, False)
-        if stride == 2:
-            self.downsample = Downsample(inplanes, planes, stride)
-        elif inplanes != planes:
-            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, False)
-        else:
-            self.downsample = None
-        self.out_dim = planes
-        self.num_conv = 2
-
-    def forward(self, inputs):
-
-        basicblock = self.conv_a(inputs)
-        basicblock = self.conv_b(basicblock)
-
-        if self.downsample is not None:
-            residual = self.downsample(inputs)
-        else:
-            residual = inputs
-        out = additive_func(residual, basicblock)
-        return F.relu(out, inplace=True)
-
-
-class ResNetBottleneck(nn.Module):
-    expansion = 4
-
-    def __init__(self, inplanes, planes, stride):
-        super(ResNetBottleneck, self).__init__()
-        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
-        self.conv_1x1 = ConvBNReLU(inplanes, planes, 1, 1, 0, False, True)
-        self.conv_3x3 = ConvBNReLU(planes, planes, 3, stride, 1, False, True)
-        self.conv_1x4 = ConvBNReLU(planes, planes * self.expansion, 1, 1, 0, False, False)
-        if stride == 2:
-            self.downsample = Downsample(inplanes, planes * self.expansion, stride)
-        elif inplanes != planes * self.expansion:
-            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, False)
-        else:
-            self.downsample = None
-        self.out_dim = planes * self.expansion
-        self.num_conv = 3
-
-    def forward(self, inputs):
-
-        bottleneck = self.conv_1x1(inputs)
-        bottleneck = self.conv_3x3(bottleneck)
-        bottleneck = self.conv_1x4(bottleneck)
-
-        if self.downsample is not None:
-            residual = self.downsample(inputs)
-        else:
-            residual = inputs
-        out = additive_func(residual, bottleneck)
-        return F.relu(out, inplace=True)
-
-
-class CifarResNet(nn.Module):
-
-    def __init__(self, block_name, depth, num_classes, zero_init_residual):
-        super(CifarResNet, self).__init__()
-
-        # Model type specifies number of layers for CIFAR-10 and CIFAR-100 model
-        if block_name == 'ResNetBasicblock':
-            block = ResNetBasicblock
-            assert (depth - 2) % 6 == 0, 'depth should be one of 20, 32, 44, 56, 110'
-            layer_blocks = (depth - 2) // 6
-        elif block_name == 'ResNetBottleneck':
-            block = ResNetBottleneck
-            assert (depth - 2) % 9 == 0, 'depth should be one of 164'
-            layer_blocks = (depth - 2) // 9
-        else:
-            raise ValueError('invalid block : {:}'.format(block_name))
-
-        self.message = 'CifarResNet : Block : {:}, Depth : {:}, Layers for each block : {:}'.format(block_name, depth,
-                                                                                                    layer_blocks)
-        self.num_classes = num_classes
-        self.channels = [16]
-        self.layers = nn.ModuleList([ConvBNReLU(3, 16, 3, 1, 1, False, True)])
-        for stage in range(3):
-            for iL in range(layer_blocks):
-                iC = self.channels[-1]
-                planes = 16 * (2 ** stage)
-                stride = 2 if stage > 0 and iL == 0 else 1
-                module = block(iC, planes, stride)
-                self.channels.append(module.out_dim)
-                self.layers.append(module)
-                self.message += "\nstage={:}, ilayer={:02d}/{:02d}, block={:03d}, iC={:3d}, oC={:3d}, stride={:}".format(
-                    stage, iL, layer_blocks, len(self.layers) - 1, iC, module.out_dim, stride)
-
-        self.avgpool = nn.AvgPool2d(8)
-        self.classifier = nn.Linear(module.out_dim, num_classes)
-        assert sum(x.num_conv for x in self.layers) + 1 == depth, 'invalid depth check {:} vs {:}'.format(
-            sum(x.num_conv for x in self.layers) + 1, depth)
-
-        self.apply(initialize_resnet)
-        if zero_init_residual:
-            for m in self.modules():
-                if isinstance(m, ResNetBasicblock):
-                    nn.init.constant_(m.conv_b.bn.weight, 0)
-                elif isinstance(m, ResNetBottleneck):
-                    nn.init.constant_(m.conv_1x4.bn.weight, 0)
-
-    def get_message(self):
-        return self.message
-
-    def forward(self, inputs):
-        x = inputs
-        for i, layer in enumerate(self.layers):
-            x = layer(x)
-        features = self.avgpool(x)
-        features = features.view(features.size(0), -1)
-        logits = self.classifier(features)
-        return features, logits
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+from .initialization import initialize_resnet
+from .SharedUtils import additive_func
+
+
+class Downsample(nn.Module):
+
+    def __init__(self, nIn, nOut, stride):
+        super(Downsample, self).__init__()
+        assert stride == 2 and nOut == 2 * nIn, 'stride:{} IO:{},{}'.format(stride, nIn, nOut)
+        self.in_dim = nIn
+        self.out_dim = nOut
+        self.avg = nn.AvgPool2d(kernel_size=2, stride=2, padding=0)
+        self.conv = nn.Conv2d(nIn, nOut, kernel_size=1, stride=1, padding=0, bias=False)
+
+    def forward(self, x):
+        x = self.avg(x)
+        out = self.conv(x)
+        return out
+
+
+class ConvBNReLU(nn.Module):
+
+    def __init__(self, nIn, nOut, kernel, stride, padding, bias, relu):
+        super(ConvBNReLU, self).__init__()
+        self.conv = nn.Conv2d(nIn, nOut, kernel_size=kernel, stride=stride, padding=padding, bias=bias)
+        self.bn = nn.BatchNorm2d(nOut)
+        if relu:
+            self.relu = nn.ReLU(inplace=True)
+        else:
+            self.relu = None
+        self.out_dim = nOut
+        self.num_conv = 1
+
+    def forward(self, x):
+        conv = self.conv(x)
+        bn = self.bn(conv)
+        if self.relu:
+            return self.relu(bn)
+        else:
+            return bn
+
+
+class ResNetBasicblock(nn.Module):
+    expansion = 1
+
+    def __init__(self, inplanes, planes, stride):
+        super(ResNetBasicblock, self).__init__()
+        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
+        self.conv_a = ConvBNReLU(inplanes, planes, 3, stride, 1, False, True)
+        self.conv_b = ConvBNReLU(planes, planes, 3, 1, 1, False, False)
+        if stride == 2:
+            self.downsample = Downsample(inplanes, planes, stride)
+        elif inplanes != planes:
+            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, False)
+        else:
+            self.downsample = None
+        self.out_dim = planes
+        self.num_conv = 2
+
+    def forward(self, inputs):
+
+        basicblock = self.conv_a(inputs)
+        basicblock = self.conv_b(basicblock)
+
+        if self.downsample is not None:
+            residual = self.downsample(inputs)
+        else:
+            residual = inputs
+        out = additive_func(residual, basicblock)
+        return F.relu(out, inplace=True)
+
+
+class ResNetBottleneck(nn.Module):
+    expansion = 4
+
+    def __init__(self, inplanes, planes, stride):
+        super(ResNetBottleneck, self).__init__()
+        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
+        self.conv_1x1 = ConvBNReLU(inplanes, planes, 1, 1, 0, False, True)
+        self.conv_3x3 = ConvBNReLU(planes, planes, 3, stride, 1, False, True)
+        self.conv_1x4 = ConvBNReLU(planes, planes * self.expansion, 1, 1, 0, False, False)
+        if stride == 2:
+            self.downsample = Downsample(inplanes, planes * self.expansion, stride)
+        elif inplanes != planes * self.expansion:
+            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, False)
+        else:
+            self.downsample = None
+        self.out_dim = planes * self.expansion
+        self.num_conv = 3
+
+    def forward(self, inputs):
+
+        bottleneck = self.conv_1x1(inputs)
+        bottleneck = self.conv_3x3(bottleneck)
+        bottleneck = self.conv_1x4(bottleneck)
+
+        if self.downsample is not None:
+            residual = self.downsample(inputs)
+        else:
+            residual = inputs
+        out = additive_func(residual, bottleneck)
+        return F.relu(out, inplace=True)
+
+
+class CifarResNet(nn.Module):
+
+    def __init__(self, block_name, depth, num_classes, zero_init_residual):
+        super(CifarResNet, self).__init__()
+
+        # Model type specifies number of layers for CIFAR-10 and CIFAR-100 model
+        if block_name == 'ResNetBasicblock':
+            block = ResNetBasicblock
+            assert (depth - 2) % 6 == 0, 'depth should be one of 20, 32, 44, 56, 110'
+            layer_blocks = (depth - 2) // 6
+        elif block_name == 'ResNetBottleneck':
+            block = ResNetBottleneck
+            assert (depth - 2) % 9 == 0, 'depth should be one of 164'
+            layer_blocks = (depth - 2) // 9
+        else:
+            raise ValueError('invalid block : {:}'.format(block_name))
+
+        self.message = 'CifarResNet : Block : {:}, Depth : {:}, Layers for each block : {:}'.format(block_name, depth,
+                                                                                                    layer_blocks)
+        self.num_classes = num_classes
+        self.channels = [16]
+        self.layers = nn.ModuleList([ConvBNReLU(3, 16, 3, 1, 1, False, True)])
+        for stage in range(3):
+            for iL in range(layer_blocks):
+                iC = self.channels[-1]
+                planes = 16 * (2 ** stage)
+                stride = 2 if stage > 0 and iL == 0 else 1
+                module = block(iC, planes, stride)
+                self.channels.append(module.out_dim)
+                self.layers.append(module)
+                self.message += "\nstage={:}, ilayer={:02d}/{:02d}, block={:03d}, iC={:3d}, oC={:3d}, stride={:}".format(
+                    stage, iL, layer_blocks, len(self.layers) - 1, iC, module.out_dim, stride)
+
+        self.avgpool = nn.AvgPool2d(8)
+        self.classifier = nn.Linear(module.out_dim, num_classes)
+        assert sum(x.num_conv for x in self.layers) + 1 == depth, 'invalid depth check {:} vs {:}'.format(
+            sum(x.num_conv for x in self.layers) + 1, depth)
+
+        self.apply(initialize_resnet)
+        if zero_init_residual:
+            for m in self.modules():
+                if isinstance(m, ResNetBasicblock):
+                    nn.init.constant_(m.conv_b.bn.weight, 0)
+                elif isinstance(m, ResNetBottleneck):
+                    nn.init.constant_(m.conv_1x4.bn.weight, 0)
+
+    def get_message(self):
+        return self.message
+
+    def forward(self, inputs):
+        x = inputs
+        for i, layer in enumerate(self.layers):
+            x = layer(x)
+        features = self.avgpool(x)
+        features = features.view(features.size(0), -1)
+        logits = self.classifier(features)
+        return features, logits
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/CifarWideResNet.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/CifarWideResNet.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-from .initialization import initialize_resnet
-
-
-class WideBasicblock(nn.Module):
-    def __init__(self, inplanes, planes, stride, dropout=False):
-        super(WideBasicblock, self).__init__()
-
-        self.bn_a = nn.BatchNorm2d(inplanes)
-        self.conv_a = nn.Conv2d(inplanes, planes, kernel_size=3, stride=stride, padding=1, bias=False)
-
-        self.bn_b = nn.BatchNorm2d(planes)
-        if dropout:
-            self.dropout = nn.Dropout2d(p=0.5, inplace=True)
-        else:
-            self.dropout = None
-        self.conv_b = nn.Conv2d(planes, planes, kernel_size=3, stride=1, padding=1, bias=False)
-
-        if inplanes != planes:
-            self.downsample = nn.Conv2d(inplanes, planes, kernel_size=1, stride=stride, padding=0, bias=False)
-        else:
-            self.downsample = None
-
-    def forward(self, x):
-
-        basicblock = self.bn_a(x)
-        basicblock = F.relu(basicblock)
-        basicblock = self.conv_a(basicblock)
-
-        basicblock = self.bn_b(basicblock)
-        basicblock = F.relu(basicblock)
-        if self.dropout is not None:
-            basicblock = self.dropout(basicblock)
-        basicblock = self.conv_b(basicblock)
-
-        if self.downsample is not None:
-            x = self.downsample(x)
-
-        return x + basicblock
-
-
-class CifarWideResNet(nn.Module):
-    """
-    ResNet optimized for the Cifar dataset, as specified in
-    https://arxiv.org/abs/1512.03385.pdf
-    """
-
-    def __init__(self, depth, widen_factor, num_classes, dropout):
-        super(CifarWideResNet, self).__init__()
-
-        # Model type specifies number of layers for CIFAR-10 and CIFAR-100 model
-        assert (depth - 4) % 6 == 0, 'depth should be one of 20, 32, 44, 56, 110'
-        layer_blocks = (depth - 4) // 6
-        print('CifarPreResNet : Depth : {} , Layers for each block : {}'.format(depth, layer_blocks))
-
-        self.num_classes = num_classes
-        self.dropout = dropout
-        self.conv_3x3 = nn.Conv2d(3, 16, kernel_size=3, stride=1, padding=1, bias=False)
-
-        self.message = 'Wide ResNet : depth={:}, widen_factor={:}, class={:}'.format(depth, widen_factor, num_classes)
-        self.inplanes = 16
-        self.stage_1 = self._make_layer(WideBasicblock, 16 * widen_factor, layer_blocks, 1)
-        self.stage_2 = self._make_layer(WideBasicblock, 32 * widen_factor, layer_blocks, 2)
-        self.stage_3 = self._make_layer(WideBasicblock, 64 * widen_factor, layer_blocks, 2)
-        self.lastact = nn.Sequential(nn.BatchNorm2d(64 * widen_factor), nn.ReLU(inplace=True))
-        self.avgpool = nn.AvgPool2d(8)
-        self.classifier = nn.Linear(64 * widen_factor, num_classes)
-
-        self.apply(initialize_resnet)
-
-    def get_message(self):
-        return self.message
-
-    def _make_layer(self, block, planes, blocks, stride):
-        layers = []
-        layers.append(block(self.inplanes, planes, stride, self.dropout))
-        self.inplanes = planes
-        for i in range(1, blocks):
-            layers.append(block(self.inplanes, planes, 1, self.dropout))
-
-        return nn.Sequential(*layers)
-
-    def forward(self, x):
-        x = self.conv_3x3(x)
-        x = self.stage_1(x)
-        x = self.stage_2(x)
-        x = self.stage_3(x)
-        x = self.lastact(x)
-        x = self.avgpool(x)
-        features = x.view(x.size(0), -1)
-        outs = self.classifier(features)
-        return features, outs
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+from .initialization import initialize_resnet
+
+
+class WideBasicblock(nn.Module):
+    def __init__(self, inplanes, planes, stride, dropout=False):
+        super(WideBasicblock, self).__init__()
+
+        self.bn_a = nn.BatchNorm2d(inplanes)
+        self.conv_a = nn.Conv2d(inplanes, planes, kernel_size=3, stride=stride, padding=1, bias=False)
+
+        self.bn_b = nn.BatchNorm2d(planes)
+        if dropout:
+            self.dropout = nn.Dropout2d(p=0.5, inplace=True)
+        else:
+            self.dropout = None
+        self.conv_b = nn.Conv2d(planes, planes, kernel_size=3, stride=1, padding=1, bias=False)
+
+        if inplanes != planes:
+            self.downsample = nn.Conv2d(inplanes, planes, kernel_size=1, stride=stride, padding=0, bias=False)
+        else:
+            self.downsample = None
+
+    def forward(self, x):
+
+        basicblock = self.bn_a(x)
+        basicblock = F.relu(basicblock)
+        basicblock = self.conv_a(basicblock)
+
+        basicblock = self.bn_b(basicblock)
+        basicblock = F.relu(basicblock)
+        if self.dropout is not None:
+            basicblock = self.dropout(basicblock)
+        basicblock = self.conv_b(basicblock)
+
+        if self.downsample is not None:
+            x = self.downsample(x)
+
+        return x + basicblock
+
+
+class CifarWideResNet(nn.Module):
+    """
+    ResNet optimized for the Cifar dataset, as specified in
+    https://arxiv.org/abs/1512.03385.pdf
+    """
+
+    def __init__(self, depth, widen_factor, num_classes, dropout):
+        super(CifarWideResNet, self).__init__()
+
+        # Model type specifies number of layers for CIFAR-10 and CIFAR-100 model
+        assert (depth - 4) % 6 == 0, 'depth should be one of 20, 32, 44, 56, 110'
+        layer_blocks = (depth - 4) // 6
+        print('CifarPreResNet : Depth : {} , Layers for each block : {}'.format(depth, layer_blocks))
+
+        self.num_classes = num_classes
+        self.dropout = dropout
+        self.conv_3x3 = nn.Conv2d(3, 16, kernel_size=3, stride=1, padding=1, bias=False)
+
+        self.message = 'Wide ResNet : depth={:}, widen_factor={:}, class={:}'.format(depth, widen_factor, num_classes)
+        self.inplanes = 16
+        self.stage_1 = self._make_layer(WideBasicblock, 16 * widen_factor, layer_blocks, 1)
+        self.stage_2 = self._make_layer(WideBasicblock, 32 * widen_factor, layer_blocks, 2)
+        self.stage_3 = self._make_layer(WideBasicblock, 64 * widen_factor, layer_blocks, 2)
+        self.lastact = nn.Sequential(nn.BatchNorm2d(64 * widen_factor), nn.ReLU(inplace=True))
+        self.avgpool = nn.AvgPool2d(8)
+        self.classifier = nn.Linear(64 * widen_factor, num_classes)
+
+        self.apply(initialize_resnet)
+
+    def get_message(self):
+        return self.message
+
+    def _make_layer(self, block, planes, blocks, stride):
+        layers = []
+        layers.append(block(self.inplanes, planes, stride, self.dropout))
+        self.inplanes = planes
+        for i in range(1, blocks):
+            layers.append(block(self.inplanes, planes, 1, self.dropout))
+
+        return nn.Sequential(*layers)
+
+    def forward(self, x):
+        x = self.conv_3x3(x)
+        x = self.stage_1(x)
+        x = self.stage_2(x)
+        x = self.stage_3(x)
+        x = self.lastact(x)
+        x = self.avgpool(x)
+        features = x.view(x.size(0), -1)
+        outs = self.classifier(features)
+        return features, outs
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/ImageNet_MobileNetV2.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/ImageNet_MobileNetV2.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-# MobileNetV2: Inverted Residuals and Linear Bottlenecks, CVPR 2018
-from torch import nn
-from .initialization import initialize_resnet
-
-
-class ConvBNReLU(nn.Module):
-    def __init__(self, in_planes, out_planes, kernel_size=3, stride=1, groups=1):
-        super(ConvBNReLU, self).__init__()
-        padding = (kernel_size - 1) // 2
-        self.conv = nn.Conv2d(in_planes, out_planes, kernel_size, stride, padding, groups=groups, bias=False)
-        self.bn = nn.BatchNorm2d(out_planes)
-        self.relu = nn.ReLU6(inplace=True)
-
-    def forward(self, x):
-        out = self.conv(x)
-        out = self.bn(out)
-        out = self.relu(out)
-        return out
-
-
-class InvertedResidual(nn.Module):
-    def __init__(self, inp, oup, stride, expand_ratio):
-        super(InvertedResidual, self).__init__()
-        self.stride = stride
-        assert stride in [1, 2]
-
-        hidden_dim = int(round(inp * expand_ratio))
-        self.use_res_connect = self.stride == 1 and inp == oup
-
-        layers = []
-        if expand_ratio != 1:
-            # pw
-            layers.append(ConvBNReLU(inp, hidden_dim, kernel_size=1))
-        layers.extend([
-            # dw
-            ConvBNReLU(hidden_dim, hidden_dim, stride=stride, groups=hidden_dim),
-            # pw-linear
-            nn.Conv2d(hidden_dim, oup, 1, 1, 0, bias=False),
-            nn.BatchNorm2d(oup),
-        ])
-        self.conv = nn.Sequential(*layers)
-
-    def forward(self, x):
-        if self.use_res_connect:
-            return x + self.conv(x)
-        else:
-            return self.conv(x)
-
-
-class MobileNetV2(nn.Module):
-    def __init__(self, num_classes, width_mult, input_channel, last_channel, block_name, dropout):
-        super(MobileNetV2, self).__init__()
-        if block_name == 'InvertedResidual':
-            block = InvertedResidual
-        else:
-            raise ValueError('invalid block name : {:}'.format(block_name))
-        inverted_residual_setting = [
-            # t, c,  n, s
-            [1, 16, 1, 1],
-            [6, 24, 2, 2],
-            [6, 32, 3, 2],
-            [6, 64, 4, 2],
-            [6, 96, 3, 1],
-            [6, 160, 3, 2],
-            [6, 320, 1, 1],
-        ]
-
-        # building first layer
-        input_channel = int(input_channel * width_mult)
-        self.last_channel = int(last_channel * max(1.0, width_mult))
-        features = [ConvBNReLU(3, input_channel, stride=2)]
-        # building inverted residual blocks
-        for t, c, n, s in inverted_residual_setting:
-            output_channel = int(c * width_mult)
-            for i in range(n):
-                stride = s if i == 0 else 1
-                features.append(block(input_channel, output_channel, stride, expand_ratio=t))
-                input_channel = output_channel
-        # building last several layers
-        features.append(ConvBNReLU(input_channel, self.last_channel, kernel_size=1))
-        # make it nn.Sequential
-        self.features = nn.Sequential(*features)
-
-        # building classifier
-        self.classifier = nn.Sequential(
-            nn.Dropout(dropout),
-            nn.Linear(self.last_channel, num_classes),
-        )
-        self.message = 'MobileNetV2 : width_mult={:}, in-C={:}, last-C={:}, block={:}, dropout={:}'.format(width_mult,
-                                                                                                           input_channel,
-                                                                                                           last_channel,
-                                                                                                           block_name,
-                                                                                                           dropout)
-
-        # weight initialization
-        self.apply(initialize_resnet)
-
-    def get_message(self):
-        return self.message
-
-    def forward(self, inputs):
-        features = self.features(inputs)
-        vectors = features.mean([2, 3])
-        predicts = self.classifier(vectors)
-        return features, predicts
+# MobileNetV2: Inverted Residuals and Linear Bottlenecks, CVPR 2018
+from torch import nn
+from .initialization import initialize_resnet
+
+
+class ConvBNReLU(nn.Module):
+    def __init__(self, in_planes, out_planes, kernel_size=3, stride=1, groups=1):
+        super(ConvBNReLU, self).__init__()
+        padding = (kernel_size - 1) // 2
+        self.conv = nn.Conv2d(in_planes, out_planes, kernel_size, stride, padding, groups=groups, bias=False)
+        self.bn = nn.BatchNorm2d(out_planes)
+        self.relu = nn.ReLU6(inplace=True)
+
+    def forward(self, x):
+        out = self.conv(x)
+        out = self.bn(out)
+        out = self.relu(out)
+        return out
+
+
+class InvertedResidual(nn.Module):
+    def __init__(self, inp, oup, stride, expand_ratio):
+        super(InvertedResidual, self).__init__()
+        self.stride = stride
+        assert stride in [1, 2]
+
+        hidden_dim = int(round(inp * expand_ratio))
+        self.use_res_connect = self.stride == 1 and inp == oup
+
+        layers = []
+        if expand_ratio != 1:
+            # pw
+            layers.append(ConvBNReLU(inp, hidden_dim, kernel_size=1))
+        layers.extend([
+            # dw
+            ConvBNReLU(hidden_dim, hidden_dim, stride=stride, groups=hidden_dim),
+            # pw-linear
+            nn.Conv2d(hidden_dim, oup, 1, 1, 0, bias=False),
+            nn.BatchNorm2d(oup),
+        ])
+        self.conv = nn.Sequential(*layers)
+
+    def forward(self, x):
+        if self.use_res_connect:
+            return x + self.conv(x)
+        else:
+            return self.conv(x)
+
+
+class MobileNetV2(nn.Module):
+    def __init__(self, num_classes, width_mult, input_channel, last_channel, block_name, dropout):
+        super(MobileNetV2, self).__init__()
+        if block_name == 'InvertedResidual':
+            block = InvertedResidual
+        else:
+            raise ValueError('invalid block name : {:}'.format(block_name))
+        inverted_residual_setting = [
+            # t, c,  n, s
+            [1, 16, 1, 1],
+            [6, 24, 2, 2],
+            [6, 32, 3, 2],
+            [6, 64, 4, 2],
+            [6, 96, 3, 1],
+            [6, 160, 3, 2],
+            [6, 320, 1, 1],
+        ]
+
+        # building first layer
+        input_channel = int(input_channel * width_mult)
+        self.last_channel = int(last_channel * max(1.0, width_mult))
+        features = [ConvBNReLU(3, input_channel, stride=2)]
+        # building inverted residual blocks
+        for t, c, n, s in inverted_residual_setting:
+            output_channel = int(c * width_mult)
+            for i in range(n):
+                stride = s if i == 0 else 1
+                features.append(block(input_channel, output_channel, stride, expand_ratio=t))
+                input_channel = output_channel
+        # building last several layers
+        features.append(ConvBNReLU(input_channel, self.last_channel, kernel_size=1))
+        # make it nn.Sequential
+        self.features = nn.Sequential(*features)
+
+        # building classifier
+        self.classifier = nn.Sequential(
+            nn.Dropout(dropout),
+            nn.Linear(self.last_channel, num_classes),
+        )
+        self.message = 'MobileNetV2 : width_mult={:}, in-C={:}, last-C={:}, block={:}, dropout={:}'.format(width_mult,
+                                                                                                           input_channel,
+                                                                                                           last_channel,
+                                                                                                           block_name,
+                                                                                                           dropout)
+
+        # weight initialization
+        self.apply(initialize_resnet)
+
+    def get_message(self):
+        return self.message
+
+    def forward(self, inputs):
+        features = self.features(inputs)
+        vectors = features.mean([2, 3])
+        predicts = self.classifier(vectors)
+        return features, predicts
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/ImageNet_ResNet.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/ImageNet_ResNet.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,178 +1,178 @@
-# Deep Residual Learning for Image Recognition, CVPR 2016
-import torch.nn as nn
-from .initialization import initialize_resnet
-
-
-def conv3x3(in_planes, out_planes, stride=1, groups=1):
-    return nn.Conv2d(in_planes, out_planes, kernel_size=3, stride=stride, padding=1, groups=groups, bias=False)
-
-
-def conv1x1(in_planes, out_planes, stride=1):
-    return nn.Conv2d(in_planes, out_planes, kernel_size=1, stride=stride, bias=False)
-
-
-class BasicBlock(nn.Module):
-    expansion = 1
-
-    def __init__(self, inplanes, planes, stride=1, downsample=None, groups=1, base_width=64):
-        super(BasicBlock, self).__init__()
-        if groups != 1 or base_width != 64:
-            raise ValueError('BasicBlock only supports groups=1 and base_width=64')
-        # Both self.conv1 and self.downsample layers downsample the input when stride != 1
-        self.conv1 = conv3x3(inplanes, planes, stride)
-        self.bn1 = nn.BatchNorm2d(planes)
-        self.relu = nn.ReLU(inplace=True)
-        self.conv2 = conv3x3(planes, planes)
-        self.bn2 = nn.BatchNorm2d(planes)
-        self.downsample = downsample
-        self.stride = stride
-
-    def forward(self, x):
-        identity = x
-
-        out = self.conv1(x)
-        out = self.bn1(out)
-        out = self.relu(out)
-
-        out = self.conv2(out)
-        out = self.bn2(out)
-
-        if self.downsample is not None:
-            identity = self.downsample(x)
-
-        out += identity
-        out = self.relu(out)
-
-        return out
-
-
-class Bottleneck(nn.Module):
-    expansion = 4
-
-    def __init__(self, inplanes, planes, stride=1, downsample=None, groups=1, base_width=64):
-        super(Bottleneck, self).__init__()
-        width = int(planes * (base_width / 64.)) * groups
-        # Both self.conv2 and self.downsample layers downsample the input when stride != 1
-        self.conv1 = conv1x1(inplanes, width)
-        self.bn1 = nn.BatchNorm2d(width)
-        self.conv2 = conv3x3(width, width, stride, groups)
-        self.bn2 = nn.BatchNorm2d(width)
-        self.conv3 = conv1x1(width, planes * self.expansion)
-        self.bn3 = nn.BatchNorm2d(planes * self.expansion)
-        self.relu = nn.ReLU(inplace=True)
-        self.downsample = downsample
-        self.stride = stride
-
-    def forward(self, x):
-        identity = x
-
-        out = self.conv1(x)
-        out = self.bn1(out)
-        out = self.relu(out)
-
-        out = self.conv2(out)
-        out = self.bn2(out)
-        out = self.relu(out)
-
-        out = self.conv3(out)
-        out = self.bn3(out)
-
-        if self.downsample is not None:
-            identity = self.downsample(x)
-
-        out += identity
-        out = self.relu(out)
-
-        return out
-
-
-class ResNet(nn.Module):
-
-    def __init__(self, block_name, layers, deep_stem, num_classes, zero_init_residual, groups, width_per_group):
-        super(ResNet, self).__init__()
-
-        # planes = [int(width_per_group * groups * 2 ** i) for i in range(4)]
-        if block_name == 'BasicBlock':
-            block = BasicBlock
-        elif block_name == 'Bottleneck':
-            block = Bottleneck
-        else:
-            raise ValueError('invalid block-name : {:}'.format(block_name))
-
-        if not deep_stem:
-            self.conv = nn.Sequential(
-                nn.Conv2d(3, 64, kernel_size=7, stride=2, padding=3, bias=False),
-                nn.BatchNorm2d(64), nn.ReLU(inplace=True))
-        else:
-            self.conv = nn.Sequential(
-                nn.Conv2d(3, 32, kernel_size=3, stride=2, padding=1, bias=False),
-                nn.BatchNorm2d(32), nn.ReLU(inplace=True),
-                nn.Conv2d(32, 32, kernel_size=3, stride=1, padding=1, bias=False),
-                nn.BatchNorm2d(32), nn.ReLU(inplace=True),
-                nn.Conv2d(32, 64, kernel_size=3, stride=1, padding=1, bias=False),
-                nn.BatchNorm2d(64), nn.ReLU(inplace=True))
-        self.inplanes = 64
-        self.maxpool = nn.MaxPool2d(kernel_size=3, stride=2, padding=1)
-        self.layer1 = self._make_layer(block, 64, layers[0], stride=1, groups=groups, base_width=width_per_group)
-        self.layer2 = self._make_layer(block, 128, layers[1], stride=2, groups=groups, base_width=width_per_group)
-        self.layer3 = self._make_layer(block, 256, layers[2], stride=2, groups=groups, base_width=width_per_group)
-        self.layer4 = self._make_layer(block, 512, layers[3], stride=2, groups=groups, base_width=width_per_group)
-        self.avgpool = nn.AdaptiveAvgPool2d((1, 1))
-        self.fc = nn.Linear(512 * block.expansion, num_classes)
-        self.message = 'block = {:}, layers = {:}, deep_stem = {:}, num_classes = {:}'.format(block, layers, deep_stem,
-                                                                                              num_classes)
-
-        self.apply(initialize_resnet)
-
-        # Zero-initialize the last BN in each residual branch,
-        # so that the residual branch starts with zeros, and each residual block behaves like an identity.
-        # This improves the model by 0.2~0.3% according to https://arxiv.org/abs/1706.02677
-        if zero_init_residual:
-            for m in self.modules():
-                if isinstance(m, Bottleneck):
-                    nn.init.constant_(m.bn3.weight, 0)
-                elif isinstance(m, BasicBlock):
-                    nn.init.constant_(m.bn2.weight, 0)
-
-    def _make_layer(self, block, planes, blocks, stride, groups, base_width):
-        downsample = None
-        if stride != 1 or self.inplanes != planes * block.expansion:
-            if stride == 2:
-                downsample = nn.Sequential(
-                    nn.AvgPool2d(kernel_size=2, stride=2, padding=0),
-                    conv1x1(self.inplanes, planes * block.expansion, 1),
-                    nn.BatchNorm2d(planes * block.expansion),
-                )
-            elif stride == 1:
-                downsample = nn.Sequential(
-                    conv1x1(self.inplanes, planes * block.expansion, stride),
-                    nn.BatchNorm2d(planes * block.expansion),
-                )
-            else:
-                raise ValueError('invalid stride [{:}] for downsample'.format(stride))
-
-        layers = []
-        layers.append(block(self.inplanes, planes, stride, downsample, groups, base_width))
-        self.inplanes = planes * block.expansion
-        for _ in range(1, blocks):
-            layers.append(block(self.inplanes, planes, 1, None, groups, base_width))
-
-        return nn.Sequential(*layers)
-
-    def get_message(self):
-        return self.message
-
-    def forward(self, x):
-        x = self.conv(x)
-        x = self.maxpool(x)
-
-        x = self.layer1(x)
-        x = self.layer2(x)
-        x = self.layer3(x)
-        x = self.layer4(x)
-
-        features = self.avgpool(x)
-        features = features.view(features.size(0), -1)
-        logits = self.fc(features)
-
-        return features, logits
+# Deep Residual Learning for Image Recognition, CVPR 2016
+import torch.nn as nn
+from .initialization import initialize_resnet
+
+
+def conv3x3(in_planes, out_planes, stride=1, groups=1):
+    return nn.Conv2d(in_planes, out_planes, kernel_size=3, stride=stride, padding=1, groups=groups, bias=False)
+
+
+def conv1x1(in_planes, out_planes, stride=1):
+    return nn.Conv2d(in_planes, out_planes, kernel_size=1, stride=stride, bias=False)
+
+
+class BasicBlock(nn.Module):
+    expansion = 1
+
+    def __init__(self, inplanes, planes, stride=1, downsample=None, groups=1, base_width=64):
+        super(BasicBlock, self).__init__()
+        if groups != 1 or base_width != 64:
+            raise ValueError('BasicBlock only supports groups=1 and base_width=64')
+        # Both self.conv1 and self.downsample layers downsample the input when stride != 1
+        self.conv1 = conv3x3(inplanes, planes, stride)
+        self.bn1 = nn.BatchNorm2d(planes)
+        self.relu = nn.ReLU(inplace=True)
+        self.conv2 = conv3x3(planes, planes)
+        self.bn2 = nn.BatchNorm2d(planes)
+        self.downsample = downsample
+        self.stride = stride
+
+    def forward(self, x):
+        identity = x
+
+        out = self.conv1(x)
+        out = self.bn1(out)
+        out = self.relu(out)
+
+        out = self.conv2(out)
+        out = self.bn2(out)
+
+        if self.downsample is not None:
+            identity = self.downsample(x)
+
+        out += identity
+        out = self.relu(out)
+
+        return out
+
+
+class Bottleneck(nn.Module):
+    expansion = 4
+
+    def __init__(self, inplanes, planes, stride=1, downsample=None, groups=1, base_width=64):
+        super(Bottleneck, self).__init__()
+        width = int(planes * (base_width / 64.)) * groups
+        # Both self.conv2 and self.downsample layers downsample the input when stride != 1
+        self.conv1 = conv1x1(inplanes, width)
+        self.bn1 = nn.BatchNorm2d(width)
+        self.conv2 = conv3x3(width, width, stride, groups)
+        self.bn2 = nn.BatchNorm2d(width)
+        self.conv3 = conv1x1(width, planes * self.expansion)
+        self.bn3 = nn.BatchNorm2d(planes * self.expansion)
+        self.relu = nn.ReLU(inplace=True)
+        self.downsample = downsample
+        self.stride = stride
+
+    def forward(self, x):
+        identity = x
+
+        out = self.conv1(x)
+        out = self.bn1(out)
+        out = self.relu(out)
+
+        out = self.conv2(out)
+        out = self.bn2(out)
+        out = self.relu(out)
+
+        out = self.conv3(out)
+        out = self.bn3(out)
+
+        if self.downsample is not None:
+            identity = self.downsample(x)
+
+        out += identity
+        out = self.relu(out)
+
+        return out
+
+
+class ResNet(nn.Module):
+
+    def __init__(self, block_name, layers, deep_stem, num_classes, zero_init_residual, groups, width_per_group):
+        super(ResNet, self).__init__()
+
+        # planes = [int(width_per_group * groups * 2 ** i) for i in range(4)]
+        if block_name == 'BasicBlock':
+            block = BasicBlock
+        elif block_name == 'Bottleneck':
+            block = Bottleneck
+        else:
+            raise ValueError('invalid block-name : {:}'.format(block_name))
+
+        if not deep_stem:
+            self.conv = nn.Sequential(
+                nn.Conv2d(3, 64, kernel_size=7, stride=2, padding=3, bias=False),
+                nn.BatchNorm2d(64), nn.ReLU(inplace=True))
+        else:
+            self.conv = nn.Sequential(
+                nn.Conv2d(3, 32, kernel_size=3, stride=2, padding=1, bias=False),
+                nn.BatchNorm2d(32), nn.ReLU(inplace=True),
+                nn.Conv2d(32, 32, kernel_size=3, stride=1, padding=1, bias=False),
+                nn.BatchNorm2d(32), nn.ReLU(inplace=True),
+                nn.Conv2d(32, 64, kernel_size=3, stride=1, padding=1, bias=False),
+                nn.BatchNorm2d(64), nn.ReLU(inplace=True))
+        self.inplanes = 64
+        self.maxpool = nn.MaxPool2d(kernel_size=3, stride=2, padding=1)
+        self.layer1 = self._make_layer(block, 64, layers[0], stride=1, groups=groups, base_width=width_per_group)
+        self.layer2 = self._make_layer(block, 128, layers[1], stride=2, groups=groups, base_width=width_per_group)
+        self.layer3 = self._make_layer(block, 256, layers[2], stride=2, groups=groups, base_width=width_per_group)
+        self.layer4 = self._make_layer(block, 512, layers[3], stride=2, groups=groups, base_width=width_per_group)
+        self.avgpool = nn.AdaptiveAvgPool2d((1, 1))
+        self.fc = nn.Linear(512 * block.expansion, num_classes)
+        self.message = 'block = {:}, layers = {:}, deep_stem = {:}, num_classes = {:}'.format(block, layers, deep_stem,
+                                                                                              num_classes)
+
+        self.apply(initialize_resnet)
+
+        # Zero-initialize the last BN in each residual branch,
+        # so that the residual branch starts with zeros, and each residual block behaves like an identity.
+        # This improves the model by 0.2~0.3% according to https://arxiv.org/abs/1706.02677
+        if zero_init_residual:
+            for m in self.modules():
+                if isinstance(m, Bottleneck):
+                    nn.init.constant_(m.bn3.weight, 0)
+                elif isinstance(m, BasicBlock):
+                    nn.init.constant_(m.bn2.weight, 0)
+
+    def _make_layer(self, block, planes, blocks, stride, groups, base_width):
+        downsample = None
+        if stride != 1 or self.inplanes != planes * block.expansion:
+            if stride == 2:
+                downsample = nn.Sequential(
+                    nn.AvgPool2d(kernel_size=2, stride=2, padding=0),
+                    conv1x1(self.inplanes, planes * block.expansion, 1),
+                    nn.BatchNorm2d(planes * block.expansion),
+                )
+            elif stride == 1:
+                downsample = nn.Sequential(
+                    conv1x1(self.inplanes, planes * block.expansion, stride),
+                    nn.BatchNorm2d(planes * block.expansion),
+                )
+            else:
+                raise ValueError('invalid stride [{:}] for downsample'.format(stride))
+
+        layers = []
+        layers.append(block(self.inplanes, planes, stride, downsample, groups, base_width))
+        self.inplanes = planes * block.expansion
+        for _ in range(1, blocks):
+            layers.append(block(self.inplanes, planes, 1, None, groups, base_width))
+
+        return nn.Sequential(*layers)
+
+    def get_message(self):
+        return self.message
+
+    def forward(self, x):
+        x = self.conv(x)
+        x = self.maxpool(x)
+
+        x = self.layer1(x)
+        x = self.layer2(x)
+        x = self.layer3(x)
+        x = self.layer4(x)
+
+        features = self.avgpool(x)
+        features = features.view(features.size(0), -1)
+        logits = self.fc(features)
+
+        return features, logits
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/SharedUtils.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/SharedUtils.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-#####################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019.01 #
-#####################################################
-import torch
-import torch.nn as nn
-
-
-def additive_func(A, B):
-    assert A.dim() == B.dim() and A.size(0) == B.size(0), '{:} vs {:}'.format(A.size(), B.size())
-    C = min(A.size(1), B.size(1))
-    if A.size(1) == B.size(1):
-        return A + B
-    elif A.size(1) < B.size(1):
-        out = B.clone()
-        out[:, :C] += A
-        return out
-    else:
-        out = A.clone()
-        out[:, :C] += B
-        return out
-
-
-def change_key(key, value):
-    def func(m):
-        if hasattr(m, key):
-            setattr(m, key, value)
-
-    return func
-
-
-def parse_channel_info(xstring):
-    blocks = xstring.split(' ')
-    blocks = [x.split('-') for x in blocks]
-    blocks = [[int(_) for _ in x] for x in blocks]
-    return blocks
+#####################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019.01 #
+#####################################################
+import torch
+import torch.nn as nn
+
+
+def additive_func(A, B):
+    assert A.dim() == B.dim() and A.size(0) == B.size(0), '{:} vs {:}'.format(A.size(), B.size())
+    C = min(A.size(1), B.size(1))
+    if A.size(1) == B.size(1):
+        return A + B
+    elif A.size(1) < B.size(1):
+        out = B.clone()
+        out[:, :C] += A
+        return out
+    else:
+        out = A.clone()
+        out[:, :C] += B
+        return out
+
+
+def change_key(key, value):
+    def func(m):
+        if hasattr(m, key):
+            setattr(m, key, value)
+
+    return func
+
+
+def parse_channel_info(xstring):
+    blocks = xstring.split(' ')
+    blocks = [x.split('-') for x in blocks]
+    blocks = [[int(_) for _ in x] for x in blocks]
+    return blocks
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/__init__.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/__init__.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-##################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
-##################################################
-from os import path as osp
-from typing import List, Text
-import torch
-
-__all__ = ['change_key', 'get_cell_based_tiny_net', 'get_search_spaces', 'get_cifar_models', 'get_imagenet_models', \
-           'obtain_model', 'obtain_search_model', 'load_net_from_checkpoint', \
-           'CellStructure', 'CellArchitectures'
-           ]
-
-# useful modules
-from .config_utils import dict2config
-from .SharedUtils import change_key
-from .cell_searchs import CellStructure, CellArchitectures
-
-
-# Cell-based NAS Models
-def get_cell_based_tiny_net(config):
-    if isinstance(config, dict): config = dict2config(config, None)  # to support the argument being a dict
-    super_type = getattr(config, 'super_type', 'basic')
-    group_names = ['DARTS-V1', 'DARTS-V2', 'GDAS', 'SETN', 'ENAS', 'RANDOM', 'generic']
-    if super_type == 'basic' and config.name in group_names:
-        from .cell_searchs import nas201_super_nets as nas_super_nets
-        try:
-            return nas_super_nets[config.name](config.C, config.N, config.max_nodes, config.num_classes, config.space,
-                                               config.affine, config.track_running_stats)
-        except:
-            return nas_super_nets[config.name](config.C, config.N, config.max_nodes, config.num_classes, config.space)
-    elif super_type == 'search-shape':
-        from .shape_searchs import GenericNAS301Model
-        genotype = CellStructure.str2structure(config.genotype)
-        return GenericNAS301Model(config.candidate_Cs, config.max_num_Cs, genotype, config.num_classes, config.affine,
-                                  config.track_running_stats)
-    elif super_type == 'nasnet-super':
-        from .cell_searchs import nasnet_super_nets as nas_super_nets
-        return nas_super_nets[config.name](config.C, config.N, config.steps, config.multiplier, \
-                                           config.stem_multiplier, config.num_classes, config.space, config.affine,
-                                           config.track_running_stats)
-    elif config.name == 'infer.tiny':
-        from .cell_infers import TinyNetwork
-        if hasattr(config, 'genotype'):
-            genotype = config.genotype
-        elif hasattr(config, 'arch_str'):
-            genotype = CellStructure.str2structure(config.arch_str)
-        else:
-            raise ValueError('Can not find genotype from this config : {:}'.format(config))
-        return TinyNetwork(config.C, config.N, genotype, config.num_classes)
-    elif config.name == 'infer.shape.tiny':
-        from .shape_infers import DynamicShapeTinyNet
-        if isinstance(config.channels, str):
-            channels = tuple([int(x) for x in config.channels.split(':')])
-        else:
-            channels = config.channels
-        genotype = CellStructure.str2structure(config.genotype)
-        return DynamicShapeTinyNet(channels, genotype, config.num_classes)
-    elif config.name == 'infer.nasnet-cifar':
-        from .cell_infers import NASNetonCIFAR
-        raise NotImplementedError
-    else:
-        raise ValueError('invalid network name : {:}'.format(config.name))
-
-
-# obtain the search space, i.e., a dict mapping the operation name into a python-function for this op
-def get_search_spaces(xtype, name) -> List[Text]:
-    if xtype == 'cell' or xtype == 'tss':  # The topology search space.
-        from .cell_operations import SearchSpaceNames
-        assert name in SearchSpaceNames, 'invalid name [{:}] in {:}'.format(name, SearchSpaceNames.keys())
-        return SearchSpaceNames[name]
-    elif xtype == 'sss':  # The size search space.
-        if name in ['nats-bench', 'nats-bench-size']:
-            return {'candidates': [8, 16, 24, 32, 40, 48, 56, 64],
-                    'numbers': 5}
-        else:
-            raise ValueError('Invalid name : {:}'.format(name))
-    else:
-        raise ValueError('invalid search-space type is {:}'.format(xtype))
-
-
-def get_cifar_models(config, extra_path=None):
-    super_type = getattr(config, 'super_type', 'basic')
-    if super_type == 'basic':
-        from .CifarResNet import CifarResNet
-        from .CifarDenseNet import DenseNet
-        from .CifarWideResNet import CifarWideResNet
-        if config.arch == 'resnet':
-            return CifarResNet(config.module, config.depth, config.class_num, config.zero_init_residual)
-        elif config.arch == 'densenet':
-            return DenseNet(config.growthRate, config.depth, config.reduction, config.class_num, config.bottleneck)
-        elif config.arch == 'wideresnet':
-            return CifarWideResNet(config.depth, config.wide_factor, config.class_num, config.dropout)
-        else:
-            raise ValueError('invalid module type : {:}'.format(config.arch))
-    elif super_type.startswith('infer'):
-        from .shape_infers import InferWidthCifarResNet
-        from .shape_infers import InferDepthCifarResNet
-        from .shape_infers import InferCifarResNet
-        from .cell_infers import NASNetonCIFAR
-        assert len(super_type.split('-')) == 2, 'invalid super_type : {:}'.format(super_type)
-        infer_mode = super_type.split('-')[1]
-        if infer_mode == 'width':
-            return InferWidthCifarResNet(config.module, config.depth, config.xchannels, config.class_num,
-                                         config.zero_init_residual)
-        elif infer_mode == 'depth':
-            return InferDepthCifarResNet(config.module, config.depth, config.xblocks, config.class_num,
-                                         config.zero_init_residual)
-        elif infer_mode == 'shape':
-            return InferCifarResNet(config.module, config.depth, config.xblocks, config.xchannels, config.class_num,
-                                    config.zero_init_residual)
-        elif infer_mode == 'nasnet.cifar':
-            genotype = config.genotype
-            if extra_path is not None:  # reload genotype by extra_path
-                if not osp.isfile(extra_path): raise ValueError('invalid extra_path : {:}'.format(extra_path))
-                xdata = torch.load(extra_path)
-                current_epoch = xdata['epoch']
-                genotype = xdata['genotypes'][current_epoch - 1]
-            C = config.C if hasattr(config, 'C') else config.ichannel
-            N = config.N if hasattr(config, 'N') else config.layers
-            return NASNetonCIFAR(C, N, config.stem_multi, config.class_num, genotype, config.auxiliary)
-        else:
-            raise ValueError('invalid infer-mode : {:}'.format(infer_mode))
-    else:
-        raise ValueError('invalid super-type : {:}'.format(super_type))
-
-
-def get_imagenet_models(config):
-    super_type = getattr(config, 'super_type', 'basic')
-    if super_type == 'basic':
-        from .ImageNet_ResNet import ResNet
-        from .ImageNet_MobileNetV2 import MobileNetV2
-        if config.arch == 'resnet':
-            return ResNet(config.block_name, config.layers, config.deep_stem, config.class_num,
-                          config.zero_init_residual, config.groups, config.width_per_group)
-        elif config.arch == 'mobilenet_v2':
-            return MobileNetV2(config.class_num, config.width_multi, config.input_channel, config.last_channel,
-                               'InvertedResidual', config.dropout)
-        else:
-            raise ValueError('invalid arch : {:}'.format(config.arch))
-    elif super_type.startswith('infer'):  # NAS searched architecture
-        assert len(super_type.split('-')) == 2, 'invalid super_type : {:}'.format(super_type)
-        infer_mode = super_type.split('-')[1]
-        if infer_mode == 'shape':
-            from .shape_infers import InferImagenetResNet
-            from .shape_infers import InferMobileNetV2
-            if config.arch == 'resnet':
-                return InferImagenetResNet(config.block_name, config.layers, config.xblocks, config.xchannels,
-                                           config.deep_stem, config.class_num, config.zero_init_residual)
-            elif config.arch == "MobileNetV2":
-                return InferMobileNetV2(config.class_num, config.xchannels, config.xblocks, config.dropout)
-            else:
-                raise ValueError('invalid arch-mode : {:}'.format(config.arch))
-        else:
-            raise ValueError('invalid infer-mode : {:}'.format(infer_mode))
-    else:
-        raise ValueError('invalid super-type : {:}'.format(super_type))
-
-
-# Try to obtain the network by config.
-def obtain_model(config, extra_path=None):
-    if config.dataset == 'cifar':
-        return get_cifar_models(config, extra_path)
-    elif config.dataset == 'imagenet':
-        return get_imagenet_models(config)
-    else:
-        raise ValueError('invalid dataset in the model config : {:}'.format(config))
-
-
-def obtain_search_model(config):
-    if config.dataset == 'cifar':
-        if config.arch == 'resnet':
-            from .shape_searchs import SearchWidthCifarResNet
-            from .shape_searchs import SearchDepthCifarResNet
-            from .shape_searchs import SearchShapeCifarResNet
-            if config.search_mode == 'width':
-                return SearchWidthCifarResNet(config.module, config.depth, config.class_num)
-            elif config.search_mode == 'depth':
-                return SearchDepthCifarResNet(config.module, config.depth, config.class_num)
-            elif config.search_mode == 'shape':
-                return SearchShapeCifarResNet(config.module, config.depth, config.class_num)
-            else:
-                raise ValueError('invalid search mode : {:}'.format(config.search_mode))
-        elif config.arch == 'simres':
-            from .shape_searchs import SearchWidthSimResNet
-            if config.search_mode == 'width':
-                return SearchWidthSimResNet(config.depth, config.class_num)
-            else:
-                raise ValueError('invalid search mode : {:}'.format(config.search_mode))
-        else:
-            raise ValueError('invalid arch : {:} for dataset [{:}]'.format(config.arch, config.dataset))
-    elif config.dataset == 'imagenet':
-        from .shape_searchs import SearchShapeImagenetResNet
-        assert config.search_mode == 'shape', 'invalid search-mode : {:}'.format(config.search_mode)
-        if config.arch == 'resnet':
-            return SearchShapeImagenetResNet(config.block_name, config.layers, config.deep_stem, config.class_num)
-        else:
-            raise ValueError('invalid model config : {:}'.format(config))
-    else:
-        raise ValueError('invalid dataset in the model config : {:}'.format(config))
-
-
-def load_net_from_checkpoint(checkpoint):
-    assert osp.isfile(checkpoint), 'checkpoint {:} does not exist'.format(checkpoint)
-    checkpoint = torch.load(checkpoint)
-    model_config = dict2config(checkpoint['model-config'], None)
-    model = obtain_model(model_config)
-    model.load_state_dict(checkpoint['base-model'])
-    return model
+##################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
+##################################################
+from os import path as osp
+from typing import List, Text
+import torch
+
+__all__ = ['change_key', 'get_cell_based_tiny_net', 'get_search_spaces', 'get_cifar_models', 'get_imagenet_models', \
+           'obtain_model', 'obtain_search_model', 'load_net_from_checkpoint', \
+           'CellStructure', 'CellArchitectures'
+           ]
+
+# useful modules
+from .config_utils import dict2config
+from .SharedUtils import change_key
+from .cell_searchs import CellStructure, CellArchitectures
+
+
+# Cell-based NAS Models
+def get_cell_based_tiny_net(config):
+    if isinstance(config, dict): config = dict2config(config, None)  # to support the argument being a dict
+    super_type = getattr(config, 'super_type', 'basic')
+    group_names = ['DARTS-V1', 'DARTS-V2', 'GDAS', 'SETN', 'ENAS', 'RANDOM', 'generic']
+    if super_type == 'basic' and config.name in group_names:
+        from .cell_searchs import nas201_super_nets as nas_super_nets
+        try:
+            return nas_super_nets[config.name](config.C, config.N, config.max_nodes, config.num_classes, config.space,
+                                               config.affine, config.track_running_stats)
+        except:
+            return nas_super_nets[config.name](config.C, config.N, config.max_nodes, config.num_classes, config.space)
+    elif super_type == 'search-shape':
+        from .shape_searchs import GenericNAS301Model
+        genotype = CellStructure.str2structure(config.genotype)
+        return GenericNAS301Model(config.candidate_Cs, config.max_num_Cs, genotype, config.num_classes, config.affine,
+                                  config.track_running_stats)
+    elif super_type == 'nasnet-super':
+        from .cell_searchs import nasnet_super_nets as nas_super_nets
+        return nas_super_nets[config.name](config.C, config.N, config.steps, config.multiplier, \
+                                           config.stem_multiplier, config.num_classes, config.space, config.affine,
+                                           config.track_running_stats)
+    elif config.name == 'infer.tiny':
+        from .cell_infers import TinyNetwork
+        if hasattr(config, 'genotype'):
+            genotype = config.genotype
+        elif hasattr(config, 'arch_str'):
+            genotype = CellStructure.str2structure(config.arch_str)
+        else:
+            raise ValueError('Can not find genotype from this config : {:}'.format(config))
+        return TinyNetwork(config.C, config.N, genotype, config.num_classes)
+    elif config.name == 'infer.shape.tiny':
+        from .shape_infers import DynamicShapeTinyNet
+        if isinstance(config.channels, str):
+            channels = tuple([int(x) for x in config.channels.split(':')])
+        else:
+            channels = config.channels
+        genotype = CellStructure.str2structure(config.genotype)
+        return DynamicShapeTinyNet(channels, genotype, config.num_classes)
+    elif config.name == 'infer.nasnet-cifar':
+        from .cell_infers import NASNetonCIFAR
+        raise NotImplementedError
+    else:
+        raise ValueError('invalid network name : {:}'.format(config.name))
+
+
+# obtain the search space, i.e., a dict mapping the operation name into a python-function for this op
+def get_search_spaces(xtype, name) -> List[Text]:
+    if xtype == 'cell' or xtype == 'tss':  # The topology search space.
+        from .cell_operations import SearchSpaceNames
+        assert name in SearchSpaceNames, 'invalid name [{:}] in {:}'.format(name, SearchSpaceNames.keys())
+        return SearchSpaceNames[name]
+    elif xtype == 'sss':  # The size search space.
+        if name in ['nats-bench', 'nats-bench-size']:
+            return {'candidates': [8, 16, 24, 32, 40, 48, 56, 64],
+                    'numbers': 5}
+        else:
+            raise ValueError('Invalid name : {:}'.format(name))
+    else:
+        raise ValueError('invalid search-space type is {:}'.format(xtype))
+
+
+def get_cifar_models(config, extra_path=None):
+    super_type = getattr(config, 'super_type', 'basic')
+    if super_type == 'basic':
+        from .CifarResNet import CifarResNet
+        from .CifarDenseNet import DenseNet
+        from .CifarWideResNet import CifarWideResNet
+        if config.arch == 'resnet':
+            return CifarResNet(config.module, config.depth, config.class_num, config.zero_init_residual)
+        elif config.arch == 'densenet':
+            return DenseNet(config.growthRate, config.depth, config.reduction, config.class_num, config.bottleneck)
+        elif config.arch == 'wideresnet':
+            return CifarWideResNet(config.depth, config.wide_factor, config.class_num, config.dropout)
+        else:
+            raise ValueError('invalid module type : {:}'.format(config.arch))
+    elif super_type.startswith('infer'):
+        from .shape_infers import InferWidthCifarResNet
+        from .shape_infers import InferDepthCifarResNet
+        from .shape_infers import InferCifarResNet
+        from .cell_infers import NASNetonCIFAR
+        assert len(super_type.split('-')) == 2, 'invalid super_type : {:}'.format(super_type)
+        infer_mode = super_type.split('-')[1]
+        if infer_mode == 'width':
+            return InferWidthCifarResNet(config.module, config.depth, config.xchannels, config.class_num,
+                                         config.zero_init_residual)
+        elif infer_mode == 'depth':
+            return InferDepthCifarResNet(config.module, config.depth, config.xblocks, config.class_num,
+                                         config.zero_init_residual)
+        elif infer_mode == 'shape':
+            return InferCifarResNet(config.module, config.depth, config.xblocks, config.xchannels, config.class_num,
+                                    config.zero_init_residual)
+        elif infer_mode == 'nasnet.cifar':
+            genotype = config.genotype
+            if extra_path is not None:  # reload genotype by extra_path
+                if not osp.isfile(extra_path): raise ValueError('invalid extra_path : {:}'.format(extra_path))
+                xdata = torch.load(extra_path)
+                current_epoch = xdata['epoch']
+                genotype = xdata['genotypes'][current_epoch - 1]
+            C = config.C if hasattr(config, 'C') else config.ichannel
+            N = config.N if hasattr(config, 'N') else config.layers
+            return NASNetonCIFAR(C, N, config.stem_multi, config.class_num, genotype, config.auxiliary)
+        else:
+            raise ValueError('invalid infer-mode : {:}'.format(infer_mode))
+    else:
+        raise ValueError('invalid super-type : {:}'.format(super_type))
+
+
+def get_imagenet_models(config):
+    super_type = getattr(config, 'super_type', 'basic')
+    if super_type == 'basic':
+        from .ImageNet_ResNet import ResNet
+        from .ImageNet_MobileNetV2 import MobileNetV2
+        if config.arch == 'resnet':
+            return ResNet(config.block_name, config.layers, config.deep_stem, config.class_num,
+                          config.zero_init_residual, config.groups, config.width_per_group)
+        elif config.arch == 'mobilenet_v2':
+            return MobileNetV2(config.class_num, config.width_multi, config.input_channel, config.last_channel,
+                               'InvertedResidual', config.dropout)
+        else:
+            raise ValueError('invalid arch : {:}'.format(config.arch))
+    elif super_type.startswith('infer'):  # NAS searched architecture
+        assert len(super_type.split('-')) == 2, 'invalid super_type : {:}'.format(super_type)
+        infer_mode = super_type.split('-')[1]
+        if infer_mode == 'shape':
+            from .shape_infers import InferImagenetResNet
+            from .shape_infers import InferMobileNetV2
+            if config.arch == 'resnet':
+                return InferImagenetResNet(config.block_name, config.layers, config.xblocks, config.xchannels,
+                                           config.deep_stem, config.class_num, config.zero_init_residual)
+            elif config.arch == "MobileNetV2":
+                return InferMobileNetV2(config.class_num, config.xchannels, config.xblocks, config.dropout)
+            else:
+                raise ValueError('invalid arch-mode : {:}'.format(config.arch))
+        else:
+            raise ValueError('invalid infer-mode : {:}'.format(infer_mode))
+    else:
+        raise ValueError('invalid super-type : {:}'.format(super_type))
+
+
+# Try to obtain the network by config.
+def obtain_model(config, extra_path=None):
+    if config.dataset == 'cifar':
+        return get_cifar_models(config, extra_path)
+    elif config.dataset == 'imagenet':
+        return get_imagenet_models(config)
+    else:
+        raise ValueError('invalid dataset in the model config : {:}'.format(config))
+
+
+def obtain_search_model(config):
+    if config.dataset == 'cifar':
+        if config.arch == 'resnet':
+            from .shape_searchs import SearchWidthCifarResNet
+            from .shape_searchs import SearchDepthCifarResNet
+            from .shape_searchs import SearchShapeCifarResNet
+            if config.search_mode == 'width':
+                return SearchWidthCifarResNet(config.module, config.depth, config.class_num)
+            elif config.search_mode == 'depth':
+                return SearchDepthCifarResNet(config.module, config.depth, config.class_num)
+            elif config.search_mode == 'shape':
+                return SearchShapeCifarResNet(config.module, config.depth, config.class_num)
+            else:
+                raise ValueError('invalid search mode : {:}'.format(config.search_mode))
+        elif config.arch == 'simres':
+            from .shape_searchs import SearchWidthSimResNet
+            if config.search_mode == 'width':
+                return SearchWidthSimResNet(config.depth, config.class_num)
+            else:
+                raise ValueError('invalid search mode : {:}'.format(config.search_mode))
+        else:
+            raise ValueError('invalid arch : {:} for dataset [{:}]'.format(config.arch, config.dataset))
+    elif config.dataset == 'imagenet':
+        from .shape_searchs import SearchShapeImagenetResNet
+        assert config.search_mode == 'shape', 'invalid search-mode : {:}'.format(config.search_mode)
+        if config.arch == 'resnet':
+            return SearchShapeImagenetResNet(config.block_name, config.layers, config.deep_stem, config.class_num)
+        else:
+            raise ValueError('invalid model config : {:}'.format(config))
+    else:
+        raise ValueError('invalid dataset in the model config : {:}'.format(config))
+
+
+def load_net_from_checkpoint(checkpoint):
+    assert osp.isfile(checkpoint), 'checkpoint {:} does not exist'.format(checkpoint)
+    checkpoint = torch.load(checkpoint)
+    model_config = dict2config(checkpoint['model-config'], None)
+    model = obtain_model(model_config)
+    model.load_state_dict(checkpoint['base-model'])
+    return model
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_infers/nasnet_cifar.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_infers/nasnet_cifar.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-#####################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019.01 #
-#####################################################
-import torch
-import torch.nn as nn
-from copy import deepcopy
-from .cells import NASNetInferCell as InferCell, AuxiliaryHeadCIFAR
-
-
-# The macro structure is based on NASNet
-class NASNetonCIFAR(nn.Module):
-
-    def __init__(self, C, N, stem_multiplier, num_classes, genotype, auxiliary, affine=True, track_running_stats=True):
-        super(NASNetonCIFAR, self).__init__()
-        self._C = C
-        self._layerN = N
-        self.stem = nn.Sequential(
-            nn.Conv2d(3, C * stem_multiplier, kernel_size=3, padding=1, bias=False),
-            nn.BatchNorm2d(C * stem_multiplier))
-
-        # config for each layer
-        layer_channels = [C] * N + [C * 2] + [C * 2] * (N - 1) + [C * 4] + [C * 4] * (N - 1)
-        layer_reductions = [False] * N + [True] + [False] * (N - 1) + [True] + [False] * (N - 1)
-
-        C_prev_prev, C_prev, C_curr, reduction_prev = C * stem_multiplier, C * stem_multiplier, C, False
-        self.auxiliary_index = None
-        self.auxiliary_head = None
-        self.cells = nn.ModuleList()
-        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
-            cell = InferCell(genotype, C_prev_prev, C_prev, C_curr, reduction, reduction_prev, affine,
-                             track_running_stats)
-            self.cells.append(cell)
-            C_prev_prev, C_prev, reduction_prev = C_prev, cell._multiplier * C_curr, reduction
-            if reduction and C_curr == C * 4 and auxiliary:
-                self.auxiliary_head = AuxiliaryHeadCIFAR(C_prev, num_classes)
-                self.auxiliary_index = index
-        self._Layer = len(self.cells)
-        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev), nn.ReLU(inplace=True))
-        self.global_pooling = nn.AdaptiveAvgPool2d(1)
-        self.classifier = nn.Linear(C_prev, num_classes)
-        self.drop_path_prob = -1
-
-    def update_drop_path(self, drop_path_prob):
-        self.drop_path_prob = drop_path_prob
-
-    def auxiliary_param(self):
-        if self.auxiliary_head is None:
-            return []
-        else:
-            return list(self.auxiliary_head.parameters())
-
-    def get_message(self):
-        string = self.extra_repr()
-        for i, cell in enumerate(self.cells):
-            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
-        return string
-
-    def extra_repr(self):
-        return ('{name}(C={_C}, N={_layerN}, L={_Layer})'.format(name=self.__class__.__name__, **self.__dict__))
-
-    def forward(self, inputs):
-        stem_feature, logits_aux = self.stem(inputs), None
-        cell_results = [stem_feature, stem_feature]
-        for i, cell in enumerate(self.cells):
-            cell_feature = cell(cell_results[-2], cell_results[-1], self.drop_path_prob)
-            cell_results.append(cell_feature)
-            if self.auxiliary_index is not None and i == self.auxiliary_index and self.training:
-                logits_aux = self.auxiliary_head(cell_results[-1])
-        out = self.lastact(cell_results[-1])
-        out = self.global_pooling(out)
-        out = out.view(out.size(0), -1)
-        logits = self.classifier(out)
-        if logits_aux is None:
-            return out, logits
-        else:
-            return out, [logits, logits_aux]
+#####################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019.01 #
+#####################################################
+import torch
+import torch.nn as nn
+from copy import deepcopy
+from .cells import NASNetInferCell as InferCell, AuxiliaryHeadCIFAR
+
+
+# The macro structure is based on NASNet
+class NASNetonCIFAR(nn.Module):
+
+    def __init__(self, C, N, stem_multiplier, num_classes, genotype, auxiliary, affine=True, track_running_stats=True):
+        super(NASNetonCIFAR, self).__init__()
+        self._C = C
+        self._layerN = N
+        self.stem = nn.Sequential(
+            nn.Conv2d(3, C * stem_multiplier, kernel_size=3, padding=1, bias=False),
+            nn.BatchNorm2d(C * stem_multiplier))
+
+        # config for each layer
+        layer_channels = [C] * N + [C * 2] + [C * 2] * (N - 1) + [C * 4] + [C * 4] * (N - 1)
+        layer_reductions = [False] * N + [True] + [False] * (N - 1) + [True] + [False] * (N - 1)
+
+        C_prev_prev, C_prev, C_curr, reduction_prev = C * stem_multiplier, C * stem_multiplier, C, False
+        self.auxiliary_index = None
+        self.auxiliary_head = None
+        self.cells = nn.ModuleList()
+        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
+            cell = InferCell(genotype, C_prev_prev, C_prev, C_curr, reduction, reduction_prev, affine,
+                             track_running_stats)
+            self.cells.append(cell)
+            C_prev_prev, C_prev, reduction_prev = C_prev, cell._multiplier * C_curr, reduction
+            if reduction and C_curr == C * 4 and auxiliary:
+                self.auxiliary_head = AuxiliaryHeadCIFAR(C_prev, num_classes)
+                self.auxiliary_index = index
+        self._Layer = len(self.cells)
+        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev), nn.ReLU(inplace=True))
+        self.global_pooling = nn.AdaptiveAvgPool2d(1)
+        self.classifier = nn.Linear(C_prev, num_classes)
+        self.drop_path_prob = -1
+
+    def update_drop_path(self, drop_path_prob):
+        self.drop_path_prob = drop_path_prob
+
+    def auxiliary_param(self):
+        if self.auxiliary_head is None:
+            return []
+        else:
+            return list(self.auxiliary_head.parameters())
+
+    def get_message(self):
+        string = self.extra_repr()
+        for i, cell in enumerate(self.cells):
+            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
+        return string
+
+    def extra_repr(self):
+        return ('{name}(C={_C}, N={_layerN}, L={_Layer})'.format(name=self.__class__.__name__, **self.__dict__))
+
+    def forward(self, inputs):
+        stem_feature, logits_aux = self.stem(inputs), None
+        cell_results = [stem_feature, stem_feature]
+        for i, cell in enumerate(self.cells):
+            cell_feature = cell(cell_results[-2], cell_results[-1], self.drop_path_prob)
+            cell_results.append(cell_feature)
+            if self.auxiliary_index is not None and i == self.auxiliary_index and self.training:
+                logits_aux = self.auxiliary_head(cell_results[-1])
+        out = self.lastact(cell_results[-1])
+        out = self.global_pooling(out)
+        out = out.view(out.size(0), -1)
+        logits = self.classifier(out)
+        if logits_aux is None:
+            return out, logits
+        else:
+            return out, [logits, logits_aux]
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_operations.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_operations.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,356 +1,356 @@
-##################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
-##################################################
-import torch
-import torch.nn as nn
-
-__all__ = ['OPS', 'RAW_OP_CLASSES', 'ResNetBasicblock', 'SearchSpaceNames']
-
-OPS = {
-    'none': lambda C_in, C_out, stride, affine, track_running_stats: Zero(C_in, C_out, stride),
-    'avg_pool_3x3': lambda C_in, C_out, stride, affine, track_running_stats: POOLING(C_in, C_out, stride, 'avg', affine,
-                                                                                     track_running_stats),
-    'max_pool_3x3': lambda C_in, C_out, stride, affine, track_running_stats: POOLING(C_in, C_out, stride, 'max', affine,
-                                                                                     track_running_stats),
-    'nor_conv_7x7': lambda C_in, C_out, stride, affine, track_running_stats: ReLUConvBN(C_in, C_out, (7, 7),
-                                                                                        (stride, stride), (3, 3),
-                                                                                        (1, 1), affine,
-                                                                                        track_running_stats),
-    'nor_conv_3x3': lambda C_in, C_out, stride, affine, track_running_stats: ReLUConvBN(C_in, C_out, (3, 3),
-                                                                                        (stride, stride), (1, 1),
-                                                                                        (1, 1), affine,
-                                                                                        track_running_stats),
-    'nor_conv_1x1': lambda C_in, C_out, stride, affine, track_running_stats: ReLUConvBN(C_in, C_out, (1, 1),
-                                                                                        (stride, stride), (0, 0),
-                                                                                        (1, 1), affine,
-                                                                                        track_running_stats),
-    'dua_sepc_3x3': lambda C_in, C_out, stride, affine, track_running_stats: DualSepConv(C_in, C_out, (3, 3),
-                                                                                         (stride, stride), (1, 1),
-                                                                                         (1, 1), affine,
-                                                                                         track_running_stats),
-    'dua_sepc_5x5': lambda C_in, C_out, stride, affine, track_running_stats: DualSepConv(C_in, C_out, (5, 5),
-                                                                                         (stride, stride), (2, 2),
-                                                                                         (1, 1), affine,
-                                                                                         track_running_stats),
-    'dil_sepc_3x3': lambda C_in, C_out, stride, affine, track_running_stats: SepConv(C_in, C_out, (3, 3),
-                                                                                     (stride, stride), (2, 2), (2, 2),
-                                                                                     affine, track_running_stats),
-    'dil_sepc_5x5': lambda C_in, C_out, stride, affine, track_running_stats: SepConv(C_in, C_out, (5, 5),
-                                                                                     (stride, stride), (4, 4), (2, 2),
-                                                                                     affine, track_running_stats),
-    'skip_connect': lambda C_in, C_out, stride, affine,
-                           track_running_stats: Identity() if stride == 1 and C_in == C_out else FactorizedReduce(C_in,
-                                                                                                                  C_out,
-                                                                                                                  stride,
-                                                                                                                  affine,
-                                                                                                                  track_running_stats),
-}
-
-CONNECT_NAS_BENCHMARK = ['none', 'skip_connect', 'nor_conv_3x3']
-NAS_BENCH_201 = ['none', 'skip_connect', 'nor_conv_1x1', 'nor_conv_3x3', 'avg_pool_3x3']
-DARTS_SPACE = ['none', 'skip_connect', 'dua_sepc_3x3', 'dua_sepc_5x5', 'dil_sepc_3x3', 'dil_sepc_5x5', 'avg_pool_3x3',
-               'max_pool_3x3']
-
-SearchSpaceNames = {'connect-nas': CONNECT_NAS_BENCHMARK,
-                    'nats-bench': NAS_BENCH_201,
-                    'nas-bench-201': NAS_BENCH_201,
-                    'darts': DARTS_SPACE}
-
-
-class ReLUConvBN(nn.Module):
-
-    def __init__(self, C_in, C_out, kernel_size, stride, padding, dilation, affine, track_running_stats=True):
-        super(ReLUConvBN, self).__init__()
-        self.op = nn.Sequential(
-            nn.ReLU(inplace=False),
-            nn.Conv2d(C_in, C_out, kernel_size, stride=stride, padding=padding, dilation=dilation, bias=not affine),
-            nn.BatchNorm2d(C_out, affine=affine, track_running_stats=track_running_stats)
-        )
-
-    def forward(self, x):
-        return self.op(x)
-
-
-class SepConv(nn.Module):
-
-    def __init__(self, C_in, C_out, kernel_size, stride, padding, dilation, affine, track_running_stats=True):
-        super(SepConv, self).__init__()
-        self.op = nn.Sequential(
-            nn.ReLU(inplace=False),
-            nn.Conv2d(C_in, C_in, kernel_size=kernel_size, stride=stride, padding=padding, dilation=dilation,
-                      groups=C_in, bias=False),
-            nn.Conv2d(C_in, C_out, kernel_size=1, padding=0, bias=not affine),
-            nn.BatchNorm2d(C_out, affine=affine, track_running_stats=track_running_stats),
-        )
-
-    def forward(self, x):
-        return self.op(x)
-
-
-class DualSepConv(nn.Module):
-
-    def __init__(self, C_in, C_out, kernel_size, stride, padding, dilation, affine, track_running_stats=True):
-        super(DualSepConv, self).__init__()
-        self.op_a = SepConv(C_in, C_in, kernel_size, stride, padding, dilation, affine, track_running_stats)
-        self.op_b = SepConv(C_in, C_out, kernel_size, 1, padding, dilation, affine, track_running_stats)
-
-    def forward(self, x):
-        x = self.op_a(x)
-        x = self.op_b(x)
-        return x
-
-
-class ResNetBasicblock(nn.Module):
-
-    def __init__(self, inplanes, planes, stride, affine=True, track_running_stats=True):
-        super(ResNetBasicblock, self).__init__()
-        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
-        self.conv_a = ReLUConvBN(inplanes, planes, 3, stride, 1, 1, affine, track_running_stats)
-        self.conv_b = ReLUConvBN(planes, planes, 3, 1, 1, 1, affine, track_running_stats)
-        if stride == 2:
-            self.downsample = nn.Sequential(
-                nn.AvgPool2d(kernel_size=2, stride=2, padding=0),
-                nn.Conv2d(inplanes, planes, kernel_size=1, stride=1, padding=0, bias=False))
-        elif inplanes != planes:
-            self.downsample = ReLUConvBN(inplanes, planes, 1, 1, 0, 1, affine, track_running_stats)
-        else:
-            self.downsample = None
-        self.in_dim = inplanes
-        self.out_dim = planes
-        self.stride = stride
-        self.num_conv = 2
-
-    def extra_repr(self):
-        string = '{name}(inC={in_dim}, outC={out_dim}, stride={stride})'.format(name=self.__class__.__name__,
-                                                                                **self.__dict__)
-        return string
-
-    def forward(self, inputs):
-
-        basicblock = self.conv_a(inputs)
-        basicblock = self.conv_b(basicblock)
-
-        if self.downsample is not None:
-            residual = self.downsample(inputs)
-        else:
-            residual = inputs
-        return residual + basicblock
-
-
-class POOLING(nn.Module):
-
-    def __init__(self, C_in, C_out, stride, mode, affine=True, track_running_stats=True):
-        super(POOLING, self).__init__()
-        if C_in == C_out:
-            self.preprocess = None
-        else:
-            self.preprocess = ReLUConvBN(C_in, C_out, 1, 1, 0, 1, affine, track_running_stats)
-        if mode == 'avg':
-            self.op = nn.AvgPool2d(3, stride=stride, padding=1, count_include_pad=False)
-        elif mode == 'max':
-            self.op = nn.MaxPool2d(3, stride=stride, padding=1)
-        else:
-            raise ValueError('Invalid mode={:} in POOLING'.format(mode))
-
-    def forward(self, inputs):
-        if self.preprocess:
-            x = self.preprocess(inputs)
-        else:
-            x = inputs
-        return self.op(x)
-
-
-class Identity(nn.Module):
-
-    def __init__(self):
-        super(Identity, self).__init__()
-
-    def forward(self, x):
-        return x
-
-
-class Zero(nn.Module):
-
-    def __init__(self, C_in, C_out, stride):
-        super(Zero, self).__init__()
-        self.C_in = C_in
-        self.C_out = C_out
-        self.stride = stride
-        self.is_zero = True
-
-    def forward(self, x):
-        if self.C_in == self.C_out:
-            if self.stride == 1:
-                return x.mul(0.)
-            else:
-                return x[:, :, ::self.stride, ::self.stride].mul(0.)
-        else:
-            shape = list(x.shape)
-            shape[1] = self.C_out
-            zeros = x.new_zeros(shape, dtype=x.dtype, device=x.device)
-            return zeros
-
-    def extra_repr(self):
-        return 'C_in={C_in}, C_out={C_out}, stride={stride}'.format(**self.__dict__)
-
-
-class FactorizedReduce(nn.Module):
-
-    def __init__(self, C_in, C_out, stride, affine, track_running_stats):
-        super(FactorizedReduce, self).__init__()
-        self.stride = stride
-        self.C_in = C_in
-        self.C_out = C_out
-        self.relu = nn.ReLU(inplace=False)
-        if stride == 2:
-            # assert C_out % 2 == 0, 'C_out : {:}'.format(C_out)
-            C_outs = [C_out // 2, C_out - C_out // 2]
-            self.convs = nn.ModuleList()
-            for i in range(2):
-                self.convs.append(nn.Conv2d(C_in, C_outs[i], 1, stride=stride, padding=0, bias=not affine))
-            self.pad = nn.ConstantPad2d((0, 1, 0, 1), 0)
-        elif stride == 1:
-            self.conv = nn.Conv2d(C_in, C_out, 1, stride=stride, padding=0, bias=not affine)
-        else:
-            raise ValueError('Invalid stride : {:}'.format(stride))
-        self.bn = nn.BatchNorm2d(C_out, affine=affine, track_running_stats=track_running_stats)
-
-    def forward(self, x):
-        if self.stride == 2:
-            x = self.relu(x)
-            y = self.pad(x)
-            out = torch.cat([self.convs[0](x), self.convs[1](y[:, :, 1:, 1:])], dim=1)
-        else:
-            out = self.conv(x)
-        out = self.bn(out)
-        return out
-
-    def extra_repr(self):
-        return 'C_in={C_in}, C_out={C_out}, stride={stride}'.format(**self.__dict__)
-
-
-# Auto-ReID: Searching for a Part-Aware ConvNet for Person Re-Identification, ICCV 2019
-class PartAwareOp(nn.Module):
-
-    def __init__(self, C_in, C_out, stride, part=4):
-        super().__init__()
-        self.part = 4
-        self.hidden = C_in // 3
-        self.avg_pool = nn.AdaptiveAvgPool2d(1)
-        self.local_conv_list = nn.ModuleList()
-        for i in range(self.part):
-            self.local_conv_list.append(
-                nn.Sequential(nn.ReLU(), nn.Conv2d(C_in, self.hidden, 1), nn.BatchNorm2d(self.hidden, affine=True))
-            )
-        self.W_K = nn.Linear(self.hidden, self.hidden)
-        self.W_Q = nn.Linear(self.hidden, self.hidden)
-
-        if stride == 2:
-            self.last = FactorizedReduce(C_in + self.hidden, C_out, 2)
-        elif stride == 1:
-            self.last = FactorizedReduce(C_in + self.hidden, C_out, 1)
-        else:
-            raise ValueError('Invalid Stride : {:}'.format(stride))
-
-    def forward(self, x):
-        batch, C, H, W = x.size()
-        assert H >= self.part, 'input size too small : {:} vs {:}'.format(x.shape, self.part)
-        IHs = [0]
-        for i in range(self.part): IHs.append(min(H, int((i + 1) * (float(H) / self.part))))
-        local_feat_list = []
-        for i in range(self.part):
-            feature = x[:, :, IHs[i]:IHs[i + 1], :]
-            xfeax = self.avg_pool(feature)
-            xfea = self.local_conv_list[i](xfeax)
-            local_feat_list.append(xfea)
-        part_feature = torch.cat(local_feat_list, dim=2).view(batch, -1, self.part)
-        part_feature = part_feature.transpose(1, 2).contiguous()
-        part_K = self.W_K(part_feature)
-        part_Q = self.W_Q(part_feature).transpose(1, 2).contiguous()
-        weight_att = torch.bmm(part_K, part_Q)
-        attention = torch.softmax(weight_att, dim=2)
-        aggreateF = torch.bmm(attention, part_feature).transpose(1, 2).contiguous()
-        features = []
-        for i in range(self.part):
-            feature = aggreateF[:, :, i:i + 1].expand(batch, self.hidden, IHs[i + 1] - IHs[i])
-            feature = feature.view(batch, self.hidden, IHs[i + 1] - IHs[i], 1)
-            features.append(feature)
-        features = torch.cat(features, dim=2).expand(batch, self.hidden, H, W)
-        final_fea = torch.cat((x, features), dim=1)
-        outputs = self.last(final_fea)
-        return outputs
-
-
-def drop_path(x, drop_prob):
-    if drop_prob > 0.:
-        keep_prob = 1. - drop_prob
-        mask = x.new_zeros(x.size(0), 1, 1, 1)
-        mask = mask.bernoulli_(keep_prob)
-        x = torch.div(x, keep_prob)
-        x.mul_(mask)
-    return x
-
-
-# Searching for A Robust Neural Architecture in Four GPU Hours
-class GDAS_Reduction_Cell(nn.Module):
-
-    def __init__(self, C_prev_prev, C_prev, C, reduction_prev, affine, track_running_stats):
-        super(GDAS_Reduction_Cell, self).__init__()
-        if reduction_prev:
-            self.preprocess0 = FactorizedReduce(C_prev_prev, C, 2, affine, track_running_stats)
-        else:
-            self.preprocess0 = ReLUConvBN(C_prev_prev, C, 1, 1, 0, 1, affine, track_running_stats)
-        self.preprocess1 = ReLUConvBN(C_prev, C, 1, 1, 0, 1, affine, track_running_stats)
-
-        self.reduction = True
-        self.ops1 = nn.ModuleList(
-            [nn.Sequential(
-                nn.ReLU(inplace=False),
-                nn.Conv2d(C, C, (1, 3), stride=(1, 2), padding=(0, 1), groups=8, bias=not affine),
-                nn.Conv2d(C, C, (3, 1), stride=(2, 1), padding=(1, 0), groups=8, bias=not affine),
-                nn.BatchNorm2d(C, affine=affine, track_running_stats=track_running_stats),
-                nn.ReLU(inplace=False),
-                nn.Conv2d(C, C, 1, stride=1, padding=0, bias=not affine),
-                nn.BatchNorm2d(C, affine=affine, track_running_stats=track_running_stats)),
-                nn.Sequential(
-                    nn.ReLU(inplace=False),
-                    nn.Conv2d(C, C, (1, 3), stride=(1, 2), padding=(0, 1), groups=8, bias=not affine),
-                    nn.Conv2d(C, C, (3, 1), stride=(2, 1), padding=(1, 0), groups=8, bias=not affine),
-                    nn.BatchNorm2d(C, affine=affine, track_running_stats=track_running_stats),
-                    nn.ReLU(inplace=False),
-                    nn.Conv2d(C, C, 1, stride=1, padding=0, bias=not affine),
-                    nn.BatchNorm2d(C, affine=affine, track_running_stats=track_running_stats))])
-
-        self.ops2 = nn.ModuleList(
-            [nn.Sequential(
-                nn.MaxPool2d(3, stride=2, padding=1),
-                nn.BatchNorm2d(C, affine=affine, track_running_stats=track_running_stats)),
-                nn.Sequential(
-                    nn.MaxPool2d(3, stride=2, padding=1),
-                    nn.BatchNorm2d(C, affine=affine, track_running_stats=track_running_stats))])
-
-    @property
-    def multiplier(self):
-        return 4
-
-    def forward(self, s0, s1, drop_prob=-1):
-        s0 = self.preprocess0(s0)
-        s1 = self.preprocess1(s1)
-
-        X0 = self.ops1[0](s0)
-        X1 = self.ops1[1](s1)
-        if self.training and drop_prob > 0.:
-            X0, X1 = drop_path(X0, drop_prob), drop_path(X1, drop_prob)
-
-        # X2 = self.ops2[0] (X0+X1)
-        X2 = self.ops2[0](s0)
-        X3 = self.ops2[1](s1)
-        if self.training and drop_prob > 0.:
-            X2, X3 = drop_path(X2, drop_prob), drop_path(X3, drop_prob)
-        return torch.cat([X0, X1, X2, X3], dim=1)
-
-
-# To manage the useful classes in this file.
-RAW_OP_CLASSES = {
-    'gdas_reduction': GDAS_Reduction_Cell
-}
+##################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
+##################################################
+import torch
+import torch.nn as nn
+
+__all__ = ['OPS', 'RAW_OP_CLASSES', 'ResNetBasicblock', 'SearchSpaceNames']
+
+OPS = {
+    'none': lambda C_in, C_out, stride, affine, track_running_stats: Zero(C_in, C_out, stride),
+    'avg_pool_3x3': lambda C_in, C_out, stride, affine, track_running_stats: POOLING(C_in, C_out, stride, 'avg', affine,
+                                                                                     track_running_stats),
+    'max_pool_3x3': lambda C_in, C_out, stride, affine, track_running_stats: POOLING(C_in, C_out, stride, 'max', affine,
+                                                                                     track_running_stats),
+    'nor_conv_7x7': lambda C_in, C_out, stride, affine, track_running_stats: ReLUConvBN(C_in, C_out, (7, 7),
+                                                                                        (stride, stride), (3, 3),
+                                                                                        (1, 1), affine,
+                                                                                        track_running_stats),
+    'nor_conv_3x3': lambda C_in, C_out, stride, affine, track_running_stats: ReLUConvBN(C_in, C_out, (3, 3),
+                                                                                        (stride, stride), (1, 1),
+                                                                                        (1, 1), affine,
+                                                                                        track_running_stats),
+    'nor_conv_1x1': lambda C_in, C_out, stride, affine, track_running_stats: ReLUConvBN(C_in, C_out, (1, 1),
+                                                                                        (stride, stride), (0, 0),
+                                                                                        (1, 1), affine,
+                                                                                        track_running_stats),
+    'dua_sepc_3x3': lambda C_in, C_out, stride, affine, track_running_stats: DualSepConv(C_in, C_out, (3, 3),
+                                                                                         (stride, stride), (1, 1),
+                                                                                         (1, 1), affine,
+                                                                                         track_running_stats),
+    'dua_sepc_5x5': lambda C_in, C_out, stride, affine, track_running_stats: DualSepConv(C_in, C_out, (5, 5),
+                                                                                         (stride, stride), (2, 2),
+                                                                                         (1, 1), affine,
+                                                                                         track_running_stats),
+    'dil_sepc_3x3': lambda C_in, C_out, stride, affine, track_running_stats: SepConv(C_in, C_out, (3, 3),
+                                                                                     (stride, stride), (2, 2), (2, 2),
+                                                                                     affine, track_running_stats),
+    'dil_sepc_5x5': lambda C_in, C_out, stride, affine, track_running_stats: SepConv(C_in, C_out, (5, 5),
+                                                                                     (stride, stride), (4, 4), (2, 2),
+                                                                                     affine, track_running_stats),
+    'skip_connect': lambda C_in, C_out, stride, affine,
+                           track_running_stats: Identity() if stride == 1 and C_in == C_out else FactorizedReduce(C_in,
+                                                                                                                  C_out,
+                                                                                                                  stride,
+                                                                                                                  affine,
+                                                                                                                  track_running_stats),
+}
+
+CONNECT_NAS_BENCHMARK = ['none', 'skip_connect', 'nor_conv_3x3']
+NAS_BENCH_201 = ['none', 'skip_connect', 'nor_conv_1x1', 'nor_conv_3x3', 'avg_pool_3x3']
+DARTS_SPACE = ['none', 'skip_connect', 'dua_sepc_3x3', 'dua_sepc_5x5', 'dil_sepc_3x3', 'dil_sepc_5x5', 'avg_pool_3x3',
+               'max_pool_3x3']
+
+SearchSpaceNames = {'connect-nas': CONNECT_NAS_BENCHMARK,
+                    'nats-bench': NAS_BENCH_201,
+                    'nas-bench-201': NAS_BENCH_201,
+                    'darts': DARTS_SPACE}
+
+
+class ReLUConvBN(nn.Module):
+
+    def __init__(self, C_in, C_out, kernel_size, stride, padding, dilation, affine, track_running_stats=True):
+        super(ReLUConvBN, self).__init__()
+        self.op = nn.Sequential(
+            nn.ReLU(inplace=False),
+            nn.Conv2d(C_in, C_out, kernel_size, stride=stride, padding=padding, dilation=dilation, bias=not affine),
+            nn.BatchNorm2d(C_out, affine=affine, track_running_stats=track_running_stats)
+        )
+
+    def forward(self, x):
+        return self.op(x)
+
+
+class SepConv(nn.Module):
+
+    def __init__(self, C_in, C_out, kernel_size, stride, padding, dilation, affine, track_running_stats=True):
+        super(SepConv, self).__init__()
+        self.op = nn.Sequential(
+            nn.ReLU(inplace=False),
+            nn.Conv2d(C_in, C_in, kernel_size=kernel_size, stride=stride, padding=padding, dilation=dilation,
+                      groups=C_in, bias=False),
+            nn.Conv2d(C_in, C_out, kernel_size=1, padding=0, bias=not affine),
+            nn.BatchNorm2d(C_out, affine=affine, track_running_stats=track_running_stats),
+        )
+
+    def forward(self, x):
+        return self.op(x)
+
+
+class DualSepConv(nn.Module):
+
+    def __init__(self, C_in, C_out, kernel_size, stride, padding, dilation, affine, track_running_stats=True):
+        super(DualSepConv, self).__init__()
+        self.op_a = SepConv(C_in, C_in, kernel_size, stride, padding, dilation, affine, track_running_stats)
+        self.op_b = SepConv(C_in, C_out, kernel_size, 1, padding, dilation, affine, track_running_stats)
+
+    def forward(self, x):
+        x = self.op_a(x)
+        x = self.op_b(x)
+        return x
+
+
+class ResNetBasicblock(nn.Module):
+
+    def __init__(self, inplanes, planes, stride, affine=True, track_running_stats=True):
+        super(ResNetBasicblock, self).__init__()
+        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
+        self.conv_a = ReLUConvBN(inplanes, planes, 3, stride, 1, 1, affine, track_running_stats)
+        self.conv_b = ReLUConvBN(planes, planes, 3, 1, 1, 1, affine, track_running_stats)
+        if stride == 2:
+            self.downsample = nn.Sequential(
+                nn.AvgPool2d(kernel_size=2, stride=2, padding=0),
+                nn.Conv2d(inplanes, planes, kernel_size=1, stride=1, padding=0, bias=False))
+        elif inplanes != planes:
+            self.downsample = ReLUConvBN(inplanes, planes, 1, 1, 0, 1, affine, track_running_stats)
+        else:
+            self.downsample = None
+        self.in_dim = inplanes
+        self.out_dim = planes
+        self.stride = stride
+        self.num_conv = 2
+
+    def extra_repr(self):
+        string = '{name}(inC={in_dim}, outC={out_dim}, stride={stride})'.format(name=self.__class__.__name__,
+                                                                                **self.__dict__)
+        return string
+
+    def forward(self, inputs):
+
+        basicblock = self.conv_a(inputs)
+        basicblock = self.conv_b(basicblock)
+
+        if self.downsample is not None:
+            residual = self.downsample(inputs)
+        else:
+            residual = inputs
+        return residual + basicblock
+
+
+class POOLING(nn.Module):
+
+    def __init__(self, C_in, C_out, stride, mode, affine=True, track_running_stats=True):
+        super(POOLING, self).__init__()
+        if C_in == C_out:
+            self.preprocess = None
+        else:
+            self.preprocess = ReLUConvBN(C_in, C_out, 1, 1, 0, 1, affine, track_running_stats)
+        if mode == 'avg':
+            self.op = nn.AvgPool2d(3, stride=stride, padding=1, count_include_pad=False)
+        elif mode == 'max':
+            self.op = nn.MaxPool2d(3, stride=stride, padding=1)
+        else:
+            raise ValueError('Invalid mode={:} in POOLING'.format(mode))
+
+    def forward(self, inputs):
+        if self.preprocess:
+            x = self.preprocess(inputs)
+        else:
+            x = inputs
+        return self.op(x)
+
+
+class Identity(nn.Module):
+
+    def __init__(self):
+        super(Identity, self).__init__()
+
+    def forward(self, x):
+        return x
+
+
+class Zero(nn.Module):
+
+    def __init__(self, C_in, C_out, stride):
+        super(Zero, self).__init__()
+        self.C_in = C_in
+        self.C_out = C_out
+        self.stride = stride
+        self.is_zero = True
+
+    def forward(self, x):
+        if self.C_in == self.C_out:
+            if self.stride == 1:
+                return x.mul(0.)
+            else:
+                return x[:, :, ::self.stride, ::self.stride].mul(0.)
+        else:
+            shape = list(x.shape)
+            shape[1] = self.C_out
+            zeros = x.new_zeros(shape, dtype=x.dtype, device=x.device)
+            return zeros
+
+    def extra_repr(self):
+        return 'C_in={C_in}, C_out={C_out}, stride={stride}'.format(**self.__dict__)
+
+
+class FactorizedReduce(nn.Module):
+
+    def __init__(self, C_in, C_out, stride, affine, track_running_stats):
+        super(FactorizedReduce, self).__init__()
+        self.stride = stride
+        self.C_in = C_in
+        self.C_out = C_out
+        self.relu = nn.ReLU(inplace=False)
+        if stride == 2:
+            # assert C_out % 2 == 0, 'C_out : {:}'.format(C_out)
+            C_outs = [C_out // 2, C_out - C_out // 2]
+            self.convs = nn.ModuleList()
+            for i in range(2):
+                self.convs.append(nn.Conv2d(C_in, C_outs[i], 1, stride=stride, padding=0, bias=not affine))
+            self.pad = nn.ConstantPad2d((0, 1, 0, 1), 0)
+        elif stride == 1:
+            self.conv = nn.Conv2d(C_in, C_out, 1, stride=stride, padding=0, bias=not affine)
+        else:
+            raise ValueError('Invalid stride : {:}'.format(stride))
+        self.bn = nn.BatchNorm2d(C_out, affine=affine, track_running_stats=track_running_stats)
+
+    def forward(self, x):
+        if self.stride == 2:
+            x = self.relu(x)
+            y = self.pad(x)
+            out = torch.cat([self.convs[0](x), self.convs[1](y[:, :, 1:, 1:])], dim=1)
+        else:
+            out = self.conv(x)
+        out = self.bn(out)
+        return out
+
+    def extra_repr(self):
+        return 'C_in={C_in}, C_out={C_out}, stride={stride}'.format(**self.__dict__)
+
+
+# Auto-ReID: Searching for a Part-Aware ConvNet for Person Re-Identification, ICCV 2019
+class PartAwareOp(nn.Module):
+
+    def __init__(self, C_in, C_out, stride, part=4):
+        super().__init__()
+        self.part = 4
+        self.hidden = C_in // 3
+        self.avg_pool = nn.AdaptiveAvgPool2d(1)
+        self.local_conv_list = nn.ModuleList()
+        for i in range(self.part):
+            self.local_conv_list.append(
+                nn.Sequential(nn.ReLU(), nn.Conv2d(C_in, self.hidden, 1), nn.BatchNorm2d(self.hidden, affine=True))
+            )
+        self.W_K = nn.Linear(self.hidden, self.hidden)
+        self.W_Q = nn.Linear(self.hidden, self.hidden)
+
+        if stride == 2:
+            self.last = FactorizedReduce(C_in + self.hidden, C_out, 2)
+        elif stride == 1:
+            self.last = FactorizedReduce(C_in + self.hidden, C_out, 1)
+        else:
+            raise ValueError('Invalid Stride : {:}'.format(stride))
+
+    def forward(self, x):
+        batch, C, H, W = x.size()
+        assert H >= self.part, 'input size too small : {:} vs {:}'.format(x.shape, self.part)
+        IHs = [0]
+        for i in range(self.part): IHs.append(min(H, int((i + 1) * (float(H) / self.part))))
+        local_feat_list = []
+        for i in range(self.part):
+            feature = x[:, :, IHs[i]:IHs[i + 1], :]
+            xfeax = self.avg_pool(feature)
+            xfea = self.local_conv_list[i](xfeax)
+            local_feat_list.append(xfea)
+        part_feature = torch.cat(local_feat_list, dim=2).view(batch, -1, self.part)
+        part_feature = part_feature.transpose(1, 2).contiguous()
+        part_K = self.W_K(part_feature)
+        part_Q = self.W_Q(part_feature).transpose(1, 2).contiguous()
+        weight_att = torch.bmm(part_K, part_Q)
+        attention = torch.softmax(weight_att, dim=2)
+        aggreateF = torch.bmm(attention, part_feature).transpose(1, 2).contiguous()
+        features = []
+        for i in range(self.part):
+            feature = aggreateF[:, :, i:i + 1].expand(batch, self.hidden, IHs[i + 1] - IHs[i])
+            feature = feature.view(batch, self.hidden, IHs[i + 1] - IHs[i], 1)
+            features.append(feature)
+        features = torch.cat(features, dim=2).expand(batch, self.hidden, H, W)
+        final_fea = torch.cat((x, features), dim=1)
+        outputs = self.last(final_fea)
+        return outputs
+
+
+def drop_path(x, drop_prob):
+    if drop_prob > 0.:
+        keep_prob = 1. - drop_prob
+        mask = x.new_zeros(x.size(0), 1, 1, 1)
+        mask = mask.bernoulli_(keep_prob)
+        x = torch.div(x, keep_prob)
+        x.mul_(mask)
+    return x
+
+
+# Searching for A Robust Neural Architecture in Four GPU Hours
+class GDAS_Reduction_Cell(nn.Module):
+
+    def __init__(self, C_prev_prev, C_prev, C, reduction_prev, affine, track_running_stats):
+        super(GDAS_Reduction_Cell, self).__init__()
+        if reduction_prev:
+            self.preprocess0 = FactorizedReduce(C_prev_prev, C, 2, affine, track_running_stats)
+        else:
+            self.preprocess0 = ReLUConvBN(C_prev_prev, C, 1, 1, 0, 1, affine, track_running_stats)
+        self.preprocess1 = ReLUConvBN(C_prev, C, 1, 1, 0, 1, affine, track_running_stats)
+
+        self.reduction = True
+        self.ops1 = nn.ModuleList(
+            [nn.Sequential(
+                nn.ReLU(inplace=False),
+                nn.Conv2d(C, C, (1, 3), stride=(1, 2), padding=(0, 1), groups=8, bias=not affine),
+                nn.Conv2d(C, C, (3, 1), stride=(2, 1), padding=(1, 0), groups=8, bias=not affine),
+                nn.BatchNorm2d(C, affine=affine, track_running_stats=track_running_stats),
+                nn.ReLU(inplace=False),
+                nn.Conv2d(C, C, 1, stride=1, padding=0, bias=not affine),
+                nn.BatchNorm2d(C, affine=affine, track_running_stats=track_running_stats)),
+                nn.Sequential(
+                    nn.ReLU(inplace=False),
+                    nn.Conv2d(C, C, (1, 3), stride=(1, 2), padding=(0, 1), groups=8, bias=not affine),
+                    nn.Conv2d(C, C, (3, 1), stride=(2, 1), padding=(1, 0), groups=8, bias=not affine),
+                    nn.BatchNorm2d(C, affine=affine, track_running_stats=track_running_stats),
+                    nn.ReLU(inplace=False),
+                    nn.Conv2d(C, C, 1, stride=1, padding=0, bias=not affine),
+                    nn.BatchNorm2d(C, affine=affine, track_running_stats=track_running_stats))])
+
+        self.ops2 = nn.ModuleList(
+            [nn.Sequential(
+                nn.MaxPool2d(3, stride=2, padding=1),
+                nn.BatchNorm2d(C, affine=affine, track_running_stats=track_running_stats)),
+                nn.Sequential(
+                    nn.MaxPool2d(3, stride=2, padding=1),
+                    nn.BatchNorm2d(C, affine=affine, track_running_stats=track_running_stats))])
+
+    @property
+    def multiplier(self):
+        return 4
+
+    def forward(self, s0, s1, drop_prob=-1):
+        s0 = self.preprocess0(s0)
+        s1 = self.preprocess1(s1)
+
+        X0 = self.ops1[0](s0)
+        X1 = self.ops1[1](s1)
+        if self.training and drop_prob > 0.:
+            X0, X1 = drop_path(X0, drop_prob), drop_path(X1, drop_prob)
+
+        # X2 = self.ops2[0] (X0+X1)
+        X2 = self.ops2[0](s0)
+        X3 = self.ops2[1](s1)
+        if self.training and drop_prob > 0.:
+            X2, X3 = drop_path(X2, drop_prob), drop_path(X3, drop_prob)
+        return torch.cat([X0, X1, X2, X3], dim=1)
+
+
+# To manage the useful classes in this file.
+RAW_OP_CLASSES = {
+    'gdas_reduction': GDAS_Reduction_Cell
+}
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/__init__.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/__init__.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-##################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
-##################################################
-# The macro structure is defined in NAS-Bench-201
-from .search_model_darts import TinyNetworkDarts
-from .search_model_gdas import TinyNetworkGDAS
-from .search_model_setn import TinyNetworkSETN
-from .search_model_enas import TinyNetworkENAS
-from .search_model_random import TinyNetworkRANDOM
-from .generic_model import GenericNAS201Model
-from .genotypes import Structure as CellStructure, architectures as CellArchitectures
-# NASNet-based macro structure
-from .search_model_gdas_nasnet import NASNetworkGDAS
-from .search_model_gdas_frc_nasnet import NASNetworkGDAS_FRC
-from .search_model_darts_nasnet import NASNetworkDARTS
-
-nas201_super_nets = {'DARTS-V1': TinyNetworkDarts,
-                     "DARTS-V2": TinyNetworkDarts,
-                     "GDAS": TinyNetworkGDAS,
-                     "SETN": TinyNetworkSETN,
-                     "ENAS": TinyNetworkENAS,
-                     "RANDOM": TinyNetworkRANDOM,
-                     "generic": GenericNAS201Model}
-
-nasnet_super_nets = {"GDAS": NASNetworkGDAS,
-                     "GDAS_FRC": NASNetworkGDAS_FRC,
-                     "DARTS": NASNetworkDARTS}
+##################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
+##################################################
+# The macro structure is defined in NAS-Bench-201
+from .search_model_darts import TinyNetworkDarts
+from .search_model_gdas import TinyNetworkGDAS
+from .search_model_setn import TinyNetworkSETN
+from .search_model_enas import TinyNetworkENAS
+from .search_model_random import TinyNetworkRANDOM
+from .generic_model import GenericNAS201Model
+from .genotypes import Structure as CellStructure, architectures as CellArchitectures
+# NASNet-based macro structure
+from .search_model_gdas_nasnet import NASNetworkGDAS
+from .search_model_gdas_frc_nasnet import NASNetworkGDAS_FRC
+from .search_model_darts_nasnet import NASNetworkDARTS
+
+nas201_super_nets = {'DARTS-V1': TinyNetworkDarts,
+                     "DARTS-V2": TinyNetworkDarts,
+                     "GDAS": TinyNetworkGDAS,
+                     "SETN": TinyNetworkSETN,
+                     "ENAS": TinyNetworkENAS,
+                     "RANDOM": TinyNetworkRANDOM,
+                     "generic": GenericNAS201Model}
+
+nasnet_super_nets = {"GDAS": NASNetworkGDAS,
+                     "GDAS_FRC": NASNetworkGDAS_FRC,
+                     "DARTS": NASNetworkDARTS}
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/generic_model.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/generic_model.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,312 +1,312 @@
-#####################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2020.07 #
-#####################################################
-import torch, random
-import torch.nn as nn
-from copy import deepcopy
-from typing import Text
-from torch.distributions.categorical import Categorical
-
-from ..cell_operations import ResNetBasicblock, drop_path
-from .search_cells import NAS201SearchCell as SearchCell
-from .genotypes import Structure
-
-
-class Controller(nn.Module):
-    # we refer to https://github.com/TDeVries/enas_pytorch/blob/master/models/controller.py
-    def __init__(self, edge2index, op_names, max_nodes, lstm_size=32, lstm_num_layers=2, tanh_constant=2.5,
-                 temperature=5.0):
-        super(Controller, self).__init__()
-        # assign the attributes
-        self.max_nodes = max_nodes
-        self.num_edge = len(edge2index)
-        self.edge2index = edge2index
-        self.num_ops = len(op_names)
-        self.op_names = op_names
-        self.lstm_size = lstm_size
-        self.lstm_N = lstm_num_layers
-        self.tanh_constant = tanh_constant
-        self.temperature = temperature
-        # create parameters
-        self.register_parameter('input_vars', nn.Parameter(torch.Tensor(1, 1, lstm_size)))
-        self.w_lstm = nn.LSTM(input_size=self.lstm_size, hidden_size=self.lstm_size, num_layers=self.lstm_N)
-        self.w_embd = nn.Embedding(self.num_ops, self.lstm_size)
-        self.w_pred = nn.Linear(self.lstm_size, self.num_ops)
-
-        nn.init.uniform_(self.input_vars, -0.1, 0.1)
-        nn.init.uniform_(self.w_lstm.weight_hh_l0, -0.1, 0.1)
-        nn.init.uniform_(self.w_lstm.weight_ih_l0, -0.1, 0.1)
-        nn.init.uniform_(self.w_embd.weight, -0.1, 0.1)
-        nn.init.uniform_(self.w_pred.weight, -0.1, 0.1)
-
-    def convert_structure(self, _arch):
-        genotypes = []
-        for i in range(1, self.max_nodes):
-            xlist = []
-            for j in range(i):
-                node_str = '{:}<-{:}'.format(i, j)
-                op_index = _arch[self.edge2index[node_str]]
-                op_name = self.op_names[op_index]
-                xlist.append((op_name, j))
-            genotypes.append(tuple(xlist))
-        return Structure(genotypes)
-
-    def forward(self):
-
-        inputs, h0 = self.input_vars, None
-        log_probs, entropys, sampled_arch = [], [], []
-        for iedge in range(self.num_edge):
-            outputs, h0 = self.w_lstm(inputs, h0)
-
-            logits = self.w_pred(outputs)
-            logits = logits / self.temperature
-            logits = self.tanh_constant * torch.tanh(logits)
-            # distribution
-            op_distribution = Categorical(logits=logits)
-            op_index = op_distribution.sample()
-            sampled_arch.append(op_index.item())
-
-            op_log_prob = op_distribution.log_prob(op_index)
-            log_probs.append(op_log_prob.view(-1))
-            op_entropy = op_distribution.entropy()
-            entropys.append(op_entropy.view(-1))
-
-            # obtain the input embedding for the next step
-            inputs = self.w_embd(op_index)
-        return torch.sum(torch.cat(log_probs)), torch.sum(torch.cat(entropys)), self.convert_structure(sampled_arch)
-
-
-class GenericNAS201Model(nn.Module):
-
-    def __init__(self, C, N, max_nodes, num_classes, search_space, affine, track_running_stats):
-        super(GenericNAS201Model, self).__init__()
-        self._C = C
-        self._layerN = N
-        self._max_nodes = max_nodes
-        self._stem = nn.Sequential(
-            nn.Conv2d(3, C, kernel_size=3, padding=1, bias=False),
-            nn.BatchNorm2d(C))
-        layer_channels = [C] * N + [C * 2] + [C * 2] * N + [C * 4] + [C * 4] * N
-        layer_reductions = [False] * N + [True] + [False] * N + [True] + [False] * N
-        C_prev, num_edge, edge2index = C, None, None
-        self._cells = nn.ModuleList()
-        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
-            if reduction:
-                cell = ResNetBasicblock(C_prev, C_curr, 2)
-            else:
-                cell = SearchCell(C_prev, C_curr, 1, max_nodes, search_space, affine, track_running_stats)
-                if num_edge is None:
-                    num_edge, edge2index = cell.num_edges, cell.edge2index
-                else:
-                    assert num_edge == cell.num_edges and edge2index == cell.edge2index, 'invalid {:} vs. {:}.'.format(
-                        num_edge, cell.num_edges)
-            self._cells.append(cell)
-            C_prev = cell.out_dim
-        self._op_names = deepcopy(search_space)
-        self._Layer = len(self._cells)
-        self.edge2index = edge2index
-        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev, affine=affine, track_running_stats=track_running_stats),
-                                     nn.ReLU(inplace=True))
-        self.global_pooling = nn.AdaptiveAvgPool2d(1)
-        self.classifier = nn.Linear(C_prev, num_classes)
-        self._num_edge = num_edge
-        # algorithm related
-        self.arch_parameters = nn.Parameter(1e-3 * torch.randn(num_edge, len(search_space)))
-        self._mode = None
-        self.dynamic_cell = None
-        self._tau = None
-        self._algo = None
-        self._drop_path = None
-        self.verbose = False
-
-    def set_algo(self, algo: Text):
-        # used for searching
-        assert self._algo is None, 'This functioin can only be called once.'
-        self._algo = algo
-        if algo == 'enas':
-            self.controller = Controller(self.edge2index, self._op_names, self._max_nodes)
-        else:
-            self.arch_parameters = nn.Parameter(1e-3 * torch.randn(self._num_edge, len(self._op_names)))
-            if algo == 'gdas':
-                self._tau = 10
-
-    def set_cal_mode(self, mode, dynamic_cell=None):
-        assert mode in ['gdas', 'enas', 'urs', 'joint', 'select', 'dynamic']
-        self._mode = mode
-        if mode == 'dynamic':
-            self.dynamic_cell = deepcopy(dynamic_cell)
-        else:
-            self.dynamic_cell = None
-
-    def set_drop_path(self, progress, drop_path_rate):
-        if drop_path_rate is None:
-            self._drop_path = None
-        elif progress is None:
-            self._drop_path = drop_path_rate
-        else:
-            self._drop_path = progress * drop_path_rate
-
-    @property
-    def mode(self):
-        return self._mode
-
-    @property
-    def drop_path(self):
-        return self._drop_path
-
-    @property
-    def weights(self):
-        xlist = list(self._stem.parameters())
-        xlist += list(self._cells.parameters())
-        xlist += list(self.lastact.parameters())
-        xlist += list(self.global_pooling.parameters())
-        xlist += list(self.classifier.parameters())
-        return xlist
-
-    def set_tau(self, tau):
-        self._tau = tau
-
-    @property
-    def tau(self):
-        return self._tau
-
-    @property
-    def alphas(self):
-        if self._algo == 'enas':
-            return list(self.controller.parameters())
-        else:
-            return [self.arch_parameters]
-
-    @property
-    def message(self):
-        string = self.extra_repr()
-        for i, cell in enumerate(self._cells):
-            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self._cells), cell.extra_repr())
-        return string
-
-    def show_alphas(self):
-        with torch.no_grad():
-            if self._algo == 'enas':
-                return 'w_pred :\n{:}'.format(self.controller.w_pred.weight)
-            else:
-                return 'arch-parameters :\n{:}'.format(nn.functional.softmax(self.arch_parameters, dim=-1).cpu())
-
-    def extra_repr(self):
-        return ('{name}(C={_C}, Max-Nodes={_max_nodes}, N={_layerN}, L={_Layer}, alg={_algo})'.format(
-            name=self.__class__.__name__, **self.__dict__))
-
-    @property
-    def genotype(self):
-        genotypes = []
-        for i in range(1, self._max_nodes):
-            xlist = []
-            for j in range(i):
-                node_str = '{:}<-{:}'.format(i, j)
-                with torch.no_grad():
-                    weights = self.arch_parameters[self.edge2index[node_str]]
-                    op_name = self._op_names[weights.argmax().item()]
-                xlist.append((op_name, j))
-            genotypes.append(tuple(xlist))
-        return Structure(genotypes)
-
-    def dync_genotype(self, use_random=False):
-        genotypes = []
-        with torch.no_grad():
-            alphas_cpu = nn.functional.softmax(self.arch_parameters, dim=-1)
-        for i in range(1, self._max_nodes):
-            xlist = []
-            for j in range(i):
-                node_str = '{:}<-{:}'.format(i, j)
-                if use_random:
-                    op_name = random.choice(self._op_names)
-                else:
-                    weights = alphas_cpu[self.edge2index[node_str]]
-                    op_index = torch.multinomial(weights, 1).item()
-                    op_name = self._op_names[op_index]
-                xlist.append((op_name, j))
-            genotypes.append(tuple(xlist))
-        return Structure(genotypes)
-
-    def get_log_prob(self, arch):
-        with torch.no_grad():
-            logits = nn.functional.log_softmax(self.arch_parameters, dim=-1)
-        select_logits = []
-        for i, node_info in enumerate(arch.nodes):
-            for op, xin in node_info:
-                node_str = '{:}<-{:}'.format(i + 1, xin)
-                op_index = self._op_names.index(op)
-                select_logits.append(logits[self.edge2index[node_str], op_index])
-        return sum(select_logits).item()
-
-    def return_topK(self, K, use_random=False):
-        archs = Structure.gen_all(self._op_names, self._max_nodes, False)
-        pairs = [(self.get_log_prob(arch), arch) for arch in archs]
-        if K < 0 or K >= len(archs): K = len(archs)
-        if use_random:
-            return random.sample(archs, K)
-        else:
-            sorted_pairs = sorted(pairs, key=lambda x: -x[0])
-            return_pairs = [sorted_pairs[_][1] for _ in range(K)]
-            return return_pairs
-
-    def normalize_archp(self):
-        if self.mode == 'gdas':
-            while True:
-                gumbels = -torch.empty_like(self.arch_parameters).exponential_().log()
-                logits = (self.arch_parameters.log_softmax(dim=1) + gumbels) / self.tau
-                probs = nn.functional.softmax(logits, dim=1)
-                index = probs.max(-1, keepdim=True)[1]
-                one_h = torch.zeros_like(logits).scatter_(-1, index, 1.0)
-                hardwts = one_h - probs.detach() + probs
-                if (torch.isinf(gumbels).any()) or (torch.isinf(probs).any()) or (torch.isnan(probs).any()):
-                    continue
-                else:
-                    break
-            with torch.no_grad():
-                hardwts_cpu = hardwts.detach().cpu()
-            return hardwts, hardwts_cpu, index, 'GUMBEL'
-        else:
-            alphas = nn.functional.softmax(self.arch_parameters, dim=-1)
-            index = alphas.max(-1, keepdim=True)[1]
-            with torch.no_grad():
-                alphas_cpu = alphas.detach().cpu()
-            return alphas, alphas_cpu, index, 'SOFTMAX'
-
-    def forward(self, inputs):
-        alphas, alphas_cpu, index, verbose_str = self.normalize_archp()
-        feature = self._stem(inputs)
-        for i, cell in enumerate(self._cells):
-            if isinstance(cell, SearchCell):
-                if self.mode == 'urs':
-                    feature = cell.forward_urs(feature)
-                    if self.verbose:
-                        verbose_str += '-forward_urs'
-                elif self.mode == 'select':
-                    feature = cell.forward_select(feature, alphas_cpu)
-                    if self.verbose:
-                        verbose_str += '-forward_select'
-                elif self.mode == 'joint':
-                    feature = cell.forward_joint(feature, alphas)
-                    if self.verbose:
-                        verbose_str += '-forward_joint'
-                elif self.mode == 'dynamic':
-                    feature = cell.forward_dynamic(feature, self.dynamic_cell)
-                    if self.verbose:
-                        verbose_str += '-forward_dynamic'
-                elif self.mode == 'gdas':
-                    feature = cell.forward_gdas(feature, alphas, index)
-                    if self.verbose:
-                        verbose_str += '-forward_gdas'
-                else:
-                    raise ValueError('invalid mode={:}'.format(self.mode))
-            else:
-                feature = cell(feature)
-            if self.drop_path is not None:
-                feature = drop_path(feature, self.drop_path)
-        if self.verbose and random.random() < 0.001:
-            print(verbose_str)
-        out = self.lastact(feature)
-        out = self.global_pooling(out)
-        out = out.view(out.size(0), -1)
-        logits = self.classifier(out)
-        return out, logits
+#####################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2020.07 #
+#####################################################
+import torch, random
+import torch.nn as nn
+from copy import deepcopy
+from typing import Text
+from torch.distributions.categorical import Categorical
+
+from ..cell_operations import ResNetBasicblock, drop_path
+from .search_cells import NAS201SearchCell as SearchCell
+from .genotypes import Structure
+
+
+class Controller(nn.Module):
+    # we refer to https://github.com/TDeVries/enas_pytorch/blob/master/models/controller.py
+    def __init__(self, edge2index, op_names, max_nodes, lstm_size=32, lstm_num_layers=2, tanh_constant=2.5,
+                 temperature=5.0):
+        super(Controller, self).__init__()
+        # assign the attributes
+        self.max_nodes = max_nodes
+        self.num_edge = len(edge2index)
+        self.edge2index = edge2index
+        self.num_ops = len(op_names)
+        self.op_names = op_names
+        self.lstm_size = lstm_size
+        self.lstm_N = lstm_num_layers
+        self.tanh_constant = tanh_constant
+        self.temperature = temperature
+        # create parameters
+        self.register_parameter('input_vars', nn.Parameter(torch.Tensor(1, 1, lstm_size)))
+        self.w_lstm = nn.LSTM(input_size=self.lstm_size, hidden_size=self.lstm_size, num_layers=self.lstm_N)
+        self.w_embd = nn.Embedding(self.num_ops, self.lstm_size)
+        self.w_pred = nn.Linear(self.lstm_size, self.num_ops)
+
+        nn.init.uniform_(self.input_vars, -0.1, 0.1)
+        nn.init.uniform_(self.w_lstm.weight_hh_l0, -0.1, 0.1)
+        nn.init.uniform_(self.w_lstm.weight_ih_l0, -0.1, 0.1)
+        nn.init.uniform_(self.w_embd.weight, -0.1, 0.1)
+        nn.init.uniform_(self.w_pred.weight, -0.1, 0.1)
+
+    def convert_structure(self, _arch):
+        genotypes = []
+        for i in range(1, self.max_nodes):
+            xlist = []
+            for j in range(i):
+                node_str = '{:}<-{:}'.format(i, j)
+                op_index = _arch[self.edge2index[node_str]]
+                op_name = self.op_names[op_index]
+                xlist.append((op_name, j))
+            genotypes.append(tuple(xlist))
+        return Structure(genotypes)
+
+    def forward(self):
+
+        inputs, h0 = self.input_vars, None
+        log_probs, entropys, sampled_arch = [], [], []
+        for iedge in range(self.num_edge):
+            outputs, h0 = self.w_lstm(inputs, h0)
+
+            logits = self.w_pred(outputs)
+            logits = logits / self.temperature
+            logits = self.tanh_constant * torch.tanh(logits)
+            # distribution
+            op_distribution = Categorical(logits=logits)
+            op_index = op_distribution.sample()
+            sampled_arch.append(op_index.item())
+
+            op_log_prob = op_distribution.log_prob(op_index)
+            log_probs.append(op_log_prob.view(-1))
+            op_entropy = op_distribution.entropy()
+            entropys.append(op_entropy.view(-1))
+
+            # obtain the input embedding for the next step
+            inputs = self.w_embd(op_index)
+        return torch.sum(torch.cat(log_probs)), torch.sum(torch.cat(entropys)), self.convert_structure(sampled_arch)
+
+
+class GenericNAS201Model(nn.Module):
+
+    def __init__(self, C, N, max_nodes, num_classes, search_space, affine, track_running_stats):
+        super(GenericNAS201Model, self).__init__()
+        self._C = C
+        self._layerN = N
+        self._max_nodes = max_nodes
+        self._stem = nn.Sequential(
+            nn.Conv2d(3, C, kernel_size=3, padding=1, bias=False),
+            nn.BatchNorm2d(C))
+        layer_channels = [C] * N + [C * 2] + [C * 2] * N + [C * 4] + [C * 4] * N
+        layer_reductions = [False] * N + [True] + [False] * N + [True] + [False] * N
+        C_prev, num_edge, edge2index = C, None, None
+        self._cells = nn.ModuleList()
+        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
+            if reduction:
+                cell = ResNetBasicblock(C_prev, C_curr, 2)
+            else:
+                cell = SearchCell(C_prev, C_curr, 1, max_nodes, search_space, affine, track_running_stats)
+                if num_edge is None:
+                    num_edge, edge2index = cell.num_edges, cell.edge2index
+                else:
+                    assert num_edge == cell.num_edges and edge2index == cell.edge2index, 'invalid {:} vs. {:}.'.format(
+                        num_edge, cell.num_edges)
+            self._cells.append(cell)
+            C_prev = cell.out_dim
+        self._op_names = deepcopy(search_space)
+        self._Layer = len(self._cells)
+        self.edge2index = edge2index
+        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev, affine=affine, track_running_stats=track_running_stats),
+                                     nn.ReLU(inplace=True))
+        self.global_pooling = nn.AdaptiveAvgPool2d(1)
+        self.classifier = nn.Linear(C_prev, num_classes)
+        self._num_edge = num_edge
+        # algorithm related
+        self.arch_parameters = nn.Parameter(1e-3 * torch.randn(num_edge, len(search_space)))
+        self._mode = None
+        self.dynamic_cell = None
+        self._tau = None
+        self._algo = None
+        self._drop_path = None
+        self.verbose = False
+
+    def set_algo(self, algo: Text):
+        # used for searching
+        assert self._algo is None, 'This functioin can only be called once.'
+        self._algo = algo
+        if algo == 'enas':
+            self.controller = Controller(self.edge2index, self._op_names, self._max_nodes)
+        else:
+            self.arch_parameters = nn.Parameter(1e-3 * torch.randn(self._num_edge, len(self._op_names)))
+            if algo == 'gdas':
+                self._tau = 10
+
+    def set_cal_mode(self, mode, dynamic_cell=None):
+        assert mode in ['gdas', 'enas', 'urs', 'joint', 'select', 'dynamic']
+        self._mode = mode
+        if mode == 'dynamic':
+            self.dynamic_cell = deepcopy(dynamic_cell)
+        else:
+            self.dynamic_cell = None
+
+    def set_drop_path(self, progress, drop_path_rate):
+        if drop_path_rate is None:
+            self._drop_path = None
+        elif progress is None:
+            self._drop_path = drop_path_rate
+        else:
+            self._drop_path = progress * drop_path_rate
+
+    @property
+    def mode(self):
+        return self._mode
+
+    @property
+    def drop_path(self):
+        return self._drop_path
+
+    @property
+    def weights(self):
+        xlist = list(self._stem.parameters())
+        xlist += list(self._cells.parameters())
+        xlist += list(self.lastact.parameters())
+        xlist += list(self.global_pooling.parameters())
+        xlist += list(self.classifier.parameters())
+        return xlist
+
+    def set_tau(self, tau):
+        self._tau = tau
+
+    @property
+    def tau(self):
+        return self._tau
+
+    @property
+    def alphas(self):
+        if self._algo == 'enas':
+            return list(self.controller.parameters())
+        else:
+            return [self.arch_parameters]
+
+    @property
+    def message(self):
+        string = self.extra_repr()
+        for i, cell in enumerate(self._cells):
+            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self._cells), cell.extra_repr())
+        return string
+
+    def show_alphas(self):
+        with torch.no_grad():
+            if self._algo == 'enas':
+                return 'w_pred :\n{:}'.format(self.controller.w_pred.weight)
+            else:
+                return 'arch-parameters :\n{:}'.format(nn.functional.softmax(self.arch_parameters, dim=-1).cpu())
+
+    def extra_repr(self):
+        return ('{name}(C={_C}, Max-Nodes={_max_nodes}, N={_layerN}, L={_Layer}, alg={_algo})'.format(
+            name=self.__class__.__name__, **self.__dict__))
+
+    @property
+    def genotype(self):
+        genotypes = []
+        for i in range(1, self._max_nodes):
+            xlist = []
+            for j in range(i):
+                node_str = '{:}<-{:}'.format(i, j)
+                with torch.no_grad():
+                    weights = self.arch_parameters[self.edge2index[node_str]]
+                    op_name = self._op_names[weights.argmax().item()]
+                xlist.append((op_name, j))
+            genotypes.append(tuple(xlist))
+        return Structure(genotypes)
+
+    def dync_genotype(self, use_random=False):
+        genotypes = []
+        with torch.no_grad():
+            alphas_cpu = nn.functional.softmax(self.arch_parameters, dim=-1)
+        for i in range(1, self._max_nodes):
+            xlist = []
+            for j in range(i):
+                node_str = '{:}<-{:}'.format(i, j)
+                if use_random:
+                    op_name = random.choice(self._op_names)
+                else:
+                    weights = alphas_cpu[self.edge2index[node_str]]
+                    op_index = torch.multinomial(weights, 1).item()
+                    op_name = self._op_names[op_index]
+                xlist.append((op_name, j))
+            genotypes.append(tuple(xlist))
+        return Structure(genotypes)
+
+    def get_log_prob(self, arch):
+        with torch.no_grad():
+            logits = nn.functional.log_softmax(self.arch_parameters, dim=-1)
+        select_logits = []
+        for i, node_info in enumerate(arch.nodes):
+            for op, xin in node_info:
+                node_str = '{:}<-{:}'.format(i + 1, xin)
+                op_index = self._op_names.index(op)
+                select_logits.append(logits[self.edge2index[node_str], op_index])
+        return sum(select_logits).item()
+
+    def return_topK(self, K, use_random=False):
+        archs = Structure.gen_all(self._op_names, self._max_nodes, False)
+        pairs = [(self.get_log_prob(arch), arch) for arch in archs]
+        if K < 0 or K >= len(archs): K = len(archs)
+        if use_random:
+            return random.sample(archs, K)
+        else:
+            sorted_pairs = sorted(pairs, key=lambda x: -x[0])
+            return_pairs = [sorted_pairs[_][1] for _ in range(K)]
+            return return_pairs
+
+    def normalize_archp(self):
+        if self.mode == 'gdas':
+            while True:
+                gumbels = -torch.empty_like(self.arch_parameters).exponential_().log()
+                logits = (self.arch_parameters.log_softmax(dim=1) + gumbels) / self.tau
+                probs = nn.functional.softmax(logits, dim=1)
+                index = probs.max(-1, keepdim=True)[1]
+                one_h = torch.zeros_like(logits).scatter_(-1, index, 1.0)
+                hardwts = one_h - probs.detach() + probs
+                if (torch.isinf(gumbels).any()) or (torch.isinf(probs).any()) or (torch.isnan(probs).any()):
+                    continue
+                else:
+                    break
+            with torch.no_grad():
+                hardwts_cpu = hardwts.detach().cpu()
+            return hardwts, hardwts_cpu, index, 'GUMBEL'
+        else:
+            alphas = nn.functional.softmax(self.arch_parameters, dim=-1)
+            index = alphas.max(-1, keepdim=True)[1]
+            with torch.no_grad():
+                alphas_cpu = alphas.detach().cpu()
+            return alphas, alphas_cpu, index, 'SOFTMAX'
+
+    def forward(self, inputs):
+        alphas, alphas_cpu, index, verbose_str = self.normalize_archp()
+        feature = self._stem(inputs)
+        for i, cell in enumerate(self._cells):
+            if isinstance(cell, SearchCell):
+                if self.mode == 'urs':
+                    feature = cell.forward_urs(feature)
+                    if self.verbose:
+                        verbose_str += '-forward_urs'
+                elif self.mode == 'select':
+                    feature = cell.forward_select(feature, alphas_cpu)
+                    if self.verbose:
+                        verbose_str += '-forward_select'
+                elif self.mode == 'joint':
+                    feature = cell.forward_joint(feature, alphas)
+                    if self.verbose:
+                        verbose_str += '-forward_joint'
+                elif self.mode == 'dynamic':
+                    feature = cell.forward_dynamic(feature, self.dynamic_cell)
+                    if self.verbose:
+                        verbose_str += '-forward_dynamic'
+                elif self.mode == 'gdas':
+                    feature = cell.forward_gdas(feature, alphas, index)
+                    if self.verbose:
+                        verbose_str += '-forward_gdas'
+                else:
+                    raise ValueError('invalid mode={:}'.format(self.mode))
+            else:
+                feature = cell(feature)
+            if self.drop_path is not None:
+                feature = drop_path(feature, self.drop_path)
+        if self.verbose and random.random() < 0.001:
+            print(verbose_str)
+        out = self.lastact(feature)
+        out = self.global_pooling(out)
+        out = out.view(out.size(0), -1)
+        logits = self.classifier(out)
+        return out, logits
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/genotypes.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/genotypes.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,214 +1,214 @@
-##################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
-##################################################
-from copy import deepcopy
-
-
-def get_combination(space, num):
-    combs = []
-    for i in range(num):
-        if i == 0:
-            for func in space:
-                combs.append([(func, i)])
-        else:
-            new_combs = []
-            for string in combs:
-                for func in space:
-                    xstring = string + [(func, i)]
-                    new_combs.append(xstring)
-            combs = new_combs
-    return combs
-
-
-class Structure:
-
-    def __init__(self, genotype):
-        assert isinstance(genotype, list) or isinstance(genotype, tuple), 'invalid class of genotype : {:}'.format(
-            type(genotype))
-        self.node_num = len(genotype) + 1
-        self.nodes = []
-        self.node_N = []
-        for idx, node_info in enumerate(genotype):
-            assert isinstance(node_info, list) or isinstance(node_info,
-                                                             tuple), 'invalid class of node_info : {:}'.format(
-                type(node_info))
-            assert len(node_info) >= 1, 'invalid length : {:}'.format(len(node_info))
-            for node_in in node_info:
-                assert isinstance(node_in, list) or isinstance(node_in, tuple), 'invalid class of in-node : {:}'.format(
-                    type(node_in))
-                assert len(node_in) == 2 and node_in[1] <= idx, 'invalid in-node : {:}'.format(node_in)
-            self.node_N.append(len(node_info))
-            self.nodes.append(tuple(deepcopy(node_info)))
-
-    def tolist(self, remove_str):
-        # convert this class to the list, if remove_str is 'none', then remove the 'none' operation.
-        # note that we re-order the input node in this function
-        # return the-genotype-list and success [if unsuccess, it is not a connectivity]
-        genotypes = []
-        for node_info in self.nodes:
-            node_info = list(node_info)
-            node_info = sorted(node_info, key=lambda x: (x[1], x[0]))
-            node_info = tuple(filter(lambda x: x[0] != remove_str, node_info))
-            if len(node_info) == 0: return None, False
-            genotypes.append(node_info)
-        return genotypes, True
-
-    def node(self, index):
-        assert index > 0 and index <= len(self), 'invalid index={:} < {:}'.format(index, len(self))
-        return self.nodes[index]
-
-    def tostr(self):
-        strings = []
-        for node_info in self.nodes:
-            string = '|'.join([x[0] + '~{:}'.format(x[1]) for x in node_info])
-            string = '|{:}|'.format(string)
-            strings.append(string)
-        return '+'.join(strings)
-
-    def check_valid(self):
-        nodes = {0: True}
-        for i, node_info in enumerate(self.nodes):
-            sums = []
-            for op, xin in node_info:
-                if op == 'none' or nodes[xin] is False:
-                    x = False
-                else:
-                    x = True
-                sums.append(x)
-            nodes[i + 1] = sum(sums) > 0
-        return nodes[len(self.nodes)]
-
-    def to_unique_str(self, consider_zero=False):
-        # this is used to identify the isomorphic cell, which rerquires the prior knowledge of operation
-        # two operations are special, i.e., none and skip_connect
-        nodes = {0: '0'}
-        for i_node, node_info in enumerate(self.nodes):
-            cur_node = []
-            for op, xin in node_info:
-                if consider_zero is None:
-                    x = '(' + nodes[xin] + ')' + '@{:}'.format(op)
-                elif consider_zero:
-                    if op == 'none' or nodes[xin] == '#':
-                        x = '#'  # zero
-                    elif op == 'skip_connect':
-                        x = nodes[xin]
-                    else:
-                        x = '(' + nodes[xin] + ')' + '@{:}'.format(op)
-                else:
-                    if op == 'skip_connect':
-                        x = nodes[xin]
-                    else:
-                        x = '(' + nodes[xin] + ')' + '@{:}'.format(op)
-                cur_node.append(x)
-            nodes[i_node + 1] = '+'.join(sorted(cur_node))
-        return nodes[len(self.nodes)]
-
-    def check_valid_op(self, op_names):
-        for node_info in self.nodes:
-            for inode_edge in node_info:
-                # assert inode_edge[0] in op_names, 'invalid op-name : {:}'.format(inode_edge[0])
-                if inode_edge[0] not in op_names: return False
-        return True
-
-    def __repr__(self):
-        return ('{name}({node_num} nodes with {node_info})'.format(name=self.__class__.__name__, node_info=self.tostr(),
-                                                                   **self.__dict__))
-
-    def __len__(self):
-        return len(self.nodes) + 1
-
-    def __getitem__(self, index):
-        return self.nodes[index]
-
-    @staticmethod
-    def str2structure(xstr):
-        if isinstance(xstr, Structure): return xstr
-        assert isinstance(xstr, str), 'must take string (not {:}) as input'.format(type(xstr))
-        nodestrs = xstr.split('+')
-        genotypes = []
-        for i, node_str in enumerate(nodestrs):
-            inputs = list(filter(lambda x: x != '', node_str.split('|')))
-            for xinput in inputs: assert len(xinput.split('~')) == 2, 'invalid input length : {:}'.format(xinput)
-            inputs = (xi.split('~') for xi in inputs)
-            input_infos = tuple((op, int(IDX)) for (op, IDX) in inputs)
-            genotypes.append(input_infos)
-        return Structure(genotypes)
-
-    @staticmethod
-    def str2fullstructure(xstr, default_name='none'):
-        assert isinstance(xstr, str), 'must take string (not {:}) as input'.format(type(xstr))
-        nodestrs = xstr.split('+')
-        genotypes = []
-        for i, node_str in enumerate(nodestrs):
-            inputs = list(filter(lambda x: x != '', node_str.split('|')))
-            for xinput in inputs: assert len(xinput.split('~')) == 2, 'invalid input length : {:}'.format(xinput)
-            inputs = (xi.split('~') for xi in inputs)
-            input_infos = list((op, int(IDX)) for (op, IDX) in inputs)
-            all_in_nodes = list(x[1] for x in input_infos)
-            for j in range(i):
-                if j not in all_in_nodes: input_infos.append((default_name, j))
-            node_info = sorted(input_infos, key=lambda x: (x[1], x[0]))
-            genotypes.append(tuple(node_info))
-        return Structure(genotypes)
-
-    @staticmethod
-    def gen_all(search_space, num, return_ori):
-        assert isinstance(search_space, list) or isinstance(search_space,
-                                                            tuple), 'invalid class of search-space : {:}'.format(
-            type(search_space))
-        assert num >= 2, 'There should be at least two nodes in a neural cell instead of {:}'.format(num)
-        all_archs = get_combination(search_space, 1)
-        for i, arch in enumerate(all_archs):
-            all_archs[i] = [tuple(arch)]
-
-        for inode in range(2, num):
-            cur_nodes = get_combination(search_space, inode)
-            new_all_archs = []
-            for previous_arch in all_archs:
-                for cur_node in cur_nodes:
-                    new_all_archs.append(previous_arch + [tuple(cur_node)])
-            all_archs = new_all_archs
-        if return_ori:
-            return all_archs
-        else:
-            return [Structure(x) for x in all_archs]
-
-
-ResNet_CODE = Structure(
-    [(('nor_conv_3x3', 0),),  # node-1
-     (('nor_conv_3x3', 1),),  # node-2
-     (('skip_connect', 0), ('skip_connect', 2))]  # node-3
-)
-
-AllConv3x3_CODE = Structure(
-    [(('nor_conv_3x3', 0),),  # node-1
-     (('nor_conv_3x3', 0), ('nor_conv_3x3', 1)),  # node-2
-     (('nor_conv_3x3', 0), ('nor_conv_3x3', 1), ('nor_conv_3x3', 2))]  # node-3
-)
-
-AllFull_CODE = Structure(
-    [(('skip_connect', 0), ('nor_conv_1x1', 0), ('nor_conv_3x3', 0), ('avg_pool_3x3', 0)),  # node-1
-     (('skip_connect', 0), ('nor_conv_1x1', 0), ('nor_conv_3x3', 0), ('avg_pool_3x3', 0), ('skip_connect', 1),
-      ('nor_conv_1x1', 1), ('nor_conv_3x3', 1), ('avg_pool_3x3', 1)),  # node-2
-     (('skip_connect', 0), ('nor_conv_1x1', 0), ('nor_conv_3x3', 0), ('avg_pool_3x3', 0), ('skip_connect', 1),
-      ('nor_conv_1x1', 1), ('nor_conv_3x3', 1), ('avg_pool_3x3', 1), ('skip_connect', 2), ('nor_conv_1x1', 2),
-      ('nor_conv_3x3', 2), ('avg_pool_3x3', 2))]  # node-3
-)
-
-AllConv1x1_CODE = Structure(
-    [(('nor_conv_1x1', 0),),  # node-1
-     (('nor_conv_1x1', 0), ('nor_conv_1x1', 1)),  # node-2
-     (('nor_conv_1x1', 0), ('nor_conv_1x1', 1), ('nor_conv_1x1', 2))]  # node-3
-)
-
-AllIdentity_CODE = Structure(
-    [(('skip_connect', 0),),  # node-1
-     (('skip_connect', 0), ('skip_connect', 1)),  # node-2
-     (('skip_connect', 0), ('skip_connect', 1), ('skip_connect', 2))]  # node-3
-)
-
-architectures = {'resnet': ResNet_CODE,
-                 'all_c3x3': AllConv3x3_CODE,
-                 'all_c1x1': AllConv1x1_CODE,
-                 'all_idnt': AllIdentity_CODE,
-                 'all_full': AllFull_CODE}
+##################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
+##################################################
+from copy import deepcopy
+
+
+def get_combination(space, num):
+    combs = []
+    for i in range(num):
+        if i == 0:
+            for func in space:
+                combs.append([(func, i)])
+        else:
+            new_combs = []
+            for string in combs:
+                for func in space:
+                    xstring = string + [(func, i)]
+                    new_combs.append(xstring)
+            combs = new_combs
+    return combs
+
+
+class Structure:
+
+    def __init__(self, genotype):
+        assert isinstance(genotype, list) or isinstance(genotype, tuple), 'invalid class of genotype : {:}'.format(
+            type(genotype))
+        self.node_num = len(genotype) + 1
+        self.nodes = []
+        self.node_N = []
+        for idx, node_info in enumerate(genotype):
+            assert isinstance(node_info, list) or isinstance(node_info,
+                                                             tuple), 'invalid class of node_info : {:}'.format(
+                type(node_info))
+            assert len(node_info) >= 1, 'invalid length : {:}'.format(len(node_info))
+            for node_in in node_info:
+                assert isinstance(node_in, list) or isinstance(node_in, tuple), 'invalid class of in-node : {:}'.format(
+                    type(node_in))
+                assert len(node_in) == 2 and node_in[1] <= idx, 'invalid in-node : {:}'.format(node_in)
+            self.node_N.append(len(node_info))
+            self.nodes.append(tuple(deepcopy(node_info)))
+
+    def tolist(self, remove_str):
+        # convert this class to the list, if remove_str is 'none', then remove the 'none' operation.
+        # note that we re-order the input node in this function
+        # return the-genotype-list and success [if unsuccess, it is not a connectivity]
+        genotypes = []
+        for node_info in self.nodes:
+            node_info = list(node_info)
+            node_info = sorted(node_info, key=lambda x: (x[1], x[0]))
+            node_info = tuple(filter(lambda x: x[0] != remove_str, node_info))
+            if len(node_info) == 0: return None, False
+            genotypes.append(node_info)
+        return genotypes, True
+
+    def node(self, index):
+        assert index > 0 and index <= len(self), 'invalid index={:} < {:}'.format(index, len(self))
+        return self.nodes[index]
+
+    def tostr(self):
+        strings = []
+        for node_info in self.nodes:
+            string = '|'.join([x[0] + '~{:}'.format(x[1]) for x in node_info])
+            string = '|{:}|'.format(string)
+            strings.append(string)
+        return '+'.join(strings)
+
+    def check_valid(self):
+        nodes = {0: True}
+        for i, node_info in enumerate(self.nodes):
+            sums = []
+            for op, xin in node_info:
+                if op == 'none' or nodes[xin] is False:
+                    x = False
+                else:
+                    x = True
+                sums.append(x)
+            nodes[i + 1] = sum(sums) > 0
+        return nodes[len(self.nodes)]
+
+    def to_unique_str(self, consider_zero=False):
+        # this is used to identify the isomorphic cell, which rerquires the prior knowledge of operation
+        # two operations are special, i.e., none and skip_connect
+        nodes = {0: '0'}
+        for i_node, node_info in enumerate(self.nodes):
+            cur_node = []
+            for op, xin in node_info:
+                if consider_zero is None:
+                    x = '(' + nodes[xin] + ')' + '@{:}'.format(op)
+                elif consider_zero:
+                    if op == 'none' or nodes[xin] == '#':
+                        x = '#'  # zero
+                    elif op == 'skip_connect':
+                        x = nodes[xin]
+                    else:
+                        x = '(' + nodes[xin] + ')' + '@{:}'.format(op)
+                else:
+                    if op == 'skip_connect':
+                        x = nodes[xin]
+                    else:
+                        x = '(' + nodes[xin] + ')' + '@{:}'.format(op)
+                cur_node.append(x)
+            nodes[i_node + 1] = '+'.join(sorted(cur_node))
+        return nodes[len(self.nodes)]
+
+    def check_valid_op(self, op_names):
+        for node_info in self.nodes:
+            for inode_edge in node_info:
+                # assert inode_edge[0] in op_names, 'invalid op-name : {:}'.format(inode_edge[0])
+                if inode_edge[0] not in op_names: return False
+        return True
+
+    def __repr__(self):
+        return ('{name}({node_num} nodes with {node_info})'.format(name=self.__class__.__name__, node_info=self.tostr(),
+                                                                   **self.__dict__))
+
+    def __len__(self):
+        return len(self.nodes) + 1
+
+    def __getitem__(self, index):
+        return self.nodes[index]
+
+    @staticmethod
+    def str2structure(xstr):
+        if isinstance(xstr, Structure): return xstr
+        assert isinstance(xstr, str), 'must take string (not {:}) as input'.format(type(xstr))
+        nodestrs = xstr.split('+')
+        genotypes = []
+        for i, node_str in enumerate(nodestrs):
+            inputs = list(filter(lambda x: x != '', node_str.split('|')))
+            for xinput in inputs: assert len(xinput.split('~')) == 2, 'invalid input length : {:}'.format(xinput)
+            inputs = (xi.split('~') for xi in inputs)
+            input_infos = tuple((op, int(IDX)) for (op, IDX) in inputs)
+            genotypes.append(input_infos)
+        return Structure(genotypes)
+
+    @staticmethod
+    def str2fullstructure(xstr, default_name='none'):
+        assert isinstance(xstr, str), 'must take string (not {:}) as input'.format(type(xstr))
+        nodestrs = xstr.split('+')
+        genotypes = []
+        for i, node_str in enumerate(nodestrs):
+            inputs = list(filter(lambda x: x != '', node_str.split('|')))
+            for xinput in inputs: assert len(xinput.split('~')) == 2, 'invalid input length : {:}'.format(xinput)
+            inputs = (xi.split('~') for xi in inputs)
+            input_infos = list((op, int(IDX)) for (op, IDX) in inputs)
+            all_in_nodes = list(x[1] for x in input_infos)
+            for j in range(i):
+                if j not in all_in_nodes: input_infos.append((default_name, j))
+            node_info = sorted(input_infos, key=lambda x: (x[1], x[0]))
+            genotypes.append(tuple(node_info))
+        return Structure(genotypes)
+
+    @staticmethod
+    def gen_all(search_space, num, return_ori):
+        assert isinstance(search_space, list) or isinstance(search_space,
+                                                            tuple), 'invalid class of search-space : {:}'.format(
+            type(search_space))
+        assert num >= 2, 'There should be at least two nodes in a neural cell instead of {:}'.format(num)
+        all_archs = get_combination(search_space, 1)
+        for i, arch in enumerate(all_archs):
+            all_archs[i] = [tuple(arch)]
+
+        for inode in range(2, num):
+            cur_nodes = get_combination(search_space, inode)
+            new_all_archs = []
+            for previous_arch in all_archs:
+                for cur_node in cur_nodes:
+                    new_all_archs.append(previous_arch + [tuple(cur_node)])
+            all_archs = new_all_archs
+        if return_ori:
+            return all_archs
+        else:
+            return [Structure(x) for x in all_archs]
+
+
+ResNet_CODE = Structure(
+    [(('nor_conv_3x3', 0),),  # node-1
+     (('nor_conv_3x3', 1),),  # node-2
+     (('skip_connect', 0), ('skip_connect', 2))]  # node-3
+)
+
+AllConv3x3_CODE = Structure(
+    [(('nor_conv_3x3', 0),),  # node-1
+     (('nor_conv_3x3', 0), ('nor_conv_3x3', 1)),  # node-2
+     (('nor_conv_3x3', 0), ('nor_conv_3x3', 1), ('nor_conv_3x3', 2))]  # node-3
+)
+
+AllFull_CODE = Structure(
+    [(('skip_connect', 0), ('nor_conv_1x1', 0), ('nor_conv_3x3', 0), ('avg_pool_3x3', 0)),  # node-1
+     (('skip_connect', 0), ('nor_conv_1x1', 0), ('nor_conv_3x3', 0), ('avg_pool_3x3', 0), ('skip_connect', 1),
+      ('nor_conv_1x1', 1), ('nor_conv_3x3', 1), ('avg_pool_3x3', 1)),  # node-2
+     (('skip_connect', 0), ('nor_conv_1x1', 0), ('nor_conv_3x3', 0), ('avg_pool_3x3', 0), ('skip_connect', 1),
+      ('nor_conv_1x1', 1), ('nor_conv_3x3', 1), ('avg_pool_3x3', 1), ('skip_connect', 2), ('nor_conv_1x1', 2),
+      ('nor_conv_3x3', 2), ('avg_pool_3x3', 2))]  # node-3
+)
+
+AllConv1x1_CODE = Structure(
+    [(('nor_conv_1x1', 0),),  # node-1
+     (('nor_conv_1x1', 0), ('nor_conv_1x1', 1)),  # node-2
+     (('nor_conv_1x1', 0), ('nor_conv_1x1', 1), ('nor_conv_1x1', 2))]  # node-3
+)
+
+AllIdentity_CODE = Structure(
+    [(('skip_connect', 0),),  # node-1
+     (('skip_connect', 0), ('skip_connect', 1)),  # node-2
+     (('skip_connect', 0), ('skip_connect', 1), ('skip_connect', 2))]  # node-3
+)
+
+architectures = {'resnet': ResNet_CODE,
+                 'all_c3x3': AllConv3x3_CODE,
+                 'all_c1x1': AllConv1x1_CODE,
+                 'all_idnt': AllIdentity_CODE,
+                 'all_full': AllFull_CODE}
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_darts.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_gdas.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,116 @@
-##################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
-########################################################
-# DARTS: Differentiable Architecture Search, ICLR 2019 #
-########################################################
-import torch
-import torch.nn as nn
-from copy import deepcopy
-from ..cell_operations import ResNetBasicblock
-from .search_cells import NAS201SearchCell as SearchCell
-from .genotypes import Structure
-
-
-class TinyNetworkDarts(nn.Module):
-
-    def __init__(self, C, N, max_nodes, num_classes, search_space, affine, track_running_stats):
-        super(TinyNetworkDarts, self).__init__()
-        self._C = C
-        self._layerN = N
-        self.max_nodes = max_nodes
-        self.stem = nn.Sequential(
-            nn.Conv2d(3, C, kernel_size=3, padding=1, bias=False),
-            nn.BatchNorm2d(C))
-
-        layer_channels = [C] * N + [C * 2] + [C * 2] * N + [C * 4] + [C * 4] * N
-        layer_reductions = [False] * N + [True] + [False] * N + [True] + [False] * N
-
-        C_prev, num_edge, edge2index = C, None, None
-        self.cells = nn.ModuleList()
-        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
-            if reduction:
-                cell = ResNetBasicblock(C_prev, C_curr, 2)
-            else:
-                cell = SearchCell(C_prev, C_curr, 1, max_nodes, search_space, affine, track_running_stats)
-                if num_edge is None:
-                    num_edge, edge2index = cell.num_edges, cell.edge2index
-                else:
-                    assert num_edge == cell.num_edges and edge2index == cell.edge2index, 'invalid {:} vs. {:}.'.format(
-                        num_edge, cell.num_edges)
-            self.cells.append(cell)
-            C_prev = cell.out_dim
-        self.op_names = deepcopy(search_space)
-        self._Layer = len(self.cells)
-        self.edge2index = edge2index
-        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev), nn.ReLU(inplace=True))
-        self.global_pooling = nn.AdaptiveAvgPool2d(1)
-        self.classifier = nn.Linear(C_prev, num_classes)
-        self.arch_parameters = nn.Parameter(1e-3 * torch.randn(num_edge, len(search_space)))
-
-    def get_weights(self):
-        xlist = list(self.stem.parameters()) + list(self.cells.parameters())
-        xlist += list(self.lastact.parameters()) + list(self.global_pooling.parameters())
-        xlist += list(self.classifier.parameters())
-        return xlist
-
-    def get_alphas(self):
-        return [self.arch_parameters]
-
-    def show_alphas(self):
-        with torch.no_grad():
-            return 'arch-parameters :\n{:}'.format(nn.functional.softmax(self.arch_parameters, dim=-1).cpu())
-
-    def get_message(self):
-        string = self.extra_repr()
-        for i, cell in enumerate(self.cells):
-            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
-        return string
-
-    def extra_repr(self):
-        return ('{name}(C={_C}, Max-Nodes={max_nodes}, N={_layerN}, L={_Layer})'.format(name=self.__class__.__name__,
-                                                                                        **self.__dict__))
-
-    def genotype(self):
-        genotypes = []
-        for i in range(1, self.max_nodes):
-            xlist = []
-            for j in range(i):
-                node_str = '{:}<-{:}'.format(i, j)
-                with torch.no_grad():
-                    weights = self.arch_parameters[self.edge2index[node_str]]
-                    op_name = self.op_names[weights.argmax().item()]
-                xlist.append((op_name, j))
-            genotypes.append(tuple(xlist))
-        return Structure(genotypes)
-
-    def forward(self, inputs):
-        alphas = nn.functional.softmax(self.arch_parameters, dim=-1)
-
-        feature = self.stem(inputs)
-        for i, cell in enumerate(self.cells):
-            if isinstance(cell, SearchCell):
-                feature = cell(feature, alphas)
-            else:
-                feature = cell(feature)
-
-        out = self.lastact(feature)
-        out = self.global_pooling(out)
-        out = out.view(out.size(0), -1)
-        logits = self.classifier(out)
-
-        return out, logits
+###########################################################################
+# Searching for A Robust Neural Architecture in Four GPU Hours, CVPR 2019 #
+###########################################################################
+import torch
+import torch.nn as nn
+from copy import deepcopy
+from ..cell_operations import ResNetBasicblock
+from .search_cells import NAS201SearchCell as SearchCell
+from .genotypes import Structure
+
+
+class TinyNetworkGDAS(nn.Module):
+
+    # def __init__(self, C, N, max_nodes, num_classes, search_space, affine=False, track_running_stats=True):
+    def __init__(self, C, N, max_nodes, num_classes, search_space, affine, track_running_stats):
+        super(TinyNetworkGDAS, self).__init__()
+        self._C = C
+        self._layerN = N
+        self.max_nodes = max_nodes
+        self.stem = nn.Sequential(
+            nn.Conv2d(3, C, kernel_size=3, padding=1, bias=False),
+            nn.BatchNorm2d(C))
+
+        layer_channels = [C] * N + [C * 2] + [C * 2] * N + [C * 4] + [C * 4] * N
+        layer_reductions = [False] * N + [True] + [False] * N + [True] + [False] * N
+
+        C_prev, num_edge, edge2index = C, None, None
+        self.cells = nn.ModuleList()
+        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
+            if reduction:
+                cell = ResNetBasicblock(C_prev, C_curr, 2)
+            else:
+                cell = SearchCell(C_prev, C_curr, 1, max_nodes, search_space, affine, track_running_stats)
+                if num_edge is None:
+                    num_edge, edge2index = cell.num_edges, cell.edge2index
+                else:
+                    assert num_edge == cell.num_edges and edge2index == cell.edge2index, 'invalid {:} vs. {:}.'.format(
+                        num_edge, cell.num_edges)
+            self.cells.append(cell)
+            C_prev = cell.out_dim
+        self.op_names = deepcopy(search_space)
+        self._Layer = len(self.cells)
+        self.edge2index = edge2index
+        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev), nn.ReLU(inplace=True))
+        self.global_pooling = nn.AdaptiveAvgPool2d(1)
+        self.classifier = nn.Linear(C_prev, num_classes)
+        self.arch_parameters = nn.Parameter(1e-3 * torch.randn(num_edge, len(search_space)))
+        self.tau = 10
+
+    def get_weights(self):
+        xlist = list(self.stem.parameters()) + list(self.cells.parameters())
+        xlist += list(self.lastact.parameters()) + list(self.global_pooling.parameters())
+        xlist += list(self.classifier.parameters())
+        return xlist
+
+    def set_tau(self, tau):
+        self.tau = tau
+
+    def get_tau(self):
+        return self.tau
+
+    def get_alphas(self):
+        return [self.arch_parameters]
+
+    def show_alphas(self):
+        with torch.no_grad():
+            return 'arch-parameters :\n{:}'.format(nn.functional.softmax(self.arch_parameters, dim=-1).cpu())
+
+    def get_message(self):
+        string = self.extra_repr()
+        for i, cell in enumerate(self.cells):
+            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
+        return string
+
+    def extra_repr(self):
+        return ('{name}(C={_C}, Max-Nodes={max_nodes}, N={_layerN}, L={_Layer})'.format(name=self.__class__.__name__,
+                                                                                        **self.__dict__))
+
+    def genotype(self):
+        genotypes = []
+        for i in range(1, self.max_nodes):
+            xlist = []
+            for j in range(i):
+                node_str = '{:}<-{:}'.format(i, j)
+                with torch.no_grad():
+                    weights = self.arch_parameters[self.edge2index[node_str]]
+                    op_name = self.op_names[weights.argmax().item()]
+                xlist.append((op_name, j))
+            genotypes.append(tuple(xlist))
+        return Structure(genotypes)
+
+    def forward(self, inputs):
+        while True:
+            gumbels = -torch.empty_like(self.arch_parameters).exponential_().log()
+            logits = (self.arch_parameters.log_softmax(dim=1) + gumbels) / self.tau
+            probs = nn.functional.softmax(logits, dim=1)
+            index = probs.max(-1, keepdim=True)[1]
+            one_h = torch.zeros_like(logits).scatter_(-1, index, 1.0)
+            hardwts = one_h - probs.detach() + probs
+            if (torch.isinf(gumbels).any()) or (torch.isinf(probs).any()) or (torch.isnan(probs).any()):
+                continue
+            else:
+                break
+
+        feature = self.stem(inputs)
+        for i, cell in enumerate(self.cells):
+            if isinstance(cell, SearchCell):
+                feature = cell.forward_gdas(feature, hardwts, index)
+            else:
+                feature = cell(feature)
+        out = self.lastact(feature)
+        out = self.global_pooling(out)
+        out = out.view(out.size(0), -1)
+        logits = self.classifier(out)
+
+        return out, logits
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_darts_nasnet.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_darts_nasnet.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-####################
-# DARTS, ICLR 2019 #
-####################
-import torch
-import torch.nn as nn
-from copy import deepcopy
-from typing import List, Text, Dict
-from .search_cells import NASNetSearchCell as SearchCell
-
-
-# The macro structure is based on NASNet
-class NASNetworkDARTS(nn.Module):
-
-    def __init__(self, C: int, N: int, steps: int, multiplier: int, stem_multiplier: int,
-                 num_classes: int, search_space: List[Text], affine: bool, track_running_stats: bool):
-        super(NASNetworkDARTS, self).__init__()
-        self._C = C
-        self._layerN = N
-        self._steps = steps
-        self._multiplier = multiplier
-        self.stem = nn.Sequential(
-            nn.Conv2d(3, C * stem_multiplier, kernel_size=3, padding=1, bias=False),
-            nn.BatchNorm2d(C * stem_multiplier))
-
-        # config for each layer
-        layer_channels = [C] * N + [C * 2] + [C * 2] * (N - 1) + [C * 4] + [C * 4] * (N - 1)
-        layer_reductions = [False] * N + [True] + [False] * (N - 1) + [True] + [False] * (N - 1)
-
-        num_edge, edge2index = None, None
-        C_prev_prev, C_prev, C_curr, reduction_prev = C * stem_multiplier, C * stem_multiplier, C, False
-
-        self.cells = nn.ModuleList()
-        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
-            cell = SearchCell(search_space, steps, multiplier, C_prev_prev, C_prev, C_curr, reduction, reduction_prev,
-                              affine, track_running_stats)
-            if num_edge is None:
-                num_edge, edge2index = cell.num_edges, cell.edge2index
-            else:
-                assert num_edge == cell.num_edges and edge2index == cell.edge2index, 'invalid {:} vs. {:}.'.format(
-                    num_edge, cell.num_edges)
-            self.cells.append(cell)
-            C_prev_prev, C_prev, reduction_prev = C_prev, multiplier * C_curr, reduction
-        self.op_names = deepcopy(search_space)
-        self._Layer = len(self.cells)
-        self.edge2index = edge2index
-        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev), nn.ReLU(inplace=True))
-        self.global_pooling = nn.AdaptiveAvgPool2d(1)
-        self.classifier = nn.Linear(C_prev, num_classes)
-        self.arch_normal_parameters = nn.Parameter(1e-3 * torch.randn(num_edge, len(search_space)))
-        self.arch_reduce_parameters = nn.Parameter(1e-3 * torch.randn(num_edge, len(search_space)))
-
-    def get_weights(self) -> List[torch.nn.Parameter]:
-        xlist = list(self.stem.parameters()) + list(self.cells.parameters())
-        xlist += list(self.lastact.parameters()) + list(self.global_pooling.parameters())
-        xlist += list(self.classifier.parameters())
-        return xlist
-
-    def get_alphas(self) -> List[torch.nn.Parameter]:
-        return [self.arch_normal_parameters, self.arch_reduce_parameters]
-
-    def show_alphas(self) -> Text:
-        with torch.no_grad():
-            A = 'arch-normal-parameters :\n{:}'.format(nn.functional.softmax(self.arch_normal_parameters, dim=-1).cpu())
-            B = 'arch-reduce-parameters :\n{:}'.format(nn.functional.softmax(self.arch_reduce_parameters, dim=-1).cpu())
-        return '{:}\n{:}'.format(A, B)
-
-    def get_message(self) -> Text:
-        string = self.extra_repr()
-        for i, cell in enumerate(self.cells):
-            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
-        return string
-
-    def extra_repr(self) -> Text:
-        return ('{name}(C={_C}, N={_layerN}, steps={_steps}, multiplier={_multiplier}, L={_Layer})'.format(
-            name=self.__class__.__name__, **self.__dict__))
-
-    def genotype(self) -> Dict[Text, List]:
-        def _parse(weights):
-            gene = []
-            for i in range(self._steps):
-                edges = []
-                for j in range(2 + i):
-                    node_str = '{:}<-{:}'.format(i, j)
-                    ws = weights[self.edge2index[node_str]]
-                    for k, op_name in enumerate(self.op_names):
-                        if op_name == 'none': continue
-                        edges.append((op_name, j, ws[k]))
-                edges = sorted(edges, key=lambda x: -x[-1])
-                selected_edges = edges[:2]
-                gene.append(tuple(selected_edges))
-            return gene
-
-        with torch.no_grad():
-            gene_normal = _parse(torch.softmax(self.arch_normal_parameters, dim=-1).cpu().numpy())
-            gene_reduce = _parse(torch.softmax(self.arch_reduce_parameters, dim=-1).cpu().numpy())
-        return {'normal': gene_normal,
-                'normal_concat': list(range(2 + self._steps - self._multiplier, self._steps + 2)),
-                'reduce': gene_reduce,
-                'reduce_concat': list(range(2 + self._steps - self._multiplier, self._steps + 2))}
-
-    def forward(self, inputs):
-
-        normal_w = nn.functional.softmax(self.arch_normal_parameters, dim=1)
-        reduce_w = nn.functional.softmax(self.arch_reduce_parameters, dim=1)
-
-        s0 = s1 = self.stem(inputs)
-        for i, cell in enumerate(self.cells):
-            if cell.reduction:
-                ww = reduce_w
-            else:
-                ww = normal_w
-            s0, s1 = s1, cell.forward_darts(s0, s1, ww)
-        out = self.lastact(s1)
-        out = self.global_pooling(out)
-        out = out.view(out.size(0), -1)
-        logits = self.classifier(out)
-
-        return out, logits
+####################
+# DARTS, ICLR 2019 #
+####################
+import torch
+import torch.nn as nn
+from copy import deepcopy
+from typing import List, Text, Dict
+from .search_cells import NASNetSearchCell as SearchCell
+
+
+# The macro structure is based on NASNet
+class NASNetworkDARTS(nn.Module):
+
+    def __init__(self, C: int, N: int, steps: int, multiplier: int, stem_multiplier: int,
+                 num_classes: int, search_space: List[Text], affine: bool, track_running_stats: bool):
+        super(NASNetworkDARTS, self).__init__()
+        self._C = C
+        self._layerN = N
+        self._steps = steps
+        self._multiplier = multiplier
+        self.stem = nn.Sequential(
+            nn.Conv2d(3, C * stem_multiplier, kernel_size=3, padding=1, bias=False),
+            nn.BatchNorm2d(C * stem_multiplier))
+
+        # config for each layer
+        layer_channels = [C] * N + [C * 2] + [C * 2] * (N - 1) + [C * 4] + [C * 4] * (N - 1)
+        layer_reductions = [False] * N + [True] + [False] * (N - 1) + [True] + [False] * (N - 1)
+
+        num_edge, edge2index = None, None
+        C_prev_prev, C_prev, C_curr, reduction_prev = C * stem_multiplier, C * stem_multiplier, C, False
+
+        self.cells = nn.ModuleList()
+        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
+            cell = SearchCell(search_space, steps, multiplier, C_prev_prev, C_prev, C_curr, reduction, reduction_prev,
+                              affine, track_running_stats)
+            if num_edge is None:
+                num_edge, edge2index = cell.num_edges, cell.edge2index
+            else:
+                assert num_edge == cell.num_edges and edge2index == cell.edge2index, 'invalid {:} vs. {:}.'.format(
+                    num_edge, cell.num_edges)
+            self.cells.append(cell)
+            C_prev_prev, C_prev, reduction_prev = C_prev, multiplier * C_curr, reduction
+        self.op_names = deepcopy(search_space)
+        self._Layer = len(self.cells)
+        self.edge2index = edge2index
+        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev), nn.ReLU(inplace=True))
+        self.global_pooling = nn.AdaptiveAvgPool2d(1)
+        self.classifier = nn.Linear(C_prev, num_classes)
+        self.arch_normal_parameters = nn.Parameter(1e-3 * torch.randn(num_edge, len(search_space)))
+        self.arch_reduce_parameters = nn.Parameter(1e-3 * torch.randn(num_edge, len(search_space)))
+
+    def get_weights(self) -> List[torch.nn.Parameter]:
+        xlist = list(self.stem.parameters()) + list(self.cells.parameters())
+        xlist += list(self.lastact.parameters()) + list(self.global_pooling.parameters())
+        xlist += list(self.classifier.parameters())
+        return xlist
+
+    def get_alphas(self) -> List[torch.nn.Parameter]:
+        return [self.arch_normal_parameters, self.arch_reduce_parameters]
+
+    def show_alphas(self) -> Text:
+        with torch.no_grad():
+            A = 'arch-normal-parameters :\n{:}'.format(nn.functional.softmax(self.arch_normal_parameters, dim=-1).cpu())
+            B = 'arch-reduce-parameters :\n{:}'.format(nn.functional.softmax(self.arch_reduce_parameters, dim=-1).cpu())
+        return '{:}\n{:}'.format(A, B)
+
+    def get_message(self) -> Text:
+        string = self.extra_repr()
+        for i, cell in enumerate(self.cells):
+            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
+        return string
+
+    def extra_repr(self) -> Text:
+        return ('{name}(C={_C}, N={_layerN}, steps={_steps}, multiplier={_multiplier}, L={_Layer})'.format(
+            name=self.__class__.__name__, **self.__dict__))
+
+    def genotype(self) -> Dict[Text, List]:
+        def _parse(weights):
+            gene = []
+            for i in range(self._steps):
+                edges = []
+                for j in range(2 + i):
+                    node_str = '{:}<-{:}'.format(i, j)
+                    ws = weights[self.edge2index[node_str]]
+                    for k, op_name in enumerate(self.op_names):
+                        if op_name == 'none': continue
+                        edges.append((op_name, j, ws[k]))
+                edges = sorted(edges, key=lambda x: -x[-1])
+                selected_edges = edges[:2]
+                gene.append(tuple(selected_edges))
+            return gene
+
+        with torch.no_grad():
+            gene_normal = _parse(torch.softmax(self.arch_normal_parameters, dim=-1).cpu().numpy())
+            gene_reduce = _parse(torch.softmax(self.arch_reduce_parameters, dim=-1).cpu().numpy())
+        return {'normal': gene_normal,
+                'normal_concat': list(range(2 + self._steps - self._multiplier, self._steps + 2)),
+                'reduce': gene_reduce,
+                'reduce_concat': list(range(2 + self._steps - self._multiplier, self._steps + 2))}
+
+    def forward(self, inputs):
+
+        normal_w = nn.functional.softmax(self.arch_normal_parameters, dim=1)
+        reduce_w = nn.functional.softmax(self.arch_reduce_parameters, dim=1)
+
+        s0 = s1 = self.stem(inputs)
+        for i, cell in enumerate(self.cells):
+            if cell.reduction:
+                ww = reduce_w
+            else:
+                ww = normal_w
+            s0, s1 = s1, cell.forward_darts(s0, s1, ww)
+        out = self.lastact(s1)
+        out = self.global_pooling(out)
+        out = out.view(out.size(0), -1)
+        logits = self.classifier(out)
+
+        return out, logits
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_enas.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_enas.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-##################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
-##########################################################################
-# Efficient Neural Architecture Search via Parameters Sharing, ICML 2018 #
-##########################################################################
-import torch
-import torch.nn as nn
-from copy import deepcopy
-from ..cell_operations import ResNetBasicblock
-from .search_cells import NAS201SearchCell as SearchCell
-from .genotypes import Structure
-from .search_model_enas_utils import Controller
-
-
-class TinyNetworkENAS(nn.Module):
-
-    def __init__(self, C, N, max_nodes, num_classes, search_space, affine, track_running_stats):
-        super(TinyNetworkENAS, self).__init__()
-        self._C = C
-        self._layerN = N
-        self.max_nodes = max_nodes
-        self.stem = nn.Sequential(
-            nn.Conv2d(3, C, kernel_size=3, padding=1, bias=False),
-            nn.BatchNorm2d(C))
-
-        layer_channels = [C] * N + [C * 2] + [C * 2] * N + [C * 4] + [C * 4] * N
-        layer_reductions = [False] * N + [True] + [False] * N + [True] + [False] * N
-
-        C_prev, num_edge, edge2index = C, None, None
-        self.cells = nn.ModuleList()
-        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
-            if reduction:
-                cell = ResNetBasicblock(C_prev, C_curr, 2)
-            else:
-                cell = SearchCell(C_prev, C_curr, 1, max_nodes, search_space, affine, track_running_stats)
-                if num_edge is None:
-                    num_edge, edge2index = cell.num_edges, cell.edge2index
-                else:
-                    assert num_edge == cell.num_edges and edge2index == cell.edge2index, 'invalid {:} vs. {:}.'.format(
-                        num_edge, cell.num_edges)
-            self.cells.append(cell)
-            C_prev = cell.out_dim
-        self.op_names = deepcopy(search_space)
-        self._Layer = len(self.cells)
-        self.edge2index = edge2index
-        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev), nn.ReLU(inplace=True))
-        self.global_pooling = nn.AdaptiveAvgPool2d(1)
-        self.classifier = nn.Linear(C_prev, num_classes)
-        # to maintain the sampled architecture
-        self.sampled_arch = None
-
-    def update_arch(self, _arch):
-        if _arch is None:
-            self.sampled_arch = None
-        elif isinstance(_arch, Structure):
-            self.sampled_arch = _arch
-        elif isinstance(_arch, (list, tuple)):
-            genotypes = []
-            for i in range(1, self.max_nodes):
-                xlist = []
-                for j in range(i):
-                    node_str = '{:}<-{:}'.format(i, j)
-                    op_index = _arch[self.edge2index[node_str]]
-                    op_name = self.op_names[op_index]
-                    xlist.append((op_name, j))
-                genotypes.append(tuple(xlist))
-            self.sampled_arch = Structure(genotypes)
-        else:
-            raise ValueError('invalid type of input architecture : {:}'.format(_arch))
-        return self.sampled_arch
-
-    def create_controller(self):
-        return Controller(len(self.edge2index), len(self.op_names))
-
-    def get_message(self):
-        string = self.extra_repr()
-        for i, cell in enumerate(self.cells):
-            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
-        return string
-
-    def extra_repr(self):
-        return ('{name}(C={_C}, Max-Nodes={max_nodes}, N={_layerN}, L={_Layer})'.format(name=self.__class__.__name__,
-                                                                                        **self.__dict__))
-
-    def forward(self, inputs):
-
-        feature = self.stem(inputs)
-        for i, cell in enumerate(self.cells):
-            if isinstance(cell, SearchCell):
-                feature = cell.forward_dynamic(feature, self.sampled_arch)
-            else:
-                feature = cell(feature)
-
-        out = self.lastact(feature)
-        out = self.global_pooling(out)
-        out = out.view(out.size(0), -1)
-        logits = self.classifier(out)
-
-        return out, logits
+##################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
+##########################################################################
+# Efficient Neural Architecture Search via Parameters Sharing, ICML 2018 #
+##########################################################################
+import torch
+import torch.nn as nn
+from copy import deepcopy
+from ..cell_operations import ResNetBasicblock
+from .search_cells import NAS201SearchCell as SearchCell
+from .genotypes import Structure
+from .search_model_enas_utils import Controller
+
+
+class TinyNetworkENAS(nn.Module):
+
+    def __init__(self, C, N, max_nodes, num_classes, search_space, affine, track_running_stats):
+        super(TinyNetworkENAS, self).__init__()
+        self._C = C
+        self._layerN = N
+        self.max_nodes = max_nodes
+        self.stem = nn.Sequential(
+            nn.Conv2d(3, C, kernel_size=3, padding=1, bias=False),
+            nn.BatchNorm2d(C))
+
+        layer_channels = [C] * N + [C * 2] + [C * 2] * N + [C * 4] + [C * 4] * N
+        layer_reductions = [False] * N + [True] + [False] * N + [True] + [False] * N
+
+        C_prev, num_edge, edge2index = C, None, None
+        self.cells = nn.ModuleList()
+        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
+            if reduction:
+                cell = ResNetBasicblock(C_prev, C_curr, 2)
+            else:
+                cell = SearchCell(C_prev, C_curr, 1, max_nodes, search_space, affine, track_running_stats)
+                if num_edge is None:
+                    num_edge, edge2index = cell.num_edges, cell.edge2index
+                else:
+                    assert num_edge == cell.num_edges and edge2index == cell.edge2index, 'invalid {:} vs. {:}.'.format(
+                        num_edge, cell.num_edges)
+            self.cells.append(cell)
+            C_prev = cell.out_dim
+        self.op_names = deepcopy(search_space)
+        self._Layer = len(self.cells)
+        self.edge2index = edge2index
+        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev), nn.ReLU(inplace=True))
+        self.global_pooling = nn.AdaptiveAvgPool2d(1)
+        self.classifier = nn.Linear(C_prev, num_classes)
+        # to maintain the sampled architecture
+        self.sampled_arch = None
+
+    def update_arch(self, _arch):
+        if _arch is None:
+            self.sampled_arch = None
+        elif isinstance(_arch, Structure):
+            self.sampled_arch = _arch
+        elif isinstance(_arch, (list, tuple)):
+            genotypes = []
+            for i in range(1, self.max_nodes):
+                xlist = []
+                for j in range(i):
+                    node_str = '{:}<-{:}'.format(i, j)
+                    op_index = _arch[self.edge2index[node_str]]
+                    op_name = self.op_names[op_index]
+                    xlist.append((op_name, j))
+                genotypes.append(tuple(xlist))
+            self.sampled_arch = Structure(genotypes)
+        else:
+            raise ValueError('invalid type of input architecture : {:}'.format(_arch))
+        return self.sampled_arch
+
+    def create_controller(self):
+        return Controller(len(self.edge2index), len(self.op_names))
+
+    def get_message(self):
+        string = self.extra_repr()
+        for i, cell in enumerate(self.cells):
+            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
+        return string
+
+    def extra_repr(self):
+        return ('{name}(C={_C}, Max-Nodes={max_nodes}, N={_layerN}, L={_Layer})'.format(name=self.__class__.__name__,
+                                                                                        **self.__dict__))
+
+    def forward(self, inputs):
+
+        feature = self.stem(inputs)
+        for i, cell in enumerate(self.cells):
+            if isinstance(cell, SearchCell):
+                feature = cell.forward_dynamic(feature, self.sampled_arch)
+            else:
+                feature = cell(feature)
+
+        out = self.lastact(feature)
+        out = self.global_pooling(out)
+        out = out.view(out.size(0), -1)
+        logits = self.classifier(out)
+
+        return out, logits
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_enas_utils.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_enas_utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-##################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
-##########################################################################
-# Efficient Neural Architecture Search via Parameters Sharing, ICML 2018 #
-##########################################################################
-import torch
-import torch.nn as nn
-from torch.distributions.categorical import Categorical
-
-
-class Controller(nn.Module):
-    # we refer to https://github.com/TDeVries/enas_pytorch/blob/master/models/controller.py
-    def __init__(self, num_edge, num_ops, lstm_size=32, lstm_num_layers=2, tanh_constant=2.5, temperature=5.0):
-        super(Controller, self).__init__()
-        # assign the attributes
-        self.num_edge = num_edge
-        self.num_ops = num_ops
-        self.lstm_size = lstm_size
-        self.lstm_N = lstm_num_layers
-        self.tanh_constant = tanh_constant
-        self.temperature = temperature
-        # create parameters
-        self.register_parameter('input_vars', nn.Parameter(torch.Tensor(1, 1, lstm_size)))
-        self.w_lstm = nn.LSTM(input_size=self.lstm_size, hidden_size=self.lstm_size, num_layers=self.lstm_N)
-        self.w_embd = nn.Embedding(self.num_ops, self.lstm_size)
-        self.w_pred = nn.Linear(self.lstm_size, self.num_ops)
-
-        nn.init.uniform_(self.input_vars, -0.1, 0.1)
-        nn.init.uniform_(self.w_lstm.weight_hh_l0, -0.1, 0.1)
-        nn.init.uniform_(self.w_lstm.weight_ih_l0, -0.1, 0.1)
-        nn.init.uniform_(self.w_embd.weight, -0.1, 0.1)
-        nn.init.uniform_(self.w_pred.weight, -0.1, 0.1)
-
-    def forward(self):
-        inputs, h0 = self.input_vars, None
-        log_probs, entropys, sampled_arch = [], [], []
-        for iedge in range(self.num_edge):
-            outputs, h0 = self.w_lstm(inputs, h0)
-
-            logits = self.w_pred(outputs)
-            logits = logits / self.temperature
-            logits = self.tanh_constant * torch.tanh(logits)
-            # distribution
-            op_distribution = Categorical(logits=logits)
-            op_index = op_distribution.sample()
-            sampled_arch.append(op_index.item())
-
-            op_log_prob = op_distribution.log_prob(op_index)
-            log_probs.append(op_log_prob.view(-1))
-            op_entropy = op_distribution.entropy()
-            entropys.append(op_entropy.view(-1))
-
-            # obtain the input embedding for the next step
-            inputs = self.w_embd(op_index)
-        return torch.sum(torch.cat(log_probs)), torch.sum(torch.cat(entropys)), sampled_arch
+##################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
+##########################################################################
+# Efficient Neural Architecture Search via Parameters Sharing, ICML 2018 #
+##########################################################################
+import torch
+import torch.nn as nn
+from torch.distributions.categorical import Categorical
+
+
+class Controller(nn.Module):
+    # we refer to https://github.com/TDeVries/enas_pytorch/blob/master/models/controller.py
+    def __init__(self, num_edge, num_ops, lstm_size=32, lstm_num_layers=2, tanh_constant=2.5, temperature=5.0):
+        super(Controller, self).__init__()
+        # assign the attributes
+        self.num_edge = num_edge
+        self.num_ops = num_ops
+        self.lstm_size = lstm_size
+        self.lstm_N = lstm_num_layers
+        self.tanh_constant = tanh_constant
+        self.temperature = temperature
+        # create parameters
+        self.register_parameter('input_vars', nn.Parameter(torch.Tensor(1, 1, lstm_size)))
+        self.w_lstm = nn.LSTM(input_size=self.lstm_size, hidden_size=self.lstm_size, num_layers=self.lstm_N)
+        self.w_embd = nn.Embedding(self.num_ops, self.lstm_size)
+        self.w_pred = nn.Linear(self.lstm_size, self.num_ops)
+
+        nn.init.uniform_(self.input_vars, -0.1, 0.1)
+        nn.init.uniform_(self.w_lstm.weight_hh_l0, -0.1, 0.1)
+        nn.init.uniform_(self.w_lstm.weight_ih_l0, -0.1, 0.1)
+        nn.init.uniform_(self.w_embd.weight, -0.1, 0.1)
+        nn.init.uniform_(self.w_pred.weight, -0.1, 0.1)
+
+    def forward(self):
+        inputs, h0 = self.input_vars, None
+        log_probs, entropys, sampled_arch = [], [], []
+        for iedge in range(self.num_edge):
+            outputs, h0 = self.w_lstm(inputs, h0)
+
+            logits = self.w_pred(outputs)
+            logits = logits / self.temperature
+            logits = self.tanh_constant * torch.tanh(logits)
+            # distribution
+            op_distribution = Categorical(logits=logits)
+            op_index = op_distribution.sample()
+            sampled_arch.append(op_index.item())
+
+            op_log_prob = op_distribution.log_prob(op_index)
+            log_probs.append(op_log_prob.view(-1))
+            op_entropy = op_distribution.entropy()
+            entropys.append(op_entropy.view(-1))
+
+            # obtain the input embedding for the next step
+            inputs = self.w_embd(op_index)
+        return torch.sum(torch.cat(log_probs)), torch.sum(torch.cat(entropys)), sampled_arch
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_gdas_frc_nasnet.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_setn_nasnet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,135 +1,149 @@
-###########################################################################
-# Searching for A Robust Neural Architecture in Four GPU Hours, CVPR 2019 #
-###########################################################################
-import torch
-import torch.nn as nn
-from copy import deepcopy
-from .search_cells import NASNetSearchCell as SearchCell
-from ..cell_operations import RAW_OP_CLASSES
-
-
-# The macro structure is based on NASNet
-class NASNetworkGDAS_FRC(nn.Module):
-
-    def __init__(self, C, N, steps, multiplier, stem_multiplier, num_classes, search_space, affine,
-                 track_running_stats):
-        super(NASNetworkGDAS_FRC, self).__init__()
-        self._C = C
-        self._layerN = N
-        self._steps = steps
-        self._multiplier = multiplier
-        self.stem = nn.Sequential(
-            nn.Conv2d(3, C * stem_multiplier, kernel_size=3, padding=1, bias=False),
-            nn.BatchNorm2d(C * stem_multiplier))
-
-        # config for each layer
-        layer_channels = [C] * N + [C * 2] + [C * 2] * (N - 1) + [C * 4] + [C * 4] * (N - 1)
-        layer_reductions = [False] * N + [True] + [False] * (N - 1) + [True] + [False] * (N - 1)
-
-        num_edge, edge2index = None, None
-        C_prev_prev, C_prev, C_curr, reduction_prev = C * stem_multiplier, C * stem_multiplier, C, False
-
-        self.cells = nn.ModuleList()
-        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
-            if reduction:
-                cell = RAW_OP_CLASSES['gdas_reduction'](C_prev_prev, C_prev, C_curr, reduction_prev, affine,
-                                                        track_running_stats)
-            else:
-                cell = SearchCell(search_space, steps, multiplier, C_prev_prev, C_prev, C_curr, reduction,
-                                  reduction_prev, affine, track_running_stats)
-            if num_edge is None:
-                num_edge, edge2index = cell.num_edges, cell.edge2index
-            else:
-                assert reduction or num_edge == cell.num_edges and edge2index == cell.edge2index, 'invalid {:} vs. {:}.'.format(
-                    num_edge, cell.num_edges)
-            self.cells.append(cell)
-            C_prev_prev, C_prev, reduction_prev = C_prev, cell.multiplier * C_curr, reduction
-        self.op_names = deepcopy(search_space)
-        self._Layer = len(self.cells)
-        self.edge2index = edge2index
-        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev), nn.ReLU(inplace=True))
-        self.global_pooling = nn.AdaptiveAvgPool2d(1)
-        self.classifier = nn.Linear(C_prev, num_classes)
-        self.arch_parameters = nn.Parameter(1e-3 * torch.randn(num_edge, len(search_space)))
-        self.tau = 10
-
-    def get_weights(self):
-        xlist = list(self.stem.parameters()) + list(self.cells.parameters())
-        xlist += list(self.lastact.parameters()) + list(self.global_pooling.parameters())
-        xlist += list(self.classifier.parameters())
-        return xlist
-
-    def set_tau(self, tau):
-        self.tau = tau
-
-    def get_tau(self):
-        return self.tau
-
-    def get_alphas(self):
-        return [self.arch_parameters]
-
-    def show_alphas(self):
-        with torch.no_grad():
-            A = 'arch-normal-parameters :\n{:}'.format(nn.functional.softmax(self.arch_parameters, dim=-1).cpu())
-        return '{:}'.format(A)
-
-    def get_message(self):
-        string = self.extra_repr()
-        for i, cell in enumerate(self.cells):
-            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
-        return string
-
-    def extra_repr(self):
-        return ('{name}(C={_C}, N={_layerN}, steps={_steps}, multiplier={_multiplier}, L={_Layer})'.format(
-            name=self.__class__.__name__, **self.__dict__))
-
-    def genotype(self):
-        def _parse(weights):
-            gene = []
-            for i in range(self._steps):
-                edges = []
-                for j in range(2 + i):
-                    node_str = '{:}<-{:}'.format(i, j)
-                    ws = weights[self.edge2index[node_str]]
-                    for k, op_name in enumerate(self.op_names):
-                        if op_name == 'none': continue
-                        edges.append((op_name, j, ws[k]))
-                edges = sorted(edges, key=lambda x: -x[-1])
-                selected_edges = edges[:2]
-                gene.append(tuple(selected_edges))
-            return gene
-
-        with torch.no_grad():
-            gene_normal = _parse(torch.softmax(self.arch_parameters, dim=-1).cpu().numpy())
-        return {'normal': gene_normal,
-                'normal_concat': list(range(2 + self._steps - self._multiplier, self._steps + 2))}
-
-    def forward(self, inputs):
-        def get_gumbel_prob(xins):
-            while True:
-                gumbels = -torch.empty_like(xins).exponential_().log()
-                logits = (xins.log_softmax(dim=1) + gumbels) / self.tau
-                probs = nn.functional.softmax(logits, dim=1)
-                index = probs.max(-1, keepdim=True)[1]
-                one_h = torch.zeros_like(logits).scatter_(-1, index, 1.0)
-                hardwts = one_h - probs.detach() + probs
-                if (torch.isinf(gumbels).any()) or (torch.isinf(probs).any()) or (torch.isnan(probs).any()):
-                    continue
-                else:
-                    break
-            return hardwts, index
-
-        hardwts, index = get_gumbel_prob(self.arch_parameters)
-
-        s0 = s1 = self.stem(inputs)
-        for i, cell in enumerate(self.cells):
-            if cell.reduction:
-                s0, s1 = s1, cell(s0, s1)
-            else:
-                s0, s1 = s1, cell.forward_gdas(s0, s1, hardwts, index)
-        out = self.lastact(s1)
-        out = self.global_pooling(out)
-        out = out.view(out.size(0), -1)
-        logits = self.classifier(out)
-
-        return out, logits
+#####################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019.01 #
+######################################################################################
+# One-Shot Neural Architecture Search via Self-Evaluated Template Network, ICCV 2019 #
+######################################################################################
+import torch
+import torch.nn as nn
+from copy import deepcopy
+from typing import List, Text, Dict
+from .search_cells import NASNetSearchCell as SearchCell
+
+
+# The macro structure is based on NASNet
+class NASNetworkSETN(nn.Module):
+
+    def __init__(self, C: int, N: int, steps: int, multiplier: int, stem_multiplier: int,
+                 num_classes: int, search_space: List[Text], affine: bool, track_running_stats: bool):
+        super(NASNetworkSETN, self).__init__()
+        self._C = C
+        self._layerN = N
+        self._steps = steps
+        self._multiplier = multiplier
+        self.stem = nn.Sequential(
+            nn.Conv2d(3, C * stem_multiplier, kernel_size=3, padding=1, bias=False),
+            nn.BatchNorm2d(C * stem_multiplier))
+
+        # config for each layer
+        layer_channels = [C] * N + [C * 2] + [C * 2] * (N - 1) + [C * 4] + [C * 4] * (N - 1)
+        layer_reductions = [False] * N + [True] + [False] * (N - 1) + [True] + [False] * (N - 1)
+
+        num_edge, edge2index = None, None
+        C_prev_prev, C_prev, C_curr, reduction_prev = C * stem_multiplier, C * stem_multiplier, C, False
+
+        self.cells = nn.ModuleList()
+        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
+            cell = SearchCell(search_space, steps, multiplier, C_prev_prev, C_prev, C_curr, reduction, reduction_prev,
+                              affine, track_running_stats)
+            if num_edge is None:
+                num_edge, edge2index = cell.num_edges, cell.edge2index
+            else:
+                assert num_edge == cell.num_edges and edge2index == cell.edge2index, 'invalid {:} vs. {:}.'.format(
+                    num_edge, cell.num_edges)
+            self.cells.append(cell)
+            C_prev_prev, C_prev, reduction_prev = C_prev, multiplier * C_curr, reduction
+        self.op_names = deepcopy(search_space)
+        self._Layer = len(self.cells)
+        self.edge2index = edge2index
+        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev), nn.ReLU(inplace=True))
+        self.global_pooling = nn.AdaptiveAvgPool2d(1)
+        self.classifier = nn.Linear(C_prev, num_classes)
+        self.arch_normal_parameters = nn.Parameter(1e-3 * torch.randn(num_edge, len(search_space)))
+        self.arch_reduce_parameters = nn.Parameter(1e-3 * torch.randn(num_edge, len(search_space)))
+        self.mode = 'urs'
+        self.dynamic_cell = None
+
+    def set_cal_mode(self, mode, dynamic_cell=None):
+        assert mode in ['urs', 'joint', 'select', 'dynamic']
+        self.mode = mode
+        if mode == 'dynamic':
+            self.dynamic_cell = deepcopy(dynamic_cell)
+        else:
+            self.dynamic_cell = None
+
+    def get_weights(self):
+        xlist = list(self.stem.parameters()) + list(self.cells.parameters())
+        xlist += list(self.lastact.parameters()) + list(self.global_pooling.parameters())
+        xlist += list(self.classifier.parameters())
+        return xlist
+
+    def get_alphas(self):
+        return [self.arch_normal_parameters, self.arch_reduce_parameters]
+
+    def show_alphas(self):
+        with torch.no_grad():
+            A = 'arch-normal-parameters :\n{:}'.format(nn.functional.softmax(self.arch_normal_parameters, dim=-1).cpu())
+            B = 'arch-reduce-parameters :\n{:}'.format(nn.functional.softmax(self.arch_reduce_parameters, dim=-1).cpu())
+        return '{:}\n{:}'.format(A, B)
+
+    def get_message(self):
+        string = self.extra_repr()
+        for i, cell in enumerate(self.cells):
+            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
+        return string
+
+    def extra_repr(self):
+        return ('{name}(C={_C}, N={_layerN}, steps={_steps}, multiplier={_multiplier}, L={_Layer})'.format(
+            name=self.__class__.__name__, **self.__dict__))
+
+    def dync_genotype(self, use_random=False):
+        genotypes = []
+        with torch.no_grad():
+            alphas_cpu = nn.functional.softmax(self.arch_parameters, dim=-1)
+        for i in range(1, self.max_nodes):
+            xlist = []
+            for j in range(i):
+                node_str = '{:}<-{:}'.format(i, j)
+                if use_random:
+                    op_name = random.choice(self.op_names)
+                else:
+                    weights = alphas_cpu[self.edge2index[node_str]]
+                    op_index = torch.multinomial(weights, 1).item()
+                    op_name = self.op_names[op_index]
+                xlist.append((op_name, j))
+            genotypes.append(tuple(xlist))
+        return Structure(genotypes)
+
+    def genotype(self):
+        def _parse(weights):
+            gene = []
+            for i in range(self._steps):
+                edges = []
+                for j in range(2 + i):
+                    node_str = '{:}<-{:}'.format(i, j)
+                    ws = weights[self.edge2index[node_str]]
+                    for k, op_name in enumerate(self.op_names):
+                        if op_name == 'none': continue
+                        edges.append((op_name, j, ws[k]))
+                edges = sorted(edges, key=lambda x: -x[-1])
+                selected_edges = edges[:2]
+                gene.append(tuple(selected_edges))
+            return gene
+
+        with torch.no_grad():
+            gene_normal = _parse(torch.softmax(self.arch_normal_parameters, dim=-1).cpu().numpy())
+            gene_reduce = _parse(torch.softmax(self.arch_reduce_parameters, dim=-1).cpu().numpy())
+        return {'normal': gene_normal,
+                'normal_concat': list(range(2 + self._steps - self._multiplier, self._steps + 2)),
+                'reduce': gene_reduce,
+                'reduce_concat': list(range(2 + self._steps - self._multiplier, self._steps + 2))}
+
+    def forward(self, inputs):
+        normal_hardwts = nn.functional.softmax(self.arch_normal_parameters, dim=-1)
+        reduce_hardwts = nn.functional.softmax(self.arch_reduce_parameters, dim=-1)
+
+        s0 = s1 = self.stem(inputs)
+        for i, cell in enumerate(self.cells):
+            # [TODO]
+            raise NotImplementedError
+            if cell.reduction:
+                hardwts, index = reduce_hardwts, reduce_index
+            else:
+                hardwts, index = normal_hardwts, normal_index
+            s0, s1 = s1, cell.forward_gdas(s0, s1, hardwts, index)
+        out = self.lastact(s1)
+        out = self.global_pooling(out)
+        out = out.view(out.size(0), -1)
+        logits = self.classifier(out)
+
+        return out, logits
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_gdas_nasnet.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_gdas_nasnet.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-###########################################################################
-# Searching for A Robust Neural Architecture in Four GPU Hours, CVPR 2019 #
-###########################################################################
-import torch
-import torch.nn as nn
-from copy import deepcopy
-from .search_cells import NASNetSearchCell as SearchCell
-
-
-# The macro structure is based on NASNet
-class NASNetworkGDAS(nn.Module):
-
-    def __init__(self, C, N, steps, multiplier, stem_multiplier, num_classes, search_space, affine,
-                 track_running_stats):
-        super(NASNetworkGDAS, self).__init__()
-        self._C = C
-        self._layerN = N
-        self._steps = steps
-        self._multiplier = multiplier
-        self.stem = nn.Sequential(
-            nn.Conv2d(3, C * stem_multiplier, kernel_size=3, padding=1, bias=False),
-            nn.BatchNorm2d(C * stem_multiplier))
-
-        # config for each layer
-        layer_channels = [C] * N + [C * 2] + [C * 2] * (N - 1) + [C * 4] + [C * 4] * (N - 1)
-        layer_reductions = [False] * N + [True] + [False] * (N - 1) + [True] + [False] * (N - 1)
-
-        num_edge, edge2index = None, None
-        C_prev_prev, C_prev, C_curr, reduction_prev = C * stem_multiplier, C * stem_multiplier, C, False
-
-        self.cells = nn.ModuleList()
-        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
-            cell = SearchCell(search_space, steps, multiplier, C_prev_prev, C_prev, C_curr, reduction, reduction_prev,
-                              affine, track_running_stats)
-            if num_edge is None:
-                num_edge, edge2index = cell.num_edges, cell.edge2index
-            else:
-                assert num_edge == cell.num_edges and edge2index == cell.edge2index, 'invalid {:} vs. {:}.'.format(
-                    num_edge, cell.num_edges)
-            self.cells.append(cell)
-            C_prev_prev, C_prev, reduction_prev = C_prev, multiplier * C_curr, reduction
-        self.op_names = deepcopy(search_space)
-        self._Layer = len(self.cells)
-        self.edge2index = edge2index
-        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev), nn.ReLU(inplace=True))
-        self.global_pooling = nn.AdaptiveAvgPool2d(1)
-        self.classifier = nn.Linear(C_prev, num_classes)
-        self.arch_normal_parameters = nn.Parameter(1e-3 * torch.randn(num_edge, len(search_space)))
-        self.arch_reduce_parameters = nn.Parameter(1e-3 * torch.randn(num_edge, len(search_space)))
-        self.tau = 10
-
-    def get_weights(self):
-        xlist = list(self.stem.parameters()) + list(self.cells.parameters())
-        xlist += list(self.lastact.parameters()) + list(self.global_pooling.parameters())
-        xlist += list(self.classifier.parameters())
-        return xlist
-
-    def set_tau(self, tau):
-        self.tau = tau
-
-    def get_tau(self):
-        return self.tau
-
-    def get_alphas(self):
-        return [self.arch_normal_parameters, self.arch_reduce_parameters]
-
-    def show_alphas(self):
-        with torch.no_grad():
-            A = 'arch-normal-parameters :\n{:}'.format(nn.functional.softmax(self.arch_normal_parameters, dim=-1).cpu())
-            B = 'arch-reduce-parameters :\n{:}'.format(nn.functional.softmax(self.arch_reduce_parameters, dim=-1).cpu())
-        return '{:}\n{:}'.format(A, B)
-
-    def get_message(self):
-        string = self.extra_repr()
-        for i, cell in enumerate(self.cells):
-            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
-        return string
-
-    def extra_repr(self):
-        return ('{name}(C={_C}, N={_layerN}, steps={_steps}, multiplier={_multiplier}, L={_Layer})'.format(
-            name=self.__class__.__name__, **self.__dict__))
-
-    def genotype(self):
-        def _parse(weights):
-            gene = []
-            for i in range(self._steps):
-                edges = []
-                for j in range(2 + i):
-                    node_str = '{:}<-{:}'.format(i, j)
-                    ws = weights[self.edge2index[node_str]]
-                    for k, op_name in enumerate(self.op_names):
-                        if op_name == 'none': continue
-                        edges.append((op_name, j, ws[k]))
-                edges = sorted(edges, key=lambda x: -x[-1])
-                selected_edges = edges[:2]
-                gene.append(tuple(selected_edges))
-            return gene
-
-        with torch.no_grad():
-            gene_normal = _parse(torch.softmax(self.arch_normal_parameters, dim=-1).cpu().numpy())
-            gene_reduce = _parse(torch.softmax(self.arch_reduce_parameters, dim=-1).cpu().numpy())
-        return {'normal': gene_normal,
-                'normal_concat': list(range(2 + self._steps - self._multiplier, self._steps + 2)),
-                'reduce': gene_reduce,
-                'reduce_concat': list(range(2 + self._steps - self._multiplier, self._steps + 2))}
-
-    def forward(self, inputs):
-        def get_gumbel_prob(xins):
-            while True:
-                gumbels = -torch.empty_like(xins).exponential_().log()
-                logits = (xins.log_softmax(dim=1) + gumbels) / self.tau
-                probs = nn.functional.softmax(logits, dim=1)
-                index = probs.max(-1, keepdim=True)[1]
-                one_h = torch.zeros_like(logits).scatter_(-1, index, 1.0)
-                hardwts = one_h - probs.detach() + probs
-                if (torch.isinf(gumbels).any()) or (torch.isinf(probs).any()) or (torch.isnan(probs).any()):
-                    continue
-                else:
-                    break
-            return hardwts, index
-
-        normal_hardwts, normal_index = get_gumbel_prob(self.arch_normal_parameters)
-        reduce_hardwts, reduce_index = get_gumbel_prob(self.arch_reduce_parameters)
-
-        s0 = s1 = self.stem(inputs)
-        for i, cell in enumerate(self.cells):
-            if cell.reduction:
-                hardwts, index = reduce_hardwts, reduce_index
-            else:
-                hardwts, index = normal_hardwts, normal_index
-            s0, s1 = s1, cell.forward_gdas(s0, s1, hardwts, index)
-        out = self.lastact(s1)
-        out = self.global_pooling(out)
-        out = out.view(out.size(0), -1)
-        logits = self.classifier(out)
-
-        return out, logits
+###########################################################################
+# Searching for A Robust Neural Architecture in Four GPU Hours, CVPR 2019 #
+###########################################################################
+import torch
+import torch.nn as nn
+from copy import deepcopy
+from .search_cells import NASNetSearchCell as SearchCell
+
+
+# The macro structure is based on NASNet
+class NASNetworkGDAS(nn.Module):
+
+    def __init__(self, C, N, steps, multiplier, stem_multiplier, num_classes, search_space, affine,
+                 track_running_stats):
+        super(NASNetworkGDAS, self).__init__()
+        self._C = C
+        self._layerN = N
+        self._steps = steps
+        self._multiplier = multiplier
+        self.stem = nn.Sequential(
+            nn.Conv2d(3, C * stem_multiplier, kernel_size=3, padding=1, bias=False),
+            nn.BatchNorm2d(C * stem_multiplier))
+
+        # config for each layer
+        layer_channels = [C] * N + [C * 2] + [C * 2] * (N - 1) + [C * 4] + [C * 4] * (N - 1)
+        layer_reductions = [False] * N + [True] + [False] * (N - 1) + [True] + [False] * (N - 1)
+
+        num_edge, edge2index = None, None
+        C_prev_prev, C_prev, C_curr, reduction_prev = C * stem_multiplier, C * stem_multiplier, C, False
+
+        self.cells = nn.ModuleList()
+        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
+            cell = SearchCell(search_space, steps, multiplier, C_prev_prev, C_prev, C_curr, reduction, reduction_prev,
+                              affine, track_running_stats)
+            if num_edge is None:
+                num_edge, edge2index = cell.num_edges, cell.edge2index
+            else:
+                assert num_edge == cell.num_edges and edge2index == cell.edge2index, 'invalid {:} vs. {:}.'.format(
+                    num_edge, cell.num_edges)
+            self.cells.append(cell)
+            C_prev_prev, C_prev, reduction_prev = C_prev, multiplier * C_curr, reduction
+        self.op_names = deepcopy(search_space)
+        self._Layer = len(self.cells)
+        self.edge2index = edge2index
+        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev), nn.ReLU(inplace=True))
+        self.global_pooling = nn.AdaptiveAvgPool2d(1)
+        self.classifier = nn.Linear(C_prev, num_classes)
+        self.arch_normal_parameters = nn.Parameter(1e-3 * torch.randn(num_edge, len(search_space)))
+        self.arch_reduce_parameters = nn.Parameter(1e-3 * torch.randn(num_edge, len(search_space)))
+        self.tau = 10
+
+    def get_weights(self):
+        xlist = list(self.stem.parameters()) + list(self.cells.parameters())
+        xlist += list(self.lastact.parameters()) + list(self.global_pooling.parameters())
+        xlist += list(self.classifier.parameters())
+        return xlist
+
+    def set_tau(self, tau):
+        self.tau = tau
+
+    def get_tau(self):
+        return self.tau
+
+    def get_alphas(self):
+        return [self.arch_normal_parameters, self.arch_reduce_parameters]
+
+    def show_alphas(self):
+        with torch.no_grad():
+            A = 'arch-normal-parameters :\n{:}'.format(nn.functional.softmax(self.arch_normal_parameters, dim=-1).cpu())
+            B = 'arch-reduce-parameters :\n{:}'.format(nn.functional.softmax(self.arch_reduce_parameters, dim=-1).cpu())
+        return '{:}\n{:}'.format(A, B)
+
+    def get_message(self):
+        string = self.extra_repr()
+        for i, cell in enumerate(self.cells):
+            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
+        return string
+
+    def extra_repr(self):
+        return ('{name}(C={_C}, N={_layerN}, steps={_steps}, multiplier={_multiplier}, L={_Layer})'.format(
+            name=self.__class__.__name__, **self.__dict__))
+
+    def genotype(self):
+        def _parse(weights):
+            gene = []
+            for i in range(self._steps):
+                edges = []
+                for j in range(2 + i):
+                    node_str = '{:}<-{:}'.format(i, j)
+                    ws = weights[self.edge2index[node_str]]
+                    for k, op_name in enumerate(self.op_names):
+                        if op_name == 'none': continue
+                        edges.append((op_name, j, ws[k]))
+                edges = sorted(edges, key=lambda x: -x[-1])
+                selected_edges = edges[:2]
+                gene.append(tuple(selected_edges))
+            return gene
+
+        with torch.no_grad():
+            gene_normal = _parse(torch.softmax(self.arch_normal_parameters, dim=-1).cpu().numpy())
+            gene_reduce = _parse(torch.softmax(self.arch_reduce_parameters, dim=-1).cpu().numpy())
+        return {'normal': gene_normal,
+                'normal_concat': list(range(2 + self._steps - self._multiplier, self._steps + 2)),
+                'reduce': gene_reduce,
+                'reduce_concat': list(range(2 + self._steps - self._multiplier, self._steps + 2))}
+
+    def forward(self, inputs):
+        def get_gumbel_prob(xins):
+            while True:
+                gumbels = -torch.empty_like(xins).exponential_().log()
+                logits = (xins.log_softmax(dim=1) + gumbels) / self.tau
+                probs = nn.functional.softmax(logits, dim=1)
+                index = probs.max(-1, keepdim=True)[1]
+                one_h = torch.zeros_like(logits).scatter_(-1, index, 1.0)
+                hardwts = one_h - probs.detach() + probs
+                if (torch.isinf(gumbels).any()) or (torch.isinf(probs).any()) or (torch.isnan(probs).any()):
+                    continue
+                else:
+                    break
+            return hardwts, index
+
+        normal_hardwts, normal_index = get_gumbel_prob(self.arch_normal_parameters)
+        reduce_hardwts, reduce_index = get_gumbel_prob(self.arch_reduce_parameters)
+
+        s0 = s1 = self.stem(inputs)
+        for i, cell in enumerate(self.cells):
+            if cell.reduction:
+                hardwts, index = reduce_hardwts, reduce_index
+            else:
+                hardwts, index = normal_hardwts, normal_index
+            s0, s1 = s1, cell.forward_gdas(s0, s1, hardwts, index)
+        out = self.lastact(s1)
+        out = self.global_pooling(out)
+        out = out.view(out.size(0), -1)
+        logits = self.classifier(out)
+
+        return out, logits
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_random.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_random.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-##################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
-##############################################################################
-# Random Search and Reproducibility for Neural Architecture Search, UAI 2019 # 
-##############################################################################
-import torch, random
-import torch.nn as nn
-from copy import deepcopy
-from ..cell_operations import ResNetBasicblock
-from .search_cells import NAS201SearchCell as SearchCell
-from .genotypes import Structure
-
-
-class TinyNetworkRANDOM(nn.Module):
-
-    def __init__(self, C, N, max_nodes, num_classes, search_space, affine, track_running_stats):
-        super(TinyNetworkRANDOM, self).__init__()
-        self._C = C
-        self._layerN = N
-        self.max_nodes = max_nodes
-        self.stem = nn.Sequential(
-            nn.Conv2d(3, C, kernel_size=3, padding=1, bias=False),
-            nn.BatchNorm2d(C))
-
-        layer_channels = [C] * N + [C * 2] + [C * 2] * N + [C * 4] + [C * 4] * N
-        layer_reductions = [False] * N + [True] + [False] * N + [True] + [False] * N
-
-        C_prev, num_edge, edge2index = C, None, None
-        self.cells = nn.ModuleList()
-        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
-            if reduction:
-                cell = ResNetBasicblock(C_prev, C_curr, 2)
-            else:
-                cell = SearchCell(C_prev, C_curr, 1, max_nodes, search_space, affine, track_running_stats)
-                if num_edge is None:
-                    num_edge, edge2index = cell.num_edges, cell.edge2index
-                else:
-                    assert num_edge == cell.num_edges and edge2index == cell.edge2index, 'invalid {:} vs. {:}.'.format(
-                        num_edge, cell.num_edges)
-            self.cells.append(cell)
-            C_prev = cell.out_dim
-        self.op_names = deepcopy(search_space)
-        self._Layer = len(self.cells)
-        self.edge2index = edge2index
-        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev), nn.ReLU(inplace=True))
-        self.global_pooling = nn.AdaptiveAvgPool2d(1)
-        self.classifier = nn.Linear(C_prev, num_classes)
-        self.arch_cache = None
-
-    def get_message(self):
-        string = self.extra_repr()
-        for i, cell in enumerate(self.cells):
-            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
-        return string
-
-    def extra_repr(self):
-        return ('{name}(C={_C}, Max-Nodes={max_nodes}, N={_layerN}, L={_Layer})'.format(name=self.__class__.__name__,
-                                                                                        **self.__dict__))
-
-    def random_genotype(self, set_cache):
-        genotypes = []
-        for i in range(1, self.max_nodes):
-            xlist = []
-            for j in range(i):
-                node_str = '{:}<-{:}'.format(i, j)
-                op_name = random.choice(self.op_names)
-                xlist.append((op_name, j))
-            genotypes.append(tuple(xlist))
-        arch = Structure(genotypes)
-        if set_cache: self.arch_cache = arch
-        return arch
-
-    def forward(self, inputs):
-
-        feature = self.stem(inputs)
-        for i, cell in enumerate(self.cells):
-            if isinstance(cell, SearchCell):
-                feature = cell.forward_dynamic(feature, self.arch_cache)
-            else:
-                feature = cell(feature)
-
-        out = self.lastact(feature)
-        out = self.global_pooling(out)
-        out = out.view(out.size(0), -1)
-        logits = self.classifier(out)
-        return out, logits
+##################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
+##############################################################################
+# Random Search and Reproducibility for Neural Architecture Search, UAI 2019 # 
+##############################################################################
+import torch, random
+import torch.nn as nn
+from copy import deepcopy
+from ..cell_operations import ResNetBasicblock
+from .search_cells import NAS201SearchCell as SearchCell
+from .genotypes import Structure
+
+
+class TinyNetworkRANDOM(nn.Module):
+
+    def __init__(self, C, N, max_nodes, num_classes, search_space, affine, track_running_stats):
+        super(TinyNetworkRANDOM, self).__init__()
+        self._C = C
+        self._layerN = N
+        self.max_nodes = max_nodes
+        self.stem = nn.Sequential(
+            nn.Conv2d(3, C, kernel_size=3, padding=1, bias=False),
+            nn.BatchNorm2d(C))
+
+        layer_channels = [C] * N + [C * 2] + [C * 2] * N + [C * 4] + [C * 4] * N
+        layer_reductions = [False] * N + [True] + [False] * N + [True] + [False] * N
+
+        C_prev, num_edge, edge2index = C, None, None
+        self.cells = nn.ModuleList()
+        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
+            if reduction:
+                cell = ResNetBasicblock(C_prev, C_curr, 2)
+            else:
+                cell = SearchCell(C_prev, C_curr, 1, max_nodes, search_space, affine, track_running_stats)
+                if num_edge is None:
+                    num_edge, edge2index = cell.num_edges, cell.edge2index
+                else:
+                    assert num_edge == cell.num_edges and edge2index == cell.edge2index, 'invalid {:} vs. {:}.'.format(
+                        num_edge, cell.num_edges)
+            self.cells.append(cell)
+            C_prev = cell.out_dim
+        self.op_names = deepcopy(search_space)
+        self._Layer = len(self.cells)
+        self.edge2index = edge2index
+        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev), nn.ReLU(inplace=True))
+        self.global_pooling = nn.AdaptiveAvgPool2d(1)
+        self.classifier = nn.Linear(C_prev, num_classes)
+        self.arch_cache = None
+
+    def get_message(self):
+        string = self.extra_repr()
+        for i, cell in enumerate(self.cells):
+            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
+        return string
+
+    def extra_repr(self):
+        return ('{name}(C={_C}, Max-Nodes={max_nodes}, N={_layerN}, L={_Layer})'.format(name=self.__class__.__name__,
+                                                                                        **self.__dict__))
+
+    def random_genotype(self, set_cache):
+        genotypes = []
+        for i in range(1, self.max_nodes):
+            xlist = []
+            for j in range(i):
+                node_str = '{:}<-{:}'.format(i, j)
+                op_name = random.choice(self.op_names)
+                xlist.append((op_name, j))
+            genotypes.append(tuple(xlist))
+        arch = Structure(genotypes)
+        if set_cache: self.arch_cache = arch
+        return arch
+
+    def forward(self, inputs):
+
+        feature = self.stem(inputs)
+        for i, cell in enumerate(self.cells):
+            if isinstance(cell, SearchCell):
+                feature = cell.forward_dynamic(feature, self.arch_cache)
+            else:
+                feature = cell(feature)
+
+        out = self.lastact(feature)
+        out = self.global_pooling(out)
+        out = out.view(out.size(0), -1)
+        logits = self.classifier(out)
+        return out, logits
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_setn.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/cell_searchs/search_model_setn.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,158 +1,158 @@
-#####################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019.01 #
-######################################################################################
-# One-Shot Neural Architecture Search via Self-Evaluated Template Network, ICCV 2019 #
-######################################################################################
-import torch, random
-import torch.nn as nn
-from copy import deepcopy
-from ..cell_operations import ResNetBasicblock
-from .search_cells import NAS201SearchCell as SearchCell
-from .genotypes import Structure
-
-
-class TinyNetworkSETN(nn.Module):
-
-    def __init__(self, C, N, max_nodes, num_classes, search_space, affine, track_running_stats):
-        super(TinyNetworkSETN, self).__init__()
-        self._C = C
-        self._layerN = N
-        self.max_nodes = max_nodes
-        self.stem = nn.Sequential(
-            nn.Conv2d(3, C, kernel_size=3, padding=1, bias=False),
-            nn.BatchNorm2d(C))
-
-        layer_channels = [C] * N + [C * 2] + [C * 2] * N + [C * 4] + [C * 4] * N
-        layer_reductions = [False] * N + [True] + [False] * N + [True] + [False] * N
-
-        C_prev, num_edge, edge2index = C, None, None
-        self.cells = nn.ModuleList()
-        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
-            if reduction:
-                cell = ResNetBasicblock(C_prev, C_curr, 2)
-            else:
-                cell = SearchCell(C_prev, C_curr, 1, max_nodes, search_space, affine, track_running_stats)
-                if num_edge is None:
-                    num_edge, edge2index = cell.num_edges, cell.edge2index
-                else:
-                    assert num_edge == cell.num_edges and edge2index == cell.edge2index, 'invalid {:} vs. {:}.'.format(
-                        num_edge, cell.num_edges)
-            self.cells.append(cell)
-            C_prev = cell.out_dim
-        self.op_names = deepcopy(search_space)
-        self._Layer = len(self.cells)
-        self.edge2index = edge2index
-        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev), nn.ReLU(inplace=True))
-        self.global_pooling = nn.AdaptiveAvgPool2d(1)
-        self.classifier = nn.Linear(C_prev, num_classes)
-        self.arch_parameters = nn.Parameter(1e-3 * torch.randn(num_edge, len(search_space)))
-        self.mode = 'urs'
-        self.dynamic_cell = None
-
-    def set_cal_mode(self, mode, dynamic_cell=None):
-        assert mode in ['urs', 'joint', 'select', 'dynamic']
-        self.mode = mode
-        if mode == 'dynamic':
-            self.dynamic_cell = deepcopy(dynamic_cell)
-        else:
-            self.dynamic_cell = None
-
-    def get_cal_mode(self):
-        return self.mode
-
-    def get_weights(self):
-        xlist = list(self.stem.parameters()) + list(self.cells.parameters())
-        xlist += list(self.lastact.parameters()) + list(self.global_pooling.parameters())
-        xlist += list(self.classifier.parameters())
-        return xlist
-
-    def get_alphas(self):
-        return [self.arch_parameters]
-
-    def get_message(self):
-        string = self.extra_repr()
-        for i, cell in enumerate(self.cells):
-            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
-        return string
-
-    def extra_repr(self):
-        return ('{name}(C={_C}, Max-Nodes={max_nodes}, N={_layerN}, L={_Layer})'.format(name=self.__class__.__name__,
-                                                                                        **self.__dict__))
-
-    def genotype(self):
-        genotypes = []
-        for i in range(1, self.max_nodes):
-            xlist = []
-            for j in range(i):
-                node_str = '{:}<-{:}'.format(i, j)
-                with torch.no_grad():
-                    weights = self.arch_parameters[self.edge2index[node_str]]
-                    op_name = self.op_names[weights.argmax().item()]
-                xlist.append((op_name, j))
-            genotypes.append(tuple(xlist))
-        return Structure(genotypes)
-
-    def dync_genotype(self, use_random=False):
-        genotypes = []
-        with torch.no_grad():
-            alphas_cpu = nn.functional.softmax(self.arch_parameters, dim=-1)
-        for i in range(1, self.max_nodes):
-            xlist = []
-            for j in range(i):
-                node_str = '{:}<-{:}'.format(i, j)
-                if use_random:
-                    op_name = random.choice(self.op_names)
-                else:
-                    weights = alphas_cpu[self.edge2index[node_str]]
-                    op_index = torch.multinomial(weights, 1).item()
-                    op_name = self.op_names[op_index]
-                xlist.append((op_name, j))
-            genotypes.append(tuple(xlist))
-        return Structure(genotypes)
-
-    def get_log_prob(self, arch):
-        with torch.no_grad():
-            logits = nn.functional.log_softmax(self.arch_parameters, dim=-1)
-        select_logits = []
-        for i, node_info in enumerate(arch.nodes):
-            for op, xin in node_info:
-                node_str = '{:}<-{:}'.format(i + 1, xin)
-                op_index = self.op_names.index(op)
-                select_logits.append(logits[self.edge2index[node_str], op_index])
-        return sum(select_logits).item()
-
-    def return_topK(self, K):
-        archs = Structure.gen_all(self.op_names, self.max_nodes, False)
-        pairs = [(self.get_log_prob(arch), arch) for arch in archs]
-        if K < 0 or K >= len(archs): K = len(archs)
-        sorted_pairs = sorted(pairs, key=lambda x: -x[0])
-        return_pairs = [sorted_pairs[_][1] for _ in range(K)]
-        return return_pairs
-
-    def forward(self, inputs):
-        alphas = nn.functional.softmax(self.arch_parameters, dim=-1)
-        with torch.no_grad():
-            alphas_cpu = alphas.detach().cpu()
-
-        feature = self.stem(inputs)
-        for i, cell in enumerate(self.cells):
-            if isinstance(cell, SearchCell):
-                if self.mode == 'urs':
-                    feature = cell.forward_urs(feature)
-                elif self.mode == 'select':
-                    feature = cell.forward_select(feature, alphas_cpu)
-                elif self.mode == 'joint':
-                    feature = cell.forward_joint(feature, alphas)
-                elif self.mode == 'dynamic':
-                    feature = cell.forward_dynamic(feature, self.dynamic_cell)
-                else:
-                    raise ValueError('invalid mode={:}'.format(self.mode))
-            else:
-                feature = cell(feature)
-
-        out = self.lastact(feature)
-        out = self.global_pooling(out)
-        out = out.view(out.size(0), -1)
-        logits = self.classifier(out)
-
-        return out, logits
+#####################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019.01 #
+######################################################################################
+# One-Shot Neural Architecture Search via Self-Evaluated Template Network, ICCV 2019 #
+######################################################################################
+import torch, random
+import torch.nn as nn
+from copy import deepcopy
+from ..cell_operations import ResNetBasicblock
+from .search_cells import NAS201SearchCell as SearchCell
+from .genotypes import Structure
+
+
+class TinyNetworkSETN(nn.Module):
+
+    def __init__(self, C, N, max_nodes, num_classes, search_space, affine, track_running_stats):
+        super(TinyNetworkSETN, self).__init__()
+        self._C = C
+        self._layerN = N
+        self.max_nodes = max_nodes
+        self.stem = nn.Sequential(
+            nn.Conv2d(3, C, kernel_size=3, padding=1, bias=False),
+            nn.BatchNorm2d(C))
+
+        layer_channels = [C] * N + [C * 2] + [C * 2] * N + [C * 4] + [C * 4] * N
+        layer_reductions = [False] * N + [True] + [False] * N + [True] + [False] * N
+
+        C_prev, num_edge, edge2index = C, None, None
+        self.cells = nn.ModuleList()
+        for index, (C_curr, reduction) in enumerate(zip(layer_channels, layer_reductions)):
+            if reduction:
+                cell = ResNetBasicblock(C_prev, C_curr, 2)
+            else:
+                cell = SearchCell(C_prev, C_curr, 1, max_nodes, search_space, affine, track_running_stats)
+                if num_edge is None:
+                    num_edge, edge2index = cell.num_edges, cell.edge2index
+                else:
+                    assert num_edge == cell.num_edges and edge2index == cell.edge2index, 'invalid {:} vs. {:}.'.format(
+                        num_edge, cell.num_edges)
+            self.cells.append(cell)
+            C_prev = cell.out_dim
+        self.op_names = deepcopy(search_space)
+        self._Layer = len(self.cells)
+        self.edge2index = edge2index
+        self.lastact = nn.Sequential(nn.BatchNorm2d(C_prev), nn.ReLU(inplace=True))
+        self.global_pooling = nn.AdaptiveAvgPool2d(1)
+        self.classifier = nn.Linear(C_prev, num_classes)
+        self.arch_parameters = nn.Parameter(1e-3 * torch.randn(num_edge, len(search_space)))
+        self.mode = 'urs'
+        self.dynamic_cell = None
+
+    def set_cal_mode(self, mode, dynamic_cell=None):
+        assert mode in ['urs', 'joint', 'select', 'dynamic']
+        self.mode = mode
+        if mode == 'dynamic':
+            self.dynamic_cell = deepcopy(dynamic_cell)
+        else:
+            self.dynamic_cell = None
+
+    def get_cal_mode(self):
+        return self.mode
+
+    def get_weights(self):
+        xlist = list(self.stem.parameters()) + list(self.cells.parameters())
+        xlist += list(self.lastact.parameters()) + list(self.global_pooling.parameters())
+        xlist += list(self.classifier.parameters())
+        return xlist
+
+    def get_alphas(self):
+        return [self.arch_parameters]
+
+    def get_message(self):
+        string = self.extra_repr()
+        for i, cell in enumerate(self.cells):
+            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
+        return string
+
+    def extra_repr(self):
+        return ('{name}(C={_C}, Max-Nodes={max_nodes}, N={_layerN}, L={_Layer})'.format(name=self.__class__.__name__,
+                                                                                        **self.__dict__))
+
+    def genotype(self):
+        genotypes = []
+        for i in range(1, self.max_nodes):
+            xlist = []
+            for j in range(i):
+                node_str = '{:}<-{:}'.format(i, j)
+                with torch.no_grad():
+                    weights = self.arch_parameters[self.edge2index[node_str]]
+                    op_name = self.op_names[weights.argmax().item()]
+                xlist.append((op_name, j))
+            genotypes.append(tuple(xlist))
+        return Structure(genotypes)
+
+    def dync_genotype(self, use_random=False):
+        genotypes = []
+        with torch.no_grad():
+            alphas_cpu = nn.functional.softmax(self.arch_parameters, dim=-1)
+        for i in range(1, self.max_nodes):
+            xlist = []
+            for j in range(i):
+                node_str = '{:}<-{:}'.format(i, j)
+                if use_random:
+                    op_name = random.choice(self.op_names)
+                else:
+                    weights = alphas_cpu[self.edge2index[node_str]]
+                    op_index = torch.multinomial(weights, 1).item()
+                    op_name = self.op_names[op_index]
+                xlist.append((op_name, j))
+            genotypes.append(tuple(xlist))
+        return Structure(genotypes)
+
+    def get_log_prob(self, arch):
+        with torch.no_grad():
+            logits = nn.functional.log_softmax(self.arch_parameters, dim=-1)
+        select_logits = []
+        for i, node_info in enumerate(arch.nodes):
+            for op, xin in node_info:
+                node_str = '{:}<-{:}'.format(i + 1, xin)
+                op_index = self.op_names.index(op)
+                select_logits.append(logits[self.edge2index[node_str], op_index])
+        return sum(select_logits).item()
+
+    def return_topK(self, K):
+        archs = Structure.gen_all(self.op_names, self.max_nodes, False)
+        pairs = [(self.get_log_prob(arch), arch) for arch in archs]
+        if K < 0 or K >= len(archs): K = len(archs)
+        sorted_pairs = sorted(pairs, key=lambda x: -x[0])
+        return_pairs = [sorted_pairs[_][1] for _ in range(K)]
+        return return_pairs
+
+    def forward(self, inputs):
+        alphas = nn.functional.softmax(self.arch_parameters, dim=-1)
+        with torch.no_grad():
+            alphas_cpu = alphas.detach().cpu()
+
+        feature = self.stem(inputs)
+        for i, cell in enumerate(self.cells):
+            if isinstance(cell, SearchCell):
+                if self.mode == 'urs':
+                    feature = cell.forward_urs(feature)
+                elif self.mode == 'select':
+                    feature = cell.forward_select(feature, alphas_cpu)
+                elif self.mode == 'joint':
+                    feature = cell.forward_joint(feature, alphas)
+                elif self.mode == 'dynamic':
+                    feature = cell.forward_dynamic(feature, self.dynamic_cell)
+                else:
+                    raise ValueError('invalid mode={:}'.format(self.mode))
+            else:
+                feature = cell(feature)
+
+        out = self.lastact(feature)
+        out = self.global_pooling(out)
+        out = out.view(out.size(0), -1)
+        logits = self.classifier(out)
+
+        return out, logits
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/clone_weights.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/clone_weights.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-import torch
-import torch.nn as nn
-
-
-def copy_conv(module, init):
-    assert isinstance(module, nn.Conv2d), 'invalid module : {:}'.format(module)
-    assert isinstance(init, nn.Conv2d), 'invalid module : {:}'.format(init)
-    new_i, new_o = module.in_channels, module.out_channels
-    module.weight.copy_(init.weight.detach()[:new_o, :new_i])
-    if module.bias is not None:
-        module.bias.copy_(init.bias.detach()[:new_o])
-
-
-def copy_bn(module, init):
-    assert isinstance(module, nn.BatchNorm2d), 'invalid module : {:}'.format(module)
-    assert isinstance(init, nn.BatchNorm2d), 'invalid module : {:}'.format(init)
-    num_features = module.num_features
-    if module.weight is not None:
-        module.weight.copy_(init.weight.detach()[:num_features])
-    if module.bias is not None:
-        module.bias.copy_(init.bias.detach()[:num_features])
-    if module.running_mean is not None:
-        module.running_mean.copy_(init.running_mean.detach()[:num_features])
-    if module.running_var is not None:
-        module.running_var.copy_(init.running_var.detach()[:num_features])
-
-
-def copy_fc(module, init):
-    assert isinstance(module, nn.Linear), 'invalid module : {:}'.format(module)
-    assert isinstance(init, nn.Linear), 'invalid module : {:}'.format(init)
-    new_i, new_o = module.in_features, module.out_features
-    module.weight.copy_(init.weight.detach()[:new_o, :new_i])
-    if module.bias is not None:
-        module.bias.copy_(init.bias.detach()[:new_o])
-
-
-def copy_base(module, init):
-    assert type(module).__name__ in ['ConvBNReLU', 'Downsample'], 'invalid module : {:}'.format(module)
-    assert type(init).__name__ in ['ConvBNReLU', 'Downsample'], 'invalid module : {:}'.format(init)
-    if module.conv is not None:
-        copy_conv(module.conv, init.conv)
-    if module.bn is not None:
-        copy_bn(module.bn, init.bn)
-
-
-def copy_basic(module, init):
-    copy_base(module.conv_a, init.conv_a)
-    copy_base(module.conv_b, init.conv_b)
-    if module.downsample is not None:
-        if init.downsample is not None:
-            copy_base(module.downsample, init.downsample)
-        # else:
-        # import pdb; pdb.set_trace()
-
-
-def init_from_model(network, init_model):
-    with torch.no_grad():
-        copy_fc(network.classifier, init_model.classifier)
-        for base, target in zip(init_model.layers, network.layers):
-            assert type(base).__name__ == type(target).__name__, 'invalid type : {:} vs {:}'.format(base, target)
-            if type(base).__name__ == 'ConvBNReLU':
-                copy_base(target, base)
-            elif type(base).__name__ == 'ResNetBasicblock':
-                copy_basic(target, base)
-            else:
-                raise ValueError('unknown type name : {:}'.format(type(base).__name__))
+import torch
+import torch.nn as nn
+
+
+def copy_conv(module, init):
+    assert isinstance(module, nn.Conv2d), 'invalid module : {:}'.format(module)
+    assert isinstance(init, nn.Conv2d), 'invalid module : {:}'.format(init)
+    new_i, new_o = module.in_channels, module.out_channels
+    module.weight.copy_(init.weight.detach()[:new_o, :new_i])
+    if module.bias is not None:
+        module.bias.copy_(init.bias.detach()[:new_o])
+
+
+def copy_bn(module, init):
+    assert isinstance(module, nn.BatchNorm2d), 'invalid module : {:}'.format(module)
+    assert isinstance(init, nn.BatchNorm2d), 'invalid module : {:}'.format(init)
+    num_features = module.num_features
+    if module.weight is not None:
+        module.weight.copy_(init.weight.detach()[:num_features])
+    if module.bias is not None:
+        module.bias.copy_(init.bias.detach()[:num_features])
+    if module.running_mean is not None:
+        module.running_mean.copy_(init.running_mean.detach()[:num_features])
+    if module.running_var is not None:
+        module.running_var.copy_(init.running_var.detach()[:num_features])
+
+
+def copy_fc(module, init):
+    assert isinstance(module, nn.Linear), 'invalid module : {:}'.format(module)
+    assert isinstance(init, nn.Linear), 'invalid module : {:}'.format(init)
+    new_i, new_o = module.in_features, module.out_features
+    module.weight.copy_(init.weight.detach()[:new_o, :new_i])
+    if module.bias is not None:
+        module.bias.copy_(init.bias.detach()[:new_o])
+
+
+def copy_base(module, init):
+    assert type(module).__name__ in ['ConvBNReLU', 'Downsample'], 'invalid module : {:}'.format(module)
+    assert type(init).__name__ in ['ConvBNReLU', 'Downsample'], 'invalid module : {:}'.format(init)
+    if module.conv is not None:
+        copy_conv(module.conv, init.conv)
+    if module.bn is not None:
+        copy_bn(module.bn, init.bn)
+
+
+def copy_basic(module, init):
+    copy_base(module.conv_a, init.conv_a)
+    copy_base(module.conv_b, init.conv_b)
+    if module.downsample is not None:
+        if init.downsample is not None:
+            copy_base(module.downsample, init.downsample)
+        # else:
+        # import pdb; pdb.set_trace()
+
+
+def init_from_model(network, init_model):
+    with torch.no_grad():
+        copy_fc(network.classifier, init_model.classifier)
+        for base, target in zip(init_model.layers, network.layers):
+            assert type(base).__name__ == type(target).__name__, 'invalid type : {:} vs {:}'.format(base, target)
+            if type(base).__name__ == 'ConvBNReLU':
+                copy_base(target, base)
+            elif type(base).__name__ == 'ResNetBasicblock':
+                copy_basic(target, base)
+            else:
+                raise ValueError('unknown type name : {:}'.format(type(base).__name__))
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/__init__.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/__init__.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-##################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
-##################################################
-from .configure_utils import load_config, dict2config, configure2str
-from .basic_args import obtain_basic_args
-from .attention_args import obtain_attention_args
-from .random_baseline import obtain_RandomSearch_args
-from .cls_kd_args import obtain_cls_kd_args
-from .cls_init_args import obtain_cls_init_args
-from .search_single_args import obtain_search_single_args
-from .search_args import obtain_search_args
-# for network pruning
-from .pruning_args import obtain_pruning_args
+##################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
+##################################################
+from .configure_utils import load_config, dict2config, configure2str
+from .basic_args import obtain_basic_args
+from .attention_args import obtain_attention_args
+from .random_baseline import obtain_RandomSearch_args
+from .cls_kd_args import obtain_cls_kd_args
+from .cls_init_args import obtain_cls_init_args
+from .search_single_args import obtain_search_single_args
+from .search_args import obtain_search_args
+# for network pruning
+from .pruning_args import obtain_pruning_args
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/attention_args.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/cls_init_args.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-import random, argparse
-from .share_args import add_shared_args
-
-
-def obtain_attention_args():
-    parser = argparse.ArgumentParser(
-        description='Train a classification model on typical image classification datasets.',
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument('--resume', type=str, help='Resume path.')
-    parser.add_argument('--init_model', type=str, help='The initialization model path.')
-    parser.add_argument('--model_config', type=str, help='The path to the model configuration')
-    parser.add_argument('--optim_config', type=str, help='The path to the optimizer configuration')
-    parser.add_argument('--procedure', type=str, help='The procedure basic prefix.')
-    parser.add_argument('--att_channel', type=int, help='.')
-    parser.add_argument('--att_spatial', type=str, help='.')
-    parser.add_argument('--att_active', type=str, help='.')
-    add_shared_args(parser)
-    # Optimization options
-    parser.add_argument('--batch_size', type=int, default=2, help='Batch size for training.')
-    args = parser.parse_args()
-
-    if args.rand_seed is None or args.rand_seed < 0:
-        args.rand_seed = random.randint(1, 100000)
-    assert args.save_dir is not None, 'save-path argument can not be None'
-    return args
+import random, argparse
+from .share_args import add_shared_args
+
+
+def obtain_cls_init_args():
+    parser = argparse.ArgumentParser(
+        description='Train a classification model on typical image classification datasets.',
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser.add_argument('--resume', type=str, help='Resume path.')
+    parser.add_argument('--init_model', type=str, help='The initialization model path.')
+    parser.add_argument('--model_config', type=str, help='The path to the model configuration')
+    parser.add_argument('--optim_config', type=str, help='The path to the optimizer configuration')
+    parser.add_argument('--procedure', type=str, help='The procedure basic prefix.')
+    parser.add_argument('--init_checkpoint', type=str, help='The checkpoint path to the initial model.')
+    add_shared_args(parser)
+    # Optimization options
+    parser.add_argument('--batch_size', type=int, default=2, help='Batch size for training.')
+    args = parser.parse_args()
+
+    if args.rand_seed is None or args.rand_seed < 0:
+        args.rand_seed = random.randint(1, 100000)
+    assert args.save_dir is not None, 'save-path argument can not be None'
+    return args
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/basic_args.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/basic_args.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-##################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2020 #
-##################################################
-import random, argparse
-from .share_args import add_shared_args
-
-
-def obtain_basic_args():
-    parser = argparse.ArgumentParser(
-        description='Train a classification model on typical image classification datasets.',
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument('--resume', type=str, help='Resume path.')
-    parser.add_argument('--init_model', type=str, help='The initialization model path.')
-    parser.add_argument('--model_config', type=str, help='The path to the model configuration')
-    parser.add_argument('--optim_config', type=str, help='The path to the optimizer configuration')
-    parser.add_argument('--procedure', type=str, help='The procedure basic prefix.')
-    parser.add_argument('--model_source', type=str, default='normal', help='The source of model defination.')
-    parser.add_argument('--extra_model_path', type=str, default=None,
-                        help='The extra model ckp file (help to indicate the searched architecture).')
-    add_shared_args(parser)
-    # Optimization options
-    parser.add_argument('--batch_size', type=int, default=2, help='Batch size for training.')
-    args = parser.parse_args()
-
-    if args.rand_seed is None or args.rand_seed < 0:
-        args.rand_seed = random.randint(1, 100000)
-    assert args.save_dir is not None, 'save-path argument can not be None'
-    return args
+##################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2020 #
+##################################################
+import random, argparse
+from .share_args import add_shared_args
+
+
+def obtain_basic_args():
+    parser = argparse.ArgumentParser(
+        description='Train a classification model on typical image classification datasets.',
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser.add_argument('--resume', type=str, help='Resume path.')
+    parser.add_argument('--init_model', type=str, help='The initialization model path.')
+    parser.add_argument('--model_config', type=str, help='The path to the model configuration')
+    parser.add_argument('--optim_config', type=str, help='The path to the optimizer configuration')
+    parser.add_argument('--procedure', type=str, help='The procedure basic prefix.')
+    parser.add_argument('--model_source', type=str, default='normal', help='The source of model defination.')
+    parser.add_argument('--extra_model_path', type=str, default=None,
+                        help='The extra model ckp file (help to indicate the searched architecture).')
+    add_shared_args(parser)
+    # Optimization options
+    parser.add_argument('--batch_size', type=int, default=2, help='Batch size for training.')
+    args = parser.parse_args()
+
+    if args.rand_seed is None or args.rand_seed < 0:
+        args.rand_seed = random.randint(1, 100000)
+    assert args.save_dir is not None, 'save-path argument can not be None'
+    return args
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/cls_init_args.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/pruning_args.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-import random, argparse
-from .share_args import add_shared_args
-
-
-def obtain_cls_init_args():
-    parser = argparse.ArgumentParser(
-        description='Train a classification model on typical image classification datasets.',
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument('--resume', type=str, help='Resume path.')
-    parser.add_argument('--init_model', type=str, help='The initialization model path.')
-    parser.add_argument('--model_config', type=str, help='The path to the model configuration')
-    parser.add_argument('--optim_config', type=str, help='The path to the optimizer configuration')
-    parser.add_argument('--procedure', type=str, help='The procedure basic prefix.')
-    parser.add_argument('--init_checkpoint', type=str, help='The checkpoint path to the initial model.')
-    add_shared_args(parser)
-    # Optimization options
-    parser.add_argument('--batch_size', type=int, default=2, help='Batch size for training.')
-    args = parser.parse_args()
-
-    if args.rand_seed is None or args.rand_seed < 0:
-        args.rand_seed = random.randint(1, 100000)
-    assert args.save_dir is not None, 'save-path argument can not be None'
-    return args
+import os, sys, time, random, argparse
+from .share_args import add_shared_args
+
+
+def obtain_pruning_args():
+    parser = argparse.ArgumentParser(
+        description='Train a classification model on typical image classification datasets.',
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser.add_argument('--resume', type=str, help='Resume path.')
+    parser.add_argument('--init_model', type=str, help='The initialization model path.')
+    parser.add_argument('--model_config', type=str, help='The path to the model configuration')
+    parser.add_argument('--optim_config', type=str, help='The path to the optimizer configuration')
+    parser.add_argument('--procedure', type=str, help='The procedure basic prefix.')
+    parser.add_argument('--keep_ratio', type=float, help='The left channel ratio compared to the original network.')
+    parser.add_argument('--model_version', type=str, help='The network version.')
+    parser.add_argument('--KD_alpha', type=float, help='The alpha parameter in knowledge distillation.')
+    parser.add_argument('--KD_temperature', type=float, help='The temperature parameter in knowledge distillation.')
+    parser.add_argument('--Regular_W_feat', type=float, help='The .')
+    parser.add_argument('--Regular_W_conv', type=float, help='The .')
+    add_shared_args(parser)
+    # Optimization options
+    parser.add_argument('--batch_size', type=int, default=2, help='Batch size for training.')
+    args = parser.parse_args()
+
+    if args.rand_seed is None or args.rand_seed < 0:
+        args.rand_seed = random.randint(1, 100000)
+    assert args.save_dir is not None, 'save-path argument can not be None'
+    assert args.keep_ratio > 0 and args.keep_ratio <= 1, 'invalid keep ratio : {:}'.format(args.keep_ratio)
+    return args
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/cls_kd_args.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/cls_kd_args.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import random, argparse
-from .share_args import add_shared_args
-
-
-def obtain_cls_kd_args():
-    parser = argparse.ArgumentParser(
-        description='Train a classification model on typical image classification datasets.',
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument('--resume', type=str, help='Resume path.')
-    parser.add_argument('--init_model', type=str, help='The initialization model path.')
-    parser.add_argument('--model_config', type=str, help='The path to the model configuration')
-    parser.add_argument('--optim_config', type=str, help='The path to the optimizer configuration')
-    parser.add_argument('--procedure', type=str, help='The procedure basic prefix.')
-    parser.add_argument('--KD_checkpoint', type=str, help='The teacher checkpoint in knowledge distillation.')
-    parser.add_argument('--KD_alpha', type=float, help='The alpha parameter in knowledge distillation.')
-    parser.add_argument('--KD_temperature', type=float, help='The temperature parameter in knowledge distillation.')
-    # parser.add_argument('--KD_feature',       type=float,                 help='Knowledge distillation at the feature level.')
-    add_shared_args(parser)
-    # Optimization options
-    parser.add_argument('--batch_size', type=int, default=2, help='Batch size for training.')
-    args = parser.parse_args()
-
-    if args.rand_seed is None or args.rand_seed < 0:
-        args.rand_seed = random.randint(1, 100000)
-    assert args.save_dir is not None, 'save-path argument can not be None'
-    return args
+import random, argparse
+from .share_args import add_shared_args
+
+
+def obtain_cls_kd_args():
+    parser = argparse.ArgumentParser(
+        description='Train a classification model on typical image classification datasets.',
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser.add_argument('--resume', type=str, help='Resume path.')
+    parser.add_argument('--init_model', type=str, help='The initialization model path.')
+    parser.add_argument('--model_config', type=str, help='The path to the model configuration')
+    parser.add_argument('--optim_config', type=str, help='The path to the optimizer configuration')
+    parser.add_argument('--procedure', type=str, help='The procedure basic prefix.')
+    parser.add_argument('--KD_checkpoint', type=str, help='The teacher checkpoint in knowledge distillation.')
+    parser.add_argument('--KD_alpha', type=float, help='The alpha parameter in knowledge distillation.')
+    parser.add_argument('--KD_temperature', type=float, help='The temperature parameter in knowledge distillation.')
+    # parser.add_argument('--KD_feature',       type=float,                 help='Knowledge distillation at the feature level.')
+    add_shared_args(parser)
+    # Optimization options
+    parser.add_argument('--batch_size', type=int, default=2, help='Batch size for training.')
+    args = parser.parse_args()
+
+    if args.rand_seed is None or args.rand_seed < 0:
+        args.rand_seed = random.randint(1, 100000)
+    assert args.save_dir is not None, 'save-path argument can not be None'
+    return args
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/pruning_args.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/search_single_args.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,34 @@
-import os, sys, time, random, argparse
-from .share_args import add_shared_args
-
-
-def obtain_pruning_args():
-    parser = argparse.ArgumentParser(
-        description='Train a classification model on typical image classification datasets.',
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument('--resume', type=str, help='Resume path.')
-    parser.add_argument('--init_model', type=str, help='The initialization model path.')
-    parser.add_argument('--model_config', type=str, help='The path to the model configuration')
-    parser.add_argument('--optim_config', type=str, help='The path to the optimizer configuration')
-    parser.add_argument('--procedure', type=str, help='The procedure basic prefix.')
-    parser.add_argument('--keep_ratio', type=float, help='The left channel ratio compared to the original network.')
-    parser.add_argument('--model_version', type=str, help='The network version.')
-    parser.add_argument('--KD_alpha', type=float, help='The alpha parameter in knowledge distillation.')
-    parser.add_argument('--KD_temperature', type=float, help='The temperature parameter in knowledge distillation.')
-    parser.add_argument('--Regular_W_feat', type=float, help='The .')
-    parser.add_argument('--Regular_W_conv', type=float, help='The .')
-    add_shared_args(parser)
-    # Optimization options
-    parser.add_argument('--batch_size', type=int, default=2, help='Batch size for training.')
-    args = parser.parse_args()
-
-    if args.rand_seed is None or args.rand_seed < 0:
-        args.rand_seed = random.randint(1, 100000)
-    assert args.save_dir is not None, 'save-path argument can not be None'
-    assert args.keep_ratio > 0 and args.keep_ratio <= 1, 'invalid keep ratio : {:}'.format(args.keep_ratio)
-    return args
+import os, sys, time, random, argparse
+from .share_args import add_shared_args
+
+
+def obtain_search_single_args():
+    parser = argparse.ArgumentParser(
+        description='Train a classification model on typical image classification datasets.',
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser.add_argument('--resume', type=str, help='Resume path.')
+    parser.add_argument('--model_config', type=str, help='The path to the model configuration')
+    parser.add_argument('--optim_config', type=str, help='The path to the optimizer configuration')
+    parser.add_argument('--split_path', type=str, help='The split file path.')
+    parser.add_argument('--search_shape', type=str, help='The shape to be searched.')
+    # parser.add_argument('--arch_para_pure',   type=int,                   help='The architecture-parameter pure or not.')
+    parser.add_argument('--gumbel_tau_max', type=float, help='The maximum tau for Gumbel.')
+    parser.add_argument('--gumbel_tau_min', type=float, help='The minimum tau for Gumbel.')
+    parser.add_argument('--procedure', type=str, help='The procedure basic prefix.')
+    parser.add_argument('--FLOP_ratio', type=float, help='The expected FLOP ratio.')
+    parser.add_argument('--FLOP_weight', type=float, help='The loss weight for FLOP.')
+    parser.add_argument('--FLOP_tolerant', type=float, help='The tolerant range for FLOP.')
+    add_shared_args(parser)
+    # Optimization options
+    parser.add_argument('--batch_size', type=int, default=2, help='Batch size for training.')
+    args = parser.parse_args()
+
+    if args.rand_seed is None or args.rand_seed < 0:
+        args.rand_seed = random.randint(1, 100000)
+    assert args.save_dir is not None, 'save-path argument can not be None'
+    assert args.gumbel_tau_max is not None and args.gumbel_tau_min is not None
+    assert args.FLOP_tolerant is not None and args.FLOP_tolerant > 0, 'invalid FLOP_tolerant : {:}'.format(
+        FLOP_tolerant)
+    # assert args.arch_para_pure is not None, 'arch_para_pure is not None: {:}'.format(args.arch_para_pure)
+    # args.arch_para_pure = bool(args.arch_para_pure)
+    return args
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/random_baseline.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/random_baseline.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import os, sys, time, random, argparse
-from .share_args import add_shared_args
-
-
-def obtain_RandomSearch_args():
-    parser = argparse.ArgumentParser(
-        description='Train a classification model on typical image classification datasets.',
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument('--resume', type=str, help='Resume path.')
-    parser.add_argument('--init_model', type=str, help='The initialization model path.')
-    parser.add_argument('--expect_flop', type=float, help='The expected flop keep ratio.')
-    parser.add_argument('--arch_nums', type=int, help='The maximum number of running random arch generating..')
-    parser.add_argument('--model_config', type=str, help='The path to the model configuration')
-    parser.add_argument('--optim_config', type=str, help='The path to the optimizer configuration')
-    parser.add_argument('--random_mode', type=str, choices=['random', 'fix'],
-                        help='The path to the optimizer configuration')
-    parser.add_argument('--procedure', type=str, help='The procedure basic prefix.')
-    add_shared_args(parser)
-    # Optimization options
-    parser.add_argument('--batch_size', type=int, default=2, help='Batch size for training.')
-    args = parser.parse_args()
-
-    if args.rand_seed is None or args.rand_seed < 0:
-        args.rand_seed = random.randint(1, 100000)
-    assert args.save_dir is not None, 'save-path argument can not be None'
-    # assert args.flop_ratio_min < args.flop_ratio_max, 'flop-ratio {:} vs {:}'.format(args.flop_ratio_min, args.flop_ratio_max)
-    return args
+import os, sys, time, random, argparse
+from .share_args import add_shared_args
+
+
+def obtain_RandomSearch_args():
+    parser = argparse.ArgumentParser(
+        description='Train a classification model on typical image classification datasets.',
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser.add_argument('--resume', type=str, help='Resume path.')
+    parser.add_argument('--init_model', type=str, help='The initialization model path.')
+    parser.add_argument('--expect_flop', type=float, help='The expected flop keep ratio.')
+    parser.add_argument('--arch_nums', type=int, help='The maximum number of running random arch generating..')
+    parser.add_argument('--model_config', type=str, help='The path to the model configuration')
+    parser.add_argument('--optim_config', type=str, help='The path to the optimizer configuration')
+    parser.add_argument('--random_mode', type=str, choices=['random', 'fix'],
+                        help='The path to the optimizer configuration')
+    parser.add_argument('--procedure', type=str, help='The procedure basic prefix.')
+    add_shared_args(parser)
+    # Optimization options
+    parser.add_argument('--batch_size', type=int, default=2, help='Batch size for training.')
+    args = parser.parse_args()
+
+    if args.rand_seed is None or args.rand_seed < 0:
+        args.rand_seed = random.randint(1, 100000)
+    assert args.save_dir is not None, 'save-path argument can not be None'
+    # assert args.flop_ratio_min < args.flop_ratio_max, 'flop-ratio {:} vs {:}'.format(args.flop_ratio_min, args.flop_ratio_max)
+    return args
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/search_args.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/search_args.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import os, sys, time, random, argparse
-from .share_args import add_shared_args
-
-
-def obtain_search_args():
-    parser = argparse.ArgumentParser(
-        description='Train a classification model on typical image classification datasets.',
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument('--resume', type=str, help='Resume path.')
-    parser.add_argument('--model_config', type=str, help='The path to the model configuration')
-    parser.add_argument('--optim_config', type=str, help='The path to the optimizer configuration')
-    parser.add_argument('--split_path', type=str, help='The split file path.')
-    # parser.add_argument('--arch_para_pure',   type=int,                   help='The architecture-parameter pure or not.')
-    parser.add_argument('--gumbel_tau_max', type=float, help='The maximum tau for Gumbel.')
-    parser.add_argument('--gumbel_tau_min', type=float, help='The minimum tau for Gumbel.')
-    parser.add_argument('--procedure', type=str, help='The procedure basic prefix.')
-    parser.add_argument('--FLOP_ratio', type=float, help='The expected FLOP ratio.')
-    parser.add_argument('--FLOP_weight', type=float, help='The loss weight for FLOP.')
-    parser.add_argument('--FLOP_tolerant', type=float, help='The tolerant range for FLOP.')
-    # ablation studies
-    parser.add_argument('--ablation_num_select', type=int, help='The number of randomly selected channels.')
-    add_shared_args(parser)
-    # Optimization options
-    parser.add_argument('--batch_size', type=int, default=2, help='Batch size for training.')
-    args = parser.parse_args()
-
-    if args.rand_seed is None or args.rand_seed < 0:
-        args.rand_seed = random.randint(1, 100000)
-    assert args.save_dir is not None, 'save-path argument can not be None'
-    assert args.gumbel_tau_max is not None and args.gumbel_tau_min is not None
-    assert args.FLOP_tolerant is not None and args.FLOP_tolerant > 0, 'invalid FLOP_tolerant : {:}'.format(
-        FLOP_tolerant)
-    # assert args.arch_para_pure is not None, 'arch_para_pure is not None: {:}'.format(args.arch_para_pure)
-    # args.arch_para_pure = bool(args.arch_para_pure)
-    return args
+import os, sys, time, random, argparse
+from .share_args import add_shared_args
+
+
+def obtain_search_args():
+    parser = argparse.ArgumentParser(
+        description='Train a classification model on typical image classification datasets.',
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser.add_argument('--resume', type=str, help='Resume path.')
+    parser.add_argument('--model_config', type=str, help='The path to the model configuration')
+    parser.add_argument('--optim_config', type=str, help='The path to the optimizer configuration')
+    parser.add_argument('--split_path', type=str, help='The split file path.')
+    # parser.add_argument('--arch_para_pure',   type=int,                   help='The architecture-parameter pure or not.')
+    parser.add_argument('--gumbel_tau_max', type=float, help='The maximum tau for Gumbel.')
+    parser.add_argument('--gumbel_tau_min', type=float, help='The minimum tau for Gumbel.')
+    parser.add_argument('--procedure', type=str, help='The procedure basic prefix.')
+    parser.add_argument('--FLOP_ratio', type=float, help='The expected FLOP ratio.')
+    parser.add_argument('--FLOP_weight', type=float, help='The loss weight for FLOP.')
+    parser.add_argument('--FLOP_tolerant', type=float, help='The tolerant range for FLOP.')
+    # ablation studies
+    parser.add_argument('--ablation_num_select', type=int, help='The number of randomly selected channels.')
+    add_shared_args(parser)
+    # Optimization options
+    parser.add_argument('--batch_size', type=int, default=2, help='Batch size for training.')
+    args = parser.parse_args()
+
+    if args.rand_seed is None or args.rand_seed < 0:
+        args.rand_seed = random.randint(1, 100000)
+    assert args.save_dir is not None, 'save-path argument can not be None'
+    assert args.gumbel_tau_max is not None and args.gumbel_tau_min is not None
+    assert args.FLOP_tolerant is not None and args.FLOP_tolerant > 0, 'invalid FLOP_tolerant : {:}'.format(
+        FLOP_tolerant)
+    # assert args.arch_para_pure is not None, 'arch_para_pure is not None: {:}'.format(args.arch_para_pure)
+    # args.arch_para_pure = bool(args.arch_para_pure)
+    return args
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/share_args.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/config_utils/share_args.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import os, sys, time, random, argparse
-
-
-def add_shared_args(parser):
-    # Data Generation
-    parser.add_argument('--dataset', type=str, help='The dataset name.')
-    parser.add_argument('--data_path', type=str, help='The dataset name.')
-    parser.add_argument('--cutout_length', type=int, help='The cutout length, negative means not use.')
-    # Printing
-    parser.add_argument('--print_freq', type=int, default=100, help='print frequency (default: 200)')
-    parser.add_argument('--print_freq_eval', type=int, default=100, help='print frequency (default: 200)')
-    # Checkpoints
-    parser.add_argument('--eval_frequency', type=int, default=1, help='evaluation frequency (default: 200)')
-    parser.add_argument('--save_dir', type=str, help='Folder to save checkpoints and log.')
-    # Acceleration
-    parser.add_argument('--workers', type=int, default=8, help='number of data loading workers (default: 8)')
-    # Random Seed
-    parser.add_argument('--rand_seed', type=int, default=-1, help='manual seed')
+import os, sys, time, random, argparse
+
+
+def add_shared_args(parser):
+    # Data Generation
+    parser.add_argument('--dataset', type=str, help='The dataset name.')
+    parser.add_argument('--data_path', type=str, help='The dataset name.')
+    parser.add_argument('--cutout_length', type=int, help='The cutout length, negative means not use.')
+    # Printing
+    parser.add_argument('--print_freq', type=int, default=100, help='print frequency (default: 200)')
+    parser.add_argument('--print_freq_eval', type=int, default=100, help='print frequency (default: 200)')
+    # Checkpoints
+    parser.add_argument('--eval_frequency', type=int, default=1, help='evaluation frequency (default: 200)')
+    parser.add_argument('--save_dir', type=str, help='Folder to save checkpoints and log.')
+    # Acceleration
+    parser.add_argument('--workers', type=int, default=8, help='number of data loading workers (default: 8)')
+    # Random Seed
+    parser.add_argument('--rand_seed', type=int, default=-1, help='manual seed')
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/initialization.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/initialization.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import torch
-import torch.nn as nn
-
-
-def initialize_resnet(m):
-    if isinstance(m, nn.Conv2d):
-        nn.init.kaiming_normal_(m.weight, mode='fan_out', nonlinearity='relu')
-        if m.bias is not None:
-            nn.init.constant_(m.bias, 0)
-    elif isinstance(m, nn.BatchNorm2d):
-        nn.init.constant_(m.weight, 1)
-        if m.bias is not None:
-            nn.init.constant_(m.bias, 0)
-    elif isinstance(m, nn.Linear):
-        nn.init.normal_(m.weight, 0, 0.01)
-        nn.init.constant_(m.bias, 0)
+import torch
+import torch.nn as nn
+
+
+def initialize_resnet(m):
+    if isinstance(m, nn.Conv2d):
+        nn.init.kaiming_normal_(m.weight, mode='fan_out', nonlinearity='relu')
+        if m.bias is not None:
+            nn.init.constant_(m.bias, 0)
+    elif isinstance(m, nn.BatchNorm2d):
+        nn.init.constant_(m.weight, 1)
+        if m.bias is not None:
+            nn.init.constant_(m.bias, 0)
+    elif isinstance(m, nn.Linear):
+        nn.init.normal_(m.weight, 0, 0.01)
+        nn.init.constant_(m.bias, 0)
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/InferMobileNetV2.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/InferMobileNetV2.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-#####################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019.01 #
-#####################################################
-# MobileNetV2: Inverted Residuals and Linear Bottlenecks, CVPR 2018
-from torch import nn
-from ..initialization import initialize_resnet
-from ..SharedUtils import parse_channel_info
-
-
-class ConvBNReLU(nn.Module):
-    def __init__(self, in_planes, out_planes, kernel_size, stride, groups, has_bn=True, has_relu=True):
-        super(ConvBNReLU, self).__init__()
-        padding = (kernel_size - 1) // 2
-        self.conv = nn.Conv2d(in_planes, out_planes, kernel_size, stride, padding, groups=groups, bias=False)
-        if has_bn:
-            self.bn = nn.BatchNorm2d(out_planes)
-        else:
-            self.bn = None
-        if has_relu:
-            self.relu = nn.ReLU6(inplace=True)
-        else:
-            self.relu = None
-
-    def forward(self, x):
-        out = self.conv(x)
-        if self.bn:   out = self.bn(out)
-        if self.relu: out = self.relu(out)
-        return out
-
-
-class InvertedResidual(nn.Module):
-    def __init__(self, channels, stride, expand_ratio, additive):
-        super(InvertedResidual, self).__init__()
-        self.stride = stride
-        assert stride in [1, 2], 'invalid stride : {:}'.format(stride)
-        assert len(channels) in [2, 3], 'invalid channels : {:}'.format(channels)
-
-        if len(channels) == 2:
-            layers = []
-        else:
-            layers = [ConvBNReLU(channels[0], channels[1], 1, 1, 1)]
-        layers.extend([
-            # dw
-            ConvBNReLU(channels[-2], channels[-2], 3, stride, channels[-2]),
-            # pw-linear
-            ConvBNReLU(channels[-2], channels[-1], 1, 1, 1, True, False),
-        ])
-        self.conv = nn.Sequential(*layers)
-        self.additive = additive
-        if self.additive and channels[0] != channels[-1]:
-            self.shortcut = ConvBNReLU(channels[0], channels[-1], 1, 1, 1, True, False)
-        else:
-            self.shortcut = None
-        self.out_dim = channels[-1]
-
-    def forward(self, x):
-        out = self.conv(x)
-        # if self.additive: return additive_func(out, x)
-        if self.shortcut:
-            return out + self.shortcut(x)
-        else:
-            return out
-
-
-class InferMobileNetV2(nn.Module):
-    def __init__(self, num_classes, xchannels, xblocks, dropout):
-        super(InferMobileNetV2, self).__init__()
-        block = InvertedResidual
-        inverted_residual_setting = [
-            # t, c,  n, s
-            [1, 16, 1, 1],
-            [6, 24, 2, 2],
-            [6, 32, 3, 2],
-            [6, 64, 4, 2],
-            [6, 96, 3, 1],
-            [6, 160, 3, 2],
-            [6, 320, 1, 1],
-        ]
-        assert len(inverted_residual_setting) == len(xblocks), 'invalid number of layers : {:} vs {:}'.format(
-            len(inverted_residual_setting), len(xblocks))
-        for block_num, ir_setting in zip(xblocks, inverted_residual_setting):
-            assert block_num <= ir_setting[2], '{:} vs {:}'.format(block_num, ir_setting)
-        xchannels = parse_channel_info(xchannels)
-        # for i, chs in enumerate(xchannels):
-        #  if i > 0: assert chs[0] == xchannels[i-1][-1], 'Layer[{:}] is invalid {:} vs {:}'.format(i, xchannels[i-1], chs)
-        self.xchannels = xchannels
-        self.message = 'InferMobileNetV2 : xblocks={:}'.format(xblocks)
-        # building first layer
-        features = [ConvBNReLU(xchannels[0][0], xchannels[0][1], 3, 2, 1)]
-        last_channel_idx = 1
-
-        # building inverted residual blocks
-        for stage, (t, c, n, s) in enumerate(inverted_residual_setting):
-            for i in range(n):
-                stride = s if i == 0 else 1
-                additv = True if i > 0 else False
-                module = block(self.xchannels[last_channel_idx], stride, t, additv)
-                features.append(module)
-                self.message += "\nstage={:}, ilayer={:02d}/{:02d}, block={:03d}, Cs={:}, stride={:}, expand={:}, original-C={:}".format(
-                    stage, i, n, len(features), self.xchannels[last_channel_idx], stride, t, c)
-                last_channel_idx += 1
-                if i + 1 == xblocks[stage]:
-                    out_channel = module.out_dim
-                    for iiL in range(i + 1, n):
-                        last_channel_idx += 1
-                    self.xchannels[last_channel_idx][0] = module.out_dim
-                    break
-        # building last several layers
-        features.append(ConvBNReLU(self.xchannels[last_channel_idx][0], self.xchannels[last_channel_idx][1], 1, 1, 1))
-        assert last_channel_idx + 2 == len(self.xchannels), '{:} vs {:}'.format(last_channel_idx, len(self.xchannels))
-        # make it nn.Sequential
-        self.features = nn.Sequential(*features)
-
-        # building classifier
-        self.classifier = nn.Sequential(
-            nn.Dropout(dropout),
-            nn.Linear(self.xchannels[last_channel_idx][1], num_classes),
-        )
-
-        # weight initialization
-        self.apply(initialize_resnet)
-
-    def get_message(self):
-        return self.message
-
-    def forward(self, inputs):
-        features = self.features(inputs)
-        vectors = features.mean([2, 3])
-        predicts = self.classifier(vectors)
-        return features, predicts
+#####################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019.01 #
+#####################################################
+# MobileNetV2: Inverted Residuals and Linear Bottlenecks, CVPR 2018
+from torch import nn
+from ..initialization import initialize_resnet
+from ..SharedUtils import parse_channel_info
+
+
+class ConvBNReLU(nn.Module):
+    def __init__(self, in_planes, out_planes, kernel_size, stride, groups, has_bn=True, has_relu=True):
+        super(ConvBNReLU, self).__init__()
+        padding = (kernel_size - 1) // 2
+        self.conv = nn.Conv2d(in_planes, out_planes, kernel_size, stride, padding, groups=groups, bias=False)
+        if has_bn:
+            self.bn = nn.BatchNorm2d(out_planes)
+        else:
+            self.bn = None
+        if has_relu:
+            self.relu = nn.ReLU6(inplace=True)
+        else:
+            self.relu = None
+
+    def forward(self, x):
+        out = self.conv(x)
+        if self.bn:   out = self.bn(out)
+        if self.relu: out = self.relu(out)
+        return out
+
+
+class InvertedResidual(nn.Module):
+    def __init__(self, channels, stride, expand_ratio, additive):
+        super(InvertedResidual, self).__init__()
+        self.stride = stride
+        assert stride in [1, 2], 'invalid stride : {:}'.format(stride)
+        assert len(channels) in [2, 3], 'invalid channels : {:}'.format(channels)
+
+        if len(channels) == 2:
+            layers = []
+        else:
+            layers = [ConvBNReLU(channels[0], channels[1], 1, 1, 1)]
+        layers.extend([
+            # dw
+            ConvBNReLU(channels[-2], channels[-2], 3, stride, channels[-2]),
+            # pw-linear
+            ConvBNReLU(channels[-2], channels[-1], 1, 1, 1, True, False),
+        ])
+        self.conv = nn.Sequential(*layers)
+        self.additive = additive
+        if self.additive and channels[0] != channels[-1]:
+            self.shortcut = ConvBNReLU(channels[0], channels[-1], 1, 1, 1, True, False)
+        else:
+            self.shortcut = None
+        self.out_dim = channels[-1]
+
+    def forward(self, x):
+        out = self.conv(x)
+        # if self.additive: return additive_func(out, x)
+        if self.shortcut:
+            return out + self.shortcut(x)
+        else:
+            return out
+
+
+class InferMobileNetV2(nn.Module):
+    def __init__(self, num_classes, xchannels, xblocks, dropout):
+        super(InferMobileNetV2, self).__init__()
+        block = InvertedResidual
+        inverted_residual_setting = [
+            # t, c,  n, s
+            [1, 16, 1, 1],
+            [6, 24, 2, 2],
+            [6, 32, 3, 2],
+            [6, 64, 4, 2],
+            [6, 96, 3, 1],
+            [6, 160, 3, 2],
+            [6, 320, 1, 1],
+        ]
+        assert len(inverted_residual_setting) == len(xblocks), 'invalid number of layers : {:} vs {:}'.format(
+            len(inverted_residual_setting), len(xblocks))
+        for block_num, ir_setting in zip(xblocks, inverted_residual_setting):
+            assert block_num <= ir_setting[2], '{:} vs {:}'.format(block_num, ir_setting)
+        xchannels = parse_channel_info(xchannels)
+        # for i, chs in enumerate(xchannels):
+        #  if i > 0: assert chs[0] == xchannels[i-1][-1], 'Layer[{:}] is invalid {:} vs {:}'.format(i, xchannels[i-1], chs)
+        self.xchannels = xchannels
+        self.message = 'InferMobileNetV2 : xblocks={:}'.format(xblocks)
+        # building first layer
+        features = [ConvBNReLU(xchannels[0][0], xchannels[0][1], 3, 2, 1)]
+        last_channel_idx = 1
+
+        # building inverted residual blocks
+        for stage, (t, c, n, s) in enumerate(inverted_residual_setting):
+            for i in range(n):
+                stride = s if i == 0 else 1
+                additv = True if i > 0 else False
+                module = block(self.xchannels[last_channel_idx], stride, t, additv)
+                features.append(module)
+                self.message += "\nstage={:}, ilayer={:02d}/{:02d}, block={:03d}, Cs={:}, stride={:}, expand={:}, original-C={:}".format(
+                    stage, i, n, len(features), self.xchannels[last_channel_idx], stride, t, c)
+                last_channel_idx += 1
+                if i + 1 == xblocks[stage]:
+                    out_channel = module.out_dim
+                    for iiL in range(i + 1, n):
+                        last_channel_idx += 1
+                    self.xchannels[last_channel_idx][0] = module.out_dim
+                    break
+        # building last several layers
+        features.append(ConvBNReLU(self.xchannels[last_channel_idx][0], self.xchannels[last_channel_idx][1], 1, 1, 1))
+        assert last_channel_idx + 2 == len(self.xchannels), '{:} vs {:}'.format(last_channel_idx, len(self.xchannels))
+        # make it nn.Sequential
+        self.features = nn.Sequential(*features)
+
+        # building classifier
+        self.classifier = nn.Sequential(
+            nn.Dropout(dropout),
+            nn.Linear(self.xchannels[last_channel_idx][1], num_classes),
+        )
+
+        # weight initialization
+        self.apply(initialize_resnet)
+
+    def get_message(self):
+        return self.message
+
+    def forward(self, inputs):
+        features = self.features(inputs)
+        vectors = features.mean([2, 3])
+        predicts = self.classifier(vectors)
+        return features, predicts
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/InferTinyCellNet.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_infers/InferTinyCellNet.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-#####################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019.01 #
-#####################################################
-from typing import List, Text, Any
-import torch.nn as nn
-from models.cell_operations import ResNetBasicblock
-from models.cell_infers.cells import InferCell
-
-
-class DynamicShapeTinyNet(nn.Module):
-
-    def __init__(self, channels: List[int], genotype: Any, num_classes: int):
-        super(DynamicShapeTinyNet, self).__init__()
-        self._channels = channels
-        if len(channels) % 3 != 2:
-            raise ValueError('invalid number of layers : {:}'.format(len(channels)))
-        self._num_stage = N = len(channels) // 3
-
-        self.stem = nn.Sequential(
-            nn.Conv2d(3, channels[0], kernel_size=3, padding=1, bias=False),
-            nn.BatchNorm2d(channels[0]))
-
-        # layer_channels   = [C    ] * N + [C*2 ] + [C*2  ] * N + [C*4 ] + [C*4  ] * N
-        layer_reductions = [False] * N + [True] + [False] * N + [True] + [False] * N
-
-        c_prev = channels[0]
-        self.cells = nn.ModuleList()
-        for index, (c_curr, reduction) in enumerate(zip(channels, layer_reductions)):
-            if reduction:
-                cell = ResNetBasicblock(c_prev, c_curr, 2, True)
-            else:
-                cell = InferCell(genotype, c_prev, c_curr, 1)
-            self.cells.append(cell)
-            c_prev = cell.out_dim
-        self._num_layer = len(self.cells)
-
-        self.lastact = nn.Sequential(nn.BatchNorm2d(c_prev), nn.ReLU(inplace=True))
-        self.global_pooling = nn.AdaptiveAvgPool2d(1)
-        self.classifier = nn.Linear(c_prev, num_classes)
-
-    def get_message(self) -> Text:
-        string = self.extra_repr()
-        for i, cell in enumerate(self.cells):
-            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
-        return string
-
-    def extra_repr(self):
-        return ('{name}(C={_channels}, N={_num_stage}, L={_num_layer})'.format(name=self.__class__.__name__,
-                                                                               **self.__dict__))
-
-    def forward(self, inputs):
-        feature = self.stem(inputs)
-        for i, cell in enumerate(self.cells):
-            feature = cell(feature)
-
-        out = self.lastact(feature)
-        out = self.global_pooling(out)
-        out = out.view(out.size(0), -1)
-        logits = self.classifier(out)
-
-        return out, logits
+#####################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019.01 #
+#####################################################
+from typing import List, Text, Any
+import torch.nn as nn
+from models.cell_operations import ResNetBasicblock
+from models.cell_infers.cells import InferCell
+
+
+class DynamicShapeTinyNet(nn.Module):
+
+    def __init__(self, channels: List[int], genotype: Any, num_classes: int):
+        super(DynamicShapeTinyNet, self).__init__()
+        self._channels = channels
+        if len(channels) % 3 != 2:
+            raise ValueError('invalid number of layers : {:}'.format(len(channels)))
+        self._num_stage = N = len(channels) // 3
+
+        self.stem = nn.Sequential(
+            nn.Conv2d(3, channels[0], kernel_size=3, padding=1, bias=False),
+            nn.BatchNorm2d(channels[0]))
+
+        # layer_channels   = [C    ] * N + [C*2 ] + [C*2  ] * N + [C*4 ] + [C*4  ] * N
+        layer_reductions = [False] * N + [True] + [False] * N + [True] + [False] * N
+
+        c_prev = channels[0]
+        self.cells = nn.ModuleList()
+        for index, (c_curr, reduction) in enumerate(zip(channels, layer_reductions)):
+            if reduction:
+                cell = ResNetBasicblock(c_prev, c_curr, 2, True)
+            else:
+                cell = InferCell(genotype, c_prev, c_curr, 1)
+            self.cells.append(cell)
+            c_prev = cell.out_dim
+        self._num_layer = len(self.cells)
+
+        self.lastact = nn.Sequential(nn.BatchNorm2d(c_prev), nn.ReLU(inplace=True))
+        self.global_pooling = nn.AdaptiveAvgPool2d(1)
+        self.classifier = nn.Linear(c_prev, num_classes)
+
+    def get_message(self) -> Text:
+        string = self.extra_repr()
+        for i, cell in enumerate(self.cells):
+            string += '\n {:02d}/{:02d} :: {:}'.format(i, len(self.cells), cell.extra_repr())
+        return string
+
+    def extra_repr(self):
+        return ('{name}(C={_channels}, N={_num_stage}, L={_num_layer})'.format(name=self.__class__.__name__,
+                                                                               **self.__dict__))
+
+    def forward(self, inputs):
+        feature = self.stem(inputs)
+        for i, cell in enumerate(self.cells):
+            feature = cell(feature)
+
+        out = self.lastact(feature)
+        out = self.global_pooling(out)
+        out = out.view(out.size(0), -1)
+        logits = self.classifier(out)
+
+        return out, logits
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchCifarResNet.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchImagenetResNet.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,558 +1,538 @@
-##################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
-##################################################
-import math, torch
-from collections import OrderedDict
-from bisect import bisect_right
-import torch.nn as nn
-from ..initialization import initialize_resnet
-from ..SharedUtils import additive_func
-from .SoftSelect import select2withP, ChannelWiseInter
-from .SoftSelect import linear_forward
-from .SoftSelect import get_width_choices
-
-
-def get_depth_choices(nDepth, return_num):
-    if nDepth == 2:
-        choices = (1, 2)
-    elif nDepth == 3:
-        choices = (1, 2, 3)
-    elif nDepth > 3:
-        choices = list(range(1, nDepth + 1, 2))
-        if choices[-1] < nDepth: choices.append(nDepth)
-    else:
-        raise ValueError('invalid nDepth : {:}'.format(nDepth))
-    if return_num:
-        return len(choices)
-    else:
-        return choices
-
-
-def conv_forward(inputs, conv, choices):
-    iC = conv.in_channels
-    fill_size = list(inputs.size())
-    fill_size[1] = iC - fill_size[1]
-    filled = torch.zeros(fill_size, device=inputs.device)
-    xinputs = torch.cat((inputs, filled), dim=1)
-    outputs = conv(xinputs)
-    selecteds = [outputs[:, :oC] for oC in choices]
-    return selecteds
-
-
-class ConvBNReLU(nn.Module):
-    num_conv = 1
-
-    def __init__(self, nIn, nOut, kernel, stride, padding, bias, has_avg, has_bn, has_relu):
-        super(ConvBNReLU, self).__init__()
-        self.InShape = None
-        self.OutShape = None
-        self.choices = get_width_choices(nOut)
-        self.register_buffer('choices_tensor', torch.Tensor(self.choices))
-
-        if has_avg:
-            self.avg = nn.AvgPool2d(kernel_size=2, stride=2, padding=0)
-        else:
-            self.avg = None
-        self.conv = nn.Conv2d(nIn, nOut, kernel_size=kernel, stride=stride, padding=padding, dilation=1, groups=1,
-                              bias=bias)
-        # if has_bn  : self.bn  = nn.BatchNorm2d(nOut)
-        # else       : self.bn  = None
-        self.has_bn = has_bn
-        self.BNs = nn.ModuleList()
-        for i, _out in enumerate(self.choices):
-            self.BNs.append(nn.BatchNorm2d(_out))
-        if has_relu:
-            self.relu = nn.ReLU(inplace=True)
-        else:
-            self.relu = None
-        self.in_dim = nIn
-        self.out_dim = nOut
-        self.search_mode = 'basic'
-
-    def get_flops(self, channels, check_range=True, divide=1):
-        iC, oC = channels
-        if check_range: assert iC <= self.conv.in_channels and oC <= self.conv.out_channels, '{:} vs {:}  |  {:} vs {:}'.format(
-            iC, self.conv.in_channels, oC, self.conv.out_channels)
-        assert isinstance(self.InShape, tuple) and len(self.InShape) == 2, 'invalid in-shape : {:}'.format(self.InShape)
-        assert isinstance(self.OutShape, tuple) and len(self.OutShape) == 2, 'invalid out-shape : {:}'.format(
-            self.OutShape)
-        # conv_per_position_flops = self.conv.kernel_size[0] * self.conv.kernel_size[1] * iC * oC / self.conv.groups
-        conv_per_position_flops = (self.conv.kernel_size[0] * self.conv.kernel_size[1] * 1.0 / self.conv.groups)
-        all_positions = self.OutShape[0] * self.OutShape[1]
-        flops = (conv_per_position_flops * all_positions / divide) * iC * oC
-        if self.conv.bias is not None: flops += all_positions / divide
-        return flops
-
-    def get_range(self):
-        return [self.choices]
-
-    def forward(self, inputs):
-        if self.search_mode == 'basic':
-            return self.basic_forward(inputs)
-        elif self.search_mode == 'search':
-            return self.search_forward(inputs)
-        else:
-            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
-
-    def search_forward(self, tuple_inputs):
-        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
-            type(tuple_inputs))
-        inputs, expected_inC, probability, index, prob = tuple_inputs
-        index, prob = torch.squeeze(index).tolist(), torch.squeeze(prob)
-        probability = torch.squeeze(probability)
-        assert len(index) == 2, 'invalid length : {:}'.format(index)
-        # compute expected flop
-        # coordinates   = torch.arange(self.x_range[0], self.x_range[1]+1).type_as(probability)
-        expected_outC = (self.choices_tensor * probability).sum()
-        expected_flop = self.get_flops([expected_inC, expected_outC], False, 1e6)
-        if self.avg:
-            out = self.avg(inputs)
-        else:
-            out = inputs
-        # convolutional layer
-        out_convs = conv_forward(out, self.conv, [self.choices[i] for i in index])
-        out_bns = [self.BNs[idx](out_conv) for idx, out_conv in zip(index, out_convs)]
-        # merge
-        out_channel = max([x.size(1) for x in out_bns])
-        outA = ChannelWiseInter(out_bns[0], out_channel)
-        outB = ChannelWiseInter(out_bns[1], out_channel)
-        out = outA * prob[0] + outB * prob[1]
-        # out = additive_func(out_bns[0]*prob[0], out_bns[1]*prob[1])
-
-        if self.relu:
-            out = self.relu(out)
-        else:
-            out = out
-        return out, expected_outC, expected_flop
-
-    def basic_forward(self, inputs):
-        if self.avg:
-            out = self.avg(inputs)
-        else:
-            out = inputs
-        conv = self.conv(out)
-        if self.has_bn:
-            out = self.BNs[-1](conv)
-        else:
-            out = conv
-        if self.relu:
-            out = self.relu(out)
-        else:
-            out = out
-        if self.InShape is None:
-            self.InShape = (inputs.size(-2), inputs.size(-1))
-            self.OutShape = (out.size(-2), out.size(-1))
-        return out
-
-
-class ResNetBasicblock(nn.Module):
-    expansion = 1
-    num_conv = 2
-
-    def __init__(self, inplanes, planes, stride):
-        super(ResNetBasicblock, self).__init__()
-        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
-        self.conv_a = ConvBNReLU(inplanes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
-        self.conv_b = ConvBNReLU(planes, planes, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=False)
-        if stride == 2:
-            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=True, has_bn=False, has_relu=False)
-        elif inplanes != planes:
-            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=False)
-        else:
-            self.downsample = None
-        self.out_dim = planes
-        self.search_mode = 'basic'
-
-    def get_range(self):
-        return self.conv_a.get_range() + self.conv_b.get_range()
-
-    def get_flops(self, channels):
-        assert len(channels) == 3, 'invalid channels : {:}'.format(channels)
-        flop_A = self.conv_a.get_flops([channels[0], channels[1]])
-        flop_B = self.conv_b.get_flops([channels[1], channels[2]])
-        if hasattr(self.downsample, 'get_flops'):
-            flop_C = self.downsample.get_flops([channels[0], channels[-1]])
-        else:
-            flop_C = 0
-        if channels[0] != channels[
-            -1] and self.downsample is None:  # this short-cut will be added during the infer-train
-            flop_C = channels[0] * channels[-1] * self.conv_b.OutShape[0] * self.conv_b.OutShape[1]
-        return flop_A + flop_B + flop_C
-
-    def forward(self, inputs):
-        if self.search_mode == 'basic':
-            return self.basic_forward(inputs)
-        elif self.search_mode == 'search':
-            return self.search_forward(inputs)
-        else:
-            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
-
-    def search_forward(self, tuple_inputs):
-        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
-            type(tuple_inputs))
-        inputs, expected_inC, probability, indexes, probs = tuple_inputs
-        assert indexes.size(0) == 2 and probs.size(0) == 2 and probability.size(0) == 2
-        out_a, expected_inC_a, expected_flop_a = self.conv_a(
-            (inputs, expected_inC, probability[0], indexes[0], probs[0]))
-        out_b, expected_inC_b, expected_flop_b = self.conv_b(
-            (out_a, expected_inC_a, probability[1], indexes[1], probs[1]))
-        if self.downsample is not None:
-            residual, _, expected_flop_c = self.downsample((inputs, expected_inC, probability[1], indexes[1], probs[1]))
-        else:
-            residual, expected_flop_c = inputs, 0
-        out = additive_func(residual, out_b)
-        return nn.functional.relu(out, inplace=True), expected_inC_b, sum(
-            [expected_flop_a, expected_flop_b, expected_flop_c])
-
-    def basic_forward(self, inputs):
-        basicblock = self.conv_a(inputs)
-        basicblock = self.conv_b(basicblock)
-        if self.downsample is not None:
-            residual = self.downsample(inputs)
-        else:
-            residual = inputs
-        out = additive_func(residual, basicblock)
-        return nn.functional.relu(out, inplace=True)
-
-
-class ResNetBottleneck(nn.Module):
-    expansion = 4
-    num_conv = 3
-
-    def __init__(self, inplanes, planes, stride):
-        super(ResNetBottleneck, self).__init__()
-        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
-        self.conv_1x1 = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=True)
-        self.conv_3x3 = ConvBNReLU(planes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
-        self.conv_1x4 = ConvBNReLU(planes, planes * self.expansion, 1, 1, 0, False, has_avg=False, has_bn=True,
-                                   has_relu=False)
-        if stride == 2:
-            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, has_avg=True, has_bn=False,
-                                         has_relu=False)
-        elif inplanes != planes * self.expansion:
-            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, has_avg=False, has_bn=True,
-                                         has_relu=False)
-        else:
-            self.downsample = None
-        self.out_dim = planes * self.expansion
-        self.search_mode = 'basic'
-
-    def get_range(self):
-        return self.conv_1x1.get_range() + self.conv_3x3.get_range() + self.conv_1x4.get_range()
-
-    def get_flops(self, channels):
-        assert len(channels) == 4, 'invalid channels : {:}'.format(channels)
-        flop_A = self.conv_1x1.get_flops([channels[0], channels[1]])
-        flop_B = self.conv_3x3.get_flops([channels[1], channels[2]])
-        flop_C = self.conv_1x4.get_flops([channels[2], channels[3]])
-        if hasattr(self.downsample, 'get_flops'):
-            flop_D = self.downsample.get_flops([channels[0], channels[-1]])
-        else:
-            flop_D = 0
-        if channels[0] != channels[
-            -1] and self.downsample is None:  # this short-cut will be added during the infer-train
-            flop_D = channels[0] * channels[-1] * self.conv_1x4.OutShape[0] * self.conv_1x4.OutShape[1]
-        return flop_A + flop_B + flop_C + flop_D
-
-    def forward(self, inputs):
-        if self.search_mode == 'basic':
-            return self.basic_forward(inputs)
-        elif self.search_mode == 'search':
-            return self.search_forward(inputs)
-        else:
-            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
-
-    def basic_forward(self, inputs):
-        bottleneck = self.conv_1x1(inputs)
-        bottleneck = self.conv_3x3(bottleneck)
-        bottleneck = self.conv_1x4(bottleneck)
-        if self.downsample is not None:
-            residual = self.downsample(inputs)
-        else:
-            residual = inputs
-        out = additive_func(residual, bottleneck)
-        return nn.functional.relu(out, inplace=True)
-
-    def search_forward(self, tuple_inputs):
-        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
-            type(tuple_inputs))
-        inputs, expected_inC, probability, indexes, probs = tuple_inputs
-        assert indexes.size(0) == 3 and probs.size(0) == 3 and probability.size(0) == 3
-        out_1x1, expected_inC_1x1, expected_flop_1x1 = self.conv_1x1(
-            (inputs, expected_inC, probability[0], indexes[0], probs[0]))
-        out_3x3, expected_inC_3x3, expected_flop_3x3 = self.conv_3x3(
-            (out_1x1, expected_inC_1x1, probability[1], indexes[1], probs[1]))
-        out_1x4, expected_inC_1x4, expected_flop_1x4 = self.conv_1x4(
-            (out_3x3, expected_inC_3x3, probability[2], indexes[2], probs[2]))
-        if self.downsample is not None:
-            residual, _, expected_flop_c = self.downsample((inputs, expected_inC, probability[2], indexes[2], probs[2]))
-        else:
-            residual, expected_flop_c = inputs, 0
-        out = additive_func(residual, out_1x4)
-        return nn.functional.relu(out, inplace=True), expected_inC_1x4, sum(
-            [expected_flop_1x1, expected_flop_3x3, expected_flop_1x4, expected_flop_c])
-
-
-class SearchShapeCifarResNet(nn.Module):
-
-    def __init__(self, block_name, depth, num_classes):
-        super(SearchShapeCifarResNet, self).__init__()
-
-        # Model type specifies number of layers for CIFAR-10 and CIFAR-100 model
-        if block_name == 'ResNetBasicblock':
-            block = ResNetBasicblock
-            assert (depth - 2) % 6 == 0, 'depth should be one of 20, 32, 44, 56, 110'
-            layer_blocks = (depth - 2) // 6
-        elif block_name == 'ResNetBottleneck':
-            block = ResNetBottleneck
-            assert (depth - 2) % 9 == 0, 'depth should be one of 164'
-            layer_blocks = (depth - 2) // 9
-        else:
-            raise ValueError('invalid block : {:}'.format(block_name))
-
-        self.message = 'SearchShapeCifarResNet : Depth : {:} , Layers for each block : {:}'.format(depth, layer_blocks)
-        self.num_classes = num_classes
-        self.channels = [16]
-        self.layers = nn.ModuleList([ConvBNReLU(3, 16, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=True)])
-        self.InShape = None
-        self.depth_info = OrderedDict()
-        self.depth_at_i = OrderedDict()
-        for stage in range(3):
-            cur_block_choices = get_depth_choices(layer_blocks, False)
-            assert cur_block_choices[-1] == layer_blocks, 'stage={:}, {:} vs {:}'.format(stage, cur_block_choices,
-                                                                                         layer_blocks)
-            self.message += "\nstage={:} ::: depth-block-choices={:} for {:} blocks.".format(stage, cur_block_choices,
-                                                                                             layer_blocks)
-            block_choices, xstart = [], len(self.layers)
-            for iL in range(layer_blocks):
-                iC = self.channels[-1]
-                planes = 16 * (2 ** stage)
-                stride = 2 if stage > 0 and iL == 0 else 1
-                module = block(iC, planes, stride)
-                self.channels.append(module.out_dim)
-                self.layers.append(module)
-                self.message += "\nstage={:}, ilayer={:02d}/{:02d}, block={:03d}, iC={:3d}, oC={:3d}, stride={:}".format(
-                    stage, iL, layer_blocks, len(self.layers) - 1, iC, module.out_dim, stride)
-                # added for depth
-                layer_index = len(self.layers) - 1
-                if iL + 1 in cur_block_choices: block_choices.append(layer_index)
-                if iL + 1 == layer_blocks:
-                    self.depth_info[layer_index] = {'choices': block_choices,
-                                                    'stage': stage,
-                                                    'xstart': xstart}
-        self.depth_info_list = []
-        for xend, info in self.depth_info.items():
-            self.depth_info_list.append((xend, info))
-            xstart, xstage = info['xstart'], info['stage']
-            for ilayer in range(xstart, xend + 1):
-                idx = bisect_right(info['choices'], ilayer - 1)
-                self.depth_at_i[ilayer] = (xstage, idx)
-
-        self.avgpool = nn.AvgPool2d(8)
-        self.classifier = nn.Linear(module.out_dim, num_classes)
-        self.InShape = None
-        self.tau = -1
-        self.search_mode = 'basic'
-        # assert sum(x.num_conv for x in self.layers) + 1 == depth, 'invalid depth check {:} vs {:}'.format(sum(x.num_conv for x in self.layers)+1, depth)
-
-        # parameters for width
-        self.Ranges = []
-        self.layer2indexRange = []
-        for i, layer in enumerate(self.layers):
-            start_index = len(self.Ranges)
-            self.Ranges += layer.get_range()
-            self.layer2indexRange.append((start_index, len(self.Ranges)))
-        assert len(self.Ranges) + 1 == depth, 'invalid depth check {:} vs {:}'.format(len(self.Ranges) + 1, depth)
-
-        self.register_parameter('width_attentions',
-                                nn.Parameter(torch.Tensor(len(self.Ranges), get_width_choices(None))))
-        self.register_parameter('depth_attentions',
-                                nn.Parameter(torch.Tensor(3, get_depth_choices(layer_blocks, True))))
-        nn.init.normal_(self.width_attentions, 0, 0.01)
-        nn.init.normal_(self.depth_attentions, 0, 0.01)
-        self.apply(initialize_resnet)
-
-    def arch_parameters(self, LR=None):
-        if LR is None:
-            return [self.width_attentions, self.depth_attentions]
-        else:
-            return [
-                {"params": self.width_attentions, "lr": LR},
-                {"params": self.depth_attentions, "lr": LR},
-            ]
-
-    def base_parameters(self):
-        return list(self.layers.parameters()) + list(self.avgpool.parameters()) + list(self.classifier.parameters())
-
-    def get_flop(self, mode, config_dict, extra_info):
-        if config_dict is not None: config_dict = config_dict.copy()
-        # select channels
-        channels = [3]
-        for i, weight in enumerate(self.width_attentions):
-            if mode == 'genotype':
-                with torch.no_grad():
-                    probe = nn.functional.softmax(weight, dim=0)
-                    C = self.Ranges[i][torch.argmax(probe).item()]
-            elif mode == 'max':
-                C = self.Ranges[i][-1]
-            elif mode == 'fix':
-                C = int(math.sqrt(extra_info) * self.Ranges[i][-1])
-            elif mode == 'random':
-                assert isinstance(extra_info, float), 'invalid extra_info : {:}'.format(extra_info)
-                with torch.no_grad():
-                    prob = nn.functional.softmax(weight, dim=0)
-                    approximate_C = int(math.sqrt(extra_info) * self.Ranges[i][-1])
-                    for j in range(prob.size(0)):
-                        prob[j] = 1 / (abs(j - (approximate_C - self.Ranges[i][j])) + 0.2)
-                    C = self.Ranges[i][torch.multinomial(prob, 1, False).item()]
-            else:
-                raise ValueError('invalid mode : {:}'.format(mode))
-            channels.append(C)
-        # select depth
-        if mode == 'genotype':
-            with torch.no_grad():
-                depth_probs = nn.functional.softmax(self.depth_attentions, dim=1)
-                choices = torch.argmax(depth_probs, dim=1).cpu().tolist()
-        elif mode == 'max' or mode == 'fix':
-            choices = [depth_probs.size(1) - 1 for _ in range(depth_probs.size(0))]
-        elif mode == 'random':
-            with torch.no_grad():
-                depth_probs = nn.functional.softmax(self.depth_attentions, dim=1)
-                choices = torch.multinomial(depth_probs, 1, False).cpu().tolist()
-        else:
-            raise ValueError('invalid mode : {:}'.format(mode))
-        selected_layers = []
-        for choice, xvalue in zip(choices, self.depth_info_list):
-            xtemp = xvalue[1]['choices'][choice] - xvalue[1]['xstart'] + 1
-            selected_layers.append(xtemp)
-        flop = 0
-        for i, layer in enumerate(self.layers):
-            s, e = self.layer2indexRange[i]
-            xchl = tuple(channels[s:e + 1])
-            if i in self.depth_at_i:
-                xstagei, xatti = self.depth_at_i[i]
-                if xatti <= choices[xstagei]:  # leave this depth
-                    flop += layer.get_flops(xchl)
-                else:
-                    flop += 0  # do not use this layer
-            else:
-                flop += layer.get_flops(xchl)
-        # the last fc layer
-        flop += channels[-1] * self.classifier.out_features
-        if config_dict is None:
-            return flop / 1e6
-        else:
-            config_dict['xchannels'] = channels
-            config_dict['xblocks'] = selected_layers
-            config_dict['super_type'] = 'infer-shape'
-            config_dict['estimated_FLOP'] = flop / 1e6
-            return flop / 1e6, config_dict
-
-    def get_arch_info(self):
-        string = "for depth and width, there are {:} + {:} attention probabilities.".format(len(self.depth_attentions),
-                                                                                            len(self.width_attentions))
-        string += '\n{:}'.format(self.depth_info)
-        discrepancy = []
-        with torch.no_grad():
-            for i, att in enumerate(self.depth_attentions):
-                prob = nn.functional.softmax(att, dim=0)
-                prob = prob.cpu();
-                selc = prob.argmax().item();
-                prob = prob.tolist()
-                prob = ['{:.3f}'.format(x) for x in prob]
-                xstring = '{:03d}/{:03d}-th : {:}'.format(i, len(self.depth_attentions), ' '.join(prob))
-                logt = ['{:.4f}'.format(x) for x in att.cpu().tolist()]
-                xstring += '  ||  {:17s}'.format(' '.join(logt))
-                prob = sorted([float(x) for x in prob])
-                disc = prob[-1] - prob[-2]
-                xstring += '  || discrepancy={:.2f} || select={:}/{:}'.format(disc, selc, len(prob))
-                discrepancy.append(disc)
-                string += '\n{:}'.format(xstring)
-            string += '\n-----------------------------------------------'
-            for i, att in enumerate(self.width_attentions):
-                prob = nn.functional.softmax(att, dim=0)
-                prob = prob.cpu();
-                selc = prob.argmax().item();
-                prob = prob.tolist()
-                prob = ['{:.3f}'.format(x) for x in prob]
-                xstring = '{:03d}/{:03d}-th : {:}'.format(i, len(self.width_attentions), ' '.join(prob))
-                logt = ['{:.3f}'.format(x) for x in att.cpu().tolist()]
-                xstring += '  ||  {:52s}'.format(' '.join(logt))
-                prob = sorted([float(x) for x in prob])
-                disc = prob[-1] - prob[-2]
-                xstring += '  || dis={:.2f} || select={:}/{:}'.format(disc, selc, len(prob))
-                discrepancy.append(disc)
-                string += '\n{:}'.format(xstring)
-        return string, discrepancy
-
-    def set_tau(self, tau_max, tau_min, epoch_ratio):
-        assert epoch_ratio >= 0 and epoch_ratio <= 1, 'invalid epoch-ratio : {:}'.format(epoch_ratio)
-        tau = tau_min + (tau_max - tau_min) * (1 + math.cos(math.pi * epoch_ratio)) / 2
-        self.tau = tau
-
-    def get_message(self):
-        return self.message
-
-    def forward(self, inputs):
-        if self.search_mode == 'basic':
-            return self.basic_forward(inputs)
-        elif self.search_mode == 'search':
-            return self.search_forward(inputs)
-        else:
-            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
-
-    def search_forward(self, inputs):
-        flop_width_probs = nn.functional.softmax(self.width_attentions, dim=1)
-        flop_depth_probs = nn.functional.softmax(self.depth_attentions, dim=1)
-        flop_depth_probs = torch.flip(torch.cumsum(torch.flip(flop_depth_probs, [1]), 1), [1])
-        selected_widths, selected_width_probs = select2withP(self.width_attentions, self.tau)
-        selected_depth_probs = select2withP(self.depth_attentions, self.tau, True)
-        with torch.no_grad():
-            selected_widths = selected_widths.cpu()
-
-        x, last_channel_idx, expected_inC, flops = inputs, 0, 3, []
-        feature_maps = []
-        for i, layer in enumerate(self.layers):
-            selected_w_index = selected_widths[last_channel_idx: last_channel_idx + layer.num_conv]
-            selected_w_probs = selected_width_probs[last_channel_idx: last_channel_idx + layer.num_conv]
-            layer_prob = flop_width_probs[last_channel_idx: last_channel_idx + layer.num_conv]
-            x, expected_inC, expected_flop = layer((x, expected_inC, layer_prob, selected_w_index, selected_w_probs))
-            feature_maps.append(x)
-            last_channel_idx += layer.num_conv
-            if i in self.depth_info:  # aggregate the information
-                choices = self.depth_info[i]['choices']
-                xstagei = self.depth_info[i]['stage']
-                # print ('iL={:}, choices={:}, stage={:}, probs={:}'.format(i, choices, xstagei, selected_depth_probs[xstagei].cpu().tolist()))
-                # for A, W in zip(choices, selected_depth_probs[xstagei]):
-                #  print('Size = {:}, W = {:}'.format(feature_maps[A].size(), W))
-                possible_tensors = []
-                max_C = max(feature_maps[A].size(1) for A in choices)
-                for tempi, A in enumerate(choices):
-                    xtensor = ChannelWiseInter(feature_maps[A], max_C)
-                    # drop_ratio = 1-(tempi+1.0)/len(choices)
-                    # xtensor = drop_path(xtensor, drop_ratio)
-                    possible_tensors.append(xtensor)
-                weighted_sum = sum(xtensor * W for xtensor, W in zip(possible_tensors, selected_depth_probs[xstagei]))
-                x = weighted_sum
-
-            if i in self.depth_at_i:
-                xstagei, xatti = self.depth_at_i[i]
-                x_expected_flop = flop_depth_probs[xstagei, xatti] * expected_flop
-            else:
-                x_expected_flop = expected_flop
-            flops.append(x_expected_flop)
-        flops.append(expected_inC * (self.classifier.out_features * 1.0 / 1e6))
-        features = self.avgpool(x)
-        features = features.view(features.size(0), -1)
-        logits = linear_forward(features, self.classifier)
-        return logits, torch.stack([sum(flops)])
-
-    def basic_forward(self, inputs):
-        if self.InShape is None: self.InShape = (inputs.size(-2), inputs.size(-1))
-        x = inputs
-        for i, layer in enumerate(self.layers):
-            x = layer(x)
-        features = self.avgpool(x)
-        features = features.view(features.size(0), -1)
-        logits = self.classifier(features)
-        return features, logits
+import math, torch
+from collections import OrderedDict
+from bisect import bisect_right
+import torch.nn as nn
+from ..initialization import initialize_resnet
+from ..SharedUtils import additive_func
+from .SoftSelect import select2withP, ChannelWiseInter
+from .SoftSelect import linear_forward
+from .SoftSelect import get_width_choices
+
+
+def get_depth_choices(layers):
+    min_depth = min(layers)
+    info = {'num': min_depth}
+    for i, depth in enumerate(layers):
+        choices = []
+        for j in range(1, min_depth + 1):
+            choices.append(int(float(depth) * j / min_depth))
+        info[i] = choices
+    return info
+
+
+def conv_forward(inputs, conv, choices):
+    iC = conv.in_channels
+    fill_size = list(inputs.size())
+    fill_size[1] = iC - fill_size[1]
+    filled = torch.zeros(fill_size, device=inputs.device)
+    xinputs = torch.cat((inputs, filled), dim=1)
+    outputs = conv(xinputs)
+    selecteds = [outputs[:, :oC] for oC in choices]
+    return selecteds
+
+
+class ConvBNReLU(nn.Module):
+    num_conv = 1
+
+    def __init__(self, nIn, nOut, kernel, stride, padding, bias, has_avg, has_bn, has_relu, last_max_pool=False):
+        super(ConvBNReLU, self).__init__()
+        self.InShape = None
+        self.OutShape = None
+        self.choices = get_width_choices(nOut)
+        self.register_buffer('choices_tensor', torch.Tensor(self.choices))
+
+        if has_avg:
+            self.avg = nn.AvgPool2d(kernel_size=2, stride=2, padding=0)
+        else:
+            self.avg = None
+        self.conv = nn.Conv2d(nIn, nOut, kernel_size=kernel, stride=stride, padding=padding, dilation=1, groups=1,
+                              bias=bias)
+        # if has_bn  : self.bn  = nn.BatchNorm2d(nOut)
+        # else       : self.bn  = None
+        self.has_bn = has_bn
+        self.BNs = nn.ModuleList()
+        for i, _out in enumerate(self.choices):
+            self.BNs.append(nn.BatchNorm2d(_out))
+        if has_relu:
+            self.relu = nn.ReLU(inplace=True)
+        else:
+            self.relu = None
+
+        if last_max_pool:
+            self.maxpool = nn.MaxPool2d(kernel_size=3, stride=2, padding=1)
+        else:
+            self.maxpool = None
+        self.in_dim = nIn
+        self.out_dim = nOut
+        self.search_mode = 'basic'
+
+    def get_flops(self, channels, check_range=True, divide=1):
+        iC, oC = channels
+        if check_range: assert iC <= self.conv.in_channels and oC <= self.conv.out_channels, '{:} vs {:}  |  {:} vs {:}'.format(
+            iC, self.conv.in_channels, oC, self.conv.out_channels)
+        assert isinstance(self.InShape, tuple) and len(self.InShape) == 2, 'invalid in-shape : {:}'.format(self.InShape)
+        assert isinstance(self.OutShape, tuple) and len(self.OutShape) == 2, 'invalid out-shape : {:}'.format(
+            self.OutShape)
+        # conv_per_position_flops = self.conv.kernel_size[0] * self.conv.kernel_size[1] * iC * oC / self.conv.groups
+        conv_per_position_flops = (self.conv.kernel_size[0] * self.conv.kernel_size[1] * 1.0 / self.conv.groups)
+        all_positions = self.OutShape[0] * self.OutShape[1]
+        flops = (conv_per_position_flops * all_positions / divide) * iC * oC
+        if self.conv.bias is not None: flops += all_positions / divide
+        return flops
+
+    def get_range(self):
+        return [self.choices]
+
+    def forward(self, inputs):
+        if self.search_mode == 'basic':
+            return self.basic_forward(inputs)
+        elif self.search_mode == 'search':
+            return self.search_forward(inputs)
+        else:
+            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
+
+    def search_forward(self, tuple_inputs):
+        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
+            type(tuple_inputs))
+        inputs, expected_inC, probability, index, prob = tuple_inputs
+        index, prob = torch.squeeze(index).tolist(), torch.squeeze(prob)
+        probability = torch.squeeze(probability)
+        assert len(index) == 2, 'invalid length : {:}'.format(index)
+        # compute expected flop
+        # coordinates   = torch.arange(self.x_range[0], self.x_range[1]+1).type_as(probability)
+        expected_outC = (self.choices_tensor * probability).sum()
+        expected_flop = self.get_flops([expected_inC, expected_outC], False, 1e6)
+        if self.avg:
+            out = self.avg(inputs)
+        else:
+            out = inputs
+        # convolutional layer
+        out_convs = conv_forward(out, self.conv, [self.choices[i] for i in index])
+        out_bns = [self.BNs[idx](out_conv) for idx, out_conv in zip(index, out_convs)]
+        # merge
+        out_channel = max([x.size(1) for x in out_bns])
+        outA = ChannelWiseInter(out_bns[0], out_channel)
+        outB = ChannelWiseInter(out_bns[1], out_channel)
+        out = outA * prob[0] + outB * prob[1]
+        # out = additive_func(out_bns[0]*prob[0], out_bns[1]*prob[1])
+
+        if self.relu: out = self.relu(out)
+        if self.maxpool: out = self.maxpool(out)
+        return out, expected_outC, expected_flop
+
+    def basic_forward(self, inputs):
+        if self.avg:
+            out = self.avg(inputs)
+        else:
+            out = inputs
+        conv = self.conv(out)
+        if self.has_bn:
+            out = self.BNs[-1](conv)
+        else:
+            out = conv
+        if self.relu:
+            out = self.relu(out)
+        else:
+            out = out
+        if self.InShape is None:
+            self.InShape = (inputs.size(-2), inputs.size(-1))
+            self.OutShape = (out.size(-2), out.size(-1))
+        if self.maxpool: out = self.maxpool(out)
+        return out
+
+
+class ResNetBasicblock(nn.Module):
+    expansion = 1
+    num_conv = 2
+
+    def __init__(self, inplanes, planes, stride):
+        super(ResNetBasicblock, self).__init__()
+        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
+        self.conv_a = ConvBNReLU(inplanes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
+        self.conv_b = ConvBNReLU(planes, planes, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=False)
+        if stride == 2:
+            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=True, has_bn=True, has_relu=False)
+        elif inplanes != planes:
+            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=False)
+        else:
+            self.downsample = None
+        self.out_dim = planes
+        self.search_mode = 'basic'
+
+    def get_range(self):
+        return self.conv_a.get_range() + self.conv_b.get_range()
+
+    def get_flops(self, channels):
+        assert len(channels) == 3, 'invalid channels : {:}'.format(channels)
+        flop_A = self.conv_a.get_flops([channels[0], channels[1]])
+        flop_B = self.conv_b.get_flops([channels[1], channels[2]])
+        if hasattr(self.downsample, 'get_flops'):
+            flop_C = self.downsample.get_flops([channels[0], channels[-1]])
+        else:
+            flop_C = 0
+        if channels[0] != channels[
+            -1] and self.downsample is None:  # this short-cut will be added during the infer-train
+            flop_C = channels[0] * channels[-1] * self.conv_b.OutShape[0] * self.conv_b.OutShape[1]
+        return flop_A + flop_B + flop_C
+
+    def forward(self, inputs):
+        if self.search_mode == 'basic':
+            return self.basic_forward(inputs)
+        elif self.search_mode == 'search':
+            return self.search_forward(inputs)
+        else:
+            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
+
+    def search_forward(self, tuple_inputs):
+        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
+            type(tuple_inputs))
+        inputs, expected_inC, probability, indexes, probs = tuple_inputs
+        assert indexes.size(0) == 2 and probs.size(0) == 2 and probability.size(0) == 2
+        # import pdb; pdb.set_trace()
+        out_a, expected_inC_a, expected_flop_a = self.conv_a(
+            (inputs, expected_inC, probability[0], indexes[0], probs[0]))
+        out_b, expected_inC_b, expected_flop_b = self.conv_b(
+            (out_a, expected_inC_a, probability[1], indexes[1], probs[1]))
+        if self.downsample is not None:
+            residual, _, expected_flop_c = self.downsample((inputs, expected_inC, probability[1], indexes[1], probs[1]))
+        else:
+            residual, expected_flop_c = inputs, 0
+        out = additive_func(residual, out_b)
+        return nn.functional.relu(out, inplace=True), expected_inC_b, sum(
+            [expected_flop_a, expected_flop_b, expected_flop_c])
+
+    def basic_forward(self, inputs):
+        basicblock = self.conv_a(inputs)
+        basicblock = self.conv_b(basicblock)
+        if self.downsample is not None:
+            residual = self.downsample(inputs)
+        else:
+            residual = inputs
+        out = additive_func(residual, basicblock)
+        return nn.functional.relu(out, inplace=True)
+
+
+class ResNetBottleneck(nn.Module):
+    expansion = 4
+    num_conv = 3
+
+    def __init__(self, inplanes, planes, stride):
+        super(ResNetBottleneck, self).__init__()
+        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
+        self.conv_1x1 = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=True)
+        self.conv_3x3 = ConvBNReLU(planes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
+        self.conv_1x4 = ConvBNReLU(planes, planes * self.expansion, 1, 1, 0, False, has_avg=False, has_bn=True,
+                                   has_relu=False)
+        if stride == 2:
+            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, has_avg=True, has_bn=True,
+                                         has_relu=False)
+        elif inplanes != planes * self.expansion:
+            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, has_avg=False, has_bn=True,
+                                         has_relu=False)
+        else:
+            self.downsample = None
+        self.out_dim = planes * self.expansion
+        self.search_mode = 'basic'
+
+    def get_range(self):
+        return self.conv_1x1.get_range() + self.conv_3x3.get_range() + self.conv_1x4.get_range()
+
+    def get_flops(self, channels):
+        assert len(channels) == 4, 'invalid channels : {:}'.format(channels)
+        flop_A = self.conv_1x1.get_flops([channels[0], channels[1]])
+        flop_B = self.conv_3x3.get_flops([channels[1], channels[2]])
+        flop_C = self.conv_1x4.get_flops([channels[2], channels[3]])
+        if hasattr(self.downsample, 'get_flops'):
+            flop_D = self.downsample.get_flops([channels[0], channels[-1]])
+        else:
+            flop_D = 0
+        if channels[0] != channels[
+            -1] and self.downsample is None:  # this short-cut will be added during the infer-train
+            flop_D = channels[0] * channels[-1] * self.conv_1x4.OutShape[0] * self.conv_1x4.OutShape[1]
+        return flop_A + flop_B + flop_C + flop_D
+
+    def forward(self, inputs):
+        if self.search_mode == 'basic':
+            return self.basic_forward(inputs)
+        elif self.search_mode == 'search':
+            return self.search_forward(inputs)
+        else:
+            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
+
+    def basic_forward(self, inputs):
+        bottleneck = self.conv_1x1(inputs)
+        bottleneck = self.conv_3x3(bottleneck)
+        bottleneck = self.conv_1x4(bottleneck)
+        if self.downsample is not None:
+            residual = self.downsample(inputs)
+        else:
+            residual = inputs
+        out = additive_func(residual, bottleneck)
+        return nn.functional.relu(out, inplace=True)
+
+    def search_forward(self, tuple_inputs):
+        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
+            type(tuple_inputs))
+        inputs, expected_inC, probability, indexes, probs = tuple_inputs
+        assert indexes.size(0) == 3 and probs.size(0) == 3 and probability.size(0) == 3
+        out_1x1, expected_inC_1x1, expected_flop_1x1 = self.conv_1x1(
+            (inputs, expected_inC, probability[0], indexes[0], probs[0]))
+        out_3x3, expected_inC_3x3, expected_flop_3x3 = self.conv_3x3(
+            (out_1x1, expected_inC_1x1, probability[1], indexes[1], probs[1]))
+        out_1x4, expected_inC_1x4, expected_flop_1x4 = self.conv_1x4(
+            (out_3x3, expected_inC_3x3, probability[2], indexes[2], probs[2]))
+        if self.downsample is not None:
+            residual, _, expected_flop_c = self.downsample((inputs, expected_inC, probability[2], indexes[2], probs[2]))
+        else:
+            residual, expected_flop_c = inputs, 0
+        out = additive_func(residual, out_1x4)
+        return nn.functional.relu(out, inplace=True), expected_inC_1x4, sum(
+            [expected_flop_1x1, expected_flop_3x3, expected_flop_1x4, expected_flop_c])
+
+
+class SearchShapeImagenetResNet(nn.Module):
+
+    def __init__(self, block_name, layers, deep_stem, num_classes):
+        super(SearchShapeImagenetResNet, self).__init__()
+
+        # Model type specifies number of layers for CIFAR-10 and CIFAR-100 model
+        if block_name == 'BasicBlock':
+            block = ResNetBasicblock
+        elif block_name == 'Bottleneck':
+            block = ResNetBottleneck
+        else:
+            raise ValueError('invalid block : {:}'.format(block_name))
+
+        self.message = 'SearchShapeCifarResNet : Depth : {:} , Layers for each block : {:}'.format(
+            sum(layers) * block.num_conv, layers)
+        self.num_classes = num_classes
+        if not deep_stem:
+            self.layers = nn.ModuleList(
+                [ConvBNReLU(3, 64, 7, 2, 3, False, has_avg=False, has_bn=True, has_relu=True, last_max_pool=True)])
+            self.channels = [64]
+        else:
+            self.layers = nn.ModuleList([ConvBNReLU(3, 32, 3, 2, 1, False, has_avg=False, has_bn=True, has_relu=True)
+                                            ,
+                                         ConvBNReLU(32, 64, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=True,
+                                                    last_max_pool=True)])
+            self.channels = [32, 64]
+
+        meta_depth_info = get_depth_choices(layers)
+        self.InShape = None
+        self.depth_info = OrderedDict()
+        self.depth_at_i = OrderedDict()
+        for stage, layer_blocks in enumerate(layers):
+            cur_block_choices = meta_depth_info[stage]
+            assert cur_block_choices[-1] == layer_blocks, 'stage={:}, {:} vs {:}'.format(stage, cur_block_choices,
+                                                                                         layer_blocks)
+            block_choices, xstart = [], len(self.layers)
+            for iL in range(layer_blocks):
+                iC = self.channels[-1]
+                planes = 64 * (2 ** stage)
+                stride = 2 if stage > 0 and iL == 0 else 1
+                module = block(iC, planes, stride)
+                self.channels.append(module.out_dim)
+                self.layers.append(module)
+                self.message += "\nstage={:}, ilayer={:02d}/{:02d}, block={:03d}, iC={:3d}, oC={:3d}, stride={:}".format(
+                    stage, iL, layer_blocks, len(self.layers) - 1, iC, module.out_dim, stride)
+                # added for depth
+                layer_index = len(self.layers) - 1
+                if iL + 1 in cur_block_choices: block_choices.append(layer_index)
+                if iL + 1 == layer_blocks:
+                    self.depth_info[layer_index] = {'choices': block_choices,
+                                                    'stage': stage,
+                                                    'xstart': xstart}
+        self.depth_info_list = []
+        for xend, info in self.depth_info.items():
+            self.depth_info_list.append((xend, info))
+            xstart, xstage = info['xstart'], info['stage']
+            for ilayer in range(xstart, xend + 1):
+                idx = bisect_right(info['choices'], ilayer - 1)
+                self.depth_at_i[ilayer] = (xstage, idx)
+
+        self.avgpool = nn.AdaptiveAvgPool2d((1, 1))
+        self.classifier = nn.Linear(module.out_dim, num_classes)
+        self.InShape = None
+        self.tau = -1
+        self.search_mode = 'basic'
+        # assert sum(x.num_conv for x in self.layers) + 1 == depth, 'invalid depth check {:} vs {:}'.format(sum(x.num_conv for x in self.layers)+1, depth)
+
+        # parameters for width
+        self.Ranges = []
+        self.layer2indexRange = []
+        for i, layer in enumerate(self.layers):
+            start_index = len(self.Ranges)
+            self.Ranges += layer.get_range()
+            self.layer2indexRange.append((start_index, len(self.Ranges)))
+
+        self.register_parameter('width_attentions',
+                                nn.Parameter(torch.Tensor(len(self.Ranges), get_width_choices(None))))
+        self.register_parameter('depth_attentions', nn.Parameter(torch.Tensor(len(layers), meta_depth_info['num'])))
+        nn.init.normal_(self.width_attentions, 0, 0.01)
+        nn.init.normal_(self.depth_attentions, 0, 0.01)
+        self.apply(initialize_resnet)
+
+    def arch_parameters(self, LR=None):
+        if LR is None:
+            return [self.width_attentions, self.depth_attentions]
+        else:
+            return [
+                {"params": self.width_attentions, "lr": LR},
+                {"params": self.depth_attentions, "lr": LR},
+            ]
+
+    def base_parameters(self):
+        return list(self.layers.parameters()) + list(self.avgpool.parameters()) + list(self.classifier.parameters())
+
+    def get_flop(self, mode, config_dict, extra_info):
+        if config_dict is not None: config_dict = config_dict.copy()
+        # select channels
+        channels = [3]
+        for i, weight in enumerate(self.width_attentions):
+            if mode == 'genotype':
+                with torch.no_grad():
+                    probe = nn.functional.softmax(weight, dim=0)
+                    C = self.Ranges[i][torch.argmax(probe).item()]
+            else:
+                raise ValueError('invalid mode : {:}'.format(mode))
+            channels.append(C)
+        # select depth
+        if mode == 'genotype':
+            with torch.no_grad():
+                depth_probs = nn.functional.softmax(self.depth_attentions, dim=1)
+                choices = torch.argmax(depth_probs, dim=1).cpu().tolist()
+        else:
+            raise ValueError('invalid mode : {:}'.format(mode))
+        selected_layers = []
+        for choice, xvalue in zip(choices, self.depth_info_list):
+            xtemp = xvalue[1]['choices'][choice] - xvalue[1]['xstart'] + 1
+            selected_layers.append(xtemp)
+        flop = 0
+        for i, layer in enumerate(self.layers):
+            s, e = self.layer2indexRange[i]
+            xchl = tuple(channels[s:e + 1])
+            if i in self.depth_at_i:
+                xstagei, xatti = self.depth_at_i[i]
+                if xatti <= choices[xstagei]:  # leave this depth
+                    flop += layer.get_flops(xchl)
+                else:
+                    flop += 0  # do not use this layer
+            else:
+                flop += layer.get_flops(xchl)
+        # the last fc layer
+        flop += channels[-1] * self.classifier.out_features
+        if config_dict is None:
+            return flop / 1e6
+        else:
+            config_dict['xchannels'] = channels
+            config_dict['xblocks'] = selected_layers
+            config_dict['super_type'] = 'infer-shape'
+            config_dict['estimated_FLOP'] = flop / 1e6
+            return flop / 1e6, config_dict
+
+    def get_arch_info(self):
+        string = "for depth and width, there are {:} + {:} attention probabilities.".format(len(self.depth_attentions),
+                                                                                            len(self.width_attentions))
+        string += '\n{:}'.format(self.depth_info)
+        discrepancy = []
+        with torch.no_grad():
+            for i, att in enumerate(self.depth_attentions):
+                prob = nn.functional.softmax(att, dim=0)
+                prob = prob.cpu();
+                selc = prob.argmax().item();
+                prob = prob.tolist()
+                prob = ['{:.3f}'.format(x) for x in prob]
+                xstring = '{:03d}/{:03d}-th : {:}'.format(i, len(self.depth_attentions), ' '.join(prob))
+                logt = ['{:.4f}'.format(x) for x in att.cpu().tolist()]
+                xstring += '  ||  {:17s}'.format(' '.join(logt))
+                prob = sorted([float(x) for x in prob])
+                disc = prob[-1] - prob[-2]
+                xstring += '  || discrepancy={:.2f} || select={:}/{:}'.format(disc, selc, len(prob))
+                discrepancy.append(disc)
+                string += '\n{:}'.format(xstring)
+            string += '\n-----------------------------------------------'
+            for i, att in enumerate(self.width_attentions):
+                prob = nn.functional.softmax(att, dim=0)
+                prob = prob.cpu();
+                selc = prob.argmax().item();
+                prob = prob.tolist()
+                prob = ['{:.3f}'.format(x) for x in prob]
+                xstring = '{:03d}/{:03d}-th : {:}'.format(i, len(self.width_attentions), ' '.join(prob))
+                logt = ['{:.3f}'.format(x) for x in att.cpu().tolist()]
+                xstring += '  ||  {:52s}'.format(' '.join(logt))
+                prob = sorted([float(x) for x in prob])
+                disc = prob[-1] - prob[-2]
+                xstring += '  || dis={:.2f} || select={:}/{:}'.format(disc, selc, len(prob))
+                discrepancy.append(disc)
+                string += '\n{:}'.format(xstring)
+        return string, discrepancy
+
+    def set_tau(self, tau_max, tau_min, epoch_ratio):
+        assert epoch_ratio >= 0 and epoch_ratio <= 1, 'invalid epoch-ratio : {:}'.format(epoch_ratio)
+        tau = tau_min + (tau_max - tau_min) * (1 + math.cos(math.pi * epoch_ratio)) / 2
+        self.tau = tau
+
+    def get_message(self):
+        return self.message
+
+    def forward(self, inputs):
+        if self.search_mode == 'basic':
+            return self.basic_forward(inputs)
+        elif self.search_mode == 'search':
+            return self.search_forward(inputs)
+        else:
+            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
+
+    def search_forward(self, inputs):
+        flop_width_probs = nn.functional.softmax(self.width_attentions, dim=1)
+        flop_depth_probs = nn.functional.softmax(self.depth_attentions, dim=1)
+        flop_depth_probs = torch.flip(torch.cumsum(torch.flip(flop_depth_probs, [1]), 1), [1])
+        selected_widths, selected_width_probs = select2withP(self.width_attentions, self.tau)
+        selected_depth_probs = select2withP(self.depth_attentions, self.tau, True)
+        with torch.no_grad():
+            selected_widths = selected_widths.cpu()
+
+        x, last_channel_idx, expected_inC, flops = inputs, 0, 3, []
+        feature_maps = []
+        for i, layer in enumerate(self.layers):
+            selected_w_index = selected_widths[last_channel_idx: last_channel_idx + layer.num_conv]
+            selected_w_probs = selected_width_probs[last_channel_idx: last_channel_idx + layer.num_conv]
+            layer_prob = flop_width_probs[last_channel_idx: last_channel_idx + layer.num_conv]
+            x, expected_inC, expected_flop = layer((x, expected_inC, layer_prob, selected_w_index, selected_w_probs))
+            feature_maps.append(x)
+            last_channel_idx += layer.num_conv
+            if i in self.depth_info:  # aggregate the information
+                choices = self.depth_info[i]['choices']
+                xstagei = self.depth_info[i]['stage']
+                # print ('iL={:}, choices={:}, stage={:}, probs={:}'.format(i, choices, xstagei, selected_depth_probs[xstagei].cpu().tolist()))
+                # for A, W in zip(choices, selected_depth_probs[xstagei]):
+                #  print('Size = {:}, W = {:}'.format(feature_maps[A].size(), W))
+                possible_tensors = []
+                max_C = max(feature_maps[A].size(1) for A in choices)
+                for tempi, A in enumerate(choices):
+                    xtensor = ChannelWiseInter(feature_maps[A], max_C)
+                    possible_tensors.append(xtensor)
+                weighted_sum = sum(xtensor * W for xtensor, W in zip(possible_tensors, selected_depth_probs[xstagei]))
+                x = weighted_sum
+
+            if i in self.depth_at_i:
+                xstagei, xatti = self.depth_at_i[i]
+                x_expected_flop = flop_depth_probs[xstagei, xatti] * expected_flop
+            else:
+                x_expected_flop = expected_flop
+            flops.append(x_expected_flop)
+        flops.append(expected_inC * (self.classifier.out_features * 1.0 / 1e6))
+        features = self.avgpool(x)
+        features = features.view(features.size(0), -1)
+        logits = linear_forward(features, self.classifier)
+        return logits, torch.stack([sum(flops)])
+
+    def basic_forward(self, inputs):
+        if self.InShape is None: self.InShape = (inputs.size(-2), inputs.size(-1))
+        x = inputs
+        for i, layer in enumerate(self.layers):
+            x = layer(x)
+        features = self.avgpool(x)
+        features = features.view(features.size(0), -1)
+        logits = self.classifier(features)
+        return features, logits
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchCifarResNet_depth.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchCifarResNet_depth.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,372 +1,372 @@
-##################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
-##################################################
-import math, torch
-from collections import OrderedDict
-from bisect import bisect_right
-import torch.nn as nn
-from ..initialization import initialize_resnet
-from ..SharedUtils import additive_func
-from .SoftSelect import select2withP, ChannelWiseInter
-from .SoftSelect import linear_forward
-from .SoftSelect import get_width_choices
-
-
-def get_depth_choices(nDepth, return_num):
-    if nDepth == 2:
-        choices = (1, 2)
-    elif nDepth == 3:
-        choices = (1, 2, 3)
-    elif nDepth > 3:
-        choices = list(range(1, nDepth + 1, 2))
-        if choices[-1] < nDepth: choices.append(nDepth)
-    else:
-        raise ValueError('invalid nDepth : {:}'.format(nDepth))
-    if return_num:
-        return len(choices)
-    else:
-        return choices
-
-
-class ConvBNReLU(nn.Module):
-    num_conv = 1
-
-    def __init__(self, nIn, nOut, kernel, stride, padding, bias, has_avg, has_bn, has_relu):
-        super(ConvBNReLU, self).__init__()
-        self.InShape = None
-        self.OutShape = None
-        self.choices = get_width_choices(nOut)
-        self.register_buffer('choices_tensor', torch.Tensor(self.choices))
-
-        if has_avg:
-            self.avg = nn.AvgPool2d(kernel_size=2, stride=2, padding=0)
-        else:
-            self.avg = None
-        self.conv = nn.Conv2d(nIn, nOut, kernel_size=kernel, stride=stride, padding=padding, dilation=1, groups=1,
-                              bias=bias)
-        if has_bn:
-            self.bn = nn.BatchNorm2d(nOut)
-        else:
-            self.bn = None
-        if has_relu:
-            self.relu = nn.ReLU(inplace=False)
-        else:
-            self.relu = None
-        self.in_dim = nIn
-        self.out_dim = nOut
-
-    def get_flops(self, divide=1):
-        iC, oC = self.in_dim, self.out_dim
-        assert iC <= self.conv.in_channels and oC <= self.conv.out_channels, '{:} vs {:}  |  {:} vs {:}'.format(iC,
-                                                                                                                self.conv.in_channels,
-                                                                                                                oC,
-                                                                                                                self.conv.out_channels)
-        assert isinstance(self.InShape, tuple) and len(self.InShape) == 2, 'invalid in-shape : {:}'.format(self.InShape)
-        assert isinstance(self.OutShape, tuple) and len(self.OutShape) == 2, 'invalid out-shape : {:}'.format(
-            self.OutShape)
-        # conv_per_position_flops = self.conv.kernel_size[0] * self.conv.kernel_size[1] * iC * oC / self.conv.groups
-        conv_per_position_flops = (self.conv.kernel_size[0] * self.conv.kernel_size[1] * 1.0 / self.conv.groups)
-        all_positions = self.OutShape[0] * self.OutShape[1]
-        flops = (conv_per_position_flops * all_positions / divide) * iC * oC
-        if self.conv.bias is not None: flops += all_positions / divide
-        return flops
-
-    def forward(self, inputs):
-        if self.avg:
-            out = self.avg(inputs)
-        else:
-            out = inputs
-        conv = self.conv(out)
-        if self.bn:
-            out = self.bn(conv)
-        else:
-            out = conv
-        if self.relu:
-            out = self.relu(out)
-        else:
-            out = out
-        if self.InShape is None:
-            self.InShape = (inputs.size(-2), inputs.size(-1))
-            self.OutShape = (out.size(-2), out.size(-1))
-        return out
-
-
-class ResNetBasicblock(nn.Module):
-    expansion = 1
-    num_conv = 2
-
-    def __init__(self, inplanes, planes, stride):
-        super(ResNetBasicblock, self).__init__()
-        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
-        self.conv_a = ConvBNReLU(inplanes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
-        self.conv_b = ConvBNReLU(planes, planes, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=False)
-        if stride == 2:
-            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=True, has_bn=False, has_relu=False)
-        elif inplanes != planes:
-            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=False)
-        else:
-            self.downsample = None
-        self.out_dim = planes
-        self.search_mode = 'basic'
-
-    def get_flops(self, divide=1):
-        flop_A = self.conv_a.get_flops(divide)
-        flop_B = self.conv_b.get_flops(divide)
-        if hasattr(self.downsample, 'get_flops'):
-            flop_C = self.downsample.get_flops(divide)
-        else:
-            flop_C = 0
-        return flop_A + flop_B + flop_C
-
-    def forward(self, inputs):
-        basicblock = self.conv_a(inputs)
-        basicblock = self.conv_b(basicblock)
-        if self.downsample is not None:
-            residual = self.downsample(inputs)
-        else:
-            residual = inputs
-        out = additive_func(residual, basicblock)
-        return nn.functional.relu(out, inplace=True)
-
-
-class ResNetBottleneck(nn.Module):
-    expansion = 4
-    num_conv = 3
-
-    def __init__(self, inplanes, planes, stride):
-        super(ResNetBottleneck, self).__init__()
-        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
-        self.conv_1x1 = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=True)
-        self.conv_3x3 = ConvBNReLU(planes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
-        self.conv_1x4 = ConvBNReLU(planes, planes * self.expansion, 1, 1, 0, False, has_avg=False, has_bn=True,
-                                   has_relu=False)
-        if stride == 2:
-            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, has_avg=True, has_bn=False,
-                                         has_relu=False)
-        elif inplanes != planes * self.expansion:
-            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, has_avg=False, has_bn=True,
-                                         has_relu=False)
-        else:
-            self.downsample = None
-        self.out_dim = planes * self.expansion
-        self.search_mode = 'basic'
-
-    def get_range(self):
-        return self.conv_1x1.get_range() + self.conv_3x3.get_range() + self.conv_1x4.get_range()
-
-    def get_flops(self, divide):
-        flop_A = self.conv_1x1.get_flops(divide)
-        flop_B = self.conv_3x3.get_flops(divide)
-        flop_C = self.conv_1x4.get_flops(divide)
-        if hasattr(self.downsample, 'get_flops'):
-            flop_D = self.downsample.get_flops(divide)
-        else:
-            flop_D = 0
-        return flop_A + flop_B + flop_C + flop_D
-
-    def forward(self, inputs):
-        bottleneck = self.conv_1x1(inputs)
-        bottleneck = self.conv_3x3(bottleneck)
-        bottleneck = self.conv_1x4(bottleneck)
-        if self.downsample is not None:
-            residual = self.downsample(inputs)
-        else:
-            residual = inputs
-        out = additive_func(residual, bottleneck)
-        return nn.functional.relu(out, inplace=True)
-
-
-class SearchDepthCifarResNet(nn.Module):
-
-    def __init__(self, block_name, depth, num_classes):
-        super(SearchDepthCifarResNet, self).__init__()
-
-        # Model type specifies number of layers for CIFAR-10 and CIFAR-100 model
-        if block_name == 'ResNetBasicblock':
-            block = ResNetBasicblock
-            assert (depth - 2) % 6 == 0, 'depth should be one of 20, 32, 44, 56, 110'
-            layer_blocks = (depth - 2) // 6
-        elif block_name == 'ResNetBottleneck':
-            block = ResNetBottleneck
-            assert (depth - 2) % 9 == 0, 'depth should be one of 164'
-            layer_blocks = (depth - 2) // 9
-        else:
-            raise ValueError('invalid block : {:}'.format(block_name))
-
-        self.message = 'SearchShapeCifarResNet : Depth : {:} , Layers for each block : {:}'.format(depth, layer_blocks)
-        self.num_classes = num_classes
-        self.channels = [16]
-        self.layers = nn.ModuleList([ConvBNReLU(3, 16, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=True)])
-        self.InShape = None
-        self.depth_info = OrderedDict()
-        self.depth_at_i = OrderedDict()
-        for stage in range(3):
-            cur_block_choices = get_depth_choices(layer_blocks, False)
-            assert cur_block_choices[-1] == layer_blocks, 'stage={:}, {:} vs {:}'.format(stage, cur_block_choices,
-                                                                                         layer_blocks)
-            self.message += "\nstage={:} ::: depth-block-choices={:} for {:} blocks.".format(stage, cur_block_choices,
-                                                                                             layer_blocks)
-            block_choices, xstart = [], len(self.layers)
-            for iL in range(layer_blocks):
-                iC = self.channels[-1]
-                planes = 16 * (2 ** stage)
-                stride = 2 if stage > 0 and iL == 0 else 1
-                module = block(iC, planes, stride)
-                self.channels.append(module.out_dim)
-                self.layers.append(module)
-                self.message += "\nstage={:}, ilayer={:02d}/{:02d}, block={:03d}, iC={:3d}, oC={:3d}, stride={:}".format(
-                    stage, iL, layer_blocks, len(self.layers) - 1, iC, module.out_dim, stride)
-                # added for depth
-                layer_index = len(self.layers) - 1
-                if iL + 1 in cur_block_choices: block_choices.append(layer_index)
-                if iL + 1 == layer_blocks:
-                    self.depth_info[layer_index] = {'choices': block_choices,
-                                                    'stage': stage,
-                                                    'xstart': xstart}
-        self.depth_info_list = []
-        for xend, info in self.depth_info.items():
-            self.depth_info_list.append((xend, info))
-            xstart, xstage = info['xstart'], info['stage']
-            for ilayer in range(xstart, xend + 1):
-                idx = bisect_right(info['choices'], ilayer - 1)
-                self.depth_at_i[ilayer] = (xstage, idx)
-
-        self.avgpool = nn.AvgPool2d(8)
-        self.classifier = nn.Linear(module.out_dim, num_classes)
-        self.InShape = None
-        self.tau = -1
-        self.search_mode = 'basic'
-        # assert sum(x.num_conv for x in self.layers) + 1 == depth, 'invalid depth check {:} vs {:}'.format(sum(x.num_conv for x in self.layers)+1, depth)
-
-        self.register_parameter('depth_attentions',
-                                nn.Parameter(torch.Tensor(3, get_depth_choices(layer_blocks, True))))
-        nn.init.normal_(self.depth_attentions, 0, 0.01)
-        self.apply(initialize_resnet)
-
-    def arch_parameters(self):
-        return [self.depth_attentions]
-
-    def base_parameters(self):
-        return list(self.layers.parameters()) + list(self.avgpool.parameters()) + list(self.classifier.parameters())
-
-    def get_flop(self, mode, config_dict, extra_info):
-        if config_dict is not None: config_dict = config_dict.copy()
-        # select depth
-        if mode == 'genotype':
-            with torch.no_grad():
-                depth_probs = nn.functional.softmax(self.depth_attentions, dim=1)
-                choices = torch.argmax(depth_probs, dim=1).cpu().tolist()
-        elif mode == 'max':
-            choices = [depth_probs.size(1) - 1 for _ in range(depth_probs.size(0))]
-        elif mode == 'random':
-            with torch.no_grad():
-                depth_probs = nn.functional.softmax(self.depth_attentions, dim=1)
-                choices = torch.multinomial(depth_probs, 1, False).cpu().tolist()
-        else:
-            raise ValueError('invalid mode : {:}'.format(mode))
-        selected_layers = []
-        for choice, xvalue in zip(choices, self.depth_info_list):
-            xtemp = xvalue[1]['choices'][choice] - xvalue[1]['xstart'] + 1
-            selected_layers.append(xtemp)
-        flop = 0
-        for i, layer in enumerate(self.layers):
-            if i in self.depth_at_i:
-                xstagei, xatti = self.depth_at_i[i]
-                if xatti <= choices[xstagei]:  # leave this depth
-                    flop += layer.get_flops()
-                else:
-                    flop += 0  # do not use this layer
-            else:
-                flop += layer.get_flops()
-        # the last fc layer
-        flop += self.classifier.in_features * self.classifier.out_features
-        if config_dict is None:
-            return flop / 1e6
-        else:
-            config_dict['xblocks'] = selected_layers
-            config_dict['super_type'] = 'infer-depth'
-            config_dict['estimated_FLOP'] = flop / 1e6
-            return flop / 1e6, config_dict
-
-    def get_arch_info(self):
-        string = "for depth, there are {:} attention probabilities.".format(len(self.depth_attentions))
-        string += '\n{:}'.format(self.depth_info)
-        discrepancy = []
-        with torch.no_grad():
-            for i, att in enumerate(self.depth_attentions):
-                prob = nn.functional.softmax(att, dim=0)
-                prob = prob.cpu();
-                selc = prob.argmax().item();
-                prob = prob.tolist()
-                prob = ['{:.3f}'.format(x) for x in prob]
-                xstring = '{:03d}/{:03d}-th : {:}'.format(i, len(self.depth_attentions), ' '.join(prob))
-                logt = ['{:.4f}'.format(x) for x in att.cpu().tolist()]
-                xstring += '  ||  {:17s}'.format(' '.join(logt))
-                prob = sorted([float(x) for x in prob])
-                disc = prob[-1] - prob[-2]
-                xstring += '  || discrepancy={:.2f} || select={:}/{:}'.format(disc, selc, len(prob))
-                discrepancy.append(disc)
-                string += '\n{:}'.format(xstring)
-        return string, discrepancy
-
-    def set_tau(self, tau_max, tau_min, epoch_ratio):
-        assert epoch_ratio >= 0 and epoch_ratio <= 1, 'invalid epoch-ratio : {:}'.format(epoch_ratio)
-        tau = tau_min + (tau_max - tau_min) * (1 + math.cos(math.pi * epoch_ratio)) / 2
-        self.tau = tau
-
-    def get_message(self):
-        return self.message
-
-    def forward(self, inputs):
-        if self.search_mode == 'basic':
-            return self.basic_forward(inputs)
-        elif self.search_mode == 'search':
-            return self.search_forward(inputs)
-        else:
-            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
-
-    def search_forward(self, inputs):
-        flop_depth_probs = nn.functional.softmax(self.depth_attentions, dim=1)
-        flop_depth_probs = torch.flip(torch.cumsum(torch.flip(flop_depth_probs, [1]), 1), [1])
-        selected_depth_probs = select2withP(self.depth_attentions, self.tau, True)
-
-        x, flops = inputs, []
-        feature_maps = []
-        for i, layer in enumerate(self.layers):
-            layer_i = layer(x)
-            feature_maps.append(layer_i)
-            if i in self.depth_info:  # aggregate the information
-                choices = self.depth_info[i]['choices']
-                xstagei = self.depth_info[i]['stage']
-                possible_tensors = []
-                for tempi, A in enumerate(choices):
-                    xtensor = feature_maps[A]
-                    possible_tensors.append(xtensor)
-                weighted_sum = sum(xtensor * W for xtensor, W in zip(possible_tensors, selected_depth_probs[xstagei]))
-                x = weighted_sum
-            else:
-                x = layer_i
-
-            if i in self.depth_at_i:
-                xstagei, xatti = self.depth_at_i[i]
-                # print ('layer-{:03d}, stage={:}, att={:}, prob={:}, flop={:}'.format(i, xstagei, xatti, flop_depth_probs[xstagei, xatti].item(), layer.get_flops(1e6)))
-                x_expected_flop = flop_depth_probs[xstagei, xatti] * layer.get_flops(1e6)
-            else:
-                x_expected_flop = layer.get_flops(1e6)
-            flops.append(x_expected_flop)
-        flops.append((self.classifier.in_features * self.classifier.out_features * 1.0 / 1e6))
-
-        features = self.avgpool(x)
-        features = features.view(features.size(0), -1)
-        logits = linear_forward(features, self.classifier)
-        return logits, torch.stack([sum(flops)])
-
-    def basic_forward(self, inputs):
-        if self.InShape is None: self.InShape = (inputs.size(-2), inputs.size(-1))
-        x = inputs
-        for i, layer in enumerate(self.layers):
-            x = layer(x)
-        features = self.avgpool(x)
-        features = features.view(features.size(0), -1)
-        logits = self.classifier(features)
-        return features, logits
+##################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
+##################################################
+import math, torch
+from collections import OrderedDict
+from bisect import bisect_right
+import torch.nn as nn
+from ..initialization import initialize_resnet
+from ..SharedUtils import additive_func
+from .SoftSelect import select2withP, ChannelWiseInter
+from .SoftSelect import linear_forward
+from .SoftSelect import get_width_choices
+
+
+def get_depth_choices(nDepth, return_num):
+    if nDepth == 2:
+        choices = (1, 2)
+    elif nDepth == 3:
+        choices = (1, 2, 3)
+    elif nDepth > 3:
+        choices = list(range(1, nDepth + 1, 2))
+        if choices[-1] < nDepth: choices.append(nDepth)
+    else:
+        raise ValueError('invalid nDepth : {:}'.format(nDepth))
+    if return_num:
+        return len(choices)
+    else:
+        return choices
+
+
+class ConvBNReLU(nn.Module):
+    num_conv = 1
+
+    def __init__(self, nIn, nOut, kernel, stride, padding, bias, has_avg, has_bn, has_relu):
+        super(ConvBNReLU, self).__init__()
+        self.InShape = None
+        self.OutShape = None
+        self.choices = get_width_choices(nOut)
+        self.register_buffer('choices_tensor', torch.Tensor(self.choices))
+
+        if has_avg:
+            self.avg = nn.AvgPool2d(kernel_size=2, stride=2, padding=0)
+        else:
+            self.avg = None
+        self.conv = nn.Conv2d(nIn, nOut, kernel_size=kernel, stride=stride, padding=padding, dilation=1, groups=1,
+                              bias=bias)
+        if has_bn:
+            self.bn = nn.BatchNorm2d(nOut)
+        else:
+            self.bn = None
+        if has_relu:
+            self.relu = nn.ReLU(inplace=False)
+        else:
+            self.relu = None
+        self.in_dim = nIn
+        self.out_dim = nOut
+
+    def get_flops(self, divide=1):
+        iC, oC = self.in_dim, self.out_dim
+        assert iC <= self.conv.in_channels and oC <= self.conv.out_channels, '{:} vs {:}  |  {:} vs {:}'.format(iC,
+                                                                                                                self.conv.in_channels,
+                                                                                                                oC,
+                                                                                                                self.conv.out_channels)
+        assert isinstance(self.InShape, tuple) and len(self.InShape) == 2, 'invalid in-shape : {:}'.format(self.InShape)
+        assert isinstance(self.OutShape, tuple) and len(self.OutShape) == 2, 'invalid out-shape : {:}'.format(
+            self.OutShape)
+        # conv_per_position_flops = self.conv.kernel_size[0] * self.conv.kernel_size[1] * iC * oC / self.conv.groups
+        conv_per_position_flops = (self.conv.kernel_size[0] * self.conv.kernel_size[1] * 1.0 / self.conv.groups)
+        all_positions = self.OutShape[0] * self.OutShape[1]
+        flops = (conv_per_position_flops * all_positions / divide) * iC * oC
+        if self.conv.bias is not None: flops += all_positions / divide
+        return flops
+
+    def forward(self, inputs):
+        if self.avg:
+            out = self.avg(inputs)
+        else:
+            out = inputs
+        conv = self.conv(out)
+        if self.bn:
+            out = self.bn(conv)
+        else:
+            out = conv
+        if self.relu:
+            out = self.relu(out)
+        else:
+            out = out
+        if self.InShape is None:
+            self.InShape = (inputs.size(-2), inputs.size(-1))
+            self.OutShape = (out.size(-2), out.size(-1))
+        return out
+
+
+class ResNetBasicblock(nn.Module):
+    expansion = 1
+    num_conv = 2
+
+    def __init__(self, inplanes, planes, stride):
+        super(ResNetBasicblock, self).__init__()
+        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
+        self.conv_a = ConvBNReLU(inplanes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
+        self.conv_b = ConvBNReLU(planes, planes, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=False)
+        if stride == 2:
+            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=True, has_bn=False, has_relu=False)
+        elif inplanes != planes:
+            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=False)
+        else:
+            self.downsample = None
+        self.out_dim = planes
+        self.search_mode = 'basic'
+
+    def get_flops(self, divide=1):
+        flop_A = self.conv_a.get_flops(divide)
+        flop_B = self.conv_b.get_flops(divide)
+        if hasattr(self.downsample, 'get_flops'):
+            flop_C = self.downsample.get_flops(divide)
+        else:
+            flop_C = 0
+        return flop_A + flop_B + flop_C
+
+    def forward(self, inputs):
+        basicblock = self.conv_a(inputs)
+        basicblock = self.conv_b(basicblock)
+        if self.downsample is not None:
+            residual = self.downsample(inputs)
+        else:
+            residual = inputs
+        out = additive_func(residual, basicblock)
+        return nn.functional.relu(out, inplace=True)
+
+
+class ResNetBottleneck(nn.Module):
+    expansion = 4
+    num_conv = 3
+
+    def __init__(self, inplanes, planes, stride):
+        super(ResNetBottleneck, self).__init__()
+        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
+        self.conv_1x1 = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=True)
+        self.conv_3x3 = ConvBNReLU(planes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
+        self.conv_1x4 = ConvBNReLU(planes, planes * self.expansion, 1, 1, 0, False, has_avg=False, has_bn=True,
+                                   has_relu=False)
+        if stride == 2:
+            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, has_avg=True, has_bn=False,
+                                         has_relu=False)
+        elif inplanes != planes * self.expansion:
+            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, has_avg=False, has_bn=True,
+                                         has_relu=False)
+        else:
+            self.downsample = None
+        self.out_dim = planes * self.expansion
+        self.search_mode = 'basic'
+
+    def get_range(self):
+        return self.conv_1x1.get_range() + self.conv_3x3.get_range() + self.conv_1x4.get_range()
+
+    def get_flops(self, divide):
+        flop_A = self.conv_1x1.get_flops(divide)
+        flop_B = self.conv_3x3.get_flops(divide)
+        flop_C = self.conv_1x4.get_flops(divide)
+        if hasattr(self.downsample, 'get_flops'):
+            flop_D = self.downsample.get_flops(divide)
+        else:
+            flop_D = 0
+        return flop_A + flop_B + flop_C + flop_D
+
+    def forward(self, inputs):
+        bottleneck = self.conv_1x1(inputs)
+        bottleneck = self.conv_3x3(bottleneck)
+        bottleneck = self.conv_1x4(bottleneck)
+        if self.downsample is not None:
+            residual = self.downsample(inputs)
+        else:
+            residual = inputs
+        out = additive_func(residual, bottleneck)
+        return nn.functional.relu(out, inplace=True)
+
+
+class SearchDepthCifarResNet(nn.Module):
+
+    def __init__(self, block_name, depth, num_classes):
+        super(SearchDepthCifarResNet, self).__init__()
+
+        # Model type specifies number of layers for CIFAR-10 and CIFAR-100 model
+        if block_name == 'ResNetBasicblock':
+            block = ResNetBasicblock
+            assert (depth - 2) % 6 == 0, 'depth should be one of 20, 32, 44, 56, 110'
+            layer_blocks = (depth - 2) // 6
+        elif block_name == 'ResNetBottleneck':
+            block = ResNetBottleneck
+            assert (depth - 2) % 9 == 0, 'depth should be one of 164'
+            layer_blocks = (depth - 2) // 9
+        else:
+            raise ValueError('invalid block : {:}'.format(block_name))
+
+        self.message = 'SearchShapeCifarResNet : Depth : {:} , Layers for each block : {:}'.format(depth, layer_blocks)
+        self.num_classes = num_classes
+        self.channels = [16]
+        self.layers = nn.ModuleList([ConvBNReLU(3, 16, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=True)])
+        self.InShape = None
+        self.depth_info = OrderedDict()
+        self.depth_at_i = OrderedDict()
+        for stage in range(3):
+            cur_block_choices = get_depth_choices(layer_blocks, False)
+            assert cur_block_choices[-1] == layer_blocks, 'stage={:}, {:} vs {:}'.format(stage, cur_block_choices,
+                                                                                         layer_blocks)
+            self.message += "\nstage={:} ::: depth-block-choices={:} for {:} blocks.".format(stage, cur_block_choices,
+                                                                                             layer_blocks)
+            block_choices, xstart = [], len(self.layers)
+            for iL in range(layer_blocks):
+                iC = self.channels[-1]
+                planes = 16 * (2 ** stage)
+                stride = 2 if stage > 0 and iL == 0 else 1
+                module = block(iC, planes, stride)
+                self.channels.append(module.out_dim)
+                self.layers.append(module)
+                self.message += "\nstage={:}, ilayer={:02d}/{:02d}, block={:03d}, iC={:3d}, oC={:3d}, stride={:}".format(
+                    stage, iL, layer_blocks, len(self.layers) - 1, iC, module.out_dim, stride)
+                # added for depth
+                layer_index = len(self.layers) - 1
+                if iL + 1 in cur_block_choices: block_choices.append(layer_index)
+                if iL + 1 == layer_blocks:
+                    self.depth_info[layer_index] = {'choices': block_choices,
+                                                    'stage': stage,
+                                                    'xstart': xstart}
+        self.depth_info_list = []
+        for xend, info in self.depth_info.items():
+            self.depth_info_list.append((xend, info))
+            xstart, xstage = info['xstart'], info['stage']
+            for ilayer in range(xstart, xend + 1):
+                idx = bisect_right(info['choices'], ilayer - 1)
+                self.depth_at_i[ilayer] = (xstage, idx)
+
+        self.avgpool = nn.AvgPool2d(8)
+        self.classifier = nn.Linear(module.out_dim, num_classes)
+        self.InShape = None
+        self.tau = -1
+        self.search_mode = 'basic'
+        # assert sum(x.num_conv for x in self.layers) + 1 == depth, 'invalid depth check {:} vs {:}'.format(sum(x.num_conv for x in self.layers)+1, depth)
+
+        self.register_parameter('depth_attentions',
+                                nn.Parameter(torch.Tensor(3, get_depth_choices(layer_blocks, True))))
+        nn.init.normal_(self.depth_attentions, 0, 0.01)
+        self.apply(initialize_resnet)
+
+    def arch_parameters(self):
+        return [self.depth_attentions]
+
+    def base_parameters(self):
+        return list(self.layers.parameters()) + list(self.avgpool.parameters()) + list(self.classifier.parameters())
+
+    def get_flop(self, mode, config_dict, extra_info):
+        if config_dict is not None: config_dict = config_dict.copy()
+        # select depth
+        if mode == 'genotype':
+            with torch.no_grad():
+                depth_probs = nn.functional.softmax(self.depth_attentions, dim=1)
+                choices = torch.argmax(depth_probs, dim=1).cpu().tolist()
+        elif mode == 'max':
+            choices = [depth_probs.size(1) - 1 for _ in range(depth_probs.size(0))]
+        elif mode == 'random':
+            with torch.no_grad():
+                depth_probs = nn.functional.softmax(self.depth_attentions, dim=1)
+                choices = torch.multinomial(depth_probs, 1, False).cpu().tolist()
+        else:
+            raise ValueError('invalid mode : {:}'.format(mode))
+        selected_layers = []
+        for choice, xvalue in zip(choices, self.depth_info_list):
+            xtemp = xvalue[1]['choices'][choice] - xvalue[1]['xstart'] + 1
+            selected_layers.append(xtemp)
+        flop = 0
+        for i, layer in enumerate(self.layers):
+            if i in self.depth_at_i:
+                xstagei, xatti = self.depth_at_i[i]
+                if xatti <= choices[xstagei]:  # leave this depth
+                    flop += layer.get_flops()
+                else:
+                    flop += 0  # do not use this layer
+            else:
+                flop += layer.get_flops()
+        # the last fc layer
+        flop += self.classifier.in_features * self.classifier.out_features
+        if config_dict is None:
+            return flop / 1e6
+        else:
+            config_dict['xblocks'] = selected_layers
+            config_dict['super_type'] = 'infer-depth'
+            config_dict['estimated_FLOP'] = flop / 1e6
+            return flop / 1e6, config_dict
+
+    def get_arch_info(self):
+        string = "for depth, there are {:} attention probabilities.".format(len(self.depth_attentions))
+        string += '\n{:}'.format(self.depth_info)
+        discrepancy = []
+        with torch.no_grad():
+            for i, att in enumerate(self.depth_attentions):
+                prob = nn.functional.softmax(att, dim=0)
+                prob = prob.cpu();
+                selc = prob.argmax().item();
+                prob = prob.tolist()
+                prob = ['{:.3f}'.format(x) for x in prob]
+                xstring = '{:03d}/{:03d}-th : {:}'.format(i, len(self.depth_attentions), ' '.join(prob))
+                logt = ['{:.4f}'.format(x) for x in att.cpu().tolist()]
+                xstring += '  ||  {:17s}'.format(' '.join(logt))
+                prob = sorted([float(x) for x in prob])
+                disc = prob[-1] - prob[-2]
+                xstring += '  || discrepancy={:.2f} || select={:}/{:}'.format(disc, selc, len(prob))
+                discrepancy.append(disc)
+                string += '\n{:}'.format(xstring)
+        return string, discrepancy
+
+    def set_tau(self, tau_max, tau_min, epoch_ratio):
+        assert epoch_ratio >= 0 and epoch_ratio <= 1, 'invalid epoch-ratio : {:}'.format(epoch_ratio)
+        tau = tau_min + (tau_max - tau_min) * (1 + math.cos(math.pi * epoch_ratio)) / 2
+        self.tau = tau
+
+    def get_message(self):
+        return self.message
+
+    def forward(self, inputs):
+        if self.search_mode == 'basic':
+            return self.basic_forward(inputs)
+        elif self.search_mode == 'search':
+            return self.search_forward(inputs)
+        else:
+            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
+
+    def search_forward(self, inputs):
+        flop_depth_probs = nn.functional.softmax(self.depth_attentions, dim=1)
+        flop_depth_probs = torch.flip(torch.cumsum(torch.flip(flop_depth_probs, [1]), 1), [1])
+        selected_depth_probs = select2withP(self.depth_attentions, self.tau, True)
+
+        x, flops = inputs, []
+        feature_maps = []
+        for i, layer in enumerate(self.layers):
+            layer_i = layer(x)
+            feature_maps.append(layer_i)
+            if i in self.depth_info:  # aggregate the information
+                choices = self.depth_info[i]['choices']
+                xstagei = self.depth_info[i]['stage']
+                possible_tensors = []
+                for tempi, A in enumerate(choices):
+                    xtensor = feature_maps[A]
+                    possible_tensors.append(xtensor)
+                weighted_sum = sum(xtensor * W for xtensor, W in zip(possible_tensors, selected_depth_probs[xstagei]))
+                x = weighted_sum
+            else:
+                x = layer_i
+
+            if i in self.depth_at_i:
+                xstagei, xatti = self.depth_at_i[i]
+                # print ('layer-{:03d}, stage={:}, att={:}, prob={:}, flop={:}'.format(i, xstagei, xatti, flop_depth_probs[xstagei, xatti].item(), layer.get_flops(1e6)))
+                x_expected_flop = flop_depth_probs[xstagei, xatti] * layer.get_flops(1e6)
+            else:
+                x_expected_flop = layer.get_flops(1e6)
+            flops.append(x_expected_flop)
+        flops.append((self.classifier.in_features * self.classifier.out_features * 1.0 / 1e6))
+
+        features = self.avgpool(x)
+        features = features.view(features.size(0), -1)
+        logits = linear_forward(features, self.classifier)
+        return logits, torch.stack([sum(flops)])
+
+    def basic_forward(self, inputs):
+        if self.InShape is None: self.InShape = (inputs.size(-2), inputs.size(-1))
+        x = inputs
+        for i, layer in enumerate(self.layers):
+            x = layer(x)
+        features = self.avgpool(x)
+        features = features.view(features.size(0), -1)
+        logits = self.classifier(features)
+        return features, logits
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchCifarResNet_width.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchCifarResNet_width.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,440 +1,440 @@
-##################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
-##################################################
-import math, torch
-import torch.nn as nn
-from ..initialization import initialize_resnet
-from ..SharedUtils import additive_func
-from .SoftSelect import select2withP, ChannelWiseInter
-from .SoftSelect import linear_forward
-from .SoftSelect import get_width_choices as get_choices
-
-
-def conv_forward(inputs, conv, choices):
-    iC = conv.in_channels
-    fill_size = list(inputs.size())
-    fill_size[1] = iC - fill_size[1]
-    filled = torch.zeros(fill_size, device=inputs.device)
-    xinputs = torch.cat((inputs, filled), dim=1)
-    outputs = conv(xinputs)
-    selecteds = [outputs[:, :oC] for oC in choices]
-    return selecteds
-
-
-class ConvBNReLU(nn.Module):
-    num_conv = 1
-
-    def __init__(self, nIn, nOut, kernel, stride, padding, bias, has_avg, has_bn, has_relu):
-        super(ConvBNReLU, self).__init__()
-        self.InShape = None
-        self.OutShape = None
-        self.choices = get_choices(nOut)
-        self.register_buffer('choices_tensor', torch.Tensor(self.choices))
-
-        if has_avg:
-            self.avg = nn.AvgPool2d(kernel_size=2, stride=2, padding=0)
-        else:
-            self.avg = None
-        self.conv = nn.Conv2d(nIn, nOut, kernel_size=kernel, stride=stride, padding=padding, dilation=1, groups=1,
-                              bias=bias)
-        # if has_bn  : self.bn  = nn.BatchNorm2d(nOut)
-        # else       : self.bn  = None
-        self.has_bn = has_bn
-        self.BNs = nn.ModuleList()
-        for i, _out in enumerate(self.choices):
-            self.BNs.append(nn.BatchNorm2d(_out))
-        if has_relu:
-            self.relu = nn.ReLU(inplace=True)
-        else:
-            self.relu = None
-        self.in_dim = nIn
-        self.out_dim = nOut
-        self.search_mode = 'basic'
-
-    def get_flops(self, channels, check_range=True, divide=1):
-        iC, oC = channels
-        if check_range: assert iC <= self.conv.in_channels and oC <= self.conv.out_channels, '{:} vs {:}  |  {:} vs {:}'.format(
-            iC, self.conv.in_channels, oC, self.conv.out_channels)
-        assert isinstance(self.InShape, tuple) and len(self.InShape) == 2, 'invalid in-shape : {:}'.format(self.InShape)
-        assert isinstance(self.OutShape, tuple) and len(self.OutShape) == 2, 'invalid out-shape : {:}'.format(
-            self.OutShape)
-        # conv_per_position_flops = self.conv.kernel_size[0] * self.conv.kernel_size[1] * iC * oC / self.conv.groups
-        conv_per_position_flops = (self.conv.kernel_size[0] * self.conv.kernel_size[1] * 1.0 / self.conv.groups)
-        all_positions = self.OutShape[0] * self.OutShape[1]
-        flops = (conv_per_position_flops * all_positions / divide) * iC * oC
-        if self.conv.bias is not None: flops += all_positions / divide
-        return flops
-
-    def get_range(self):
-        return [self.choices]
-
-    def forward(self, inputs):
-        if self.search_mode == 'basic':
-            return self.basic_forward(inputs)
-        elif self.search_mode == 'search':
-            return self.search_forward(inputs)
-        else:
-            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
-
-    def search_forward(self, tuple_inputs):
-        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
-            type(tuple_inputs))
-        inputs, expected_inC, probability, index, prob = tuple_inputs
-        index, prob = torch.squeeze(index).tolist(), torch.squeeze(prob)
-        probability = torch.squeeze(probability)
-        assert len(index) == 2, 'invalid length : {:}'.format(index)
-        # compute expected flop
-        # coordinates   = torch.arange(self.x_range[0], self.x_range[1]+1).type_as(probability)
-        expected_outC = (self.choices_tensor * probability).sum()
-        expected_flop = self.get_flops([expected_inC, expected_outC], False, 1e6)
-        if self.avg:
-            out = self.avg(inputs)
-        else:
-            out = inputs
-        # convolutional layer
-        out_convs = conv_forward(out, self.conv, [self.choices[i] for i in index])
-        out_bns = [self.BNs[idx](out_conv) for idx, out_conv in zip(index, out_convs)]
-        # merge
-        out_channel = max([x.size(1) for x in out_bns])
-        outA = ChannelWiseInter(out_bns[0], out_channel)
-        outB = ChannelWiseInter(out_bns[1], out_channel)
-        out = outA * prob[0] + outB * prob[1]
-        # out = additive_func(out_bns[0]*prob[0], out_bns[1]*prob[1])
-
-        if self.relu:
-            out = self.relu(out)
-        else:
-            out = out
-        return out, expected_outC, expected_flop
-
-    def basic_forward(self, inputs):
-        if self.avg:
-            out = self.avg(inputs)
-        else:
-            out = inputs
-        conv = self.conv(out)
-        if self.has_bn:
-            out = self.BNs[-1](conv)
-        else:
-            out = conv
-        if self.relu:
-            out = self.relu(out)
-        else:
-            out = out
-        if self.InShape is None:
-            self.InShape = (inputs.size(-2), inputs.size(-1))
-            self.OutShape = (out.size(-2), out.size(-1))
-        return out
-
-
-class ResNetBasicblock(nn.Module):
-    expansion = 1
-    num_conv = 2
-
-    def __init__(self, inplanes, planes, stride):
-        super(ResNetBasicblock, self).__init__()
-        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
-        self.conv_a = ConvBNReLU(inplanes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
-        self.conv_b = ConvBNReLU(planes, planes, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=False)
-        if stride == 2:
-            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=True, has_bn=False, has_relu=False)
-        elif inplanes != planes:
-            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=False)
-        else:
-            self.downsample = None
-        self.out_dim = planes
-        self.search_mode = 'basic'
-
-    def get_range(self):
-        return self.conv_a.get_range() + self.conv_b.get_range()
-
-    def get_flops(self, channels):
-        assert len(channels) == 3, 'invalid channels : {:}'.format(channels)
-        flop_A = self.conv_a.get_flops([channels[0], channels[1]])
-        flop_B = self.conv_b.get_flops([channels[1], channels[2]])
-        if hasattr(self.downsample, 'get_flops'):
-            flop_C = self.downsample.get_flops([channels[0], channels[-1]])
-        else:
-            flop_C = 0
-        if channels[0] != channels[
-            -1] and self.downsample is None:  # this short-cut will be added during the infer-train
-            flop_C = channels[0] * channels[-1] * self.conv_b.OutShape[0] * self.conv_b.OutShape[1]
-        return flop_A + flop_B + flop_C
-
-    def forward(self, inputs):
-        if self.search_mode == 'basic':
-            return self.basic_forward(inputs)
-        elif self.search_mode == 'search':
-            return self.search_forward(inputs)
-        else:
-            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
-
-    def search_forward(self, tuple_inputs):
-        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
-            type(tuple_inputs))
-        inputs, expected_inC, probability, indexes, probs = tuple_inputs
-        assert indexes.size(0) == 2 and probs.size(0) == 2 and probability.size(0) == 2
-        out_a, expected_inC_a, expected_flop_a = self.conv_a(
-            (inputs, expected_inC, probability[0], indexes[0], probs[0]))
-        out_b, expected_inC_b, expected_flop_b = self.conv_b(
-            (out_a, expected_inC_a, probability[1], indexes[1], probs[1]))
-        if self.downsample is not None:
-            residual, _, expected_flop_c = self.downsample((inputs, expected_inC, probability[1], indexes[1], probs[1]))
-        else:
-            residual, expected_flop_c = inputs, 0
-        out = additive_func(residual, out_b)
-        return nn.functional.relu(out, inplace=True), expected_inC_b, sum(
-            [expected_flop_a, expected_flop_b, expected_flop_c])
-
-    def basic_forward(self, inputs):
-        basicblock = self.conv_a(inputs)
-        basicblock = self.conv_b(basicblock)
-        if self.downsample is not None:
-            residual = self.downsample(inputs)
-        else:
-            residual = inputs
-        out = additive_func(residual, basicblock)
-        return nn.functional.relu(out, inplace=True)
-
-
-class ResNetBottleneck(nn.Module):
-    expansion = 4
-    num_conv = 3
-
-    def __init__(self, inplanes, planes, stride):
-        super(ResNetBottleneck, self).__init__()
-        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
-        self.conv_1x1 = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=True)
-        self.conv_3x3 = ConvBNReLU(planes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
-        self.conv_1x4 = ConvBNReLU(planes, planes * self.expansion, 1, 1, 0, False, has_avg=False, has_bn=True,
-                                   has_relu=False)
-        if stride == 2:
-            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, has_avg=True, has_bn=False,
-                                         has_relu=False)
-        elif inplanes != planes * self.expansion:
-            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, has_avg=False, has_bn=True,
-                                         has_relu=False)
-        else:
-            self.downsample = None
-        self.out_dim = planes * self.expansion
-        self.search_mode = 'basic'
-
-    def get_range(self):
-        return self.conv_1x1.get_range() + self.conv_3x3.get_range() + self.conv_1x4.get_range()
-
-    def get_flops(self, channels):
-        assert len(channels) == 4, 'invalid channels : {:}'.format(channels)
-        flop_A = self.conv_1x1.get_flops([channels[0], channels[1]])
-        flop_B = self.conv_3x3.get_flops([channels[1], channels[2]])
-        flop_C = self.conv_1x4.get_flops([channels[2], channels[3]])
-        if hasattr(self.downsample, 'get_flops'):
-            flop_D = self.downsample.get_flops([channels[0], channels[-1]])
-        else:
-            flop_D = 0
-        if channels[0] != channels[
-            -1] and self.downsample is None:  # this short-cut will be added during the infer-train
-            flop_D = channels[0] * channels[-1] * self.conv_1x4.OutShape[0] * self.conv_1x4.OutShape[1]
-        return flop_A + flop_B + flop_C + flop_D
-
-    def forward(self, inputs):
-        if self.search_mode == 'basic':
-            return self.basic_forward(inputs)
-        elif self.search_mode == 'search':
-            return self.search_forward(inputs)
-        else:
-            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
-
-    def basic_forward(self, inputs):
-        bottleneck = self.conv_1x1(inputs)
-        bottleneck = self.conv_3x3(bottleneck)
-        bottleneck = self.conv_1x4(bottleneck)
-        if self.downsample is not None:
-            residual = self.downsample(inputs)
-        else:
-            residual = inputs
-        out = additive_func(residual, bottleneck)
-        return nn.functional.relu(out, inplace=True)
-
-    def search_forward(self, tuple_inputs):
-        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
-            type(tuple_inputs))
-        inputs, expected_inC, probability, indexes, probs = tuple_inputs
-        assert indexes.size(0) == 3 and probs.size(0) == 3 and probability.size(0) == 3
-        out_1x1, expected_inC_1x1, expected_flop_1x1 = self.conv_1x1(
-            (inputs, expected_inC, probability[0], indexes[0], probs[0]))
-        out_3x3, expected_inC_3x3, expected_flop_3x3 = self.conv_3x3(
-            (out_1x1, expected_inC_1x1, probability[1], indexes[1], probs[1]))
-        out_1x4, expected_inC_1x4, expected_flop_1x4 = self.conv_1x4(
-            (out_3x3, expected_inC_3x3, probability[2], indexes[2], probs[2]))
-        if self.downsample is not None:
-            residual, _, expected_flop_c = self.downsample((inputs, expected_inC, probability[2], indexes[2], probs[2]))
-        else:
-            residual, expected_flop_c = inputs, 0
-        out = additive_func(residual, out_1x4)
-        return nn.functional.relu(out, inplace=True), expected_inC_1x4, sum(
-            [expected_flop_1x1, expected_flop_3x3, expected_flop_1x4, expected_flop_c])
-
-
-class SearchWidthCifarResNet(nn.Module):
-
-    def __init__(self, block_name, depth, num_classes):
-        super(SearchWidthCifarResNet, self).__init__()
-
-        # Model type specifies number of layers for CIFAR-10 and CIFAR-100 model
-        if block_name == 'ResNetBasicblock':
-            block = ResNetBasicblock
-            assert (depth - 2) % 6 == 0, 'depth should be one of 20, 32, 44, 56, 110'
-            layer_blocks = (depth - 2) // 6
-        elif block_name == 'ResNetBottleneck':
-            block = ResNetBottleneck
-            assert (depth - 2) % 9 == 0, 'depth should be one of 164'
-            layer_blocks = (depth - 2) // 9
-        else:
-            raise ValueError('invalid block : {:}'.format(block_name))
-
-        self.message = 'SearchWidthCifarResNet : Depth : {:} , Layers for each block : {:}'.format(depth, layer_blocks)
-        self.num_classes = num_classes
-        self.channels = [16]
-        self.layers = nn.ModuleList([ConvBNReLU(3, 16, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=True)])
-        self.InShape = None
-        for stage in range(3):
-            for iL in range(layer_blocks):
-                iC = self.channels[-1]
-                planes = 16 * (2 ** stage)
-                stride = 2 if stage > 0 and iL == 0 else 1
-                module = block(iC, planes, stride)
-                self.channels.append(module.out_dim)
-                self.layers.append(module)
-                self.message += "\nstage={:}, ilayer={:02d}/{:02d}, block={:03d}, iC={:3d}, oC={:3d}, stride={:}".format(
-                    stage, iL, layer_blocks, len(self.layers) - 1, iC, module.out_dim, stride)
-
-        self.avgpool = nn.AvgPool2d(8)
-        self.classifier = nn.Linear(module.out_dim, num_classes)
-        self.InShape = None
-        self.tau = -1
-        self.search_mode = 'basic'
-        # assert sum(x.num_conv for x in self.layers) + 1 == depth, 'invalid depth check {:} vs {:}'.format(sum(x.num_conv for x in self.layers)+1, depth)
-
-        # parameters for width
-        self.Ranges = []
-        self.layer2indexRange = []
-        for i, layer in enumerate(self.layers):
-            start_index = len(self.Ranges)
-            self.Ranges += layer.get_range()
-            self.layer2indexRange.append((start_index, len(self.Ranges)))
-        assert len(self.Ranges) + 1 == depth, 'invalid depth check {:} vs {:}'.format(len(self.Ranges) + 1, depth)
-
-        self.register_parameter('width_attentions', nn.Parameter(torch.Tensor(len(self.Ranges), get_choices(None))))
-        nn.init.normal_(self.width_attentions, 0, 0.01)
-        self.apply(initialize_resnet)
-
-    def arch_parameters(self):
-        return [self.width_attentions]
-
-    def base_parameters(self):
-        return list(self.layers.parameters()) + list(self.avgpool.parameters()) + list(self.classifier.parameters())
-
-    def get_flop(self, mode, config_dict, extra_info):
-        if config_dict is not None: config_dict = config_dict.copy()
-        # weights = [F.softmax(x, dim=0) for x in self.width_attentions]
-        channels = [3]
-        for i, weight in enumerate(self.width_attentions):
-            if mode == 'genotype':
-                with torch.no_grad():
-                    probe = nn.functional.softmax(weight, dim=0)
-                    C = self.Ranges[i][torch.argmax(probe).item()]
-            elif mode == 'max':
-                C = self.Ranges[i][-1]
-            elif mode == 'fix':
-                C = int(math.sqrt(extra_info) * self.Ranges[i][-1])
-            elif mode == 'random':
-                assert isinstance(extra_info, float), 'invalid extra_info : {:}'.format(extra_info)
-                with torch.no_grad():
-                    prob = nn.functional.softmax(weight, dim=0)
-                    approximate_C = int(math.sqrt(extra_info) * self.Ranges[i][-1])
-                    for j in range(prob.size(0)):
-                        prob[j] = 1 / (abs(j - (approximate_C - self.Ranges[i][j])) + 0.2)
-                    C = self.Ranges[i][torch.multinomial(prob, 1, False).item()]
-            else:
-                raise ValueError('invalid mode : {:}'.format(mode))
-            channels.append(C)
-        flop = 0
-        for i, layer in enumerate(self.layers):
-            s, e = self.layer2indexRange[i]
-            xchl = tuple(channels[s:e + 1])
-            flop += layer.get_flops(xchl)
-        # the last fc layer
-        flop += channels[-1] * self.classifier.out_features
-        if config_dict is None:
-            return flop / 1e6
-        else:
-            config_dict['xchannels'] = channels
-            config_dict['super_type'] = 'infer-width'
-            config_dict['estimated_FLOP'] = flop / 1e6
-            return flop / 1e6, config_dict
-
-    def get_arch_info(self):
-        string = "for width, there are {:} attention probabilities.".format(len(self.width_attentions))
-        discrepancy = []
-        with torch.no_grad():
-            for i, att in enumerate(self.width_attentions):
-                prob = nn.functional.softmax(att, dim=0)
-                prob = prob.cpu();
-                selc = prob.argmax().item();
-                prob = prob.tolist()
-                prob = ['{:.3f}'.format(x) for x in prob]
-                xstring = '{:03d}/{:03d}-th : {:}'.format(i, len(self.width_attentions), ' '.join(prob))
-                logt = ['{:.3f}'.format(x) for x in att.cpu().tolist()]
-                xstring += '  ||  {:52s}'.format(' '.join(logt))
-                prob = sorted([float(x) for x in prob])
-                disc = prob[-1] - prob[-2]
-                xstring += '  || dis={:.2f} || select={:}/{:}'.format(disc, selc, len(prob))
-                discrepancy.append(disc)
-                string += '\n{:}'.format(xstring)
-        return string, discrepancy
-
-    def set_tau(self, tau_max, tau_min, epoch_ratio):
-        assert epoch_ratio >= 0 and epoch_ratio <= 1, 'invalid epoch-ratio : {:}'.format(epoch_ratio)
-        tau = tau_min + (tau_max - tau_min) * (1 + math.cos(math.pi * epoch_ratio)) / 2
-        self.tau = tau
-
-    def get_message(self):
-        return self.message
-
-    def forward(self, inputs):
-        if self.search_mode == 'basic':
-            return self.basic_forward(inputs)
-        elif self.search_mode == 'search':
-            return self.search_forward(inputs)
-        else:
-            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
-
-    def search_forward(self, inputs):
-        flop_probs = nn.functional.softmax(self.width_attentions, dim=1)
-        selected_widths, selected_probs = select2withP(self.width_attentions, self.tau)
-        with torch.no_grad():
-            selected_widths = selected_widths.cpu()
-
-        x, last_channel_idx, expected_inC, flops = inputs, 0, 3, []
-        for i, layer in enumerate(self.layers):
-            selected_w_index = selected_widths[last_channel_idx: last_channel_idx + layer.num_conv]
-            selected_w_probs = selected_probs[last_channel_idx: last_channel_idx + layer.num_conv]
-            layer_prob = flop_probs[last_channel_idx: last_channel_idx + layer.num_conv]
-            x, expected_inC, expected_flop = layer((x, expected_inC, layer_prob, selected_w_index, selected_w_probs))
-            last_channel_idx += layer.num_conv
-            flops.append(expected_flop)
-        flops.append(expected_inC * (self.classifier.out_features * 1.0 / 1e6))
-        features = self.avgpool(x)
-        features = features.view(features.size(0), -1)
-        logits = linear_forward(features, self.classifier)
-        return logits, torch.stack([sum(flops)])
-
-    def basic_forward(self, inputs):
-        if self.InShape is None: self.InShape = (inputs.size(-2), inputs.size(-1))
-        x = inputs
-        for i, layer in enumerate(self.layers):
-            x = layer(x)
-        features = self.avgpool(x)
-        features = features.view(features.size(0), -1)
-        logits = self.classifier(features)
-        return features, logits
+##################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
+##################################################
+import math, torch
+import torch.nn as nn
+from ..initialization import initialize_resnet
+from ..SharedUtils import additive_func
+from .SoftSelect import select2withP, ChannelWiseInter
+from .SoftSelect import linear_forward
+from .SoftSelect import get_width_choices as get_choices
+
+
+def conv_forward(inputs, conv, choices):
+    iC = conv.in_channels
+    fill_size = list(inputs.size())
+    fill_size[1] = iC - fill_size[1]
+    filled = torch.zeros(fill_size, device=inputs.device)
+    xinputs = torch.cat((inputs, filled), dim=1)
+    outputs = conv(xinputs)
+    selecteds = [outputs[:, :oC] for oC in choices]
+    return selecteds
+
+
+class ConvBNReLU(nn.Module):
+    num_conv = 1
+
+    def __init__(self, nIn, nOut, kernel, stride, padding, bias, has_avg, has_bn, has_relu):
+        super(ConvBNReLU, self).__init__()
+        self.InShape = None
+        self.OutShape = None
+        self.choices = get_choices(nOut)
+        self.register_buffer('choices_tensor', torch.Tensor(self.choices))
+
+        if has_avg:
+            self.avg = nn.AvgPool2d(kernel_size=2, stride=2, padding=0)
+        else:
+            self.avg = None
+        self.conv = nn.Conv2d(nIn, nOut, kernel_size=kernel, stride=stride, padding=padding, dilation=1, groups=1,
+                              bias=bias)
+        # if has_bn  : self.bn  = nn.BatchNorm2d(nOut)
+        # else       : self.bn  = None
+        self.has_bn = has_bn
+        self.BNs = nn.ModuleList()
+        for i, _out in enumerate(self.choices):
+            self.BNs.append(nn.BatchNorm2d(_out))
+        if has_relu:
+            self.relu = nn.ReLU(inplace=True)
+        else:
+            self.relu = None
+        self.in_dim = nIn
+        self.out_dim = nOut
+        self.search_mode = 'basic'
+
+    def get_flops(self, channels, check_range=True, divide=1):
+        iC, oC = channels
+        if check_range: assert iC <= self.conv.in_channels and oC <= self.conv.out_channels, '{:} vs {:}  |  {:} vs {:}'.format(
+            iC, self.conv.in_channels, oC, self.conv.out_channels)
+        assert isinstance(self.InShape, tuple) and len(self.InShape) == 2, 'invalid in-shape : {:}'.format(self.InShape)
+        assert isinstance(self.OutShape, tuple) and len(self.OutShape) == 2, 'invalid out-shape : {:}'.format(
+            self.OutShape)
+        # conv_per_position_flops = self.conv.kernel_size[0] * self.conv.kernel_size[1] * iC * oC / self.conv.groups
+        conv_per_position_flops = (self.conv.kernel_size[0] * self.conv.kernel_size[1] * 1.0 / self.conv.groups)
+        all_positions = self.OutShape[0] * self.OutShape[1]
+        flops = (conv_per_position_flops * all_positions / divide) * iC * oC
+        if self.conv.bias is not None: flops += all_positions / divide
+        return flops
+
+    def get_range(self):
+        return [self.choices]
+
+    def forward(self, inputs):
+        if self.search_mode == 'basic':
+            return self.basic_forward(inputs)
+        elif self.search_mode == 'search':
+            return self.search_forward(inputs)
+        else:
+            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
+
+    def search_forward(self, tuple_inputs):
+        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
+            type(tuple_inputs))
+        inputs, expected_inC, probability, index, prob = tuple_inputs
+        index, prob = torch.squeeze(index).tolist(), torch.squeeze(prob)
+        probability = torch.squeeze(probability)
+        assert len(index) == 2, 'invalid length : {:}'.format(index)
+        # compute expected flop
+        # coordinates   = torch.arange(self.x_range[0], self.x_range[1]+1).type_as(probability)
+        expected_outC = (self.choices_tensor * probability).sum()
+        expected_flop = self.get_flops([expected_inC, expected_outC], False, 1e6)
+        if self.avg:
+            out = self.avg(inputs)
+        else:
+            out = inputs
+        # convolutional layer
+        out_convs = conv_forward(out, self.conv, [self.choices[i] for i in index])
+        out_bns = [self.BNs[idx](out_conv) for idx, out_conv in zip(index, out_convs)]
+        # merge
+        out_channel = max([x.size(1) for x in out_bns])
+        outA = ChannelWiseInter(out_bns[0], out_channel)
+        outB = ChannelWiseInter(out_bns[1], out_channel)
+        out = outA * prob[0] + outB * prob[1]
+        # out = additive_func(out_bns[0]*prob[0], out_bns[1]*prob[1])
+
+        if self.relu:
+            out = self.relu(out)
+        else:
+            out = out
+        return out, expected_outC, expected_flop
+
+    def basic_forward(self, inputs):
+        if self.avg:
+            out = self.avg(inputs)
+        else:
+            out = inputs
+        conv = self.conv(out)
+        if self.has_bn:
+            out = self.BNs[-1](conv)
+        else:
+            out = conv
+        if self.relu:
+            out = self.relu(out)
+        else:
+            out = out
+        if self.InShape is None:
+            self.InShape = (inputs.size(-2), inputs.size(-1))
+            self.OutShape = (out.size(-2), out.size(-1))
+        return out
+
+
+class ResNetBasicblock(nn.Module):
+    expansion = 1
+    num_conv = 2
+
+    def __init__(self, inplanes, planes, stride):
+        super(ResNetBasicblock, self).__init__()
+        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
+        self.conv_a = ConvBNReLU(inplanes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
+        self.conv_b = ConvBNReLU(planes, planes, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=False)
+        if stride == 2:
+            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=True, has_bn=False, has_relu=False)
+        elif inplanes != planes:
+            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=False)
+        else:
+            self.downsample = None
+        self.out_dim = planes
+        self.search_mode = 'basic'
+
+    def get_range(self):
+        return self.conv_a.get_range() + self.conv_b.get_range()
+
+    def get_flops(self, channels):
+        assert len(channels) == 3, 'invalid channels : {:}'.format(channels)
+        flop_A = self.conv_a.get_flops([channels[0], channels[1]])
+        flop_B = self.conv_b.get_flops([channels[1], channels[2]])
+        if hasattr(self.downsample, 'get_flops'):
+            flop_C = self.downsample.get_flops([channels[0], channels[-1]])
+        else:
+            flop_C = 0
+        if channels[0] != channels[
+            -1] and self.downsample is None:  # this short-cut will be added during the infer-train
+            flop_C = channels[0] * channels[-1] * self.conv_b.OutShape[0] * self.conv_b.OutShape[1]
+        return flop_A + flop_B + flop_C
+
+    def forward(self, inputs):
+        if self.search_mode == 'basic':
+            return self.basic_forward(inputs)
+        elif self.search_mode == 'search':
+            return self.search_forward(inputs)
+        else:
+            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
+
+    def search_forward(self, tuple_inputs):
+        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
+            type(tuple_inputs))
+        inputs, expected_inC, probability, indexes, probs = tuple_inputs
+        assert indexes.size(0) == 2 and probs.size(0) == 2 and probability.size(0) == 2
+        out_a, expected_inC_a, expected_flop_a = self.conv_a(
+            (inputs, expected_inC, probability[0], indexes[0], probs[0]))
+        out_b, expected_inC_b, expected_flop_b = self.conv_b(
+            (out_a, expected_inC_a, probability[1], indexes[1], probs[1]))
+        if self.downsample is not None:
+            residual, _, expected_flop_c = self.downsample((inputs, expected_inC, probability[1], indexes[1], probs[1]))
+        else:
+            residual, expected_flop_c = inputs, 0
+        out = additive_func(residual, out_b)
+        return nn.functional.relu(out, inplace=True), expected_inC_b, sum(
+            [expected_flop_a, expected_flop_b, expected_flop_c])
+
+    def basic_forward(self, inputs):
+        basicblock = self.conv_a(inputs)
+        basicblock = self.conv_b(basicblock)
+        if self.downsample is not None:
+            residual = self.downsample(inputs)
+        else:
+            residual = inputs
+        out = additive_func(residual, basicblock)
+        return nn.functional.relu(out, inplace=True)
+
+
+class ResNetBottleneck(nn.Module):
+    expansion = 4
+    num_conv = 3
+
+    def __init__(self, inplanes, planes, stride):
+        super(ResNetBottleneck, self).__init__()
+        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
+        self.conv_1x1 = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=True)
+        self.conv_3x3 = ConvBNReLU(planes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
+        self.conv_1x4 = ConvBNReLU(planes, planes * self.expansion, 1, 1, 0, False, has_avg=False, has_bn=True,
+                                   has_relu=False)
+        if stride == 2:
+            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, has_avg=True, has_bn=False,
+                                         has_relu=False)
+        elif inplanes != planes * self.expansion:
+            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, has_avg=False, has_bn=True,
+                                         has_relu=False)
+        else:
+            self.downsample = None
+        self.out_dim = planes * self.expansion
+        self.search_mode = 'basic'
+
+    def get_range(self):
+        return self.conv_1x1.get_range() + self.conv_3x3.get_range() + self.conv_1x4.get_range()
+
+    def get_flops(self, channels):
+        assert len(channels) == 4, 'invalid channels : {:}'.format(channels)
+        flop_A = self.conv_1x1.get_flops([channels[0], channels[1]])
+        flop_B = self.conv_3x3.get_flops([channels[1], channels[2]])
+        flop_C = self.conv_1x4.get_flops([channels[2], channels[3]])
+        if hasattr(self.downsample, 'get_flops'):
+            flop_D = self.downsample.get_flops([channels[0], channels[-1]])
+        else:
+            flop_D = 0
+        if channels[0] != channels[
+            -1] and self.downsample is None:  # this short-cut will be added during the infer-train
+            flop_D = channels[0] * channels[-1] * self.conv_1x4.OutShape[0] * self.conv_1x4.OutShape[1]
+        return flop_A + flop_B + flop_C + flop_D
+
+    def forward(self, inputs):
+        if self.search_mode == 'basic':
+            return self.basic_forward(inputs)
+        elif self.search_mode == 'search':
+            return self.search_forward(inputs)
+        else:
+            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
+
+    def basic_forward(self, inputs):
+        bottleneck = self.conv_1x1(inputs)
+        bottleneck = self.conv_3x3(bottleneck)
+        bottleneck = self.conv_1x4(bottleneck)
+        if self.downsample is not None:
+            residual = self.downsample(inputs)
+        else:
+            residual = inputs
+        out = additive_func(residual, bottleneck)
+        return nn.functional.relu(out, inplace=True)
+
+    def search_forward(self, tuple_inputs):
+        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
+            type(tuple_inputs))
+        inputs, expected_inC, probability, indexes, probs = tuple_inputs
+        assert indexes.size(0) == 3 and probs.size(0) == 3 and probability.size(0) == 3
+        out_1x1, expected_inC_1x1, expected_flop_1x1 = self.conv_1x1(
+            (inputs, expected_inC, probability[0], indexes[0], probs[0]))
+        out_3x3, expected_inC_3x3, expected_flop_3x3 = self.conv_3x3(
+            (out_1x1, expected_inC_1x1, probability[1], indexes[1], probs[1]))
+        out_1x4, expected_inC_1x4, expected_flop_1x4 = self.conv_1x4(
+            (out_3x3, expected_inC_3x3, probability[2], indexes[2], probs[2]))
+        if self.downsample is not None:
+            residual, _, expected_flop_c = self.downsample((inputs, expected_inC, probability[2], indexes[2], probs[2]))
+        else:
+            residual, expected_flop_c = inputs, 0
+        out = additive_func(residual, out_1x4)
+        return nn.functional.relu(out, inplace=True), expected_inC_1x4, sum(
+            [expected_flop_1x1, expected_flop_3x3, expected_flop_1x4, expected_flop_c])
+
+
+class SearchWidthCifarResNet(nn.Module):
+
+    def __init__(self, block_name, depth, num_classes):
+        super(SearchWidthCifarResNet, self).__init__()
+
+        # Model type specifies number of layers for CIFAR-10 and CIFAR-100 model
+        if block_name == 'ResNetBasicblock':
+            block = ResNetBasicblock
+            assert (depth - 2) % 6 == 0, 'depth should be one of 20, 32, 44, 56, 110'
+            layer_blocks = (depth - 2) // 6
+        elif block_name == 'ResNetBottleneck':
+            block = ResNetBottleneck
+            assert (depth - 2) % 9 == 0, 'depth should be one of 164'
+            layer_blocks = (depth - 2) // 9
+        else:
+            raise ValueError('invalid block : {:}'.format(block_name))
+
+        self.message = 'SearchWidthCifarResNet : Depth : {:} , Layers for each block : {:}'.format(depth, layer_blocks)
+        self.num_classes = num_classes
+        self.channels = [16]
+        self.layers = nn.ModuleList([ConvBNReLU(3, 16, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=True)])
+        self.InShape = None
+        for stage in range(3):
+            for iL in range(layer_blocks):
+                iC = self.channels[-1]
+                planes = 16 * (2 ** stage)
+                stride = 2 if stage > 0 and iL == 0 else 1
+                module = block(iC, planes, stride)
+                self.channels.append(module.out_dim)
+                self.layers.append(module)
+                self.message += "\nstage={:}, ilayer={:02d}/{:02d}, block={:03d}, iC={:3d}, oC={:3d}, stride={:}".format(
+                    stage, iL, layer_blocks, len(self.layers) - 1, iC, module.out_dim, stride)
+
+        self.avgpool = nn.AvgPool2d(8)
+        self.classifier = nn.Linear(module.out_dim, num_classes)
+        self.InShape = None
+        self.tau = -1
+        self.search_mode = 'basic'
+        # assert sum(x.num_conv for x in self.layers) + 1 == depth, 'invalid depth check {:} vs {:}'.format(sum(x.num_conv for x in self.layers)+1, depth)
+
+        # parameters for width
+        self.Ranges = []
+        self.layer2indexRange = []
+        for i, layer in enumerate(self.layers):
+            start_index = len(self.Ranges)
+            self.Ranges += layer.get_range()
+            self.layer2indexRange.append((start_index, len(self.Ranges)))
+        assert len(self.Ranges) + 1 == depth, 'invalid depth check {:} vs {:}'.format(len(self.Ranges) + 1, depth)
+
+        self.register_parameter('width_attentions', nn.Parameter(torch.Tensor(len(self.Ranges), get_choices(None))))
+        nn.init.normal_(self.width_attentions, 0, 0.01)
+        self.apply(initialize_resnet)
+
+    def arch_parameters(self):
+        return [self.width_attentions]
+
+    def base_parameters(self):
+        return list(self.layers.parameters()) + list(self.avgpool.parameters()) + list(self.classifier.parameters())
+
+    def get_flop(self, mode, config_dict, extra_info):
+        if config_dict is not None: config_dict = config_dict.copy()
+        # weights = [F.softmax(x, dim=0) for x in self.width_attentions]
+        channels = [3]
+        for i, weight in enumerate(self.width_attentions):
+            if mode == 'genotype':
+                with torch.no_grad():
+                    probe = nn.functional.softmax(weight, dim=0)
+                    C = self.Ranges[i][torch.argmax(probe).item()]
+            elif mode == 'max':
+                C = self.Ranges[i][-1]
+            elif mode == 'fix':
+                C = int(math.sqrt(extra_info) * self.Ranges[i][-1])
+            elif mode == 'random':
+                assert isinstance(extra_info, float), 'invalid extra_info : {:}'.format(extra_info)
+                with torch.no_grad():
+                    prob = nn.functional.softmax(weight, dim=0)
+                    approximate_C = int(math.sqrt(extra_info) * self.Ranges[i][-1])
+                    for j in range(prob.size(0)):
+                        prob[j] = 1 / (abs(j - (approximate_C - self.Ranges[i][j])) + 0.2)
+                    C = self.Ranges[i][torch.multinomial(prob, 1, False).item()]
+            else:
+                raise ValueError('invalid mode : {:}'.format(mode))
+            channels.append(C)
+        flop = 0
+        for i, layer in enumerate(self.layers):
+            s, e = self.layer2indexRange[i]
+            xchl = tuple(channels[s:e + 1])
+            flop += layer.get_flops(xchl)
+        # the last fc layer
+        flop += channels[-1] * self.classifier.out_features
+        if config_dict is None:
+            return flop / 1e6
+        else:
+            config_dict['xchannels'] = channels
+            config_dict['super_type'] = 'infer-width'
+            config_dict['estimated_FLOP'] = flop / 1e6
+            return flop / 1e6, config_dict
+
+    def get_arch_info(self):
+        string = "for width, there are {:} attention probabilities.".format(len(self.width_attentions))
+        discrepancy = []
+        with torch.no_grad():
+            for i, att in enumerate(self.width_attentions):
+                prob = nn.functional.softmax(att, dim=0)
+                prob = prob.cpu();
+                selc = prob.argmax().item();
+                prob = prob.tolist()
+                prob = ['{:.3f}'.format(x) for x in prob]
+                xstring = '{:03d}/{:03d}-th : {:}'.format(i, len(self.width_attentions), ' '.join(prob))
+                logt = ['{:.3f}'.format(x) for x in att.cpu().tolist()]
+                xstring += '  ||  {:52s}'.format(' '.join(logt))
+                prob = sorted([float(x) for x in prob])
+                disc = prob[-1] - prob[-2]
+                xstring += '  || dis={:.2f} || select={:}/{:}'.format(disc, selc, len(prob))
+                discrepancy.append(disc)
+                string += '\n{:}'.format(xstring)
+        return string, discrepancy
+
+    def set_tau(self, tau_max, tau_min, epoch_ratio):
+        assert epoch_ratio >= 0 and epoch_ratio <= 1, 'invalid epoch-ratio : {:}'.format(epoch_ratio)
+        tau = tau_min + (tau_max - tau_min) * (1 + math.cos(math.pi * epoch_ratio)) / 2
+        self.tau = tau
+
+    def get_message(self):
+        return self.message
+
+    def forward(self, inputs):
+        if self.search_mode == 'basic':
+            return self.basic_forward(inputs)
+        elif self.search_mode == 'search':
+            return self.search_forward(inputs)
+        else:
+            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
+
+    def search_forward(self, inputs):
+        flop_probs = nn.functional.softmax(self.width_attentions, dim=1)
+        selected_widths, selected_probs = select2withP(self.width_attentions, self.tau)
+        with torch.no_grad():
+            selected_widths = selected_widths.cpu()
+
+        x, last_channel_idx, expected_inC, flops = inputs, 0, 3, []
+        for i, layer in enumerate(self.layers):
+            selected_w_index = selected_widths[last_channel_idx: last_channel_idx + layer.num_conv]
+            selected_w_probs = selected_probs[last_channel_idx: last_channel_idx + layer.num_conv]
+            layer_prob = flop_probs[last_channel_idx: last_channel_idx + layer.num_conv]
+            x, expected_inC, expected_flop = layer((x, expected_inC, layer_prob, selected_w_index, selected_w_probs))
+            last_channel_idx += layer.num_conv
+            flops.append(expected_flop)
+        flops.append(expected_inC * (self.classifier.out_features * 1.0 / 1e6))
+        features = self.avgpool(x)
+        features = features.view(features.size(0), -1)
+        logits = linear_forward(features, self.classifier)
+        return logits, torch.stack([sum(flops)])
+
+    def basic_forward(self, inputs):
+        if self.InShape is None: self.InShape = (inputs.size(-2), inputs.size(-1))
+        x = inputs
+        for i, layer in enumerate(self.layers):
+            x = layer(x)
+        features = self.avgpool(x)
+        features = features.view(features.size(0), -1)
+        logits = self.classifier(features)
+        return features, logits
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchImagenetResNet.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchCifarResNet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,538 +1,558 @@
-import math, torch
-from collections import OrderedDict
-from bisect import bisect_right
-import torch.nn as nn
-from ..initialization import initialize_resnet
-from ..SharedUtils import additive_func
-from .SoftSelect import select2withP, ChannelWiseInter
-from .SoftSelect import linear_forward
-from .SoftSelect import get_width_choices
-
-
-def get_depth_choices(layers):
-    min_depth = min(layers)
-    info = {'num': min_depth}
-    for i, depth in enumerate(layers):
-        choices = []
-        for j in range(1, min_depth + 1):
-            choices.append(int(float(depth) * j / min_depth))
-        info[i] = choices
-    return info
-
-
-def conv_forward(inputs, conv, choices):
-    iC = conv.in_channels
-    fill_size = list(inputs.size())
-    fill_size[1] = iC - fill_size[1]
-    filled = torch.zeros(fill_size, device=inputs.device)
-    xinputs = torch.cat((inputs, filled), dim=1)
-    outputs = conv(xinputs)
-    selecteds = [outputs[:, :oC] for oC in choices]
-    return selecteds
-
-
-class ConvBNReLU(nn.Module):
-    num_conv = 1
-
-    def __init__(self, nIn, nOut, kernel, stride, padding, bias, has_avg, has_bn, has_relu, last_max_pool=False):
-        super(ConvBNReLU, self).__init__()
-        self.InShape = None
-        self.OutShape = None
-        self.choices = get_width_choices(nOut)
-        self.register_buffer('choices_tensor', torch.Tensor(self.choices))
-
-        if has_avg:
-            self.avg = nn.AvgPool2d(kernel_size=2, stride=2, padding=0)
-        else:
-            self.avg = None
-        self.conv = nn.Conv2d(nIn, nOut, kernel_size=kernel, stride=stride, padding=padding, dilation=1, groups=1,
-                              bias=bias)
-        # if has_bn  : self.bn  = nn.BatchNorm2d(nOut)
-        # else       : self.bn  = None
-        self.has_bn = has_bn
-        self.BNs = nn.ModuleList()
-        for i, _out in enumerate(self.choices):
-            self.BNs.append(nn.BatchNorm2d(_out))
-        if has_relu:
-            self.relu = nn.ReLU(inplace=True)
-        else:
-            self.relu = None
-
-        if last_max_pool:
-            self.maxpool = nn.MaxPool2d(kernel_size=3, stride=2, padding=1)
-        else:
-            self.maxpool = None
-        self.in_dim = nIn
-        self.out_dim = nOut
-        self.search_mode = 'basic'
-
-    def get_flops(self, channels, check_range=True, divide=1):
-        iC, oC = channels
-        if check_range: assert iC <= self.conv.in_channels and oC <= self.conv.out_channels, '{:} vs {:}  |  {:} vs {:}'.format(
-            iC, self.conv.in_channels, oC, self.conv.out_channels)
-        assert isinstance(self.InShape, tuple) and len(self.InShape) == 2, 'invalid in-shape : {:}'.format(self.InShape)
-        assert isinstance(self.OutShape, tuple) and len(self.OutShape) == 2, 'invalid out-shape : {:}'.format(
-            self.OutShape)
-        # conv_per_position_flops = self.conv.kernel_size[0] * self.conv.kernel_size[1] * iC * oC / self.conv.groups
-        conv_per_position_flops = (self.conv.kernel_size[0] * self.conv.kernel_size[1] * 1.0 / self.conv.groups)
-        all_positions = self.OutShape[0] * self.OutShape[1]
-        flops = (conv_per_position_flops * all_positions / divide) * iC * oC
-        if self.conv.bias is not None: flops += all_positions / divide
-        return flops
-
-    def get_range(self):
-        return [self.choices]
-
-    def forward(self, inputs):
-        if self.search_mode == 'basic':
-            return self.basic_forward(inputs)
-        elif self.search_mode == 'search':
-            return self.search_forward(inputs)
-        else:
-            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
-
-    def search_forward(self, tuple_inputs):
-        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
-            type(tuple_inputs))
-        inputs, expected_inC, probability, index, prob = tuple_inputs
-        index, prob = torch.squeeze(index).tolist(), torch.squeeze(prob)
-        probability = torch.squeeze(probability)
-        assert len(index) == 2, 'invalid length : {:}'.format(index)
-        # compute expected flop
-        # coordinates   = torch.arange(self.x_range[0], self.x_range[1]+1).type_as(probability)
-        expected_outC = (self.choices_tensor * probability).sum()
-        expected_flop = self.get_flops([expected_inC, expected_outC], False, 1e6)
-        if self.avg:
-            out = self.avg(inputs)
-        else:
-            out = inputs
-        # convolutional layer
-        out_convs = conv_forward(out, self.conv, [self.choices[i] for i in index])
-        out_bns = [self.BNs[idx](out_conv) for idx, out_conv in zip(index, out_convs)]
-        # merge
-        out_channel = max([x.size(1) for x in out_bns])
-        outA = ChannelWiseInter(out_bns[0], out_channel)
-        outB = ChannelWiseInter(out_bns[1], out_channel)
-        out = outA * prob[0] + outB * prob[1]
-        # out = additive_func(out_bns[0]*prob[0], out_bns[1]*prob[1])
-
-        if self.relu: out = self.relu(out)
-        if self.maxpool: out = self.maxpool(out)
-        return out, expected_outC, expected_flop
-
-    def basic_forward(self, inputs):
-        if self.avg:
-            out = self.avg(inputs)
-        else:
-            out = inputs
-        conv = self.conv(out)
-        if self.has_bn:
-            out = self.BNs[-1](conv)
-        else:
-            out = conv
-        if self.relu:
-            out = self.relu(out)
-        else:
-            out = out
-        if self.InShape is None:
-            self.InShape = (inputs.size(-2), inputs.size(-1))
-            self.OutShape = (out.size(-2), out.size(-1))
-        if self.maxpool: out = self.maxpool(out)
-        return out
-
-
-class ResNetBasicblock(nn.Module):
-    expansion = 1
-    num_conv = 2
-
-    def __init__(self, inplanes, planes, stride):
-        super(ResNetBasicblock, self).__init__()
-        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
-        self.conv_a = ConvBNReLU(inplanes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
-        self.conv_b = ConvBNReLU(planes, planes, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=False)
-        if stride == 2:
-            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=True, has_bn=True, has_relu=False)
-        elif inplanes != planes:
-            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=False)
-        else:
-            self.downsample = None
-        self.out_dim = planes
-        self.search_mode = 'basic'
-
-    def get_range(self):
-        return self.conv_a.get_range() + self.conv_b.get_range()
-
-    def get_flops(self, channels):
-        assert len(channels) == 3, 'invalid channels : {:}'.format(channels)
-        flop_A = self.conv_a.get_flops([channels[0], channels[1]])
-        flop_B = self.conv_b.get_flops([channels[1], channels[2]])
-        if hasattr(self.downsample, 'get_flops'):
-            flop_C = self.downsample.get_flops([channels[0], channels[-1]])
-        else:
-            flop_C = 0
-        if channels[0] != channels[
-            -1] and self.downsample is None:  # this short-cut will be added during the infer-train
-            flop_C = channels[0] * channels[-1] * self.conv_b.OutShape[0] * self.conv_b.OutShape[1]
-        return flop_A + flop_B + flop_C
-
-    def forward(self, inputs):
-        if self.search_mode == 'basic':
-            return self.basic_forward(inputs)
-        elif self.search_mode == 'search':
-            return self.search_forward(inputs)
-        else:
-            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
-
-    def search_forward(self, tuple_inputs):
-        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
-            type(tuple_inputs))
-        inputs, expected_inC, probability, indexes, probs = tuple_inputs
-        assert indexes.size(0) == 2 and probs.size(0) == 2 and probability.size(0) == 2
-        # import pdb; pdb.set_trace()
-        out_a, expected_inC_a, expected_flop_a = self.conv_a(
-            (inputs, expected_inC, probability[0], indexes[0], probs[0]))
-        out_b, expected_inC_b, expected_flop_b = self.conv_b(
-            (out_a, expected_inC_a, probability[1], indexes[1], probs[1]))
-        if self.downsample is not None:
-            residual, _, expected_flop_c = self.downsample((inputs, expected_inC, probability[1], indexes[1], probs[1]))
-        else:
-            residual, expected_flop_c = inputs, 0
-        out = additive_func(residual, out_b)
-        return nn.functional.relu(out, inplace=True), expected_inC_b, sum(
-            [expected_flop_a, expected_flop_b, expected_flop_c])
-
-    def basic_forward(self, inputs):
-        basicblock = self.conv_a(inputs)
-        basicblock = self.conv_b(basicblock)
-        if self.downsample is not None:
-            residual = self.downsample(inputs)
-        else:
-            residual = inputs
-        out = additive_func(residual, basicblock)
-        return nn.functional.relu(out, inplace=True)
-
-
-class ResNetBottleneck(nn.Module):
-    expansion = 4
-    num_conv = 3
-
-    def __init__(self, inplanes, planes, stride):
-        super(ResNetBottleneck, self).__init__()
-        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
-        self.conv_1x1 = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=True)
-        self.conv_3x3 = ConvBNReLU(planes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
-        self.conv_1x4 = ConvBNReLU(planes, planes * self.expansion, 1, 1, 0, False, has_avg=False, has_bn=True,
-                                   has_relu=False)
-        if stride == 2:
-            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, has_avg=True, has_bn=True,
-                                         has_relu=False)
-        elif inplanes != planes * self.expansion:
-            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, has_avg=False, has_bn=True,
-                                         has_relu=False)
-        else:
-            self.downsample = None
-        self.out_dim = planes * self.expansion
-        self.search_mode = 'basic'
-
-    def get_range(self):
-        return self.conv_1x1.get_range() + self.conv_3x3.get_range() + self.conv_1x4.get_range()
-
-    def get_flops(self, channels):
-        assert len(channels) == 4, 'invalid channels : {:}'.format(channels)
-        flop_A = self.conv_1x1.get_flops([channels[0], channels[1]])
-        flop_B = self.conv_3x3.get_flops([channels[1], channels[2]])
-        flop_C = self.conv_1x4.get_flops([channels[2], channels[3]])
-        if hasattr(self.downsample, 'get_flops'):
-            flop_D = self.downsample.get_flops([channels[0], channels[-1]])
-        else:
-            flop_D = 0
-        if channels[0] != channels[
-            -1] and self.downsample is None:  # this short-cut will be added during the infer-train
-            flop_D = channels[0] * channels[-1] * self.conv_1x4.OutShape[0] * self.conv_1x4.OutShape[1]
-        return flop_A + flop_B + flop_C + flop_D
-
-    def forward(self, inputs):
-        if self.search_mode == 'basic':
-            return self.basic_forward(inputs)
-        elif self.search_mode == 'search':
-            return self.search_forward(inputs)
-        else:
-            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
-
-    def basic_forward(self, inputs):
-        bottleneck = self.conv_1x1(inputs)
-        bottleneck = self.conv_3x3(bottleneck)
-        bottleneck = self.conv_1x4(bottleneck)
-        if self.downsample is not None:
-            residual = self.downsample(inputs)
-        else:
-            residual = inputs
-        out = additive_func(residual, bottleneck)
-        return nn.functional.relu(out, inplace=True)
-
-    def search_forward(self, tuple_inputs):
-        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
-            type(tuple_inputs))
-        inputs, expected_inC, probability, indexes, probs = tuple_inputs
-        assert indexes.size(0) == 3 and probs.size(0) == 3 and probability.size(0) == 3
-        out_1x1, expected_inC_1x1, expected_flop_1x1 = self.conv_1x1(
-            (inputs, expected_inC, probability[0], indexes[0], probs[0]))
-        out_3x3, expected_inC_3x3, expected_flop_3x3 = self.conv_3x3(
-            (out_1x1, expected_inC_1x1, probability[1], indexes[1], probs[1]))
-        out_1x4, expected_inC_1x4, expected_flop_1x4 = self.conv_1x4(
-            (out_3x3, expected_inC_3x3, probability[2], indexes[2], probs[2]))
-        if self.downsample is not None:
-            residual, _, expected_flop_c = self.downsample((inputs, expected_inC, probability[2], indexes[2], probs[2]))
-        else:
-            residual, expected_flop_c = inputs, 0
-        out = additive_func(residual, out_1x4)
-        return nn.functional.relu(out, inplace=True), expected_inC_1x4, sum(
-            [expected_flop_1x1, expected_flop_3x3, expected_flop_1x4, expected_flop_c])
-
-
-class SearchShapeImagenetResNet(nn.Module):
-
-    def __init__(self, block_name, layers, deep_stem, num_classes):
-        super(SearchShapeImagenetResNet, self).__init__()
-
-        # Model type specifies number of layers for CIFAR-10 and CIFAR-100 model
-        if block_name == 'BasicBlock':
-            block = ResNetBasicblock
-        elif block_name == 'Bottleneck':
-            block = ResNetBottleneck
-        else:
-            raise ValueError('invalid block : {:}'.format(block_name))
-
-        self.message = 'SearchShapeCifarResNet : Depth : {:} , Layers for each block : {:}'.format(
-            sum(layers) * block.num_conv, layers)
-        self.num_classes = num_classes
-        if not deep_stem:
-            self.layers = nn.ModuleList(
-                [ConvBNReLU(3, 64, 7, 2, 3, False, has_avg=False, has_bn=True, has_relu=True, last_max_pool=True)])
-            self.channels = [64]
-        else:
-            self.layers = nn.ModuleList([ConvBNReLU(3, 32, 3, 2, 1, False, has_avg=False, has_bn=True, has_relu=True)
-                                            ,
-                                         ConvBNReLU(32, 64, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=True,
-                                                    last_max_pool=True)])
-            self.channels = [32, 64]
-
-        meta_depth_info = get_depth_choices(layers)
-        self.InShape = None
-        self.depth_info = OrderedDict()
-        self.depth_at_i = OrderedDict()
-        for stage, layer_blocks in enumerate(layers):
-            cur_block_choices = meta_depth_info[stage]
-            assert cur_block_choices[-1] == layer_blocks, 'stage={:}, {:} vs {:}'.format(stage, cur_block_choices,
-                                                                                         layer_blocks)
-            block_choices, xstart = [], len(self.layers)
-            for iL in range(layer_blocks):
-                iC = self.channels[-1]
-                planes = 64 * (2 ** stage)
-                stride = 2 if stage > 0 and iL == 0 else 1
-                module = block(iC, planes, stride)
-                self.channels.append(module.out_dim)
-                self.layers.append(module)
-                self.message += "\nstage={:}, ilayer={:02d}/{:02d}, block={:03d}, iC={:3d}, oC={:3d}, stride={:}".format(
-                    stage, iL, layer_blocks, len(self.layers) - 1, iC, module.out_dim, stride)
-                # added for depth
-                layer_index = len(self.layers) - 1
-                if iL + 1 in cur_block_choices: block_choices.append(layer_index)
-                if iL + 1 == layer_blocks:
-                    self.depth_info[layer_index] = {'choices': block_choices,
-                                                    'stage': stage,
-                                                    'xstart': xstart}
-        self.depth_info_list = []
-        for xend, info in self.depth_info.items():
-            self.depth_info_list.append((xend, info))
-            xstart, xstage = info['xstart'], info['stage']
-            for ilayer in range(xstart, xend + 1):
-                idx = bisect_right(info['choices'], ilayer - 1)
-                self.depth_at_i[ilayer] = (xstage, idx)
-
-        self.avgpool = nn.AdaptiveAvgPool2d((1, 1))
-        self.classifier = nn.Linear(module.out_dim, num_classes)
-        self.InShape = None
-        self.tau = -1
-        self.search_mode = 'basic'
-        # assert sum(x.num_conv for x in self.layers) + 1 == depth, 'invalid depth check {:} vs {:}'.format(sum(x.num_conv for x in self.layers)+1, depth)
-
-        # parameters for width
-        self.Ranges = []
-        self.layer2indexRange = []
-        for i, layer in enumerate(self.layers):
-            start_index = len(self.Ranges)
-            self.Ranges += layer.get_range()
-            self.layer2indexRange.append((start_index, len(self.Ranges)))
-
-        self.register_parameter('width_attentions',
-                                nn.Parameter(torch.Tensor(len(self.Ranges), get_width_choices(None))))
-        self.register_parameter('depth_attentions', nn.Parameter(torch.Tensor(len(layers), meta_depth_info['num'])))
-        nn.init.normal_(self.width_attentions, 0, 0.01)
-        nn.init.normal_(self.depth_attentions, 0, 0.01)
-        self.apply(initialize_resnet)
-
-    def arch_parameters(self, LR=None):
-        if LR is None:
-            return [self.width_attentions, self.depth_attentions]
-        else:
-            return [
-                {"params": self.width_attentions, "lr": LR},
-                {"params": self.depth_attentions, "lr": LR},
-            ]
-
-    def base_parameters(self):
-        return list(self.layers.parameters()) + list(self.avgpool.parameters()) + list(self.classifier.parameters())
-
-    def get_flop(self, mode, config_dict, extra_info):
-        if config_dict is not None: config_dict = config_dict.copy()
-        # select channels
-        channels = [3]
-        for i, weight in enumerate(self.width_attentions):
-            if mode == 'genotype':
-                with torch.no_grad():
-                    probe = nn.functional.softmax(weight, dim=0)
-                    C = self.Ranges[i][torch.argmax(probe).item()]
-            else:
-                raise ValueError('invalid mode : {:}'.format(mode))
-            channels.append(C)
-        # select depth
-        if mode == 'genotype':
-            with torch.no_grad():
-                depth_probs = nn.functional.softmax(self.depth_attentions, dim=1)
-                choices = torch.argmax(depth_probs, dim=1).cpu().tolist()
-        else:
-            raise ValueError('invalid mode : {:}'.format(mode))
-        selected_layers = []
-        for choice, xvalue in zip(choices, self.depth_info_list):
-            xtemp = xvalue[1]['choices'][choice] - xvalue[1]['xstart'] + 1
-            selected_layers.append(xtemp)
-        flop = 0
-        for i, layer in enumerate(self.layers):
-            s, e = self.layer2indexRange[i]
-            xchl = tuple(channels[s:e + 1])
-            if i in self.depth_at_i:
-                xstagei, xatti = self.depth_at_i[i]
-                if xatti <= choices[xstagei]:  # leave this depth
-                    flop += layer.get_flops(xchl)
-                else:
-                    flop += 0  # do not use this layer
-            else:
-                flop += layer.get_flops(xchl)
-        # the last fc layer
-        flop += channels[-1] * self.classifier.out_features
-        if config_dict is None:
-            return flop / 1e6
-        else:
-            config_dict['xchannels'] = channels
-            config_dict['xblocks'] = selected_layers
-            config_dict['super_type'] = 'infer-shape'
-            config_dict['estimated_FLOP'] = flop / 1e6
-            return flop / 1e6, config_dict
-
-    def get_arch_info(self):
-        string = "for depth and width, there are {:} + {:} attention probabilities.".format(len(self.depth_attentions),
-                                                                                            len(self.width_attentions))
-        string += '\n{:}'.format(self.depth_info)
-        discrepancy = []
-        with torch.no_grad():
-            for i, att in enumerate(self.depth_attentions):
-                prob = nn.functional.softmax(att, dim=0)
-                prob = prob.cpu();
-                selc = prob.argmax().item();
-                prob = prob.tolist()
-                prob = ['{:.3f}'.format(x) for x in prob]
-                xstring = '{:03d}/{:03d}-th : {:}'.format(i, len(self.depth_attentions), ' '.join(prob))
-                logt = ['{:.4f}'.format(x) for x in att.cpu().tolist()]
-                xstring += '  ||  {:17s}'.format(' '.join(logt))
-                prob = sorted([float(x) for x in prob])
-                disc = prob[-1] - prob[-2]
-                xstring += '  || discrepancy={:.2f} || select={:}/{:}'.format(disc, selc, len(prob))
-                discrepancy.append(disc)
-                string += '\n{:}'.format(xstring)
-            string += '\n-----------------------------------------------'
-            for i, att in enumerate(self.width_attentions):
-                prob = nn.functional.softmax(att, dim=0)
-                prob = prob.cpu();
-                selc = prob.argmax().item();
-                prob = prob.tolist()
-                prob = ['{:.3f}'.format(x) for x in prob]
-                xstring = '{:03d}/{:03d}-th : {:}'.format(i, len(self.width_attentions), ' '.join(prob))
-                logt = ['{:.3f}'.format(x) for x in att.cpu().tolist()]
-                xstring += '  ||  {:52s}'.format(' '.join(logt))
-                prob = sorted([float(x) for x in prob])
-                disc = prob[-1] - prob[-2]
-                xstring += '  || dis={:.2f} || select={:}/{:}'.format(disc, selc, len(prob))
-                discrepancy.append(disc)
-                string += '\n{:}'.format(xstring)
-        return string, discrepancy
-
-    def set_tau(self, tau_max, tau_min, epoch_ratio):
-        assert epoch_ratio >= 0 and epoch_ratio <= 1, 'invalid epoch-ratio : {:}'.format(epoch_ratio)
-        tau = tau_min + (tau_max - tau_min) * (1 + math.cos(math.pi * epoch_ratio)) / 2
-        self.tau = tau
-
-    def get_message(self):
-        return self.message
-
-    def forward(self, inputs):
-        if self.search_mode == 'basic':
-            return self.basic_forward(inputs)
-        elif self.search_mode == 'search':
-            return self.search_forward(inputs)
-        else:
-            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
-
-    def search_forward(self, inputs):
-        flop_width_probs = nn.functional.softmax(self.width_attentions, dim=1)
-        flop_depth_probs = nn.functional.softmax(self.depth_attentions, dim=1)
-        flop_depth_probs = torch.flip(torch.cumsum(torch.flip(flop_depth_probs, [1]), 1), [1])
-        selected_widths, selected_width_probs = select2withP(self.width_attentions, self.tau)
-        selected_depth_probs = select2withP(self.depth_attentions, self.tau, True)
-        with torch.no_grad():
-            selected_widths = selected_widths.cpu()
-
-        x, last_channel_idx, expected_inC, flops = inputs, 0, 3, []
-        feature_maps = []
-        for i, layer in enumerate(self.layers):
-            selected_w_index = selected_widths[last_channel_idx: last_channel_idx + layer.num_conv]
-            selected_w_probs = selected_width_probs[last_channel_idx: last_channel_idx + layer.num_conv]
-            layer_prob = flop_width_probs[last_channel_idx: last_channel_idx + layer.num_conv]
-            x, expected_inC, expected_flop = layer((x, expected_inC, layer_prob, selected_w_index, selected_w_probs))
-            feature_maps.append(x)
-            last_channel_idx += layer.num_conv
-            if i in self.depth_info:  # aggregate the information
-                choices = self.depth_info[i]['choices']
-                xstagei = self.depth_info[i]['stage']
-                # print ('iL={:}, choices={:}, stage={:}, probs={:}'.format(i, choices, xstagei, selected_depth_probs[xstagei].cpu().tolist()))
-                # for A, W in zip(choices, selected_depth_probs[xstagei]):
-                #  print('Size = {:}, W = {:}'.format(feature_maps[A].size(), W))
-                possible_tensors = []
-                max_C = max(feature_maps[A].size(1) for A in choices)
-                for tempi, A in enumerate(choices):
-                    xtensor = ChannelWiseInter(feature_maps[A], max_C)
-                    possible_tensors.append(xtensor)
-                weighted_sum = sum(xtensor * W for xtensor, W in zip(possible_tensors, selected_depth_probs[xstagei]))
-                x = weighted_sum
-
-            if i in self.depth_at_i:
-                xstagei, xatti = self.depth_at_i[i]
-                x_expected_flop = flop_depth_probs[xstagei, xatti] * expected_flop
-            else:
-                x_expected_flop = expected_flop
-            flops.append(x_expected_flop)
-        flops.append(expected_inC * (self.classifier.out_features * 1.0 / 1e6))
-        features = self.avgpool(x)
-        features = features.view(features.size(0), -1)
-        logits = linear_forward(features, self.classifier)
-        return logits, torch.stack([sum(flops)])
-
-    def basic_forward(self, inputs):
-        if self.InShape is None: self.InShape = (inputs.size(-2), inputs.size(-1))
-        x = inputs
-        for i, layer in enumerate(self.layers):
-            x = layer(x)
-        features = self.avgpool(x)
-        features = features.view(features.size(0), -1)
-        logits = self.classifier(features)
-        return features, logits
+##################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
+##################################################
+import math, torch
+from collections import OrderedDict
+from bisect import bisect_right
+import torch.nn as nn
+from ..initialization import initialize_resnet
+from ..SharedUtils import additive_func
+from .SoftSelect import select2withP, ChannelWiseInter
+from .SoftSelect import linear_forward
+from .SoftSelect import get_width_choices
+
+
+def get_depth_choices(nDepth, return_num):
+    if nDepth == 2:
+        choices = (1, 2)
+    elif nDepth == 3:
+        choices = (1, 2, 3)
+    elif nDepth > 3:
+        choices = list(range(1, nDepth + 1, 2))
+        if choices[-1] < nDepth: choices.append(nDepth)
+    else:
+        raise ValueError('invalid nDepth : {:}'.format(nDepth))
+    if return_num:
+        return len(choices)
+    else:
+        return choices
+
+
+def conv_forward(inputs, conv, choices):
+    iC = conv.in_channels
+    fill_size = list(inputs.size())
+    fill_size[1] = iC - fill_size[1]
+    filled = torch.zeros(fill_size, device=inputs.device)
+    xinputs = torch.cat((inputs, filled), dim=1)
+    outputs = conv(xinputs)
+    selecteds = [outputs[:, :oC] for oC in choices]
+    return selecteds
+
+
+class ConvBNReLU(nn.Module):
+    num_conv = 1
+
+    def __init__(self, nIn, nOut, kernel, stride, padding, bias, has_avg, has_bn, has_relu):
+        super(ConvBNReLU, self).__init__()
+        self.InShape = None
+        self.OutShape = None
+        self.choices = get_width_choices(nOut)
+        self.register_buffer('choices_tensor', torch.Tensor(self.choices))
+
+        if has_avg:
+            self.avg = nn.AvgPool2d(kernel_size=2, stride=2, padding=0)
+        else:
+            self.avg = None
+        self.conv = nn.Conv2d(nIn, nOut, kernel_size=kernel, stride=stride, padding=padding, dilation=1, groups=1,
+                              bias=bias)
+        # if has_bn  : self.bn  = nn.BatchNorm2d(nOut)
+        # else       : self.bn  = None
+        self.has_bn = has_bn
+        self.BNs = nn.ModuleList()
+        for i, _out in enumerate(self.choices):
+            self.BNs.append(nn.BatchNorm2d(_out))
+        if has_relu:
+            self.relu = nn.ReLU(inplace=True)
+        else:
+            self.relu = None
+        self.in_dim = nIn
+        self.out_dim = nOut
+        self.search_mode = 'basic'
+
+    def get_flops(self, channels, check_range=True, divide=1):
+        iC, oC = channels
+        if check_range: assert iC <= self.conv.in_channels and oC <= self.conv.out_channels, '{:} vs {:}  |  {:} vs {:}'.format(
+            iC, self.conv.in_channels, oC, self.conv.out_channels)
+        assert isinstance(self.InShape, tuple) and len(self.InShape) == 2, 'invalid in-shape : {:}'.format(self.InShape)
+        assert isinstance(self.OutShape, tuple) and len(self.OutShape) == 2, 'invalid out-shape : {:}'.format(
+            self.OutShape)
+        # conv_per_position_flops = self.conv.kernel_size[0] * self.conv.kernel_size[1] * iC * oC / self.conv.groups
+        conv_per_position_flops = (self.conv.kernel_size[0] * self.conv.kernel_size[1] * 1.0 / self.conv.groups)
+        all_positions = self.OutShape[0] * self.OutShape[1]
+        flops = (conv_per_position_flops * all_positions / divide) * iC * oC
+        if self.conv.bias is not None: flops += all_positions / divide
+        return flops
+
+    def get_range(self):
+        return [self.choices]
+
+    def forward(self, inputs):
+        if self.search_mode == 'basic':
+            return self.basic_forward(inputs)
+        elif self.search_mode == 'search':
+            return self.search_forward(inputs)
+        else:
+            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
+
+    def search_forward(self, tuple_inputs):
+        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
+            type(tuple_inputs))
+        inputs, expected_inC, probability, index, prob = tuple_inputs
+        index, prob = torch.squeeze(index).tolist(), torch.squeeze(prob)
+        probability = torch.squeeze(probability)
+        assert len(index) == 2, 'invalid length : {:}'.format(index)
+        # compute expected flop
+        # coordinates   = torch.arange(self.x_range[0], self.x_range[1]+1).type_as(probability)
+        expected_outC = (self.choices_tensor * probability).sum()
+        expected_flop = self.get_flops([expected_inC, expected_outC], False, 1e6)
+        if self.avg:
+            out = self.avg(inputs)
+        else:
+            out = inputs
+        # convolutional layer
+        out_convs = conv_forward(out, self.conv, [self.choices[i] for i in index])
+        out_bns = [self.BNs[idx](out_conv) for idx, out_conv in zip(index, out_convs)]
+        # merge
+        out_channel = max([x.size(1) for x in out_bns])
+        outA = ChannelWiseInter(out_bns[0], out_channel)
+        outB = ChannelWiseInter(out_bns[1], out_channel)
+        out = outA * prob[0] + outB * prob[1]
+        # out = additive_func(out_bns[0]*prob[0], out_bns[1]*prob[1])
+
+        if self.relu:
+            out = self.relu(out)
+        else:
+            out = out
+        return out, expected_outC, expected_flop
+
+    def basic_forward(self, inputs):
+        if self.avg:
+            out = self.avg(inputs)
+        else:
+            out = inputs
+        conv = self.conv(out)
+        if self.has_bn:
+            out = self.BNs[-1](conv)
+        else:
+            out = conv
+        if self.relu:
+            out = self.relu(out)
+        else:
+            out = out
+        if self.InShape is None:
+            self.InShape = (inputs.size(-2), inputs.size(-1))
+            self.OutShape = (out.size(-2), out.size(-1))
+        return out
+
+
+class ResNetBasicblock(nn.Module):
+    expansion = 1
+    num_conv = 2
+
+    def __init__(self, inplanes, planes, stride):
+        super(ResNetBasicblock, self).__init__()
+        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
+        self.conv_a = ConvBNReLU(inplanes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
+        self.conv_b = ConvBNReLU(planes, planes, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=False)
+        if stride == 2:
+            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=True, has_bn=False, has_relu=False)
+        elif inplanes != planes:
+            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=False)
+        else:
+            self.downsample = None
+        self.out_dim = planes
+        self.search_mode = 'basic'
+
+    def get_range(self):
+        return self.conv_a.get_range() + self.conv_b.get_range()
+
+    def get_flops(self, channels):
+        assert len(channels) == 3, 'invalid channels : {:}'.format(channels)
+        flop_A = self.conv_a.get_flops([channels[0], channels[1]])
+        flop_B = self.conv_b.get_flops([channels[1], channels[2]])
+        if hasattr(self.downsample, 'get_flops'):
+            flop_C = self.downsample.get_flops([channels[0], channels[-1]])
+        else:
+            flop_C = 0
+        if channels[0] != channels[
+            -1] and self.downsample is None:  # this short-cut will be added during the infer-train
+            flop_C = channels[0] * channels[-1] * self.conv_b.OutShape[0] * self.conv_b.OutShape[1]
+        return flop_A + flop_B + flop_C
+
+    def forward(self, inputs):
+        if self.search_mode == 'basic':
+            return self.basic_forward(inputs)
+        elif self.search_mode == 'search':
+            return self.search_forward(inputs)
+        else:
+            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
+
+    def search_forward(self, tuple_inputs):
+        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
+            type(tuple_inputs))
+        inputs, expected_inC, probability, indexes, probs = tuple_inputs
+        assert indexes.size(0) == 2 and probs.size(0) == 2 and probability.size(0) == 2
+        out_a, expected_inC_a, expected_flop_a = self.conv_a(
+            (inputs, expected_inC, probability[0], indexes[0], probs[0]))
+        out_b, expected_inC_b, expected_flop_b = self.conv_b(
+            (out_a, expected_inC_a, probability[1], indexes[1], probs[1]))
+        if self.downsample is not None:
+            residual, _, expected_flop_c = self.downsample((inputs, expected_inC, probability[1], indexes[1], probs[1]))
+        else:
+            residual, expected_flop_c = inputs, 0
+        out = additive_func(residual, out_b)
+        return nn.functional.relu(out, inplace=True), expected_inC_b, sum(
+            [expected_flop_a, expected_flop_b, expected_flop_c])
+
+    def basic_forward(self, inputs):
+        basicblock = self.conv_a(inputs)
+        basicblock = self.conv_b(basicblock)
+        if self.downsample is not None:
+            residual = self.downsample(inputs)
+        else:
+            residual = inputs
+        out = additive_func(residual, basicblock)
+        return nn.functional.relu(out, inplace=True)
+
+
+class ResNetBottleneck(nn.Module):
+    expansion = 4
+    num_conv = 3
+
+    def __init__(self, inplanes, planes, stride):
+        super(ResNetBottleneck, self).__init__()
+        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
+        self.conv_1x1 = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=True)
+        self.conv_3x3 = ConvBNReLU(planes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
+        self.conv_1x4 = ConvBNReLU(planes, planes * self.expansion, 1, 1, 0, False, has_avg=False, has_bn=True,
+                                   has_relu=False)
+        if stride == 2:
+            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, has_avg=True, has_bn=False,
+                                         has_relu=False)
+        elif inplanes != planes * self.expansion:
+            self.downsample = ConvBNReLU(inplanes, planes * self.expansion, 1, 1, 0, False, has_avg=False, has_bn=True,
+                                         has_relu=False)
+        else:
+            self.downsample = None
+        self.out_dim = planes * self.expansion
+        self.search_mode = 'basic'
+
+    def get_range(self):
+        return self.conv_1x1.get_range() + self.conv_3x3.get_range() + self.conv_1x4.get_range()
+
+    def get_flops(self, channels):
+        assert len(channels) == 4, 'invalid channels : {:}'.format(channels)
+        flop_A = self.conv_1x1.get_flops([channels[0], channels[1]])
+        flop_B = self.conv_3x3.get_flops([channels[1], channels[2]])
+        flop_C = self.conv_1x4.get_flops([channels[2], channels[3]])
+        if hasattr(self.downsample, 'get_flops'):
+            flop_D = self.downsample.get_flops([channels[0], channels[-1]])
+        else:
+            flop_D = 0
+        if channels[0] != channels[
+            -1] and self.downsample is None:  # this short-cut will be added during the infer-train
+            flop_D = channels[0] * channels[-1] * self.conv_1x4.OutShape[0] * self.conv_1x4.OutShape[1]
+        return flop_A + flop_B + flop_C + flop_D
+
+    def forward(self, inputs):
+        if self.search_mode == 'basic':
+            return self.basic_forward(inputs)
+        elif self.search_mode == 'search':
+            return self.search_forward(inputs)
+        else:
+            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
+
+    def basic_forward(self, inputs):
+        bottleneck = self.conv_1x1(inputs)
+        bottleneck = self.conv_3x3(bottleneck)
+        bottleneck = self.conv_1x4(bottleneck)
+        if self.downsample is not None:
+            residual = self.downsample(inputs)
+        else:
+            residual = inputs
+        out = additive_func(residual, bottleneck)
+        return nn.functional.relu(out, inplace=True)
+
+    def search_forward(self, tuple_inputs):
+        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
+            type(tuple_inputs))
+        inputs, expected_inC, probability, indexes, probs = tuple_inputs
+        assert indexes.size(0) == 3 and probs.size(0) == 3 and probability.size(0) == 3
+        out_1x1, expected_inC_1x1, expected_flop_1x1 = self.conv_1x1(
+            (inputs, expected_inC, probability[0], indexes[0], probs[0]))
+        out_3x3, expected_inC_3x3, expected_flop_3x3 = self.conv_3x3(
+            (out_1x1, expected_inC_1x1, probability[1], indexes[1], probs[1]))
+        out_1x4, expected_inC_1x4, expected_flop_1x4 = self.conv_1x4(
+            (out_3x3, expected_inC_3x3, probability[2], indexes[2], probs[2]))
+        if self.downsample is not None:
+            residual, _, expected_flop_c = self.downsample((inputs, expected_inC, probability[2], indexes[2], probs[2]))
+        else:
+            residual, expected_flop_c = inputs, 0
+        out = additive_func(residual, out_1x4)
+        return nn.functional.relu(out, inplace=True), expected_inC_1x4, sum(
+            [expected_flop_1x1, expected_flop_3x3, expected_flop_1x4, expected_flop_c])
+
+
+class SearchShapeCifarResNet(nn.Module):
+
+    def __init__(self, block_name, depth, num_classes):
+        super(SearchShapeCifarResNet, self).__init__()
+
+        # Model type specifies number of layers for CIFAR-10 and CIFAR-100 model
+        if block_name == 'ResNetBasicblock':
+            block = ResNetBasicblock
+            assert (depth - 2) % 6 == 0, 'depth should be one of 20, 32, 44, 56, 110'
+            layer_blocks = (depth - 2) // 6
+        elif block_name == 'ResNetBottleneck':
+            block = ResNetBottleneck
+            assert (depth - 2) % 9 == 0, 'depth should be one of 164'
+            layer_blocks = (depth - 2) // 9
+        else:
+            raise ValueError('invalid block : {:}'.format(block_name))
+
+        self.message = 'SearchShapeCifarResNet : Depth : {:} , Layers for each block : {:}'.format(depth, layer_blocks)
+        self.num_classes = num_classes
+        self.channels = [16]
+        self.layers = nn.ModuleList([ConvBNReLU(3, 16, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=True)])
+        self.InShape = None
+        self.depth_info = OrderedDict()
+        self.depth_at_i = OrderedDict()
+        for stage in range(3):
+            cur_block_choices = get_depth_choices(layer_blocks, False)
+            assert cur_block_choices[-1] == layer_blocks, 'stage={:}, {:} vs {:}'.format(stage, cur_block_choices,
+                                                                                         layer_blocks)
+            self.message += "\nstage={:} ::: depth-block-choices={:} for {:} blocks.".format(stage, cur_block_choices,
+                                                                                             layer_blocks)
+            block_choices, xstart = [], len(self.layers)
+            for iL in range(layer_blocks):
+                iC = self.channels[-1]
+                planes = 16 * (2 ** stage)
+                stride = 2 if stage > 0 and iL == 0 else 1
+                module = block(iC, planes, stride)
+                self.channels.append(module.out_dim)
+                self.layers.append(module)
+                self.message += "\nstage={:}, ilayer={:02d}/{:02d}, block={:03d}, iC={:3d}, oC={:3d}, stride={:}".format(
+                    stage, iL, layer_blocks, len(self.layers) - 1, iC, module.out_dim, stride)
+                # added for depth
+                layer_index = len(self.layers) - 1
+                if iL + 1 in cur_block_choices: block_choices.append(layer_index)
+                if iL + 1 == layer_blocks:
+                    self.depth_info[layer_index] = {'choices': block_choices,
+                                                    'stage': stage,
+                                                    'xstart': xstart}
+        self.depth_info_list = []
+        for xend, info in self.depth_info.items():
+            self.depth_info_list.append((xend, info))
+            xstart, xstage = info['xstart'], info['stage']
+            for ilayer in range(xstart, xend + 1):
+                idx = bisect_right(info['choices'], ilayer - 1)
+                self.depth_at_i[ilayer] = (xstage, idx)
+
+        self.avgpool = nn.AvgPool2d(8)
+        self.classifier = nn.Linear(module.out_dim, num_classes)
+        self.InShape = None
+        self.tau = -1
+        self.search_mode = 'basic'
+        # assert sum(x.num_conv for x in self.layers) + 1 == depth, 'invalid depth check {:} vs {:}'.format(sum(x.num_conv for x in self.layers)+1, depth)
+
+        # parameters for width
+        self.Ranges = []
+        self.layer2indexRange = []
+        for i, layer in enumerate(self.layers):
+            start_index = len(self.Ranges)
+            self.Ranges += layer.get_range()
+            self.layer2indexRange.append((start_index, len(self.Ranges)))
+        assert len(self.Ranges) + 1 == depth, 'invalid depth check {:} vs {:}'.format(len(self.Ranges) + 1, depth)
+
+        self.register_parameter('width_attentions',
+                                nn.Parameter(torch.Tensor(len(self.Ranges), get_width_choices(None))))
+        self.register_parameter('depth_attentions',
+                                nn.Parameter(torch.Tensor(3, get_depth_choices(layer_blocks, True))))
+        nn.init.normal_(self.width_attentions, 0, 0.01)
+        nn.init.normal_(self.depth_attentions, 0, 0.01)
+        self.apply(initialize_resnet)
+
+    def arch_parameters(self, LR=None):
+        if LR is None:
+            return [self.width_attentions, self.depth_attentions]
+        else:
+            return [
+                {"params": self.width_attentions, "lr": LR},
+                {"params": self.depth_attentions, "lr": LR},
+            ]
+
+    def base_parameters(self):
+        return list(self.layers.parameters()) + list(self.avgpool.parameters()) + list(self.classifier.parameters())
+
+    def get_flop(self, mode, config_dict, extra_info):
+        if config_dict is not None: config_dict = config_dict.copy()
+        # select channels
+        channels = [3]
+        for i, weight in enumerate(self.width_attentions):
+            if mode == 'genotype':
+                with torch.no_grad():
+                    probe = nn.functional.softmax(weight, dim=0)
+                    C = self.Ranges[i][torch.argmax(probe).item()]
+            elif mode == 'max':
+                C = self.Ranges[i][-1]
+            elif mode == 'fix':
+                C = int(math.sqrt(extra_info) * self.Ranges[i][-1])
+            elif mode == 'random':
+                assert isinstance(extra_info, float), 'invalid extra_info : {:}'.format(extra_info)
+                with torch.no_grad():
+                    prob = nn.functional.softmax(weight, dim=0)
+                    approximate_C = int(math.sqrt(extra_info) * self.Ranges[i][-1])
+                    for j in range(prob.size(0)):
+                        prob[j] = 1 / (abs(j - (approximate_C - self.Ranges[i][j])) + 0.2)
+                    C = self.Ranges[i][torch.multinomial(prob, 1, False).item()]
+            else:
+                raise ValueError('invalid mode : {:}'.format(mode))
+            channels.append(C)
+        # select depth
+        if mode == 'genotype':
+            with torch.no_grad():
+                depth_probs = nn.functional.softmax(self.depth_attentions, dim=1)
+                choices = torch.argmax(depth_probs, dim=1).cpu().tolist()
+        elif mode == 'max' or mode == 'fix':
+            choices = [depth_probs.size(1) - 1 for _ in range(depth_probs.size(0))]
+        elif mode == 'random':
+            with torch.no_grad():
+                depth_probs = nn.functional.softmax(self.depth_attentions, dim=1)
+                choices = torch.multinomial(depth_probs, 1, False).cpu().tolist()
+        else:
+            raise ValueError('invalid mode : {:}'.format(mode))
+        selected_layers = []
+        for choice, xvalue in zip(choices, self.depth_info_list):
+            xtemp = xvalue[1]['choices'][choice] - xvalue[1]['xstart'] + 1
+            selected_layers.append(xtemp)
+        flop = 0
+        for i, layer in enumerate(self.layers):
+            s, e = self.layer2indexRange[i]
+            xchl = tuple(channels[s:e + 1])
+            if i in self.depth_at_i:
+                xstagei, xatti = self.depth_at_i[i]
+                if xatti <= choices[xstagei]:  # leave this depth
+                    flop += layer.get_flops(xchl)
+                else:
+                    flop += 0  # do not use this layer
+            else:
+                flop += layer.get_flops(xchl)
+        # the last fc layer
+        flop += channels[-1] * self.classifier.out_features
+        if config_dict is None:
+            return flop / 1e6
+        else:
+            config_dict['xchannels'] = channels
+            config_dict['xblocks'] = selected_layers
+            config_dict['super_type'] = 'infer-shape'
+            config_dict['estimated_FLOP'] = flop / 1e6
+            return flop / 1e6, config_dict
+
+    def get_arch_info(self):
+        string = "for depth and width, there are {:} + {:} attention probabilities.".format(len(self.depth_attentions),
+                                                                                            len(self.width_attentions))
+        string += '\n{:}'.format(self.depth_info)
+        discrepancy = []
+        with torch.no_grad():
+            for i, att in enumerate(self.depth_attentions):
+                prob = nn.functional.softmax(att, dim=0)
+                prob = prob.cpu();
+                selc = prob.argmax().item();
+                prob = prob.tolist()
+                prob = ['{:.3f}'.format(x) for x in prob]
+                xstring = '{:03d}/{:03d}-th : {:}'.format(i, len(self.depth_attentions), ' '.join(prob))
+                logt = ['{:.4f}'.format(x) for x in att.cpu().tolist()]
+                xstring += '  ||  {:17s}'.format(' '.join(logt))
+                prob = sorted([float(x) for x in prob])
+                disc = prob[-1] - prob[-2]
+                xstring += '  || discrepancy={:.2f} || select={:}/{:}'.format(disc, selc, len(prob))
+                discrepancy.append(disc)
+                string += '\n{:}'.format(xstring)
+            string += '\n-----------------------------------------------'
+            for i, att in enumerate(self.width_attentions):
+                prob = nn.functional.softmax(att, dim=0)
+                prob = prob.cpu();
+                selc = prob.argmax().item();
+                prob = prob.tolist()
+                prob = ['{:.3f}'.format(x) for x in prob]
+                xstring = '{:03d}/{:03d}-th : {:}'.format(i, len(self.width_attentions), ' '.join(prob))
+                logt = ['{:.3f}'.format(x) for x in att.cpu().tolist()]
+                xstring += '  ||  {:52s}'.format(' '.join(logt))
+                prob = sorted([float(x) for x in prob])
+                disc = prob[-1] - prob[-2]
+                xstring += '  || dis={:.2f} || select={:}/{:}'.format(disc, selc, len(prob))
+                discrepancy.append(disc)
+                string += '\n{:}'.format(xstring)
+        return string, discrepancy
+
+    def set_tau(self, tau_max, tau_min, epoch_ratio):
+        assert epoch_ratio >= 0 and epoch_ratio <= 1, 'invalid epoch-ratio : {:}'.format(epoch_ratio)
+        tau = tau_min + (tau_max - tau_min) * (1 + math.cos(math.pi * epoch_ratio)) / 2
+        self.tau = tau
+
+    def get_message(self):
+        return self.message
+
+    def forward(self, inputs):
+        if self.search_mode == 'basic':
+            return self.basic_forward(inputs)
+        elif self.search_mode == 'search':
+            return self.search_forward(inputs)
+        else:
+            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
+
+    def search_forward(self, inputs):
+        flop_width_probs = nn.functional.softmax(self.width_attentions, dim=1)
+        flop_depth_probs = nn.functional.softmax(self.depth_attentions, dim=1)
+        flop_depth_probs = torch.flip(torch.cumsum(torch.flip(flop_depth_probs, [1]), 1), [1])
+        selected_widths, selected_width_probs = select2withP(self.width_attentions, self.tau)
+        selected_depth_probs = select2withP(self.depth_attentions, self.tau, True)
+        with torch.no_grad():
+            selected_widths = selected_widths.cpu()
+
+        x, last_channel_idx, expected_inC, flops = inputs, 0, 3, []
+        feature_maps = []
+        for i, layer in enumerate(self.layers):
+            selected_w_index = selected_widths[last_channel_idx: last_channel_idx + layer.num_conv]
+            selected_w_probs = selected_width_probs[last_channel_idx: last_channel_idx + layer.num_conv]
+            layer_prob = flop_width_probs[last_channel_idx: last_channel_idx + layer.num_conv]
+            x, expected_inC, expected_flop = layer((x, expected_inC, layer_prob, selected_w_index, selected_w_probs))
+            feature_maps.append(x)
+            last_channel_idx += layer.num_conv
+            if i in self.depth_info:  # aggregate the information
+                choices = self.depth_info[i]['choices']
+                xstagei = self.depth_info[i]['stage']
+                # print ('iL={:}, choices={:}, stage={:}, probs={:}'.format(i, choices, xstagei, selected_depth_probs[xstagei].cpu().tolist()))
+                # for A, W in zip(choices, selected_depth_probs[xstagei]):
+                #  print('Size = {:}, W = {:}'.format(feature_maps[A].size(), W))
+                possible_tensors = []
+                max_C = max(feature_maps[A].size(1) for A in choices)
+                for tempi, A in enumerate(choices):
+                    xtensor = ChannelWiseInter(feature_maps[A], max_C)
+                    # drop_ratio = 1-(tempi+1.0)/len(choices)
+                    # xtensor = drop_path(xtensor, drop_ratio)
+                    possible_tensors.append(xtensor)
+                weighted_sum = sum(xtensor * W for xtensor, W in zip(possible_tensors, selected_depth_probs[xstagei]))
+                x = weighted_sum
+
+            if i in self.depth_at_i:
+                xstagei, xatti = self.depth_at_i[i]
+                x_expected_flop = flop_depth_probs[xstagei, xatti] * expected_flop
+            else:
+                x_expected_flop = expected_flop
+            flops.append(x_expected_flop)
+        flops.append(expected_inC * (self.classifier.out_features * 1.0 / 1e6))
+        features = self.avgpool(x)
+        features = features.view(features.size(0), -1)
+        logits = linear_forward(features, self.classifier)
+        return logits, torch.stack([sum(flops)])
+
+    def basic_forward(self, inputs):
+        if self.InShape is None: self.InShape = (inputs.size(-2), inputs.size(-1))
+        x = inputs
+        for i, layer in enumerate(self.layers):
+            x = layer(x)
+        features = self.avgpool(x)
+        features = features.view(features.size(0), -1)
+        logits = self.classifier(features)
+        return features, logits
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchSimResNet_width.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SearchSimResNet_width.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,347 +1,347 @@
-##################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
-##################################################
-import math, torch
-import torch.nn as nn
-from ..initialization import initialize_resnet
-from ..SharedUtils import additive_func
-from .SoftSelect import select2withP, ChannelWiseInter
-from .SoftSelect import linear_forward
-from .SoftSelect import get_width_choices as get_choices
-
-
-def conv_forward(inputs, conv, choices):
-    iC = conv.in_channels
-    fill_size = list(inputs.size())
-    fill_size[1] = iC - fill_size[1]
-    filled = torch.zeros(fill_size, device=inputs.device)
-    xinputs = torch.cat((inputs, filled), dim=1)
-    outputs = conv(xinputs)
-    selecteds = [outputs[:, :oC] for oC in choices]
-    return selecteds
-
-
-class ConvBNReLU(nn.Module):
-    num_conv = 1
-
-    def __init__(self, nIn, nOut, kernel, stride, padding, bias, has_avg, has_bn, has_relu):
-        super(ConvBNReLU, self).__init__()
-        self.InShape = None
-        self.OutShape = None
-        self.choices = get_choices(nOut)
-        self.register_buffer('choices_tensor', torch.Tensor(self.choices))
-
-        if has_avg:
-            self.avg = nn.AvgPool2d(kernel_size=2, stride=2, padding=0)
-        else:
-            self.avg = None
-        self.conv = nn.Conv2d(nIn, nOut, kernel_size=kernel, stride=stride, padding=padding, dilation=1, groups=1,
-                              bias=bias)
-        # if has_bn  : self.bn  = nn.BatchNorm2d(nOut)
-        # else       : self.bn  = None
-        self.has_bn = has_bn
-        self.BNs = nn.ModuleList()
-        for i, _out in enumerate(self.choices):
-            self.BNs.append(nn.BatchNorm2d(_out))
-        if has_relu:
-            self.relu = nn.ReLU(inplace=True)
-        else:
-            self.relu = None
-        self.in_dim = nIn
-        self.out_dim = nOut
-        self.search_mode = 'basic'
-
-    def get_flops(self, channels, check_range=True, divide=1):
-        iC, oC = channels
-        if check_range: assert iC <= self.conv.in_channels and oC <= self.conv.out_channels, '{:} vs {:}  |  {:} vs {:}'.format(
-            iC, self.conv.in_channels, oC, self.conv.out_channels)
-        assert isinstance(self.InShape, tuple) and len(self.InShape) == 2, 'invalid in-shape : {:}'.format(self.InShape)
-        assert isinstance(self.OutShape, tuple) and len(self.OutShape) == 2, 'invalid out-shape : {:}'.format(
-            self.OutShape)
-        # conv_per_position_flops = self.conv.kernel_size[0] * self.conv.kernel_size[1] * iC * oC / self.conv.groups
-        conv_per_position_flops = (self.conv.kernel_size[0] * self.conv.kernel_size[1] * 1.0 / self.conv.groups)
-        all_positions = self.OutShape[0] * self.OutShape[1]
-        flops = (conv_per_position_flops * all_positions / divide) * iC * oC
-        if self.conv.bias is not None: flops += all_positions / divide
-        return flops
-
-    def get_range(self):
-        return [self.choices]
-
-    def forward(self, inputs):
-        if self.search_mode == 'basic':
-            return self.basic_forward(inputs)
-        elif self.search_mode == 'search':
-            return self.search_forward(inputs)
-        else:
-            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
-
-    def search_forward(self, tuple_inputs):
-        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
-            type(tuple_inputs))
-        inputs, expected_inC, probability, index, prob = tuple_inputs
-        index, prob = torch.squeeze(index).tolist(), torch.squeeze(prob)
-        probability = torch.squeeze(probability)
-        assert len(index) == 2, 'invalid length : {:}'.format(index)
-        # compute expected flop
-        # coordinates   = torch.arange(self.x_range[0], self.x_range[1]+1).type_as(probability)
-        expected_outC = (self.choices_tensor * probability).sum()
-        expected_flop = self.get_flops([expected_inC, expected_outC], False, 1e6)
-        if self.avg:
-            out = self.avg(inputs)
-        else:
-            out = inputs
-        # convolutional layer
-        out_convs = conv_forward(out, self.conv, [self.choices[i] for i in index])
-        out_bns = [self.BNs[idx](out_conv) for idx, out_conv in zip(index, out_convs)]
-        # merge
-        out_channel = max([x.size(1) for x in out_bns])
-        outA = ChannelWiseInter(out_bns[0], out_channel)
-        outB = ChannelWiseInter(out_bns[1], out_channel)
-        out = outA * prob[0] + outB * prob[1]
-        # out = additive_func(out_bns[0]*prob[0], out_bns[1]*prob[1])
-
-        if self.relu:
-            out = self.relu(out)
-        else:
-            out = out
-        return out, expected_outC, expected_flop
-
-    def basic_forward(self, inputs):
-        if self.avg:
-            out = self.avg(inputs)
-        else:
-            out = inputs
-        conv = self.conv(out)
-        if self.has_bn:
-            out = self.BNs[-1](conv)
-        else:
-            out = conv
-        if self.relu:
-            out = self.relu(out)
-        else:
-            out = out
-        if self.InShape is None:
-            self.InShape = (inputs.size(-2), inputs.size(-1))
-            self.OutShape = (out.size(-2), out.size(-1))
-        return out
-
-
-class SimBlock(nn.Module):
-    expansion = 1
-    num_conv = 1
-
-    def __init__(self, inplanes, planes, stride):
-        super(SimBlock, self).__init__()
-        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
-        self.conv = ConvBNReLU(inplanes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
-        if stride == 2:
-            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=True, has_bn=False, has_relu=False)
-        elif inplanes != planes:
-            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=False)
-        else:
-            self.downsample = None
-        self.out_dim = planes
-        self.search_mode = 'basic'
-
-    def get_range(self):
-        return self.conv.get_range()
-
-    def get_flops(self, channels):
-        assert len(channels) == 2, 'invalid channels : {:}'.format(channels)
-        flop_A = self.conv.get_flops([channels[0], channels[1]])
-        if hasattr(self.downsample, 'get_flops'):
-            flop_C = self.downsample.get_flops([channels[0], channels[-1]])
-        else:
-            flop_C = 0
-        if channels[0] != channels[
-            -1] and self.downsample is None:  # this short-cut will be added during the infer-train
-            flop_C = channels[0] * channels[-1] * self.conv.OutShape[0] * self.conv.OutShape[1]
-        return flop_A + flop_C
-
-    def forward(self, inputs):
-        if self.search_mode == 'basic':
-            return self.basic_forward(inputs)
-        elif self.search_mode == 'search':
-            return self.search_forward(inputs)
-        else:
-            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
-
-    def search_forward(self, tuple_inputs):
-        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
-            type(tuple_inputs))
-        inputs, expected_inC, probability, indexes, probs = tuple_inputs
-        assert indexes.size(0) == 1 and probs.size(0) == 1 and probability.size(
-            0) == 1, 'invalid size : {:}, {:}, {:}'.format(indexes.size(), probs.size(), probability.size())
-        out, expected_next_inC, expected_flop = self.conv((inputs, expected_inC, probability[0], indexes[0], probs[0]))
-        if self.downsample is not None:
-            residual, _, expected_flop_c = self.downsample(
-                (inputs, expected_inC, probability[-1], indexes[-1], probs[-1]))
-        else:
-            residual, expected_flop_c = inputs, 0
-        out = additive_func(residual, out)
-        return nn.functional.relu(out, inplace=True), expected_next_inC, sum([expected_flop, expected_flop_c])
-
-    def basic_forward(self, inputs):
-        basicblock = self.conv(inputs)
-        if self.downsample is not None:
-            residual = self.downsample(inputs)
-        else:
-            residual = inputs
-        out = additive_func(residual, basicblock)
-        return nn.functional.relu(out, inplace=True)
-
-
-class SearchWidthSimResNet(nn.Module):
-
-    def __init__(self, depth, num_classes):
-        super(SearchWidthSimResNet, self).__init__()
-
-        assert (depth - 2) % 3 == 0, 'depth should be one of 5, 8, 11, 14, ... instead of {:}'.format(depth)
-        layer_blocks = (depth - 2) // 3
-        self.message = 'SearchWidthSimResNet : Depth : {:} , Layers for each block : {:}'.format(depth, layer_blocks)
-        self.num_classes = num_classes
-        self.channels = [16]
-        self.layers = nn.ModuleList([ConvBNReLU(3, 16, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=True)])
-        self.InShape = None
-        for stage in range(3):
-            for iL in range(layer_blocks):
-                iC = self.channels[-1]
-                planes = 16 * (2 ** stage)
-                stride = 2 if stage > 0 and iL == 0 else 1
-                module = SimBlock(iC, planes, stride)
-                self.channels.append(module.out_dim)
-                self.layers.append(module)
-                self.message += "\nstage={:}, ilayer={:02d}/{:02d}, block={:03d}, iC={:3d}, oC={:3d}, stride={:}".format(
-                    stage, iL, layer_blocks, len(self.layers) - 1, iC, module.out_dim, stride)
-
-        self.avgpool = nn.AvgPool2d(8)
-        self.classifier = nn.Linear(module.out_dim, num_classes)
-        self.InShape = None
-        self.tau = -1
-        self.search_mode = 'basic'
-        # assert sum(x.num_conv for x in self.layers) + 1 == depth, 'invalid depth check {:} vs {:}'.format(sum(x.num_conv for x in self.layers)+1, depth)
-
-        # parameters for width
-        self.Ranges = []
-        self.layer2indexRange = []
-        for i, layer in enumerate(self.layers):
-            start_index = len(self.Ranges)
-            self.Ranges += layer.get_range()
-            self.layer2indexRange.append((start_index, len(self.Ranges)))
-        assert len(self.Ranges) + 1 == depth, 'invalid depth check {:} vs {:}'.format(len(self.Ranges) + 1, depth)
-
-        self.register_parameter('width_attentions', nn.Parameter(torch.Tensor(len(self.Ranges), get_choices(None))))
-        nn.init.normal_(self.width_attentions, 0, 0.01)
-        self.apply(initialize_resnet)
-
-    def arch_parameters(self):
-        return [self.width_attentions]
-
-    def base_parameters(self):
-        return list(self.layers.parameters()) + list(self.avgpool.parameters()) + list(self.classifier.parameters())
-
-    def get_flop(self, mode, config_dict, extra_info):
-        if config_dict is not None: config_dict = config_dict.copy()
-        # weights = [F.softmax(x, dim=0) for x in self.width_attentions]
-        channels = [3]
-        for i, weight in enumerate(self.width_attentions):
-            if mode == 'genotype':
-                with torch.no_grad():
-                    probe = nn.functional.softmax(weight, dim=0)
-                    C = self.Ranges[i][torch.argmax(probe).item()]
-            elif mode == 'max':
-                C = self.Ranges[i][-1]
-            elif mode == 'fix':
-                C = int(math.sqrt(extra_info) * self.Ranges[i][-1])
-            elif mode == 'random':
-                assert isinstance(extra_info, float), 'invalid extra_info : {:}'.format(extra_info)
-                with torch.no_grad():
-                    prob = nn.functional.softmax(weight, dim=0)
-                    approximate_C = int(math.sqrt(extra_info) * self.Ranges[i][-1])
-                    for j in range(prob.size(0)):
-                        prob[j] = 1 / (abs(j - (approximate_C - self.Ranges[i][j])) + 0.2)
-                    C = self.Ranges[i][torch.multinomial(prob, 1, False).item()]
-            else:
-                raise ValueError('invalid mode : {:}'.format(mode))
-            channels.append(C)
-        flop = 0
-        for i, layer in enumerate(self.layers):
-            s, e = self.layer2indexRange[i]
-            xchl = tuple(channels[s:e + 1])
-            flop += layer.get_flops(xchl)
-        # the last fc layer
-        flop += channels[-1] * self.classifier.out_features
-        if config_dict is None:
-            return flop / 1e6
-        else:
-            config_dict['xchannels'] = channels
-            config_dict['super_type'] = 'infer-width'
-            config_dict['estimated_FLOP'] = flop / 1e6
-            return flop / 1e6, config_dict
-
-    def get_arch_info(self):
-        string = "for width, there are {:} attention probabilities.".format(len(self.width_attentions))
-        discrepancy = []
-        with torch.no_grad():
-            for i, att in enumerate(self.width_attentions):
-                prob = nn.functional.softmax(att, dim=0)
-                prob = prob.cpu();
-                selc = prob.argmax().item();
-                prob = prob.tolist()
-                prob = ['{:.3f}'.format(x) for x in prob]
-                xstring = '{:03d}/{:03d}-th : {:}'.format(i, len(self.width_attentions), ' '.join(prob))
-                logt = ['{:.3f}'.format(x) for x in att.cpu().tolist()]
-                xstring += '  ||  {:52s}'.format(' '.join(logt))
-                prob = sorted([float(x) for x in prob])
-                disc = prob[-1] - prob[-2]
-                xstring += '  || dis={:.2f} || select={:}/{:}'.format(disc, selc, len(prob))
-                discrepancy.append(disc)
-                string += '\n{:}'.format(xstring)
-        return string, discrepancy
-
-    def set_tau(self, tau_max, tau_min, epoch_ratio):
-        assert epoch_ratio >= 0 and epoch_ratio <= 1, 'invalid epoch-ratio : {:}'.format(epoch_ratio)
-        tau = tau_min + (tau_max - tau_min) * (1 + math.cos(math.pi * epoch_ratio)) / 2
-        self.tau = tau
-
-    def get_message(self):
-        return self.message
-
-    def forward(self, inputs):
-        if self.search_mode == 'basic':
-            return self.basic_forward(inputs)
-        elif self.search_mode == 'search':
-            return self.search_forward(inputs)
-        else:
-            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
-
-    def search_forward(self, inputs):
-        flop_probs = nn.functional.softmax(self.width_attentions, dim=1)
-        selected_widths, selected_probs = select2withP(self.width_attentions, self.tau)
-        with torch.no_grad():
-            selected_widths = selected_widths.cpu()
-
-        x, last_channel_idx, expected_inC, flops = inputs, 0, 3, []
-        for i, layer in enumerate(self.layers):
-            selected_w_index = selected_widths[last_channel_idx: last_channel_idx + layer.num_conv]
-            selected_w_probs = selected_probs[last_channel_idx: last_channel_idx + layer.num_conv]
-            layer_prob = flop_probs[last_channel_idx: last_channel_idx + layer.num_conv]
-            x, expected_inC, expected_flop = layer((x, expected_inC, layer_prob, selected_w_index, selected_w_probs))
-            last_channel_idx += layer.num_conv
-            flops.append(expected_flop)
-        flops.append(expected_inC * (self.classifier.out_features * 1.0 / 1e6))
-        features = self.avgpool(x)
-        features = features.view(features.size(0), -1)
-        logits = linear_forward(features, self.classifier)
-        return logits, torch.stack([sum(flops)])
-
-    def basic_forward(self, inputs):
-        if self.InShape is None: self.InShape = (inputs.size(-2), inputs.size(-1))
-        x = inputs
-        for i, layer in enumerate(self.layers):
-            x = layer(x)
-        features = self.avgpool(x)
-        features = features.view(features.size(0), -1)
-        logits = self.classifier(features)
-        return features, logits
+##################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
+##################################################
+import math, torch
+import torch.nn as nn
+from ..initialization import initialize_resnet
+from ..SharedUtils import additive_func
+from .SoftSelect import select2withP, ChannelWiseInter
+from .SoftSelect import linear_forward
+from .SoftSelect import get_width_choices as get_choices
+
+
+def conv_forward(inputs, conv, choices):
+    iC = conv.in_channels
+    fill_size = list(inputs.size())
+    fill_size[1] = iC - fill_size[1]
+    filled = torch.zeros(fill_size, device=inputs.device)
+    xinputs = torch.cat((inputs, filled), dim=1)
+    outputs = conv(xinputs)
+    selecteds = [outputs[:, :oC] for oC in choices]
+    return selecteds
+
+
+class ConvBNReLU(nn.Module):
+    num_conv = 1
+
+    def __init__(self, nIn, nOut, kernel, stride, padding, bias, has_avg, has_bn, has_relu):
+        super(ConvBNReLU, self).__init__()
+        self.InShape = None
+        self.OutShape = None
+        self.choices = get_choices(nOut)
+        self.register_buffer('choices_tensor', torch.Tensor(self.choices))
+
+        if has_avg:
+            self.avg = nn.AvgPool2d(kernel_size=2, stride=2, padding=0)
+        else:
+            self.avg = None
+        self.conv = nn.Conv2d(nIn, nOut, kernel_size=kernel, stride=stride, padding=padding, dilation=1, groups=1,
+                              bias=bias)
+        # if has_bn  : self.bn  = nn.BatchNorm2d(nOut)
+        # else       : self.bn  = None
+        self.has_bn = has_bn
+        self.BNs = nn.ModuleList()
+        for i, _out in enumerate(self.choices):
+            self.BNs.append(nn.BatchNorm2d(_out))
+        if has_relu:
+            self.relu = nn.ReLU(inplace=True)
+        else:
+            self.relu = None
+        self.in_dim = nIn
+        self.out_dim = nOut
+        self.search_mode = 'basic'
+
+    def get_flops(self, channels, check_range=True, divide=1):
+        iC, oC = channels
+        if check_range: assert iC <= self.conv.in_channels and oC <= self.conv.out_channels, '{:} vs {:}  |  {:} vs {:}'.format(
+            iC, self.conv.in_channels, oC, self.conv.out_channels)
+        assert isinstance(self.InShape, tuple) and len(self.InShape) == 2, 'invalid in-shape : {:}'.format(self.InShape)
+        assert isinstance(self.OutShape, tuple) and len(self.OutShape) == 2, 'invalid out-shape : {:}'.format(
+            self.OutShape)
+        # conv_per_position_flops = self.conv.kernel_size[0] * self.conv.kernel_size[1] * iC * oC / self.conv.groups
+        conv_per_position_flops = (self.conv.kernel_size[0] * self.conv.kernel_size[1] * 1.0 / self.conv.groups)
+        all_positions = self.OutShape[0] * self.OutShape[1]
+        flops = (conv_per_position_flops * all_positions / divide) * iC * oC
+        if self.conv.bias is not None: flops += all_positions / divide
+        return flops
+
+    def get_range(self):
+        return [self.choices]
+
+    def forward(self, inputs):
+        if self.search_mode == 'basic':
+            return self.basic_forward(inputs)
+        elif self.search_mode == 'search':
+            return self.search_forward(inputs)
+        else:
+            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
+
+    def search_forward(self, tuple_inputs):
+        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
+            type(tuple_inputs))
+        inputs, expected_inC, probability, index, prob = tuple_inputs
+        index, prob = torch.squeeze(index).tolist(), torch.squeeze(prob)
+        probability = torch.squeeze(probability)
+        assert len(index) == 2, 'invalid length : {:}'.format(index)
+        # compute expected flop
+        # coordinates   = torch.arange(self.x_range[0], self.x_range[1]+1).type_as(probability)
+        expected_outC = (self.choices_tensor * probability).sum()
+        expected_flop = self.get_flops([expected_inC, expected_outC], False, 1e6)
+        if self.avg:
+            out = self.avg(inputs)
+        else:
+            out = inputs
+        # convolutional layer
+        out_convs = conv_forward(out, self.conv, [self.choices[i] for i in index])
+        out_bns = [self.BNs[idx](out_conv) for idx, out_conv in zip(index, out_convs)]
+        # merge
+        out_channel = max([x.size(1) for x in out_bns])
+        outA = ChannelWiseInter(out_bns[0], out_channel)
+        outB = ChannelWiseInter(out_bns[1], out_channel)
+        out = outA * prob[0] + outB * prob[1]
+        # out = additive_func(out_bns[0]*prob[0], out_bns[1]*prob[1])
+
+        if self.relu:
+            out = self.relu(out)
+        else:
+            out = out
+        return out, expected_outC, expected_flop
+
+    def basic_forward(self, inputs):
+        if self.avg:
+            out = self.avg(inputs)
+        else:
+            out = inputs
+        conv = self.conv(out)
+        if self.has_bn:
+            out = self.BNs[-1](conv)
+        else:
+            out = conv
+        if self.relu:
+            out = self.relu(out)
+        else:
+            out = out
+        if self.InShape is None:
+            self.InShape = (inputs.size(-2), inputs.size(-1))
+            self.OutShape = (out.size(-2), out.size(-1))
+        return out
+
+
+class SimBlock(nn.Module):
+    expansion = 1
+    num_conv = 1
+
+    def __init__(self, inplanes, planes, stride):
+        super(SimBlock, self).__init__()
+        assert stride == 1 or stride == 2, 'invalid stride {:}'.format(stride)
+        self.conv = ConvBNReLU(inplanes, planes, 3, stride, 1, False, has_avg=False, has_bn=True, has_relu=True)
+        if stride == 2:
+            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=True, has_bn=False, has_relu=False)
+        elif inplanes != planes:
+            self.downsample = ConvBNReLU(inplanes, planes, 1, 1, 0, False, has_avg=False, has_bn=True, has_relu=False)
+        else:
+            self.downsample = None
+        self.out_dim = planes
+        self.search_mode = 'basic'
+
+    def get_range(self):
+        return self.conv.get_range()
+
+    def get_flops(self, channels):
+        assert len(channels) == 2, 'invalid channels : {:}'.format(channels)
+        flop_A = self.conv.get_flops([channels[0], channels[1]])
+        if hasattr(self.downsample, 'get_flops'):
+            flop_C = self.downsample.get_flops([channels[0], channels[-1]])
+        else:
+            flop_C = 0
+        if channels[0] != channels[
+            -1] and self.downsample is None:  # this short-cut will be added during the infer-train
+            flop_C = channels[0] * channels[-1] * self.conv.OutShape[0] * self.conv.OutShape[1]
+        return flop_A + flop_C
+
+    def forward(self, inputs):
+        if self.search_mode == 'basic':
+            return self.basic_forward(inputs)
+        elif self.search_mode == 'search':
+            return self.search_forward(inputs)
+        else:
+            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
+
+    def search_forward(self, tuple_inputs):
+        assert isinstance(tuple_inputs, tuple) and len(tuple_inputs) == 5, 'invalid type input : {:}'.format(
+            type(tuple_inputs))
+        inputs, expected_inC, probability, indexes, probs = tuple_inputs
+        assert indexes.size(0) == 1 and probs.size(0) == 1 and probability.size(
+            0) == 1, 'invalid size : {:}, {:}, {:}'.format(indexes.size(), probs.size(), probability.size())
+        out, expected_next_inC, expected_flop = self.conv((inputs, expected_inC, probability[0], indexes[0], probs[0]))
+        if self.downsample is not None:
+            residual, _, expected_flop_c = self.downsample(
+                (inputs, expected_inC, probability[-1], indexes[-1], probs[-1]))
+        else:
+            residual, expected_flop_c = inputs, 0
+        out = additive_func(residual, out)
+        return nn.functional.relu(out, inplace=True), expected_next_inC, sum([expected_flop, expected_flop_c])
+
+    def basic_forward(self, inputs):
+        basicblock = self.conv(inputs)
+        if self.downsample is not None:
+            residual = self.downsample(inputs)
+        else:
+            residual = inputs
+        out = additive_func(residual, basicblock)
+        return nn.functional.relu(out, inplace=True)
+
+
+class SearchWidthSimResNet(nn.Module):
+
+    def __init__(self, depth, num_classes):
+        super(SearchWidthSimResNet, self).__init__()
+
+        assert (depth - 2) % 3 == 0, 'depth should be one of 5, 8, 11, 14, ... instead of {:}'.format(depth)
+        layer_blocks = (depth - 2) // 3
+        self.message = 'SearchWidthSimResNet : Depth : {:} , Layers for each block : {:}'.format(depth, layer_blocks)
+        self.num_classes = num_classes
+        self.channels = [16]
+        self.layers = nn.ModuleList([ConvBNReLU(3, 16, 3, 1, 1, False, has_avg=False, has_bn=True, has_relu=True)])
+        self.InShape = None
+        for stage in range(3):
+            for iL in range(layer_blocks):
+                iC = self.channels[-1]
+                planes = 16 * (2 ** stage)
+                stride = 2 if stage > 0 and iL == 0 else 1
+                module = SimBlock(iC, planes, stride)
+                self.channels.append(module.out_dim)
+                self.layers.append(module)
+                self.message += "\nstage={:}, ilayer={:02d}/{:02d}, block={:03d}, iC={:3d}, oC={:3d}, stride={:}".format(
+                    stage, iL, layer_blocks, len(self.layers) - 1, iC, module.out_dim, stride)
+
+        self.avgpool = nn.AvgPool2d(8)
+        self.classifier = nn.Linear(module.out_dim, num_classes)
+        self.InShape = None
+        self.tau = -1
+        self.search_mode = 'basic'
+        # assert sum(x.num_conv for x in self.layers) + 1 == depth, 'invalid depth check {:} vs {:}'.format(sum(x.num_conv for x in self.layers)+1, depth)
+
+        # parameters for width
+        self.Ranges = []
+        self.layer2indexRange = []
+        for i, layer in enumerate(self.layers):
+            start_index = len(self.Ranges)
+            self.Ranges += layer.get_range()
+            self.layer2indexRange.append((start_index, len(self.Ranges)))
+        assert len(self.Ranges) + 1 == depth, 'invalid depth check {:} vs {:}'.format(len(self.Ranges) + 1, depth)
+
+        self.register_parameter('width_attentions', nn.Parameter(torch.Tensor(len(self.Ranges), get_choices(None))))
+        nn.init.normal_(self.width_attentions, 0, 0.01)
+        self.apply(initialize_resnet)
+
+    def arch_parameters(self):
+        return [self.width_attentions]
+
+    def base_parameters(self):
+        return list(self.layers.parameters()) + list(self.avgpool.parameters()) + list(self.classifier.parameters())
+
+    def get_flop(self, mode, config_dict, extra_info):
+        if config_dict is not None: config_dict = config_dict.copy()
+        # weights = [F.softmax(x, dim=0) for x in self.width_attentions]
+        channels = [3]
+        for i, weight in enumerate(self.width_attentions):
+            if mode == 'genotype':
+                with torch.no_grad():
+                    probe = nn.functional.softmax(weight, dim=0)
+                    C = self.Ranges[i][torch.argmax(probe).item()]
+            elif mode == 'max':
+                C = self.Ranges[i][-1]
+            elif mode == 'fix':
+                C = int(math.sqrt(extra_info) * self.Ranges[i][-1])
+            elif mode == 'random':
+                assert isinstance(extra_info, float), 'invalid extra_info : {:}'.format(extra_info)
+                with torch.no_grad():
+                    prob = nn.functional.softmax(weight, dim=0)
+                    approximate_C = int(math.sqrt(extra_info) * self.Ranges[i][-1])
+                    for j in range(prob.size(0)):
+                        prob[j] = 1 / (abs(j - (approximate_C - self.Ranges[i][j])) + 0.2)
+                    C = self.Ranges[i][torch.multinomial(prob, 1, False).item()]
+            else:
+                raise ValueError('invalid mode : {:}'.format(mode))
+            channels.append(C)
+        flop = 0
+        for i, layer in enumerate(self.layers):
+            s, e = self.layer2indexRange[i]
+            xchl = tuple(channels[s:e + 1])
+            flop += layer.get_flops(xchl)
+        # the last fc layer
+        flop += channels[-1] * self.classifier.out_features
+        if config_dict is None:
+            return flop / 1e6
+        else:
+            config_dict['xchannels'] = channels
+            config_dict['super_type'] = 'infer-width'
+            config_dict['estimated_FLOP'] = flop / 1e6
+            return flop / 1e6, config_dict
+
+    def get_arch_info(self):
+        string = "for width, there are {:} attention probabilities.".format(len(self.width_attentions))
+        discrepancy = []
+        with torch.no_grad():
+            for i, att in enumerate(self.width_attentions):
+                prob = nn.functional.softmax(att, dim=0)
+                prob = prob.cpu();
+                selc = prob.argmax().item();
+                prob = prob.tolist()
+                prob = ['{:.3f}'.format(x) for x in prob]
+                xstring = '{:03d}/{:03d}-th : {:}'.format(i, len(self.width_attentions), ' '.join(prob))
+                logt = ['{:.3f}'.format(x) for x in att.cpu().tolist()]
+                xstring += '  ||  {:52s}'.format(' '.join(logt))
+                prob = sorted([float(x) for x in prob])
+                disc = prob[-1] - prob[-2]
+                xstring += '  || dis={:.2f} || select={:}/{:}'.format(disc, selc, len(prob))
+                discrepancy.append(disc)
+                string += '\n{:}'.format(xstring)
+        return string, discrepancy
+
+    def set_tau(self, tau_max, tau_min, epoch_ratio):
+        assert epoch_ratio >= 0 and epoch_ratio <= 1, 'invalid epoch-ratio : {:}'.format(epoch_ratio)
+        tau = tau_min + (tau_max - tau_min) * (1 + math.cos(math.pi * epoch_ratio)) / 2
+        self.tau = tau
+
+    def get_message(self):
+        return self.message
+
+    def forward(self, inputs):
+        if self.search_mode == 'basic':
+            return self.basic_forward(inputs)
+        elif self.search_mode == 'search':
+            return self.search_forward(inputs)
+        else:
+            raise ValueError('invalid search_mode = {:}'.format(self.search_mode))
+
+    def search_forward(self, inputs):
+        flop_probs = nn.functional.softmax(self.width_attentions, dim=1)
+        selected_widths, selected_probs = select2withP(self.width_attentions, self.tau)
+        with torch.no_grad():
+            selected_widths = selected_widths.cpu()
+
+        x, last_channel_idx, expected_inC, flops = inputs, 0, 3, []
+        for i, layer in enumerate(self.layers):
+            selected_w_index = selected_widths[last_channel_idx: last_channel_idx + layer.num_conv]
+            selected_w_probs = selected_probs[last_channel_idx: last_channel_idx + layer.num_conv]
+            layer_prob = flop_probs[last_channel_idx: last_channel_idx + layer.num_conv]
+            x, expected_inC, expected_flop = layer((x, expected_inC, layer_prob, selected_w_index, selected_w_probs))
+            last_channel_idx += layer.num_conv
+            flops.append(expected_flop)
+        flops.append(expected_inC * (self.classifier.out_features * 1.0 / 1e6))
+        features = self.avgpool(x)
+        features = features.view(features.size(0), -1)
+        logits = linear_forward(features, self.classifier)
+        return logits, torch.stack([sum(flops)])
+
+    def basic_forward(self, inputs):
+        if self.InShape is None: self.InShape = (inputs.size(-2), inputs.size(-1))
+        x = inputs
+        for i, layer in enumerate(self.layers):
+            x = layer(x)
+        features = self.avgpool(x)
+        features = features.view(features.size(0), -1)
+        logits = self.classifier(features)
+        return features, logits
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SoftSelect.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/SoftSelect.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-##################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
-##################################################
-import math, torch
-import torch.nn as nn
-
-
-def select2withP(logits, tau, just_prob=False, num=2, eps=1e-7):
-    if tau <= 0:
-        new_logits = logits
-        probs = nn.functional.softmax(new_logits, dim=1)
-    else:
-        while True:  # a trick to avoid the gumbels bug
-            gumbels = -torch.empty_like(logits).exponential_().log()
-            new_logits = (logits.log_softmax(dim=1) + gumbels) / tau
-            probs = nn.functional.softmax(new_logits, dim=1)
-            if (not torch.isinf(gumbels).any()) and (not torch.isinf(probs).any()) and (
-            not torch.isnan(probs).any()): break
-
-    if just_prob: return probs
-
-    # with torch.no_grad(): # add eps for unexpected torch error
-    #  probs = nn.functional.softmax(new_logits, dim=1)
-    #  selected_index = torch.multinomial(probs + eps, 2, False)
-    with torch.no_grad():  # add eps for unexpected torch error
-        probs = probs.cpu()
-        selected_index = torch.multinomial(probs + eps, num, False).to(logits.device)
-    selected_logit = torch.gather(new_logits, 1, selected_index)
-    selcted_probs = nn.functional.softmax(selected_logit, dim=1)
-    return selected_index, selcted_probs
-
-
-def ChannelWiseInter(inputs, oC, mode='v2'):
-    if mode == 'v1':
-        return ChannelWiseInterV1(inputs, oC)
-    elif mode == 'v2':
-        return ChannelWiseInterV2(inputs, oC)
-    else:
-        raise ValueError('invalid mode : {:}'.format(mode))
-
-
-def ChannelWiseInterV1(inputs, oC):
-    assert inputs.dim() == 4, 'invalid dimension : {:}'.format(inputs.size())
-
-    def start_index(a, b, c):
-        return int(math.floor(float(a * c) / b))
-
-    def end_index(a, b, c):
-        return int(math.ceil(float((a + 1) * c) / b))
-
-    batch, iC, H, W = inputs.size()
-    outputs = torch.zeros((batch, oC, H, W), dtype=inputs.dtype, device=inputs.device)
-    if iC == oC: return inputs
-    for ot in range(oC):
-        istartT, iendT = start_index(ot, oC, iC), end_index(ot, oC, iC)
-        values = inputs[:, istartT:iendT].mean(dim=1)
-        outputs[:, ot, :, :] = values
-    return outputs
-
-
-def ChannelWiseInterV2(inputs, oC):
-    assert inputs.dim() == 4, 'invalid dimension : {:}'.format(inputs.size())
-    batch, C, H, W = inputs.size()
-    if C == oC:
-        return inputs
-    else:
-        return nn.functional.adaptive_avg_pool3d(inputs, (oC, H, W))
-    # inputs_5D = inputs.view(batch, 1, C, H, W)
-    # otputs_5D = nn.functional.interpolate(inputs_5D, (oC,H,W), None, 'area', None)
-    # otputs    = otputs_5D.view(batch, oC, H, W)
-    # otputs_5D = nn.functional.interpolate(inputs_5D, (oC,H,W), None, 'trilinear', False)
-    # return otputs
-
-
-def linear_forward(inputs, linear):
-    if linear is None: return inputs
-    iC = inputs.size(1)
-    weight = linear.weight[:, :iC]
-    if linear.bias is None:
-        bias = None
-    else:
-        bias = linear.bias
-    return nn.functional.linear(inputs, weight, bias)
-
-
-def get_width_choices(nOut):
-    xsrange = [0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0]
-    if nOut is None:
-        return len(xsrange)
-    else:
-        Xs = [int(nOut * i) for i in xsrange]
-        # xs = [ int(nOut * i // 10) for i in range(2, 11)]
-        # Xs = [x for i, x in enumerate(xs) if i+1 == len(xs) or xs[i+1] > x+1]
-        Xs = sorted(list(set(Xs)))
-        return tuple(Xs)
-
-
-def get_depth_choices(nDepth):
-    if nDepth is None:
-        return 3
-    else:
-        assert nDepth >= 3, 'nDepth should be greater than 2 vs {:}'.format(nDepth)
-        if nDepth == 1:
-            return (1, 1, 1)
-        elif nDepth == 2:
-            return (1, 1, 2)
-        elif nDepth >= 3:
-            return (nDepth // 3, nDepth * 2 // 3, nDepth)
-        else:
-            raise ValueError('invalid Depth : {:}'.format(nDepth))
-
-
-def drop_path(x, drop_prob):
-    if drop_prob > 0.:
-        keep_prob = 1. - drop_prob
-        mask = x.new_zeros(x.size(0), 1, 1, 1)
-        mask = mask.bernoulli_(keep_prob)
-        x = x * (mask / keep_prob)
-        # x.div_(keep_prob)
-        # x.mul_(mask)
-    return x
+##################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
+##################################################
+import math, torch
+import torch.nn as nn
+
+
+def select2withP(logits, tau, just_prob=False, num=2, eps=1e-7):
+    if tau <= 0:
+        new_logits = logits
+        probs = nn.functional.softmax(new_logits, dim=1)
+    else:
+        while True:  # a trick to avoid the gumbels bug
+            gumbels = -torch.empty_like(logits).exponential_().log()
+            new_logits = (logits.log_softmax(dim=1) + gumbels) / tau
+            probs = nn.functional.softmax(new_logits, dim=1)
+            if (not torch.isinf(gumbels).any()) and (not torch.isinf(probs).any()) and (
+            not torch.isnan(probs).any()): break
+
+    if just_prob: return probs
+
+    # with torch.no_grad(): # add eps for unexpected torch error
+    #  probs = nn.functional.softmax(new_logits, dim=1)
+    #  selected_index = torch.multinomial(probs + eps, 2, False)
+    with torch.no_grad():  # add eps for unexpected torch error
+        probs = probs.cpu()
+        selected_index = torch.multinomial(probs + eps, num, False).to(logits.device)
+    selected_logit = torch.gather(new_logits, 1, selected_index)
+    selcted_probs = nn.functional.softmax(selected_logit, dim=1)
+    return selected_index, selcted_probs
+
+
+def ChannelWiseInter(inputs, oC, mode='v2'):
+    if mode == 'v1':
+        return ChannelWiseInterV1(inputs, oC)
+    elif mode == 'v2':
+        return ChannelWiseInterV2(inputs, oC)
+    else:
+        raise ValueError('invalid mode : {:}'.format(mode))
+
+
+def ChannelWiseInterV1(inputs, oC):
+    assert inputs.dim() == 4, 'invalid dimension : {:}'.format(inputs.size())
+
+    def start_index(a, b, c):
+        return int(math.floor(float(a * c) / b))
+
+    def end_index(a, b, c):
+        return int(math.ceil(float((a + 1) * c) / b))
+
+    batch, iC, H, W = inputs.size()
+    outputs = torch.zeros((batch, oC, H, W), dtype=inputs.dtype, device=inputs.device)
+    if iC == oC: return inputs
+    for ot in range(oC):
+        istartT, iendT = start_index(ot, oC, iC), end_index(ot, oC, iC)
+        values = inputs[:, istartT:iendT].mean(dim=1)
+        outputs[:, ot, :, :] = values
+    return outputs
+
+
+def ChannelWiseInterV2(inputs, oC):
+    assert inputs.dim() == 4, 'invalid dimension : {:}'.format(inputs.size())
+    batch, C, H, W = inputs.size()
+    if C == oC:
+        return inputs
+    else:
+        return nn.functional.adaptive_avg_pool3d(inputs, (oC, H, W))
+    # inputs_5D = inputs.view(batch, 1, C, H, W)
+    # otputs_5D = nn.functional.interpolate(inputs_5D, (oC,H,W), None, 'area', None)
+    # otputs    = otputs_5D.view(batch, oC, H, W)
+    # otputs_5D = nn.functional.interpolate(inputs_5D, (oC,H,W), None, 'trilinear', False)
+    # return otputs
+
+
+def linear_forward(inputs, linear):
+    if linear is None: return inputs
+    iC = inputs.size(1)
+    weight = linear.weight[:, :iC]
+    if linear.bias is None:
+        bias = None
+    else:
+        bias = linear.bias
+    return nn.functional.linear(inputs, weight, bias)
+
+
+def get_width_choices(nOut):
+    xsrange = [0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0]
+    if nOut is None:
+        return len(xsrange)
+    else:
+        Xs = [int(nOut * i) for i in xsrange]
+        # xs = [ int(nOut * i // 10) for i in range(2, 11)]
+        # Xs = [x for i, x in enumerate(xs) if i+1 == len(xs) or xs[i+1] > x+1]
+        Xs = sorted(list(set(Xs)))
+        return tuple(Xs)
+
+
+def get_depth_choices(nDepth):
+    if nDepth is None:
+        return 3
+    else:
+        assert nDepth >= 3, 'nDepth should be greater than 2 vs {:}'.format(nDepth)
+        if nDepth == 1:
+            return (1, 1, 1)
+        elif nDepth == 2:
+            return (1, 1, 2)
+        elif nDepth >= 3:
+            return (nDepth // 3, nDepth * 2 // 3, nDepth)
+        else:
+            raise ValueError('invalid Depth : {:}'.format(nDepth))
+
+
+def drop_path(x, drop_prob):
+    if drop_prob > 0.:
+        keep_prob = 1. - drop_prob
+        mask = x.new_zeros(x.size(0), 1, 1, 1)
+        mask = mask.bernoulli_(keep_prob)
+        x = x * (mask / keep_prob)
+        # x.div_(keep_prob)
+        # x.mul_(mask)
+    return x
```

### Comparing `evoxbench-1.0.2/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/test.py` & `evoxbench-1.0.3/evoxbench/database/hw_nas_bench_api/nas_201_models/shape_searchs/test.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-##################################################
-# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
-##################################################
-import torch
-import torch.nn as nn
-from SoftSelect import ChannelWiseInter
-
-if __name__ == '__main__':
-
-    tensors = torch.rand((16, 128, 7, 7))
-
-    for oc in range(200, 210):
-        out_v1 = ChannelWiseInter(tensors, oc, 'v1')
-        out_v2 = ChannelWiseInter(tensors, oc, 'v2')
-        assert (out_v1 == out_v2).any().item() == 1
-    for oc in range(48, 160):
-        out_v1 = ChannelWiseInter(tensors, oc, 'v1')
-        out_v2 = ChannelWiseInter(tensors, oc, 'v2')
-        assert (out_v1 == out_v2).any().item() == 1
+##################################################
+# Copyright (c) Xuanyi Dong [GitHub D-X-Y], 2019 #
+##################################################
+import torch
+import torch.nn as nn
+from SoftSelect import ChannelWiseInter
+
+if __name__ == '__main__':
+
+    tensors = torch.rand((16, 128, 7, 7))
+
+    for oc in range(200, 210):
+        out_v1 = ChannelWiseInter(tensors, oc, 'v1')
+        out_v2 = ChannelWiseInter(tensors, oc, 'v2')
+        assert (out_v1 == out_v2).any().item() == 1
+    for oc in range(48, 160):
+        out_v1 = ChannelWiseInter(tensors, oc, 'v1')
+        out_v2 = ChannelWiseInter(tensors, oc, 'v2')
+        assert (out_v1 == out_v2).any().item() == 1
```

### Comparing `evoxbench-1.0.2/evoxbench/database/init.py` & `evoxbench-1.0.3/evoxbench/database/init.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-import json
-import os
-import sys
-from pathlib import Path
-import traceback
-
-import django
-
-CONFIG_FILE_DIR = Path.home() / '.config' / 'evoxbench'
-CONFIG_FILE_PATH = CONFIG_FILE_DIR / 'config.json'
-
-
-def auto_config():
-    if not CONFIG_FILE_PATH.exists() or not CONFIG_FILE_PATH.is_file():
-        print("First time running evoxbench, please config the database path manually!")
-        return
-    try:
-        with open(CONFIG_FILE_PATH, "r", encoding='utf-8') as f:
-            if not f.readable():
-                print(f"Failed to read auto configuration file, path {CONFIG_FILE_PATH}")
-                return
-
-            config = json.load(f)
-            os.environ.setdefault("EVOXBENCH_DATA", config['database'])
-            if "model" in config:
-                os.environ.setdefault("EVOXBENCH_MODEL", config['model'])
-            sys.path.append(config['database'])
-            os.environ["DJANGO_ALLOW_ASYNC_UNSAFE"] = "true"
-            os.environ.setdefault('DJANGO_SETTINGS_MODULE', "ORM.settings")
-            django.setup()
-            print(f"Auto Configuration Succeed!, Using database {config['database']}.")
-    except Exception as e:
-        traceback.print_exc()
-        print(f"Auto Configuration file corrupted, path {CONFIG_FILE_PATH}, reason: {str(e)}")
-
-
-def init(cwd: str = ""):
-    cwd = cwd or str(Path(os.getcwd()) / "data")
-    os.environ.setdefault("EVOXBENCH_DATA", str(cwd))
-    sys.path.append(cwd)
-    os.environ["DJANGO_ALLOW_ASYNC_UNSAFE"] = "true"
-    os.environ.setdefault('DJANGO_SETTINGS_MODULE', "ORM.settings")
-    django.setup()
-
-
-def config(database_path: str, data_path: str):
-    CONFIG_FILE_DIR.mkdir(parents=True, exist_ok=True)
-    CONFIG_FILE_PATH.touch()
-    if CONFIG_FILE_PATH.is_file():
-        try:
-            config = {
-                'database': database_path,
-                'model': data_path
-            }
-            with open(CONFIG_FILE_PATH, "w", encoding='utf-8') as f:
-                json.dump(config, f)
-                print('Configuration Succeed!')
-                init(database_path)
-                return
-        except Exception as e:
-            raise e
-            print(f"Configuration Failed!\n{str(e)}")
-    print(f"Configuration Failed, it's not a regular file")
+import json
+import os
+import sys
+from pathlib import Path
+import traceback
+
+import django
+
+CONFIG_FILE_DIR = Path.home() / '.config' / 'evoxbench'
+CONFIG_FILE_PATH = CONFIG_FILE_DIR / 'config.json'
+
+
+def auto_config():
+    if not CONFIG_FILE_PATH.exists() or not CONFIG_FILE_PATH.is_file():
+        print("First time running evoxbench, please config the database path manually!")
+        return
+    try:
+        with open(CONFIG_FILE_PATH, "r", encoding='utf-8') as f:
+            if not f.readable():
+                print(f"Failed to read auto configuration file, path {CONFIG_FILE_PATH}")
+                return
+
+            config = json.load(f)
+            os.environ.setdefault("EVOXBENCH_DATA", config['database'])
+            if "model" in config:
+                os.environ.setdefault("EVOXBENCH_MODEL", config['model'])
+            sys.path.append(config['database'])
+            os.environ["DJANGO_ALLOW_ASYNC_UNSAFE"] = "true"
+            os.environ.setdefault('DJANGO_SETTINGS_MODULE', "ORM.settings")
+            django.setup()
+            print(f"Auto Configuration Succeed!, Using database {config['database']}.")
+    except Exception as e:
+        traceback.print_exc()
+        print(f"Auto Configuration file corrupted, path {CONFIG_FILE_PATH}, reason: {str(e)}")
+
+
+def init(cwd: str = ""):
+    cwd = cwd or str(Path(os.getcwd()) / "data")
+    os.environ.setdefault("EVOXBENCH_DATA", str(cwd))
+    sys.path.append(cwd)
+    os.environ["DJANGO_ALLOW_ASYNC_UNSAFE"] = "true"
+    os.environ.setdefault('DJANGO_SETTINGS_MODULE', "ORM.settings")
+    django.setup()
+
+
+def config(database_path: str, data_path: str):
+    CONFIG_FILE_DIR.mkdir(parents=True, exist_ok=True)
+    CONFIG_FILE_PATH.touch()
+    if CONFIG_FILE_PATH.is_file():
+        try:
+            config = {
+                'database': database_path,
+                'model': data_path
+            }
+            with open(CONFIG_FILE_PATH, "w", encoding='utf-8') as f:
+                json.dump(config, f)
+                print('Configuration Succeed!')
+                init(database_path)
+                return
+        except Exception as e:
+            raise e
+            print(f"Configuration Failed!\n{str(e)}")
+    print(f"Configuration Failed, it's not a regular file")
```

### Comparing `evoxbench-1.0.2/evoxbench/database/mobilenetv3/migrations/0001_initial.py` & `evoxbench-1.0.3/evoxbench/database/mobilenetv3/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Generated by Django 3.2.12 on 2022-05-07 14:56
-
-from django.db import migrations, models
-
-
-class Migration(migrations.Migration):
-    initial = True
-
-    dependencies = [
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='MobileNetV3Result',
-            fields=[
-                ('id', models.BigAutoField(primary_key=True, serialize=False)),
-                ('index', models.TextField(db_index=True, max_length=256, null=True)),
-                ('phenotype', models.JSONField(default=dict)),
-                ('genotype', models.JSONField(default=dict)),
-                ('result', models.JSONField(default=dict)),
-                ('params', models.IntegerField()),
-                ('flops', models.IntegerField()),
-                ('latency', models.FloatField()),
-                ('valid_acc', models.FloatField()),
-                ('test_acc', models.FloatField()),
-            ],
-            options={
-                'abstract': False,
-            },
-        ),
-    ]
+# Generated by Django 3.2.12 on 2022-05-07 14:56
+
+from django.db import migrations, models
+
+
+class Migration(migrations.Migration):
+    initial = True
+
+    dependencies = [
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='MobileNetV3Result',
+            fields=[
+                ('id', models.BigAutoField(primary_key=True, serialize=False)),
+                ('index', models.TextField(db_index=True, max_length=256, null=True)),
+                ('phenotype', models.JSONField(default=dict)),
+                ('genotype', models.JSONField(default=dict)),
+                ('result', models.JSONField(default=dict)),
+                ('params', models.IntegerField()),
+                ('flops', models.IntegerField()),
+                ('latency', models.FloatField()),
+                ('valid_acc', models.FloatField()),
+                ('test_acc', models.FloatField()),
+            ],
+            options={
+                'abstract': False,
+            },
+        ),
+    ]
```

### Comparing `evoxbench-1.0.2/evoxbench/database/nasbench101/migrations/0001_initial.py` & `evoxbench-1.0.3/evoxbench/database/resnet50/migrations/0001_initial.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-# Generated by Django 3.2.12 on 2022-03-19 09:13
-
-from django.db import migrations, models
-
-
-class Migration(migrations.Migration):
-    initial = True
-
-    dependencies = [
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='NASBench101Result',
-            fields=[
-                ('id', models.BigAutoField(primary_key=True, serialize=False)),
-                ('index', models.TextField(db_index=True, max_length=256, null=True)),
-                ('phenotype', models.JSONField(default=dict)),
-                ('genotype', models.JSONField(default=dict)),
-                ('result', models.JSONField(default=dict)),
-                ('epoch4', models.JSONField(default=dict)),
-                ('epoch12', models.JSONField(default=dict)),
-                ('epoch36', models.JSONField(default=dict)),
-                ('epoch108', models.JSONField(default=dict)),
-            ],
-            options={
-                'abstract': False,
-            },
-        ),
-    ]
+# Generated by Django 3.2.12 on 2022-05-07 14:56
+
+from django.db import migrations, models
+
+
+class Migration(migrations.Migration):
+    initial = True
+
+    dependencies = [
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='ResNet50Result',
+            fields=[
+                ('id', models.BigAutoField(primary_key=True, serialize=False)),
+                ('index', models.TextField(db_index=True, max_length=256, null=True)),
+                ('phenotype', models.JSONField(default=dict)),
+                ('genotype', models.JSONField(default=dict)),
+                ('result', models.JSONField(default=dict)),
+                ('params', models.IntegerField()),
+                ('flops', models.IntegerField()),
+                ('latency', models.FloatField()),
+                ('valid_acc', models.FloatField()),
+                ('test_acc', models.FloatField()),
+            ],
+            options={
+                'abstract': False,
+            },
+        ),
+    ]
```

### Comparing `evoxbench-1.0.2/evoxbench/database/nasbench101/models.py` & `evoxbench-1.0.3/evoxbench/database/nasbench101/models.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from operator import mod
-from nasbenchbase.models import NASBenchResult
-from django.db import models
-
-
-class NASBench101Result(NASBenchResult):
-    # epoch4 = models.JSONField(default=dict)
-    # epoch12 = models.JSONField(default=dict)
-    # epoch36 = models.JSONField(default=dict)
-    # epoch108 = models.JSONField(default=dict)
-    # image = models.ImageField(upload_to='', null=True)
-    flops = models.FloatField(default=-1)
-    params = models.FloatField(default=-1)
-    final_test_accuracy = models.JSONField(default=dict)
-    final_validation_accuracy = models.JSONField(default=dict)
+from operator import mod
+from nasbenchbase.models import NASBenchResult
+from django.db import models
+
+
+class NASBench101Result(NASBenchResult):
+    # epoch4 = models.JSONField(default=dict)
+    # epoch12 = models.JSONField(default=dict)
+    # epoch36 = models.JSONField(default=dict)
+    # epoch108 = models.JSONField(default=dict)
+    # image = models.ImageField(upload_to='', null=True)
+    flops = models.FloatField(default=-1)
+    params = models.FloatField(default=-1)
+    final_test_accuracy = models.JSONField(default=dict)
+    final_validation_accuracy = models.JSONField(default=dict)
```

### Comparing `evoxbench-1.0.2/evoxbench/database/nasbench201/migrations/0001_initial.py` & `evoxbench-1.0.3/evoxbench/database/nasbench201/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# Generated by Django 3.2.12 on 2022-03-20 14:40
-
-from django.db import migrations, models
-
-
-class Migration(migrations.Migration):
-    initial = True
-
-    dependencies = [
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='NASBench201Result',
-            fields=[
-                ('id', models.BigAutoField(primary_key=True, serialize=False)),
-                ('genotype', models.JSONField(default=dict)),
-                ('result', models.JSONField(default=dict)),
-                ('index', models.IntegerField(db_index=True)),
-                ('phenotype', models.CharField(db_index=True, max_length=256)),
-                ('cost12', models.JSONField(default=dict)),
-                ('cost200', models.JSONField(default=dict)),
-            ],
-            options={
-                'abstract': False,
-            },
-        ),
-    ]
+# Generated by Django 3.2.12 on 2022-03-20 14:40
+
+from django.db import migrations, models
+
+
+class Migration(migrations.Migration):
+    initial = True
+
+    dependencies = [
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='NASBench201Result',
+            fields=[
+                ('id', models.BigAutoField(primary_key=True, serialize=False)),
+                ('genotype', models.JSONField(default=dict)),
+                ('result', models.JSONField(default=dict)),
+                ('index', models.IntegerField(db_index=True)),
+                ('phenotype', models.CharField(db_index=True, max_length=256)),
+                ('cost12', models.JSONField(default=dict)),
+                ('cost200', models.JSONField(default=dict)),
+            ],
+            options={
+                'abstract': False,
+            },
+        ),
+    ]
```

### Comparing `evoxbench-1.0.2/evoxbench/database/nasbench201/models.py` & `evoxbench-1.0.3/evoxbench/database/nasbench201/models.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from email.policy import default
-from nasbenchbase.models import NASBenchResult
-from django.db import models
-
-
-class NASBench201Result(NASBenchResult):
-    index = models.IntegerField(db_index=True)
-    phenotype = models.CharField(max_length=256, db_index=True)
-    cost12 = models.JSONField(default=dict)
-    cost200 = models.JSONField(default=dict)
-    # res12 = models.JSONField(default=dict)
-    # res200 = models.JSONField(default=dict)
-    hw_info = models.JSONField(default=dict)
-    more_info = models.JSONField(default=dict)
+from email.policy import default
+from nasbenchbase.models import NASBenchResult
+from django.db import models
+
+
+class NASBench201Result(NASBenchResult):
+    index = models.IntegerField(db_index=True)
+    phenotype = models.CharField(max_length=256, db_index=True)
+    cost12 = models.JSONField(default=dict)
+    cost200 = models.JSONField(default=dict)
+    # res12 = models.JSONField(default=dict)
+    # res200 = models.JSONField(default=dict)
+    hw_info = models.JSONField(default=dict)
+    more_info = models.JSONField(default=dict)
```

### Comparing `evoxbench-1.0.2/evoxbench/database/natsbenchsss/migrations/0001_initial.py` & `evoxbench-1.0.3/evoxbench/database/natsbenchsss/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Generated by Django 3.2.12 on 2022-04-04 13:09
-
-from django.db import migrations, models
-
-
-class Migration(migrations.Migration):
-    initial = True
-
-    dependencies = [
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='NATSBenchResult',
-            fields=[
-                ('id', models.BigAutoField(primary_key=True, serialize=False)),
-                ('phenotype', models.JSONField(default=dict)),
-                ('genotype', models.JSONField(default=dict)),
-                ('result', models.JSONField(default=dict)),
-                ('cifar10_valid', models.JSONField()),
-                ('cifar10', models.JSONField()),
-                ('cifar100', models.JSONField()),
-                ('ImageNet16_120', models.JSONField()),
-                ('index', models.IntegerField()),
-            ],
-            options={
-                'abstract': False,
-            },
-        ),
-    ]
+# Generated by Django 3.2.12 on 2022-04-04 13:09
+
+from django.db import migrations, models
+
+
+class Migration(migrations.Migration):
+    initial = True
+
+    dependencies = [
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='NATSBenchResult',
+            fields=[
+                ('id', models.BigAutoField(primary_key=True, serialize=False)),
+                ('phenotype', models.JSONField(default=dict)),
+                ('genotype', models.JSONField(default=dict)),
+                ('result', models.JSONField(default=dict)),
+                ('cifar10_valid', models.JSONField()),
+                ('cifar10', models.JSONField()),
+                ('cifar100', models.JSONField()),
+                ('ImageNet16_120', models.JSONField()),
+                ('index', models.IntegerField()),
+            ],
+            options={
+                'abstract': False,
+            },
+        ),
+    ]
```

### Comparing `evoxbench-1.0.2/evoxbench/modules/benchmark.py` & `evoxbench-1.0.3/evoxbench/modules/benchmark.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-import numpy as np
-from numpy import ndarray
-from abc import ABC, abstractmethod
-
-from .evaluator import Evaluator
-from .search_space import SearchSpace
-
-__all__ = ['Benchmark']
-
-
-class Benchmark(ABC):
-    def __init__(self,
-                 search_space: SearchSpace,
-                 evaluator: Evaluator,
-                 normalized_objectives=False,
-                 **kwargs):
-        self.search_space = search_space
-        self.evaluator = evaluator
-        self.normalized_objectives = normalized_objectives
-
-    @property
-    @abstractmethod
-    def name(self):
-        raise NotImplementedError
-
-    @property
-    def pareto_front(self):
-        return None
-
-    @property
-    def pareto_set(self):
-        return None
-
-    @property
-    def _utopian_point(self):
-        return None
-
-    @property
-    def _nadir_point(self):
-        return None
-
-    @property
-    def utopian_point(self):
-        if self._utopian_point is not None:
-            return np.array(self._utopian_point)
-        elif self.pareto_front is not None:
-            return np.min(self.pareto_front, axis=0)
-        else:
-            return None
-
-    @property
-    def nadir_point(self):
-        if self._nadir_point is not None:
-            return np.array(self._nadir_point)
-        elif self.pareto_front is not None:
-            return np.max(self.pareto_front, axis=0)
-        else:
-            return None
-
-    @property
-    def _hv_ref_point(self):
-        return None
-
-    @property
-    def hv_ref_point(self):
-        # reference point for calculating hypervolume
-        if self._hv_ref_point is not None:
-            return self._hv_ref_point
-        elif self.nadir_point is not None:
-            return self.nadir_point
-        else:
-            return None
-
-    def normalize(self, F: np.array):
-        """ method to normalize the objectives  """
-        assert self.utopian_point is not None, "Missing Pareto front or utopian point for normalization"
-        assert self.nadir_point is not None, "Missing Pareto front or nadir point for normalization"
-        return (F - self.utopian_point) / (self.nadir_point - self.utopian_point)
-
-    def to_matrix(self, batch_stats: dict) -> ndarray:
-        # convert performance dict to objective matrix
-        return np.array([list(v.values()) for v in batch_stats])
-
-    def evaluate(self, X, **kwargs):
-        # convert genotype X to architecture phenotype
-        archs = self.search_space.decode(X)
-
-        # query for performance
-        batch_stats = self.evaluator.evaluate(archs, **kwargs)
-
-        # convert performance dict to objective matrix
-        F = self.to_matrix(batch_stats)
-
-        # normalize objective matrix
-        if self.normalized_objectives:
-            F = self.normalize(F)
-
-        return F
-
-    def calc_perf_indicator(self, inputs, indicator='igd'):
-
-        # The performance indicator that calculates IGD and HV are from [pymoo](https://pymoo.org/).
-        try:
-            from pymoo.indicators.igd import IGD
-            from pymoo.indicators.hv import HV
-            from pymoo.util.nds.non_dominated_sorting import NonDominatedSorting
-        except ImportError:
-            raise ImportError('please first install pymoo from https://pymoo.org/')
-
-        assert indicator in ['igd', 'hv', 'normalized_hv'], "The requested performance indicator is not supported"
-
-        if indicator == 'igd':
-            assert self.pareto_front is not None, "Pareto front needs to be defined before IGD calculation"
-
-        if indicator == 'hv':
-            assert self.hv_ref_point is not None, "A reference point need to be defined before HV calculation"
-
-        if indicator == 'igd':
-            # normalize Pareto front
-            pf = self.normalize(self.pareto_front)
-            metric = IGD(pf=pf)
-        elif 'hv' in indicator:
-            hv_ref_point = self.normalize(self.hv_ref_point)
-            metric = HV(ref_point=hv_ref_point)
-        else:
-            raise KeyError("the requested performance indicator is not define")
-
-        if isinstance(inputs[0], ndarray):
-            # re-evaluate the true performance
-            F = self.evaluate(inputs, true_eval=True)  # use true/mean accuracy
-
-        else:
-            batch_stats = self.evaluator.evaluate(inputs, true_eval=True)
-            F = self.to_matrix(batch_stats)
-
-        if not self.normalized_objectives:
-            F = self.normalize(F)  # in case the benchmark evaluator does not normalize objs by default
-
-        # filter out the non-dominated solutions
-        nd_front = NonDominatedSorting().do(F, only_non_dominated_front=True)
-        performance = metric(F[nd_front])
-
-        if indicator == 'normalized_hv' and self.pareto_front is not None:
-            hv_norm = metric(self.normalize(self.pareto_front))
-            performance = performance / hv_norm
-
-        return performance
+import numpy as np
+from numpy import ndarray
+from abc import ABC, abstractmethod
+
+from .evaluator import Evaluator
+from .search_space import SearchSpace
+
+__all__ = ['Benchmark']
+
+
+class Benchmark(ABC):
+    def __init__(self,
+                 search_space: SearchSpace,
+                 evaluator: Evaluator,
+                 normalized_objectives=False,
+                 **kwargs):
+        self.search_space = search_space
+        self.evaluator = evaluator
+        self.normalized_objectives = normalized_objectives
+
+    @property
+    @abstractmethod
+    def name(self):
+        raise NotImplementedError
+
+    @property
+    def pareto_front(self):
+        return None
+
+    @property
+    def pareto_set(self):
+        return None
+
+    @property
+    def _utopian_point(self):
+        return None
+
+    @property
+    def _nadir_point(self):
+        return None
+
+    @property
+    def utopian_point(self):
+        if self._utopian_point is not None:
+            return np.array(self._utopian_point)
+        elif self.pareto_front is not None:
+            return np.min(self.pareto_front, axis=0)
+        else:
+            return None
+
+    @property
+    def nadir_point(self):
+        if self._nadir_point is not None:
+            return np.array(self._nadir_point)
+        elif self.pareto_front is not None:
+            return np.max(self.pareto_front, axis=0)
+        else:
+            return None
+
+    @property
+    def _hv_ref_point(self):
+        return None
+
+    @property
+    def hv_ref_point(self):
+        # reference point for calculating hypervolume
+        if self._hv_ref_point is not None:
+            return self._hv_ref_point
+        elif self.nadir_point is not None:
+            return self.nadir_point
+        else:
+            return None
+
+    def normalize(self, F: np.array):
+        """ method to normalize the objectives  """
+        assert self.utopian_point is not None, "Missing Pareto front or utopian point for normalization"
+        assert self.nadir_point is not None, "Missing Pareto front or nadir point for normalization"
+        return (F - self.utopian_point) / (self.nadir_point - self.utopian_point)
+
+    def to_matrix(self, batch_stats: dict) -> ndarray:
+        # convert performance dict to objective matrix
+        return np.array([list(v.values()) for v in batch_stats])
+
+    def evaluate(self, X, **kwargs):
+        # convert genotype X to architecture phenotype
+        archs = self.search_space.decode(X)
+
+        # query for performance
+        batch_stats = self.evaluator.evaluate(archs, **kwargs)
+
+        # convert performance dict to objective matrix
+        F = self.to_matrix(batch_stats)
+
+        # normalize objective matrix
+        if self.normalized_objectives:
+            F = self.normalize(F)
+
+        return F
+
+    def calc_perf_indicator(self, inputs, indicator='igd'):
+
+        # The performance indicator that calculates IGD and HV are from [pymoo](https://pymoo.org/).
+        try:
+            from pymoo.indicators.igd import IGD
+            from pymoo.indicators.hv import HV
+            from pymoo.util.nds.non_dominated_sorting import NonDominatedSorting
+        except ImportError:
+            raise ImportError('please first install pymoo from https://pymoo.org/')
+
+        assert indicator in ['igd', 'hv', 'normalized_hv'], "The requested performance indicator is not supported"
+
+        if indicator == 'igd':
+            assert self.pareto_front is not None, "Pareto front needs to be defined before IGD calculation"
+
+        if indicator == 'hv':
+            assert self.hv_ref_point is not None, "A reference point need to be defined before HV calculation"
+
+        if indicator == 'igd':
+            # normalize Pareto front
+            pf = self.normalize(self.pareto_front)
+            metric = IGD(pf=pf)
+        elif 'hv' in indicator:
+            hv_ref_point = self.normalize(self.hv_ref_point)
+            metric = HV(ref_point=hv_ref_point)
+        else:
+            raise KeyError("the requested performance indicator is not define")
+
+        if isinstance(inputs[0], ndarray):
+            # re-evaluate the true performance
+            F = self.evaluate(inputs, true_eval=True)  # use true/mean accuracy
+
+        else:
+            batch_stats = self.evaluator.evaluate(inputs, true_eval=True)
+            F = self.to_matrix(batch_stats)
+
+        if not self.normalized_objectives:
+            F = self.normalize(F)  # in case the benchmark evaluator does not normalize objs by default
+
+        # filter out the non-dominated solutions
+        nd_front = NonDominatedSorting().do(F, only_non_dominated_front=True)
+        performance = metric(F[nd_front])
+
+        if indicator == 'normalized_hv' and self.pareto_front is not None:
+            hv_norm = metric(self.normalize(self.pareto_front))
+            performance = performance / hv_norm
+
+        return performance
```

### Comparing `evoxbench-1.0.2/evoxbench/modules/evaluator.py` & `evoxbench-1.0.3/evoxbench/modules/evaluator.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from abc import ABC, abstractmethod
-
-__all__ = ['Evaluator']
-
-
-class Evaluator(ABC):
-    def __init__(self,
-                 objs='err&params',  # objectives to be minimized
-                 **kwargs):
-        self.objs = objs
-
-    @property
-    @abstractmethod
-    def name(self):
-        raise NotImplementedError
-
-    @property
-    def n_objs(self):
-        return len(self.objs.split('&'))
-
-    @abstractmethod
-    def evaluate(self, archs, **kwargs):
-        """ method to evaluate the population """
-        raise NotImplementedError
+from abc import ABC, abstractmethod
+
+__all__ = ['Evaluator']
+
+
+class Evaluator(ABC):
+    def __init__(self,
+                 objs='err&params',  # objectives to be minimized
+                 **kwargs):
+        self.objs = objs
+
+    @property
+    @abstractmethod
+    def name(self):
+        raise NotImplementedError
+
+    @property
+    def n_objs(self):
+        return len(self.objs.split('&'))
+
+    @abstractmethod
+    def evaluate(self, archs, **kwargs):
+        """ method to evaluate the population """
+        raise NotImplementedError
```

### Comparing `evoxbench-1.0.2/evoxbench/modules/search_space.py` & `evoxbench-1.0.3/evoxbench/modules/search_space.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import numpy as np
-from abc import ABC, abstractmethod
-
-__all__ = ['SearchSpace']
-
-
-class SearchSpace(ABC):
-    def __init__(self, **kwargs):
-        # attributes below have to be filled by child class
-        self.n_var = None
-        self.lb = None
-        self.ub = None
-        self.categories = None
-
-    @property
-    @abstractmethod
-    def name(self):
-        raise NotImplementedError
-
-    @abstractmethod
-    def _sample(self):
-        """ method to randomly create an architecture phenotype """
-        raise NotImplementedError
-
-    def sample(self, n_samples):
-        subnets = []
-        for _ in range(n_samples):
-            subnets.append(self._sample())
-        return subnets
-
-    @abstractmethod
-    def _encode(self, arch):
-        """ method to convert architectural string to search decision variable vector """
-        raise NotImplementedError
-
-    def encode(self, archs):
-        X = []
-        for arch in archs:
-            X.append(self._encode(arch))
-        return np.array(X)
-
-    @abstractmethod
-    def _decode(self, x):
-        """ method to convert decision variable vector to architectural string """
-        raise NotImplementedError
-
-    def decode(self, X):
-        archs = []
-        for x in X:
-            archs.append(self._decode(x))
-        return archs
-
-    @abstractmethod
-    def visualize(self, arch):
-        """ method to visualize an architecture """
-        raise NotImplementedError
+import numpy as np
+from abc import ABC, abstractmethod
+
+__all__ = ['SearchSpace']
+
+
+class SearchSpace(ABC):
+    def __init__(self, **kwargs):
+        # attributes below have to be filled by child class
+        self.n_var = None
+        self.lb = None
+        self.ub = None
+        self.categories = None
+
+    @property
+    @abstractmethod
+    def name(self):
+        raise NotImplementedError
+
+    @abstractmethod
+    def _sample(self):
+        """ method to randomly create an architecture phenotype """
+        raise NotImplementedError
+
+    def sample(self, n_samples):
+        subnets = []
+        for _ in range(n_samples):
+            subnets.append(self._sample())
+        return subnets
+
+    @abstractmethod
+    def _encode(self, arch):
+        """ method to convert architectural string to search decision variable vector """
+        raise NotImplementedError
+
+    def encode(self, archs):
+        X = []
+        for arch in archs:
+            X.append(self._encode(arch))
+        return np.array(X)
+
+    @abstractmethod
+    def _decode(self, x):
+        """ method to convert decision variable vector to architectural string """
+        raise NotImplementedError
+
+    def decode(self, X):
+        archs = []
+        for x in X:
+            archs.append(self._decode(x))
+        return archs
+
+    @abstractmethod
+    def visualize(self, arch):
+        """ method to visualize an architecture """
+        raise NotImplementedError
```

### Comparing `evoxbench-1.0.2/evoxbench/modules/surrogate_model.py` & `evoxbench-1.0.3/evoxbench/modules/surrogate_model.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-import json
-import numpy as np
-from abc import ABC, abstractmethod
-
-__all__ = ['SurrogateModel', 'MLPPredictor']
-
-
-class SurrogateModel(ABC):
-    def __init__(self, **kwargs):
-        pass
-
-    @property
-    @abstractmethod
-    def name(self):
-        """ name of the surrogate model """
-        raise NotImplementedError
-
-    @abstractmethod
-    def fit(self, X, **kwargs):
-        """ method to fit/learn/train a surrogate model from data """
-        raise NotImplementedError
-
-    @abstractmethod
-    def predict(self, features, **kwargs):
-        """ method to predict performance from architecture features """
-        raise NotImplementedError
-
-
-class MLPPredictor(SurrogateModel):
-    def __init__(self,
-                 pretrained,  # pretrained weights and bias dict
-                 ):
-
-        super().__init__()
-
-        # weights = json.load(open(pretrained, 'r'))
-        checkpoints = json.load(open(pretrained, 'r'))
-
-        weights = checkpoints['state_dicts']
-        self.remap_factor = checkpoints['remap_factor']
-        self.base_acc = checkpoints['base_acc']
-
-        if not isinstance(weights, list):
-            weights = [weights]
-
-        models = []
-        for weight in weights:
-            model = {}
-            for key, values in weight.items():
-                model[key] = np.array(values)
-
-            model['normalization_factor'] = weight['normalization_factor']
-            models.append(model)
-
-        self.models = models
-
-        # self.model = {}
-        # for key, values in json.load(open(pretrained, 'r')).items():
-        #     self.model[key] = np.array(values)
-
-    @property
-    def name(self):
-        return 'MLP Predictor'
-
-    def fit(self, X, **kwargs):
-        raise NotImplementedError
-
-    def forward(self, X, model):
-        for i in range(1, 4):
-            X = np.matmul(X, model['W{}'.format(i)].transpose()) + model['b{}'.format(i)][None, :]
-            X = np.maximum(X, 0)
-
-        X = np.matmul(X, model['W4'].transpose())
-        X += model['b4'][None, :]
-        # if 'b4' in model:
-        #
-
-        # if 'base_acc' in model:
-        #     X += model['base_acc']
-
-        # if 'normalization_factor' in model:
-        #     X = (X - model['normalization_factor'][0]) / model['normalization_factor'][1]
-
-        # if 'remap_factor' in model:
-        #     X = X * model['remap_factor'][1] + model['remap_factor'][0]
-
-        # return X
-        X += self.base_acc
-        # normalization
-        X = (X - model['normalization_factor'][0]) / model['normalization_factor'][1]
-
-        return X * self.remap_factor[1] + self.remap_factor[0]  # remap to range
-
-    def predict(self, features, is_noisy=False, **kwargs):
-
-        if is_noisy:
-            pred = self.forward(features, np.random.choice(self.models))
-        else:
-            pred = 0
-            for model in self.models:
-                pred += self.forward(features, model)
-
-            pred = pred / len(self.models)
-        return pred
-
-
-if __name__ == '__main__':
-    import copy
-    import torch
-
-    state_dict = torch.load("/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/data/mnv3/acc_predictor.pth",
-                            map_location=torch.device("cpu"))
-
-    for key, values in state_dict.items():
-        print(key)
-        print(values.size())
-    exit()
-    new_state_dict = {}
-    w_i, b_i = 1, 1
-    for key, values in state_dict.items():
-        if 'weight' in key:
-            new_state_dict['W{}'.format(w_i)] = copy.deepcopy(values.cpu().detach().numpy().tolist())
-            w_i += 1
-        if 'bias' in key:
-            new_state_dict['b{}'.format(b_i)] = copy.deepcopy(values.cpu().detach().numpy().tolist())
-            b_i += 1
-
-    for key, values in new_state_dict.items():
-        print(key)
-        print(values)
-
-    with open('/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/data/mnv3/acc_predictor.json', 'w') as fp:
-        json.dump(new_state_dict, fp)
+import json
+import numpy as np
+from abc import ABC, abstractmethod
+
+__all__ = ['SurrogateModel', 'MLPPredictor']
+
+
+class SurrogateModel(ABC):
+    def __init__(self, **kwargs):
+        pass
+
+    @property
+    @abstractmethod
+    def name(self):
+        """ name of the surrogate model """
+        raise NotImplementedError
+
+    @abstractmethod
+    def fit(self, X, **kwargs):
+        """ method to fit/learn/train a surrogate model from data """
+        raise NotImplementedError
+
+    @abstractmethod
+    def predict(self, features, **kwargs):
+        """ method to predict performance from architecture features """
+        raise NotImplementedError
+
+
+class MLPPredictor(SurrogateModel):
+    def __init__(self,
+                 pretrained,  # pretrained weights and bias dict
+                 ):
+
+        super().__init__()
+
+        # weights = json.load(open(pretrained, 'r'))
+        checkpoints = json.load(open(pretrained, 'r'))
+
+        weights = checkpoints['state_dicts']
+        self.remap_factor = checkpoints['remap_factor']
+        self.base_acc = checkpoints['base_acc']
+
+        if not isinstance(weights, list):
+            weights = [weights]
+
+        models = []
+        for weight in weights:
+            model = {}
+            for key, values in weight.items():
+                model[key] = np.array(values)
+
+            model['normalization_factor'] = weight['normalization_factor']
+            models.append(model)
+
+        self.models = models
+
+        # self.model = {}
+        # for key, values in json.load(open(pretrained, 'r')).items():
+        #     self.model[key] = np.array(values)
+
+    @property
+    def name(self):
+        return 'MLP Predictor'
+
+    def fit(self, X, **kwargs):
+        raise NotImplementedError
+
+    def forward(self, X, model):
+        for i in range(1, 4):
+            X = np.matmul(X, model['W{}'.format(i)].transpose()) + model['b{}'.format(i)][None, :]
+            X = np.maximum(X, 0)
+
+        X = np.matmul(X, model['W4'].transpose())
+        X += model['b4'][None, :]
+        # if 'b4' in model:
+        #
+
+        # if 'base_acc' in model:
+        #     X += model['base_acc']
+
+        # if 'normalization_factor' in model:
+        #     X = (X - model['normalization_factor'][0]) / model['normalization_factor'][1]
+
+        # if 'remap_factor' in model:
+        #     X = X * model['remap_factor'][1] + model['remap_factor'][0]
+
+        # return X
+        X += self.base_acc
+        # normalization
+        X = (X - model['normalization_factor'][0]) / model['normalization_factor'][1]
+
+        return X * self.remap_factor[1] + self.remap_factor[0]  # remap to range
+
+    def predict(self, features, is_noisy=False, **kwargs):
+
+        if is_noisy:
+            pred = self.forward(features, np.random.choice(self.models))
+        else:
+            pred = 0
+            for model in self.models:
+                pred += self.forward(features, model)
+
+            pred = pred / len(self.models)
+        return pred
+
+
+if __name__ == '__main__':
+    import copy
+    import torch
+
+    state_dict = torch.load("/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/data/mnv3/acc_predictor.pth",
+                            map_location=torch.device("cpu"))
+
+    for key, values in state_dict.items():
+        print(key)
+        print(values.size())
+    exit()
+    new_state_dict = {}
+    w_i, b_i = 1, 1
+    for key, values in state_dict.items():
+        if 'weight' in key:
+            new_state_dict['W{}'.format(w_i)] = copy.deepcopy(values.cpu().detach().numpy().tolist())
+            w_i += 1
+        if 'bias' in key:
+            new_state_dict['b{}'.format(b_i)] = copy.deepcopy(values.cpu().detach().numpy().tolist())
+            b_i += 1
+
+    for key, values in new_state_dict.items():
+        print(key)
+        print(values)
+
+    with open('/Users/luzhicha/Dropbox/2022/EvoXBench/python_codes/data/mnv3/acc_predictor.json', 'w') as fp:
+        json.dump(new_state_dict, fp)
```

### Comparing `evoxbench-1.0.2/evoxbench/test_suites/c10mop.py` & `evoxbench-1.0.3/evoxbench/test_suites/c10mop.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from evoxbench.benchmarks import NASBench101Benchmark, NASBench201Benchmark, NATSBenchmark, DARTSBenchmark
-
-__all__ = ['c10mop']
-
-
-def c10mop(problem_id):
-    if problem_id == 1:
-        return NASBench101Benchmark(
-            objs='err&params', normalized_objectives=True)
-    elif problem_id == 2:
-        return NASBench101Benchmark(
-            objs='err&params&flops', normalized_objectives=True)
-    elif problem_id == 3:
-        return NATSBenchmark(
-            90, objs='err&params&flops', dataset='cifar10', normalized_objectives=True)
-    elif problem_id == 4:
-        return NATSBenchmark(
-            90, objs='err&params&flops&latency', dataset='cifar10', normalized_objectives=True)
-    elif problem_id == 5:
-        return NASBench201Benchmark(
-            200, objs='err&params&flops&edgegpu_latency&edgegpu_energy', dataset='cifar10',
-            normalized_objectives=True)
-    elif problem_id == 6:
-        return NASBench201Benchmark(
-            200, objs='err&params&flops&eyeriss_latency&eyeriss_energy&eyeriss_arithmetic_intensity', dataset='cifar10',
-            normalized_objectives=True)
-    elif problem_id == 7:
-        return NASBench201Benchmark(
-            200, objs='err&params&flops&edgegpu_latency&edgegpu_energy'
-                      '&eyeriss_latency&eyeriss_energy&eyeriss_arithmetic_intensity', dataset='cifar10',
-            normalized_objectives=True)
-    elif problem_id == 8:
-        return DARTSBenchmark(
-            objs='err&params', normalized_objectives=False)
-    elif problem_id == 9:
-        return DARTSBenchmark(
-            objs='err&params&flops', normalized_objectives=False)
-    else:
-        raise ValueError("the requested problem id does not exist")
+from evoxbench.benchmarks import NASBench101Benchmark, NASBench201Benchmark, NATSBenchmark, DARTSBenchmark
+
+__all__ = ['c10mop']
+
+
+def c10mop(problem_id):
+    if problem_id == 1:
+        return NASBench101Benchmark(
+            objs='err&params', normalized_objectives=True)
+    elif problem_id == 2:
+        return NASBench101Benchmark(
+            objs='err&params&flops', normalized_objectives=True)
+    elif problem_id == 3:
+        return NATSBenchmark(
+            90, objs='err&params&flops', dataset='cifar10', normalized_objectives=True)
+    elif problem_id == 4:
+        return NATSBenchmark(
+            90, objs='err&params&flops&latency', dataset='cifar10', normalized_objectives=True)
+    elif problem_id == 5:
+        return NASBench201Benchmark(
+            200, objs='err&params&flops&edgegpu_latency&edgegpu_energy', dataset='cifar10',
+            normalized_objectives=True)
+    elif problem_id == 6:
+        return NASBench201Benchmark(
+            200, objs='err&params&flops&eyeriss_latency&eyeriss_energy&eyeriss_arithmetic_intensity', dataset='cifar10',
+            normalized_objectives=True)
+    elif problem_id == 7:
+        return NASBench201Benchmark(
+            200, objs='err&params&flops&edgegpu_latency&edgegpu_energy'
+                      '&eyeriss_latency&eyeriss_energy&eyeriss_arithmetic_intensity', dataset='cifar10',
+            normalized_objectives=True)
+    elif problem_id == 8:
+        return DARTSBenchmark(
+            objs='err&params', normalized_objectives=False)
+    elif problem_id == 9:
+        return DARTSBenchmark(
+            objs='err&params&flops', normalized_objectives=False)
+    else:
+        raise ValueError("the requested problem id does not exist")
```

### Comparing `evoxbench-1.0.2/evoxbench.egg-info/SOURCES.txt` & `evoxbench-1.0.3/evoxbench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evoxbench-1.0.2/setup.py` & `evoxbench-1.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-from setuptools import setup, find_packages
-import pathlib
-
-here = pathlib.Path(__file__).parent.resolve()
-
-# Get the long description from the README file
-long_description = (here / "README.md").read_text(encoding="utf-8")
-
-setup(
-    # lowercase name so that:
-    # $ pip install evoxbench
-    # instead of
-    # $ pip install EvoXBench
-    name="evoxbench",
-    version="1.0.2",
-    description="A benchmark for NAS algorithms",  # Optional
-    long_description=long_description,  # Optional
-    long_description_content_type="text/markdown",
-    url="https://github.com/EMI-Group/evoxbench",  # Optional
-    author="EMI-Group",  # Optional
-    author_email="emi-group@outlook.com",  # Optional
-    # Classifiers help users find your project by categorizing it.
-    #
-    # For a list of valid classifiers, see https://pypi.org/classifiers/
-    classifiers=[  # Optional
-        # How mature is this project? Common values are
-        #   3 - Alpha
-        #   4 - Beta
-        #   5 - Production/Stable
-        "Development Status :: 3 - Alpha",
-        # Indicate who your project is intended for
-        "Intended Audience :: Science/Research",
-        "Topic :: Software Development :: Build Tools",
-        # Pick your license as you wish
-        "License :: OSI Approved :: MIT License",
-        # Specify the Python versions you support here. In particular, ensure
-        # that you indicate you support Python 3. These classifiers are *not*
-        # checked by 'pip install'. See instead 'python_requires' below.
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3 :: Only",
-    ],
-    # This field adds keywords for your project which will appear on the
-    # project page. What does your project relate to?
-    #
-    # Note that this is a list of additional keywords, separated
-    # by commas, to be used to assist searching for the distribution in a
-    # larger catalog.
-    keywords="benchmark, evolution algorithm, neural architecture search",  # Optional
-    # When your source code is in a subdirectory under the project root, e.g.
-    # `src/`, it is necessary to specify the `package_dir` argument.
-    # package_dir={"": ""},
-    # find_packages failed to work, so manually list packages.
-    # data_files=[('', ['evoxbench/__main__.py'])],
-    packages=find_packages(),
-    # packages=[
-    #     "evoxbench",
-    #     "evoxbench.benchmarks", "evoxbench.api", "evoxbench.modules",
-    #     "evoxbench.api.pymoo"
-    #     ],  # Required
-    # Specify which Python versions you support. In contrast to the
-    # 'Programming Language' classifiers above, 'pip install' will check this
-    # and refuse to install the project if the version does not match. See
-    # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
-    python_requires=">=3.7, <4",
-    # Only top-level dependencies
-    install_requires=[
-        "pyyaml",
-        "django",
-        "numpy",
-        # "pymoo",
-        "scikit-learn",
-        "scipy",
-    ],  # Optional
-    # List additional groups of dependencies here (e.g. development
-    # dependencies). Users will be able to install these using the "extras"
-    # syntax, for example:
-    #
-    #   $ pip install sampleproject[dev]
-    #
-    # Similar to `install_requires` above, these must be valid existing
-    # projects.
-    # extras_require={  # Optional
-    #     "dev": ["check-manifest"],
-    # },
-
-    # To provide executable scripts, use entry points in preference to the
-    # "scripts" keyword. Entry points provide cross-platform support and allow
-    # `pip` to create the appropriate form of executable for the target
-    # platform.
-    #
-    # For example, the following would provide a command called `evoxbenchrpc` which
-    # executes the function `main` from this package when invoked:
-    entry_points={
-        "console_scripts": [
-            # "evoxbench=evoxbench.__main__:main",
-            "evoxbenchrpc=evoxbench.api.rpc:main",
-        ],
-    },
-    # List additional URLs that are relevant to your project as a dict.
-    #
-    # This field corresponds to the "Project-URL" metadata fields:
-    # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
-    #
-    # Examples listed include a pattern for specifying where the package tracks
-    # issues, where the source is hosted, where to say thanks to the package
-    # maintainers, and where to support the project financially. The key is
-    # what's used to render the link text on PyPI.
-    project_urls={  # Optional
-        "Bug Reports": "https://github.com/EMI-Group/evoxbench/issues",
-        "Source": "https://github.com/EMI-Group/evoxbench",
-    },
-
-    zip_safe=False,
-)
+from setuptools import setup, find_packages
+import pathlib
+
+here = pathlib.Path(__file__).parent.resolve()
+
+# Get the long description from the README file
+long_description = (here / "README.md").read_text(encoding="utf-8")
+
+setup(
+    # lowercase name so that:
+    # $ pip install evoxbench
+    # instead of
+    # $ pip install EvoXBench
+    name="evoxbench",
+    version="1.0.3",
+    description="A benchmark for NAS algorithms",  # Optional
+    long_description=long_description,  # Optional
+    long_description_content_type="text/markdown",
+    url="https://github.com/EMI-Group/evoxbench",  # Optional
+    author="EMI-Group",  # Optional
+    author_email="emi-group@outlook.com",  # Optional
+    # Classifiers help users find your project by categorizing it.
+    #
+    # For a list of valid classifiers, see https://pypi.org/classifiers/
+    classifiers=[  # Optional
+        # How mature is this project? Common values are
+        #   3 - Alpha
+        #   4 - Beta
+        #   5 - Production/Stable
+        "Development Status :: 3 - Alpha",
+        # Indicate who your project is intended for
+        "Intended Audience :: Science/Research",
+        "Topic :: Software Development :: Build Tools",
+        # Pick your license as you wish
+        "License :: OSI Approved :: MIT License",
+        # Specify the Python versions you support here. In particular, ensure
+        # that you indicate you support Python 3. These classifiers are *not*
+        # checked by 'pip install'. See instead 'python_requires' below.
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3 :: Only",
+    ],
+    # This field adds keywords for your project which will appear on the
+    # project page. What does your project relate to?
+    #
+    # Note that this is a list of additional keywords, separated
+    # by commas, to be used to assist searching for the distribution in a
+    # larger catalog.
+    keywords="benchmark, evolution algorithm, neural architecture search",  # Optional
+    # When your source code is in a subdirectory under the project root, e.g.
+    # `src/`, it is necessary to specify the `package_dir` argument.
+    # package_dir={"": ""},
+    # find_packages failed to work, so manually list packages.
+    # data_files=[('', ['evoxbench/__main__.py'])],
+    packages=find_packages(),
+    # packages=[
+    #     "evoxbench",
+    #     "evoxbench.benchmarks", "evoxbench.api", "evoxbench.modules",
+    #     "evoxbench.api.pymoo"
+    #     ],  # Required
+    # Specify which Python versions you support. In contrast to the
+    # 'Programming Language' classifiers above, 'pip install' will check this
+    # and refuse to install the project if the version does not match. See
+    # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
+    python_requires=">=3.7, <4",
+    # Only top-level dependencies
+    install_requires=[
+        "pyyaml",
+        "django",
+        "numpy",
+        # "pymoo",
+        "scikit-learn",
+        "scipy",
+    ],  # Optional
+    # List additional groups of dependencies here (e.g. development
+    # dependencies). Users will be able to install these using the "extras"
+    # syntax, for example:
+    #
+    #   $ pip install sampleproject[dev]
+    #
+    # Similar to `install_requires` above, these must be valid existing
+    # projects.
+    # extras_require={  # Optional
+    #     "dev": ["check-manifest"],
+    # },
+
+    # To provide executable scripts, use entry points in preference to the
+    # "scripts" keyword. Entry points provide cross-platform support and allow
+    # `pip` to create the appropriate form of executable for the target
+    # platform.
+    #
+    # For example, the following would provide a command called `evoxbenchrpc` which
+    # executes the function `main` from this package when invoked:
+    entry_points={
+        "console_scripts": [
+            # "evoxbench=evoxbench.__main__:main",
+            "evoxbenchrpc=evoxbench.api.rpc:main",
+        ],
+    },
+    # List additional URLs that are relevant to your project as a dict.
+    #
+    # This field corresponds to the "Project-URL" metadata fields:
+    # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
+    #
+    # Examples listed include a pattern for specifying where the package tracks
+    # issues, where the source is hosted, where to say thanks to the package
+    # maintainers, and where to support the project financially. The key is
+    # what's used to render the link text on PyPI.
+    project_urls={  # Optional
+        "Bug Reports": "https://github.com/EMI-Group/evoxbench/issues",
+        "Source": "https://github.com/EMI-Group/evoxbench",
+    },
+
+    zip_safe=False,
+)
```

