# Comparing `tmp/datarobot_early_access-3.2.0.2023.4.17.tar.gz` & `tmp/datarobot_early_access-3.2.0.2023.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datarobot_early_access-3.2.0.2023.4.17.tar", last modified: Mon Apr 17 16:47:09 2023, max compression
+gzip compressed data, was "dist/datarobot_early_access-3.2.0.2023.4.3.tar", last modified: Mon Apr  3 16:47:08 2023, max compression
```

## Comparing `datarobot_early_access-3.2.0.2023.4.17.tar` & `datarobot_early_access-3.2.0.2023.4.3.tar`

### file list

```diff
@@ -1,164 +1,215 @@
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   164414 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/CHANGES.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/LICENSE.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/MANIFEST.in
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4184 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8482 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/README.md
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5631 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/common_setup.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2153 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_compat.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/__init__.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/helpers/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/helpers/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5320 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/helpers/partitioning_methods.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13072 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/data_matching.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/documentai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/documentai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26523 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/documentai/document.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      485 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/idiomatic_project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4383 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21414 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/model_lineage.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14822 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/model_package.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54473 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7536 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/retraining.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16695 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/client.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23748 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7993 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/errors.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/helpers/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22432 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/helpers/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/helpers/binary_data_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1127 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/helpers/deployment_monitoring.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/helpers/eligibility_result.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/helpers/feature_discovery.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/helpers/image_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    94380 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/helpers/partitioning_methods.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/mixins/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/mixins/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/mixins/browser_mixin.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/mixins/update_attributes_mixin.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4201 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12505 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/accuracy.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/advanced_tuning.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/anomaly_assessment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/api_object.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15447 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/automated_documentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    82114 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/batch_prediction_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10455 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/blueprint.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/calendar_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/change_request.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/cluster.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/cluster_insight.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/compliance_doc_template.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4887 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6953 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/connector.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11955 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/credential.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24027 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/custom_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11963 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/custom_model_test.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    40995 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/custom_model_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15409 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/custom_task.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21195 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/custom_task_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/custom_task_version_dependency_build.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8969 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/data_drift.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/data_engine_query_generator.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16402 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/data_source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13812 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/data_store.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55708 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/datetime_trend_plots.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    92348 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/deployment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6583 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/driver.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/execution_environment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/execution_environment_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5374 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/external_baseline_validation.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/external_dataset_scores_insights/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/feature.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/feature_association_matrix/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/feature_association_matrix/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6177 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16677 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/feature_effect.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10333 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/feature_fit.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/featurelist.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/imported_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21264 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2370 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/missing_report.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   268121 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/modeljob.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/pairwise_statistics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/pareto_front.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/payoff_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/predict_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10203 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/prediction_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34744 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/prediction_explanations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/prediction_server.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/prime_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   209294 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55518 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/rating_table.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/recommended_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/relationships_configuration.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2831 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/restore_discarded_features.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7730 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/ruleset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/secondary_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/segmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10058 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/service_stats.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/shap_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/shap_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/shap_matrix_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4214 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/training_predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1822 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/types.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/use_cases/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      305 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/use_cases/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15114 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/use_cases/use_case.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/user_blueprints/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/user_blueprints/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/user_blueprints/models.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/user_blueprints/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2668 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/validators.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/visualai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/visualai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/visualai/augmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/visualai/images.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/visualai/insights.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/models/word_cloud.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/py.typed
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17131 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/rest.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/utils/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15590 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/utils/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/utils/deprecation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/utils/logger.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/utils/pagination.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/utils/retry.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/utils/source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/utils/sourcedata.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4061 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot/utils/waiters.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot_early_access.egg-info/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4184 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot_early_access.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5475 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot_early_access.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot_early_access.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1072 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot_early_access.egg-info/requires.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/datarobot_early_access.egg-info/top_level.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3173 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/pyproject.toml
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2023-04-17 16:47:09.000000 datarobot_early_access-3.2.0.2023.4.17/setup.cfg
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/setup.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2403 2023-04-17 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.17/setup_weekly.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   163889 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/CHANGES.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/LICENSE.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/MANIFEST.in
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8482 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/README.md
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5719 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/common_setup.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2140 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_compat.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/__init__.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/helpers/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/helpers/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5320 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/helpers/partitioning_methods.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13072 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/data_matching.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/documentai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/documentai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26517 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/documentai/document.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      485 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/idiomatic_project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4383 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21414 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/model_lineage.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14822 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/model_package.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54473 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7536 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/retraining.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16695 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/client.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23584 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7993 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/errors.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22432 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/binary_data_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1127 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/deployment_monitoring.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/eligibility_result.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/feature_discovery.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/image_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    94333 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/partitioning_methods.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/mixins/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/mixins/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/mixins/browser_mixin.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/mixins/update_attributes_mixin.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3943 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12505 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/accuracy.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/advanced_tuning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27440 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/anomaly_assessment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/api_object.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15427 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/automated_documentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    82114 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/batch_prediction_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10455 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/calendar_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/change_request.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/cluster.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/cluster_insight.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/compliance_doc_template.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4887 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6953 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/connector.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11955 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/credential.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24027 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11963 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_model_test.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    40997 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15409 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_task.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21197 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_task_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_task_version_dependency_build.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8969 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/data_drift.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/data_engine_query_generator.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16402 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/data_source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13812 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/data_store.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55708 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/datetime_trend_plots.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    92370 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6583 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/driver.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/execution_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/execution_environment_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5374 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_baseline_validation.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4509 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_association_matrix/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_association_matrix/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6177 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16677 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_effect.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10333 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_fit.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/featurelist.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/imported_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21264 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2370 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/missing_report.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   268121 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/modeljob.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/pairwise_statistics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/pareto_front.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/payoff_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/predict_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10203 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/prediction_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    33395 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/prediction_explanations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/prediction_server.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/prime_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   209294 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55518 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/rating_table.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/recommended_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/relationships_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2831 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/restore_discarded_features.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8203 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/ruleset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/secondary_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/segmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10058 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/service_stats.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/shap_matrix_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4214 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/training_predictions.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/user_blueprints/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/user_blueprints/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69622 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/user_blueprints/models.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/user_blueprints/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2668 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/validators.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/visualai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/visualai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/visualai/augmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/visualai/images.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/visualai/insights.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/models/word_cloud.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/py.typed
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17131 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/rest.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15333 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/deprecation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/logger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/pagination.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/retry.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/sourcedata.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4061 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/waiters.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot_early_access.egg-info/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot_early_access.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7050 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot_early_access.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot_early_access.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1121 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot_early_access.egg-info/requires.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2023-04-03 16:47:07.000000 datarobot_early_access-3.2.0.2023.4.3/datarobot_early_access.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6404 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/Makefile
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/autodoc/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18051 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/autodoc/api_reference.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10245 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/conf.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/examples/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1958 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/examples/index.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      415 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/getting_started.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      961 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/index.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        2 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/predicted.csv
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/admin/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3474 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/admin/credentials.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      415 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/admin/index.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3688 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/admin/sharing.rst
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/data/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7711 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/data/database_connectivity.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9959 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/data/dataset.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22218 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/data/feature_discovery.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      612 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/data/index.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      391 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/index.rst
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/mlops/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    29303 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/mlops/custom_model.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26179 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/mlops/deployment.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      427 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/mlops/index.rst
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4396 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/blueprint.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      570 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/index.rst
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5077 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/insights/automated_documentation.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4033 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/insights/external_testset.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      536 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/insights/index.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10234 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/insights/prediction_explanations.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2277 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/insights/rating_table.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5305 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/job.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21949 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/model.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3232 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/model_recommendation.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3385 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/prime.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16205 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/project.rst
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11364 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/binary_data.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7430 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/custom_task.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10036 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/datetime_partition.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      620 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/index.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6625 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/monotonic_constraints.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6204 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/segmented_modeling.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    36391 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/time_series.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10392 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/unsupervised_anomaly.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7376 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/unsupervised_clustering.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14760 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/modeling/spec/visualai.rst
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/predictions/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    39016 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/predictions/batch_predictions.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1180 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/predictions/index.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9015 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/reference/predictions/predict_job.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      319 2023-04-03 16:46:09.000000 datarobot_early_access-3.2.0.2023.4.3/docs/version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3173 2023-04-03 16:46:10.000000 datarobot_early_access-3.2.0.2023.4.3/pyproject.toml
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2023-04-03 16:47:08.000000 datarobot_early_access-3.2.0.2023.4.3/setup.cfg
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2023-04-03 16:46:10.000000 datarobot_early_access-3.2.0.2023.4.3/setup.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2403 2023-04-03 16:46:10.000000 datarobot_early_access-3.2.0.2023.4.3/setup_weekly.py
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/CHANGES.rst` & `datarobot_early_access-3.2.0.2023.4.3/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 #########
 Changelog
 #########
 3.2.0b0
 ========
-
+ 
 New Features
 ************
  - Added the ability to share deployments. See :ref:`deployment sharing <deployment_sharing>` for more information on sharing deployments.
 
  - Added new methods get_bias_and_fairness_settings and update_bias_and_fairness_settings to retrieve or update bias and fairness settings
    :meth:`Deployment.get_bias_and_fairness_settings<datarobot.models.Deployment.get_bias_and_fairness_settings>`
    :meth:`Deployment.update_bias_and_fairness_settings<datarobot.models.Deployment.update_bias_and_fairness_settings>`
 
-- Added a new class :class:`UseCase <datarobot.UseCase>` for interacting with the DataRobot Use Cases API.
-
 Enhancements
 ************
 - Improve error message of :meth:`SampleImage.list<datarobot.models.visualai.SampleImage.list>`
   to clarify that a selected parameter cannot be used when a project has not proceeded to the
   correct stage prior to calling this method.
 
 - Extended :meth:`SampleImage.list<datarobot.models.visualai.SampleImage.list>` by two parameters
   to filter for a target value range in regression projects.
 
-- Added text explanations data to :meth:`PredictionExplanations <datarobot.PredictionExplanations>` and made sure it is returned in both :py:meth:`datarobot.PredictionExplanations.get_all_as_dataframe`  and :py:meth:`datarobot.PredictionExplanations.get_rows` method.
+- Added text explanations data to :meth:`PredictionExplanations <datarobot.PredictionExplanations>`
 
 Bugfixes
 ********
-- Fix incompatibilities with Pandas 2.0 in :meth:`DatetimePartitioning.to_dataframe <datarobot.DatetimePartitioning.to_dataframe>`.
-
+ 
 API Changes
 ***********
-
+ 
 Deprecation Summary
 *******************
-
+ 
 Configuration Changes
 *********************
-- Removes dependency on package `contextlib2 <https://pypi.org/project/contextlib2/>`_  since the package is Python 3.7+.
-
+ 
 Documentation Changes
 *********************
 
 Experimental changes
 *********************
 - Added experimental support for data matching:
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/LICENSE.txt` & `datarobot_early_access-3.2.0.2023.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/PKG-INFO` & `datarobot_early_access-3.2.0.2023.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot_early_access
-Version: 3.2.0.2023.4.17
+Version: 3.2.0.2023.4.3
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/README.md` & `datarobot_early_access-3.2.0.2023.4.3/README.md`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/common_setup.py` & `datarobot_early_access-3.2.0.2023.4.3/common_setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
+# Copyright 2021 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
@@ -131,20 +131,23 @@
 ] + images_require
 
 dev_require = (
     tests_require
     + lint_require
     + images_require
     + [
-        "Sphinx==4.3.2",
-        "sphinx_rtd_theme==1.0.0",
-        "nbsphinx==0.8.9",
-        "numpydoc==1.4.0",
+        "Sphinx==1.8.3",
+        "sphinx_rtd_theme==0.1.9",
+        "nbsphinx>=0.2.9,<1",
+        "mistune==0.8.4",
+        "nbconvert==5.3.1",
+        "numpydoc>=0.6.0",
         "jupyter_contrib_nbextensions",
-        "sphinx-autodoc-typehints==1.17.1",
+        "tornado<6.0",
+        "jsonschema<=4.3.1",
     ]
 )
 
 example_require = [
     "jupyter<=5.0",
     "fredapi==0.4.0",
     "matplotlib>=2.1.0",
@@ -174,18 +177,19 @@
     license="DataRobot Tool and Utility Agreement",
     packages=None,
     package_data={"datarobot": ["py.typed"]},
     python_requires=">=3.7",
     long_description=None,
     classifiers=None,
     install_requires=[
+        "contextlib2>=0.5.5",
         "pandas>=0.15",
         "numpy",
         "pyyaml>=3.11",
-        "requests>=2.28.1",
+        "requests>=2.21",
         "requests_toolbelt>=0.6",
         "trafaret>=0.7,<2.2,!=1.1.0",
         "urllib3>=1.23",
         "typing-extensions==4.3.0",
     ],
     extras_require={
         "dev": dev_require,
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/__init__.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,10 +92,9 @@
     SegmentInfo,
     ShapImpact,
     ShapMatrix,
     ShapMatrixJob,
     SharingAccess,
     TrainingPredictions,
     TrainingPredictionsJob,
-    UseCase,
     UserBlueprint,
 )
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/_compat.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/__init__.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/helpers/partitioning_methods.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/helpers/partitioning_methods.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/data_matching.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/data_matching.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/documentai/document.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/documentai/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 FeaturesWithSamples = namedtuple(
     "FeaturesWithSamples", ["model_id", "feature_name", "document_task"]
 )
 
 
 if TYPE_CHECKING:
-    from PIL.Image import Image
+    from PIL import Image
     from mypy_extensions import TypedDict
 
     class PredictionType(TypedDict):
         values: Union[float, List[float]]
         labels: NotRequired[List[str]]
 
     class TextLine(TypedDict):
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/idiomatic_project.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/idiomatic_project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/model.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/model_lineage.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/model_lineage.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/model_package.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/model_package.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/project_options.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/_experimental/models/retraining.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/_experimental/models/retraining.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/client.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/client.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/enums.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -862,15 +862,7 @@
     USER = "user"
     CUSTOM = "custom"
 
 
 class ComplianceDocTemplateType(str, Enum):
     NORMAL = "normal"
     TIME_SERIES = "time_series"
-
-
-class UseCaseEntities(str, Enum):
-    PROJECT = "project"
-    DATASET = "dataset"
-    NOTEBOOK = "notebook"
-    APPLICATION = "application"
-    RECIPE = "recipe"
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/errors.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/errors.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/helpers/__init__.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/helpers/binary_data_utils.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/helpers/deployment_monitoring.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/deployment_monitoring.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/helpers/eligibility_result.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/helpers/feature_discovery.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/helpers/image_utils.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/image_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/helpers/partitioning_methods.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/helpers/partitioning_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -2051,11 +2051,10 @@
             "end_date": {
                 "available_training": self.available_training_end_date,
                 "primary_training": self.primary_training_end_date,
                 "gap": self.gap_end_date,
                 "holdout": self.holdout_end_date,
             },
         }
-        display_df_list = [pd.DataFrame.from_dict(display_dict)]
-        display_df_list.extend([bt.to_dataframe() for bt in self.backtests])
-        final_df = pd.concat(display_df_list)
+        display_df = pd.DataFrame.from_dict(display_dict)
+        final_df = display_df.append([bt.to_dataframe() for bt in self.backtests])
         return final_df
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/mixins/browser_mixin.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/mixins/update_attributes_mixin.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/__init__.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,17 +108,8 @@
 from .segmentation import SegmentationTask, SegmentInfo
 from .service_stats import ServiceStats, ServiceStatsOverTime
 from .shap_impact import ShapImpact
 from .shap_matrix import ShapMatrix
 from .shap_matrix_job import ShapMatrixJob
 from .sharing import SharingAccess
 from .training_predictions import TrainingPredictions
-from .types import (
-    AnomalyAssessmentDataPoint,
-    AnomalyAssessmentPreviewBin,
-    AnomalyAssessmentRecordMetadata,
-    RegionExplanationsData,
-    RocCurveEstimatedMetric,
-    ShapleyFeatureContribution,
-)
-from .use_cases import UseCase, UseCaseUser
 from .user_blueprints import UserBlueprint
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/accuracy.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/accuracy.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/advanced_tuning.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/anomaly_assessment.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/anomaly_assessment.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,25 +11,19 @@
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from operator import itemgetter
 from typing import Any, cast, Dict, Iterable, List, Optional, Union
 
 import trafaret as t
-from typing_extensions import Literal, Unpack
+from typing_extensions import Literal, TypedDict, Unpack
 
 from datarobot._compat import Int, String
 from datarobot.enums import AnomalyAssessmentStatus, DATA_SUBSET, SOURCE_TYPE
 from datarobot.models.api_object import APIObject
-from datarobot.models.types import (
-    AnomalyAssessmentDataPoint,
-    AnomalyAssessmentPreviewBin,
-    AnomalyAssessmentRecordMetadata,
-    RegionExplanationsData,
-)
 from datarobot.utils import from_api
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.waiters import wait_for_async_resolution
 
 DEFAULT_BATCH_SIZE = 1000
 
 RecordMetadataTrafaret = t.Dict(
@@ -40,16 +34,50 @@
         t.Key("backtest"): t.Or(String(), Int),
         t.Key("source"): t.Enum(*SOURCE_TYPE.ALL),  # type: ignore[attr-defined]
         t.Key("series_id"): t.Or(String(), t.Null),
     }
 )
 
 
+class RecordMetadata(TypedDict):
+    record_id: str
+    project_id: str
+    model_id: str
+    backtest: Union[str, int]
+    source: SOURCE_TYPE
+    series_id: Optional[str]
+
+
+class PreviewBin(TypedDict):
+    avg_predicted: Optional[float]
+    max_predicted: Optional[float]
+    start_date: str
+    end_date: str
+    frequency: int
+
+
+class RegionExplanationsData(TypedDict):
+    explanations: List[DataPoint]
+    shap_base_value: Optional[float]
+
+
+class ShapleyFeatureContribution(TypedDict):
+    feature_value: str
+    strength: float
+    feature: str
+
+
+class DataPoint(TypedDict):
+    shap_explanation: Optional[List[ShapleyFeatureContribution]]
+    timestamp: str
+    prediction: float
+
+
 class BaseAPIObject(APIObject):  # pylint: disable=missing-class-docstring
-    def __init__(self, **record_kwargs: Unpack[AnomalyAssessmentRecordMetadata]) -> None:
+    def __init__(self, **record_kwargs: Unpack[RecordMetadata]) -> None:
         self.record_id: str = record_kwargs["record_id"]
         self.project_id: str = record_kwargs["project_id"]
         self.model_id: str = record_kwargs["model_id"]
         self.backtest: Union[str, int] = record_kwargs["backtest"]
         self.source: Union[
             Literal[SOURCE_TYPE.TRAINING], Literal[SOURCE_TYPE.VALIDATION]
         ] = record_kwargs["source"]
@@ -190,15 +218,15 @@
         status_details: str,
         start_date: Optional[str],
         end_date: Optional[str],
         prediction_threshold: Optional[float],
         preview_location: Optional[str],
         delete_location: str,
         latest_explanations_location: Optional[str],
-        **record_kwargs: Unpack[AnomalyAssessmentRecordMetadata],
+        **record_kwargs: Unpack[RecordMetadata],
     ) -> None:
         self.status = status
         self.status_details = status_details
         self.start_date = start_date
         self.end_date = end_date
         self.prediction_threshold = prediction_threshold
         self.preview_location = preview_location
@@ -378,15 +406,15 @@
             self.record_id,
             start_date=start_date,
             end_date=end_date,
             points_count=points_count,
         )
 
     def get_explanations_data_in_regions(
-        self, regions: List[AnomalyAssessmentPreviewBin], prediction_threshold: float = 0.0
+        self, regions: List[PreviewBin], prediction_threshold: float = 0.0
     ) -> RegionExplanationsData:
         """Get predictions along with explanations for the specified regions, sorted by
         predictions in descending order.
 
         Parameters
         ----------
         regions: list of preview_bins
@@ -395,15 +423,15 @@
             If specified, only points with score greater or equal to the threshold will be returned.
 
         Returns
         -------
         dict in a form of {'explanations': explanations, 'shap_base_value': shap_base_value}
 
         """
-        explanations: List[AnomalyAssessmentDataPoint] = []
+        explanations: List[DataPoint] = []
         shap_base_value: Optional[float] = None
         for region in regions:
             response = self.get_explanations(
                 start_date=region["start_date"], end_date=region["end_date"]
             )
             shap_base_value = response.shap_base_value
             for item in response.data:
@@ -498,16 +526,16 @@
         .ignore_extra("*")
     )
 
     def __init__(
         self,
         start_date: str,
         end_date: str,
-        preview_bins: List[AnomalyAssessmentPreviewBin],
-        **record_kwargs: Unpack[AnomalyAssessmentRecordMetadata],
+        preview_bins: List[PreviewBin],
+        **record_kwargs: Unpack[RecordMetadata],
     ) -> None:
         self.preview_bins = preview_bins
         self.start_date = start_date
         self.end_date = end_date
         super().__init__(**record_kwargs)
 
     @classmethod
@@ -526,17 +554,15 @@
         AnomalyAssessmentPredictionsPreview
 
         """
         url = cls._path.format(project_id=project_id, record_id=record_id)
         r_data = cls._client.get(url).json()
         return cast("AnomalyAssessmentPredictionsPreview", cls.from_server_data(r_data))
 
-    def find_anomalous_regions(
-        self, max_prediction_threshold: float = 0.0
-    ) -> List[AnomalyAssessmentPreviewBin]:
+    def find_anomalous_regions(self, max_prediction_threshold: float = 0.0) -> List[PreviewBin]:
         """Sort preview bins by max_predicted value and select those with max predicted value
          greater or equal to max prediction threshold.
          Sort the result by max predicted value in descending order.
 
         Parameters
         ----------
         max_prediction_threshold: float, optional
@@ -653,19 +679,19 @@
         .merge(RecordMetadataTrafaret)
         .ignore_extra("*")
     )
 
     def __init__(
         self,
         shap_base_value: float,
-        data: List[AnomalyAssessmentDataPoint],
+        data: List[DataPoint],
         start_date: Optional[str],
         end_date: Optional[str],
         count: int,
-        **record_kwargs: Unpack[AnomalyAssessmentRecordMetadata],
+        **record_kwargs: Unpack[RecordMetadata],
     ) -> None:
         self.shap_base_value = shap_base_value
         self.data = data
         self.count = count
         self.start_date = start_date
         self.end_date = end_date
         super().__init__(**record_kwargs)
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/api_object.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/api_object.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/automated_documentation.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/automated_documentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
 from datetime import datetime
 from typing import cast, List, Optional, Tuple
 
-from requests import Response
+from requests.models import Response
 import trafaret as t
 from typing_extensions import TypedDict
 
 from datarobot._compat import String
 from datarobot.enums import DEFAULT_MAX_WAIT, DocumentType, Locales
 from datarobot.models.api_object import APIObject
 from datarobot.utils import camelize, from_api, get_id_from_location, parse_time
@@ -180,15 +180,15 @@
         """Request generation of an automated document.
 
         Required attributes to request document generation: ``document_type``, ``entity_id``,
         and ``output_format``.
 
         Returns
         -------
-        :class:`requests.models.Response`
+        requests.models.Response
 
         Examples
         --------
         .. code-block:: python
 
             import datarobot as dr
 
@@ -227,15 +227,15 @@
     def download(self) -> Response:
         """
         Download a generated Automated Document.
         Document ID is required to download a file.
 
         Returns
         -------
-        :class:`requests.models.Response`
+        requests.models.Response
 
         Examples
         --------
 
         Generating and downloading the generated document:
 
         .. code-block:: python
@@ -299,15 +299,15 @@
 
     def delete(self) -> Response:
         """
         Delete a document using its ID.
 
         Returns
         -------
-        :class:`requests.models.Response`
+        requests.models.Response
 
         Examples
         --------
 
         .. code-block:: python
 
             import datarobot as dr
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/batch_prediction_job.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/batch_prediction_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/blueprint.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/calendar_file.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/change_request.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/cluster.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/cluster_insight.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/compliance_doc_template.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/compliance_doc_template.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/confusion_chart.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/connector.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/connector.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/credential.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/credential.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/custom_model.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/custom_model_test.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_model_test.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/custom_model_version.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_model_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #
-# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
-import contextlib
 import copy
 import json
 import os
 
+import contextlib2
 from requests_toolbelt import MultipartEncoder
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import DEFAULT_MAX_WAIT, NETWORK_EGRESS_POLICY
 from datarobot.errors import InvalidUsageError
 from datarobot.models.api_object import APIObject
@@ -684,15 +684,15 @@
         network_egress_policy=None,
         maximum_memory=None,
         replicas=None,
         required_metadata_values=None,
     ):
         url = cls._path.format(custom_model_id)
 
-        with contextlib.ExitStack() as stack:
+        with contextlib2.ExitStack() as stack:
             upload_data = [
                 ("isMajorUpdate", str(is_major_update)),
                 ("baseEnvironmentId", base_environment_id),
             ]
 
             if folder_path:
                 for root_path, _, file_paths in os.walk(folder_path):
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/custom_task.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_task.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/custom_task_version.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_task_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #
-# Copyright 2021-2023 DataRobot, Inc. and its affiliates.
+# Copyright 2021-2022 DataRobot, Inc. and its affiliates.
 #
 # All rights reserved.
 #
 # DataRobot, Inc.
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 from __future__ import annotations
 
-import contextlib
 import json
 import os
 
+import contextlib2
 from requests_toolbelt import MultipartEncoder
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.models.api_object import APIObject
 from datarobot.models.custom_model_version import (
     CustomDependency,
@@ -352,15 +352,15 @@
             )
 
         if maximum_memory:
             upload_data.append(("maximumMemory", str(maximum_memory)))
 
         cls._verify_folder_path(folder_path)
 
-        with contextlib.ExitStack() as stack:
+        with contextlib2.ExitStack() as stack:
             if folder_path:
                 for dir_name, _, file_names in os.walk(folder_path):
                     for file_name in file_names:
                         file_path = os.path.join(dir_name, file_name)
                         file = stack.enter_context(
                             open(file_path, "rb")  # pylint: disable=consider-using-with
                         )
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/custom_task_version_dependency_build.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/data_drift.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/data_drift.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/data_engine_query_generator.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/data_source.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/data_source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/data_store.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/data_store.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/dataset.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/datetime_trend_plots.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/deployment.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1570,15 +1570,15 @@
         model_id: Optional[str] = None,
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         execution_time_quantile: Optional[float] = None,
         response_time_quantile: Optional[float] = None,
         slow_requests_threshold: Optional[float] = None,
     ) -> ServiceStats:
-        """Retrieves values of many service stat metrics aggregated over a time period.
+        """Retrieve value of service stat metrics over a certain time period.
 
         .. versionadded:: v2.18
 
         Parameters
         ----------
         model_id : str, optional
             the id of the model
@@ -1618,15 +1618,15 @@
         model_id: Optional[str] = None,
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         bucket_size: Optional[str] = None,
         quantile: Optional[float] = None,
         threshold: Optional[int] = None,
     ) -> ServiceStatsOverTime:
-        """Retrieves values of a single service stat metric over a time period.
+        """Retrieve information about how a service stat metric changes over a certain time period.
 
         .. versionadded:: v2.18
 
         Parameters
         ----------
         metric : SERVICE_STAT_METRIC, optional
             the service stat metric to retrieve
@@ -1740,15 +1740,15 @@
         model_id: Optional[str] = None,
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         start: Optional[datetime] = None,
         end: Optional[datetime] = None,
         target_classes: Optional[List[str]] = None,
     ) -> Accuracy:
-        """Retrieves values of many accuracy metrics aggregated over a time period.
+        """Retrieve values of accuracy metrics over a certain time period.
 
         .. versionadded:: v2.18
 
         Parameters
         ----------
         model_id : str
             the id of the model
@@ -1785,15 +1785,15 @@
         metric: Optional[ACCURACY_METRIC] = None,
         model_id: Optional[str] = None,
         start_time: Optional[datetime] = None,
         end_time: Optional[datetime] = None,
         bucket_size: Optional[str] = None,
         target_classes: Optional[List[str]] = None,
     ) -> AccuracyOverTime:
-        """Retrieves values of a single accuracy metric over a time period.
+        """Retrieve information about how an accuracy metric changes over a certain time period.
 
         .. versionadded:: v2.18
 
         Parameters
         ----------
         metric : ACCURACY_METRIC
             the accuracy metric to retrieve
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/driver.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/driver.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/execution_environment.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/execution_environment_version.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/external_baseline_validation.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_baseline_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from datarobot.models.roc_curve import RocCurveThresholdMixin, RocPointsTrafaret
 from datarobot.utils.pagination import unpaginate
 
 from ..api_object import APIObject
 from .external_scores import DEFAULT_BATCH_SIZE
 
 if TYPE_CHECKING:
-    from datarobot.models.types import RocCurveEstimatedMetric
+    from datarobot.models.roc_curve import EstimatedMetric
 
 
 class ExternalRocCurve(APIObject, RocCurveThresholdMixin):
     """ROC curve data for the model and prediction dataset with target or actual value column in
     unsupervised case.
 
     .. versionadded:: v2.21
@@ -48,15 +48,15 @@
     _path = "projects/{project_id}/models/{model_id}/datasetRocCurves/"
 
     _converter = t.Dict({t.Key("dataset_id"): String}).merge(RocPointsTrafaret).ignore_extra("*")
 
     def __init__(
         self,
         dataset_id: str,
-        roc_points: List[RocCurveEstimatedMetric],
+        roc_points: List[EstimatedMetric],
         negative_class_predictions: List[float],
         positive_class_predictions: List[float],
     ) -> None:
         self.dataset_id = dataset_id
         self.roc_points = roc_points
         self.negative_class_predictions = negative_class_predictions
         self.positive_class_predictions = positive_class_predictions
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/feature.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/feature_effect.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_effect.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/feature_fit.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/feature_fit.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/featurelist.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/imported_model.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/imported_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/job.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/lift_chart.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/missing_report.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/model.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/modeljob.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/pairwise_statistics.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/pareto_front.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/payoff_matrix.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/predict_job.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/prediction_dataset.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/prediction_explanations.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/prediction_explanations.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #
 # This is proprietary source code of DataRobot, Inc. and its
 # affiliates.
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 import abc
 from datetime import datetime
-import json
 
 import pandas as pd
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.enums import TARGET_TYPE
 from datarobot.models.project_options import ProjectOptions
@@ -25,54 +24,47 @@
 
 int_float_string = t.Type(int) | t.Type(float) | String(allow_blank=True)
 
 prediction_values_trafaret = t.Dict(
     {t.Key("label", optional=True): int_float_string, t.Key("value"): t.Float}
 ).ignore_extra("*")
 
-per_ngram_text_explanations_trafaret = t.Or(
-    t.List(
-        t.Dict(
-            {
-                t.Key("ngrams"): t.List(
-                    t.Dict({t.Key("ending_index"): Int, t.Key("starting_index"): Int})
-                ),
-                t.Key("is_unknown"): t.Bool,
-                t.Key("qualitative_strength"): String,
-                t.Key("strength"): t.Float,
-            }
-        )
-    ),
-    t.Null,
+per_ngram_text_explanations_trafaret = t.Dict(
+    {
+        t.Key("ngrams"): t.List(t.Dict({t.Key("ending_index"): Int, t.Key("starting_index"): Int})),
+        t.Key("is_unknown"): t.Bool,
+        t.Key("qualitative_strength"): String,
+        t.Key("strength"): t.Float,
+    }
 )
 
 prediction_explanations_entry_trafaret = t.Dict(
     {
         t.Key("label", optional=True): int_float_string,
         t.Key("feature"): String,
         t.Key("feature_value"): int_float_string,
         t.Key("strength"): t.Float,
         t.Key("qualitative_strength"): String,
-        t.Key("per_ngram_text_explanations", optional=True): per_ngram_text_explanations_trafaret,
+        t.Key("per_ngram_text_explanations", optional=True): t.List(
+            per_ngram_text_explanations_trafaret
+        ),
     }
 ).ignore_extra("*")
 
 prediction_explanations_trafaret = t.Dict(
     {
         t.Key("row_id"): Int,
         t.Key("prediction"): int_float_string,
         t.Key("adjusted_prediction", optional=True): int_float_string,
         t.Key("prediction_values"): t.List(prediction_values_trafaret),
         t.Key("adjusted_prediction_values", optional=True): t.List(prediction_values_trafaret),
         t.Key("prediction_explanations"): t.List(prediction_explanations_entry_trafaret),
     }
 ).ignore_extra("*")
 
-KEEP_ATTRS = ["data.prediction_explanations.per_ngram_text_explanations"]
-
 
 class PredictionExplanationsMode:
     """Prediction explanations mode for multiclass models"""
 
     @abc.abstractmethod
     def get_api_parameters(self, batch_route=False):
         """Get parameters passed in corresponding API call
@@ -505,29 +497,25 @@
             - explanation_0_feature_value : the value the feature took on
             - explanation_0_label : the output being driven by this explanation.  For regression
               projects, this is the name of the target feature.  For classification projects, this
               is the class label whose probability increasing would correspond to a positive
               strength.
             - explanation_0_qualitative_strength : a human-readable description of how strongly the
               feature affected the prediction (e.g. '+++', '--', '+') for this explanation
-            - explanation_0_per_ngram_text_explanations : Text prediction explanations data in json
-              formatted string.
             - explanation_0_strength : the amount this feature's value affected the prediction
             - ...
             - explanation_N_feature : the name of the feature contributing to the prediction for
               this explanation
             - explanation_N_feature_value : the value the feature took on
             - explanation_N_label : the output being driven by this explanation.  For regression
               projects, this is the name of the target feature.  For classification projects, this
               is the class label whose probability increasing would correspond to a positive
               strength.
             - explanation_N_qualitative_strength : a human-readable description of how strongly the
               feature affected the prediction (e.g. '+++', '--', '+') for this explanation
-            - explanation_N_per_ngram_text_explanations : Text prediction explanations data in json
-              formatted string.
             - explanation_N_strength : the amount this feature's value affected the prediction
 
         For classification projects, the server does not guarantee any ordering on the prediction
         values, however within this function we sort the values so that `class_X` corresponds to
         the same class from row to row.
 
         Parameters
@@ -541,18 +529,14 @@
         dataframe: pandas.DataFrame
         """
         columns = ["row_id", "prediction"]
         rows = self.get_rows(
             batch_size=1, exclude_adjusted_predictions=exclude_adjusted_predictions
         )
         first_row = next(rows)
-        has_text_explanations = (
-            first_row.prediction_explanations
-            and "per_ngram_text_explanations" in first_row.prediction_explanations[0]
-        )
         adjusted_predictions_in_data = first_row.adjusted_prediction is not None
         if adjusted_predictions_in_data:
             columns.append("adjusted_prediction")
         # for regression, length is 1; for classification, length is number of levels in target
         # i.e. 2 for binary classification
         is_classification = len(first_row.prediction_values) > 1
         # include class label/probability for classification project
@@ -568,30 +552,25 @@
                             f"{prefix}_explanation_{i}_feature",
                             f"{prefix}_explanation_{i}_feature_value",
                             f"{prefix}_explanation_{i}_label",
                             f"{prefix}_explanation_{i}_qualitative_strength",
                             f"{prefix}_explanation_{i}_strength",
                         ]
                     )
-                    if has_text_explanations:
-                        columns.append(f"{prefix}_explanation_{i}_per_ngram_text_explanations")
-
         else:
             for i in range(self.max_explanations):
                 columns.extend(
                     [
                         f"explanation_{i}_feature",
                         f"explanation_{i}_feature_value",
                         f"explanation_{i}_label",
                         f"explanation_{i}_qualitative_strength",
                         f"explanation_{i}_strength",
                     ]
                 )
-                if has_text_explanations:
-                    columns.append(f"explanation_{i}_per_ngram_text_explanations")
         pred_expl_list = []
 
         for i, row in enumerate(
             self.get_rows(exclude_adjusted_predictions=exclude_adjusted_predictions)
         ):
             data = [row.row_id, row.prediction]
             if adjusted_predictions_in_data:
@@ -618,34 +597,26 @@
                             pred_expl["feature"],
                             pred_expl["feature_value"],
                             pred_expl["label"],
                             pred_expl["qualitative_strength"],
                             pred_expl["strength"],
                         ]
                     )
-                    if has_text_explanations:
-                        data.append(
-                            json.dumps(pred_expl["per_ngram_text_explanations"], ensure_ascii=False)
-                        )
                 pred_expl_list.append(data + [None] * (len(columns) - len(data)))
             else:
                 for pred_expl in row.prediction_explanations:
                     data.extend(
                         [
                             pred_expl["feature"],
                             pred_expl["feature_value"],
                             pred_expl["label"],
                             pred_expl["qualitative_strength"],
                             pred_expl["strength"],
                         ]
                     )
-                    if has_text_explanations:
-                        data.append(
-                            json.dumps(pred_expl["per_ngram_text_explanations"], ensure_ascii=False)
-                        )
                 pred_expl_list.append(data + [None] * (len(columns) - len(data)))
 
         return pd.DataFrame(data=pred_expl_list, columns=columns)
 
     def download_to_csv(self, filename, encoding="utf-8", exclude_adjusted_predictions=True):
         """
         Save prediction explanations rows into CSV file.
@@ -862,8 +833,8 @@
         params = {
             "offset": offset,
             "exclude_adjusted_predictions": "true" if exclude_adjusted_predictions else "false",
         }
         if limit:
             params["limit"] = limit
         path = f"{cls._path_template.format(project_id)}{prediction_explanations_id}/"
-        return cls.from_location(path, keep_attrs=KEEP_ATTRS, params=params)
+        return cls.from_location(path, params=params)
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/prediction_server.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/predictions.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/prime_file.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/project.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/project_options.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/rating_table.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/recommended_model.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/relationships_configuration.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/relationships_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/residuals.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/restore_discarded_features.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/roc_curve.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/roc_curve.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,26 +16,43 @@
 import numpy as np
 import trafaret as t
 
 from datarobot._compat import Int, String
 from datarobot.models.api_object import APIObject
 
 if TYPE_CHECKING:
-    from datarobot.models.types import RocCurveEstimatedMetric
+    from mypy_extensions import TypedDict
+
+    class EstimatedMetric(TypedDict):
+        """Typed dict for estimated metric"""
+
+        accuracy: float
+        f1_score: float
+        false_negative_score: int
+        true_negative_score: int
+        true_negative_rate: float
+        matthews_correlation_coefficient: float
+        true_positive_score: int
+        positive_predictive_value: float
+        false_positive_score: int
+        false_positive_rate: float
+        negative_predictive_value: float
+        true_positive_rate: float
+        threshold: float
 
 
 class RocCurveThresholdMixin:  # pylint: disable=missing-class-docstring
-    roc_points: Optional[List[RocCurveEstimatedMetric]] = None
+    roc_points: Optional[List[EstimatedMetric]] = None
 
     @staticmethod
     def _validate_threshold(threshold: float) -> None:
         if threshold > 1 or threshold < 0:
             raise ValueError("threshold must be from [0, 1] interval")
 
-    def estimate_threshold(self, threshold: float) -> RocCurveEstimatedMetric:
+    def estimate_threshold(self, threshold: float) -> EstimatedMetric:
         """Return metrics estimation for given threshold.
 
         Parameters
         ----------
         threshold : float from [0, 1] interval
             Threshold we want estimation for
 
@@ -141,15 +158,15 @@
     """
 
     _converter = RocCurveTrafaret
 
     def __init__(
         self,
         source: str,
-        roc_points: List[RocCurveEstimatedMetric],
+        roc_points: List[EstimatedMetric],
         negative_class_predictions: List[float],
         positive_class_predictions: List[float],
         source_model_id: str,
     ) -> None:
         self.source = source
         self.roc_points = roc_points
         self.negative_class_predictions = negative_class_predictions
@@ -195,15 +212,15 @@
         .merge(RocCurveTrafaret)
         .ignore_extra("*")
     )
 
     def __init__(
         self,
         source: str,
-        roc_points: List[RocCurveEstimatedMetric],
+        roc_points: List[EstimatedMetric],
         negative_class_predictions: List[float],
         positive_class_predictions: List[float],
         source_model_id: str,
         label: str,
         kolmogorov_smirnov_metric: float,
         auc: float,
     ) -> None:
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/ruleset.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/secondary_dataset.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/segmentation.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/service_stats.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/service_stats.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/shap_impact.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/shap_matrix.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/shap_matrix_job.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/shap_matrix_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/sharing.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/trafarets.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/training_predictions.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/user_blueprints/models.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/user_blueprints/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -510,15 +510,15 @@
         datarobot.errors.ClientError
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
 
         Returns
         -------
-        :class:`requests.models.Response`
+        requests.models.Response
         """
         return cast(
             Response, cls._client.delete(cls._path.format(userBlueprintId=user_blueprint_id))
         )
 
     @classmethod
     def get_input_types(cls) -> UserBlueprintAvailableInput:
@@ -747,15 +747,15 @@
         datarobot.errors.ClientError
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
 
         Returns
         -------
-        :class:`requests.models.Response`
+        requests.models.Response
         """
         return UserBlueprintSharingUpdateController.update_shared_roles(
             user_blueprint_id=user_blueprint_id, roles=roles
         )
 
     @classmethod
     def search_catalog(
@@ -1369,15 +1369,15 @@
         datarobot.errors.ClientError
             if the server responded with 4xx status
         datarobot.errors.ServerError
             if the server responded with 5xx status
 
         Returns
         -------
-        :class:`requests.models.Response`
+        requests.models.Response
         """
         roles_json = []
         for role in roles:
             if not isinstance(
                 role,
                 (dict, GrantAccessControlWithUsernameValidator, GrantAccessControlWithIdValidator),
             ):
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/user_blueprints/trafarets.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/validators.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/visualai/augmentation.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/visualai/images.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/visualai/images.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/visualai/insights.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/visualai/insights.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/models/word_cloud.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/rest.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/rest.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/utils/__init__.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """This module is not considered part of the public interface. As of 2.3, anything here
 may change or be removed without warning."""
 from __future__ import annotations
 
 from collections import defaultdict
-from copy import deepcopy
 from datetime import date, datetime
 import re
 from typing import Any, cast, Dict, Iterable, List, Match, Optional, Tuple, TYPE_CHECKING, Union
 
 from dateutil import parser, tz
 import numpy as np
 import pandas as pd
@@ -71,17 +70,15 @@
     do_recursive: bool = True,
     keep_attrs: Optional[Union[Iterable[str], Iterable[List[str]]]] = None,
     keep_null_keys: bool = False,
 ) -> ServerDataType:
     if type(data) not in (dict, list):
         return data
     if isinstance(data, list):
-        return _from_api_list(
-            data, do_recursive=do_recursive, keep_attrs=keep_attrs, keep_null_keys=keep_null_keys
-        )
+        return _from_api_list(data, do_recursive=do_recursive, keep_null_keys=keep_null_keys)
     return _from_api_dict(
         data, do_recursive=do_recursive, keep_attrs=keep_attrs, keep_null_keys=keep_null_keys
     )
 
 
 # pylint: disable-next=missing-function-docstring
 def _from_api_dict(
@@ -108,37 +105,30 @@
         k_under = underscorize(k)
         if v is None and k_under not in current_level and not keep_null_keys:
             continue
         if do_recursive:
             data_val = from_api(
                 v,
                 do_recursive=do_recursive,
-                keep_attrs=deepcopy(next_level_attrs),
+                keep_attrs=next_level_attrs,
                 keep_null_keys=keep_null_keys,
             )
         else:
             data_val = v
         app_data[k_under] = data_val
     return app_data
 
 
 def _from_api_list(
     data: ServerDataListType,
     do_recursive: bool = True,
-    keep_attrs: Optional[Union[Iterable[str], Iterable[List[str]]]] = None,
     keep_null_keys: bool = False,
 ) -> List[Any]:
     return [
-        from_api(
-            datum,
-            do_recursive=do_recursive,
-            keep_attrs=deepcopy(keep_attrs),
-            keep_null_keys=keep_null_keys,
-        )
-        for datum in data
+        from_api(datum, do_recursive=do_recursive, keep_null_keys=keep_null_keys) for datum in data
     ]
 
 
 def remove_empty_keys(
     metadata: Dict[str, Any],
     keep_attrs: Optional[List[str]] = None,
 ) -> Dict[str, Any]:
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/utils/deprecation.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/utils/pagination.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/utils/retry.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/utils/source.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/utils/sourcedata.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot/utils/waiters.py` & `datarobot_early_access-3.2.0.2023.4.3/datarobot/utils/waiters.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot_early_access.egg-info/PKG-INFO` & `datarobot_early_access-3.2.0.2023.4.3/datarobot_early_access.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot-early-access
-Version: 3.2.0.2023.4.17
+Version: 3.2.0.2023.4.3
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/datarobot_early_access.egg-info/requires.txt` & `datarobot_early_access-3.2.0.2023.4.3/datarobot_early_access.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+contextlib2>=0.5.5
 pandas>=0.15
 numpy
 pyyaml>=3.11
-requests>=2.28.1
+requests>=2.21
 requests_toolbelt>=0.6
 trafaret!=1.1.0,<2.2,>=0.7
 urllib3>=1.23
 typing-extensions==4.3.0
 
 [dev]
 mock==3.0.5
@@ -22,20 +23,23 @@
 types-PyYAML==6.0.12
 types-python-dateutil==2.8.19
 types-pytz==2022.2.1.0
 types-requests==2.28.11
 types-urllib3==1.26.25
 Pillow==9.2.0
 Pillow==9.2.0
-Sphinx==4.3.2
-sphinx_rtd_theme==1.0.0
-nbsphinx==0.8.9
-numpydoc==1.4.0
+Sphinx==1.8.3
+sphinx_rtd_theme==0.1.9
+nbsphinx<1,>=0.2.9
+mistune==0.8.4
+nbconvert==5.3.1
+numpydoc>=0.6.0
 jupyter_contrib_nbextensions
-sphinx-autodoc-typehints==1.17.1
+tornado<6.0
+jsonschema<=4.3.1
 
 [examples]
 jupyter<=5.0
 fredapi==0.4.0
 matplotlib>=2.1.0
 seaborn<=0.8
 scikit-learn<=0.18.2
```

### Comparing `datarobot_early_access-3.2.0.2023.4.17/pyproject.toml` & `datarobot_early_access-3.2.0.2023.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/setup.py` & `datarobot_early_access-3.2.0.2023.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.4.17/setup_weekly.py` & `datarobot_early_access-3.2.0.2023.4.3/setup_weekly.py`

 * *Files identical despite different names*

