# Comparing `tmp/cognite_sdk-5.9.2.tar.gz` & `tmp/cognite_sdk-5.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-5.9.2.tar", max compression
+gzip compressed data, was "cognite_sdk-5.9.3.tar", max compression
```

## Comparing `cognite_sdk-5.9.2.tar` & `cognite_sdk-5.9.3.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0        0        0    11349 2023-03-27 18:30:06.397951 cognite_sdk-5.9.2/LICENSE
--rw-r--r--   0        0        0     3945 2023-03-27 18:30:06.397951 cognite_sdk-5.9.2/README.md
--rw-r--r--   0        0        0      427 2023-03-27 18:30:06.397951 cognite_sdk-5.9.2/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-03-27 18:30:06.397951 cognite_sdk-5.9.2/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6906 2023-03-27 18:30:06.397951 cognite_sdk-5.9.2/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    48459 2023-03-27 18:30:06.397951 cognite_sdk-5.9.2/cognite/client/_api/assets.py
--rw-r--r--   0        0        0    10748 2023-03-27 18:30:06.397951 cognite_sdk-5.9.2/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54567 2023-03-27 18:30:06.397951 cognite_sdk-5.9.2/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    76587 2023-03-27 18:30:06.397951 cognite_sdk-5.9.2/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12095 2023-03-27 18:30:06.397951 cognite_sdk-5.9.2/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-03-27 18:30:06.397951 cognite_sdk-5.9.2/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    20651 2023-03-27 18:30:06.397951 cognite_sdk-5.9.2/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17606 2023-03-27 18:30:06.397951 cognite_sdk-5.9.2/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41420 2023-03-27 18:30:06.397951 cognite_sdk-5.9.2/cognite/client/_api/files.py
--rw-r--r--   0        0        0    44788 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49923 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0    17931 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6011 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/labels.py
--rw-r--r--   0        0        0     1410 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/login.py
--rw-r--r--   0        0        0    24394 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22633 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37692 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7598 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    31841 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27450 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    18903 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    19361 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4910 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4672 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9285 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     2111 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    37003 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_api_client.py
--rw-r--r--   0        0        0     7283 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      258 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_constants.py
--rw-r--r--   0        0        0     6544 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/beta.py
--rw-r--r--   0        0        0     4380 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/config.py
--rw-r--r--   0        0        0    16808 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/credentials.py
--rw-r--r--   0        0        0     4985 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    18855 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     3344 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8746 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34145 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33551 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     6682 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    31534 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11008 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    15551 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13657 2023-03-27 18:30:06.401951 cognite_sdk-5.9.2/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16514 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16465 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     7962 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5868 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     1034 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/login.py
--rw-r--r--   0        0        0     4098 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12271 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17620 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     9370 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16814 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11789 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12078 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    24170 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    13108 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11425 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2354 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2451 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2747 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9418 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/py.typed
--rw-r--r--   0        0        0     8644 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/testing.py
--rw-r--r--   0        0        0      302 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     8780 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0    10121 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     5548 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     2842 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4149 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     1787 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/utils/_text.py
--rw-r--r--   0        0        0     5989 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     3313 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     1628 2023-03-27 18:30:06.405951 cognite_sdk-5.9.2/pyproject.toml
--rw-r--r--   0        0        0     5362 1970-01-01 00:00:00.000000 cognite_sdk-5.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-03-27 19:33:41.983133 cognite_sdk-5.9.3/LICENSE
+-rw-r--r--   0        0        0     3945 2023-03-27 19:33:41.983133 cognite_sdk-5.9.3/README.md
+-rw-r--r--   0        0        0      427 2023-03-27 19:33:41.983133 cognite_sdk-5.9.3/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-27 19:33:41.983133 cognite_sdk-5.9.3/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     6906 2023-03-27 19:33:41.983133 cognite_sdk-5.9.3/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    48459 2023-03-27 19:33:41.983133 cognite_sdk-5.9.3/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0    10748 2023-03-27 19:33:41.983133 cognite_sdk-5.9.3/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54567 2023-03-27 19:33:41.983133 cognite_sdk-5.9.3/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    76587 2023-03-27 19:33:41.983133 cognite_sdk-5.9.3/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12095 2023-03-27 19:33:41.983133 cognite_sdk-5.9.3/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-03-27 19:33:41.983133 cognite_sdk-5.9.3/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    20651 2023-03-27 19:33:41.983133 cognite_sdk-5.9.3/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17606 2023-03-27 19:33:41.983133 cognite_sdk-5.9.3/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41420 2023-03-27 19:33:41.983133 cognite_sdk-5.9.3/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    44855 2023-03-27 19:33:41.983133 cognite_sdk-5.9.3/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    49923 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0    17931 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6011 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0     1410 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api/login.py
+-rw-r--r--   0        0        0    24394 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22633 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    37692 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7598 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    31841 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    27450 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    18903 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    19361 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     4910 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4672 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9285 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     2111 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    37003 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     7283 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      258 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6544 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/beta.py
+-rw-r--r--   0        0        0     4380 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/config.py
+-rw-r--r--   0        0        0    16808 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/credentials.py
+-rw-r--r--   0        0        0     4985 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    18855 2023-03-27 19:33:41.987133 cognite_sdk-5.9.3/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     3344 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8746 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34145 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33551 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     6682 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    31534 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11008 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    15551 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13657 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16559 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16465 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     7962 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5868 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     1034 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/login.py
+-rw-r--r--   0        0        0     4098 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12271 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17620 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     9370 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16814 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11789 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12078 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    24170 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    13108 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11425 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2354 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2451 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2747 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9418 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/py.typed
+-rw-r--r--   0        0        0     8644 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/testing.py
+-rw-r--r--   0        0        0      302 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     8780 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0    10121 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     5548 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     2842 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4149 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     1787 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0     6091 2023-03-27 19:33:41.991133 cognite_sdk-5.9.3/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     3313 2023-03-27 19:33:41.995133 cognite_sdk-5.9.3/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     1628 2023-03-27 19:33:41.995133 cognite_sdk-5.9.3/pyproject.toml
+-rw-r--r--   0        0        0     5362 1970-01-01 00:00:00.000000 cognite_sdk-5.9.3/PKG-INFO
```

### Comparing `cognite_sdk-5.9.2/LICENSE` & `cognite_sdk-5.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/README.md` & `cognite_sdk-5.9.3/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/annotations.py` & `cognite_sdk-5.9.3/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/assets.py` & `cognite_sdk-5.9.3/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/data_sets.py` & `cognite_sdk-5.9.3/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-5.9.3/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/datapoints.py` & `cognite_sdk-5.9.3/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/diagrams.py` & `cognite_sdk-5.9.3/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/entity_matching.py` & `cognite_sdk-5.9.3/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/events.py` & `cognite_sdk-5.9.3/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-5.9.3/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/files.py` & `cognite_sdk-5.9.3/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/functions.py` & `cognite_sdk-5.9.3/cognite/client/_api/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -999,17 +999,16 @@
                 }
             ]
         }
 
         if data:
             body["items"][0]["data"] = data
 
-        url = "/functions/schedules"
-        res = self._post(url, json=body)
-        return FunctionSchedule._load(res.json()["items"][0])
+        res = self._post(self._RESOURCE_PATH, json=body)
+        return FunctionSchedule._load(res.json()["items"][0], cognite_client=self._cognite_client)
 
     def delete(self, id: int) -> None:
         """`Delete a schedule associated with a specific project. <https://docs.cognite.com/api/v1/#operation/deleteFunctionSchedules>`_
 
         Args:
             id (int): Id of the schedule
 
@@ -1022,30 +1021,31 @@
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> c.functions.schedules.delete(id = 123)
 
         """
         body = {"items": [{"id": id}]}
-        url = "/functions/schedules/delete"
+        url = f"{self._RESOURCE_PATH}/delete"
         self._post(url, json=body)
 
-    def get_input_data(self, id: int) -> Dict:
+    def get_input_data(self, id: int) -> Optional[Dict]:
         """`Retrieve the input data to the associated function. <https://docs.cognite.com/api/v1/#operation/getFunctionScheduleInputData>`_
         Args:
             id (int): Id of the schedule
 
         Returns:
-            Input data to the associated function. This data is passed
+            Optional[Dict]: Input data to the associated function or None if not set. This data is passed
             deserialized into the function through the data argument.
+
         Examples:
 
             Get schedule input data::
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
-                >>> c.functions.schedules.get_input_data(id = 123)
+                >>> c.functions.schedules.get_input_data(id=123)
         """
-        url = f"/functions/schedules/{id}/input_data"
+        url = f"{self._RESOURCE_PATH}/{id}/input_data"
         res = self._get(url)
 
-        return res.json()["data"]
+        return res.json().get("data")
```

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/geospatial.py` & `cognite_sdk-5.9.3/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/iam.py` & `cognite_sdk-5.9.3/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/labels.py` & `cognite_sdk-5.9.3/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/login.py` & `cognite_sdk-5.9.3/cognite/client/_api/login.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/raw.py` & `cognite_sdk-5.9.3/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/relationships.py` & `cognite_sdk-5.9.3/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/sequences.py` & `cognite_sdk-5.9.3/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-5.9.3/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/templates.py` & `cognite_sdk-5.9.3/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/three_d.py` & `cognite_sdk-5.9.3/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/time_series.py` & `cognite_sdk-5.9.3/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-5.9.3/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-5.9.3/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-5.9.3/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-5.9.3/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/transformations/schema.py` & `cognite_sdk-5.9.3/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api/vision.py` & `cognite_sdk-5.9.3/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_api_client.py` & `cognite_sdk-5.9.3/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_cognite_client.py` & `cognite_sdk-5.9.3/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_http_client.py` & `cognite_sdk-5.9.3/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-5.9.3/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-5.9.3/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-5.9.3/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_proto/data_points.proto` & `cognite_sdk-5.9.3/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-5.9.3/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-5.9.3/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-5.9.3/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-5.9.3/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-5.9.3/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-5.9.3/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/config.py` & `cognite_sdk-5.9.3/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/credentials.py` & `cognite_sdk-5.9.3/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/__init__.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/_base.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/annotations.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/assets.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/contextualization.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/data_sets.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/datapoints.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/events.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/files.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/functions.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,20 +233,20 @@
         self.function_external_id = function_external_id
         self.description = description
         self.cron_expression = cron_expression
         self.created_time = created_time
         self.session_id = session_id
         self._cognite_client = cast("CogniteClient", cognite_client)
 
-    def get_input_data(self) -> dict:
+    def get_input_data(self) -> Optional[dict]:
         """
         Retrieve the input data to the associated function.
 
         Returns:
-            Input data to the associated function. This data is passed
+            Optional[Dict]: Input data to the associated function or None if not set. This data is passed
             deserialized into the function through the data argument.
         """
         return self._cognite_client.functions.schedules.get_input_data(id=self.id)
 
 
 class FunctionSchedulesFilter(CogniteFilter):
     def __init__(
```

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/geospatial.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/iam.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/labels.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/login.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/login.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/raw.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/relationships.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/sequences.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/shared.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/templates.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/three_d.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/time_series.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-5.9.3/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/exceptions.py` & `cognite_sdk-5.9.3/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/testing.py` & `cognite_sdk-5.9.3/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/utils/_auxiliary.py` & `cognite_sdk-5.9.3/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/utils/_concurrency.py` & `cognite_sdk-5.9.3/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/utils/_graph.py` & `cognite_sdk-5.9.3/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/utils/_identifier.py` & `cognite_sdk-5.9.3/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/utils/_logging.py` & `cognite_sdk-5.9.3/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-5.9.3/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-5.9.3/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-5.9.3/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/utils/_text.py` & `cognite_sdk-5.9.3/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/cognite/client/utils/_time.py` & `cognite_sdk-5.9.3/cognite/client/utils/_time.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import numbers
 import re
 import time
 from datetime import datetime, timedelta, timezone
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union, overload
 
 UNIT_IN_MS_WITHOUT_WEEK = {"s": 1000, "m": 60000, "h": 3600000, "d": 86400000}
 UNIT_IN_MS = {**UNIT_IN_MS_WITHOUT_WEEK, "w": 604800000}
 
 MIN_TIMESTAMP_MS = -2208988800000  # 1900-01-01 00:00:00.000
 MAX_TIMESTAMP_MS = 4102444799999  # 2099-12-31 23:59:59.999
 
@@ -121,29 +121,36 @@
 
 
 def _convert_time_attributes_in_dict(item: Dict) -> Dict:
     new_item = {}
     for k, v in item.items():
         if k in TIME_ATTRIBUTES:
             try:
-                v = str(datetime.utcfromtimestamp(v / 1000))
-            except (ValueError, OSError):
+                v = str(ms_to_datetime(v).replace(tzinfo=None))
+            except ValueError:
                 pass
         new_item[k] = v
     return new_item
 
 
+@overload
+def convert_time_attributes_to_datetime(item: Dict) -> Dict:
+    ...
+
+
+@overload
+def convert_time_attributes_to_datetime(item: List[Dict]) -> List[Dict]:
+    ...
+
+
 def convert_time_attributes_to_datetime(item: Union[Dict, List[Dict]]) -> Union[Dict, List[Dict]]:
     if isinstance(item, dict):
         return _convert_time_attributes_in_dict(item)
     if isinstance(item, list):
-        new_items = []
-        for el in item:
-            new_items.append(_convert_time_attributes_in_dict(el))
-        return new_items
+        return list(map(_convert_time_attributes_in_dict, item))
     raise TypeError("item must be dict or list of dicts")
 
 
 def align_start_and_end_for_granularity(start: int, end: int, granularity: str) -> Tuple[int, int]:
     # Note the API always aligns `start` with 1s, 1m, 1h or 1d (even when given e.g. 73h)
     remainder = start % granularity_unit_to_ms(granularity)
     if remainder:
```

### Comparing `cognite_sdk-5.9.2/cognite/client/utils/_version_checker.py` & `cognite_sdk-5.9.3/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-5.9.2/pyproject.toml` & `cognite_sdk-5.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "5.9.2"
+version = "5.9.3"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 
 packages = [{ include="cognite", from="." }]
```

### Comparing `cognite_sdk-5.9.2/PKG-INFO` & `cognite_sdk-5.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 5.9.2
+Version: 5.9.3
 Summary: Cognite Python SDK
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 5.9.2 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 5.9.3 Summary: Cognite Python
 SDK Author: Erlend Vollset Author-email: erlend.vollset@cognite.com Requires-
 Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Provides-Extra: all Provides-Extra:
 functions Provides-Extra: geo Provides-Extra: numpy Provides-Extra: pandas
 Provides-Extra: pyodide Provides-Extra: sympy Requires-Dist: geopandas
```

