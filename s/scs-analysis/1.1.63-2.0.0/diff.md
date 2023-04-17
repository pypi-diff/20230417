# Comparing `tmp/scs-analysis-1.1.63.tar.gz` & `tmp/scs-analysis-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs-analysis-1.1.63.tar", last modified: Mon Mar 20 10:13:02 2023, max compression
+gzip compressed data, was "scs-analysis-2.0.0.tar", last modified: Mon Apr 17 09:23:19 2023, max compression
```

## Comparing `scs-analysis-1.1.63.tar` & `scs-analysis-2.0.0.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:13:02.880317 scs-analysis-1.1.63/
--rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/LICENSE
--rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/MANIFEST.in
--rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-03-20 10:13:02.880317 scs-analysis-1.1.63/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)      766 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/README.md
--rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/README.rst
--rw-rw-r--   0 jade      (1002) jade      (1002)      235 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/requirements.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-03-20 10:13:02.880317 scs-analysis-1.1.63/setup.cfg
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5452 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/setup.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:13:02.864319 scs-analysis-1.1.63/src/
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:13:02.872318 scs-analysis-1.1.63/src/scs_analysis/
--rwxrwxr-x   0 jade      (1002) jade      (1002)      184 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/__init__.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2466 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/access_key.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     8568 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/alert.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3559 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/alert_status.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2235 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/aws_api_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4536 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/aws_byline.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2655 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/aws_client_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7224 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/aws_mqtt_client.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7385 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/aws_mqtt_control.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6971 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/aws_topic_history.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2139 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/aws_topic_publisher.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2918 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/aws_upload_interval.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)    15307 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/baseline.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5964 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/baseline_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:13:02.872318 scs-analysis-1.1.63/src/scs_analysis/chart/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/chart/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1630 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/chart/chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4353 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/chart/histo_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4149 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/chart/multi_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4128 2022-09-20 10:07:36.000000 scs-analysis-1.1.63/src/scs_analysis/chart/single_chart.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:13:02.880317 scs-analysis-1.1.63/src/scs_analysis/cmd/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1966 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_access_key.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7915 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_alert.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3474 2022-09-20 10:07:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_alert_status.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2713 2022-11-09 12:09:25.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_aws_api_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3826 2022-11-09 12:09:25.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_aws_byline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3092 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_aws_client_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7868 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_aws_topic_history.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1522 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7223 2022-09-20 10:07:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6605 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_baseline_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4498 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_cognito_devices.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2943 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_cognito_password.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3570 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3183 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_cognito_user_identity.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7027 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_cognito_users.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5051 2022-09-20 10:07:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_configuration_csv.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4330 2022-09-20 10:07:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_configuration_monitor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4076 2022-09-20 10:07:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3321 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_csv_collation_summary.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2867 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_csv_collator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3410 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_csv_join.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2774 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_csv_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2761 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_csv_segmentor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3372 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_csv_writer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4066 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_histo_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3039 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_localised_datetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2011 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_monitor_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5603 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_mqtt_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4622 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_mqtt_control.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6780 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_mqtt_peers.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3378 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_multi_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3490 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_node.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5404 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_organisation_devices.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4190 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_organisation_path_roots.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4489 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_organisation_user_paths.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6422 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_organisation_users.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4992 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_organisations.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1931 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_osio_api_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2265 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_osio_client_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1571 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_osio_topic.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3892 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_osio_topic_history.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2678 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_osio_topic_publisher.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3560 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_aggregate.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3536 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_collator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2628 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_concentration.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2813 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_distance.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1875 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_duplicates.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3020 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_error.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1677 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_filter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1688 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_interval.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4763 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_iso_8601.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_low_pass.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2312 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_median.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2782 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_nullify.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1224 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_paths.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1579 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_record.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3898 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_slope.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1577 2022-09-20 10:07:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_sort.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3100 2022-09-20 10:07:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_stats.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5204 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_subset.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2264 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_tally.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_time_shift.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2325 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_timezone.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3701 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_single_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1441 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_socket_receiver.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1540 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_uds.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5919 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/cognito_devices.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5678 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/cognito_password.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5384 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/cognito_user_credentials.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7784 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/cognito_user_identity.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7885 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/cognito_users.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7280 2022-09-20 10:07:36.000000 scs-analysis-1.1.63/src/scs_analysis/configuration_csv.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3362 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/configuration_monitor.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3697 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/configuration_monitor_check.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6401 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/csv_collation_summary.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3967 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/csv_collator.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6835 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/csv_join.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5065 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/csv_reader.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4697 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/csv_segmentor.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3800 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/csv_writer.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:13:02.880317 scs-analysis-1.1.63/src/scs_analysis/handler/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/handler/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4051 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/handler/aws_mqtt_publisher.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2329 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/handler/batch_download_reporter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1436 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/handler/configuration_csv_generator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/handler/csv_collator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5893 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/handler/csv_segmentor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1184 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/handler/mqtt_reporter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1552 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/handler/osio_mqtt_client_handler.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1622 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/handler/osio_mqtt_control_handler.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2007 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/handler/sample_midpoint.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/handler/sample_regression.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4308 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/histo_chart.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2127 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/localised_datetime.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2544 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/monitor_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6301 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/mqtt_peers.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4367 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/multi_chart.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5982 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/node.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6258 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/organisation_devices.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4749 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/organisation_path_roots.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5181 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/organisation_user_paths.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6112 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/organisation_users.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5656 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/organisations.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1637 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/osio_api_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4951 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/osio_client_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5808 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/osio_mqtt_client.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6563 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/osio_mqtt_control.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3912 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/osio_topic_history.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3738 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/osio_topic_publisher.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7233 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/sample_aggregate.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4822 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/sample_average.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5162 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/sample_collator.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5566 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/sample_concentration.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3970 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/sample_distance.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3598 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/sample_duplicates.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4685 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/sample_error.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3103 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/sample_interval.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7990 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/sample_iso_8601.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3803 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/sample_low_pass.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3572 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/sample_max.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3777 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/sample_median.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3530 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/sample_midpoint.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3571 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/sample_min.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5072 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/sample_noise.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4017 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/sample_nullify.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1667 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/sample_paths.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3321 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/sample_regression.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5711 2023-03-20 10:12:25.000000 scs-analysis-1.1.63/src/scs_analysis/sample_slope.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2502 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/sample_sort.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5928 2022-09-20 10:07:36.000000 scs-analysis-1.1.63/src/scs_analysis/sample_stats.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6001 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/sample_subset.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2897 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/sample_time_shift.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4732 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/sample_timezone.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4463 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/single_chart.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2451 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/socket_receiver.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1891 2023-02-06 14:01:57.000000 scs-analysis-1.1.63/src/scs_analysis/timer.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1849 2022-08-17 09:53:36.000000 scs-analysis-1.1.63/src/scs_analysis/uds_receiver.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:13:02.872318 scs-analysis-1.1.63/src/scs_analysis.egg-info/
--rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-03-20 10:13:02.000000 scs-analysis-1.1.63/src/scs_analysis.egg-info/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)     6489 2023-03-20 10:13:02.000000 scs-analysis-1.1.63/src/scs_analysis.egg-info/SOURCES.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-03-20 10:13:02.000000 scs-analysis-1.1.63/src/scs_analysis.egg-info/dependency_links.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)      250 2023-03-20 10:13:02.000000 scs-analysis-1.1.63/src/scs_analysis.egg-info/requires.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)       13 2023-03-20 10:13:02.000000 scs-analysis-1.1.63/src/scs_analysis.egg-info/top_level.txt
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-04-17 09:23:19.674593 scs-analysis-2.0.0/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/LICENSE
+-rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/MANIFEST.in
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-04-17 09:23:19.674593 scs-analysis-2.0.0/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)      766 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/README.md
+-rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/README.rst
+-rw-rw-r--   0 jade      (1002) jade      (1002)      235 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/requirements.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-04-17 09:23:19.674593 scs-analysis-2.0.0/setup.cfg
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5453 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/setup.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-04-17 09:23:19.642593 scs-analysis-2.0.0/src/
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-04-17 09:23:19.658594 scs-analysis-2.0.0/src/scs_analysis/
+-rwxrwxr-x   0 jade      (1002) jade      (1002)      183 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/__init__.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2467 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/access_key.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     8568 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/alert.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3559 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/alert_status.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2235 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/aws_api_auth.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4536 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/aws_byline.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2655 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/aws_client_auth.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7224 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/aws_mqtt_client.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7386 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/aws_mqtt_control.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6971 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/aws_topic_history.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2139 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/aws_topic_publisher.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2918 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/aws_upload_interval.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)    15290 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/baseline.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5964 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/baseline_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-04-17 09:23:19.658594 scs-analysis-2.0.0/src/scs_analysis/chart/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/chart/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1630 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/chart/chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4546 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/chart/histo_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4249 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/chart/multi_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4317 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/chart/single_chart.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-04-17 09:23:19.670593 scs-analysis-2.0.0/src/scs_analysis/cmd/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1966 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_access_key.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7915 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_alert.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3474 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_alert_status.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2713 2022-11-09 12:09:25.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_api_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3826 2022-11-09 12:09:25.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_byline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3092 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_client_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7868 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_topic_history.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1522 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7223 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6605 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_baseline_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4498 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_devices.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2943 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_password.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3570 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3183 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_user_identity.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7027 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_users.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5051 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_configuration_csv.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4330 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_configuration_monitor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4076 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3321 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_collation_summary.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2867 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_collator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3410 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_join.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2774 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2761 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_segmentor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3372 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_writer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4066 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_histo_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3039 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_localised_datetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2011 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_monitor_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5603 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_mqtt_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4622 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_mqtt_control.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6780 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_mqtt_peers.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3378 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_multi_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3490 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_node.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5404 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisation_devices.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4524 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisation_path_roots.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4630 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisation_user_paths.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6422 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisation_users.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4992 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisations.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1931 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_api_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2265 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_client_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1571 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_topic.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3892 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_topic_history.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2678 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_topic_publisher.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3560 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_aggregate.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3536 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_collator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2628 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_concentration.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2813 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_distance.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2189 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_duplicates.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3020 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_error.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1677 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_filter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1688 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_interval.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4763 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_iso_8601.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_low_pass.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2312 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_median.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2782 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_nullify.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1224 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_paths.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1579 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_record.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3899 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_slope.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1577 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_sort.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3100 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_stats.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5204 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_subset.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2264 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_tally.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_time_shift.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2325 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_timezone.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3701 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_single_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1441 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_socket_receiver.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1540 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_uds.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5870 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cognito_devices.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5742 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cognito_password.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5459 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cognito_user_credentials.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     8074 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cognito_user_identity.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     8110 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cognito_users.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7280 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/configuration_csv.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3362 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/configuration_monitor.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3697 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/configuration_monitor_check.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6401 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/csv_collation_summary.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3967 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/csv_collator.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6835 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/csv_join.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5065 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/csv_reader.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4697 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/csv_segmentor.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3800 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/csv_writer.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-04-17 09:23:19.674593 scs-analysis-2.0.0/src/scs_analysis/handler/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4051 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/handler/aws_mqtt_publisher.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2329 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/batch_download_reporter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1436 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/configuration_csv_generator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/csv_collator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5893 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/csv_segmentor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1184 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/mqtt_reporter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1552 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/osio_mqtt_client_handler.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1622 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/osio_mqtt_control_handler.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2007 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/sample_midpoint.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/sample_regression.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4308 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/histo_chart.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2127 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/localised_datetime.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2544 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/monitor_auth.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6301 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/mqtt_peers.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4367 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/multi_chart.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5982 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/node.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6237 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/organisation_devices.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5053 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/organisation_path_roots.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5266 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/organisation_user_paths.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6124 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/organisation_users.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5640 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/organisations.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1637 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/osio_api_auth.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4951 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/osio_client_auth.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5808 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/osio_mqtt_client.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6563 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/osio_mqtt_control.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3912 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/osio_topic_history.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3738 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/osio_topic_publisher.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7233 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/sample_aggregate.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4822 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_average.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5162 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_collator.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5566 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_concentration.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3970 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/sample_distance.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3765 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/sample_duplicates.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4685 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_error.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3103 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_interval.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7990 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_iso_8601.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3803 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_low_pass.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3572 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_max.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3777 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_median.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3530 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_midpoint.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3571 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_min.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5072 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/sample_noise.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4017 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_nullify.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1667 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/sample_paths.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3321 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/sample_regression.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5707 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/sample_slope.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2502 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_sort.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5928 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/sample_stats.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6001 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_subset.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2897 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_time_shift.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4732 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/sample_timezone.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4463 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/single_chart.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2451 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/socket_receiver.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1891 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/timer.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1849 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/uds_receiver.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-04-17 09:23:19.658594 scs-analysis-2.0.0/src/scs_analysis.egg-info/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-04-17 09:23:19.000000 scs-analysis-2.0.0/src/scs_analysis.egg-info/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6489 2023-04-17 09:23:19.000000 scs-analysis-2.0.0/src/scs_analysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-04-17 09:23:19.000000 scs-analysis-2.0.0/src/scs_analysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)      250 2023-04-17 09:23:19.000000 scs-analysis-2.0.0/src/scs_analysis.egg-info/requires.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)       13 2023-04-17 09:23:19.000000 scs-analysis-2.0.0/src/scs_analysis.egg-info/top_level.txt
```

### Comparing `scs-analysis-1.1.63/LICENSE` & `scs-analysis-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/PKG-INFO` & `scs-analysis-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 1.1.63
+Version: 2.0.0
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `scs-analysis-1.1.63/README.md` & `scs-analysis-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/setup.py` & `scs-analysis-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/south-coast-science/scs_analysis",
     package_dir={'': 'src'},
     packages=setuptools.find_packages('src'),
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows :: Windows 10",
         "Operating System :: POSIX",
     ],
     scripts=[
         'src/scs_analysis/access_key.py',
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/access_key.py` & `scs-analysis-2.0.0/src/scs_analysis/access_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
         else:
             password = AccessKey.password_from_user()
 
             try:
                 access_key = AccessKey.load(Host, encryption_key=password)
             except (KeyError, ValueError):
-                logger.error("incorrect password")
+                logger.error("incorrect password.")
                 exit(1)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # end...
 
         if access_key:
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/alert.py` & `scs-analysis-2.0.0/src/scs_analysis/alert.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/alert_status.py` & `scs-analysis-2.0.0/src/scs_analysis/alert_status.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/aws_api_auth.py` & `scs-analysis-2.0.0/src/scs_analysis/aws_api_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/aws_byline.py` & `scs-analysis-2.0.0/src/scs_analysis/aws_byline.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/aws_client_auth.py` & `scs-analysis-2.0.0/src/scs_analysis/aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/aws_mqtt_client.py` & `scs-analysis-2.0.0/src/scs_analysis/aws_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/aws_mqtt_control.py` & `scs-analysis-2.0.0/src/scs_analysis/aws_mqtt_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             if not AccessKey.exists(Host):
                 logger.error("AccessKey not available.")
                 exit(1)
 
             try:
                 key = AccessKey.load(Host, encryption_key=AccessKey.password_from_user())
             except (KeyError, ValueError):
-                logger.error("incorrect password")
+                logger.error("incorrect password.")
                 exit(1)
 
             s3_client = Client.construct('s3', key)
             s3_resource_client = Client.resource('s3', key)
 
             manager = S3PersistenceManager(s3_client, s3_resource_client)
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/aws_topic_history.py` & `scs-analysis-2.0.0/src/scs_analysis/aws_topic_history.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/aws_topic_publisher.py` & `scs-analysis-2.0.0/src/scs_analysis/aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/aws_upload_interval.py` & `scs-analysis-2.0.0/src/scs_analysis/aws_upload_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/baseline.py` & `scs-analysis-2.0.0/src/scs_analysis/baseline.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,14 @@
 # TODO: review Ox handling
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     MQTT_TIMEOUT = 60           # seconds
 
-    logger = None
     key = None
     monitor_auth = None
     mqtt_client = None
 
     processed_count = 0
 
     # ----------------------------------------------------------------------------------------------------------------
@@ -123,15 +122,15 @@
         if not AccessKey.exists(Host):
             logger.error("AccessKey not available.")
             exit(1)
 
         try:
             key = AccessKey.load(Host, encryption_key=AccessKey.password_from_user())
         except (KeyError, ValueError):
-            logger.error("incorrect password")
+            logger.error("incorrect password.")
             exit(1)
 
         # APIAuth (for MessageManager)...
         api_auth = APIAuth.load(Host)
 
         if api_auth is None:
             logger.error("APIAuth is not available")
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/baseline_conf.py` & `scs-analysis-2.0.0/src/scs_analysis/baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/chart/chart.py` & `scs-analysis-2.0.0/src/scs_analysis/chart/chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/chart/histo_chart.py` & `scs-analysis-2.0.0/src/scs_analysis/chart/histo_chart.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 source repo: scs_analysis
 
 uses matplotlibrc configuration file
 
 https://matplotlib.org/faq/usage_faq.html
 https://stackoverflow.com/questions/28269157/plotting-in-a-non-blocking-way-with-matplotlib?noredirect=1&lq=1
 http://bastibe.de/2013-05-30-speeding-up-matplotlib.html
+
+Deprecation warnings with Matplotlib 3.4 #383
+https://github.com/raysect/source/issues/383
 """
 
 from matplotlib import pyplot as plt
 from matplotlib.ticker import MaxNLocator
 
 from scs_analysis.chart.chart import Chart
 
@@ -45,15 +48,16 @@
         self.__outfile = outfile
 
         # histo...
         self.__histogram = Histogram(x_min, x_max, bin_count, precision, path)
 
         # plotter...
         self.__fig, self.__ax = plt.subplots()
-        self.__fig.canvas.set_window_title(self.title(path))
+        # self.__fig.canvas.set_window_title(self.title(path))                  # deprecated
+        self.__fig.canvas.manager.set_window_title(self.title(path))
         self.__fig.tight_layout()
 
         self.__fig.canvas.mpl_connect('close_event', self.close)
 
         self.__ax.set(xlim=[self.__x_min, self.__x_max], ylim=[0, self.__y_max])
         self.__ax.yaxis.set_major_locator(MaxNLocator(integer=True))
         self.__ax.yaxis.grid(True)
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/chart/multi_chart.py` & `scs-analysis-2.0.0/src/scs_analysis/chart/multi_chart.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 source repo: scs_analysis
 
 uses matplotlibrc configuration file
 
 https://matplotlib.org/faq/usage_faq.html
 https://stackoverflow.com/questions/28269157/plotting-in-a-non-blocking-way-with-matplotlib?noredirect=1&lq=1
+
+Deprecation warnings with Matplotlib 3.4 #383
+https://github.com/raysect/source/issues/383
 """
 
 from matplotlib import pyplot as plt
 
 from scs_analysis.chart.chart import Chart
 
 
@@ -38,15 +41,15 @@
         # data...
         self.__x_data = range(x_count)
 
         self.__y_data = self.__init_data(x_count)
 
         # plotter...
         fig = plt.figure()
-        fig.canvas.set_window_title(self.title(', '.join(self.__paths)))
+        fig.canvas.manager.set_window_title(self.title(', '.join(self.__paths)))
         fig.tight_layout()
 
         fig.canvas.mpl_connect('close_event', self.close)
 
         ax1 = plt.axes()
         ax1.xaxis.grid(True)
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/chart/single_chart.py` & `scs-analysis-2.0.0/src/scs_analysis/chart/single_chart.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 uses matplotlibrc configuration file
 
 https://matplotlib.org/faq/usage_faq.html
 https://matplotlib.org/stable/users/interactive_guide.html
 https://stackoverflow.com/questions/28269157/plotting-in-a-non-blocking-way-with-matplotlib?noredirect=1&lq=1
 http://physicalmodelingwithpython.blogspot.com/2015/07/raising-figure-window-to-foreground.html
+
+Deprecation warnings with Matplotlib 3.4 #383
+https://github.com/raysect/source/issues/383
 """
 
 from matplotlib import pyplot as plt
 
 from scs_analysis.chart.chart import Chart
 
 
@@ -43,15 +46,16 @@
         self.__first_datum = None
 
         initial_datum = 0 if is_relative else y_min
         self.__y_data = [initial_datum] * x_count
 
         # plotter...
         fig = plt.figure()
-        fig.canvas.set_window_title(self.title(path))
+        # fig.canvas.set_window_title(self.title(path))                     # deprecated
+        fig.canvas.manager.set_window_title(self.title(path))
         fig.tight_layout()
 
         fig.canvas.mpl_connect('close_event', self.close)
 
         ax1 = plt.axes()
         ax1.xaxis.grid(True)
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_access_key.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_access_key.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_alert.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_alert.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_alert_status.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_alert_status.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_aws_api_auth.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_api_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_aws_byline.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_byline.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_aws_client_auth.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_aws_topic_history.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_topic_history.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_aws_topic_publisher.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_baseline.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_baseline_conf.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_cognito_devices.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_devices.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_cognito_password.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_password.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_cognito_user_credentials.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_user_credentials.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_cognito_user_identity.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_user_identity.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_cognito_users.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_configuration_csv.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_configuration_csv.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_configuration_monitor.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_configuration_monitor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_configuration_monitor_check.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_configuration_monitor_check.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_csv_collation_summary.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_csv_collator.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_csv_join.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_join.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_csv_reader.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_csv_segmentor.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_csv_writer.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_histo_chart.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_localised_datetime.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_localised_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_monitor_auth.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_mqtt_client.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_mqtt_control.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_mqtt_control.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_mqtt_peers.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_mqtt_peers.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_multi_chart.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_node.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_node.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_organisation_devices.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisation_devices.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_organisation_path_roots.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisation_path_roots.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 class CmdOrganisationPathRoots(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] { -F -l ORG_LABEL | "
+        self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] { -F [-l ORG_LABEL] | "
                                                     "-C -l ORG_LABEL -r PATH_ROOT | "
                                                     "-D -l ORG_LABEL -r PATH_ROOT } "
-                                                    "[-i INDENT] [-v]", version="%prog 1.0")
+                                                    "[-m] [-i INDENT] [-v]", version="%prog 1.0")
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
@@ -39,14 +39,17 @@
         self.__parser.add_option("--org-label", "-l", type="string", action="store", dest="org_label",
                                  help="the organisation label")
 
         self.__parser.add_option("--path-root", "-r", type="string", action="store", dest="path_root",
                                  help="the organisation path root")
 
         # output...
+        self.__parser.add_option("--memberships", "-m", action="store_true", dest="memberships", default=False,
+                                 help="show path root's user path memberships")
+
         self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
@@ -65,15 +68,15 @@
 
         if self.delete:
             count += 1
 
         if count != 1:
             return False
 
-        if self.org_label is None:
+        if not self.find and self.org_label is None:
             return False
 
         if (self.create or self.delete) and self.path_root is None:
             return False
 
         return True
 
@@ -107,14 +110,19 @@
 
     @property
     def path_root(self):
         return self.__opts.path_root
 
 
     @property
+    def memberships(self):
+        return self.__opts.memberships
+
+
+    @property
     def indent(self):
         return self.__opts.indent
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
@@ -124,10 +132,10 @@
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
         return "CmdOrganisationPathRoots:{credentials_name:%s, find:%s, create:%s, delete:%s, " \
-               "org_label:%s, path_root:%s, indent:%s, verbose:%s}" % \
+               "org_label:%s, path_root:%s, memberships:%s, indent:%s, verbose:%s}" % \
                (self.credentials_name, self.find, self.__opts.create, self.__opts.delete,
-                self.org_label, self.path_root, self.indent, self.verbose)
+                self.org_label, self.path_root, self.memberships, self.indent, self.verbose)
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_organisation_user_paths.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisation_user_paths.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class CmdOrganisationUserPaths(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] { -F -e EMAIL -r PATH_ROOT | "
+        self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] { -F { -e EMAIL | -r PATH_ROOT } | "
                                                     "-C -e EMAIL -r PATH_ROOT -x PATH_EXTENSION | "
                                                     "-D -e EMAIL -r PATH_ROOT -x PATH_EXTENSION } "
                                                     "[-i INDENT] [-v]", version="%prog 1.0")
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
@@ -68,16 +68,20 @@
 
         if self.delete:
             count += 1
 
         if count != 1:
             return False
 
-        if self.email is None or self.path_root is None:
-            return False
+        if self.find:
+            if self.email is None and self.path_root is None:
+                return False
+        else:
+            if self.email is None or self.path_root is None:
+                return False
 
         if (self.create or self.delete) and self.path_extension is None:
             return False
 
         return True
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_organisation_users.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisation_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_organisations.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisations.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_osio_api_auth.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_api_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_osio_client_auth.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_osio_topic.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_topic.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_osio_topic_history.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_topic_history.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_osio_topic_publisher.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_aggregate.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_collator.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_concentration.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_concentration.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_distance.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_distance.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_duplicates.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_record.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,48 @@
 """
-Created on 3 Mar 2019
+Created on 11 Jul 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleDuplicates(object):
+class CmdSampleRecord(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-c] [-v] PATH", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [-v] [PATH]", version="%prog 1.0")
 
         # optional...
-        self.__parser.add_option("--counts", "-c", action="store_true", dest="counts", default=False,
-                                 help="only list the count of matching documents")
-
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if len(self.__args) != 1:
+        if self.path is None:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def counts(self):
-        return self.__opts.counts
-
-
-    @property
     def verbose(self):
         return self.__opts.verbose
 
 
     @property
     def path(self):
         return self.__args[0] if len(self.__args) > 0 else None
@@ -59,8 +51,8 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSampleDuplicates:{counts:%s, verbose:%s, path:%s}" % (self.counts, self.verbose, self.path)
+        return "CmdSampleRecord:{verbose:%s, path:%s}" % (self.verbose, self.path)
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_error.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_error.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_filter.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_filter.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_interval.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_iso_8601.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_low_pass.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_low_pass.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_median.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_median.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_nullify.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_nullify.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_paths.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_record.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_uds.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
-Created on 11 Jul 2016
+Created on 25 Apr 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleRecord(object):
+class CmdUDS(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-v] [PATH]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [-v] UDS_SUB", version="%prog 1.0")
 
         # optional...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
@@ -35,24 +35,24 @@
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def verbose(self):
-        return self.__opts.verbose
+    def path(self):
+        return self.__args[0] if len(self.__args) > 0 else None
 
 
     @property
-    def path(self):
-        return self.__args[0] if len(self.__args) > 0 else None
+    def verbose(self):
+        return self.__opts.verbose
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSampleRecord:{verbose:%s, path:%s}" % (self.verbose, self.path)
+        return "CmdUDS:{verbose:%s}" % self.verbose
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_slope.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_slope.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self.__parser.add_option("--iso-path", "-i", type="string", nargs=1, action="store", default="rec", dest="iso",
                                  help="path for ISO 8601 datetime field (default 'rec')")
 
         self.__parser.add_option("--tally", "-t", type="int", nargs=1, action="store", default=2, dest="tally",
                                  help="compute for rolling TALLY number of data points (default 2)")
 
         self.__parser.add_option("--max-interval", "-m", type="string", nargs=1, action="store", dest="max_interval",
-                                 help="restart regresson on long intervals")
+                                 help="restart regression on long intervals")
 
         self.__parser.add_option("--exclude-incomplete", "-x", action="store_true", dest="exclude_incomplete",
                                  default=False, help="exclude incomplete tallies")
 
         self.__parser.add_option("--prec", "-p", type="int", nargs=1, action="store", default=6, dest="precision",
                                  help="precision (default 6 decimal places)")
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_sort.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_stats.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_subset.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_tally.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_tally.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_time_shift.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_sample_timezone.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_timezone.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_single_chart.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_socket_receiver.py` & `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_socket_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cmd/cmd_uds.py` & `scs-analysis-2.0.0/src/scs_analysis/handler/mqtt_reporter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,45 @@
 """
-Created on 25 Apr 2017
+Created on 6 Jul 2018
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
-import optparse
+import sys
+
+from scs_core.data.datetime import LocalizedDatetime
 
 
 # --------------------------------------------------------------------------------------------------------------------
+# reporter...
+
+class MQTTReporter(object):
+    """
+    classdocs
+    """
 
-class CmdUDS(object):
-    """unix command line handler"""
+    # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self):
+    def __init__(self, verbose):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-v] UDS_SUB", version="%prog 1.0")
-
-        # optional...
-        self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
-                                 help="report narrative to stderr")
-
-        self.__opts, self.__args = self.__parser.parse_args()
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    def is_valid(self):
-        if self.path is None:
-            return False
-
-        return True
+        self.__verbose = verbose
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    @property
-    def path(self):
-        return self.__args[0] if len(self.__args) > 0 else None
-
-
-    @property
-    def verbose(self):
-        return self.__opts.verbose
+    def print(self, status):
+        if not self.__verbose:
+            return
+
+        now = LocalizedDatetime.now().utc()
+        print("%s:         mqtt: %s" % (now.as_time(), status), file=sys.stderr)
+        sys.stderr.flush()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def print_help(self, file):
-        self.__parser.print_help(file)
-
-
     def __str__(self, *args, **kwargs):
-        return "CmdUDS:{verbose:%s}" % self.verbose
+        return "MQTTReporter:{verbose:%s}" % self.__verbose
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cognito_devices.py` & `scs-analysis-2.0.0/src/scs_analysis/cognito_devices.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,45 +11,46 @@
 The cognito_users utility is used to create, update and retrieve AWS Cognito identities. This utility can only be used
 by organisation administrators and superusers.
 
 If the --Create function is used, an email is sent to the new user. The verification link in the email must be
 excercised in order for the account to gain a CONFIRMED status.
 
 SYNOPSIS
-cognito_devices.py  [-c CREDENTIALS] { -F [-t TAG] | -C TAG SHARED_SECRET | -U TAG SHARED_SECRET | -D TAG }
+cognito_devices.py  [-c CREDENTIALS] { -F [-t TAG] [-m] | -C TAG SHARED_SECRET | -U TAG SHARED_SECRET | -D TAG } \
 [-i INDENT] [-v]
 
 EXAMPLES
-cognito_users.py -Fe bruno.beloff@southcoastscience.com
+cognito_devices.py -vi4 -c super -F -m
 
 DOCUMENT EXAMPLE
-{"username": "8", "creation-date": "2021-11-24T12:51:12Z", "confirmation-status": "CONFIRMED", "enabled": true,
-"email": "bruno.beloff@southcoastscience.com", "given-name": "Bruno", "family-name": "Beloff", "is-super": true}
+{"username": "scs-ph1-28", "created": "2023-04-04T09:08:55Z", "last-updated": "2023-04-04T09:08:56Z"}
 
 SEE ALSO
 scs_analysis/cognito_credentials
+scs_analysis/cognito_users
+scs_analysis/organisation_devices
 
 RESOURCES
 https://docs.aws.amazon.com/cognito/latest/developerguide/signing-up-users-in-your-app.html
 https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-settings-policies.html
 """
 
 import requests
 import sys
 
 from scs_analysis.cmd.cmd_cognito_devices import CmdCognitoDevices
 
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_device import CognitoDeviceIdentity
 from scs_core.aws.security.cognito_device_finder import CognitoDeviceFinder
 from scs_core.aws.security.cognito_device_manager import CognitoDeviceManager
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
 from scs_core.aws.security.cognito_membership import CognitoMembership
-from scs_core.aws.security.organisation_manager import OrganisationManager
 
-from scs_core.aws.security.cognito_user import CognitoUserCredentials
+from scs_core.aws.security.organisation_manager import OrganisationManager
 
 from scs_core.data.json import JSONify
 
 from scs_core.sys.http_exception import HTTPConflictException
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
@@ -83,23 +84,23 @@
 
         # ------------------------------------------------------------------------------------------------------------
         # auth...
 
         gatekeeper = CognitoLoginManager(requests)
 
         # CognitoUserCredentials...
-        if not CognitoUserCredentials.exists(Host, name=cmd.credentials_name):
+        if not CognitoClientCredentials.exists(Host, name=cmd.credentials_name):
             logger.error("Cognito credentials not available.")
             exit(1)
 
         try:
-            password = CognitoUserCredentials.password_from_user()
-            credentials = CognitoUserCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
+            password = CognitoClientCredentials.password_from_user()
+            credentials = CognitoClientCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
         except (KeyError, ValueError):
-            logger.error("incorrect password")
+            logger.error("incorrect password.")
             exit(1)
 
         auth = gatekeeper.user_login(credentials)
 
         if not auth.is_ok():
             logger.error("login: %s" % auth.authentication_status.description)
             exit(1)
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cognito_password.py` & `scs-analysis-2.0.0/src/scs_analysis/cognito_password.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,18 @@
 """
 
 import requests
 import sys
 
 from scs_analysis.cmd.cmd_cognito_password import CmdCognitoPassword
 
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager, AuthenticationStatus
-from scs_core.aws.security.cognito_user import CognitoUserCredentials, CognitoUserIdentity
 from scs_core.aws.security.cognito_password_manager import CognitoPasswordManager
+from scs_core.aws.security.cognito_user import CognitoUserIdentity
 
 from scs_core.data.datum import Datum
 
 from scs_core.sys.http_exception import HTTPException, HTTPBadRequestException, HTTPUnauthorizedException, \
     HTTPNotFoundException, HTTPNotAllowedException
 
 from scs_core.sys.logging import Logging
@@ -144,15 +145,15 @@
                 logger.error("no user could be found for email '%s'." % cmd.email)
                 exit(1)
 
         if cmd.set_password:
             temporary_password = StdIO.prompt("Enter temporary password")
 
             # login
-            credentials = CognitoUserCredentials(None, cmd.email, temporary_password, None)
+            credentials = CognitoClientCredentials(None, cmd.email, temporary_password, None)
             auth = gatekeeper.user_login(credentials)
 
             if auth.authentication_status != AuthenticationStatus.Challenge:
                 logger.error(auth.authentication_status.description)
                 exit(1)
 
             do_password(True)
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cognito_user_credentials.py` & `scs-analysis-2.0.0/src/scs_analysis/cognito_user_credentials.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,35 +38,36 @@
 """
 
 import requests
 import sys
 
 from scs_analysis.cmd.cmd_cognito_user_credentials import CmdCognitoUserCredentials
 
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
-from scs_core.aws.security.cognito_user import CognitoUserCredentials, CognitoUserIdentity
+from scs_core.aws.security.cognito_user import CognitoUserIdentity
 
 from scs_core.data.datum import Datum
 from scs_core.data.json import JSONify
 
 from scs_core.sys.http_exception import HTTPException
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 def load_credentials(credentials_name):
     try:
-        password = CognitoUserCredentials.password_from_user()
-        return CognitoUserCredentials.load(Host, name=credentials_name, encryption_key=password)
+        password = CognitoClientCredentials.password_from_user()
+        return CognitoClientCredentials.load(Host, name=credentials_name, encryption_key=password)
 
     except (KeyError, ValueError):
-        logger.error("incorrect password")
+        logger.error("incorrect password.")
         exit(1)
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
@@ -89,20 +90,20 @@
         logger.info(cmd)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
         if cmd.list:
-            for conf_name in CognitoUserCredentials.list(Host):
+            for conf_name in CognitoClientCredentials.list(Host):
                 print(conf_name, file=sys.stderr)
             exit(0)
 
         if cmd.set:
-            credentials = CognitoUserCredentials.from_user(cmd.credentials_name)
+            credentials = CognitoClientCredentials.from_user(cmd.credentials_name)
 
             if not Datum.is_email_address(credentials.email):
                 logger.error("The email address is not valid.")
                 exit(1)
 
             if not CognitoUserIdentity.is_valid_password(credentials.password):
                 logger.error("The password must include lower and upper case, numeric and punctuation characters.")
@@ -113,15 +114,15 @@
         if cmd.update_password:
             credentials = load_credentials(cmd.credentials_name)
 
             if credentials is None:
                 logger.error("credentials not found.")
                 exit(1)
 
-            credentials = CognitoUserCredentials.from_user(cmd.credentials_name, existing_email=credentials.email)
+            credentials = CognitoClientCredentials.from_user(cmd.credentials_name, existing_email=credentials.email)
 
             if not Datum.is_email_address(credentials.email):
                 logger.error("The email address is not valid.")
                 exit(1)
 
             if not CognitoUserIdentity.is_valid_password(credentials.password):
                 logger.error("The password must include lower and upper case, numeric and punctuation characters.")
@@ -142,15 +143,15 @@
 
             result = gatekeeper.user_login(credentials)
             logger.error(result.authentication_status.description)
 
             exit(0 if result.is_ok() else 1)
 
         elif cmd.delete:
-            CognitoUserCredentials.delete(Host)
+            CognitoClientCredentials.delete(Host)
 
         else:
             credentials = load_credentials(cmd.credentials_name)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # end...
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cognito_user_identity.py` & `scs-analysis-2.0.0/src/scs_analysis/cognito_user_identity.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 """
 
 import requests
 import sys
 
 from scs_analysis.cmd.cmd_cognito_user_identity import CmdCognitoUserIdentity
 
-from scs_core.aws.security.cognito_user_manager import CognitoUserCreator, CognitoUserEditor
-
-from scs_core.aws.security.cognito_user_finder import CognitoUserFinder
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
-from scs_core.aws.security.cognito_user import CognitoUserCredentials, CognitoUserIdentity
+from scs_core.aws.security.cognito_user import CognitoUserIdentity
+from scs_core.aws.security.cognito_user_finder import CognitoUserFinder
+from scs_core.aws.security.cognito_user_manager import CognitoUserCreator, CognitoUserEditor
 
 from scs_core.data.datum import Datum
 from scs_core.data.json import JSONify
 
 from scs_core.sys.http_exception import HTTPConflictException
 from scs_core.sys.logging import Logging
 
@@ -82,23 +82,23 @@
         # ------------------------------------------------------------------------------------------------------------
         # auth...
 
         if not cmd.create:
             gatekeeper = CognitoLoginManager(requests)
 
             # CognitoUserCredentials...
-            if not CognitoUserCredentials.exists(Host, name=cmd.credentials_name):
+            if not CognitoClientCredentials.exists(Host, name=cmd.credentials_name):
                 logger.error("Cognito credentials not available.")
                 exit(1)
 
             try:
-                password = CognitoUserCredentials.password_from_user()
-                credentials = CognitoUserCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
+                password = CognitoClientCredentials.password_from_user()
+                credentials = CognitoClientCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
             except (KeyError, ValueError):
-                logger.error("incorrect password")
+                logger.error("incorrect password.")
                 exit(1)
 
             auth = gatekeeper.user_login(credentials)
 
             if not auth.is_ok():
                 logger.error("login: %s" % auth.authentication_status.description)
                 exit(1)
@@ -123,35 +123,37 @@
             email = StdIO.prompt("Enter email address")
             password = StdIO.prompt("Enter password")
             retrieval_password = StdIO.prompt("Enter retrieval password (RETURN for same)")
 
             if not retrieval_password:
                 retrieval_password = password
 
+            # validate...
             if not given_name or not given_name:
                 logger.error("Given name and family name are required.")
                 exit(1)
 
             if not Datum.is_email_address(email):
                 logger.error("The email address is not valid.")
                 exit(1)
 
             if not CognitoUserIdentity.is_valid_password(password):
                 logger.error("The password must include lower and upper case, numeric and punctuation characters.")
                 exit(1)
 
-            report = CognitoUserIdentity(None, None, None, True, False, email, given_name, family_name, password,
+            # save identity...
+            report = CognitoUserIdentity(email, None, None, True, False, email, given_name, family_name, password,
                                          False, False, None)
 
             manager = CognitoUserCreator(requests)
             report = manager.create(report)
 
             # create credentials...
-            credentials = CognitoUserCredentials(cmd.credentials_name, email, password, retrieval_password)
-            credentials.save(Host)
+            credentials = CognitoClientCredentials(cmd.credentials_name, email, password, retrieval_password)
+            credentials.save(Host, encryption_key=retrieval_password)
 
         if cmd.update:
             # find...
             identity = finder.get_self(auth.id_token)
 
             # update identity...
             given_name = StdIO.prompt("Enter given name", default=identity.given_name)
@@ -170,37 +172,40 @@
 
             else:
                 retrieval_password = StdIO.prompt("Enter retrieval password (RETURN to keep existing)")
 
                 if not retrieval_password:
                     retrieval_password = credentials.retrieval_password
 
+            # validate...
+            if not given_name or not given_name:
+                logger.error("Given name and family name are required.")
+                exit(1)
+
             if not Datum.is_email_address(email):
                 logger.error("The email address '%s' is not valid." % email)
                 exit(1)
 
             if password and not CognitoUserIdentity.is_valid_password(password):
                 logger.error("The password '%s' is not valid." % password)
                 exit(1)
 
+            # save identity...
             identity = CognitoUserIdentity(identity.username, None, None, True, identity.email_verified,
                                            email, given_name, family_name, password,
                                            identity.is_super, identity.is_tester, None)
 
             auth = gatekeeper.user_login(credentials)                          # renew credentials
             manager = CognitoUserEditor(requests, auth.id_token)
             report = manager.update(identity)
 
             # update credentials...
-            credentials = CognitoUserCredentials(credentials.name, email, password, retrieval_password)
+            credentials = CognitoClientCredentials(credentials.name, email, password, retrieval_password)
             credentials.save(Host, encryption_key=retrieval_password)
 
-            # report...
-            # report = finder.get_self(auth.id_token)
-
 
     # ----------------------------------------------------------------------------------------------------------------
     # end...
 
         if report is not None:
             print(JSONify.dumps(report, indent=cmd.indent))
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/cognito_users.py` & `scs-analysis-2.0.0/src/scs_analysis/cognito_users.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,36 +23,40 @@
 
 DOCUMENT EXAMPLE
 {"username": "8", "creation-date": "2021-11-24T12:51:12Z", "confirmation-status": "CONFIRMED", "enabled": true,
 "email": "bruno.beloff@southcoastscience.com", "given-name": "Bruno", "family-name": "Beloff", "is-super": true}
 
 SEE ALSO
 scs_analysis/cognito_credentials
+scs_analysis/cognito_devices
+scs_analysis/organisation_users
 
 RESOURCES
 https://docs.aws.amazon.com/cognito/latest/developerguide/signing-up-users-in-your-app.html
 https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-settings-policies.html
 """
 
 import requests
 import sys
 
 from scs_analysis.cmd.cmd_cognito_users import CmdCognitoUsers
 
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
 from scs_core.aws.security.cognito_membership import CognitoMembership
-from scs_core.aws.security.cognito_user import CognitoUserCredentials, CognitoUserIdentity
+from scs_core.aws.security.cognito_user import CognitoUserIdentity
 from scs_core.aws.security.cognito_user_finder import CognitoUserFinder
 from scs_core.aws.security.cognito_user_manager import CognitoUserCreator, CognitoUserEditor, CognitoUserDeleter
+
 from scs_core.aws.security.organisation_manager import OrganisationManager
 
 from scs_core.data.datum import Datum
 from scs_core.data.json import JSONify
 
-from scs_core.sys.http_exception import HTTPConflictException
+from scs_core.sys.http_exception import HTTPException, HTTPConflictException
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
@@ -87,23 +91,23 @@
         # ------------------------------------------------------------------------------------------------------------
         # auth...
 
         if not cmd.create:
             gatekeeper = CognitoLoginManager(requests)
 
             # CognitoUserCredentials...
-            if not CognitoUserCredentials.exists(Host, name=cmd.credentials_name):
+            if not CognitoClientCredentials.exists(Host, name=cmd.credentials_name):
                 logger.error("Cognito credentials not available.")
                 exit(1)
 
             try:
-                password = CognitoUserCredentials.password_from_user()
-                credentials = CognitoUserCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
+                password = CognitoClientCredentials.password_from_user()
+                credentials = CognitoClientCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
             except (KeyError, ValueError):
-                logger.error("incorrect password")
+                logger.error("incorrect password.")
                 exit(1)
 
             auth = gatekeeper.user_login(credentials)
 
             if not auth.is_ok():
                 logger.error("login: %s" % auth.authentication_status.description)
                 exit(1)
@@ -207,7 +211,11 @@
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     except HTTPConflictException as ex:
         logger.error("the email address '%s' is already in use." % cmd.email)
         exit(1)
+
+    except HTTPException as ex:
+        logger.error(ex.data)
+        exit(1)
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/configuration_csv.py` & `scs-analysis-2.0.0/src/scs_analysis/configuration_csv.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/configuration_monitor.py` & `scs-analysis-2.0.0/src/scs_analysis/configuration_monitor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/configuration_monitor_check.py` & `scs-analysis-2.0.0/src/scs_analysis/configuration_monitor_check.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/csv_collation_summary.py` & `scs-analysis-2.0.0/src/scs_analysis/csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/csv_collator.py` & `scs-analysis-2.0.0/src/scs_analysis/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/csv_join.py` & `scs-analysis-2.0.0/src/scs_analysis/csv_join.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/csv_reader.py` & `scs-analysis-2.0.0/src/scs_analysis/csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/csv_segmentor.py` & `scs-analysis-2.0.0/src/scs_analysis/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/csv_writer.py` & `scs-analysis-2.0.0/src/scs_analysis/csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/handler/aws_mqtt_publisher.py` & `scs-analysis-2.0.0/src/scs_analysis/handler/aws_mqtt_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/handler/aws_mqtt_subscription_handler.py` & `scs-analysis-2.0.0/src/scs_analysis/handler/aws_mqtt_subscription_handler.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/handler/batch_download_reporter.py` & `scs-analysis-2.0.0/src/scs_analysis/handler/batch_download_reporter.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/handler/configuration_csv_generator.py` & `scs-analysis-2.0.0/src/scs_analysis/handler/configuration_csv_generator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/handler/csv_collator.py` & `scs-analysis-2.0.0/src/scs_analysis/handler/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/handler/csv_segmentor.py` & `scs-analysis-2.0.0/src/scs_analysis/handler/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/handler/osio_mqtt_client_handler.py` & `scs-analysis-2.0.0/src/scs_analysis/handler/osio_mqtt_client_handler.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/handler/osio_mqtt_control_handler.py` & `scs-analysis-2.0.0/src/scs_analysis/handler/osio_mqtt_control_handler.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/handler/sample_midpoint.py` & `scs-analysis-2.0.0/src/scs_analysis/handler/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/handler/sample_regression.py` & `scs-analysis-2.0.0/src/scs_analysis/handler/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/histo_chart.py` & `scs-analysis-2.0.0/src/scs_analysis/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/localised_datetime.py` & `scs-analysis-2.0.0/src/scs_analysis/localised_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/monitor_auth.py` & `scs-analysis-2.0.0/src/scs_analysis/monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/mqtt_peers.py` & `scs-analysis-2.0.0/src/scs_analysis/mqtt_peers.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/multi_chart.py` & `scs-analysis-2.0.0/src/scs_analysis/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/node.py` & `scs-analysis-2.0.0/src/scs_analysis/node.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/organisation_devices.py` & `scs-analysis-2.0.0/src/scs_analysis/organisation_devices.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,26 +24,26 @@
 {"DeviceTag": "scs-bgx-401", "OrgID": 1, "DevicePath": "south-coast-science-demo/brighton/loc/1/",
 "EnvironmentPath": "south-coast-science-demo/brighton/device/praxis-000401/",
 "StartDatetime": "2022-01-17T10:40:04Z", "EndDatetime": null,
 "DeploymentLabel": "Preston Circus"}
 
 SEE ALSO
 scs_analysis/cognito_credentials
+scs_analysis/cognito_devices
 """
 
-import logging
 import requests
 import sys
 
 from scs_analysis.cmd.cmd_organisation_devices import CmdOrganisationDevices
 
 from scs_core.aws.config.project import Project
 
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
-from scs_core.aws.security.cognito_user import CognitoUserCredentials
 
 from scs_core.aws.security.organisation import Organisation, OrganisationPathRoot, OrganisationDevice
 from scs_core.aws.security.organisation_manager import OrganisationManager
 
 from scs_core.data.datetime import LocalizedDatetime
 from scs_core.data.datum import Datum
 from scs_core.data.json import JSONify
@@ -55,31 +55,28 @@
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     logger = None
-    credentials = None
-    auth = None
-    cognito = None
     org = None
     report = []
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
         cmd = CmdOrganisationDevices()
 
         if not cmd.is_valid():
             cmd.print_help(sys.stderr)
             exit(2)
 
-        Logging.config('organisation_devices', level=logging.DEBUG)
+        Logging.config('organisation_devices', verbose=cmd.verbose)
         logger = Logging.getLogger()
 
         logger.info(cmd)
 
         if cmd.org_label is not None and not Organisation.is_valid_label(cmd.org_label):
             logger.error("the organisation label '%s' is not valid." % cmd.org_label)
             exit(2)
@@ -104,23 +101,23 @@
 
         # ------------------------------------------------------------------------------------------------------------
         # auth...
 
         gatekeeper = CognitoLoginManager(requests)
 
         # CognitoUserCredentials...
-        if not CognitoUserCredentials.exists(Host, name=cmd.credentials_name):
+        if not CognitoClientCredentials.exists(Host, name=cmd.credentials_name):
             logger.error("Cognito credentials not available.")
             exit(1)
 
         try:
-            password = CognitoUserCredentials.password_from_user()
-            credentials = CognitoUserCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
+            password = CognitoClientCredentials.password_from_user()
+            credentials = CognitoClientCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
         except (KeyError, ValueError):
-            logger.error("incorrect password")
+            logger.error("incorrect password.")
             exit(1)
 
 
         auth = gatekeeper.user_login(credentials)
 
         if not auth.is_ok():
             logger.error("login: %s" % auth.authentication_status.description)
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/organisation_path_roots.py` & `scs-analysis-2.0.0/src/scs_analysis/organisation_user_paths.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,151 +4,161 @@
 Created on 18 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The organisation_path_roots utility is used to
+The organisation_user_paths utility is used to
 
 SYNOPSIS
-organisation_path_roots.py  [-c CREDENTIALS] { -F -l ORG_LABEL | \
--C -l ORG_LABEL -r PATH_ROOT | \
--D -l ORG_LABEL -r PATH_ROOT } \
+organisation_user_paths.py  [-c CREDENTIALS] { -F -e EMAIL -r PATH_ROOT | \
+-C -e EMAIL -r PATH_ROOT -x PATH_EXTENSION | \
+-D -e EMAIL -r PATH_ROOT -x PATH_EXTENSION } \
 [-i INDENT] [-v]
 
 EXAMPLES
-organisation_path_roots.py -F -l NARA
+organisation_user_paths.py -F -u NARA
 
 DOCUMENT EXAMPLE
-{"OPRID": 11, "OrgID": 1, "PathRoot": "ricardo/"}
+{"Username": 111, "OrgID": 1, "IsOrgAdmin": true, "IsDeviceAdmin": true, "IsSuspended": false}
 
 SEE ALSO
 scs_analysis/cognito_credentials
 """
 
 import requests
 import sys
 
-from scs_analysis.cmd.cmd_organisation_path_roots import CmdOrganisationPathRoots
+from scs_analysis.cmd.cmd_organisation_user_paths import CmdOrganisationUserPaths
 
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
-from scs_core.aws.security.cognito_user import CognitoUserCredentials
 
-from scs_core.aws.security.organisation import Organisation, OrganisationPathRoot
+from scs_core.aws.security.organisation import OrganisationPathRoot, OrganisationUserPath
 from scs_core.aws.security.organisation_manager import OrganisationManager
+from scs_core.aws.security.cognito_user_finder import CognitoUserFinder
 
+
+from scs_core.data.datum import Datum
 from scs_core.data.json import JSONify
 
 from scs_core.sys.http_exception import HTTPException
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     logger = None
-    credentials = None
-    auth = None
-    org = None
-    report = None
+    report = []
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
-        cmd = CmdOrganisationPathRoots()
+        cmd = CmdOrganisationUserPaths()
 
         if not cmd.is_valid():
             cmd.print_help(sys.stderr)
             exit(2)
 
-        Logging.config('organisation_path_roots', verbose=cmd.verbose)
+        Logging.config('organisation_user_paths', verbose=cmd.verbose)
         logger = Logging.getLogger()
 
         logger.info(cmd)
 
-        if not Organisation.is_valid_label(cmd.org_label):
-            logger.error("the organisation label '%s' is not valid." % cmd.org_label)
+        if not Datum.is_email_address(cmd.email):
+            logger.error("email address '%s' is not valid." % cmd.email)
+            exit(2)
+
+        if cmd.path_root and not OrganisationPathRoot.is_valid_path_root(cmd.path_root):
+            logger.error("path root '%s' is not valid." % cmd.path_root)
             exit(2)
 
-        if cmd.path_root is not None and not OrganisationPathRoot.is_valid_path_root(cmd.path_root):
-            logger.error("the path root '%s' is not valid." % cmd.path_root)
+        if cmd.path_extension is not None and not OrganisationUserPath.is_valid_path_extension(cmd.path_extension):
+            logger.error("path extension '%s' is not valid." % cmd.path_extension)
             exit(2)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # auth...
 
         gatekeeper = CognitoLoginManager(requests)
 
         # CognitoUserCredentials...
-        if not CognitoUserCredentials.exists(Host, name=cmd.credentials_name):
+        if not CognitoClientCredentials.exists(Host, name=cmd.credentials_name):
             logger.error("Cognito credentials not available.")
             exit(1)
 
         try:
-            password = CognitoUserCredentials.password_from_user()
-            credentials = CognitoUserCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
+            password = CognitoClientCredentials.password_from_user()
+            credentials = CognitoClientCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
         except (KeyError, ValueError):
-            logger.error("incorrect password")
+            logger.error("incorrect password.")
             exit(1)
 
         auth = gatekeeper.user_login(credentials)
 
         if not auth.is_ok():
             logger.error("login: %s" % auth.authentication_status.description)
             exit(1)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
+        finder = CognitoUserFinder(requests)
         manager = OrganisationManager(requests)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # validate...
 
-        if cmd.org_label is not None:
-            org = manager.get_organisation_by_label(auth.id_token, cmd.org_label)
+        cognito = finder.get_by_email(auth.id_token, cmd.email)
+
+        if cognito is None:
+            logger.error("no Cognito user found for email: '%s'." % cmd.email)
+            exit(1)
+
+        if cmd.path_root:
+            opr = manager.get_opr_by_path_root(auth.id_token, cmd.path_root)
 
-            if org is None:
-                logger.error("no organisation found for label: '%s'." % cmd.org_label)
+            if opr is None:
+                logger.error("no organisation path root found for path: '%s'." % cmd.path_root)
                 exit(1)
 
+            opr_id = opr.opr_id
+
+        else:
+            opr_id = None
+
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
         if cmd.find:
-            report = manager.find_oprs_by_organisation(auth.id_token, org.org_id)
+            report = manager.find_oups(auth.id_token, username=cognito.username, opr_id=opr_id)
 
         if cmd.create:
-            org = OrganisationPathRoot(0, org.org_id, cmd.path_root)
-            report = manager.insert_opr(auth.id_token, org)
+            report = OrganisationUserPath(cognito.username, opr_id, cmd.path_extension)
+            manager.assert_oup(auth.id_token, report)
 
         if cmd.delete:
-            opr = manager.get_opr_by_path_root(auth.id_token, cmd.path_root)
-
-            if opr is None:
-                logger.error("no path root found for path: '%s'." % cmd.path_root)
-                exit(1)
-
-            # delete...
-            manager.delete_opr(auth.id_token, cmd.delete)
+            oup = OrganisationUserPath(cognito.username, opr_id, cmd.path_extension)
+            manager.delete_oup(auth.id_token, oup)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # end...
 
-        if report is not None:
+        if not cmd.delete:
             print(JSONify.dumps(report, indent=cmd.indent))
 
         if cmd.find:
             logger.info("found: %s" % len(report))
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/organisation_user_paths.py` & `scs-analysis-2.0.0/src/scs_analysis/organisation_users.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,107 +4,101 @@
 Created on 18 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The organisation_user_paths utility is used to
+The organisation_users utility is used to
 
 SYNOPSIS
-organisation_user_paths.py  [-c CREDENTIALS] { -F -e EMAIL -r PATH_ROOT | \
--C -e EMAIL -r PATH_ROOT -x PATH_EXTENSION | \
--D -e EMAIL -r PATH_ROOT -x PATH_EXTENSION } \
+organisation_users.py  [-c CREDENTIALS] { -F { -e EMAIL | -l ORG_LABEL } | \
+-R -e EMAIL -l ORG_LABEL | \
+-C -e EMAIL -l ORG_LABEL -o { 1 | 0 } -d { 1 | 0 } | \
+-U -e EMAIL -l ORG_LABEL [-o { 1 | 0 }] [-d { 1 | 0 }] [-s { 1 | 0 }] | \
+-D -e EMAIL -l ORG_LABEL } \
 [-i INDENT] [-v]
 
 EXAMPLES
-organisation_user_paths.py -F -u NARA
+organisation_users.py -F -l NARA
 
 DOCUMENT EXAMPLE
 {"Username": 111, "OrgID": 1, "IsOrgAdmin": true, "IsDeviceAdmin": true, "IsSuspended": false}
 
 SEE ALSO
 scs_analysis/cognito_credentials
+scs_analysis/cognito_users
 """
 
 import requests
 import sys
 
-from scs_analysis.cmd.cmd_organisation_user_paths import CmdOrganisationUserPaths
+from scs_analysis.cmd.cmd_organisation_users import CmdOrganisationUsers
 
-from scs_core.aws.security.cognito_user_finder import CognitoUserFinder
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
-from scs_core.aws.security.cognito_user import CognitoUserCredentials
+from scs_core.aws.security.cognito_user_finder import CognitoUserFinder
 
-from scs_core.aws.security.organisation import OrganisationPathRoot, OrganisationUserPath
+from scs_core.aws.security.organisation import OrganisationUser
 from scs_core.aws.security.organisation_manager import OrganisationManager
 
+
 from scs_core.data.datum import Datum
 from scs_core.data.json import JSONify
 
 from scs_core.sys.http_exception import HTTPException
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     logger = None
-    credentials = None
-    auth = None
     cognito = None
     org = None
     report = []
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
-        cmd = CmdOrganisationUserPaths()
+        cmd = CmdOrganisationUsers()
 
         if not cmd.is_valid():
             cmd.print_help(sys.stderr)
             exit(2)
 
-        Logging.config('organisation_user_paths', verbose=cmd.verbose)
+        Logging.config('organisation_users', verbose=cmd.verbose)
         logger = Logging.getLogger()
 
         logger.info(cmd)
 
-        if not Datum.is_email_address(cmd.email):
+        if cmd.email is not None and not Datum.is_email_address(cmd.email):
             logger.error("email address '%s' is not valid." % cmd.email)
             exit(2)
 
-        if not OrganisationPathRoot.is_valid_path_root(cmd.path_root):
-            logger.error("path root '%s' is not valid." % cmd.path_root)
-            exit(2)
-
-        if cmd.path_extension is not None and not OrganisationUserPath.is_valid_path_extension(cmd.path_extension):
-            logger.error("path extension '%s' is not valid." % cmd.path_extension)
-            exit(2)
-
 
         # ------------------------------------------------------------------------------------------------------------
         # auth...
 
         gatekeeper = CognitoLoginManager(requests)
 
         # CognitoUserCredentials...
-        if not CognitoUserCredentials.exists(Host, name=cmd.credentials_name):
+        if not CognitoClientCredentials.exists(Host, name=cmd.credentials_name):
             logger.error("Cognito credentials not available.")
             exit(1)
 
         try:
-            password = CognitoUserCredentials.password_from_user()
-            credentials = CognitoUserCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
+            password = CognitoClientCredentials.password_from_user()
+            credentials = CognitoClientCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
         except (KeyError, ValueError):
-            logger.error("incorrect password")
+            logger.error("incorrect password.")
             exit(1)
 
         auth = gatekeeper.user_login(credentials)
 
         if not auth.is_ok():
             logger.error("login: %s" % auth.authentication_status.description)
             exit(1)
@@ -116,40 +110,68 @@
         finder = CognitoUserFinder(requests)
         manager = OrganisationManager(requests)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # validate...
 
-        cognito = finder.get_by_email(auth.id_token, cmd.email)
-
-        if cognito is None:
-            logger.error("no Cognito user found for email: '%s'." % cmd.email)
-            exit(1)
-
-        opr = manager.get_opr_by_path_root(auth.id_token, cmd.path_root)
-
-        if opr is None:
-            logger.error("no organisation path root found for path: '%s'." % cmd.path_root)
-            exit(1)
+        if cmd.email:
+            cognito = finder.get_by_email(auth.id_token, cmd.email)
 
+            if cognito is None:
+                logger.error("no Cognito user found for email: '%s'." % cmd.email)
+                exit(1)
+
+        if cmd.org_label:
+            org = manager.get_organisation_by_label(auth.id_token, cmd.org_label)
+
+            if org is None:
+                logger.error("no organisation found for label: '%s'." % cmd.org_label)
+                exit(1)
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
         if cmd.find:
-            report = manager.find_oups(auth.id_token, cognito.username, opr.opr_id)
+            if cmd.email:
+                report = manager.find_users_by_username(auth.id_token, cognito.username)
+
+            elif cmd.org_label:
+                report = manager.find_users_by_organisation(auth.id_token, org.org_id)
+
+            else:
+                report = manager.find_users(auth.id_token)
+
+        if cmd.retrieve:
+            report = manager.get_user(auth.id_token, cognito.username, org.org_id)
 
         if cmd.create:
-            report = OrganisationUserPath(cognito.username, opr.opr_id, cmd.path_extension)
-            manager.assert_oup(auth.id_token, report)
+            is_org_admin = cmd.org_admin == 1
+            is_device_admin = cmd.device_admin == 1
+            is_suspended = False
+
+            report = OrganisationUser(cognito.username, org.org_id, is_org_admin, is_device_admin, is_suspended)
+            manager.assert_user(auth.id_token, report)
+
+        if cmd.update:
+            user = manager.get_user(auth.id_token, cognito.username, org.org_id)
+
+            if user is None:
+                logger.error("no organisation user found for email: '%s' and label '%s'." % (cmd.email, cmd.org_label))
+                exit(1)
+
+            is_org_admin = user.is_org_admin if cmd.org_admin is None else bool(cmd.org_admin)
+            is_device_admin = user.is_device_admin if cmd.device_admin is None else bool(cmd.device_admin)
+            is_suspended = user.is_suspended if cmd.suspended is None else bool(cmd.suspended)
+
+            report = OrganisationUser(cognito.username, org.org_id, is_org_admin, is_device_admin, is_suspended)
+            manager.assert_user(auth.id_token, report)
 
         if cmd.delete:
-            oup = OrganisationUserPath(cognito.username, opr.opr_id, cmd.path_extension)
-            manager.delete_oup(auth.id_token, oup)
+            manager.delete_user(auth.id_token, cognito.username, org.org_id)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # end...
 
         if report is not None:
             print(JSONify.dumps(report, indent=cmd.indent))
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/organisation_users.py` & `scs-analysis-2.0.0/src/scs_analysis/organisations.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,177 +1,165 @@
 #!/usr/bin/env python3
 
 """
-Created on 18 Jan 2022
+Created on 10 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The organisation_users utility is used to
+The organisations utility is used to
 
 SYNOPSIS
-organisation_users.py  [-c CREDENTIALS] { -F { -e EMAIL | -l ORG_LABEL } | \
--R -e EMAIL -l ORG_LABEL | \
--C -e EMAIL -l ORG_LABEL -o { 1 | 0 } -d { 1 | 0 } | \
--U -e EMAIL -l ORG_LABEL [-o { 1 | 0 }] [-d { 1 | 0 }] [-s { 1 | 0 }] | \
--D -e EMAIL -l ORG_LABEL } \
-[-i INDENT] [-v]
+organisations.py  { -F | -C -l LABEL -n LONG_NAME -u URL -o OWNER_EMAIL | \
+-U LABEL [-l LABEL] [-n LONG_NAME] [-u URL] [-o OWNER_EMAIL] | -D LABEL } [-i INDENT] [-v]
 
 EXAMPLES
-organisation_users.py -F -l NARA
+organisations.py -F
 
 DOCUMENT EXAMPLE
-{"Username": 111, "OrgID": 1, "IsOrgAdmin": true, "IsDeviceAdmin": true, "IsSuspended": false}
+{"OrgID": 1, "Label": "SCS", "LongName": "South Coast Science", "URL": "https://www.southcoastscience.com",
+"Owner": "bruno.beloff@southcoastscience.com"}
 
 SEE ALSO
 scs_analysis/cognito_credentials
 """
 
 import requests
 import sys
 
-from scs_analysis.cmd.cmd_organisation_users import CmdOrganisationUsers
+from scs_analysis.cmd.cmd_organisations import CmdOrganisations
 
-from scs_core.aws.security.cognito_user_finder import CognitoUserFinder
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
-from scs_core.aws.security.cognito_user import CognitoUserCredentials
 
-from scs_core.aws.security.organisation import OrganisationUser
+from scs_core.aws.security.organisation import Organisation
 from scs_core.aws.security.organisation_manager import OrganisationManager
 
-from scs_core.data.datum import Datum
 from scs_core.data.json import JSONify
 
 from scs_core.sys.http_exception import HTTPException
 from scs_core.sys.logging import Logging
 
+from scs_host.comms.stdio import StdIO
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     logger = None
-    credentials = None
-    auth = None
-    cognito = None
-    org = None
-    report = []
+    report = None
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
-        cmd = CmdOrganisationUsers()
+        cmd = CmdOrganisations()
 
         if not cmd.is_valid():
             cmd.print_help(sys.stderr)
             exit(2)
 
-        Logging.config('organisation_users', verbose=cmd.verbose)
+        Logging.config('organisations', verbose=cmd.verbose)       # level=logging.DEBUG
         logger = Logging.getLogger()
 
         logger.info(cmd)
 
-        if cmd.email is not None and not Datum.is_email_address(cmd.email):
-            logger.error("email address '%s' is not valid." % cmd.email)
+        if cmd.label is not None and not Organisation.is_valid_label(cmd.label):
+            logger.error("the label '%s' is not valid." % cmd.label)
+            exit(2)
+
+        if cmd.long_name is not None and not Organisation.is_valid_long_name(cmd.long_name):
+            logger.error("the long name '%s' is not valid." % cmd.long_name)
+            exit(2)
+
+        if cmd.url is not None and not Organisation.is_valid_url(cmd.url):
+            logger.error("the URL '%s' is not valid." % cmd.url)
+            exit(2)
+
+        if cmd.owner is not None and not Organisation.is_valid_owner(cmd.owner):
+            logger.error("the owner email address '%s' is not valid." % cmd.owner)
             exit(2)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # auth...
 
         gatekeeper = CognitoLoginManager(requests)
 
         # CognitoUserCredentials...
-        if not CognitoUserCredentials.exists(Host, name=cmd.credentials_name):
+        if not CognitoClientCredentials.exists(Host, name=cmd.credentials_name):
             logger.error("Cognito credentials not available.")
             exit(1)
 
         try:
-            password = CognitoUserCredentials.password_from_user()
-            credentials = CognitoUserCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
+            password = CognitoClientCredentials.password_from_user()
+            credentials = CognitoClientCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
         except (KeyError, ValueError):
-            logger.error("incorrect password")
+            logger.error("incorrect password.")
             exit(1)
 
         auth = gatekeeper.user_login(credentials)
 
         if not auth.is_ok():
             logger.error("login: %s" % auth.authentication_status.description)
             exit(1)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
-        finder = CognitoUserFinder(requests)
         manager = OrganisationManager(requests)
 
 
         # ------------------------------------------------------------------------------------------------------------
-        # validate...
-
-        if cmd.email:
-            cognito = finder.get_by_email(auth.id_token, cmd.email)
-
-            if cognito is None:
-                logger.error("no Cognito user found for email: '%s'." % cmd.email)
-                exit(1)
-
-        if cmd.org_label:
-            org = manager.get_organisation_by_label(auth.id_token, cmd.org_label)
-
-            if org is None:
-                logger.error("no organisation found for label: '%s'." % cmd.org_label)
-                exit(1)
-
-        # ------------------------------------------------------------------------------------------------------------
         # run...
 
         if cmd.find:
-            if cmd.email:
-                report = manager.find_users_by_username(auth.id_token, cognito.username)
-
-            elif cmd.org_label:
-                report = manager.find_users_by_organisation(auth.id_token, org.org_id)
-
-            else:
-                report = manager.find_users(auth.id_token)
-
-        if cmd.retrieve:
-            report = manager.get_user(auth.id_token, cognito.username, org.org_id)
+            report = sorted(manager.find_organisations(auth.id_token))
 
         if cmd.create:
-            is_org_admin = cmd.org_admin == 1
-            is_device_admin = cmd.device_admin == 1
-            is_suspended = False
-
-            report = OrganisationUser(cognito.username, org.org_id, is_org_admin, is_device_admin, is_suspended)
-            manager.assert_user(auth.id_token, report)
+            org = Organisation(0, cmd.label, cmd.long_name, cmd.url, cmd.owner)
+            report = manager.insert_organisation(auth.id_token, org)
 
         if cmd.update:
-            user = manager.get_user(auth.id_token, cognito.username, org.org_id)
+            # find...
+            org = manager.get_organisation_by_label(auth.id_token, cmd.update)
 
-            if user is None:
-                logger.error("no organisation user found for email: '%s' and label '%s'." % (cmd.email, cmd.org_label))
+            if org is None:
+                logger.error("no organisation found for label: '%s'." % cmd.update)
                 exit(1)
 
-            is_org_admin = user.is_org_admin if cmd.org_admin is None else bool(cmd.org_admin)
-            is_device_admin = user.is_device_admin if cmd.device_admin is None else bool(cmd.device_admin)
-            is_suspended = user.is_suspended if cmd.suspended is None else bool(cmd.suspended)
+            # update...
+            label = org.label if cmd.label is None else cmd.label
+            long_name = org.long_name if cmd.long_name is None else cmd.long_name
+            url = org.url if cmd.url is None else cmd.url
+            owner = org.owner if cmd.owner is None else cmd.owner
 
-            report = OrganisationUser(cognito.username, org.org_id, is_org_admin, is_device_admin, is_suspended)
-            manager.assert_user(auth.id_token, report)
+            report = Organisation(org.org_id, label, long_name, url, owner)
+            manager.update_organisation(auth.id_token, report)
 
         if cmd.delete:
-            manager.delete_user(auth.id_token, cognito.username, org.org_id)
+            # find...
+            org = manager.get_organisation_by_label(auth.id_token, cmd.delete)
+
+            if org is None:
+                logger.error("no organisation found for label: '%s'" % cmd.delete)
+                exit(1)
+
+            # check...
+            response = StdIO.prompt('Are you sure? (Y/n)')
+            if response != 'Y':
+                exit(0)
+
+            # delete...
+            manager.delete_organisation(auth.id_token, org.org_id)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # end...
 
         if report is not None:
             print(JSONify.dumps(report, indent=cmd.indent))
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/organisations.py` & `scs-analysis-2.0.0/src/scs_analysis/organisation_path_roots.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,110 +1,100 @@
 #!/usr/bin/env python3
 
 """
-Created on 10 Jan 2022
+Created on 18 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The organisations utility is used to
+The organisation_path_roots utility is used to
 
 SYNOPSIS
-organisations.py  { -F | -C -l LABEL -n LONG_NAME -u URL -o OWNER_EMAIL | \
--U LABEL [-l LABEL] [-n LONG_NAME] [-u URL] [-o OWNER_EMAIL] | -D LABEL } [-i INDENT] [-v]
+organisation_path_roots.py  [-c CREDENTIALS] \
+{ -F -l ORG_LABEL | -C -l ORG_LABEL -r PATH_ROOT | -D -l ORG_LABEL -r PATH_ROOT } [-m] [-i INDENT] [-v]
 
 EXAMPLES
-organisations.py -F
+organisation_path_roots.py -vi4 -c super -Fl 4sfera -m
 
 DOCUMENT EXAMPLE
-{"OrgID": 1, "Label": "SCS", "LongName": "South Coast Science", "URL": "https://www.southcoastscience.com",
-"Owner": "bruno.beloff@southcoastscience.com"}
+{"OPRID": 11, "OrgID": 1, "PathRoot": "ricardo/"}
 
 SEE ALSO
 scs_analysis/cognito_credentials
 """
 
 import requests
 import sys
 
-from scs_analysis.cmd.cmd_organisations import CmdOrganisations
+from scs_analysis.cmd.cmd_organisation_path_roots import CmdOrganisationPathRoots
 
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
-from scs_core.aws.security.cognito_user import CognitoUserCredentials
 
-from scs_core.aws.security.organisation import Organisation
+from scs_core.aws.security.organisation import Organisation, OrganisationPathRoot
 from scs_core.aws.security.organisation_manager import OrganisationManager
+from scs_core.aws.security.opr_membership import OPRMembership
 
 from scs_core.data.json import JSONify
 
 from scs_core.sys.http_exception import HTTPException
 from scs_core.sys.logging import Logging
 
-from scs_host.comms.stdio import StdIO
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     logger = None
-    credentials = None
-    auth = None
+    org = None
     report = None
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
-        cmd = CmdOrganisations()
+        cmd = CmdOrganisationPathRoots()
 
         if not cmd.is_valid():
             cmd.print_help(sys.stderr)
             exit(2)
 
-        Logging.config('organisations', verbose=cmd.verbose)       # level=logging.DEBUG
+        Logging.config('organisation_path_roots', verbose=cmd.verbose)
         logger = Logging.getLogger()
 
         logger.info(cmd)
 
-        if cmd.label is not None and not Organisation.is_valid_label(cmd.label):
-            logger.error("the label '%s' is not valid." % cmd.label)
+        if cmd.org_label is not None and not Organisation.is_valid_label(cmd.org_label):
+            logger.error("the organisation label '%s' is not valid." % cmd.org_label)
             exit(2)
 
-        if cmd.long_name is not None and not Organisation.is_valid_long_name(cmd.long_name):
-            logger.error("the long name '%s' is not valid." % cmd.long_name)
-            exit(2)
-
-        if cmd.url is not None and not Organisation.is_valid_url(cmd.url):
-            logger.error("the URL '%s' is not valid." % cmd.url)
-            exit(2)
-
-        if cmd.owner is not None and not Organisation.is_valid_owner(cmd.owner):
-            logger.error("the owner email address '%s' is not valid." % cmd.owner)
+        if cmd.path_root is not None and not OrganisationPathRoot.is_valid_path_root(cmd.path_root):
+            logger.error("the path root '%s' is not valid." % cmd.path_root)
             exit(2)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # auth...
 
         gatekeeper = CognitoLoginManager(requests)
 
         # CognitoUserCredentials...
-        if not CognitoUserCredentials.exists(Host, name=cmd.credentials_name):
+        if not CognitoClientCredentials.exists(Host, name=cmd.credentials_name):
             logger.error("Cognito credentials not available.")
             exit(1)
 
         try:
-            password = CognitoUserCredentials.password_from_user()
-            credentials = CognitoUserCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
+            password = CognitoClientCredentials.password_from_user()
+            credentials = CognitoClientCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
         except (KeyError, ValueError):
-            logger.error("incorrect password")
+            logger.error("incorrect password.")
             exit(1)
 
         auth = gatekeeper.user_login(credentials)
 
         if not auth.is_ok():
             logger.error("login: %s" % auth.authentication_status.description)
             exit(1)
@@ -113,55 +103,52 @@
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
         manager = OrganisationManager(requests)
 
 
         # ------------------------------------------------------------------------------------------------------------
-        # run...
+        # validate...
 
-        if cmd.find:
-            report = sorted(manager.find_organisations(auth.id_token))
-
-        if cmd.create:
-            org = Organisation(0, cmd.label, cmd.long_name, cmd.url, cmd.owner)
-            report = manager.insert_organisation(auth.id_token, org)
-
-        if cmd.update:
-            # find...
-            org = manager.get_organisation_by_label(auth.id_token, cmd.update)
+        if cmd.org_label is not None:
+            org = manager.get_organisation_by_label(auth.id_token, cmd.org_label)
 
             if org is None:
-                logger.error("no organisation found for label: '%s'." % cmd.update)
+                logger.error("no organisation found for label: '%s'." % cmd.org_label)
                 exit(1)
 
-            # update...
-            label = org.label if cmd.label is None else cmd.label
-            long_name = org.long_name if cmd.long_name is None else cmd.long_name
-            url = org.url if cmd.url is None else cmd.url
-            owner = org.owner if cmd.owner is None else cmd.owner
+            org_id = org.org_id
+
+        else:
+            org_id = None
 
-            report = Organisation(org.org_id, label, long_name, url, owner)
-            manager.update_organisation(auth.id_token, report)
+
+        # ------------------------------------------------------------------------------------------------------------
+        # run...
+
+        if cmd.find:
+            report = manager.find_oprs(auth.id_token, org_id=org_id)
+
+            if cmd.memberships:
+                oups = manager.find_oups(auth.id_token)
+                report = OPRMembership.merge(report, oups)
+
+        if cmd.create:
+            org = OrganisationPathRoot(0, org.org_id, cmd.path_root)
+            report = manager.insert_opr(auth.id_token, org)
 
         if cmd.delete:
-            # find...
-            org = manager.get_organisation_by_label(auth.id_token, cmd.delete)
+            opr = manager.get_opr_by_path_root(auth.id_token, cmd.path_root)
 
-            if org is None:
-                logger.error("no organisation found for label: '%s'" % cmd.delete)
+            if opr is None:
+                logger.error("no path root found for path: '%s'." % cmd.path_root)
                 exit(1)
 
-            # check...
-            response = StdIO.prompt('Are you sure? (Y/n)')
-            if response != 'Y':
-                exit(0)
-
             # delete...
-            manager.delete_organisation(auth.id_token, org.org_id)
+            manager.delete_opr(auth.id_token, cmd.delete)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # end...
 
         if report is not None:
             print(JSONify.dumps(report, indent=cmd.indent))
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/osio_api_auth.py` & `scs-analysis-2.0.0/src/scs_analysis/osio_api_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/osio_client_auth.py` & `scs-analysis-2.0.0/src/scs_analysis/osio_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/osio_mqtt_client.py` & `scs-analysis-2.0.0/src/scs_analysis/osio_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/osio_mqtt_control.py` & `scs-analysis-2.0.0/src/scs_analysis/osio_mqtt_control.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/osio_topic_history.py` & `scs-analysis-2.0.0/src/scs_analysis/osio_topic_history.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/osio_topic_publisher.py` & `scs-analysis-2.0.0/src/scs_analysis/osio_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_aggregate.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_average.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_average.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_collator.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_concentration.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_concentration.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_distance.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_distance.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_duplicates.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_duplicates.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,49 +4,49 @@
 Created on 3 Mar 2019
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The sample_duplicates utility is used to find duplicate values in a sequence of input JSON documents, for a specified
-leaf node path. It is particularly useful in searching for duplicate recording datetimes.
+The sample_duplicates utility is used to find duplicate values in a sequence of input JSON documents, optionally
+for a specified node path. It is particularly useful in searching for duplicate recording datetimes.
 
 If an input document does not contain the specified path, then it is ignored.
 
-The default output report is sequence of JSON dictionaries with a field for each value where duplicates were found.
-The value for this field is itself a dictionary, with a field for the index of each input document, and value being
-the input document itself.
+In the default mode, the utility outputs the rows that were duplicates (or contained duplicate field values). If the
+--exclude flag is set, then sample_duplicates generates a version of the input data that contains no duplicates.
 
 In the --counts mode, the output report is sequence of JSON dictionaries with a field for each value where duplicates
 were found, whose value is the number of matching documents.
 
 SYNOPSIS
-sample_duplicates.py [-c] [-v] PATH
+sample_duplicates.py [{ -x | -c }] [-v] [PATH]
 
 EXAMPLES
 csv_reader.py climate.csv | sample_duplicates.py -v val.hmd
 
 DOCUMENT EXAMPLE - OUTPUT
 default mode:
-{"17.5": {"278728": {"val": {"hmd": 17.5, "tmp": 25.7}, "rec": "2019-02-25T15:28:18Z", "tag": "scs-bgx-303"},
-"278731": {"val": {"hmd": 17.5, "tmp": 25.7}, "rec": "2019-02-25T15:31:18Z", "tag": "scs-bgx-303"}}}
+{"val": {"hmd": 17.5, "tmp": 25.7}, "rec": "2019-02-25T15:28:18Z", "tag": "scs-bgx-303"}
+{"val": {"hmd": 17.5, "tmp": 25.7}, "rec": "2019-02-25T15:31:18Z", "tag": "scs-bgx-303"}
 
 counts mode:
 {"17.5": 2}
 """
 
 import sys
 
 from scs_analysis.cmd.cmd_sample_duplicates import CmdSampleDuplicates
 
 from scs_core.data.duplicates import Duplicates
-from scs_core.data.json import JSONify
 from scs_core.data.path_dict import PathDict
 
+from scs_core.sys.logging import Logging
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     dupes = None
 
@@ -58,61 +58,68 @@
 
     cmd = CmdSampleDuplicates()
 
     if not cmd.is_valid():
         cmd.print_help(sys.stderr)
         exit(2)
 
-    if cmd.verbose:
-        print("sample_duplicates: %s" % cmd, file=sys.stderr)
+    Logging.config('sample_duplicates', verbose=cmd.verbose)
+    logger = Logging.getLogger()
+
+    logger.info(cmd)
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
         dupes = Duplicates()
-
+        non_dupes = []
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
         for line in sys.stdin:
             jstr = line.strip()
             datum = PathDict.construct_from_jstr(jstr)
 
             if datum is None:
                 continue
 
             document_count += 1
 
-            if not datum.has_path(cmd.path):
+            if not datum.has_sub_path(cmd.path):
                 continue
 
-            dupes.test(document_count, datum.node(cmd.path), datum)
+            is_duplicate = dupes.test(document_count, datum.node(cmd.path), datum)
+
+            if not cmd.counts:
+                if cmd.exclude:
+                    if not is_duplicate:
+                        non_dupes.append(jstr)
+                else:
+                    if is_duplicate:
+                        print(jstr)
 
             processed_count += 1
 
 
         # ------------------------------------------------------------------------------------------------------------
         # report...
 
+        if cmd.exclude:
+            for datum in non_dupes:
+                print(datum)
+
         if cmd.counts:
             for count in dupes.match_counts():
-                print(JSONify.dumps(count))
-
-        else:
-            for match in dupes.matches():
-                print(JSONify.dumps(match))
+                print(count)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # end...
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     finally:
-        if cmd.verbose:
-            print("sample_duplicates: documents: %d processed: %d" % (document_count, processed_count), file=sys.stderr)
-
-            if dupes is not None:
-                print("sample_duplicates: values with duplicates: %d" % dupes.matched_key_count, file=sys.stderr)
+        logger.info("documents: %d processed: %d" % (document_count, processed_count))
+        logger.info("values with duplicates: %d total duplicates: %d" % (dupes.matched_key_count, dupes.total_matches))
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_error.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_error.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_interval.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_iso_8601.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_low_pass.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_low_pass.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_max.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_max.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_median.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_median.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_midpoint.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_min.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_min.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_noise.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_noise.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_nullify.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_nullify.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_paths.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_regression.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_slope.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_slope.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
             if rec is None:
                 logger.error("invalid ISO 8601 value '%s' in %s." % (rec_node, jstr))
                 exit(1)
 
             # exclude long intervals...
             if cmd.max_interval and prev_rec is not None and rec - prev_rec > cmd.max_interval:
-                logger.info("resetting regression on %s" % jstr)
+                logger.info("regression reset on %s" % jstr)
                 regression.reset()
 
             # value...
             if source_path not in paths:
                 if source_path + '.cur' in paths:
                     source_path += '.cur'               # we are extending an existing slope analysis
                 else:
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_sort.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_stats.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_subset.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_time_shift.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/sample_timezone.py` & `scs-analysis-2.0.0/src/scs_analysis/sample_timezone.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/single_chart.py` & `scs-analysis-2.0.0/src/scs_analysis/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/socket_receiver.py` & `scs-analysis-2.0.0/src/scs_analysis/socket_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/timer.py` & `scs-analysis-2.0.0/src/scs_analysis/timer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis/uds_receiver.py` & `scs-analysis-2.0.0/src/scs_analysis/uds_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-1.1.63/src/scs_analysis.egg-info/PKG-INFO` & `scs-analysis-2.0.0/src/scs_analysis.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 1.1.63
+Version: 2.0.0
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `scs-analysis-1.1.63/src/scs_analysis.egg-info/SOURCES.txt` & `scs-analysis-2.0.0/src/scs_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

