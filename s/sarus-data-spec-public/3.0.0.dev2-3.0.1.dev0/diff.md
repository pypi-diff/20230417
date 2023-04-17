# Comparing `tmp/sarus_data_spec_public-3.0.0.dev2.tar.gz` & `tmp/sarus_data_spec_public-3.0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus_data_spec_public-3.0.0.dev2.tar", last modified: Fri Apr  7 10:10:41 2023, max compression
+gzip compressed data, was "sarus_data_spec_public-3.0.1.dev0.tar", last modified: Mon Apr 17 16:16:48 2023, max compression
```

## Comparing `sarus_data_spec_public-3.0.0.dev2.tar` & `sarus_data_spec_public-3.0.1.dev0.tar`

### file list

```diff
@@ -1,178 +1,183 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.635953 sarus_data_spec_public-3.0.0.dev2/
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      436 2023-04-07 10:10:41.635953 sarus_data_spec_public-3.0.0.dev2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.588950 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/
--rwxrwxrwx   0 root         (0) root         (0)      830 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.590950 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/arrow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/arrow/array.py
--rw-rw-rw-   0 root         (0) root         (0)     7487 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/arrow/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9355 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/arrow/type.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/attribute.py
--rw-rw-rw-   0 root         (0) root         (0)     4618 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.591950 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/config/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2744 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/config/privacy_properties.yaml
--rw-rw-rw-   0 root         (0) root         (0)     6116 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/config/routing.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3500 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.593950 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/context/
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/context/public.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/context/state.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/context/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    18070 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.594950 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_rewriter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_rewriter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2286 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_rewriter/base.py
--rw-rw-rw-   0 root         (0) root         (0)    12251 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_rewriter/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_rewriter/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.596950 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_validator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_validator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11081 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_validator/base.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_validator/privacy_limit.py
--rw-rw-rw-   0 root         (0) root         (0)     2710 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_validator/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     4470 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_validator/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     8849 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.597951 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6890 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/async_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    27491 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.598950 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/computations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/computations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8138 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/computations/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.599951 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/computations/local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/computations/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/computations/local/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2172 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/computations/local/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.599951 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/computations/remote/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/computations/remote/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3302 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/computations/remote/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.600951 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3552 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.601951 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.604951 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13974 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/external_op.py
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/imblearn.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.605951 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/pandas/
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    28993 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
--rw-rw-rw-   0 root         (0) root         (0)    27823 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     7976 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/protection_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4765 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/sklearn.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/skopt.py
--rw-rw-rw-   0 root         (0) root         (0)     3093 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/std.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/xgboost.py
--rw-rw-rw-   0 root         (0) root         (0)     9996 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.610952 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13739 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/extract.py
--rw-rw-rw-   0 root         (0) root         (0)    11529 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/filter.py
--rw-rw-rw-   0 root         (0) root         (0)    10703 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/get_item.py
--rw-rw-rw-   0 root         (0) root         (0)    10747 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/project.py
--rw-rw-rw-   0 root         (0) root         (0)     6519 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/sample.py
--rw-rw-rw-   0 root         (0) root         (0)     4290 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/select_sql.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/shuffle.py
--rw-rw-rw-   0 root         (0) root         (0)    10106 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/standard_op.py
--rw-rw-rw-   0 root         (0) root         (0)    10991 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/synthetic.py
--rw-rw-rw-   0 root         (0) root         (0)    27153 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.611951 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/source/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/source/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4015 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/source/model.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/source/privacy_params.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/source/random_seed.py
--rw-rw-rw-   0 root         (0) root         (0)     2670 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/source/routing.py
--rw-rw-rw-   0 root         (0) root         (0)    12255 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/marginals.py
--rw-rw-rw-   0 root         (0) root         (0)     3127 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3004 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/predicate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.631953 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/
--rw-rw-rw-   0 root         (0) root         (0)     1978 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/attribute.proto
--rw-r--r--   0 root         (0) root         (0)     5552 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/attribute_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/bounds.proto
--rw-r--r--   0 root         (0) root         (0)     6306 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/bounds_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/bounds_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/constraint.proto
--rw-r--r--   0 root         (0) root         (0)     8070 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/constraint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/constraint_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1233 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/dataset.proto
--rw-r--r--   0 root         (0) root         (0)    24833 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/dataset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8880 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/dataset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/links.proto
--rw-r--r--   0 root         (0) root         (0)    11282 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/links_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4193 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/links_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/manager.proto
--rw-r--r--   0 root         (0) root         (0)     4572 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/manager_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/marginals.proto
--rw-r--r--   0 root         (0) root         (0)     6408 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/marginals_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2177 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/marginals_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/path.proto
--rw-r--r--   0 root         (0) root         (0)     4998 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/path_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/path_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/predicate.proto
--rw-r--r--   0 root         (0) root         (0)    13369 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/predicate_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4859 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/predicate_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/proto_container.proto
--rw-r--r--   0 root         (0) root         (0)     5086 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/proto_container_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/proto_container_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/relation.proto
--rw-r--r--   0 root         (0) root         (0)     5982 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/relation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/relation_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3044 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/scalar.proto
--rw-r--r--   0 root         (0) root         (0)    32882 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/scalar_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14459 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/scalar_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      695 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/schema.proto
--rw-r--r--   0 root         (0) root         (0)    12546 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/schema_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/schema_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/size.proto
--rw-r--r--   0 root         (0) root         (0)     6233 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/size_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2162 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/size_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3909 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/statistics.proto
--rw-r--r--   0 root         (0) root         (0)    91981 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/statistics_pb2.py
--rw-r--r--   0 root         (0) root         (0)    32903 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/statistics_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/status.proto
--rw-r--r--   0 root         (0) root         (0)    18816 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     5557 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/transform.proto
--rw-r--r--   0 root         (0) root         (0)   105993 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/transform_pb2.py
--rw-r--r--   0 root         (0) root         (0)    37589 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/transform_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4496 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/type.proto
--rw-r--r--   0 root         (0) root         (0)    73431 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/type_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28800 2023-04-07 10:10:31.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/type_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3914 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/utilities.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    11280 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/scalar.py
--rw-rw-rw-   0 root         (0) root         (0)     4555 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/size.py
--rw-rw-rw-   0 root         (0) root         (0)    43542 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)    17816 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.633953 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11812 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/storage/local.py
--rw-rw-rw-   0 root         (0) root         (0)     5153 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/storage/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3078 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/storage/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    30392 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/transform.py
--rw-rw-rw-   0 root         (0) root         (0)   127509 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/type.py
--rw-rw-rw-   0 root         (0) root         (0)    34377 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3983 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/variant_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 10:10:41.635953 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)      436 2023-04-07 10:10:41.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6566 2023-04-07 10:10:41.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 10:10:41.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 10:10:41.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec_public.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      113 2023-04-07 10:10:41.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-07 10:10:41.000000 sarus_data_spec_public-3.0.0.dev2/sarus_data_spec_public.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     4625 2023-04-07 10:10:41.636953 sarus_data_spec_public-3.0.0.dev2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1191 2023-04-07 10:10:19.000000 sarus_data_spec_public-3.0.0.dev2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.760588 sarus_data_spec_public-3.0.1.dev0/
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      436 2023-04-17 16:16:48.760588 sarus_data_spec_public-3.0.1.dev0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.707583 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/
+-rwxrwxrwx   0 root         (0) root         (0)      830 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.710583 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5582 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/admin_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/array.py
+-rw-rw-rw-   0 root         (0) root         (0)     2795 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/pandas_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6260 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9709 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/type.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)     4618 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.711583 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/config/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2744 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/config/privacy_properties.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     6687 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/config/routing.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3587 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.712583 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/context/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/context/public.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/context/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/context/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    18537 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.714583 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_rewriter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_rewriter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2286 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_rewriter/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    12691 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_rewriter/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_rewriter/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.716584 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11044 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/privacy_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4470 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8849 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8284 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/json_serialisation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.717584 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7230 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/async_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    28484 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.718584 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8138 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.719584 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/local/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2172 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/local/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.720584 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/remote/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/remote/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/remote/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.721584 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3552 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.721584 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.726585 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15727 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/external_op.py
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/imblearn.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.727585 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28988 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)    28830 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     7976 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/protection_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5482 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     9271 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/sklearn.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/skopt.py
+-rw-rw-rw-   0 root         (0) root         (0)     3093 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/std.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      821 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/xgboost.py
+-rw-rw-rw-   0 root         (0) root         (0)    10449 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.732585 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13739 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)    11529 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)    10703 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/get_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    10747 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     6519 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/select_sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/shuffle.py
+-rw-rw-rw-   0 root         (0) root         (0)    10106 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/standard_op.py
+-rw-rw-rw-   0 root         (0) root         (0)    10991 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/synthetic.py
+-rw-rw-rw-   0 root         (0) root         (0)    27153 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.733585 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/source/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/source/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/source/privacy_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/source/random_seed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/source/routing.py
+-rw-rw-rw-   0 root         (0) root         (0)    12588 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/marginals.py
+-rw-rw-rw-   0 root         (0) root         (0)     3127 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/predicate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.756588 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/
+-rw-rw-rw-   0 root         (0) root         (0)     1978 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/attribute.proto
+-rw-r--r--   0 root         (0) root         (0)     5552 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/attribute_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/bounds.proto
+-rw-r--r--   0 root         (0) root         (0)     6306 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/bounds_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/bounds_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      322 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/constraint.proto
+-rw-r--r--   0 root         (0) root         (0)     8070 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/constraint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/constraint_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/dataset.proto
+-rw-r--r--   0 root         (0) root         (0)    24833 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/dataset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8880 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/dataset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/links.proto
+-rw-r--r--   0 root         (0) root         (0)    11282 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/links_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4193 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/links_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/manager.proto
+-rw-r--r--   0 root         (0) root         (0)     4572 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/manager_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/manager_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/marginals.proto
+-rw-r--r--   0 root         (0) root         (0)     6408 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/marginals_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/marginals_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/path.proto
+-rw-r--r--   0 root         (0) root         (0)     4998 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/path_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/path_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/predicate.proto
+-rw-r--r--   0 root         (0) root         (0)    13369 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/predicate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4859 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/predicate_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/proto_container.proto
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/proto_container_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/proto_container_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/relation.proto
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/relation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/relation_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3044 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/scalar.proto
+-rw-r--r--   0 root         (0) root         (0)    32882 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/scalar_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14459 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/scalar_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      695 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/schema.proto
+-rw-r--r--   0 root         (0) root         (0)    12546 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/schema_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/schema_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/size.proto
+-rw-r--r--   0 root         (0) root         (0)     6233 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/size_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/size_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/statistics.proto
+-rw-r--r--   0 root         (0) root         (0)    91981 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/statistics_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    32903 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/statistics_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/status.proto
+-rw-r--r--   0 root         (0) root         (0)    18816 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     5640 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/transform.proto
+-rw-r--r--   0 root         (0) root         (0)   107770 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/transform_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    38135 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/transform_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4496 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/type.proto
+-rw-r--r--   0 root         (0) root         (0)    73431 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28800 2023-04-17 16:16:37.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/type_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3914 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/utilities.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    10611 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4555 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/size.py
+-rw-rw-rw-   0 root         (0) root         (0)    43542 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)    17816 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.758588 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11812 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/storage/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     5153 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/storage/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3078 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/storage/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    31051 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)   136116 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/type.py
+-rw-rw-rw-   0 root         (0) root         (0)    35122 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3983 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/variant_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 16:16:48.760588 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      436 2023-04-17 16:16:48.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6787 2023-04-17 16:16:48.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 16:16:48.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 16:16:48.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec_public.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      113 2023-04-17 16:16:48.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-17 16:16:48.000000 sarus_data_spec_public-3.0.1.dev0/sarus_data_spec_public.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4878 2023-04-17 16:16:48.761588 sarus_data_spec_public-3.0.1.dev0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1191 2023-04-17 16:16:24.000000 sarus_data_spec_public-3.0.1.dev0/setup.py
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/__init__.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sarus_data_spec.transform import Transform
 from sarus_data_spec.variant_constraint import VariantConstraint
 
 """A library to manage Sarus datasets"""
 # pylint: disable=unused-variable
 
 PACKAGE_NAME: Final[str] = 'sarus_data_spec'
-VERSION: Final[str] = '3.0.0.dev2'
+VERSION: Final[str] = '3.0.1.dev0'
 
 try:
     import sarus_data_spec.context.worker as sw
 
     push_global_context(sw.WorkerContext())
 except ModuleNotFoundError as exception:
     if exception.name == 'sarus_data_spec.context.worker':
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/arrow/array.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/array.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/arrow/schema.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import typing as t
 
 import pyarrow as pa
 
-from sarus_data_spec.constants import DATA, PUBLIC, USER_COLUMN, WEIGHTS
 from sarus_data_spec.type import Struct, Type
 import sarus_data_spec.arrow.type as arrow_type
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 
 
 def to_arrow(schema: sp.Schema) -> pa.schema:
@@ -211,48 +210,18 @@
             pass
 
     visitor = SchemaVisitor()
     _type.accept(visitor)
     return visitor.schema
 
 
-def has_protected_format(schema: pa.Schema) -> bool:
-    """Checks if the pyarrow schema corresponds to the Sarus protected
-    format."""
-    return set(schema.names) == {DATA, USER_COLUMN, WEIGHTS, PUBLIC}
-
-
 def type_from_arrow_schema(schema: pa.Schema) -> st.Type:
     """Convert a Pyarrow schema to a Sarus Type.
 
-    NB:
-      - This does not handle the multitable case.
-      - We need to handle differently the protected schema case because we
-        cannot easily explore the StructType with Pyarrow < 10
+    NB: This does not handle the multitable case.
     """
-    if has_protected_format(schema):
-        # TODO Remove this case when we have Pyarrow >= 10.0
-
-        def normalize_field_name(field_name: str) -> str:
-            """When flattening the fields, the field name becomes
-            `data.field_name`."""
-            return field_name[(len(DATA) + 1) :]
-
-        data_fields = {
-            normalize_field_name(field.name): arrow_type.type_from_arrow(
-                field.type, nullable=False
-            )
-            for field in schema.field(DATA).flatten()
-        }
-        fields = {
-            name: arrow_type.type_from_arrow(data_type, nullable=False)
-            for name, data_type in zip(schema.names, schema.types)
-            if name != DATA
-        }
-        fields[DATA] = Struct(fields=data_fields)
-    else:
-        fields = {
-            name: arrow_type.type_from_arrow(data_type, nullable=False)
-            for name, data_type in zip(schema.names, schema.types)
-        }
+    fields = {
+        name: arrow_type.type_from_arrow(data_type, nullable=False)
+        for name, data_type in zip(schema.names, schema.types)
+    }
 
     return Struct(fields=fields)
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/arrow/type.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/arrow/type.py`

 * *Files 5% similar despite different names*

```diff
@@ -297,14 +297,27 @@
                 return sdt.Duration(unit=type.unit)
             else:
                 raise ValueError(
                     'Duration type with nanosecond resolution not supported'
                 )
     if pa.types.is_null(type):
         return sdt.Unit()
+    if pa.types.is_struct(type):
+        struct_type = t.cast(pa.StructType, type)
+        return sdt.Struct(
+            {
+                struct_type.field(i).name: type_from_arrow(
+                    struct_type.field(i).type, nullable=False
+                )
+                for i in range(struct_type.num_fields)
+            }
+        )
     raise NotImplementedError('Type not implemented')
 
 
-def type_from_arrow(arrow_type: pa.DataType, nullable: bool) -> st.Type:
+def type_from_arrow(
+    arrow_type: pa.DataType,
+    nullable: bool,
+) -> st.Type:
     if nullable and not (pa.types.is_null(arrow_type)):
         return sdt.Optional(type=from_arrow(arrow_type))
     return from_arrow(arrow_type)
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/attribute.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/attribute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/base.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/bounds.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/bounds.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/config/__init__.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/config/privacy_properties.yaml` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/config/privacy_properties.yaml`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/config/routing.yaml` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/config/routing.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -100,60 +100,62 @@
     SK_INVERSE_TRANSFORM: sk_inverse_transform
     SK_PREDICT: sk_predict
     SK_PREDICT_LOG_PROBA: sk_predict_log_proba
     SK_PREDICT_PROBA: sk_predict_proba
     SK_SCORE: sk_score
     SK_TRANSFORM: sk_transform
     SK_SCALE: sk_scale
-    SK_ONEHOT: model_fit
-    SK_PCA: model_fit
+    SK_ONEHOT: sk_onehot
+    SK_PCA: sk_pca
     # cluster
-    SK_AFFINITY_PROPAGATION: model_fit
-    SK_AGGLOMERATIVE_CLUSTERING: model_fit
-    SK_BIRCH: model_fit
-    SK_DBSCAN: model_fit
-    SK_FEATURE_AGGLOMERATION: model_fit
-    SK_KMEANS: model_fit
-    SK_MINIBATCH_KMEANS: model_fit
-    SK_MEAN_SHIFT: model_fit
-    SK_OPTICS: model_fit
-    SK_SPECTRAL_CLUSTERING: model_fit
-    SK_SPECTRAL_BICLUSTERING: model_fit
-    SK_SPECTRAL_COCLUSTERING: model_fit
+    SK_AFFINITY_PROPAGATION: sk_affinity_propagation
+    SK_AGGLOMERATIVE_CLUSTERING: sk_agglomerative_clustering
+    SK_BIRCH: sk_birch
+    SK_DBSCAN: sk_dbscan
+    SK_FEATURE_AGGLOMERATION: sk_feature_agglomeration
+    SK_KMEANS: sk_kmeans
+    SK_MINIBATCH_KMEANS: sk_minibatch_kmeans
+    SK_MEAN_SHIFT: sk_mean_shift
+    SK_OPTICS: sk_optics
+    SK_SPECTRAL_CLUSTERING: sk_spectral_clustering
+    SK_SPECTRAL_BICLUSTERING: sk_spectral_biclustering
+    SK_SPECTRAL_COCLUSTERING: sk_spectral_coclustering
     # compose
     SK_COLUMN_TRANSFORMER: sk_column_transformer
     # ensemble
-    SK_ADABOOST_CLASSIFIER: model_fit
-    SK_ADABOOST_REGRESSOR: model_fit
-    SK_BAGGING_CLASSIFIER: model_fit
-    SK_BAGGING_REGRESSOR: model_fit
-    SK_EXTRA_TREES_CLASSIFIER: model_fit
-    SK_EXTRA_TREES_REGRESSOR: model_fit
-    SK_GRADIENT_BOOSTING_CLASSIFIER: model_fit
-    SK_GRADIENT_BOOSTING_REGRESSOR: model_fit
-    SK_ISOLATION_FOREST: model_fit
-    SK_RANDOM_FOREST_CLASSIFIER: model_fit
-    SK_RANDOM_FOREST_REGRESSOR: model_fit
-    SK_RANDOM_TREES_EMBEDDING: model_fit
-    SK_STACKING_CLASSIFIER: model_fit
-    SK_STACKING_REGRESSOR: model_fit
-    SK_VOTING_CLASSIFIER: model_fit
-    SK_VOTING_REGRESSOR: model_fit
-    SK_HIST_GRADIENT_BOOSTING_CLASSIFIER: model_fit
-    SK_HIST_GRADIENT_BOOSTING_REGRESSOR: model_fit
+    SK_ADABOOST_CLASSIFIER: sk_adaboost_classifier
+    SK_ADABOOST_REGRESSOR: sk_adaboost_regressor
+    SK_BAGGING_CLASSIFIER: sk_bagging_classifier
+    SK_BAGGING_REGRESSOR: sk_bagging_regressor
+    SK_EXTRA_TREES_CLASSIFIER: sk_extra_trees_classifier
+    SK_EXTRA_TREES_REGRESSOR: sk_extra_trees_regressor
+    SK_GRADIENT_BOOSTING_CLASSIFIER: sk_gradient_boosting_classifier
+    SK_GRADIENT_BOOSTING_REGRESSOR: sk_gradient_boosting_regressor
+    SK_ISOLATION_FOREST: sk_isolation_forest
+    SK_RANDOM_FOREST_CLASSIFIER: sk_random_forest_classifier
+    SK_RANDOM_FOREST_REGRESSOR: sk_random_forest_regressor
+    SK_RANDOM_TREES_EMBEDDING: sk_random_trees_embedding
+    SK_STACKING_CLASSIFIER: sk_stacking_classifier
+    SK_STACKING_REGRESSOR: sk_stacking_regressor
+    SK_VOTING_CLASSIFIER: sk_voting_classifier
+    SK_VOTING_REGRESSOR: sk_voting_regressor
+    SK_HIST_GRADIENT_BOOSTING_CLASSIFIER: sk_hist_gradient_boosting_classifier
+    SK_HIST_GRADIENT_BOOSTING_REGRESSOR: sk_hist_gradient_boosting_regressor
     # impute
     SK_SIMPLE_IMPUTER: sk_simple_imputer
     # linear_model
     SK_LINEAR_REGRESSION : sk_linear_regression
     # model selection
     SK_CROSS_VAL_SCORE: sk_cross_val_score
     SK_TRAIN_TEST_SPLIT: sk_train_test_split
     SK_GET_N_SPLITS: sk_get_n_splits
     SK_SPLIT: sk_split
     SK_TIME_SERIES_SPLIT: sk_time_series_split
+    SK_REPEATED_STRATIFIED_KFOLD: sk_repeated_stratified_kfold
+    SK_KFOLD: sk_kfold
     # metrics
     SK_ACCURACY_SCORE: sk_accuracy_score
     SK_AVERAGE_PRECISION_SCORE: sk_average_precision_score
     SK_CLASSIFICATION_REPORT: sk_classification_report
     SK_CONFUSION_MATRIX: sk_confusion_matrix
     SK_F1_SCORE: sk_f1_score
     SK_PLOT_CONFUSION_MATRIX: sk_plot_confusion_matrix
@@ -168,21 +170,25 @@
     # pipeline
     SK_PIPELINE: sk_pipeline
     # preprocessing
     SK_FUNCTION_TRANSFORMER: sk_function_transformer
     # ensemble predict
     SK_RANDOM_FOREST_CLASSIFIER_PREDICT: sk_predict
     SK_LABEL_ENCODER_FIT_TRANSFORM: sk_label_encoder_fit_transform
+    SK_LABEL_ENCODER: sk_label_encoder
     # inspection
     SK_PERMUTATION_IMPORTANCE: sk_permutation_importance
+    # svm
+    SK_SVC: sk_svc
 
   xgboost:
     XGB_FIT: xgb_fit
     XGB_PREDICT: xgb_predict
     XGB_PREDICT_PROBA: xgb_predict_proba
+    XGB_CLASSIFIER: xgb_classifier
 
   skopt:
     SKOPT_BAYES_SEARCH_CV: skopt_bayes_search_cv
 
   imblearn:
     IMB_PIPELINE: imb_pipeline
     IMB_RANDOM_UNDER_SAMPLER: imb_random_under_sampler
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/constants.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from enum import Enum
 
-import pandas as pd
-
 from sarus_data_spec import typing as st
 
 DATA = 'data'
 USER_COLUMN = 'sarus_protected_entity'
 WEIGHTS = 'sarus_weights'
 PUBLIC = 'sarus_is_public'
 
@@ -33,14 +31,15 @@
 TEXT_CHARSET = 'text_char_set'
 TEXT_EXACT_CHARSET = 'FullUserInput'
 TEXT_ALPHABET_NAME = 'text_alphabet_name'
 SQL_MAPPING = 'sql_mapping'
 FLOAT_DISTRIBUTION = 'distribution_model'
 FLOAT_DIST_PARAMS = 'parameters'
 MAX_MAX_MULT = 'max_max_multiplicity'
+RECOMPUTE_TYPE_RANGES = 'recompute_type_ranges'
 
 # constants for dataset properties
 DATASET_SLUGNAME = 'slugname'
 
 # constants for schema properties
 PRIMARY_KEYS = 'primary_keys'
 FOREIGN_KEYS = 'foreign_keys'
@@ -112,15 +111,15 @@
 QUERIES = 'queries'
 
 # Attributes names
 PRIVATE_QUERY = "private_query"
 IS_REMOTE = "is_remote"
 VARIANT_UUID = "variant_uuid"
 RELATIONSHIP_SPEC = "relationship_spec"
-
+VALIDATED_TYPE = 'validated_type'
 
 # SYNTHETIC DATA
 SYNTHETIC_MODEL = 'sarus_synthetic_model'
 TRAIN_CORRELATIONS = 'train_correlations'
 
 
 class SyntheticDataSettings:
@@ -138,9 +137,10 @@
     "sqlite": st.SQLDialect.SQLLITE,
     "oracle": st.SQLDialect.ORACLE,
     "bigquery": st.SQLDialect.BIG_QUERY,
     "redshift": st.SQLDialect.REDSHIFT,
     "hive": st.SQLDialect.HIVE,
 }
 
-# List of types a Dataset can be converted to
-DATASET_TYPES = [pd.DataFrame]
+# Possible values
+POSSIBLE_VALUES_LENGTH = 'possible_values_length'
+POSSIBLE_VALUES = 'possible_values'
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/context/public.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/context/public.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/context/typing.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/context/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataset.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,17 @@
             if last_status.task(task) is None:
                 return None
         return last_status
 
     def schema(self) -> st.Schema:
         return self.manager().schema(self)
 
+    async def async_schema(self) -> st.Schema:
+        return await self.manager().async_schema(self)
+
     def size(self) -> t.Optional[Size]:
         return cast('Size', self.manager().size(self))
 
     def bounds(self) -> t.Optional[Bounds]:
         return cast('Bounds', self.manager().bounds(self))
 
     def marginals(self) -> t.Optional[Marginals]:
@@ -242,14 +245,23 @@
 
     def to_pandas(self) -> pd.DataFrame:
         return self.manager().to_pandas(self)
 
     async def async_to_pandas(self) -> pd.DataFrame:
         return await self.manager().async_to_pandas(self)
 
+    async def async_to(
+        self, kind: t.Type, drop_admin: bool = True
+    ) -> st.DatasetCastable:
+        """Convert a Dataset's to a Python type."""
+        return await self.manager().async_to(self, kind, drop_admin)
+
+    def to(self, kind: t.Type, drop_admin: bool = True) -> st.DatasetCastable:
+        return self.manager().to(self, kind, drop_admin)
+
     def to_tensorflow(self) -> tf.data.Dataset:
         return self.manager().to_tensorflow(self)
 
     async def async_to_tensorflow(self) -> tf.data.Dataset:
         return await self.manager().async_to_tensorflow(self)
 
     # A Visitor acceptor
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_rewriter/base.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_rewriter/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_rewriter/simple_rules.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_rewriter/simple_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,8 +369,19 @@
     )
     attach_variant(
         original=dataspec,
         variant=dp_variant,
         kind=st.ConstraintKind.DP,
     )
 
+    # We also attach the dataspec's synthetic variant to be the DP dataspec's
+    # synthetic variant. This is to avoid to have DP computations in the MOCK.
+    syn_variant = dataspec.variant(st.ConstraintKind.SYNTHETIC)
+    if syn_variant is None:
+        raise ValueError("Could not find a synthetic variant.")
+    attach_variant(
+        original=dp_variant,
+        variant=syn_variant,
+        kind=st.ConstraintKind.SYNTHETIC,
+    )
+
     return dp_variant, public_context
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_rewriter/typing.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_rewriter/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_validator/base.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,16 +175,15 @@
             is_public = all(
                 [self.is_public(ds) for ds in args_parents]
                 + [self.is_public(ds) for ds in kwargs_parents.values()]
             )
         elif dataspec.prototype() == sp.Scalar:
             scalar = cast(st.Scalar, dataspec)
             assert (
-                scalar.is_model()
-                or scalar.is_random_seed()
+                scalar.is_random_seed()
                 or scalar.is_privacy_params()
                 or scalar.is_synthetic_model()
             )
             is_public = True
         else:
             is_public = False
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_validator/privacy_limit.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/privacy_limit.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_validator/simple_rules.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/simple_rules.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/dataspec_validator/typing.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/dataspec_validator/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/deprecation.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/deprecation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/factory.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/factory.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/async_utils.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/async_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,24 +26,21 @@
         # this method allows to set the curr loop
         # as running,standard method asyncio.set_event_loop
         # does not work
         events._set_running_loop(curr_loop)
     return result
 
 
-def sync_iterator(
-    async_iterator_coro: t.Coroutine,
-) -> t.Iterator[t.Any]:
-    """This methods returns an iterator from an async iterator coroutine.
-    It first executes the coroutine to obtain an async generator.
-    Then, generator method allows to execute one step at a time the
+def sync_iterator_from_async_iterator(
+    async_iterator: t.AsyncIterator[T],
+) -> t.Iterator[T]:
+    """This methods returns an iterator from an async iterator.
+    The generator method allows to execute one step at a time the
     anext method of the async generator.
     """
-
-    async_gen = sync(async_iterator_coro)
     # The loop used to generate batches
     new_loop = asyncio.new_event_loop()
     new_loop._check_running = lambda: None  # type:ignore
     # method monkey patched since it raises an error
     # if another loop exists
 
     def generator() -> t.Iterator[T]:
@@ -56,15 +53,15 @@
         while keep_on:
             reset_at_completion = True
             try:
                 curr_loop = asyncio.get_running_loop()
             except RuntimeError:
                 reset_at_completion = False
             try:
-                batch = new_loop.run_until_complete(async_gen.__anext__())
+                batch = new_loop.run_until_complete(async_iterator.__anext__())
 
             except StopAsyncIteration:
                 keep_on = False
                 if reset_at_completion:
                     events._set_running_loop(curr_loop)
             except Exception as exception:
                 if reset_at_completion:
@@ -75,14 +72,26 @@
                     # asyncio.set_event_loop(curr_loop) not working
                     events._set_running_loop(curr_loop)
                 yield batch
 
     return generator()
 
 
+def sync_iterator(
+    async_iterator_coro: t.Coroutine,
+) -> t.Iterator[t.Any]:
+    """This methods returns an iterator from an async iterator coroutine.
+    It first executes the coroutine to obtain an async generator.
+    Then, generator method allows to execute one step at a time the
+    anext method of the async generator.
+    """
+    async_gen = sync(async_iterator_coro)
+    return sync_iterator_from_async_iterator(async_gen)
+
+
 async def async_iter(data_list: t.Collection[T]) -> t.AsyncIterator[T]:
     """Convert a collection into an AsyncIterator."""
     for data in data_list:
         yield data
 
 
 async def decoupled_async_iter(
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/base.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 import os
 import typing as t
 import warnings
 
 import pandas as pd
 import pyarrow as pa
 
+from sarus_data_spec.arrow.admin_utils import async_to_arrow_extract_data_only
 from sarus_data_spec.arrow.array import convert_record_batch
+from sarus_data_spec.arrow.conversion import async_cast_arrow_batches
 from sarus_data_spec.attribute import attach_properties
 from sarus_data_spec.constants import (
     BIG_DATA_TASK,
     BIG_DATA_THRESHOLD,
     DATASET_N_BYTES,
     DATASET_N_LINES,
-    DATASET_TYPES,
     IS_BIG_DATA,
     IS_REMOTE,
     THRESHOLD_TYPE,
 )
 from sarus_data_spec.dataspec_rewriter.base import BaseDataspecRewriter
 from sarus_data_spec.dataspec_validator.base import BaseDataspecValidator
 from sarus_data_spec.manager.async_utils import sync, sync_iterator
@@ -197,28 +198,29 @@
             'public_paths',
             'automatic_budget',
             'attribute_budget',
             'sd_budget',
             'sampling_ratios',
             'derive_seed',
             'relationship_spec',
+            'validated_user_type',
         ]:
             return sp.type_name(sp.Scalar), attach_nothing
 
         # Other internal transforms return a Dataset
         if not transform.is_external():
             return sp.type_name(sp.Dataset), attach_nothing
 
         # Compute the mock value for external transforms
         mock_value = self.mock_value(transform, *arguments, **named_arguments)
 
         # Infer output types
         dataspec_type = (
             sp.type_name(sp.Dataset)
-            if type(mock_value) in DATASET_TYPES
+            if type(mock_value) in t.get_args(st.DatasetCastable)
             else sp.type_name(sp.Scalar)
         )
 
         # Return the output type
         return dataspec_type, attach_nothing
 
     def is_big_data(self, dataset: st.Dataset) -> bool:
@@ -347,14 +349,19 @@
         raise NotImplementedError
 
     def computation_max_delay(self, dataspec: st.DataSpec) -> int:
         raise NotImplementedError
 
     # ------SYNC COMPUTATIONS METHODS--------------
 
+    def to(
+        self, dataset: st.Dataset, kind: t.Type, drop_admin: bool = True
+    ) -> st.DatasetCastable:
+        return sync(self.async_to(dataset, kind, drop_admin))
+
     def bounds(self, dataset: st.Dataset) -> st.Bounds:
         return t.cast(Bounds, sync(self.async_bounds(dataset)))
 
     def cache_scalar(self, scalar: st.Scalar) -> None:
         sync(self.async_cache_scalar(scalar=scalar))
 
     def links(self, dataset: st.Dataset) -> st.Links:
@@ -408,14 +415,34 @@
         return sync(self.async_to_tensorflow(dataset=dataset))
 
     def value(self, scalar: st.Scalar) -> st.DataSpecValue:
         return sync(self.async_value(scalar=scalar))
 
     # ------ASYNC COMPUTATIONS--------
 
+    async def async_to(
+        self, dataset: st.Dataset, kind: t.Type, drop_admin: bool = True
+    ) -> st.DatasetCastable:
+        """Convert a Dataset's to a Python type."""
+        if drop_admin:
+            batches_async_it = await async_to_arrow_extract_data_only(
+                dataset=dataset, batch_size=BATCH_SIZE
+            )
+        else:
+            if kind not in [pd.DataFrame, t.Iterator[pa.RecordBatch]]:
+                raise TypeError(
+                    f"The target type {kind} is not compatible"
+                    " with the protection."
+                )
+            batches_async_it = await dataset.async_to_arrow(
+                batch_size=BATCH_SIZE
+            )
+
+        return await async_cast_arrow_batches(batches_async_it, kind)
+
     async def async_bounds(self, dataset: st.Dataset) -> st.Bounds:
         raise NotImplementedError
 
     async def async_cache_scalar(self, scalar: st.Scalar) -> None:
         await self.cache_scalar_computation.complete_task(dataspec=scalar)
 
     async def async_prepare(self, dataspec: st.DataSpec) -> None:
@@ -513,19 +540,17 @@
             element for element in results if isinstance(element, Exception)
         ]
         if len(exceptions) == 0:
             return
         raise error_aggregation(exceptions)
 
     async def async_to_pandas(self, dataset: st.Dataset) -> pd.DataFrame:
-        batches_async_it = await self.async_to_arrow(
-            dataset=dataset, batch_size=BATCH_SIZE
+        return await self.async_to(
+            dataset=dataset, kind=pd.DataFrame, drop_admin=False
         )
-        arrow_batches = [batch async for batch in batches_async_it]
-        return pa.Table.from_batches(arrow_batches).to_pandas()
 
     async def async_value(self, scalar: st.Scalar) -> t.Any:
         """Reads asynchronously value of a scalar."""
         computation = self.dataspec_computation(scalar)
         return await computation.task_result(dataspec=scalar)
 
     # -------- COMPILATION---------
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/computations/base.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/computations/local/base.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/local/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/computations/local/schema.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/local/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/computations/remote/base.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/computations/remote/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/base.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/external_op.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/external_op.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+from __future__ import annotations
+
 import hashlib
 import importlib
 import inspect
-import pickle as pkl
 import typing as t
 
-import pandas as pd
 import pyarrow as pa
 
+from sarus_data_spec.arrow.admin_utils import (
+    compute_admin_data,
+    merge_data_and_admin,
+)
+from sarus_data_spec.arrow.conversion import to_pyarrow_table
 from sarus_data_spec.arrow.schema import type_from_arrow_schema
 from sarus_data_spec.config import ROUTING
 from sarus_data_spec.dataspec_validator.typing import PEPKind
 from sarus_data_spec.manager.async_utils import async_iter
 from sarus_data_spec.manager.ops.base import (
     DatasetImplementation,
     DatasetStaticChecker,
@@ -20,21 +25,16 @@
 from sarus_data_spec.schema import schema as schema_builder
 from sarus_data_spec.transform import external, transform_id
 import sarus_data_spec.manager.typing as smt
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.type as sdt
 import sarus_data_spec.typing as st
 
-from .protection_utils import (
-    ExternalOpImplementation,
-    arguments_values,
-    arguments_values_and_protected_entity,
-    output_protected_entity,
-    to_pyarrow_table_with_protected_entity,
-)
+from .signature import ExternalSignature
+from .utils import static_and_dynamic_arguments, static_arguments
 
 
 class ExternalScalarStaticChecker(DataspecStaticChecker):
     async def private_queries(self) -> t.List[st.PrivateQuery]:
         """Return the PrivateQueries summarizing DP characteristics."""
         transform = self.dataspec.transform()
         ds_args, ds_kwargs = self.dataspec.parents()
@@ -104,28 +104,33 @@
 
         return True
 
     def dp_transform(self) -> t.Optional[st.Transform]:
         """Return the dataspec's DP equivalent transform if existing."""
         transform = self.dataspec.transform()
         op_implementation = external_implementation(transform)
-        py_args, py_kwargs, ds_args_pos = static_arguments(transform)
+        py_args, py_kwargs, ds_args_pos, ds_types = static_arguments(transform)
 
         dp_implementation = op_implementation.dp_equivalent()
         if dp_implementation is None:
             return None
 
         dp_transform_id = dp_implementation.transform_id
         assert dp_transform_id is not None
 
+        # Types won't be used since budget & seed are scalars
+        ds_types["budget"] = ""
+        ds_types["seed"] = ""
+
         return external(
             dp_transform_id,
             py_args=py_args,
             py_kwargs=py_kwargs,
             ds_args_pos=ds_args_pos,
+            ds_types=ds_types,
         )
 
 
 class ExternalDatasetStaticChecker(
     ExternalScalarStaticChecker, DatasetStaticChecker
 ):
     def __init__(self, dataset: st.Dataset):
@@ -207,46 +212,42 @@
 
 
 class ExternalDatasetOp(DatasetImplementation):
     async def to_arrow(
         self, batch_size: int
     ) -> t.AsyncIterator[pa.RecordBatch]:
         transform = self.dataset.transform()
-        ds_args, ds_kwargs = self.dataset.parents()
-
         implementation = external_implementation(transform)
-        args, kwargs = static_and_dynamic_arguments(
-            transform, *ds_args, **ds_kwargs
-        )
 
+        signature = ExternalSignature.from_dataspec(self.dataset)
         static_checker = ExternalDatasetStaticChecker(self.dataset)
         if static_checker.is_dp():
-            (
-                data_args,
-                data_kwargs,
-                pe,
-            ) = await arguments_values_and_protected_entity(*args, **kwargs)
+            args, kwargs = signature.args(), signature.kwargs()
             result = await implementation.call(
-                *data_args, **data_kwargs, pe=pe, dataspec=self.dataset
+                *args, **kwargs, signature=signature
             )
             table = to_pyarrow_table(result)
 
         elif self.dataset.is_pep():
             (
-                data_args,
-                data_kwargs,
-                pe,
-            ) = await arguments_values_and_protected_entity(*args, **kwargs)
-            result = await implementation.call(*data_args, **data_kwargs)
-            output_pe = output_protected_entity(pe, result)
-            table = to_pyarrow_table_with_protected_entity(result, output_pe)
+                args_values,
+                kwargs_values,
+                protected_entity,
+            ) = await signature.arguments_values_and_admin_data()
+            result = await implementation.call(*args_values, **kwargs_values)
+            ds_result = t.cast(st.DatasetCastable, result)
+            output_protected_entity = compute_admin_data(
+                protected_entity, ds_result
+            )
+            data_table = to_pyarrow_table(ds_result)
+            table = merge_data_and_admin(data_table, output_protected_entity)
 
         else:
-            data_args, data_kwargs = await arguments_values(*args, **kwargs)
-            result = await implementation.call(*data_args, **data_kwargs)
+            (args_values, kwargs_values) = await signature.arguments_values()
+            result = await implementation.call(*args_values, **kwargs_values)
             table = to_pyarrow_table(result)
 
         return async_iter(table.to_batches(max_chunksize=batch_size))
 
 
 class ExternalScalarOp(ScalarImplementation):
     async def value(self) -> t.Any:
@@ -266,66 +267,139 @@
 
     This function computes the output value without manipulating the
     corresponding Dataspec. This is useful when we need to have access
     to the value of a Dataspec before its creation:
       - for computing a Mock value and inferring if the result is
         a Scalar or a Dataset.
     """
+    signature = ExternalSignature(transform, ds_args, ds_kwargs)
     implementation = external_implementation(transform)
-    args, kwargs = static_and_dynamic_arguments(
-        transform, *ds_args, **ds_kwargs
-    )
+    args, kwargs = signature.args(), signature.kwargs()
 
     if implementation.is_dp(*args, **kwargs):
-        data = await implementation.call(*args, **kwargs)
+        data = await implementation.call(*args, **kwargs, signature=signature)
 
     else:
-        data_args, data_kwargs = await arguments_values(*args, **kwargs)
-        data = await implementation.call(*data_args, **data_kwargs)
+        (args_values, kwargs_values) = await signature.arguments_values()
+        data = await implementation.call(*args_values, **kwargs_values)
 
     return data
 
 
-def to_pyarrow_table(data: t.Any) -> pa.Table:
-    """Convert the result of an external transform to a Pyarrow Table."""
-    if not isinstance(data, pd.DataFrame):
-        raise TypeError(f"Cannot convert {type(data)} to Arrow batches.")
+class ExternalOpImplementation:
+    """External PEP op implementation class.
 
-    df = t.cast(pd.DataFrame, data)
-    return pa.Table.from_pandas(df)
+    This class wraps together several elements of an external op
+    implementation:
+        - `call` is the function that computes the output value from the
+          input(s) value(s).
+    """
 
+    transform_id: str
+    _dp_equivalent: t.Optional[t.Type[ExternalOpImplementation]] = None
+    allowed_pep_args: t.List[t.Set[str]] = []
 
-def group_by_pep(
-    op_implementation: smt.ExternalOpImplementation,
-    *args: t.Any,
-    **kwargs: t.Any,
-) -> t.Tuple[t.Dict[str, st.DataSpec], t.Dict[str, st.DataSpec]]:
-    """Get Dataspec arguments and split them between PEP and non PEP.
+    def dp_equivalent(self) -> t.Optional[ExternalOpImplementation]:
+        if not self._dp_equivalent:
+            return None
+        return self._dp_equivalent()
 
-    This also identifies positional arguments by names based on the `call`
-    signature.
+    @staticmethod
+    async def call(*args: t.Any, **kwargs: t.Any) -> t.Any:
+        raise NotImplementedError
+
+    def pep_kind(self, *args: t.Any, **kwargs: t.Any) -> PEPKind:
+        """Return the PEP properties of the transform.
+
+        It takes the transform arguments as input because it can depend on some
+        transform parameters. For instance, it is not PEP if we are aggregating
+        the rows (axis=0) and it is PEP if we are aggregating the columns
+        (axis=1).
+
+        NB: This function should have the same signature as the call function.
+        """
+        # Default implementation
+        return PEPKind.NOT_PEP
+
+    def is_dp(self, *args: t.Any, **kwargs: t.Any) -> bool:
+        """Return True if the DP transform is compatible with the arguments.
+
+        It takes the transform arguments as input because it can depend on some
+        transform parameters. For instance, if we are aggregating the rows
+        (axis=0), then there might be an equivalent DP transform but if we are
+        aggregating the columns there might not (axis=1).
+
+        NB: This function should have the same signature as the call function.
+        """
+        return False
+
+    async def private_queries(
+        self,
+        *args: t.Any,
+        budget: t.Optional[st.Scalar] = None,
+        seed: t.Optional[st.Scalar] = None,
+        **kwargs: t.Any,
+    ) -> t.List[st.PrivateQuery]:
+        """Takes as input the args of the transform (static and dynamic)."""
+        if budget is None or seed is None:
+            return []
+        # Evaluate budget and seed
+        budget_value = await budget.async_value()
+        seed_value = await seed.async_value()
+        queries, _ = await self.private_queries_and_task(
+            *args, budget=budget_value, seed=seed_value, **kwargs
+        )
+        return queries
+
+    @staticmethod
+    async def private_queries_and_task(
+        *args: t.Any, **kwargs: t.Any
+    ) -> t.Tuple[t.List[st.PrivateQuery], st.Task]:
+        raise NotImplementedError
+
+
+def make_all_named_arguments(
+    op_implementation: smt.ExternalOpImplementation,
+    args: t.Collection[t.Any],
+    kwargs: t.Dict[str, t.Any],
+) -> t.Dict[str, t.Any]:
+    """Attribute a name to all arguments serialized in the protobuf by using
+    the implementation's `call` method signature.
     """
-    # Add name to positional arguments to identify them by their names
     n_args = len(args)
     argument_names = list(
         inspect.signature(op_implementation.call).parameters.keys()
     )
     """
     Example :
     In [1]: def foo(a, b=3):
     ...:     return a+b
-    ...:
 
     In [2]: list(inspect.signature(foo).parameters.keys())
     Out[2]: ['a', 'b']
     """
     for arg_name, arg_val in zip(argument_names[:n_args], args):
         # put all args in kwargs
         kwargs[arg_name] = arg_val
 
+    return kwargs
+
+
+def group_by_pep(
+    op_implementation: smt.ExternalOpImplementation,
+    *args: t.Any,
+    **kwargs: t.Any,
+) -> t.Tuple[t.Dict[str, st.DataSpec], t.Dict[str, st.DataSpec]]:
+    """Get Dataspec arguments and split them between PEP and non PEP.
+
+    This also identifies positional arguments by names based on the `call`
+    signature.
+    """
+    kwargs = make_all_named_arguments(op_implementation, args, kwargs)
+
     # Keep only dataspec args and split PEP from non PEP
     dataspec_args = {
         arg_name: arg
         for arg_name, arg in kwargs.items()
         if isinstance(arg, st.DataSpec)
     }
     pep_args = {
@@ -337,43 +411,14 @@
         arg_name: arg
         for arg_name, arg in dataspec_args.items()
         if arg_name not in pep_args
     }
     return pep_args, non_pep_args
 
 
-def static_arguments(
-    transform: st.Transform,
-) -> t.Tuple[t.Dict[int, t.Any], t.Dict[str, t.Any], t.List[int]]:
-    """Return the external arguments serialized in the protobuf."""
-    assert transform and transform.is_external()
-
-    transform_spec = transform.protobuf().spec
-    external_args = pkl.loads(transform_spec.external.named_arguments)
-    py_args = external_args["py_args"]
-    py_kwargs = external_args["py_kwargs"]
-    ds_args_pos = external_args["ds_args_pos"]
-    return py_args, py_kwargs, ds_args_pos
-
-
-def static_and_dynamic_arguments(
-    transform: st.Transform, *ds_args: st.DataSpec, **ds_kwargs: st.DataSpec
-) -> t.Tuple[t.List[t.Any], t.Dict[str, t.Any]]:
-    """Return all the external arguments.
-
-    This returns static arguments interleaved with Dataspecs.
-    """
-    py_args, py_kwargs, ds_args_pos = static_arguments(transform)
-    pos_values = {pos: val for pos, val in zip(ds_args_pos, ds_args)}
-    kwargs = {**py_kwargs, **ds_kwargs}
-    pos_args = {**pos_values, **py_args}
-    args = [pos_args[i] for i in range(len(pos_args))]
-    return args, kwargs
-
-
 def external_implementation(
     transform: st.Transform,
 ) -> smt.ExternalOpImplementation:
     """Return the implementation of an external op from a DataSpec.
 
     The mapping is done by the config file.
     """
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/imblearn.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/imblearn.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/numpy.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/numpy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import pandas as pd
 import pandas._typing as pdt
 
 from sarus_data_spec.dataspec_validator.typing import PEPKind
 import sarus_data_spec.typing as st
 
-from ..protection_utils import ExternalOpImplementation
+from ..external_op import ExternalOpImplementation
 from .pandas_dp import (
     pd_mean_dp,
     pd_median_dp,
     pd_shape_dp,
     pd_std_dp,
     pd_sum_dp,
 )
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,16 @@
 import pandas as pd
 import pandas._typing as pdt
 
 from sarus_data_spec.constants import MAX_MAX_MULT
 from sarus_data_spec.protobuf.utilities import unwrap
 import sarus_data_spec.typing as st
 
-from ..protection_utils import (
-    ExternalOpImplementation,
-    arguments_values,
-    arguments_values_and_protected_entity,
-)
+from ..external_op import ExternalOpImplementation
+from ..signature import ExternalSignature
 
 logger = logging.getLogger(__name__)
 
 try:
     from sarus_statistics.ops.bounds.op import BoundOp
     from sarus_statistics.ops.histograms.op import CountOp
     from sarus_statistics.ops.max_multiplicity.op import MaxMultiplicityOp
@@ -114,28 +111,32 @@
         return list(composed_query.all_subqueries()), tasks
 
     @staticmethod
     async def call(  # type: ignore[override]
         parent_ds: st.Dataset,
         budget: st.Scalar,
         seed: st.Scalar,
+        signature: ExternalSignature,
     ) -> t.Any:
         """Implementation of DP shape.
 
         A DP implementation receives additional arguments compared to a
         standard external implementation:
             - `budget`: a list of sp.Scalar.PrivacyParams.Point
                 object containing each an epsilon and a delta values
             - `seed`: an integer used to parametrize random number generators
             - `pe`: theprotected entity used by `sarus_statistics` primitives
         """
         # Evaluate arguments
-        (dataframe, budget_value, seed_value), _ = await arguments_values(
-            parent_ds, budget, seed
-        )
+        dataframe, _ = await signature._value_and_pe("parent_ds", 0)
+        (
+            budget_value,
+            _,
+        ) = await signature._value_and_pe("budget")
+        seed_value, _ = await signature._value_and_pe("seed")
 
         # Get QB task parametrization
         _, tasks = await pd_shape_dp.private_queries_and_task(
             parent_ds, budget_value
         )
 
         epsilon = budget_value[0].epsilon
@@ -247,20 +248,27 @@
         axis: t.Optional[pdt.Axis] = None,
         skipna: bool = True,
         level: t.Optional[pdt.Level] = None,
         numeric_only: t.Optional[bool] = None,
         min_count: int = 0,
         budget: t.Optional[st.Scalar] = None,
         seed: t.Optional[st.Scalar] = None,
+        signature: t.Optional[ExternalSignature] = None,
         **kwargs: t.Any,
     ) -> t.Any:
         # Evaluate arguments
-        (dataframe, budget_value, seed_value), _ = await arguments_values(
-            parent_ds, budget, seed
-        )
+        if not signature:
+            raise ValueError("Signature is None.")
+
+        dataframe, _ = await signature._value_and_pe("parent_ds", 0)
+        (
+            budget_value,
+            _,
+        ) = await signature._value_and_pe("budget")
+        seed_value, _ = await signature._value_and_pe("seed")
 
         assert type(dataframe) in [pd.DataFrame, pd.Series]
         assert numeric_only
         assert axis == 0
         assert level is None
         assert min_count == 0
         assert seed_value
@@ -402,24 +410,28 @@
         parent_ds: st.Dataset,
         axis: t.Optional[pdt.Axis] = 0,
         skipna: bool = True,
         level: t.Optional[pdt.Level] = None,
         numeric_only: t.Optional[bool] = None,
         budget: t.Optional[st.Scalar] = None,
         seed: t.Optional[st.Scalar] = None,
+        signature: t.Optional[ExternalSignature] = None,
         **kwargs: t.Any,
     ) -> t.Any:
         # Evaluate arguments
+        if not signature:
+            raise ValueError("Signature is None.")
+
+        dataframe, pe_table = await signature._value_and_pe("parent_ds", 0)
         (
-            (dataframe, budget_value, seed_value),
+            budget_value,
             _,
-            pe,
-        ) = await arguments_values_and_protected_entity(
-            parent_ds, budget, seed
-        )
+        ) = await signature._value_and_pe("budget")
+        pe = pe_table.to_pandas()
+        seed_value, _ = await signature._value_and_pe("seed")
 
         assert type(dataframe) in [pd.DataFrame, pd.Series]
         assert pe.shape[0] == dataframe.shape[0]
         assert numeric_only
         assert axis == 0
         assert level is None
         assert seed_value
@@ -559,24 +571,28 @@
         parent_ds: st.Dataset,
         axis: t.Optional[pdt.Axis] = 0,
         skipna: bool = True,
         level: t.Optional[pdt.Level] = None,
         numeric_only: t.Optional[bool] = None,
         budget: t.Optional[st.Scalar] = None,
         seed: t.Optional[st.Scalar] = None,
+        signature: t.Optional[ExternalSignature] = None,
         **kwargs: t.Any,
     ) -> t.Any:
         # Evaluate arguments
+        if not signature:
+            raise ValueError("Signature is None.")
+
+        dataframe, pe_table = await signature._value_and_pe("parent_ds", 0)
         (
-            (dataframe, budget_value, seed_value),
+            budget_value,
             _,
-            pe,
-        ) = await arguments_values_and_protected_entity(
-            parent_ds, budget, seed
-        )
+        ) = await signature._value_and_pe("budget")
+        pe = pe_table.to_pandas()
+        seed_value, _ = await signature._value_and_pe("seed")
 
         assert type(dataframe) in [pd.DataFrame, pd.Series]
         assert pe.shape[0] == dataframe.shape[0]
         assert numeric_only
         assert axis == 0
         assert level is None
         assert seed_value
@@ -719,24 +735,28 @@
         axis: t.Optional[pdt.Axis] = 0,
         skipna: bool = True,
         level: t.Optional[pdt.Level] = None,
         numeric_only: t.Optional[bool] = None,
         ddof: int = 1,
         budget: t.Optional[st.Scalar] = None,
         seed: t.Optional[st.Scalar] = None,
+        signature: t.Optional[ExternalSignature] = None,
         **kwargs: t.Any,
     ) -> t.Any:
         # Evaluate arguments
+        if not signature:
+            raise ValueError("Signature is None.")
+
+        dataframe, pe_table = await signature._value_and_pe("parent_ds", 0)
         (
-            (dataframe, budget_value, seed_value),
+            budget_value,
             _,
-            pe,
-        ) = await arguments_values_and_protected_entity(
-            parent_ds, budget, seed
-        )
+        ) = await signature._value_and_pe("budget")
+        pe = pe_table.to_pandas()
+        seed_value, _ = await signature._value_and_pe("seed")
 
         assert type(dataframe) in [pd.DataFrame, pd.Series]
         assert pe.shape[0] == dataframe.shape[0]
         assert numeric_only
         assert axis == 0
         assert level is None
         assert seed_value
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/protection_utils.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/protection_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/std.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/std.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/external/xgboost.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/external/xgboost.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 
 try:
     import xgboost  # type: ignore[import]
 except ModuleNotFoundError:
     pass  # error message in typing.py
 
 
+async def xgb_classifier(
+    *args: Any,
+    **kwargs: Any,
+) -> Any:
+    return xgboost.XGBClassifier(*args, **kwargs)
+
+
 async def xgb_fit(
     model: xgboost.XGBClassifier, *args: Any, **kwargs: Any
 ) -> xgboost.XGBClassifier:
     fitted_model = model.fit(*args, **kwargs)
     return fitted_model
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/routing.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/routing.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,21 +135,29 @@
         Transcode,
         TranscodeStaticChecker,
     )
 except ModuleNotFoundError:
     logger = logging.getLogger(__name__)
     logger.info("Transforms: GroupPE not available.")
 try:
-    from sarus_data_spec.manager.ops.processor.standard.relationship_spec import (  # noqa: E501
+    from sarus_data_spec.manager.ops.processor.standard.user_settings.relationship_spec import (  # noqa: E501
         RelationshipSpecOp,
         RelationshipSpecOpStaticChecker,
     )
 except ModuleNotFoundError:
     logger = logging.getLogger(__name__)
     logger.info("Transforms: RelationshipSpec not available.")
+try:
+    from sarus_data_spec.manager.ops.processor.standard.user_settings.validated import (  # noqa: E501
+        ValidatedUserTypeOp,
+        ValidatedUserTypeOpStaticChecker,
+    )
+except ModuleNotFoundError:
+    logger = logging.getLogger(__name__)
+    logger.info("Transforms: ValidatedUserType not available.")
 import sarus_data_spec.typing as st
 
 
 def get_dataset_op(
     transform: st.Transform,
 ) -> t.Tuple[t.Type[DatasetImplementation], t.Type[DatasetStaticChecker]]:
     if transform.is_external():
@@ -211,14 +219,16 @@
         return SDBudget, SDBudgetStaticChecker
     elif transform.name() == 'sampling_ratios':
         return SamplingRatios, SamplingRatiosStaticChecker
     elif transform.name() == 'derive_seed':
         return DeriveSeed, DeriveSeedStaticChecker
     elif transform.name() == 'relationship_spec':
         return RelationshipSpecOp, RelationshipSpecOpStaticChecker
+    elif transform.name() == 'validated_user_type':
+        return ValidatedUserTypeOp, ValidatedUserTypeOpStaticChecker
     else:
         raise NotImplementedError(f"scalar_transformed for {transform}")
 
 
 class TransformedDataset(DatasetImplementation):
     def __init__(self, dataset: st.Dataset):
         super().__init__(dataset)
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/extract.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/extract.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/filter.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/filter.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/get_item.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/get_item.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/project.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/project.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/sample.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/sample.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/select_sql.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/select_sql.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/shuffle.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/shuffle.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/standard_op.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/standard_op.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/synthetic.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/synthetic.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/ops/source/routing.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/ops/source/routing.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import typing as t
 
 import pyarrow as pa
 
 from sarus_data_spec.manager.ops.base import ScalarImplementation
 import sarus_data_spec.typing as st
 
-from .model import Model
 from .privacy_params import PrivacyParams
 from .random_seed import RandomSeed
 
 logger = logging.getLogger(__name__)
 try:
     from sarus_data_spec.manager.ops.source.sql_source import SourceSQL
 except ModuleNotFoundError:
@@ -29,17 +28,15 @@
         SyntheticModel,
     )
 except ModuleNotFoundError:
     logger.info("Synthetic generation not available")
 
 
 def get_scalar_op(scalar: st.Scalar) -> t.Type[ScalarImplementation]:
-    if scalar.is_model():
-        return Model
-    elif scalar.is_random_seed():
+    if scalar.is_random_seed():
         return RandomSeed
     elif scalar.is_privacy_params():
         return PrivacyParams
     elif scalar.is_synthetic_model():
         return SyntheticModel
     else:
         raise NotImplementedError(f"Source scalar for {scalar}")
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/manager/typing.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/manager/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,25 @@
 
     def to_pandas(self, dataset: st.Dataset) -> pd.DataFrame:
         ...
 
     async def async_to_pandas(self, dataset: st.Dataset) -> pd.DataFrame:
         ...
 
+    async def async_to(
+        self, dataset: st.Dataset, kind: t.Type, drop_admin: bool = True
+    ) -> st.DatasetCastable:
+        """Casts a Dataset to a Python type passed as argument."""
+        ...
+
+    def to(
+        self, dataset: st.Dataset, kind: t.Type, drop_admin: bool = True
+    ) -> st.DatasetCastable:
+        ...
+
     def to_tensorflow(self, dataset: st.Dataset) -> tf.data.Dataset:
         ...
 
     async def async_to_tensorflow(
         self, dataset: st.Dataset
     ) -> tf.data.Dataset:
         ...
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/marginals.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/marginals.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/path.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/path.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/predicate.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/predicate.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/__init__.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/attribute_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/attribute_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/bounds_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/bounds_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/bounds_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/bounds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/constraint_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/constraint_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/constraint_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/constraint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/dataset.proto` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/dataset.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/dataset_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/dataset_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/links_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/links_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/links_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/manager_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/manager_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/marginals_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/marginals_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/marginals_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/marginals_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/path_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/path_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/path_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/path_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/predicate.proto` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/predicate.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/predicate_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/predicate_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/predicate_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/predicate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/proto_container_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/proto_container_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/proto_container_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/proto_container_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/relation.proto` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/relation.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/relation_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/relation_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/relation_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/relation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/scalar.proto` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/scalar.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/scalar_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/scalar_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/scalar_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/scalar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/schema.proto` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/schema.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/schema_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/schema_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/size_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/size_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/size_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/size_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/statistics.proto` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/statistics.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/statistics_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/statistics_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/statistics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/status.proto` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/status.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/status_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/status_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/status_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/transform.proto` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/transform.proto`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
       DeriveSeed derive_seed = 24;
       GroupByPE group_by_pe = 25;
       SamplingRatios sampling_ratios = 26;
       SelectSql select_sql = 27;
       Extract extract = 28;
       RelationshipSpec relationship_spec = 29;
       DifferentiatedSample differentiated_sample = 30;
+      ValidatedUserType validated_user_type=31;
     }
   }
 
   message External {
     bytes arguments = 1;
     bytes named_arguments = 2;
     OpIdentifier op_identifier = 3;
@@ -256,8 +257,10 @@
       string query = 2;
     }
   }
 
   message Extract {
     int32 size = 1;
   }
+   message ValidatedUserType {
+  }
 }
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/transform_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/transform_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='sarus_data_spec/protobuf/transform.proto',
   package='',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n(sarus_data_spec/protobuf/transform.proto\x1a#sarus_data_spec/protobuf/type.proto\x1a#sarus_data_spec/protobuf/path.proto\x1a%sarus_data_spec/protobuf/scalar.proto\"\xcd\x1f\n\tTransform\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0b\n\x03\x64oc\x18\x03 \x01(\t\x12\x1d\n\x04spec\x18\x04 \x01(\x0b\x32\x0f.Transform.Spec\x12.\n\nproperties\x18\x05 \x03(\x0b\x32\x1a.Transform.PropertiesEntry\x12\x12\n\ninversible\x18\x06 \x01(\x08\x12\x19\n\x11schema_preserving\x18\x07 \x01(\x08\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xfd\n\n\x04Spec\x12\'\n\x08identity\x18\x01 \x01(\x0b\x32\x13.Transform.IdentityH\x00\x12\'\n\x08variable\x18\x02 \x01(\x0b\x32\x13.Transform.VariableH\x00\x12\'\n\x08\x63omposed\x18\x03 \x01(\x0b\x32\x13.Transform.ComposedH\x00\x12%\n\x07project\x18\x04 \x01(\x0b\x32\x12.Transform.ProjectH\x00\x12#\n\x06\x66ilter\x18\x05 \x01(\x0b\x32\x11.Transform.FilterH\x00\x12%\n\x07shuffle\x18\x06 \x01(\x0b\x32\x12.Transform.ShuffleH\x00\x12\x1f\n\x04join\x18\x07 \x01(\x0b\x32\x0f.Transform.JoinH\x00\x12\x1f\n\x04\x63\x61st\x18\x08 \x01(\x0b\x32\x0f.Transform.CastH\x00\x12#\n\x06sample\x18\t \x01(\x0b\x32\x11.Transform.SampleH\x00\x12\x30\n\ruser_settings\x18\n \x01(\x0b\x32\x17.Transform.UserSettingsH\x00\x12-\n\x0fprotect_dataset\x18\x0b \x01(\x0b\x32\x12.Transform.ProtectH\x00\x12\'\n\x08\x65xternal\x18\x0c \x01(\x0b\x32\x13.Transform.ExternalH\x00\x12)\n\tsynthetic\x18\r \x01(\x0b\x32\x14.Transform.SyntheticH\x00\x12)\n\ttranscode\x18\x0e \x01(\x0b\x32\x14.Transform.TranscodeH\x00\x12\x38\n\x11inverse_transcode\x18\x0f \x01(\x0b\x32\x1b.Transform.InverseTranscodeH\x00\x12&\n\x08get_item\x18\x10 \x01(\x0b\x32\x12.Transform.GetItemH\x00\x12\x34\n\x0fprotected_paths\x18\x11 \x01(\x0b\x32\x19.Transform.ProtectedPathsH\x00\x12\x43\n\x17\x61utomatic_user_settings\x18\x12 \x01(\x0b\x32 .Transform.AutomaticUserSettingsH\x00\x12.\n\x0cpublic_paths\x18\x13 \x01(\x0b\x32\x16.Transform.PublicPathsH\x00\x12\x30\n\rassign_budget\x18\x14 \x01(\x0b\x32\x17.Transform.AssignBudgetH\x00\x12\x36\n\x10\x61utomatic_budget\x18\x15 \x01(\x0b\x32\x1a.Transform.AutomaticBudgetH\x00\x12\x37\n\x10\x61ttribute_budget\x18\x16 \x01(\x0b\x32\x1b.Transform.AttributesBudgetH\x00\x12(\n\tsd_budget\x18\x17 \x01(\x0b\x32\x13.Transform.SDBudgetH\x00\x12,\n\x0b\x64\x65rive_seed\x18\x18 \x01(\x0b\x32\x15.Transform.DeriveSeedH\x00\x12+\n\x0bgroup_by_pe\x18\x19 \x01(\x0b\x32\x14.Transform.GroupByPEH\x00\x12\x34\n\x0fsampling_ratios\x18\x1a \x01(\x0b\x32\x19.Transform.SamplingRatiosH\x00\x12*\n\nselect_sql\x18\x1b \x01(\x0b\x32\x14.Transform.SelectSqlH\x00\x12%\n\x07\x65xtract\x18\x1c \x01(\x0b\x32\x12.Transform.ExtractH\x00\x12\x38\n\x11relationship_spec\x18\x1d \x01(\x0b\x32\x1b.Transform.RelationshipSpecH\x00\x12@\n\x15\x64ifferentiated_sample\x18\x1e \x01(\x0b\x32\x1f.Transform.DifferentiatedSampleH\x00\x42\x06\n\x04spec\x1a\xa1\x06\n\x08\x45xternal\x12\x11\n\targuments\x18\x01 \x01(\x0c\x12\x17\n\x0fnamed_arguments\x18\x02 \x01(\x0c\x12\x37\n\rop_identifier\x18\x03 \x01(\x0b\x32 .Transform.External.OpIdentifier\x1a\xcb\x03\n\x0cOpIdentifier\x12&\n\x03std\x18\x01 \x01(\x0b\x32\x17.Transform.External.StdH\x00\x12,\n\x06pandas\x18\x02 \x01(\x0b\x32\x1a.Transform.External.PandasH\x00\x12*\n\x05numpy\x18\x03 \x01(\x0b\x32\x19.Transform.External.NumpyH\x00\x12\x34\n\ntensorflow\x18\x04 \x01(\x0b\x32\x1e.Transform.External.TensorflowH\x00\x12.\n\x07sklearn\x18\x05 \x01(\x0b\x32\x1b.Transform.External.SklearnH\x00\x12?\n\x10pandas_profiling\x18\x06 \x01(\x0b\x32#.Transform.External.PandasProfilingH\x00\x12.\n\x07xgboost\x18\x07 \x01(\x0b\x32\x1b.Transform.External.XGBoostH\x00\x12*\n\x05skopt\x18\x08 \x01(\x0b\x32\x19.Transform.External.SkoptH\x00\x12\x30\n\x08imblearn\x18\t \x01(\x0b\x32\x1c.Transform.External.ImblearnH\x00\x42\x04\n\x02op\x1a\x13\n\x03Std\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x16\n\x06Pandas\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Numpy\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1a\n\nTensorflow\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x17\n\x07Sklearn\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1f\n\x0fPandasProfiling\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x17\n\x07XGBoost\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Skopt\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x18\n\x08Imblearn\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\n\n\x08Identity\x1a*\n\x08Variable\x12\x10\n\x08position\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x1a\xa9\x01\n\x08\x43omposed\x12\x11\n\ttransform\x18\x01 \x01(\t\x12\x11\n\targuments\x18\x02 \x03(\t\x12@\n\x0fnamed_arguments\x18\x03 \x03(\x0b\x32\'.Transform.Composed.NamedArgumentsEntry\x1a\x35\n\x13NamedArgumentsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x34\n\x07Project\x12)\n\nprojection\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a/\n\x06\x46ilter\x12%\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a\t\n\x07Shuffle\x1a)\n\x04Join\x12!\n\x02on\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a+\n\x04\x43\x61st\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a\x61\n\x06Sample\x12\x12\n\x08\x66raction\x18\x01 \x01(\x01H\x00\x12\x0e\n\x04size\x18\x02 \x01(\x03H\x00\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.ScalarB\x0c\n\nproportion\x1av\n\x0fSchemaInference\x12:\n\x0b\x63\x61st_policy\x18\x01 \x01(\x0e\x32%.Transform.SchemaInference.CastPolicy\"\'\n\nCastPolicy\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bMOST_LIKELY\x10\x01\x1a\x16\n\x07GroupBy\x12\x0b\n\x03key\x18\x01 \x01(\t\x1a\x0b\n\tSynthetic\x1a\x0e\n\x0cUserSettings\x1a/\n\x15\x41utomaticUserSettings\x12\x16\n\x0emax_categories\x18\x01 \x01(\x03\x1a\t\n\x07Protect\x1a\x0b\n\tTranscode\x1a\x12\n\x10InverseTranscode\x1ao\n\x14\x44ifferentiatedSample\x12\x12\n\x08\x66raction\x18\x01 \x01(\x01H\x00\x12\x0e\n\x04size\x18\x02 \x01(\x03H\x00\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.ScalarB\x0c\n\nproportion\x1a\x10\n\x0eProtectedPaths\x1a\r\n\x0bPublicPaths\x1a.\n\x07GetItem\x12#\n\x04path\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Path\x1a\x0e\n\x0c\x41ssignBudget\x1a\x11\n\x0f\x41utomaticBudget\x1a\x12\n\x10\x41ttributesBudget\x1a\n\n\x08SDBudget\x1a$\n\nDeriveSeed\x12\x16\n\x0erandom_integer\x18\x01 \x01(\x03\x1a\x0b\n\tGroupByPE\x1a\x10\n\x0eSamplingRatios\x1a\x12\n\x10RelationshipSpec\x1a\xaf\x03\n\tSelectSql\x12\x0f\n\x05query\x18\x01 \x01(\tH\x00\x12>\n\x0f\x61liased_queries\x18\x02 \x01(\x0b\x32#.Transform.SelectSql.AliasedQueriesH\x00\x12\x34\n\x0bsql_dialect\x18\x03 \x01(\x0e\x32\x1f.Transform.SelectSql.SQLDialect\x1aJ\n\x0e\x41liasedQueries\x12\x38\n\raliased_query\x18\x01 \x03(\x0b\x32!.Transform.SelectSql.AliasedQuery\x1a\x42\n\x0c\x41liasedQuery\x12#\n\x04path\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Path\x12\r\n\x05query\x18\x02 \x01(\t\"\x80\x01\n\nSQLDialect\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08POSTGRES\x10\x01\x12\x0e\n\nSQL_SERVER\x10\x02\x12\n\n\x06MY_SQL\x10\x03\x12\x0b\n\x07SQLLITE\x10\x04\x12\n\n\x06ORACLE\x10\x05\x12\r\n\tBIG_QUERY\x10\x06\x12\x0c\n\x08REDSHIFT\x10\x07\x12\x08\n\x04HIVE\x10\x08\x42\x08\n\x06select\x1a\x17\n\x07\x45xtract\x12\x0c\n\x04size\x18\x01 \x01(\x05\x62\x06proto3'
+  serialized_pb=b'\n(sarus_data_spec/protobuf/transform.proto\x1a#sarus_data_spec/protobuf/type.proto\x1a#sarus_data_spec/protobuf/path.proto\x1a%sarus_data_spec/protobuf/scalar.proto\"\x9f \n\tTransform\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0b\n\x03\x64oc\x18\x03 \x01(\t\x12\x1d\n\x04spec\x18\x04 \x01(\x0b\x32\x0f.Transform.Spec\x12.\n\nproperties\x18\x05 \x03(\x0b\x32\x1a.Transform.PropertiesEntry\x12\x12\n\ninversible\x18\x06 \x01(\x08\x12\x19\n\x11schema_preserving\x18\x07 \x01(\x08\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xba\x0b\n\x04Spec\x12\'\n\x08identity\x18\x01 \x01(\x0b\x32\x13.Transform.IdentityH\x00\x12\'\n\x08variable\x18\x02 \x01(\x0b\x32\x13.Transform.VariableH\x00\x12\'\n\x08\x63omposed\x18\x03 \x01(\x0b\x32\x13.Transform.ComposedH\x00\x12%\n\x07project\x18\x04 \x01(\x0b\x32\x12.Transform.ProjectH\x00\x12#\n\x06\x66ilter\x18\x05 \x01(\x0b\x32\x11.Transform.FilterH\x00\x12%\n\x07shuffle\x18\x06 \x01(\x0b\x32\x12.Transform.ShuffleH\x00\x12\x1f\n\x04join\x18\x07 \x01(\x0b\x32\x0f.Transform.JoinH\x00\x12\x1f\n\x04\x63\x61st\x18\x08 \x01(\x0b\x32\x0f.Transform.CastH\x00\x12#\n\x06sample\x18\t \x01(\x0b\x32\x11.Transform.SampleH\x00\x12\x30\n\ruser_settings\x18\n \x01(\x0b\x32\x17.Transform.UserSettingsH\x00\x12-\n\x0fprotect_dataset\x18\x0b \x01(\x0b\x32\x12.Transform.ProtectH\x00\x12\'\n\x08\x65xternal\x18\x0c \x01(\x0b\x32\x13.Transform.ExternalH\x00\x12)\n\tsynthetic\x18\r \x01(\x0b\x32\x14.Transform.SyntheticH\x00\x12)\n\ttranscode\x18\x0e \x01(\x0b\x32\x14.Transform.TranscodeH\x00\x12\x38\n\x11inverse_transcode\x18\x0f \x01(\x0b\x32\x1b.Transform.InverseTranscodeH\x00\x12&\n\x08get_item\x18\x10 \x01(\x0b\x32\x12.Transform.GetItemH\x00\x12\x34\n\x0fprotected_paths\x18\x11 \x01(\x0b\x32\x19.Transform.ProtectedPathsH\x00\x12\x43\n\x17\x61utomatic_user_settings\x18\x12 \x01(\x0b\x32 .Transform.AutomaticUserSettingsH\x00\x12.\n\x0cpublic_paths\x18\x13 \x01(\x0b\x32\x16.Transform.PublicPathsH\x00\x12\x30\n\rassign_budget\x18\x14 \x01(\x0b\x32\x17.Transform.AssignBudgetH\x00\x12\x36\n\x10\x61utomatic_budget\x18\x15 \x01(\x0b\x32\x1a.Transform.AutomaticBudgetH\x00\x12\x37\n\x10\x61ttribute_budget\x18\x16 \x01(\x0b\x32\x1b.Transform.AttributesBudgetH\x00\x12(\n\tsd_budget\x18\x17 \x01(\x0b\x32\x13.Transform.SDBudgetH\x00\x12,\n\x0b\x64\x65rive_seed\x18\x18 \x01(\x0b\x32\x15.Transform.DeriveSeedH\x00\x12+\n\x0bgroup_by_pe\x18\x19 \x01(\x0b\x32\x14.Transform.GroupByPEH\x00\x12\x34\n\x0fsampling_ratios\x18\x1a \x01(\x0b\x32\x19.Transform.SamplingRatiosH\x00\x12*\n\nselect_sql\x18\x1b \x01(\x0b\x32\x14.Transform.SelectSqlH\x00\x12%\n\x07\x65xtract\x18\x1c \x01(\x0b\x32\x12.Transform.ExtractH\x00\x12\x38\n\x11relationship_spec\x18\x1d \x01(\x0b\x32\x1b.Transform.RelationshipSpecH\x00\x12@\n\x15\x64ifferentiated_sample\x18\x1e \x01(\x0b\x32\x1f.Transform.DifferentiatedSampleH\x00\x12;\n\x13validated_user_type\x18\x1f \x01(\x0b\x32\x1c.Transform.ValidatedUserTypeH\x00\x42\x06\n\x04spec\x1a\xa1\x06\n\x08\x45xternal\x12\x11\n\targuments\x18\x01 \x01(\x0c\x12\x17\n\x0fnamed_arguments\x18\x02 \x01(\x0c\x12\x37\n\rop_identifier\x18\x03 \x01(\x0b\x32 .Transform.External.OpIdentifier\x1a\xcb\x03\n\x0cOpIdentifier\x12&\n\x03std\x18\x01 \x01(\x0b\x32\x17.Transform.External.StdH\x00\x12,\n\x06pandas\x18\x02 \x01(\x0b\x32\x1a.Transform.External.PandasH\x00\x12*\n\x05numpy\x18\x03 \x01(\x0b\x32\x19.Transform.External.NumpyH\x00\x12\x34\n\ntensorflow\x18\x04 \x01(\x0b\x32\x1e.Transform.External.TensorflowH\x00\x12.\n\x07sklearn\x18\x05 \x01(\x0b\x32\x1b.Transform.External.SklearnH\x00\x12?\n\x10pandas_profiling\x18\x06 \x01(\x0b\x32#.Transform.External.PandasProfilingH\x00\x12.\n\x07xgboost\x18\x07 \x01(\x0b\x32\x1b.Transform.External.XGBoostH\x00\x12*\n\x05skopt\x18\x08 \x01(\x0b\x32\x19.Transform.External.SkoptH\x00\x12\x30\n\x08imblearn\x18\t \x01(\x0b\x32\x1c.Transform.External.ImblearnH\x00\x42\x04\n\x02op\x1a\x13\n\x03Std\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x16\n\x06Pandas\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Numpy\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1a\n\nTensorflow\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x17\n\x07Sklearn\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1f\n\x0fPandasProfiling\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x17\n\x07XGBoost\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Skopt\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x18\n\x08Imblearn\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\n\n\x08Identity\x1a*\n\x08Variable\x12\x10\n\x08position\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x1a\xa9\x01\n\x08\x43omposed\x12\x11\n\ttransform\x18\x01 \x01(\t\x12\x11\n\targuments\x18\x02 \x03(\t\x12@\n\x0fnamed_arguments\x18\x03 \x03(\x0b\x32\'.Transform.Composed.NamedArgumentsEntry\x1a\x35\n\x13NamedArgumentsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x34\n\x07Project\x12)\n\nprojection\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a/\n\x06\x46ilter\x12%\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a\t\n\x07Shuffle\x1a)\n\x04Join\x12!\n\x02on\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a+\n\x04\x43\x61st\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a\x61\n\x06Sample\x12\x12\n\x08\x66raction\x18\x01 \x01(\x01H\x00\x12\x0e\n\x04size\x18\x02 \x01(\x03H\x00\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.ScalarB\x0c\n\nproportion\x1av\n\x0fSchemaInference\x12:\n\x0b\x63\x61st_policy\x18\x01 \x01(\x0e\x32%.Transform.SchemaInference.CastPolicy\"\'\n\nCastPolicy\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bMOST_LIKELY\x10\x01\x1a\x16\n\x07GroupBy\x12\x0b\n\x03key\x18\x01 \x01(\t\x1a\x0b\n\tSynthetic\x1a\x0e\n\x0cUserSettings\x1a/\n\x15\x41utomaticUserSettings\x12\x16\n\x0emax_categories\x18\x01 \x01(\x03\x1a\t\n\x07Protect\x1a\x0b\n\tTranscode\x1a\x12\n\x10InverseTranscode\x1ao\n\x14\x44ifferentiatedSample\x12\x12\n\x08\x66raction\x18\x01 \x01(\x01H\x00\x12\x0e\n\x04size\x18\x02 \x01(\x03H\x00\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.ScalarB\x0c\n\nproportion\x1a\x10\n\x0eProtectedPaths\x1a\r\n\x0bPublicPaths\x1a.\n\x07GetItem\x12#\n\x04path\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Path\x1a\x0e\n\x0c\x41ssignBudget\x1a\x11\n\x0f\x41utomaticBudget\x1a\x12\n\x10\x41ttributesBudget\x1a\n\n\x08SDBudget\x1a$\n\nDeriveSeed\x12\x16\n\x0erandom_integer\x18\x01 \x01(\x03\x1a\x0b\n\tGroupByPE\x1a\x10\n\x0eSamplingRatios\x1a\x12\n\x10RelationshipSpec\x1a\xaf\x03\n\tSelectSql\x12\x0f\n\x05query\x18\x01 \x01(\tH\x00\x12>\n\x0f\x61liased_queries\x18\x02 \x01(\x0b\x32#.Transform.SelectSql.AliasedQueriesH\x00\x12\x34\n\x0bsql_dialect\x18\x03 \x01(\x0e\x32\x1f.Transform.SelectSql.SQLDialect\x1aJ\n\x0e\x41liasedQueries\x12\x38\n\raliased_query\x18\x01 \x03(\x0b\x32!.Transform.SelectSql.AliasedQuery\x1a\x42\n\x0c\x41liasedQuery\x12#\n\x04path\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Path\x12\r\n\x05query\x18\x02 \x01(\t\"\x80\x01\n\nSQLDialect\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08POSTGRES\x10\x01\x12\x0e\n\nSQL_SERVER\x10\x02\x12\n\n\x06MY_SQL\x10\x03\x12\x0b\n\x07SQLLITE\x10\x04\x12\n\n\x06ORACLE\x10\x05\x12\r\n\tBIG_QUERY\x10\x06\x12\x0c\n\x08REDSHIFT\x10\x07\x12\x08\n\x04HIVE\x10\x08\x42\x08\n\x06select\x1a\x17\n\x07\x45xtract\x12\x0c\n\x04size\x18\x01 \x01(\x05\x1a\x13\n\x11ValidatedUserTypeb\x06proto3'
   ,
   dependencies=[sarus__data__spec_dot_protobuf_dot_type__pb2.DESCRIPTOR,sarus__data__spec_dot_protobuf_dot_path__pb2.DESCRIPTOR,sarus__data__spec_dot_protobuf_dot_scalar__pb2.DESCRIPTOR,])
 
 
 
 _TRANSFORM_SCHEMAINFERENCE_CASTPOLICY = _descriptor.EnumDescriptor(
   name='CastPolicy',
@@ -44,16 +44,16 @@
       name='MOST_LIKELY', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3209,
-  serialized_end=3248,
+  serialized_start=3270,
+  serialized_end=3309,
 )
 _sym_db.RegisterEnumDescriptor(_TRANSFORM_SCHEMAINFERENCE_CASTPOLICY)
 
 _TRANSFORM_SELECTSQL_SQLDIALECT = _descriptor.EnumDescriptor(
   name='SQLDialect',
   full_name='Transform.SelectSql.SQLDialect',
   filename=None,
@@ -104,16 +104,16 @@
       name='HIVE', index=8, number=8,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=4040,
-  serialized_end=4168,
+  serialized_start=4101,
+  serialized_end=4229,
 )
 _sym_db.RegisterEnumDescriptor(_TRANSFORM_SELECTSQL_SQLDIALECT)
 
 
 _TRANSFORM_PROPERTIESENTRY = _descriptor.Descriptor(
   name='PropertiesEntry',
   full_name='Transform.PropertiesEntry',
@@ -366,14 +366,21 @@
     _descriptor.FieldDescriptor(
       name='differentiated_sample', full_name='Transform.Spec.differentiated_sample', index=29,
       number=30, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='validated_user_type', full_name='Transform.Spec.validated_user_type', index=30,
+      number=31, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
@@ -384,15 +391,15 @@
     _descriptor.OneofDescriptor(
       name='spec', full_name='Transform.Spec.spec',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
   serialized_start=390,
-  serialized_end=1795,
+  serialized_end=1856,
 )
 
 _TRANSFORM_EXTERNAL_OPIDENTIFIER = _descriptor.Descriptor(
   name='OpIdentifier',
   full_name='Transform.External.OpIdentifier',
   filename=None,
   file=DESCRIPTOR,
@@ -475,16 +482,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='op', full_name='Transform.External.OpIdentifier.op',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=1912,
-  serialized_end=2371,
+  serialized_start=1973,
+  serialized_end=2432,
 )
 
 _TRANSFORM_EXTERNAL_STD = _descriptor.Descriptor(
   name='Std',
   full_name='Transform.External.Std',
   filename=None,
   file=DESCRIPTOR,
@@ -506,16 +513,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2373,
-  serialized_end=2392,
+  serialized_start=2434,
+  serialized_end=2453,
 )
 
 _TRANSFORM_EXTERNAL_PANDAS = _descriptor.Descriptor(
   name='Pandas',
   full_name='Transform.External.Pandas',
   filename=None,
   file=DESCRIPTOR,
@@ -537,16 +544,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2394,
-  serialized_end=2416,
+  serialized_start=2455,
+  serialized_end=2477,
 )
 
 _TRANSFORM_EXTERNAL_NUMPY = _descriptor.Descriptor(
   name='Numpy',
   full_name='Transform.External.Numpy',
   filename=None,
   file=DESCRIPTOR,
@@ -568,16 +575,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2418,
-  serialized_end=2439,
+  serialized_start=2479,
+  serialized_end=2500,
 )
 
 _TRANSFORM_EXTERNAL_TENSORFLOW = _descriptor.Descriptor(
   name='Tensorflow',
   full_name='Transform.External.Tensorflow',
   filename=None,
   file=DESCRIPTOR,
@@ -599,16 +606,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2441,
-  serialized_end=2467,
+  serialized_start=2502,
+  serialized_end=2528,
 )
 
 _TRANSFORM_EXTERNAL_SKLEARN = _descriptor.Descriptor(
   name='Sklearn',
   full_name='Transform.External.Sklearn',
   filename=None,
   file=DESCRIPTOR,
@@ -630,16 +637,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2469,
-  serialized_end=2492,
+  serialized_start=2530,
+  serialized_end=2553,
 )
 
 _TRANSFORM_EXTERNAL_PANDASPROFILING = _descriptor.Descriptor(
   name='PandasProfiling',
   full_name='Transform.External.PandasProfiling',
   filename=None,
   file=DESCRIPTOR,
@@ -661,16 +668,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2494,
-  serialized_end=2525,
+  serialized_start=2555,
+  serialized_end=2586,
 )
 
 _TRANSFORM_EXTERNAL_XGBOOST = _descriptor.Descriptor(
   name='XGBoost',
   full_name='Transform.External.XGBoost',
   filename=None,
   file=DESCRIPTOR,
@@ -692,16 +699,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2527,
-  serialized_end=2550,
+  serialized_start=2588,
+  serialized_end=2611,
 )
 
 _TRANSFORM_EXTERNAL_SKOPT = _descriptor.Descriptor(
   name='Skopt',
   full_name='Transform.External.Skopt',
   filename=None,
   file=DESCRIPTOR,
@@ -723,16 +730,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2552,
-  serialized_end=2573,
+  serialized_start=2613,
+  serialized_end=2634,
 )
 
 _TRANSFORM_EXTERNAL_IMBLEARN = _descriptor.Descriptor(
   name='Imblearn',
   full_name='Transform.External.Imblearn',
   filename=None,
   file=DESCRIPTOR,
@@ -754,16 +761,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2575,
-  serialized_end=2599,
+  serialized_start=2636,
+  serialized_end=2660,
 )
 
 _TRANSFORM_EXTERNAL = _descriptor.Descriptor(
   name='External',
   full_name='Transform.External',
   filename=None,
   file=DESCRIPTOR,
@@ -799,16 +806,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1798,
-  serialized_end=2599,
+  serialized_start=1859,
+  serialized_end=2660,
 )
 
 _TRANSFORM_IDENTITY = _descriptor.Descriptor(
   name='Identity',
   full_name='Transform.Identity',
   filename=None,
   file=DESCRIPTOR,
@@ -823,16 +830,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2601,
-  serialized_end=2611,
+  serialized_start=2662,
+  serialized_end=2672,
 )
 
 _TRANSFORM_VARIABLE = _descriptor.Descriptor(
   name='Variable',
   full_name='Transform.Variable',
   filename=None,
   file=DESCRIPTOR,
@@ -861,16 +868,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2613,
-  serialized_end=2655,
+  serialized_start=2674,
+  serialized_end=2716,
 )
 
 _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY = _descriptor.Descriptor(
   name='NamedArgumentsEntry',
   full_name='Transform.Composed.NamedArgumentsEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -899,16 +906,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2774,
-  serialized_end=2827,
+  serialized_start=2835,
+  serialized_end=2888,
 )
 
 _TRANSFORM_COMPOSED = _descriptor.Descriptor(
   name='Composed',
   full_name='Transform.Composed',
   filename=None,
   file=DESCRIPTOR,
@@ -944,16 +951,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2658,
-  serialized_end=2827,
+  serialized_start=2719,
+  serialized_end=2888,
 )
 
 _TRANSFORM_PROJECT = _descriptor.Descriptor(
   name='Project',
   full_name='Transform.Project',
   filename=None,
   file=DESCRIPTOR,
@@ -975,16 +982,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2829,
-  serialized_end=2881,
+  serialized_start=2890,
+  serialized_end=2942,
 )
 
 _TRANSFORM_FILTER = _descriptor.Descriptor(
   name='Filter',
   full_name='Transform.Filter',
   filename=None,
   file=DESCRIPTOR,
@@ -1006,16 +1013,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2883,
-  serialized_end=2930,
+  serialized_start=2944,
+  serialized_end=2991,
 )
 
 _TRANSFORM_SHUFFLE = _descriptor.Descriptor(
   name='Shuffle',
   full_name='Transform.Shuffle',
   filename=None,
   file=DESCRIPTOR,
@@ -1030,16 +1037,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2932,
-  serialized_end=2941,
+  serialized_start=2993,
+  serialized_end=3002,
 )
 
 _TRANSFORM_JOIN = _descriptor.Descriptor(
   name='Join',
   full_name='Transform.Join',
   filename=None,
   file=DESCRIPTOR,
@@ -1061,16 +1068,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2943,
-  serialized_end=2984,
+  serialized_start=3004,
+  serialized_end=3045,
 )
 
 _TRANSFORM_CAST = _descriptor.Descriptor(
   name='Cast',
   full_name='Transform.Cast',
   filename=None,
   file=DESCRIPTOR,
@@ -1092,16 +1099,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2986,
-  serialized_end=3029,
+  serialized_start=3047,
+  serialized_end=3090,
 )
 
 _TRANSFORM_SAMPLE = _descriptor.Descriptor(
   name='Sample',
   full_name='Transform.Sample',
   filename=None,
   file=DESCRIPTOR,
@@ -1142,16 +1149,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='proportion', full_name='Transform.Sample.proportion',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=3031,
-  serialized_end=3128,
+  serialized_start=3092,
+  serialized_end=3189,
 )
 
 _TRANSFORM_SCHEMAINFERENCE = _descriptor.Descriptor(
   name='SchemaInference',
   full_name='Transform.SchemaInference',
   filename=None,
   file=DESCRIPTOR,
@@ -1174,16 +1181,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3130,
-  serialized_end=3248,
+  serialized_start=3191,
+  serialized_end=3309,
 )
 
 _TRANSFORM_GROUPBY = _descriptor.Descriptor(
   name='GroupBy',
   full_name='Transform.GroupBy',
   filename=None,
   file=DESCRIPTOR,
@@ -1205,16 +1212,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3250,
-  serialized_end=3272,
+  serialized_start=3311,
+  serialized_end=3333,
 )
 
 _TRANSFORM_SYNTHETIC = _descriptor.Descriptor(
   name='Synthetic',
   full_name='Transform.Synthetic',
   filename=None,
   file=DESCRIPTOR,
@@ -1229,16 +1236,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3274,
-  serialized_end=3285,
+  serialized_start=3335,
+  serialized_end=3346,
 )
 
 _TRANSFORM_USERSETTINGS = _descriptor.Descriptor(
   name='UserSettings',
   full_name='Transform.UserSettings',
   filename=None,
   file=DESCRIPTOR,
@@ -1253,16 +1260,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3287,
-  serialized_end=3301,
+  serialized_start=3348,
+  serialized_end=3362,
 )
 
 _TRANSFORM_AUTOMATICUSERSETTINGS = _descriptor.Descriptor(
   name='AutomaticUserSettings',
   full_name='Transform.AutomaticUserSettings',
   filename=None,
   file=DESCRIPTOR,
@@ -1284,16 +1291,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3303,
-  serialized_end=3350,
+  serialized_start=3364,
+  serialized_end=3411,
 )
 
 _TRANSFORM_PROTECT = _descriptor.Descriptor(
   name='Protect',
   full_name='Transform.Protect',
   filename=None,
   file=DESCRIPTOR,
@@ -1308,16 +1315,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3352,
-  serialized_end=3361,
+  serialized_start=3413,
+  serialized_end=3422,
 )
 
 _TRANSFORM_TRANSCODE = _descriptor.Descriptor(
   name='Transcode',
   full_name='Transform.Transcode',
   filename=None,
   file=DESCRIPTOR,
@@ -1332,16 +1339,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3363,
-  serialized_end=3374,
+  serialized_start=3424,
+  serialized_end=3435,
 )
 
 _TRANSFORM_INVERSETRANSCODE = _descriptor.Descriptor(
   name='InverseTranscode',
   full_name='Transform.InverseTranscode',
   filename=None,
   file=DESCRIPTOR,
@@ -1356,16 +1363,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3376,
-  serialized_end=3394,
+  serialized_start=3437,
+  serialized_end=3455,
 )
 
 _TRANSFORM_DIFFERENTIATEDSAMPLE = _descriptor.Descriptor(
   name='DifferentiatedSample',
   full_name='Transform.DifferentiatedSample',
   filename=None,
   file=DESCRIPTOR,
@@ -1406,16 +1413,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='proportion', full_name='Transform.DifferentiatedSample.proportion',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=3396,
-  serialized_end=3507,
+  serialized_start=3457,
+  serialized_end=3568,
 )
 
 _TRANSFORM_PROTECTEDPATHS = _descriptor.Descriptor(
   name='ProtectedPaths',
   full_name='Transform.ProtectedPaths',
   filename=None,
   file=DESCRIPTOR,
@@ -1430,16 +1437,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3509,
-  serialized_end=3525,
+  serialized_start=3570,
+  serialized_end=3586,
 )
 
 _TRANSFORM_PUBLICPATHS = _descriptor.Descriptor(
   name='PublicPaths',
   full_name='Transform.PublicPaths',
   filename=None,
   file=DESCRIPTOR,
@@ -1454,16 +1461,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3527,
-  serialized_end=3540,
+  serialized_start=3588,
+  serialized_end=3601,
 )
 
 _TRANSFORM_GETITEM = _descriptor.Descriptor(
   name='GetItem',
   full_name='Transform.GetItem',
   filename=None,
   file=DESCRIPTOR,
@@ -1485,16 +1492,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3542,
-  serialized_end=3588,
+  serialized_start=3603,
+  serialized_end=3649,
 )
 
 _TRANSFORM_ASSIGNBUDGET = _descriptor.Descriptor(
   name='AssignBudget',
   full_name='Transform.AssignBudget',
   filename=None,
   file=DESCRIPTOR,
@@ -1509,16 +1516,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3590,
-  serialized_end=3604,
+  serialized_start=3651,
+  serialized_end=3665,
 )
 
 _TRANSFORM_AUTOMATICBUDGET = _descriptor.Descriptor(
   name='AutomaticBudget',
   full_name='Transform.AutomaticBudget',
   filename=None,
   file=DESCRIPTOR,
@@ -1533,16 +1540,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3606,
-  serialized_end=3623,
+  serialized_start=3667,
+  serialized_end=3684,
 )
 
 _TRANSFORM_ATTRIBUTESBUDGET = _descriptor.Descriptor(
   name='AttributesBudget',
   full_name='Transform.AttributesBudget',
   filename=None,
   file=DESCRIPTOR,
@@ -1557,16 +1564,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3625,
-  serialized_end=3643,
+  serialized_start=3686,
+  serialized_end=3704,
 )
 
 _TRANSFORM_SDBUDGET = _descriptor.Descriptor(
   name='SDBudget',
   full_name='Transform.SDBudget',
   filename=None,
   file=DESCRIPTOR,
@@ -1581,16 +1588,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3645,
-  serialized_end=3655,
+  serialized_start=3706,
+  serialized_end=3716,
 )
 
 _TRANSFORM_DERIVESEED = _descriptor.Descriptor(
   name='DeriveSeed',
   full_name='Transform.DeriveSeed',
   filename=None,
   file=DESCRIPTOR,
@@ -1612,16 +1619,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3657,
-  serialized_end=3693,
+  serialized_start=3718,
+  serialized_end=3754,
 )
 
 _TRANSFORM_GROUPBYPE = _descriptor.Descriptor(
   name='GroupByPE',
   full_name='Transform.GroupByPE',
   filename=None,
   file=DESCRIPTOR,
@@ -1636,16 +1643,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3695,
-  serialized_end=3706,
+  serialized_start=3756,
+  serialized_end=3767,
 )
 
 _TRANSFORM_SAMPLINGRATIOS = _descriptor.Descriptor(
   name='SamplingRatios',
   full_name='Transform.SamplingRatios',
   filename=None,
   file=DESCRIPTOR,
@@ -1660,16 +1667,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3708,
-  serialized_end=3724,
+  serialized_start=3769,
+  serialized_end=3785,
 )
 
 _TRANSFORM_RELATIONSHIPSPEC = _descriptor.Descriptor(
   name='RelationshipSpec',
   full_name='Transform.RelationshipSpec',
   filename=None,
   file=DESCRIPTOR,
@@ -1684,16 +1691,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3726,
-  serialized_end=3744,
+  serialized_start=3787,
+  serialized_end=3805,
 )
 
 _TRANSFORM_SELECTSQL_ALIASEDQUERIES = _descriptor.Descriptor(
   name='AliasedQueries',
   full_name='Transform.SelectSql.AliasedQueries',
   filename=None,
   file=DESCRIPTOR,
@@ -1715,16 +1722,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3895,
-  serialized_end=3969,
+  serialized_start=3956,
+  serialized_end=4030,
 )
 
 _TRANSFORM_SELECTSQL_ALIASEDQUERY = _descriptor.Descriptor(
   name='AliasedQuery',
   full_name='Transform.SelectSql.AliasedQuery',
   filename=None,
   file=DESCRIPTOR,
@@ -1753,16 +1760,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3971,
-  serialized_end=4037,
+  serialized_start=4032,
+  serialized_end=4098,
 )
 
 _TRANSFORM_SELECTSQL = _descriptor.Descriptor(
   name='SelectSql',
   full_name='Transform.SelectSql',
   filename=None,
   file=DESCRIPTOR,
@@ -1804,16 +1811,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='select', full_name='Transform.SelectSql.select',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=3747,
-  serialized_end=4178,
+  serialized_start=3808,
+  serialized_end=4239,
 )
 
 _TRANSFORM_EXTRACT = _descriptor.Descriptor(
   name='Extract',
   full_name='Transform.Extract',
   filename=None,
   file=DESCRIPTOR,
@@ -1835,16 +1842,40 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4180,
-  serialized_end=4203,
+  serialized_start=4241,
+  serialized_end=4264,
+)
+
+_TRANSFORM_VALIDATEDUSERTYPE = _descriptor.Descriptor(
+  name='ValidatedUserType',
+  full_name='Transform.ValidatedUserType',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=4266,
+  serialized_end=4285,
 )
 
 _TRANSFORM = _descriptor.Descriptor(
   name='Transform',
   full_name='Transform',
   filename=None,
   file=DESCRIPTOR,
@@ -1899,25 +1930,25 @@
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
-  nested_types=[_TRANSFORM_PROPERTIESENTRY, _TRANSFORM_SPEC, _TRANSFORM_EXTERNAL, _TRANSFORM_IDENTITY, _TRANSFORM_VARIABLE, _TRANSFORM_COMPOSED, _TRANSFORM_PROJECT, _TRANSFORM_FILTER, _TRANSFORM_SHUFFLE, _TRANSFORM_JOIN, _TRANSFORM_CAST, _TRANSFORM_SAMPLE, _TRANSFORM_SCHEMAINFERENCE, _TRANSFORM_GROUPBY, _TRANSFORM_SYNTHETIC, _TRANSFORM_USERSETTINGS, _TRANSFORM_AUTOMATICUSERSETTINGS, _TRANSFORM_PROTECT, _TRANSFORM_TRANSCODE, _TRANSFORM_INVERSETRANSCODE, _TRANSFORM_DIFFERENTIATEDSAMPLE, _TRANSFORM_PROTECTEDPATHS, _TRANSFORM_PUBLICPATHS, _TRANSFORM_GETITEM, _TRANSFORM_ASSIGNBUDGET, _TRANSFORM_AUTOMATICBUDGET, _TRANSFORM_ATTRIBUTESBUDGET, _TRANSFORM_SDBUDGET, _TRANSFORM_DERIVESEED, _TRANSFORM_GROUPBYPE, _TRANSFORM_SAMPLINGRATIOS, _TRANSFORM_RELATIONSHIPSPEC, _TRANSFORM_SELECTSQL, _TRANSFORM_EXTRACT, ],
+  nested_types=[_TRANSFORM_PROPERTIESENTRY, _TRANSFORM_SPEC, _TRANSFORM_EXTERNAL, _TRANSFORM_IDENTITY, _TRANSFORM_VARIABLE, _TRANSFORM_COMPOSED, _TRANSFORM_PROJECT, _TRANSFORM_FILTER, _TRANSFORM_SHUFFLE, _TRANSFORM_JOIN, _TRANSFORM_CAST, _TRANSFORM_SAMPLE, _TRANSFORM_SCHEMAINFERENCE, _TRANSFORM_GROUPBY, _TRANSFORM_SYNTHETIC, _TRANSFORM_USERSETTINGS, _TRANSFORM_AUTOMATICUSERSETTINGS, _TRANSFORM_PROTECT, _TRANSFORM_TRANSCODE, _TRANSFORM_INVERSETRANSCODE, _TRANSFORM_DIFFERENTIATEDSAMPLE, _TRANSFORM_PROTECTEDPATHS, _TRANSFORM_PUBLICPATHS, _TRANSFORM_GETITEM, _TRANSFORM_ASSIGNBUDGET, _TRANSFORM_AUTOMATICBUDGET, _TRANSFORM_ATTRIBUTESBUDGET, _TRANSFORM_SDBUDGET, _TRANSFORM_DERIVESEED, _TRANSFORM_GROUPBYPE, _TRANSFORM_SAMPLINGRATIOS, _TRANSFORM_RELATIONSHIPSPEC, _TRANSFORM_SELECTSQL, _TRANSFORM_EXTRACT, _TRANSFORM_VALIDATEDUSERTYPE, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=158,
-  serialized_end=4203,
+  serialized_end=4285,
 )
 
 _TRANSFORM_PROPERTIESENTRY.containing_type = _TRANSFORM
 _TRANSFORM_SPEC.fields_by_name['identity'].message_type = _TRANSFORM_IDENTITY
 _TRANSFORM_SPEC.fields_by_name['variable'].message_type = _TRANSFORM_VARIABLE
 _TRANSFORM_SPEC.fields_by_name['composed'].message_type = _TRANSFORM_COMPOSED
 _TRANSFORM_SPEC.fields_by_name['project'].message_type = _TRANSFORM_PROJECT
@@ -1943,14 +1974,15 @@
 _TRANSFORM_SPEC.fields_by_name['derive_seed'].message_type = _TRANSFORM_DERIVESEED
 _TRANSFORM_SPEC.fields_by_name['group_by_pe'].message_type = _TRANSFORM_GROUPBYPE
 _TRANSFORM_SPEC.fields_by_name['sampling_ratios'].message_type = _TRANSFORM_SAMPLINGRATIOS
 _TRANSFORM_SPEC.fields_by_name['select_sql'].message_type = _TRANSFORM_SELECTSQL
 _TRANSFORM_SPEC.fields_by_name['extract'].message_type = _TRANSFORM_EXTRACT
 _TRANSFORM_SPEC.fields_by_name['relationship_spec'].message_type = _TRANSFORM_RELATIONSHIPSPEC
 _TRANSFORM_SPEC.fields_by_name['differentiated_sample'].message_type = _TRANSFORM_DIFFERENTIATEDSAMPLE
+_TRANSFORM_SPEC.fields_by_name['validated_user_type'].message_type = _TRANSFORM_VALIDATEDUSERTYPE
 _TRANSFORM_SPEC.containing_type = _TRANSFORM
 _TRANSFORM_SPEC.oneofs_by_name['spec'].fields.append(
   _TRANSFORM_SPEC.fields_by_name['identity'])
 _TRANSFORM_SPEC.fields_by_name['identity'].containing_oneof = _TRANSFORM_SPEC.oneofs_by_name['spec']
 _TRANSFORM_SPEC.oneofs_by_name['spec'].fields.append(
   _TRANSFORM_SPEC.fields_by_name['variable'])
 _TRANSFORM_SPEC.fields_by_name['variable'].containing_oneof = _TRANSFORM_SPEC.oneofs_by_name['spec']
@@ -2034,14 +2066,17 @@
 _TRANSFORM_SPEC.fields_by_name['extract'].containing_oneof = _TRANSFORM_SPEC.oneofs_by_name['spec']
 _TRANSFORM_SPEC.oneofs_by_name['spec'].fields.append(
   _TRANSFORM_SPEC.fields_by_name['relationship_spec'])
 _TRANSFORM_SPEC.fields_by_name['relationship_spec'].containing_oneof = _TRANSFORM_SPEC.oneofs_by_name['spec']
 _TRANSFORM_SPEC.oneofs_by_name['spec'].fields.append(
   _TRANSFORM_SPEC.fields_by_name['differentiated_sample'])
 _TRANSFORM_SPEC.fields_by_name['differentiated_sample'].containing_oneof = _TRANSFORM_SPEC.oneofs_by_name['spec']
+_TRANSFORM_SPEC.oneofs_by_name['spec'].fields.append(
+  _TRANSFORM_SPEC.fields_by_name['validated_user_type'])
+_TRANSFORM_SPEC.fields_by_name['validated_user_type'].containing_oneof = _TRANSFORM_SPEC.oneofs_by_name['spec']
 _TRANSFORM_EXTERNAL_OPIDENTIFIER.fields_by_name['std'].message_type = _TRANSFORM_EXTERNAL_STD
 _TRANSFORM_EXTERNAL_OPIDENTIFIER.fields_by_name['pandas'].message_type = _TRANSFORM_EXTERNAL_PANDAS
 _TRANSFORM_EXTERNAL_OPIDENTIFIER.fields_by_name['numpy'].message_type = _TRANSFORM_EXTERNAL_NUMPY
 _TRANSFORM_EXTERNAL_OPIDENTIFIER.fields_by_name['tensorflow'].message_type = _TRANSFORM_EXTERNAL_TENSORFLOW
 _TRANSFORM_EXTERNAL_OPIDENTIFIER.fields_by_name['sklearn'].message_type = _TRANSFORM_EXTERNAL_SKLEARN
 _TRANSFORM_EXTERNAL_OPIDENTIFIER.fields_by_name['pandas_profiling'].message_type = _TRANSFORM_EXTERNAL_PANDASPROFILING
 _TRANSFORM_EXTERNAL_OPIDENTIFIER.fields_by_name['xgboost'].message_type = _TRANSFORM_EXTERNAL_XGBOOST
@@ -2149,14 +2184,15 @@
 _TRANSFORM_SELECTSQL.oneofs_by_name['select'].fields.append(
   _TRANSFORM_SELECTSQL.fields_by_name['query'])
 _TRANSFORM_SELECTSQL.fields_by_name['query'].containing_oneof = _TRANSFORM_SELECTSQL.oneofs_by_name['select']
 _TRANSFORM_SELECTSQL.oneofs_by_name['select'].fields.append(
   _TRANSFORM_SELECTSQL.fields_by_name['aliased_queries'])
 _TRANSFORM_SELECTSQL.fields_by_name['aliased_queries'].containing_oneof = _TRANSFORM_SELECTSQL.oneofs_by_name['select']
 _TRANSFORM_EXTRACT.containing_type = _TRANSFORM
+_TRANSFORM_VALIDATEDUSERTYPE.containing_type = _TRANSFORM
 _TRANSFORM.fields_by_name['spec'].message_type = _TRANSFORM_SPEC
 _TRANSFORM.fields_by_name['properties'].message_type = _TRANSFORM_PROPERTIESENTRY
 DESCRIPTOR.message_types_by_name['Transform'] = _TRANSFORM
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 Transform = _reflection.GeneratedProtocolMessageType('Transform', (_message.Message,), {
 
@@ -2484,14 +2520,21 @@
 
   'Extract' : _reflection.GeneratedProtocolMessageType('Extract', (_message.Message,), {
     'DESCRIPTOR' : _TRANSFORM_EXTRACT,
     '__module__' : 'sarus_data_spec.protobuf.transform_pb2'
     # @@protoc_insertion_point(class_scope:Transform.Extract)
     })
   ,
+
+  'ValidatedUserType' : _reflection.GeneratedProtocolMessageType('ValidatedUserType', (_message.Message,), {
+    'DESCRIPTOR' : _TRANSFORM_VALIDATEDUSERTYPE,
+    '__module__' : 'sarus_data_spec.protobuf.transform_pb2'
+    # @@protoc_insertion_point(class_scope:Transform.ValidatedUserType)
+    })
+  ,
   'DESCRIPTOR' : _TRANSFORM,
   '__module__' : 'sarus_data_spec.protobuf.transform_pb2'
   # @@protoc_insertion_point(class_scope:Transform)
   })
 _sym_db.RegisterMessage(Transform)
 _sym_db.RegisterMessage(Transform.PropertiesEntry)
 _sym_db.RegisterMessage(Transform.Spec)
@@ -2536,12 +2579,13 @@
 _sym_db.RegisterMessage(Transform.GroupByPE)
 _sym_db.RegisterMessage(Transform.SamplingRatios)
 _sym_db.RegisterMessage(Transform.RelationshipSpec)
 _sym_db.RegisterMessage(Transform.SelectSql)
 _sym_db.RegisterMessage(Transform.SelectSql.AliasedQueries)
 _sym_db.RegisterMessage(Transform.SelectSql.AliasedQuery)
 _sym_db.RegisterMessage(Transform.Extract)
+_sym_db.RegisterMessage(Transform.ValidatedUserType)
 
 
 _TRANSFORM_PROPERTIESENTRY._options = None
 _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._options = None
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/transform_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/transform_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         DERIVE_SEED_FIELD_NUMBER: builtins.int
         GROUP_BY_PE_FIELD_NUMBER: builtins.int
         SAMPLING_RATIOS_FIELD_NUMBER: builtins.int
         SELECT_SQL_FIELD_NUMBER: builtins.int
         EXTRACT_FIELD_NUMBER: builtins.int
         RELATIONSHIP_SPEC_FIELD_NUMBER: builtins.int
         DIFFERENTIATED_SAMPLE_FIELD_NUMBER: builtins.int
+        VALIDATED_USER_TYPE_FIELD_NUMBER: builtins.int
         @property
         def identity(self) -> global___Transform.Identity: ...
         @property
         def variable(self) -> global___Transform.Variable: ...
         @property
         def composed(self) -> global___Transform.Composed: ...
         @property
@@ -121,14 +122,16 @@
         def select_sql(self) -> global___Transform.SelectSql: ...
         @property
         def extract(self) -> global___Transform.Extract: ...
         @property
         def relationship_spec(self) -> global___Transform.RelationshipSpec: ...
         @property
         def differentiated_sample(self) -> global___Transform.DifferentiatedSample: ...
+        @property
+        def validated_user_type(self) -> global___Transform.ValidatedUserType: ...
         def __init__(self,
             *,
             identity : typing.Optional[global___Transform.Identity] = ...,
             variable : typing.Optional[global___Transform.Variable] = ...,
             composed : typing.Optional[global___Transform.Composed] = ...,
             project : typing.Optional[global___Transform.Project] = ...,
             filter : typing.Optional[global___Transform.Filter] = ...,
@@ -153,18 +156,19 @@
             derive_seed : typing.Optional[global___Transform.DeriveSeed] = ...,
             group_by_pe : typing.Optional[global___Transform.GroupByPE] = ...,
             sampling_ratios : typing.Optional[global___Transform.SamplingRatios] = ...,
             select_sql : typing.Optional[global___Transform.SelectSql] = ...,
             extract : typing.Optional[global___Transform.Extract] = ...,
             relationship_spec : typing.Optional[global___Transform.RelationshipSpec] = ...,
             differentiated_sample : typing.Optional[global___Transform.DifferentiatedSample] = ...,
+            validated_user_type : typing.Optional[global___Transform.ValidatedUserType] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"assign_budget",b"assign_budget",u"attribute_budget",b"attribute_budget",u"automatic_budget",b"automatic_budget",u"automatic_user_settings",b"automatic_user_settings",u"cast",b"cast",u"composed",b"composed",u"derive_seed",b"derive_seed",u"differentiated_sample",b"differentiated_sample",u"external",b"external",u"extract",b"extract",u"filter",b"filter",u"get_item",b"get_item",u"group_by_pe",b"group_by_pe",u"identity",b"identity",u"inverse_transcode",b"inverse_transcode",u"join",b"join",u"project",b"project",u"protect_dataset",b"protect_dataset",u"protected_paths",b"protected_paths",u"public_paths",b"public_paths",u"relationship_spec",b"relationship_spec",u"sample",b"sample",u"sampling_ratios",b"sampling_ratios",u"sd_budget",b"sd_budget",u"select_sql",b"select_sql",u"shuffle",b"shuffle",u"spec",b"spec",u"synthetic",b"synthetic",u"transcode",b"transcode",u"user_settings",b"user_settings",u"variable",b"variable"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"assign_budget",b"assign_budget",u"attribute_budget",b"attribute_budget",u"automatic_budget",b"automatic_budget",u"automatic_user_settings",b"automatic_user_settings",u"cast",b"cast",u"composed",b"composed",u"derive_seed",b"derive_seed",u"differentiated_sample",b"differentiated_sample",u"external",b"external",u"extract",b"extract",u"filter",b"filter",u"get_item",b"get_item",u"group_by_pe",b"group_by_pe",u"identity",b"identity",u"inverse_transcode",b"inverse_transcode",u"join",b"join",u"project",b"project",u"protect_dataset",b"protect_dataset",u"protected_paths",b"protected_paths",u"public_paths",b"public_paths",u"relationship_spec",b"relationship_spec",u"sample",b"sample",u"sampling_ratios",b"sampling_ratios",u"sd_budget",b"sd_budget",u"select_sql",b"select_sql",u"shuffle",b"shuffle",u"spec",b"spec",u"synthetic",b"synthetic",u"transcode",b"transcode",u"user_settings",b"user_settings",u"variable",b"variable"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal[u"spec",b"spec"]) -> typing.Optional[typing_extensions.Literal["identity","variable","composed","project","filter","shuffle","join","cast","sample","user_settings","protect_dataset","external","synthetic","transcode","inverse_transcode","get_item","protected_paths","automatic_user_settings","public_paths","assign_budget","automatic_budget","attribute_budget","sd_budget","derive_seed","group_by_pe","sampling_ratios","select_sql","extract","relationship_spec","differentiated_sample"]]: ...
+        def HasField(self, field_name: typing_extensions.Literal[u"assign_budget",b"assign_budget",u"attribute_budget",b"attribute_budget",u"automatic_budget",b"automatic_budget",u"automatic_user_settings",b"automatic_user_settings",u"cast",b"cast",u"composed",b"composed",u"derive_seed",b"derive_seed",u"differentiated_sample",b"differentiated_sample",u"external",b"external",u"extract",b"extract",u"filter",b"filter",u"get_item",b"get_item",u"group_by_pe",b"group_by_pe",u"identity",b"identity",u"inverse_transcode",b"inverse_transcode",u"join",b"join",u"project",b"project",u"protect_dataset",b"protect_dataset",u"protected_paths",b"protected_paths",u"public_paths",b"public_paths",u"relationship_spec",b"relationship_spec",u"sample",b"sample",u"sampling_ratios",b"sampling_ratios",u"sd_budget",b"sd_budget",u"select_sql",b"select_sql",u"shuffle",b"shuffle",u"spec",b"spec",u"synthetic",b"synthetic",u"transcode",b"transcode",u"user_settings",b"user_settings",u"validated_user_type",b"validated_user_type",u"variable",b"variable"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal[u"assign_budget",b"assign_budget",u"attribute_budget",b"attribute_budget",u"automatic_budget",b"automatic_budget",u"automatic_user_settings",b"automatic_user_settings",u"cast",b"cast",u"composed",b"composed",u"derive_seed",b"derive_seed",u"differentiated_sample",b"differentiated_sample",u"external",b"external",u"extract",b"extract",u"filter",b"filter",u"get_item",b"get_item",u"group_by_pe",b"group_by_pe",u"identity",b"identity",u"inverse_transcode",b"inverse_transcode",u"join",b"join",u"project",b"project",u"protect_dataset",b"protect_dataset",u"protected_paths",b"protected_paths",u"public_paths",b"public_paths",u"relationship_spec",b"relationship_spec",u"sample",b"sample",u"sampling_ratios",b"sampling_ratios",u"sd_budget",b"sd_budget",u"select_sql",b"select_sql",u"shuffle",b"shuffle",u"spec",b"spec",u"synthetic",b"synthetic",u"transcode",b"transcode",u"user_settings",b"user_settings",u"validated_user_type",b"validated_user_type",u"variable",b"variable"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing_extensions.Literal[u"spec",b"spec"]) -> typing.Optional[typing_extensions.Literal["identity","variable","composed","project","filter","shuffle","join","cast","sample","user_settings","protect_dataset","external","synthetic","transcode","inverse_transcode","get_item","protected_paths","automatic_user_settings","public_paths","assign_budget","automatic_budget","attribute_budget","sd_budget","derive_seed","group_by_pe","sampling_ratios","select_sql","extract","relationship_spec","differentiated_sample","validated_user_type"]]: ...
 
     class External(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class OpIdentifier(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             STD_FIELD_NUMBER: builtins.int
             PANDAS_FIELD_NUMBER: builtins.int
@@ -678,14 +682,19 @@
         size: builtins.int = ...
         def __init__(self,
             *,
             size : builtins.int = ...,
             ) -> None: ...
         def ClearField(self, field_name: typing_extensions.Literal[u"size",b"size"]) -> None: ...
 
+    class ValidatedUserType(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+        def __init__(self,
+            ) -> None: ...
+
     UUID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     DOC_FIELD_NUMBER: builtins.int
     SPEC_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     INVERSIBLE_FIELD_NUMBER: builtins.int
     SCHEMA_PRESERVING_FIELD_NUMBER: builtins.int
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/type.proto` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/type_pb2.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/type_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/type_pb2.pyi` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/typing.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/protobuf/utilities.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/protobuf/utilities.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/scalar.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/scalar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,11 @@
 from __future__ import annotations
 
-from typing import (
-    Any,
-    Collection,
-    Dict,
-    List,
-    Optional,
-    Set,
-    Tuple,
-    Type,
-    cast,
-)
+from typing import Collection, Dict, List, Optional, Set, Tuple, Type, cast
 import datetime
-import pickle as pkl
 import typing as t
 
 from sarus_data_spec.base import Referring
 from sarus_data_spec.transform import Transform
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 
@@ -56,18 +45,14 @@
         """Is the dataspec a remotely defined dataset."""
         return self.manager().is_remote(self)
 
     def is_source(self) -> bool:
         """Is the scalar not composed."""
         return not self.is_transformed()
 
-    def is_model(self) -> bool:
-        """Is the scalar a model."""
-        return self._protobuf.spec.HasField("model")
-
     def is_privacy_params(self) -> bool:
         """Is the scalar privacy parameters."""
         return self._protobuf.spec.HasField("privacy_params")
 
     def is_random_seed(self) -> bool:
         """Is the scalar a random seed."""
         if self._protobuf.spec.HasField("random_seed"):
@@ -268,32 +253,14 @@
     def attribute(self, name: str) -> Optional[st.Attribute]:
         return self.manager().attribute(name=name, dataspec=self)
 
     def attributes(self, name: str) -> List[st.Attribute]:
         return self.manager().attributes(name=name, dataspec=self)
 
 
-# Builders
-def model(
-    model_class: sp.Scalar.Model.ModelClass.V, *args: Any, **kwargs: Any
-) -> Scalar:
-    return Scalar(
-        sp.Scalar(
-            name=sp.Scalar.Model.ModelClass.Name(model_class),
-            spec=sp.Scalar.Spec(
-                model=sp.Scalar.Model(
-                    model_class=model_class,
-                    arguments=pkl.dumps(args),
-                    named_arguments=pkl.dumps(kwargs),
-                )
-            ),
-        )
-    )
-
-
 def privacy_budget(privacy_limit: st.PrivacyLimit) -> Scalar:
     delta_epsilon_dict = privacy_limit.delta_epsilon_dict()
     return Scalar(
         sp.Scalar(
             name='privacy_budget',
             spec=sp.Scalar.Spec(
                 privacy_params=sp.Scalar.PrivacyParameters(
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/schema.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/schema.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/size.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/size.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/statistics.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/statistics.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/status.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/status.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/storage/local.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/storage/local.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/storage/typing.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/storage/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/storage/utils.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/storage/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/transform.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import datetime
-import pickle as pkl
 import typing as t
 
 import numpy as np
 
 from sarus_data_spec.base import Referrable
+from sarus_data_spec.json_serialisation import SarusJSONEncoder
 from sarus_data_spec.path import straight_path
 import sarus_data_spec.dataset as sd
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 
 
 class Transform(Referrable[sp.Transform]):
@@ -473,33 +473,37 @@
 
 
 def external(
     id: str,
     py_args: t.Dict[int, t.Any] = {},
     py_kwargs: t.Dict[str, t.Any] = {},
     ds_args_pos: t.List[int] = [],
+    ds_types: t.Dict[t.Union[int, str], str] = {},
 ) -> Transform:
     """Create an external library transform.
 
     Args:
         id (str): id in the form library.name (e.g. sklearn.PD_MEAN)
         py_args (Dict[int, Any]):
             the Python objects passed as arguments to the transform.
         py_kwargs (Dict[int, Any]):
             the Python objects passed as keyword arguments to the transform.
         ds_args_pos (List[int]):
             the positions of Dataspecs passed in args.
+        ds_types (Dict[int | str, str]):
+            the types of the Dataspecs passed as arguments.
     """
     external = sp.Transform.External(
-        arguments=pkl.dumps([]),
-        named_arguments=pkl.dumps(
+        arguments=SarusJSONEncoder.encode_bytes([]),
+        named_arguments=SarusJSONEncoder.encode_bytes(
             {
                 "py_args": py_args,
                 "py_kwargs": py_kwargs,
                 "ds_args_pos": ds_args_pos,
+                "ds_types": ds_types,
             }
         ),
         op_identifier=op_identifier_from_id(id),
     )
 
     return Transform(
         sp.Transform(
@@ -933,9 +937,22 @@
             spec=sp.Transform.Spec(
                 relationship_spec=sp.Transform.RelationshipSpec()
             ),
         )
     )
 
 
+def validated_user_type() -> st.Transform:
+    """Transform that allows to set whether the user has validated
+    the schema or if some types have to be changed"""
+    return Transform(
+        sp.Transform(
+            name='validated_user_type',
+            spec=sp.Transform.Spec(
+                validated_user_type=sp.Transform.ValidatedUserType()
+            ),
+        )
+    )
+
+
 if t.TYPE_CHECKING:
     test_transform: st.Transform = Transform(sp.Transform())
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/type.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     PUBLIC,
     TEXT_CHARSET,
     TEXT_MAX_LENGTH,
     USER_COLUMN,
     WEIGHTS,
 )
 from sarus_data_spec.path import Path
+from sarus_data_spec.path import path as path_builder
 from sarus_data_spec.predicate import Predicate
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 
 try:
     import tensorflow as tf
 except ModuleNotFoundError:
@@ -66,15 +67,16 @@
             WEIGHTS,
             DATA,
         }
 
         type = self.protobuf()
         if type.HasField('struct'):
             field_names = {element.name for element in type.struct.fields}
-            return field_names == protected_fields
+            # there may be additional administrative columns
+            return protected_fields.issubset(field_names)
         else:
             return False
 
     def data_type(self) -> Type:
         """Returns the first type level containing the data,
         hence skips the protected_entity struct if there is one"""
         if self.has_protected_format():
@@ -1880,15 +1882,15 @@
                 self, properties: t.Optional[t.Mapping[str, str]] = None
             ) -> None:
                 raise NotImplementedError
 
             def Unit(
                 self, properties: t.Optional[t.Mapping[str, str]] = None
             ) -> None:
-                self.result = pa.nulls(0)
+                self.result = pa.nulls(1)
 
             def Boolean(
                 self, properties: t.Optional[t.Mapping[str, str]] = None
             ) -> None:
                 self.result = pa.array([True], type=pa.bool_())
 
             def Id(
@@ -1897,29 +1899,55 @@
                 reference: t.Optional[st.Path] = None,
                 base: t.Optional[st.IdBase] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
                 # TODO: we should clarify for Ids, user_input
                 # and so on, to be consistent
                 if base == st.IdBase.STRING:
-                    self.result = pa.array(['1'], pa.string())
-                elif base == st.IdBase.INT64:
-                    self.result = pa.array([1], pa.int64())
+                    self.Text(
+                        encoding="",
+                        possible_values=['1'],
+                        properties={
+                            TEXT_CHARSET: "[\"1\"]",
+                            TEXT_MAX_LENGTH: "1",
+                        },
+                    )
+                elif base in (
+                    st.IdBase.INT8,
+                    st.IdBase.INT16,
+                    st.IdBase.INT32,
+                    st.IdBase.INT64,
+                ):
+                    int_base = {
+                        st.IdBase.INT8: st.IntegerBase.INT8,
+                        st.IdBase.INT16: st.IntegerBase.INT16,
+                        st.IdBase.INT32: st.IntegerBase.INT32,
+                        st.IdBase.INT64: st.IntegerBase.INT64,
+                    }[base]
+                    self.Integer(
+                        min=1, max=1, base=int_base, possible_values=[1]
+                    )
                 else:
                     raise NotImplementedError
 
             def Integer(
                 self,
                 min: int,
                 max: int,
                 base: st.IntegerBase,
                 possible_values: t.Iterable[int],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
-                self.result = pa.array([int((min + max) / 2)], type=pa.int64())
+                pa_type: pa.DataType = {
+                    st.IntegerBase.INT8: pa.int8(),
+                    st.IntegerBase.INT16: pa.int16(),
+                    st.IntegerBase.INT32: pa.int32(),
+                    st.IntegerBase.INT64: pa.int64(),
+                }[base]
+                self.result = pa.array([int((min + max) / 2)], type=pa_type)
 
             def Enum(
                 self,
                 name: str,
                 name_values: t.Sequence[t.Tuple[str, int]],
                 ordered: bool,
                 properties: t.Optional[t.Mapping[str, str]] = None,
@@ -1930,15 +1958,25 @@
                 self,
                 min: float,
                 max: float,
                 base: st.FloatBase,
                 possible_values: t.Iterable[float],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
-                self.result = pa.array([(min + max) / 2], type=pa.float64())
+                pa_type: pa.DataType = {
+                    st.FloatBase.FLOAT16: pa.float16(),
+                    st.FloatBase.FLOAT32: pa.float32(),
+                    st.FloatBase.FLOAT64: pa.float64(),
+                }[base]
+
+                x: t.Union[float, np.float16] = (min + max) / 2
+                if base == st.FloatBase.FLOAT16:
+                    x = np.float16(x)
+
+                self.result = pa.array([x], type=pa_type)
 
             def Text(
                 self,
                 encoding: str,
                 possible_values: t.Iterable[str],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
@@ -2792,14 +2830,229 @@
             ) -> None:
                 raise NotImplementedError
 
         visitor = ToTensorflow(properties=self.properties())
         self.accept(visitor)
         return visitor.result
 
+    def path_leaves(self) -> t.Sequence[st.Path]:
+        """Returns the list of each path to a leaf in the type. If the type
+        is a leaf, it returns an empty list"""
+
+        class PathLeaves(st.TypeVisitor):
+            result = []
+
+            def Struct(
+                self,
+                fields: t.Mapping[str, st.Type],
+                name: t.Optional[str] = None,
+                properties: t.Optional[t.Mapping[str, str]] = None,
+            ) -> None:
+                for field_name, field_type in fields.items():
+                    sub_paths = field_type.path_leaves()
+                    if len(sub_paths) > 0:
+                        self.result.extend(
+                            [
+                                path_builder(label=field_name, paths=[el])
+                                for el in sub_paths
+                            ]
+                        )
+                    else:
+                        self.result.extend(
+                            [path_builder(label=field_name, paths=[])]
+                        )
+
+            def Union(
+                self,
+                fields: t.Mapping[str, st.Type],
+                name: t.Optional[str] = None,
+                properties: t.Optional[t.Mapping[str, str]] = None,
+            ) -> None:
+                for field_name, field_type in fields.items():
+                    sub_paths = field_type.path_leaves()
+                    if len(sub_paths) > 0:
+                        self.result.extend(
+                            [
+                                path_builder(label=field_name, paths=[el])
+                                for el in sub_paths
+                            ]
+                        )
+                    else:
+                        self.result.extend(
+                            [path_builder(label=field_name, paths=[])]
+                        )
+
+            def Optional(
+                self,
+                type: st.Type,
+                name: t.Optional[str] = None,
+                properties: t.Optional[t.Mapping[str, str]] = None,
+            ) -> None:
+
+                sub_paths = type.path_leaves()
+                if len(sub_paths) > 0:
+                    self.result.extend(
+                        [
+                            path_builder(label=OPTIONAL_VALUE, paths=[el])
+                            for el in sub_paths
+                        ]
+                    )
+                else:
+                    self.result.extend(
+                        [path_builder(label=OPTIONAL_VALUE, paths=[])]
+                    )
+
+            def Null(
+                self, properties: t.Optional[t.Mapping[str, str]] = None
+            ) -> None:
+                pass
+
+            def Unit(
+                self, properties: t.Optional[t.Mapping[str, str]] = None
+            ) -> None:
+                pass
+
+            def Boolean(
+                self, properties: t.Optional[t.Mapping[str, str]] = None
+            ) -> None:
+                pass
+
+            def Id(
+                self,
+                unique: bool,
+                reference: t.Optional[st.Path] = None,
+                base: t.Optional[st.IdBase] = None,
+                properties: t.Optional[t.Mapping[str, str]] = None,
+            ) -> None:
+                pass
+
+            def Integer(
+                self,
+                min: int,
+                max: int,
+                base: st.IntegerBase,
+                possible_values: t.Iterable[int],
+                properties: t.Optional[t.Mapping[str, str]] = None,
+            ) -> None:
+                pass
+
+            def Enum(
+                self,
+                name: str,
+                name_values: t.Sequence[t.Tuple[str, int]],
+                ordered: bool,
+                properties: t.Optional[t.Mapping[str, str]] = None,
+            ) -> None:
+                pass
+
+            def Float(
+                self,
+                min: float,
+                max: float,
+                base: st.FloatBase,
+                possible_values: t.Iterable[float],
+                properties: t.Optional[t.Mapping[str, str]] = None,
+            ) -> None:
+                pass
+
+            def Text(
+                self,
+                encoding: str,
+                possible_values: t.Iterable[str],
+                properties: t.Optional[t.Mapping[str, str]] = None,
+            ) -> None:
+                pass
+
+            def Bytes(
+                self, properties: t.Optional[t.Mapping[str, str]] = None
+            ) -> None:
+                pass
+
+            def List(
+                self,
+                type: st.Type,
+                max_size: int,
+                name: t.Optional[str] = None,
+                properties: t.Optional[t.Mapping[str, str]] = None,
+            ) -> None:
+                raise NotImplementedError
+
+            def Array(
+                self,
+                type: st.Type,
+                shape: t.Tuple[int, ...],
+                name: t.Optional[str] = None,
+                properties: t.Optional[t.Mapping[str, str]] = None,
+            ) -> None:
+                raise NotImplementedError
+
+            def Datetime(
+                self,
+                format: str,
+                min: str,
+                max: str,
+                base: st.DatetimeBase,
+                possible_values: t.Iterable[str],
+                properties: t.Optional[t.Mapping[str, str]] = None,
+            ) -> None:
+                pass
+
+            def Date(
+                self,
+                format: str,
+                min: str,
+                max: str,
+                base: st.DateBase,
+                possible_values: t.Iterable[str],
+                properties: t.Optional[t.Mapping[str, str]] = None,
+            ) -> None:
+                pass
+
+            def Time(
+                self,
+                format: str,
+                min: str,
+                max: str,
+                base: st.TimeBase,
+                possible_values: t.Iterable[str],
+                properties: t.Optional[t.Mapping[str, str]] = None,
+            ) -> None:
+                pass
+
+            def Duration(
+                self,
+                unit: str,
+                min: int,
+                max: int,
+                possible_values: t.Iterable[int],
+                properties: t.Optional[t.Mapping[str, str]] = None,
+            ) -> None:
+                pass
+
+            def Constrained(
+                self,
+                type: st.Type,
+                constraint: st.Predicate,
+                name: t.Optional[str] = None,
+                properties: t.Optional[t.Mapping[str, str]] = None,
+            ) -> None:
+                raise NotImplementedError
+
+            def Hypothesis(
+                self,
+                *types: t.Tuple[st.Type, float],
+                name: t.Optional[str] = None,
+                properties: t.Optional[t.Mapping[str, str]] = None,
+            ) -> None:
+                raise NotImplementedError
+
+        visitor = PathLeaves()
+        self.accept(visitor)
+        return visitor.result
+
 
 # A few builders
 def Null(
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Type:
     return Type(
         sp.Type(name='Null', null=sp.Type.Null(), properties=properties)
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/typing.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,20 @@
 
 if t.TYPE_CHECKING:
     from sklearn import svm
 
     DataSpecValue = t.Union[pd.DataFrame, np.ndarray, svm.SVC]
 else:
     DataSpecValue = t.Any
+
+
+# List of types a Dataset can be converted to
+DatasetCastable = t.Union[pd.DataFrame, pd.Series, t.Iterator[pa.RecordBatch]]
+
+
 P = t.TypeVar('P', bound=Protobuf, covariant=True)
 
 
 @t.runtime_checkable
 class HasProtobuf(t.Protocol[P]):
     """An object backed by a protocol buffer message."""
 
@@ -308,14 +314,17 @@
 
     def is_file(self) -> bool:
         ...
 
     def schema(self) -> Schema:
         ...
 
+    async def async_schema(self) -> Schema:
+        ...
+
     def size(self) -> t.Optional[Size]:
         ...
 
     def bounds(self) -> t.Optional[Bounds]:
         ...
 
     def marginals(self) -> t.Optional[Marginals]:
@@ -346,14 +355,23 @@
 
     def to_tensorflow(self) -> tf.data.Dataset:
         ...
 
     async def async_to_tensorflow(self) -> tf.data.Dataset:
         ...
 
+    async def async_to(
+        self, kind: t.Type, drop_admin: bool = True
+    ) -> DatasetCastable:
+        """Casts a Dataset to a Python type passed as argument."""
+        ...
+
+    def to(self, kind: t.Type, drop_admin: bool = True) -> DatasetCastable:
+        ...
+
     def dot(self) -> str:
         """return a graphviz representation of the dataset"""
         ...
 
     def sql(
         self,
         query: t.Union[str, t.Mapping[t.Union[str, t.Tuple[str, ...]], str]],
@@ -379,17 +397,14 @@
 
 
 class Scalar(DataSpec[sp.Scalar], t.Protocol):
     def prototype(self) -> t.Type[sp.Scalar]:
         """Return the type of the underlying protobuf."""
         ...
 
-    def is_model(self) -> bool:
-        ...
-
     def is_privacy_params(self) -> bool:
         """Is the scalar privacy parameters."""
 
     def is_random_seed(self) -> bool:
         """Is the scalar a random seed."""
 
     def is_synthetic_model(self) -> bool:
@@ -722,14 +737,18 @@
         """Return the type of the underlying protobuf."""
         ...
 
     def name(self) -> str:
         """Returns the name of the underlying protobuf."""
         ...
 
+    def data_type(self) -> Type:
+        """Returns the first type level containing the data,
+        hence skips the protected_entity struct if there is one"""
+
     def has_protected_format(self) -> bool:
         """Return True if the Type has the protected formalism."""
         ...
 
     def latex(self: Type, parenthesized: bool = False) -> str:
         """return a latex representation of the type"""
         ...
@@ -797,14 +816,18 @@
 
     def tensorflow_example(self: Type) -> t.Any:
         """Returns an example of a dictionary with tensors as leaves
         that match the type..
         For an optional type, it returns a non missing value of the type.
         """
 
+    def path_leaves(self) -> t.Sequence[Path]:
+        """Returns the list of each path to a leaf in the type. If the type
+        is a leaf, it returns an empty list"""
+
 
 class IdBase(Enum):
     INT64 = sp.Type.Id.INT64
     INT32 = sp.Type.Id.INT32
     INT16 = sp.Type.Id.INT16
     INT8 = sp.Type.Id.INT8
     STRING = sp.Type.Id.STRING
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec/variant_constraint.py` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec/variant_constraint.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.0.0.dev2/sarus_data_spec_public.egg-info/SOURCES.txt` & `sarus_data_spec_public-3.0.1.dev0/sarus_data_spec_public.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,33 @@
 sarus_data_spec/attribute.py
 sarus_data_spec/base.py
 sarus_data_spec/bounds.py
 sarus_data_spec/constants.py
 sarus_data_spec/dataset.py
 sarus_data_spec/deprecation.py
 sarus_data_spec/factory.py
+sarus_data_spec/json_serialisation.py
 sarus_data_spec/marginals.py
 sarus_data_spec/path.py
 sarus_data_spec/predicate.py
 sarus_data_spec/py.typed
 sarus_data_spec/scalar.py
 sarus_data_spec/schema.py
 sarus_data_spec/size.py
 sarus_data_spec/statistics.py
 sarus_data_spec/status.py
 sarus_data_spec/transform.py
 sarus_data_spec/type.py
 sarus_data_spec/typing.py
 sarus_data_spec/variant_constraint.py
 sarus_data_spec/arrow/__init__.py
+sarus_data_spec/arrow/admin_utils.py
 sarus_data_spec/arrow/array.py
+sarus_data_spec/arrow/conversion.py
+sarus_data_spec/arrow/pandas_utils.py
 sarus_data_spec/arrow/schema.py
 sarus_data_spec/arrow/type.py
 sarus_data_spec/config/__init__.py
 sarus_data_spec/config/privacy_properties.yaml
 sarus_data_spec/config/routing.yaml
 sarus_data_spec/context/__init__.py
 sarus_data_spec/context/public.py
@@ -60,17 +64,19 @@
 sarus_data_spec/manager/ops/processor/routing.py
 sarus_data_spec/manager/ops/processor/external/__init__.py
 sarus_data_spec/manager/ops/processor/external/external_op.py
 sarus_data_spec/manager/ops/processor/external/imblearn.py
 sarus_data_spec/manager/ops/processor/external/numpy.py
 sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
 sarus_data_spec/manager/ops/processor/external/protection_utils.py
+sarus_data_spec/manager/ops/processor/external/signature.py
 sarus_data_spec/manager/ops/processor/external/sklearn.py
 sarus_data_spec/manager/ops/processor/external/skopt.py
 sarus_data_spec/manager/ops/processor/external/std.py
+sarus_data_spec/manager/ops/processor/external/utils.py
 sarus_data_spec/manager/ops/processor/external/xgboost.py
 sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
 sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
 sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
 sarus_data_spec/manager/ops/processor/standard/__init__.py
 sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
 sarus_data_spec/manager/ops/processor/standard/extract.py
@@ -80,15 +86,14 @@
 sarus_data_spec/manager/ops/processor/standard/sample.py
 sarus_data_spec/manager/ops/processor/standard/select_sql.py
 sarus_data_spec/manager/ops/processor/standard/shuffle.py
 sarus_data_spec/manager/ops/processor/standard/standard_op.py
 sarus_data_spec/manager/ops/processor/standard/synthetic.py
 sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
 sarus_data_spec/manager/ops/source/__init__.py
-sarus_data_spec/manager/ops/source/model.py
 sarus_data_spec/manager/ops/source/privacy_params.py
 sarus_data_spec/manager/ops/source/random_seed.py
 sarus_data_spec/manager/ops/source/routing.py
 sarus_data_spec/protobuf/__init__.py
 sarus_data_spec/protobuf/attribute.proto
 sarus_data_spec/protobuf/attribute_pb2.py
 sarus_data_spec/protobuf/attribute_pb2.pyi
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/setup.cfg` & `sarus_data_spec_public-3.0.1.dev0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 [options]
 zip_safe = False
 python_requires = >=3.8
 include_package_data = True
 packages = sarus_data_spec.config
 py_modules = 
 	sarus_data_spec.arrow.array
+	sarus_data_spec.arrow.conversion
+	sarus_data_spec.arrow.pandas_utils
+	sarus_data_spec.arrow.admin_utils
 	sarus_data_spec.arrow.schema
 	sarus_data_spec.arrow.type
 	sarus_data_spec.attribute
 	sarus_data_spec.base
 	sarus_data_spec.bounds
 	sarus_data_spec.constants
 	sarus_data_spec.dataset
@@ -36,14 +39,15 @@
 	sarus_data_spec.schema
 	sarus_data_spec.size
 	sarus_data_spec.statistics
 	sarus_data_spec.status
 	sarus_data_spec.transform
 	sarus_data_spec.type
 	sarus_data_spec.typing
+	sarus_data_spec.json_serialisation
 	sarus_data_spec.variant_constraint
 	sarus_data_spec.storage.typing
 	sarus_data_spec.storage.utils
 	sarus_data_spec.storage.local
 	sarus_data_spec.manager.typing
 	sarus_data_spec.manager.base
 	sarus_data_spec.manager.base
@@ -74,15 +78,17 @@
 	sarus_data_spec.manager.ops.processor.external.numpy
 	sarus_data_spec.manager.ops.processor.external.pandas.pandas
 	sarus_data_spec.manager.ops.processor.external.pandas.pandas_dp
 	sarus_data_spec.manager.ops.processor.external.pandas_profiling
 	sarus_data_spec.manager.ops.processor.external.protection_utils
 	sarus_data_spec.manager.ops.processor.external.sklearn
 	sarus_data_spec.manager.ops.processor.external.skopt
+	sarus_data_spec.manager.ops.processor.external.signature
 	sarus_data_spec.manager.ops.processor.external.std
+	sarus_data_spec.manager.ops.processor.external.utils
 	sarus_data_spec.manager.ops.processor.external.xgboost
 	sarus_data_spec.dataspec_rewriter.typing
 	sarus_data_spec.dataspec_rewriter.base
 	sarus_data_spec.dataspec_rewriter.simple_rules
 	sarus_data_spec.dataspec_validator.typing
 	sarus_data_spec.dataspec_validator.base
 	sarus_data_spec.dataspec_validator.simple_rules
```

### Comparing `sarus_data_spec_public-3.0.0.dev2/setup.py` & `sarus_data_spec_public-3.0.1.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
     def run(self):
         generate_proto_code()
         build_py.run(self)
 
 
 if __name__ == '__main__':
-    setup(version='3.0.0.dev2')
+    setup(version='3.0.1.dev0')
```

