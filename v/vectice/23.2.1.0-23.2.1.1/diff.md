# Comparing `tmp/vectice-23.2.1.0.tar.gz` & `tmp/vectice-23.2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectice-23.2.1.0.tar", last modified: Mon Apr 17 08:04:27 2023, max compression
+gzip compressed data, was "vectice-23.2.1.1.tar", last modified: Mon Apr 17 08:09:05 2023, max compression
```

## Comparing `vectice-23.2.1.0.tar` & `vectice-23.2.1.1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:04:27.272502 vectice-23.2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 08:04:13.000000 vectice-23.2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-17 08:04:27.272502 vectice-23.2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-17 08:04:13.000000 vectice-23.2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-17 08:04:13.000000 vectice-23.2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-17 08:04:27.272502 vectice-23.2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-17 08:04:13.000000 vectice-23.2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:04:27.244502 vectice-23.2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:04:27.248502 vectice-23.2.1.0/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:04:27.252502 vectice-23.2.1.0/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    25024 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/gql_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/gql_code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/gql_feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:04:27.256502 vectice-23.2.1.0/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/user_declared_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/api/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:04:27.264502 vectice-23.2.1.0/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:04:27.264502 vectice-23.2.1.0/src/vectice/models/datasource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/datasource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:04:27.264502 vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/file_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/gcs_data_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:04:27.268502 vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/s3_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/git_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:04:27.268502 vectice-23.2.1.0/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/resource/bigquery_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:04:27.268502 vectice-23.2.1.0/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/resource/metadata/column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/resource/metadata/dataframe_column_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/resource/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/step_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/step_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/step_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/step_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/step_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:04:27.272502 vectice-23.2.1.0/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/utils/automatic_link_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-17 08:04:13.000000 vectice-23.2.1.0/src/vectice/utils/logging_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:04:27.248502 vectice-23.2.1.0/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-17 08:04:27.000000 vectice-23.2.1.0/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-17 08:04:27.000000 vectice-23.2.1.0/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:04:27.000000 vectice-23.2.1.0/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-17 08:04:27.000000 vectice-23.2.1.0/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 08:04:27.000000 vectice-23.2.1.0/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.407174 vectice-23.2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 08:08:56.000000 vectice-23.2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-17 08:09:05.407174 vectice-23.2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-17 08:08:56.000000 vectice-23.2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-17 08:08:56.000000 vectice-23.2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-17 08:09:05.407174 vectice-23.2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-17 08:08:56.000000 vectice-23.2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.387174 vectice-23.2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.391174 vectice-23.2.1.1/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.395174 vectice-23.2.1.1/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25024 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/gql_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/gql_code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/gql_feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.399174 vectice-23.2.1.1/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/user_declared_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/api/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.403174 vectice-23.2.1.1/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.403174 vectice-23.2.1.1/src/vectice/models/datasource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.403174 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/file_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/gcs_data_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.403174 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/s3_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/git_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.403174 vectice-23.2.1.1/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/bigquery_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.403174 vectice-23.2.1.1/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/metadata/dataframe_column_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/step_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/step_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/step_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/step_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/step_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.403174 vectice-23.2.1.1/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/utils/automatic_link_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-17 08:08:56.000000 vectice-23.2.1.1/src/vectice/utils/logging_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:09:05.395174 vectice-23.2.1.1/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-17 08:09:05.000000 vectice-23.2.1.1/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-17 08:09:05.000000 vectice-23.2.1.1/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:09:05.000000 vectice-23.2.1.1/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-17 08:09:05.000000 vectice-23.2.1.1/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 08:09:05.000000 vectice-23.2.1.1/src/vectice.egg-info/top_level.txt
```

### Comparing `vectice-23.2.1.0/LICENSE` & `vectice-23.2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/PKG-INFO` & `vectice-23.2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.1.0
+Version: 23.2.1.1
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.2.1.0/setup.py` & `vectice-23.2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/__init__.py` & `vectice-23.2.1.1/src/vectice/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/__init__.py` & `vectice-23.2.1.1/src/vectice/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/_auth.py` & `vectice-23.2.1.1/src/vectice/api/_auth.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/_utils.py` & `vectice-23.2.1.1/src/vectice/api/_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/attachment.py` & `vectice-23.2.1.1/src/vectice/api/attachment.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/client.py` & `vectice-23.2.1.1/src/vectice/api/client.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/gql_api.py` & `vectice-23.2.1.1/src/vectice/api/gql_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/gql_code.py` & `vectice-23.2.1.1/src/vectice/api/gql_code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/gql_code_version.py` & `vectice-23.2.1.1/src/vectice/api/gql_code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/gql_dataset.py` & `vectice-23.2.1.1/src/vectice/api/gql_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/gql_feature_flag.py` & `vectice-23.2.1.1/src/vectice/api/gql_feature_flag.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/gql_model.py` & `vectice-23.2.1.1/src/vectice/api/gql_model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/gql_user_workspace_api.py` & `vectice-23.2.1.1/src/vectice/api/gql_user_workspace_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/http_error.py` & `vectice-23.2.1.1/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/http_error_handlers.py` & `vectice-23.2.1.1/src/vectice/api/http_error_handlers.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/iteration.py` & `vectice-23.2.1.1/src/vectice/api/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/__init__.py` & `vectice-23.2.1.1/src/vectice/api/json/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/artifact_version.py` & `vectice-23.2.1.1/src/vectice/api/json/artifact_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/code.py` & `vectice-23.2.1.1/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/code_version.py` & `vectice-23.2.1.1/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/dataset_register.py` & `vectice-23.2.1.1/src/vectice/api/json/dataset_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/files_metadata.py` & `vectice-23.2.1.1/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/iteration.py` & `vectice-23.2.1.1/src/vectice/api/json/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/last_assets.py` & `vectice-23.2.1.1/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/metric.py` & `vectice-23.2.1.1/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/model.py` & `vectice-23.2.1.1/src/vectice/api/json/model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/model_register.py` & `vectice-23.2.1.1/src/vectice/api/json/model_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/model_version.py` & `vectice-23.2.1.1/src/vectice/api/json/model_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/paged_response.py` & `vectice-23.2.1.1/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/phase.py` & `vectice-23.2.1.1/src/vectice/api/json/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/project.py` & `vectice-23.2.1.1/src/vectice/api/json/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/property.py` & `vectice-23.2.1.1/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/public_config.py` & `vectice-23.2.1.1/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/step.py` & `vectice-23.2.1.1/src/vectice/api/json/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/json/workspace.py` & `vectice-23.2.1.1/src/vectice/api/json/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/last_assets.py` & `vectice-23.2.1.1/src/vectice/api/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/phase.py` & `vectice-23.2.1.1/src/vectice/api/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/project.py` & `vectice-23.2.1.1/src/vectice/api/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/rest_api.py` & `vectice-23.2.1.1/src/vectice/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/step.py` & `vectice-23.2.1.1/src/vectice/api/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/version.py` & `vectice-23.2.1.1/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/api/workspace.py` & `vectice-23.2.1.1/src/vectice/api/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/connection.py` & `vectice-23.2.1.1/src/vectice/connection.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/__init__.py` & `vectice-23.2.1.1/src/vectice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/attachment_container.py` & `vectice-23.2.1.1/src/vectice/models/attachment_container.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/dataset.py` & `vectice-23.2.1.1/src/vectice/models/dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/__init__.py` & `vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/data_wrapper.py` & `vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/data_wrapper.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/file_data_wrapper.py` & `vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/file_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/gcs_data_wrapper.py` & `vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/gcs_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/metadata/__init__.py` & `vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/metadata/db_metadata.py` & `vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/metadata/db_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/metadata/files_metadata.py` & `vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/metadata/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/datasource/datawrapper/s3_data_wrapper.py` & `vectice-23.2.1.1/src/vectice/models/datasource/datawrapper/s3_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/git_version.py` & `vectice-23.2.1.1/src/vectice/models/git_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/iteration.py` & `vectice-23.2.1.1/src/vectice/models/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/metric.py` & `vectice-23.2.1.1/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/model.py` & `vectice-23.2.1.1/src/vectice/models/model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/phase.py` & `vectice-23.2.1.1/src/vectice/models/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/project.py` & `vectice-23.2.1.1/src/vectice/models/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/property.py` & `vectice-23.2.1.1/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/resource/__init__.py` & `vectice-23.2.1.1/src/vectice/models/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/resource/base.py` & `vectice-23.2.1.1/src/vectice/models/resource/base.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/resource/bigquery_resource.py` & `vectice-23.2.1.1/src/vectice/models/resource/bigquery_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
-from google.api_core.exceptions import Forbidden
-
 from vectice.models.resource.base import Resource
 from vectice.models.resource.metadata import DatasetSourceOrigin
 from vectice.models.resource.metadata.column_metadata import DBColumn
 from vectice.models.resource.metadata.db_metadata import DBMetadata, MetadataDB
 
 if TYPE_CHECKING:
     from google.cloud.bigquery import Client as BQClient
@@ -66,14 +64,16 @@
             path: The path to retrieve the dataset or the table.
         """
         super().__init__()
         self.path = path
         self.bq_client = bq_client
 
     def _fetch_data(self) -> dict[str, Table | None]:
+        from google.api_core.exceptions import Forbidden
+
         count_dots_in_path = self.path.count(".")
         is_dataset = count_dots_in_path == 1
         is_table = count_dots_in_path == 2
 
         if is_table is True:
             table_name = self.path.rpartition(".")[-1]
             tb = None
```

### Comparing `vectice-23.2.1.0/src/vectice/models/resource/description.py` & `vectice-23.2.1.1/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/resource/file_resource.py` & `vectice-23.2.1.1/src/vectice/models/resource/file_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/resource/gcs_resource.py` & `vectice-23.2.1.1/src/vectice/models/resource/gcs_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/resource/metadata/__init__.py` & `vectice-23.2.1.1/src/vectice/models/resource/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/resource/metadata/base.py` & `vectice-23.2.1.1/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/resource/metadata/column_metadata.py` & `vectice-23.2.1.1/src/vectice/models/resource/metadata/column_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/resource/metadata/dataframe_column_parser.py` & `vectice-23.2.1.1/src/vectice/models/resource/metadata/dataframe_column_parser.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-23.2.1.1/src/vectice/models/resource/metadata/db_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/resource/metadata/files_metadata.py` & `vectice-23.2.1.1/src/vectice/models/resource/metadata/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/resource/metadata/source.py` & `vectice-23.2.1.1/src/vectice/models/resource/metadata/source.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/resource/s3_resource.py` & `vectice-23.2.1.1/src/vectice/models/resource/s3_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/step.py` & `vectice-23.2.1.1/src/vectice/models/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/step_dataset.py` & `vectice-23.2.1.1/src/vectice/models/step_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/step_image.py` & `vectice-23.2.1.1/src/vectice/models/step_image.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/step_model.py` & `vectice-23.2.1.1/src/vectice/models/step_model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/step_number.py` & `vectice-23.2.1.1/src/vectice/models/step_number.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/step_string.py` & `vectice-23.2.1.1/src/vectice/models/step_string.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/models/workspace.py` & `vectice-23.2.1.1/src/vectice/models/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/utils/automatic_link_utils.py` & `vectice-23.2.1.1/src/vectice/utils/automatic_link_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/utils/common_utils.py` & `vectice-23.2.1.1/src/vectice/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/utils/configuration.py` & `vectice-23.2.1.1/src/vectice/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/utils/deprecation.py` & `vectice-23.2.1.1/src/vectice/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/utils/last_assets.py` & `vectice-23.2.1.1/src/vectice/utils/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice/utils/logging_utils.py` & `vectice-23.2.1.1/src/vectice/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice.egg-info/PKG-INFO` & `vectice-23.2.1.1/src/vectice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.1.0
+Version: 23.2.1.1
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.2.1.0/src/vectice.egg-info/SOURCES.txt` & `vectice-23.2.1.1/src/vectice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vectice-23.2.1.0/src/vectice.egg-info/requires.txt` & `vectice-23.2.1.1/src/vectice.egg-info/requires.txt`

 * *Files identical despite different names*

