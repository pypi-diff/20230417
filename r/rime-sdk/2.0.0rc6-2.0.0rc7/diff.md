# Comparing `tmp/rime_sdk-2.0.0rc6.tar.gz` & `tmp/rime_sdk-2.0.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rime_sdk-2.0.0rc6.tar", last modified: Wed Apr 12 04:35:30 2023, max compression
+gzip compressed data, was "rime_sdk-2.0.0rc7.tar", last modified: Mon Apr 17 02:24:05 2023, max compression
```

## Comparing `rime_sdk-2.0.0rc6.tar` & `rime_sdk-2.0.0rc7.tar`

### file list

```diff
@@ -1,477 +1,477 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.543780 rime_sdk-2.0.0rc6/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-04-12 04:35:30.543780 rime_sdk-2.0.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27071 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.459778 rime_sdk-2.0.0rc6/rime_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57754 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.463778 rime_sdk-2.0.0rc6/rime_sdk/data_format_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/data_format_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/data_format_check/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/data_format_check/data_format_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/data_format_check/nlp_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/data_format_check/tabular_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    22486 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.467779 rime_sdk-2.0.0rc6/rime_sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28424 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/file_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/rest_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/security_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/swagger_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/swagger_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/throttle_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16763 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    55004 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    23861 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.467779 rime_sdk-2.0.0rc6/rime_sdk/swagger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.467779 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)    45243 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.471778 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22707 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25158 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/data_collector_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/detection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/file_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/image_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26851 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/integration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26951 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/job_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/model_testing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29422 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    55776 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/project_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    57282 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/registry_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    50274 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/results_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/rime_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    41732 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.543780 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    43392 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_custom_loader_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_data_collector_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_data_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_delta_lake_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_location_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_location_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/model_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/model_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/model_model_path_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_object_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_project_with_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_any.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_rca_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_rca_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/registry_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_archived_job_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_config_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_float_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_int_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_named_double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_str_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_termination_reason.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_token_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/role_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_connection_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/user_private_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/user_user_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-04-12 04:35:26.000000 rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14716 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/rime_sdk/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:35:30.459778 rime_sdk-2.0.0rc6/rime_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-04-12 04:35:30.000000 rime_sdk-2.0.0rc6/rime_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31351 2023-04-12 04:35:30.000000 rime_sdk-2.0.0rc6/rime_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 04:35:30.000000 rime_sdk-2.0.0rc6/rime_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-12 04:35:30.000000 rime_sdk-2.0.0rc6/rime_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-12 04:35:30.000000 rime_sdk-2.0.0rc6/rime_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 04:35:30.000000 rime_sdk-2.0.0rc6/rime_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 04:35:30.547780 rime_sdk-2.0.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-12 04:34:53.000000 rime_sdk-2.0.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.340397 rime_sdk-2.0.0rc7/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-17 02:24:05.340397 rime_sdk-2.0.0rc7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.300397 rime_sdk-2.0.0rc7/rime_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57906 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.300397 rime_sdk-2.0.0rc7/rime_sdk/data_format_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/data_format_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/data_format_check/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/data_format_check/data_format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/data_format_check/nlp_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/data_format_check/tabular_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22506 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.304397 rime_sdk-2.0.0rc7/rime_sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28424 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/rest_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/security_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/swagger_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/swagger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/throttle_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16763 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55004 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23861 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.304397 rime_sdk-2.0.0rc7/rime_sdk/swagger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.304397 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    45249 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.304397 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22707 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25158 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/data_collector_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/detection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/file_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/image_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26851 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/integration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26951 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/job_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/model_testing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29422 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55776 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/project_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57282 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/registry_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50274 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/results_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/rime_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41732 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.340397 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    43398 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_custom_loader_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_data_collector_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_data_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_delta_lake_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_location_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_location_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/model_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/model_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/model_model_path_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_object_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_project_with_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/protobuf_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_rca_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_rca_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_archived_job_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_config_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_float_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_int_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_named_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_str_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_table_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_termination_reason.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_token_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/role_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_connection_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/user_private_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/user_user_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14716 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.300397 rime_sdk-2.0.0rc7/rime_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-17 02:24:05.000000 rime_sdk-2.0.0rc7/rime_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31354 2023-04-17 02:24:05.000000 rime_sdk-2.0.0rc7/rime_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 02:24:05.000000 rime_sdk-2.0.0rc7/rime_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-17 02:24:05.000000 rime_sdk-2.0.0rc7/rime_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-17 02:24:05.000000 rime_sdk-2.0.0rc7/rime_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 02:24:05.000000 rime_sdk-2.0.0rc7/rime_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 02:24:05.340397 rime_sdk-2.0.0rc7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/setup.py
```

### Comparing `rime_sdk-2.0.0rc6/LICENSE` & `rime_sdk-2.0.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/__init__.py` & `rime_sdk-2.0.0rc7/rime_sdk/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-"""Python package providing access to RIME's backend services.
+"""Python package providing access to Robust Intelligence.
 
-The main entry point should be through the Client. The other
-classes provide more modular functionality.
+The RIME SDK provides a programmatic interface to a Robust Intelligence
+instance, allowing you to create projects, start stress tests, query the
+backend for test run results, and more from within your Python code. To
+begin, initialize a client, which acts as the main entry point to SDK
+functions.
 
 """
 from rime_sdk.client import (
     Client,
     ManagedImagePackageRequirement,
     ManagedImagePipRequirement,
 )
```

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/client.py` & `rime_sdk-2.0.0rc7/rime_sdk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Library to initiate backend RIME service requests."""
+import atexit
 import json
 import logging
 import re
 from collections import Counter
 from datetime import date, datetime
 from http import HTTPStatus
 from inspect import getmembers
@@ -149,14 +150,16 @@
         # client certificate file
         configuration.cert_file = cert_file
         # client key file
         configuration.key_file = key_file
         # Set this to True/False to enable/disable SSL hostname verification.
         configuration.assert_hostname = assert_hostname
         self._api_client = ApiClient(configuration)
+        # Prevent race condition in pool.close() triggered by swagger generated code
+        atexit.register(self._api_client.pool.close)
         # Sets the timeout and hardcoded retries parameter for the api client.
         self._api_client.rest_client.pool_manager.connection_pool_kw[
             "timeout"
         ] = channel_timeout
         self._api_client.rest_client.pool_manager.connection_pool_kw["retries"] = Retry(
             total=3, status_forcelist=self.RETRY_HTTP_STATUS
         )
```

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/data_collector.py` & `rime_sdk-2.0.0rc7/rime_sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/data_format_check/cli.py` & `rime_sdk-2.0.0rc7/rime_sdk/data_format_check/cli.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/data_format_check/data_format_checker.py` & `rime_sdk-2.0.0rc7/rime_sdk/data_format_check/data_format_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/data_format_check/nlp_checker.py` & `rime_sdk-2.0.0rc7/rime_sdk/data_format_check/nlp_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/data_format_check/tabular_checker.py` & `rime_sdk-2.0.0rc7/rime_sdk/data_format_check/tabular_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/detection_event.py` & `rime_sdk-2.0.0rc7/rime_sdk/detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/firewall.py` & `rime_sdk-2.0.0rc7/rime_sdk/firewall.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 from rime_sdk.internal.throttle_queue import ThrottleQueue
 from rime_sdk.internal.utils import convert_dict_to_html, make_link
 from rime_sdk.job import ContinuousTestJob
 from rime_sdk.monitor import Monitor
 from rime_sdk.swagger import swagger_client
 from rime_sdk.swagger.swagger_client import (
     ApiClient,
+    ContinuoustestsFirewallIdUuidBody,
     FirewallFirewall,
     FirewallFirewallFirewallIdUuidBody,
     FirewallScheduledCTInfo,
-    RimeStartContinuousTestRequest,
     RimeUpdateFirewallResponse,
     RimeUUID,
     RuntimeinfoCustomImage,
     RuntimeinfoCustomImageType,
     RuntimeinfoResourceRequest,
     RuntimeinfoRunTimeInfo,
     TestrunTestRunIncrementalConfig,
@@ -494,16 +494,15 @@
             )
 
         if cpu_request_millicores is not None and cpu_request_millicores <= 0:
             raise ValueError(
                 "The requested number of millicores of CPU must be positive"
             )
 
-        req = RimeStartContinuousTestRequest(
-            firewall_id=RimeUUID(self._firewall_id),
+        req = ContinuoustestsFirewallIdUuidBody(
             test_run_incremental_config=TestrunTestRunIncrementalConfig(
                 eval_dataset_id=eval_data_id,
                 run_time_info=RuntimeinfoRunTimeInfo(
                     agent_id=RimeUUID(agent_id) if agent_id else None,
                     resource_request=RuntimeinfoResourceRequest(
                         ram_request_megabytes=ram_request_megabytes,
                         cpu_request_millicores=cpu_request_millicores,
@@ -523,9 +522,11 @@
                 managed_image_name=rime_managed_image
             )
         with RESTErrorHandler():
             Firewall._throttler.throttle(  # pylint: disable=W0212
                 throttling_msg="Your request is throttled to limit # of model tests."
             )
             api = swagger_client.ModelTestingApi(self._api_client)
-            job: RimeJobMetadata = api.model_testing_start_continuous_test(body=req).job
+            job: RimeJobMetadata = api.model_testing_start_continuous_test(
+                body=req, firewall_id_uuid=self._firewall_id,
+            ).job
         return ContinuousTestJob(self._api_client, job.job_id)
```

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/image_builder.py` & `rime_sdk-2.0.0rc7/rime_sdk/image_builder.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/internal/config_parser.py` & `rime_sdk-2.0.0rc7/rime_sdk/internal/config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/internal/constants.py` & `rime_sdk-2.0.0rc7/rime_sdk/internal/constants.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/internal/decorators.py` & `rime_sdk-2.0.0rc7/rime_sdk/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/internal/file_upload.py` & `rime_sdk-2.0.0rc7/rime_sdk/internal/file_upload.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/internal/rest_error_handler.py` & `rime_sdk-2.0.0rc7/rime_sdk/internal/rest_error_handler.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/internal/security_config_parser.py` & `rime_sdk-2.0.0rc7/rime_sdk/internal/security_config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/internal/swagger_parser.py` & `rime_sdk-2.0.0rc7/rime_sdk/internal/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/internal/swagger_utils.py` & `rime_sdk-2.0.0rc7/rime_sdk/internal/swagger_utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/internal/test_helpers.py` & `rime_sdk-2.0.0rc7/rime_sdk/internal/test_helpers.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/internal/throttle_queue.py` & `rime_sdk-2.0.0rc7/rime_sdk/internal/throttle_queue.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/internal/utils.py` & `rime_sdk-2.0.0rc7/rime_sdk/internal/utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/job.py` & `rime_sdk-2.0.0rc7/rime_sdk/job.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/monitor.py` & `rime_sdk-2.0.0rc7/rime_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/project.py` & `rime_sdk-2.0.0rc7/rime_sdk/project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/registry.py` & `rime_sdk-2.0.0rc7/rime_sdk/registry.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/__init__.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 # import ApiClient
 from rime_sdk.swagger.swagger_client.api_client import ApiClient
 from rime_sdk.swagger.swagger_client.configuration import Configuration
 # import models into sdk package
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_category_test_identifier import ArtifactIdentifierCategoryTestIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_subset_test_metric_identifier import ArtifactIdentifierSubsetTestMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_test_case_metric_identifier import ArtifactIdentifierTestCaseMetricIdentifier
+from rime_sdk.swagger.swagger_client.models.continuoustests_firewall_id_uuid_body import ContinuoustestsFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.create_agent_request_aws_config import CreateAgentRequestAWSConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_gcp_config import CreateAgentRequestGCPConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_local_config import CreateAgentRequestLocalConfig
 from rime_sdk.swagger.swagger_client.models.create_firewall_request_scheduled_ct_parameters import CreateFirewallRequestScheduledCTParameters
 from rime_sdk.swagger.swagger_client.models.custom_image_pull_secret import CustomImagePullSecret
 from rime_sdk.swagger.swagger_client.models.custom_metric_custom_metric_metadata import CustomMetricCustomMetricMetadata
 from rime_sdk.swagger.swagger_client.models.custommonitors_name_body import CustommonitorsNameBody
@@ -312,15 +313,14 @@
 from rime_sdk.swagger.swagger_client.models.rime_reset_password_response import RimeResetPasswordResponse
 from rime_sdk.swagger.swagger_client.models.rime_resolve_detection_event_response import RimeResolveDetectionEventResponse
 from rime_sdk.swagger.swagger_client.models.rime_safe_url import RimeSafeURL
 from rime_sdk.swagger.swagger_client.models.rime_send_ri_email_response import RimeSendRIEmailResponse
 from rime_sdk.swagger.swagger_client.models.rime_severity import RimeSeverity
 from rime_sdk.swagger.swagger_client.models.rime_severity_counts import RimeSeverityCounts
 from rime_sdk.swagger.swagger_client.models.rime_sort_spec import RimeSortSpec
-from rime_sdk.swagger.swagger_client.models.rime_start_continuous_test_request import RimeStartContinuousTestRequest
 from rime_sdk.swagger.swagger_client.models.rime_start_continuous_test_response import RimeStartContinuousTestResponse
 from rime_sdk.swagger.swagger_client.models.rime_start_file_scan_request import RimeStartFileScanRequest
 from rime_sdk.swagger.swagger_client.models.rime_start_file_scan_response import RimeStartFileScanResponse
 from rime_sdk.swagger.swagger_client.models.rime_start_stress_test_response import RimeStartStressTestResponse
 from rime_sdk.swagger.swagger_client.models.rime_store_datapoints_response import RimeStoreDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.rime_store_predictions_request_prediction import RimeStorePredictionsRequestPrediction
 from rime_sdk.swagger.swagger_client.models.rime_store_predictions_response import RimeStorePredictionsResponse
```

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/__init__.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/agent_manager_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/agent_manager_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/data_collector_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/data_collector_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/detection_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/detection_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/feature_flag_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/feature_flag_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/file_scanning_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/file_scanning_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/file_upload_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/file_upload_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/firewall_service_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/firewall_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/image_registry_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/image_registry_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/integration_service_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/integration_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/job_reader_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/job_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/model_card_service_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/model_card_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/model_testing_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/model_testing_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,53 +123,55 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def model_testing_start_continuous_test(self, body, **kwargs):  # noqa: E501
+    def model_testing_start_continuous_test(self, body, firewall_id_uuid, **kwargs):  # noqa: E501
         """StartContinuousTest  # noqa: E501
 
         Starts a Continuous Test and returns a Job object containing metadata for the Test Run.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.model_testing_start_continuous_test(body, async_req=True)
+        >>> thread = api.model_testing_start_continuous_test(body, firewall_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param RimeStartContinuousTestRequest body: (required)
+        :param ContinuoustestsFirewallIdUuidBody body: (required)
+        :param str firewall_id_uuid: Unique object ID. (required)
         :return: RimeStartContinuousTestResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.model_testing_start_continuous_test_with_http_info(body, **kwargs)  # noqa: E501
+            return self.model_testing_start_continuous_test_with_http_info(body, firewall_id_uuid, **kwargs)  # noqa: E501
         else:
-            (data) = self.model_testing_start_continuous_test_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.model_testing_start_continuous_test_with_http_info(body, firewall_id_uuid, **kwargs)  # noqa: E501
             return data
 
-    def model_testing_start_continuous_test_with_http_info(self, body, **kwargs):  # noqa: E501
+    def model_testing_start_continuous_test_with_http_info(self, body, firewall_id_uuid, **kwargs):  # noqa: E501
         """StartContinuousTest  # noqa: E501
 
         Starts a Continuous Test and returns a Job object containing metadata for the Test Run.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.model_testing_start_continuous_test_with_http_info(body, async_req=True)
+        >>> thread = api.model_testing_start_continuous_test_with_http_info(body, firewall_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param RimeStartContinuousTestRequest body: (required)
+        :param ContinuoustestsFirewallIdUuidBody body: (required)
+        :param str firewall_id_uuid: Unique object ID. (required)
         :return: RimeStartContinuousTestResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body']  # noqa: E501
+        all_params = ['body', 'firewall_id_uuid']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -180,18 +182,24 @@
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
             raise ValueError("Missing the required parameter `body` when calling `model_testing_start_continuous_test`")  # noqa: E501
+        # verify the required parameter 'firewall_id_uuid' is set
+        if ('firewall_id_uuid' not in params or
+                params['firewall_id_uuid'] is None):
+            raise ValueError("Missing the required parameter `firewall_id_uuid` when calling `model_testing_start_continuous_test`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'firewall_id_uuid' in params:
+            path_params['firewallId.uuid'] = params['firewall_id_uuid']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -207,15 +215,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1/continuous-tests', 'POST',
+            '/v1/continuous-tests/{firewallId.uuid}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='RimeStartContinuousTestResponse',  # noqa: E501
```

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/monitor_service_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/monitor_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/notification_setting_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/notification_setting_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/project_service_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/project_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/registry_service_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/registry_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/results_reader_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/results_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/rime_info_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/rime_info_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/user_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api/workspace_service_api.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/workspace_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/api_client.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/configuration.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/__init__.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from __future__ import absolute_import
 
 # import models into model package
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_category_test_identifier import ArtifactIdentifierCategoryTestIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_subset_test_metric_identifier import ArtifactIdentifierSubsetTestMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_test_case_metric_identifier import ArtifactIdentifierTestCaseMetricIdentifier
+from rime_sdk.swagger.swagger_client.models.continuoustests_firewall_id_uuid_body import ContinuoustestsFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.create_agent_request_aws_config import CreateAgentRequestAWSConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_gcp_config import CreateAgentRequestGCPConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_local_config import CreateAgentRequestLocalConfig
 from rime_sdk.swagger.swagger_client.models.create_firewall_request_scheduled_ct_parameters import CreateFirewallRequestScheduledCTParameters
 from rime_sdk.swagger.swagger_client.models.custom_image_pull_secret import CustomImagePullSecret
 from rime_sdk.swagger.swagger_client.models.custom_metric_custom_metric_metadata import CustomMetricCustomMetricMetadata
 from rime_sdk.swagger.swagger_client.models.custommonitors_name_body import CustommonitorsNameBody
@@ -287,15 +288,14 @@
 from rime_sdk.swagger.swagger_client.models.rime_reset_password_response import RimeResetPasswordResponse
 from rime_sdk.swagger.swagger_client.models.rime_resolve_detection_event_response import RimeResolveDetectionEventResponse
 from rime_sdk.swagger.swagger_client.models.rime_safe_url import RimeSafeURL
 from rime_sdk.swagger.swagger_client.models.rime_send_ri_email_response import RimeSendRIEmailResponse
 from rime_sdk.swagger.swagger_client.models.rime_severity import RimeSeverity
 from rime_sdk.swagger.swagger_client.models.rime_severity_counts import RimeSeverityCounts
 from rime_sdk.swagger.swagger_client.models.rime_sort_spec import RimeSortSpec
-from rime_sdk.swagger.swagger_client.models.rime_start_continuous_test_request import RimeStartContinuousTestRequest
 from rime_sdk.swagger.swagger_client.models.rime_start_continuous_test_response import RimeStartContinuousTestResponse
 from rime_sdk.swagger.swagger_client.models.rime_start_file_scan_request import RimeStartFileScanRequest
 from rime_sdk.swagger.swagger_client.models.rime_start_file_scan_response import RimeStartFileScanResponse
 from rime_sdk.swagger.swagger_client.models.rime_start_stress_test_response import RimeStartStressTestResponse
 from rime_sdk.swagger.swagger_client.models.rime_store_datapoints_response import RimeStoreDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.rime_store_predictions_request_prediction import RimeStorePredictionsRequestPrediction
 from rime_sdk.swagger.swagger_client.models.rime_store_predictions_response import RimeStorePredictionsResponse
```

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/dataset_dataset.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/dataset_dataset.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_detection_event.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_detail.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_event_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_resolution.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_resolution.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_custom_loader_location.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_custom_loader_location.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_data_collector_location.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_data_collector_location.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_data_location.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_data_location.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_delta_lake_location.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_delta_lake_location.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_location_args.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_location_args.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_location_params.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_location_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/googlerpc_status.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_level.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/model_model.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/model_model.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/model_model_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/model_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/model_model_path_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/model_model_path_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_threshold.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitor_transform.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_transform.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_digest_config.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_digest_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_notification_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_object_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_object_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_request.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_create_project_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_create_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_get_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_owner_details.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_project.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_project_with_owner_details.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_project_with_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_update_project_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_update_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_any.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_rca_result.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_rca_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_rca_role.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_rca_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/registry_metadata.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/registry_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/registry_validity_status.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/registry_validity_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_actor_role.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_actor_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_agent.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent_status.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_agent_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_archived_job_logs.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_archived_job_logs.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_metric.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_category_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_config_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_config_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_row.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_failing_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_feature_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_float_list.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_float_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -28,43 +28,53 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'monitor_id': 'RimeUUID',
         'monitor_name': 'str',
         'metric_name': 'str',
         'threshold': 'MonitorThreshold',
-        'data_points': 'list[RimeMonitorDataPoint]'
+        'data_points': 'list[RimeMonitorDataPoint]',
+        'description_html': 'str',
+        'long_description_tabs': 'list[RimeLongDescriptionTab]'
     }
 
     attribute_map = {
         'monitor_id': 'monitorId',
         'monitor_name': 'monitorName',
         'metric_name': 'metricName',
         'threshold': 'threshold',
-        'data_points': 'dataPoints'
+        'data_points': 'dataPoints',
+        'description_html': 'descriptionHtml',
+        'long_description_tabs': 'longDescriptionTabs'
     }
 
-    def __init__(self, monitor_id=None, monitor_name=None, metric_name=None, threshold=None, data_points=None):  # noqa: E501
+    def __init__(self, monitor_id=None, monitor_name=None, metric_name=None, threshold=None, data_points=None, description_html=None, long_description_tabs=None):  # noqa: E501
         """RimeGetMonitorResultResponse - a model defined in Swagger"""  # noqa: E501
         self._monitor_id = None
         self._monitor_name = None
         self._metric_name = None
         self._threshold = None
         self._data_points = None
+        self._description_html = None
+        self._long_description_tabs = None
         self.discriminator = None
         if monitor_id is not None:
             self.monitor_id = monitor_id
         if monitor_name is not None:
             self.monitor_name = monitor_name
         if metric_name is not None:
             self.metric_name = metric_name
         if threshold is not None:
             self.threshold = threshold
         if data_points is not None:
             self.data_points = data_points
+        if description_html is not None:
+            self.description_html = description_html
+        if long_description_tabs is not None:
+            self.long_description_tabs = long_description_tabs
 
     @property
     def monitor_id(self):
         """Gets the monitor_id of this RimeGetMonitorResultResponse.  # noqa: E501
 
 
         :return: The monitor_id of this RimeGetMonitorResultResponse.  # noqa: E501
@@ -167,14 +177,60 @@
 
         :param data_points: The data_points of this RimeGetMonitorResultResponse.  # noqa: E501
         :type: list[RimeMonitorDataPoint]
         """
 
         self._data_points = data_points
 
+    @property
+    def description_html(self):
+        """Gets the description_html of this RimeGetMonitorResultResponse.  # noqa: E501
+
+        Description of the monitor that may contain HTML.  # noqa: E501
+
+        :return: The description_html of this RimeGetMonitorResultResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._description_html
+
+    @description_html.setter
+    def description_html(self, description_html):
+        """Sets the description_html of this RimeGetMonitorResultResponse.
+
+        Description of the monitor that may contain HTML.  # noqa: E501
+
+        :param description_html: The description_html of this RimeGetMonitorResultResponse.  # noqa: E501
+        :type: str
+        """
+
+        self._description_html = description_html
+
+    @property
+    def long_description_tabs(self):
+        """Gets the long_description_tabs of this RimeGetMonitorResultResponse.  # noqa: E501
+
+        More detailed information about the monitor.  # noqa: E501
+
+        :return: The long_description_tabs of this RimeGetMonitorResultResponse.  # noqa: E501
+        :rtype: list[RimeLongDescriptionTab]
+        """
+        return self._long_description_tabs
+
+    @long_description_tabs.setter
+    def long_description_tabs(self, long_description_tabs):
+        """Sets the long_description_tabs of this RimeGetMonitorResultResponse.
+
+        More detailed information about the monitor.  # noqa: E501
+
+        :param long_description_tabs: The long_description_tabs of this RimeGetMonitorResultResponse.  # noqa: E501
+        :type: list[RimeLongDescriptionTab]
+        """
+
+        self._long_description_tabs = long_description_tabs
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_image_reference.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_image_reference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_int_list.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_int_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_integration_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_integration_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_data.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_data.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_view.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_view.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_feature.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_license_feature.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_limit.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_license_limit.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_limit_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_managed_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_card.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_task.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_task.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_named_double.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_named_double.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_order.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_order.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_safe_url.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_safe_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_request.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,42 +11,42 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeStartContinuousTestRequest(object):
+class ContinuoustestsFirewallIdUuidBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'firewall_id': 'RimeUUID',
+        'firewall_id': 'object',
         'test_run_incremental_config': 'TestrunTestRunIncrementalConfig',
         'override_existing_bins': 'bool',
         'experimental_fields': 'dict(str, object)'
     }
 
     attribute_map = {
         'firewall_id': 'firewallId',
         'test_run_incremental_config': 'testRunIncrementalConfig',
         'override_existing_bins': 'overrideExistingBins',
         'experimental_fields': 'experimentalFields'
     }
 
     def __init__(self, firewall_id=None, test_run_incremental_config=None, override_existing_bins=None, experimental_fields=None):  # noqa: E501
-        """RimeStartContinuousTestRequest - a model defined in Swagger"""  # noqa: E501
+        """ContinuoustestsFirewallIdUuidBody - a model defined in Swagger"""  # noqa: E501
         self._firewall_id = None
         self._test_run_incremental_config = None
         self._override_existing_bins = None
         self._experimental_fields = None
         self.discriminator = None
         if firewall_id is not None:
             self.firewall_id = firewall_id
@@ -55,93 +55,95 @@
         if override_existing_bins is not None:
             self.override_existing_bins = override_existing_bins
         if experimental_fields is not None:
             self.experimental_fields = experimental_fields
 
     @property
     def firewall_id(self):
-        """Gets the firewall_id of this RimeStartContinuousTestRequest.  # noqa: E501
+        """Gets the firewall_id of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
 
+        Uniquely specifies a Firewall.  # noqa: E501
 
-        :return: The firewall_id of this RimeStartContinuousTestRequest.  # noqa: E501
-        :rtype: RimeUUID
+        :return: The firewall_id of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
+        :rtype: object
         """
         return self._firewall_id
 
     @firewall_id.setter
     def firewall_id(self, firewall_id):
-        """Sets the firewall_id of this RimeStartContinuousTestRequest.
+        """Sets the firewall_id of this ContinuoustestsFirewallIdUuidBody.
 
+        Uniquely specifies a Firewall.  # noqa: E501
 
-        :param firewall_id: The firewall_id of this RimeStartContinuousTestRequest.  # noqa: E501
-        :type: RimeUUID
+        :param firewall_id: The firewall_id of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
+        :type: object
         """
 
         self._firewall_id = firewall_id
 
     @property
     def test_run_incremental_config(self):
-        """Gets the test_run_incremental_config of this RimeStartContinuousTestRequest.  # noqa: E501
+        """Gets the test_run_incremental_config of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
 
 
-        :return: The test_run_incremental_config of this RimeStartContinuousTestRequest.  # noqa: E501
+        :return: The test_run_incremental_config of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
         :rtype: TestrunTestRunIncrementalConfig
         """
         return self._test_run_incremental_config
 
     @test_run_incremental_config.setter
     def test_run_incremental_config(self, test_run_incremental_config):
-        """Sets the test_run_incremental_config of this RimeStartContinuousTestRequest.
+        """Sets the test_run_incremental_config of this ContinuoustestsFirewallIdUuidBody.
 
 
-        :param test_run_incremental_config: The test_run_incremental_config of this RimeStartContinuousTestRequest.  # noqa: E501
+        :param test_run_incremental_config: The test_run_incremental_config of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
         :type: TestrunTestRunIncrementalConfig
         """
 
         self._test_run_incremental_config = test_run_incremental_config
 
     @property
     def override_existing_bins(self):
-        """Gets the override_existing_bins of this RimeStartContinuousTestRequest.  # noqa: E501
+        """Gets the override_existing_bins of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
 
 
-        :return: The override_existing_bins of this RimeStartContinuousTestRequest.  # noqa: E501
+        :return: The override_existing_bins of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
         :rtype: bool
         """
         return self._override_existing_bins
 
     @override_existing_bins.setter
     def override_existing_bins(self, override_existing_bins):
-        """Sets the override_existing_bins of this RimeStartContinuousTestRequest.
+        """Sets the override_existing_bins of this ContinuoustestsFirewallIdUuidBody.
 
 
-        :param override_existing_bins: The override_existing_bins of this RimeStartContinuousTestRequest.  # noqa: E501
+        :param override_existing_bins: The override_existing_bins of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
         :type: bool
         """
 
         self._override_existing_bins = override_existing_bins
 
     @property
     def experimental_fields(self):
-        """Gets the experimental_fields of this RimeStartContinuousTestRequest.  # noqa: E501
+        """Gets the experimental_fields of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
 
         Fields that enable experimental functionality.  WARNING: these fields are experimental; ie, their functionality may not be reliable or backwards-compatible. Do not use these fields in production.  # noqa: E501
 
-        :return: The experimental_fields of this RimeStartContinuousTestRequest.  # noqa: E501
+        :return: The experimental_fields of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
         :rtype: dict(str, object)
         """
         return self._experimental_fields
 
     @experimental_fields.setter
     def experimental_fields(self, experimental_fields):
-        """Sets the experimental_fields of this RimeStartContinuousTestRequest.
+        """Sets the experimental_fields of this ContinuoustestsFirewallIdUuidBody.
 
         Fields that enable experimental functionality.  WARNING: these fields are experimental; ie, their functionality may not be reliable or backwards-compatible. Do not use these fields in production.  # noqa: E501
 
-        :param experimental_fields: The experimental_fields of this RimeStartContinuousTestRequest.  # noqa: E501
+        :param experimental_fields: The experimental_fields of this ContinuoustestsFirewallIdUuidBody.  # noqa: E501
         :type: dict(str, object)
         """
 
         self._experimental_fields = experimental_fields
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -160,15 +162,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeStartContinuousTestRequest, dict):
+        if issubclass(ContinuoustestsFirewallIdUuidBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -176,15 +178,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeStartContinuousTestRequest):
+        if not isinstance(other, ContinuoustestsFirewallIdUuidBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_str_list.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_str_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_subject_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_subject_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_suggestion.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_suggestion.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_table_column.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_tag.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_tag.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_termination_reason.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_termination_reason.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_time_interval.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_time_interval.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_token_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_token_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_role.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_uuid.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_uuid.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/role_users_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/role_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/role_workspace_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/role_workspace_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/schemanotification_config.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/schemanotification_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/statedb_job_status.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/statedb_job_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_connection_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_connection_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_category.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/user_private_info.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/user_private_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/user_role.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/user_user_detail.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/user_user_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/swagger/swagger_client/rest.py` & `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/test_batch.py` & `rime_sdk-2.0.0rc7/rime_sdk/test_batch.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk/test_run.py` & `rime_sdk-2.0.0rc7/rime_sdk/test_run.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc6/rime_sdk.egg-info/SOURCES.txt` & `rime_sdk-2.0.0rc7/rime_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 rime_sdk/swagger/swagger_client/api/rime_info_api.py
 rime_sdk/swagger/swagger_client/api/user_api.py
 rime_sdk/swagger/swagger_client/api/workspace_service_api.py
 rime_sdk/swagger/swagger_client/models/__init__.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
 rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
 rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
 rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
 rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
 rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
 rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
@@ -336,15 +337,14 @@
 rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
 rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
 rime_sdk/swagger/swagger_client/models/rime_safe_url.py
 rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
 rime_sdk/swagger/swagger_client/models/rime_severity.py
 rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
 rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
-rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_request.py
 rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
 rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
 rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
 rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
 rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
 rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
 rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
```

### Comparing `rime_sdk-2.0.0rc6/setup.py` & `rime_sdk-2.0.0rc7/setup.py`

 * *Files identical despite different names*

