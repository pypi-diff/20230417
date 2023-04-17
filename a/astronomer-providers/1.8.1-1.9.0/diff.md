# Comparing `tmp/astronomer-providers-1.8.1.tar.gz` & `tmp/astronomer-providers-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astronomer-providers-1.8.1.tar", last modified: Thu Sep  1 15:14:49 2022, max compression
+gzip compressed data, was "astronomer-providers-1.9.0.tar", last modified: Tue Sep 13 11:12:20 2022, max compression
```

## Comparing `astronomer-providers-1.8.1.tar` & `astronomer-providers-1.9.0.tar`

### file list

```diff
@@ -1,235 +1,259 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.728909 astronomer-providers-1.8.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7872 2022-09-01 15:14:49.728909 astronomer-providers-1.8.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6269 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.500902 astronomer-providers-1.8.1/astronomer/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.504902 astronomer-providers-1.8.1/astronomer/providers/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.504902 astronomer-providers-1.8.1/astronomer/providers/amazon/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.504902 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.504902 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1607 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/example_aws_nuke.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10542 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/example_batch.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7422 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/example_emr_eks_containers_job.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3531 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/example_emr_sensor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8361 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/example_redshift_cluster_management.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7594 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/example_redshift_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7196 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/example_redshift_sql.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4475 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/example_s3.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.508902 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3724 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/base_aws.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      781 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/base_aws_async.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10209 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/batch_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7586 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/emr.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7551 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/redshift_cluster.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9267 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/redshift_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3104 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/redshift_sql.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14590 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/s3.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.508902 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/operators/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/operators/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3878 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/operators/batch.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3092 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/operators/emr.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9701 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/operators/redshift_cluster.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2976 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/operators/redshift_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2820 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/operators/redshift_sql.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.508902 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/sensors/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/sensors/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2142 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/sensors/batch.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6038 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/sensors/emr.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2284 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/sensors/redshift_cluster.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9178 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/sensors/s3.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.508902 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/triggers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/triggers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7179 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/triggers/batch.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12601 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/triggers/emr.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6984 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/triggers/redshift_cluster.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2249 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/triggers/redshift_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2109 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/triggers/redshift_sql.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7766 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/amazon/aws/triggers/s3.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.508902 astronomer-providers-1.8.1/astronomer/providers/apache/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.508902 astronomer-providers-1.8.1/astronomer/providers/apache/hive/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/hive/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.508902 astronomer-providers-1.8.1/astronomer/providers/apache/hive/example_dags/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/hive/example_dags/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14479 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/hive/example_dags/example_hive.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.508902 astronomer-providers-1.8.1/astronomer/providers/apache/hive/hooks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/hive/hooks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3879 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/hive/hooks/hive.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.508902 astronomer-providers-1.8.1/astronomer/providers/apache/hive/sensors/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/hive/sensors/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3189 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/hive/sensors/hive_partition.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2993 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/hive/sensors/named_hive_partition.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.508902 astronomer-providers-1.8.1/astronomer/providers/apache/hive/triggers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/hive/triggers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2549 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/hive/triggers/hive_partition.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2650 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/hive/triggers/named_hive_partition.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.508902 astronomer-providers-1.8.1/astronomer/providers/apache/livy/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/livy/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.508902 astronomer-providers-1.8.1/astronomer/providers/apache/livy/example_dags/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/livy/example_dags/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11913 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/livy/example_dags/example_livy.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.512902 astronomer-providers-1.8.1/astronomer/providers/apache/livy/hooks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/livy/hooks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15936 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/livy/hooks/livy.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.512902 astronomer-providers-1.8.1/astronomer/providers/apache/livy/operators/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/livy/operators/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3856 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/livy/operators/livy.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.512902 astronomer-providers-1.8.1/astronomer/providers/apache/livy/triggers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/livy/triggers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5504 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/apache/livy/triggers/livy.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.512902 astronomer-providers-1.8.1/astronomer/providers/cncf/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/cncf/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.512902 astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.512902 astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/example_dags/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/example_dags/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1666 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/example_dags/example_kubernetes_pod_operator.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.512902 astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/hooks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/hooks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3135 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/hooks/kubernetes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      819 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/hooks/kubernetes_async.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.512902 astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/operators/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/operators/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6206 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/operators/kubernetes_pod.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.512902 astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/triggers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/triggers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6475 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/triggers/wait_container.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.512902 astronomer-providers-1.8.1/astronomer/providers/core/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/core/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.512902 astronomer-providers-1.8.1/astronomer/providers/core/example_dags/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/core/example_dags/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2134 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/core/example_dags/example_external_task.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      885 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/core/example_dags/example_external_task_wait_for_me.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      994 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/core/example_dags/example_file_sensor.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.512902 astronomer-providers-1.8.1/astronomer/providers/core/sensors/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/core/sensors/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3399 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/core/sensors/external_task.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1973 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/core/sensors/filesystem.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.512902 astronomer-providers-1.8.1/astronomer/providers/core/triggers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/core/triggers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5269 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/core/triggers/external_task.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2075 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/core/triggers/filesystem.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.512902 astronomer-providers-1.8.1/astronomer/providers/databricks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/databricks/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.512902 astronomer-providers-1.8.1/astronomer/providers/databricks/example_dags/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/databricks/example_dags/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2510 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/databricks/example_dags/example_databricks.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.512902 astronomer-providers-1.8.1/astronomer/providers/databricks/hooks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/databricks/hooks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5917 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/databricks/hooks/databricks.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.512902 astronomer-providers-1.8.1/astronomer/providers/databricks/operators/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/databricks/operators/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5310 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/databricks/operators/databricks.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.516902 astronomer-providers-1.8.1/astronomer/providers/databricks/triggers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/databricks/triggers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4062 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/databricks/triggers/databricks.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.516902 astronomer-providers-1.8.1/astronomer/providers/google/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.516902 astronomer-providers-1.8.1/astronomer/providers/google/cloud/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.516902 astronomer-providers-1.8.1/astronomer/providers/google/cloud/example_dags/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/example_dags/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7990 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/example_dags/example_bigquery_queries.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3478 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/example_dags/example_bigquery_sensors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7271 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/example_dags/example_dataproc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3336 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/example_dags/example_gcp_nuke.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4652 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/example_dags/example_gcs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2140 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/example_dags/example_kubernetes_engine.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.516902 astronomer-providers-1.8.1/astronomer/providers/google/cloud/extractors/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/extractors/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5931 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/extractors/bigquery.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.516902 astronomer-providers-1.8.1/astronomer/providers/google/cloud/hooks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/hooks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12574 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/hooks/bigquery.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5615 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/hooks/dataproc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      801 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/hooks/gcs.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.516902 astronomer-providers-1.8.1/astronomer/providers/google/cloud/operators/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/operators/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19242 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/operators/bigquery.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19093 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/operators/dataproc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5730 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/operators/kubernetes_engine.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.516902 astronomer-providers-1.8.1/astronomer/providers/google/cloud/sensors/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/sensors/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3788 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/sensors/bigquery.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13401 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/sensors/gcs.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.516902 astronomer-providers-1.8.1/astronomer/providers/google/cloud/triggers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/triggers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21910 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/triggers/bigquery.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13731 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/triggers/dataproc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17721 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/triggers/gcs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5414 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/cloud/triggers/kubernetes_engine.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.516902 astronomer-providers-1.8.1/astronomer/providers/google/common/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/common/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.516902 astronomer-providers-1.8.1/astronomer/providers/google/common/hooks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/common/hooks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      912 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/google/common/hooks/base_google.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.516902 astronomer-providers-1.8.1/astronomer/providers/http/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/http/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.516902 astronomer-providers-1.8.1/astronomer/providers/http/example_dags/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/http/example_dags/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1161 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/http/example_dags/example_http.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.520902 astronomer-providers-1.8.1/astronomer/providers/http/hooks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/http/hooks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5793 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/http/hooks/http.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.520902 astronomer-providers-1.8.1/astronomer/providers/http/sensors/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/http/sensors/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5045 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/http/sensors/http.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.520902 astronomer-providers-1.8.1/astronomer/providers/http/triggers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/http/triggers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3294 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/http/triggers/http.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.520902 astronomer-providers-1.8.1/astronomer/providers/microsoft/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/microsoft/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.520902 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.520902 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/example_dags/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/example_dags/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8686 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/example_dags/example_adf_run_pipeline.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5723 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/example_dags/example_wasb_sensors.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.520902 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/hooks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/hooks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5244 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/hooks/data_factory.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6146 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/hooks/wasb.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.520902 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/operators/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/operators/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4564 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/operators/data_factory.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.520902 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/sensors/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/sensors/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2145 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/sensors/data_factory.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5327 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/sensors/wasb.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.520902 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/triggers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/triggers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8554 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/triggers/data_factory.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6659 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/triggers/wasb.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.520902 astronomer-providers-1.8.1/astronomer/providers/snowflake/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/snowflake/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.728909 astronomer-providers-1.8.1/astronomer/providers/snowflake/example_dags/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/snowflake/example_dags/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2306 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/snowflake/example_dags/example_snowflake.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1706 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/snowflake/example_dags/example_snowflake_sql_api.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.728909 astronomer-providers-1.8.1/astronomer/providers/snowflake/extractors/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/snowflake/extractors/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6553 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/snowflake/extractors/snowflake.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.728909 astronomer-providers-1.8.1/astronomer/providers/snowflake/hooks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/snowflake/hooks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6382 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/snowflake/hooks/snowflake.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11295 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/snowflake/hooks/snowflake_sql_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6081 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/snowflake/hooks/sql_api_generate_jwt.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.728909 astronomer-providers-1.8.1/astronomer/providers/snowflake/operators/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/snowflake/operators/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13903 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/snowflake/operators/snowflake.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.728909 astronomer-providers-1.8.1/astronomer/providers/snowflake/triggers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/snowflake/triggers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5911 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/astronomer/providers/snowflake/triggers/snowflake_trigger.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-01 15:14:49.728909 astronomer-providers-1.8.1/astronomer_providers.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7872 2022-09-01 15:14:49.000000 astronomer-providers-1.8.1/astronomer_providers.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9170 2022-09-01 15:14:49.000000 astronomer-providers-1.8.1/astronomer_providers.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-09-01 15:14:49.000000 astronomer-providers-1.8.1/astronomer_providers.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       32 2022-09-01 15:14:49.000000 astronomer-providers-1.8.1/astronomer_providers.egg-info/namespace_packages.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-09-01 15:14:49.000000 astronomer-providers-1.8.1/astronomer_providers.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1827 2022-09-01 15:14:49.000000 astronomer-providers-1.8.1/astronomer_providers.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       11 2022-09-01 15:14:49.000000 astronomer-providers-1.8.1/astronomer_providers.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      994 2022-09-01 15:14:44.000000 astronomer-providers-1.8.1/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3778 2022-09-01 15:14:49.728909 astronomer-providers-1.8.1/setup.cfg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.254918 astronomer-providers-1.9.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7994 2022-09-13 11:12:20.254918 astronomer-providers-1.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6365 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/README.rst
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.226917 astronomer-providers-1.9.0/astronomer/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.230918 astronomer-providers-1.9.0/astronomer/providers/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.230918 astronomer-providers-1.9.0/astronomer/providers/amazon/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.230918 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.234917 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1607 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/example_aws_nuke.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10542 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/example_batch.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7422 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/example_emr_eks_containers_job.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3531 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/example_emr_sensor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8361 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/example_redshift_cluster_management.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7594 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/example_redshift_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7196 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/example_redshift_sql.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4475 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/example_s3.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.234917 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/extractors/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/extractors/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1025 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/extractors/redshift.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.234917 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3724 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/base_aws.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      781 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/base_aws_async.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10209 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/batch_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7586 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/emr.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7551 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/redshift_cluster.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9267 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/redshift_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3104 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/redshift_sql.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14590 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/s3.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.234917 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/operators/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/operators/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3878 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/operators/batch.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3092 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/operators/emr.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9701 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/operators/redshift_cluster.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3045 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/operators/redshift_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2889 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/operators/redshift_sql.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.234917 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/sensors/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/sensors/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2142 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/sensors/batch.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6038 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/sensors/emr.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2284 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/sensors/redshift_cluster.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9178 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/sensors/s3.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.238917 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/triggers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/triggers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7179 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/triggers/batch.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12601 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/triggers/emr.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6984 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/triggers/redshift_cluster.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2249 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/triggers/redshift_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2109 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/triggers/redshift_sql.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7766 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/amazon/aws/triggers/s3.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.238917 astronomer-providers-1.9.0/astronomer/providers/apache/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.238917 astronomer-providers-1.9.0/astronomer/providers/apache/hive/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/hive/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.238917 astronomer-providers-1.9.0/astronomer/providers/apache/hive/example_dags/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/hive/example_dags/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14479 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/hive/example_dags/example_hive.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.238917 astronomer-providers-1.9.0/astronomer/providers/apache/hive/hooks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/hive/hooks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3879 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/hive/hooks/hive.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.238917 astronomer-providers-1.9.0/astronomer/providers/apache/hive/sensors/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/hive/sensors/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3189 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/hive/sensors/hive_partition.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2993 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/hive/sensors/named_hive_partition.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.238917 astronomer-providers-1.9.0/astronomer/providers/apache/hive/triggers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/hive/triggers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2549 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/hive/triggers/hive_partition.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2650 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/hive/triggers/named_hive_partition.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.238917 astronomer-providers-1.9.0/astronomer/providers/apache/livy/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/livy/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.238917 astronomer-providers-1.9.0/astronomer/providers/apache/livy/example_dags/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/livy/example_dags/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11913 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/livy/example_dags/example_livy.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.238917 astronomer-providers-1.9.0/astronomer/providers/apache/livy/hooks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/livy/hooks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15936 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/livy/hooks/livy.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.238917 astronomer-providers-1.9.0/astronomer/providers/apache/livy/operators/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/livy/operators/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3856 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/livy/operators/livy.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.238917 astronomer-providers-1.9.0/astronomer/providers/apache/livy/triggers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/livy/triggers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5504 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/apache/livy/triggers/livy.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.238917 astronomer-providers-1.9.0/astronomer/providers/cncf/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/cncf/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.238917 astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.238917 astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/example_dags/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/example_dags/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1666 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/example_dags/example_kubernetes_pod_operator.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/hooks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/hooks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3135 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/hooks/kubernetes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      819 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/hooks/kubernetes_async.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/operators/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/operators/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6206 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/operators/kubernetes_pod.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/triggers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/triggers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6475 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/triggers/wait_container.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/core/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/core/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/core/example_dags/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/core/example_dags/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2134 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/core/example_dags/example_external_task.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      885 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/core/example_dags/example_external_task_wait_for_me.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      994 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/core/example_dags/example_file_sensor.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/core/sensors/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/core/sensors/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3399 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/core/sensors/external_task.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1973 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/core/sensors/filesystem.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/core/triggers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/core/triggers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5269 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/core/triggers/external_task.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2075 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/core/triggers/filesystem.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/databricks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/databricks/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/databricks/example_dags/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/databricks/example_dags/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2510 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/databricks/example_dags/example_databricks.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/databricks/hooks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/databricks/hooks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5917 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/databricks/hooks/databricks.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/databricks/operators/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/databricks/operators/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5310 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/databricks/operators/databricks.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/databricks/triggers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/databricks/triggers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4062 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/databricks/triggers/databricks.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/dbt/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/dbt/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/dbt/cloud/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/dbt/cloud/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/dbt/cloud/example_dags/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/dbt/cloud/example_dags/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2219 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/dbt/cloud/example_dags/example_dbt_cloud.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/dbt/cloud/hooks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/dbt/cloud/hooks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5651 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/dbt/cloud/hooks/dbt.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/dbt/cloud/operators/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/dbt/cloud/operators/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3652 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/dbt/cloud/operators/dbt.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.242918 astronomer-providers-1.9.0/astronomer/providers/dbt/cloud/sensors/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/dbt/cloud/sensors/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2230 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/dbt/cloud/sensors/dbt.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.246918 astronomer-providers-1.9.0/astronomer/providers/dbt/cloud/triggers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/dbt/cloud/triggers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4143 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/dbt/cloud/triggers/dbt.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.246918 astronomer-providers-1.9.0/astronomer/providers/google/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.246918 astronomer-providers-1.9.0/astronomer/providers/google/cloud/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.246918 astronomer-providers-1.9.0/astronomer/providers/google/cloud/example_dags/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/example_dags/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7990 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/example_dags/example_bigquery_queries.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3478 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/example_dags/example_bigquery_sensors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7271 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/example_dags/example_dataproc.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3336 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/example_dags/example_gcp_nuke.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4652 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/example_dags/example_gcs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2140 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/example_dags/example_kubernetes_engine.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.246918 astronomer-providers-1.9.0/astronomer/providers/google/cloud/extractors/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/extractors/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5926 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/extractors/bigquery.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.246918 astronomer-providers-1.9.0/astronomer/providers/google/cloud/hooks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/hooks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10101 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/hooks/bigquery.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5615 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/hooks/dataproc.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      801 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/hooks/gcs.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.246918 astronomer-providers-1.9.0/astronomer/providers/google/cloud/operators/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/operators/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18763 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/operators/bigquery.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19093 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/operators/dataproc.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5730 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/operators/kubernetes_engine.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.246918 astronomer-providers-1.9.0/astronomer/providers/google/cloud/sensors/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/sensors/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3788 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/sensors/bigquery.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13401 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/sensors/gcs.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.246918 astronomer-providers-1.9.0/astronomer/providers/google/cloud/triggers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/triggers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21910 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/triggers/bigquery.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13731 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/triggers/dataproc.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17721 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/triggers/gcs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5414 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/cloud/triggers/kubernetes_engine.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.250918 astronomer-providers-1.9.0/astronomer/providers/google/common/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/common/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.250918 astronomer-providers-1.9.0/astronomer/providers/google/common/hooks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/common/hooks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      912 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/google/common/hooks/base_google.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.250918 astronomer-providers-1.9.0/astronomer/providers/http/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/http/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.250918 astronomer-providers-1.9.0/astronomer/providers/http/example_dags/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/http/example_dags/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1161 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/http/example_dags/example_http.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.250918 astronomer-providers-1.9.0/astronomer/providers/http/hooks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/http/hooks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5793 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/http/hooks/http.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.250918 astronomer-providers-1.9.0/astronomer/providers/http/sensors/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/http/sensors/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5045 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/http/sensors/http.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.250918 astronomer-providers-1.9.0/astronomer/providers/http/triggers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/http/triggers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3294 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/http/triggers/http.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.250918 astronomer-providers-1.9.0/astronomer/providers/microsoft/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/microsoft/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.250918 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.250918 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/example_dags/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/example_dags/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8686 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/example_dags/example_adf_run_pipeline.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5723 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/example_dags/example_wasb_sensors.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.250918 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/hooks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/hooks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5244 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/hooks/data_factory.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6146 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/hooks/wasb.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.250918 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/operators/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/operators/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4564 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/operators/data_factory.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.250918 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/sensors/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/sensors/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2145 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/sensors/data_factory.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5327 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/sensors/wasb.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.250918 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/triggers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/triggers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8554 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/triggers/data_factory.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6659 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/triggers/wasb.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/package.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.250918 astronomer-providers-1.9.0/astronomer/providers/snowflake/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/snowflake/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.250918 astronomer-providers-1.9.0/astronomer/providers/snowflake/example_dags/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/snowflake/example_dags/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2306 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/snowflake/example_dags/example_snowflake.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1706 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/snowflake/example_dags/example_snowflake_sql_api.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.254918 astronomer-providers-1.9.0/astronomer/providers/snowflake/extractors/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/snowflake/extractors/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6553 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/snowflake/extractors/snowflake.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.254918 astronomer-providers-1.9.0/astronomer/providers/snowflake/hooks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/snowflake/hooks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6382 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/snowflake/hooks/snowflake.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11295 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/snowflake/hooks/snowflake_sql_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6081 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/snowflake/hooks/sql_api_generate_jwt.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.254918 astronomer-providers-1.9.0/astronomer/providers/snowflake/operators/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/snowflake/operators/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13903 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/snowflake/operators/snowflake.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.254918 astronomer-providers-1.9.0/astronomer/providers/snowflake/triggers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/snowflake/triggers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5911 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/astronomer/providers/snowflake/triggers/snowflake_trigger.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-09-13 11:12:20.254918 astronomer-providers-1.9.0/astronomer_providers.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7994 2022-09-13 11:12:20.000000 astronomer-providers-1.9.0/astronomer_providers.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9950 2022-09-13 11:12:20.000000 astronomer-providers-1.9.0/astronomer_providers.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-09-13 11:12:20.000000 astronomer-providers-1.9.0/astronomer_providers.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       89 2022-09-13 11:12:20.000000 astronomer-providers-1.9.0/astronomer_providers.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       32 2022-09-13 11:12:20.000000 astronomer-providers-1.9.0/astronomer_providers.egg-info/namespace_packages.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-09-13 11:12:19.000000 astronomer-providers-1.9.0/astronomer_providers.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1926 2022-09-13 11:12:20.000000 astronomer-providers-1.9.0/astronomer_providers.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       11 2022-09-13 11:12:20.000000 astronomer-providers-1.9.0/astronomer_providers.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      994 2022-09-13 11:12:14.000000 astronomer-providers-1.9.0/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3992 2022-09-13 11:12:20.254918 astronomer-providers-1.9.0/setup.cfg
```

### Comparing `astronomer-providers-1.8.1/PKG-INFO` & `astronomer-providers-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-providers
-Version: 1.8.1
+Version: 1.9.0
 Summary: Apache Airflow Providers containing Deferrable Operators & Sensors from Astronomer
 Home-page: https://github.com/astronomer/astronomer-providers/
 Author: Astronomer
 Author-email: humans@astronomer.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/astronomer/astronomer-providers/
 Project-URL: Homepage, https://astronomer.io/
@@ -25,14 +25,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Provides-Extra: amazon
 Provides-Extra: apache.hive
 Provides-Extra: apache.livy
 Provides-Extra: cncf.kubernetes
 Provides-Extra: databricks
+Provides-Extra: dbt.cloud
 Provides-Extra: google
 Provides-Extra: http
 Provides-Extra: microsoft.azure
 Provides-Extra: snowflake
 Provides-Extra: openlineage
 Provides-Extra: docs
 Provides-Extra: tests
@@ -120,14 +121,18 @@
      - ``pip install 'astronomer-providers[cncf.kubernetes]'``
      - Cncf Kubernetes
 
    * - ``databricks``
      - ``pip install 'astronomer-providers[databricks]'``
      - Databricks
 
+   * - ``dbt.cloud``
+     - ``pip install 'astronomer-providers[dbt.cloud]'``
+     - Dbt Cloud
+
    * - ``google``
      - ``pip install 'astronomer-providers[google]'``
      - Google
 
    * - ``http``
      - ``pip install 'astronomer-providers[http]'``
      - Http
```

### Comparing `astronomer-providers-1.8.1/README.rst` & `astronomer-providers-1.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,18 @@
      - ``pip install 'astronomer-providers[cncf.kubernetes]'``
      - Cncf Kubernetes
 
    * - ``databricks``
      - ``pip install 'astronomer-providers[databricks]'``
      - Databricks
 
+   * - ``dbt.cloud``
+     - ``pip install 'astronomer-providers[dbt.cloud]'``
+     - Dbt Cloud
+
    * - ``google``
      - ``pip install 'astronomer-providers[google]'``
      - Google
 
    * - ``http``
      - ``pip install 'astronomer-providers[http]'``
      - Http
```

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/example_aws_nuke.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/example_aws_nuke.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/example_batch.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/example_batch.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/example_emr_eks_containers_job.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/example_emr_eks_containers_job.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/example_emr_sensor.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/example_emr_sensor.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/example_redshift_cluster_management.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/example_redshift_cluster_management.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/example_redshift_data.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/example_redshift_data.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/example_redshift_sql.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/example_redshift_sql.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/example_dags/example_s3.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/example_dags/example_s3.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/base_aws.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/base_aws.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/base_aws_async.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/base_aws_async.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/batch_client.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/batch_client.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/emr.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/emr.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/redshift_cluster.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/redshift_data.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/redshift_data.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/redshift_sql.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/redshift_sql.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/hooks/s3.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/hooks/s3.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/operators/batch.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/operators/batch.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/operators/emr.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/operators/emr.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/operators/redshift_cluster.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/operators/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/operators/redshift_data.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/operators/redshift_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         defers trigger to poll for the status for the queries executed.
         """
         redshift_data_hook = RedshiftDataHook(aws_conn_id=self.aws_conn_id)
         query_ids, response = redshift_data_hook.execute_query(sql=self.sql, params=self.params)
         self.log.info("Query IDs %s", query_ids)
         if response.get("status") == "error":
             self.execute_complete(context, event=response)
+        context["ti"].xcom_push(key="return_value", value=query_ids)
         self.defer(
             timeout=self.execution_timeout,
             trigger=RedshiftDataTrigger(
                 task_id=self.task_id,
                 poll_interval=self.poll_interval,
                 aws_conn_id=self.aws_conn_id,
                 query_ids=query_ids,
```

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/operators/redshift_sql.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/operators/redshift_sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         defers trigger to poll for the status for the query executed
         """
         redshift_data_hook = RedshiftDataHook(aws_conn_id=self.redshift_conn_id)
         query_ids, response = redshift_data_hook.execute_query(sql=cast(str, self.sql), params=self.params)
         if response.get("status") == "error":
             self.execute_complete({}, response)
             return
+        context["ti"].xcom_push(key="return_value", value=query_ids)
         self.defer(
             timeout=self.execution_timeout,
             trigger=RedshiftSQLTrigger(
                 task_id=self.task_id,
                 polling_period_seconds=self.poll_interval,
                 aws_conn_id=self.redshift_conn_id,
                 query_ids=query_ids,
```

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/sensors/batch.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/sensors/batch.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/sensors/emr.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/sensors/emr.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/sensors/redshift_cluster.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/sensors/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/sensors/s3.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/sensors/s3.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/triggers/batch.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/triggers/batch.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/triggers/emr.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/triggers/emr.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/triggers/redshift_cluster.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/triggers/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/triggers/redshift_data.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/triggers/redshift_data.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/triggers/redshift_sql.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/triggers/redshift_sql.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/amazon/aws/triggers/s3.py` & `astronomer-providers-1.9.0/astronomer/providers/amazon/aws/triggers/s3.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/apache/hive/example_dags/example_hive.py` & `astronomer-providers-1.9.0/astronomer/providers/apache/hive/example_dags/example_hive.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/apache/hive/hooks/hive.py` & `astronomer-providers-1.9.0/astronomer/providers/apache/hive/hooks/hive.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/apache/hive/sensors/hive_partition.py` & `astronomer-providers-1.9.0/astronomer/providers/apache/hive/sensors/hive_partition.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/apache/hive/sensors/named_hive_partition.py` & `astronomer-providers-1.9.0/astronomer/providers/apache/hive/sensors/named_hive_partition.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/apache/hive/triggers/hive_partition.py` & `astronomer-providers-1.9.0/astronomer/providers/apache/hive/triggers/hive_partition.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/apache/hive/triggers/named_hive_partition.py` & `astronomer-providers-1.9.0/astronomer/providers/apache/hive/triggers/named_hive_partition.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/apache/livy/example_dags/example_livy.py` & `astronomer-providers-1.9.0/astronomer/providers/apache/livy/example_dags/example_livy.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/apache/livy/hooks/livy.py` & `astronomer-providers-1.9.0/astronomer/providers/apache/livy/hooks/livy.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/apache/livy/operators/livy.py` & `astronomer-providers-1.9.0/astronomer/providers/apache/livy/operators/livy.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/apache/livy/triggers/livy.py` & `astronomer-providers-1.9.0/astronomer/providers/apache/livy/triggers/livy.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/example_dags/example_kubernetes_pod_operator.py` & `astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/example_dags/example_kubernetes_pod_operator.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/hooks/kubernetes.py` & `astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/hooks/kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/hooks/kubernetes_async.py` & `astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/hooks/kubernetes_async.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/operators/kubernetes_pod.py` & `astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/operators/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/cncf/kubernetes/triggers/wait_container.py` & `astronomer-providers-1.9.0/astronomer/providers/cncf/kubernetes/triggers/wait_container.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/core/example_dags/example_external_task.py` & `astronomer-providers-1.9.0/astronomer/providers/core/example_dags/example_external_task.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/core/example_dags/example_external_task_wait_for_me.py` & `astronomer-providers-1.9.0/astronomer/providers/core/example_dags/example_external_task_wait_for_me.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/core/example_dags/example_file_sensor.py` & `astronomer-providers-1.9.0/astronomer/providers/core/example_dags/example_file_sensor.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/core/sensors/external_task.py` & `astronomer-providers-1.9.0/astronomer/providers/core/sensors/external_task.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/core/sensors/filesystem.py` & `astronomer-providers-1.9.0/astronomer/providers/core/sensors/filesystem.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/core/triggers/external_task.py` & `astronomer-providers-1.9.0/astronomer/providers/core/triggers/external_task.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/core/triggers/filesystem.py` & `astronomer-providers-1.9.0/astronomer/providers/core/triggers/filesystem.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/databricks/example_dags/example_databricks.py` & `astronomer-providers-1.9.0/astronomer/providers/databricks/example_dags/example_databricks.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/databricks/hooks/databricks.py` & `astronomer-providers-1.9.0/astronomer/providers/databricks/hooks/databricks.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/databricks/operators/databricks.py` & `astronomer-providers-1.9.0/astronomer/providers/databricks/operators/databricks.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/databricks/triggers/databricks.py` & `astronomer-providers-1.9.0/astronomer/providers/databricks/triggers/databricks.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/example_dags/example_bigquery_queries.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/example_dags/example_bigquery_queries.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/example_dags/example_bigquery_sensors.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/example_dags/example_bigquery_sensors.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/example_dags/example_dataproc.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/example_dags/example_dataproc.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/example_dags/example_gcp_nuke.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/example_dags/example_gcp_nuke.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/example_dags/example_gcs.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/example_dags/example_gcs.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/example_dags/example_kubernetes_engine.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/example_dags/example_kubernetes_engine.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/extractors/bigquery.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/extractors/bigquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import json
 from typing import Any, List, Optional, Union
 
 import attr
 from airflow.exceptions import AirflowException
 from airflow.models.taskinstance import TaskInstance
+from airflow.providers.google.cloud.hooks.bigquery import BigQueryHook
 from google.cloud.bigquery import Client
 from openlineage.airflow.extractors.base import BaseExtractor, TaskMetadata
 from openlineage.airflow.utils import get_job_name
 from openlineage.client.facet import SqlJobFacet
 from openlineage.common.provider.bigquery import BigQueryDatasetsProvider
 from openlineage.common.sql import parse
 
-from astronomer.providers.google.cloud.hooks.bigquery import _BigQueryHook
 from astronomer.providers.google.cloud.operators.bigquery import (
     BigQueryCheckOperatorAsync,
     BigQueryGetDataOperatorAsync,
     BigQueryInsertJobOperatorAsync,
     BigQueryIntervalCheckOperatorAsync,
     BigQueryValueCheckOperatorAsync,
 )
@@ -52,15 +52,15 @@
 
     def _get_big_query_client(self) -> Client:
         """
         Gets the BigQuery client to fetch job metadata.
         The method checks whether a connection hook is available with the Airflow configuration for the operator, and
         if yes, returns the same connection. Otherwise, returns the Client instance of``google.cloud.bigquery``.
         """
-        hook = _BigQueryHook(gcp_conn_id=self.operator.gcp_conn_id)
+        hook = BigQueryHook(gcp_conn_id=self.operator.gcp_conn_id)
         return hook.get_client(project_id=hook.project_id, location=hook.location)
 
     def _get_xcom_bigquery_job_id(self, task_instance: TaskInstance) -> Any:
         """
         Pulls the BigQuery Job ID from XCOM for the task instance whose metadata needs to be extracted.
 
         :param task_instance: Instance of the Airflow task whose BigQuery ``job_id`` needs to be pulled from XCOM.
```

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/hooks/bigquery.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/hooks/bigquery.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,87 +1,25 @@
 from typing import Any, Dict, List, Optional, Union, cast
 
 from aiohttp import ClientSession as ClientSession
 from airflow.exceptions import AirflowException
 from airflow.providers.google.cloud.hooks.bigquery import BigQueryHook
-from airflow.providers.google.common.hooks.base_google import GoogleBaseHook
 from gcloud.aio.bigquery import Job, Table
 from google.cloud.bigquery import CopyJob, ExtractJob, LoadJob, QueryJob
 from requests import Session
 
 from astronomer.providers.google.common.hooks.base_google import GoogleBaseHookAsync
 
 BigQueryJob = Union[CopyJob, QueryJob, LoadJob, ExtractJob]
 
 
-class _BigQueryHook(BigQueryHook):
-    @GoogleBaseHook.fallback_to_default_project_id
-    def insert_job(
-        self,
-        configuration: Dict[str, Any],
-        job_id: Optional[str] = None,
-        project_id: Optional[str] = None,
-        location: Optional[str] = None,
-        nowait: bool = False,
-    ) -> BigQueryJob:
-        """
-        Executes a BigQuery job. Initiates the job and returns job id.
-
-        See here: https://cloud.google.com/bigquery/docs/reference/v2/jobs
-
-        :param configuration: The configuration parameter maps directly to
-            BigQuery's configuration field in the job object. See
-            https://cloud.google.com/bigquery/docs/reference/v2/jobs for
-            details.
-        :param job_id: The ID of the job. The ID must contain only letters (a-z, A-Z),
-            numbers (0-9), underscores (_), or dashes (-). The maximum length is 1,024
-            characters. If not provided then uuid will be generated.
-        :param project_id: Google Cloud Project where the job is running
-        :param location: location the job is running
-        :param nowait: specify whether to insert job without waiting for the result
-        """
-        location = location or self.location
-        job_id = job_id or self._custom_job_id(configuration)
-
-        client = self.get_client(project_id=project_id, location=location)
-        job_data = {
-            "configuration": configuration,
-            "jobReference": {"jobId": job_id, "projectId": project_id, "location": location},
-        }
-
-        supported_jobs = {
-            LoadJob._JOB_TYPE: LoadJob,
-            CopyJob._JOB_TYPE: CopyJob,
-            ExtractJob._JOB_TYPE: ExtractJob,
-            QueryJob._JOB_TYPE: QueryJob,
-        }
-
-        job = None
-        for job_type, job_object in supported_jobs.items():
-            if job_type in configuration:
-                job = job_object
-                break
-
-        if not job:
-            raise AirflowException(f"Unknown job type. Supported types: {supported_jobs.keys()}")
-        job = job.from_api_repr(job_data, client)
-        self.log.info("Inserting job %s", job.job_id)
-        if nowait:
-            # Initiate the job and don't wait for it to complete.
-            job._begin()
-        else:
-            # Start the job and wait for it to complete and get the result.
-            job.result()
-        return job
-
-
 class BigQueryHookAsync(GoogleBaseHookAsync):
-    """Big query async hook inherits from GoogleBaseHookAsync class and connects to the google Big query"""
+    """Big query async hook inherits from GoogleBaseHookAsync class and connects to the Google Big Query"""
 
-    sync_hook_class = _BigQueryHook
+    sync_hook_class = BigQueryHook
 
     async def get_job_instance(
         self, project_id: Optional[str], job_id: Optional[str], session: ClientSession
     ) -> Job:
         """Get the specified job resource by job ID and project ID."""
         with await self.service_file_as_context() as f:
             return Job(job_id=job_id, project=project_id, service_file=f, session=cast(Session, session))
```

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/hooks/dataproc.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/hooks/dataproc.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/hooks/gcs.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/hooks/gcs.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/operators/bigquery.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/operators/bigquery.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """This module contains Google BigQueryAsync providers."""
 from typing import Any, Dict
 
 from airflow.exceptions import AirflowException
 from airflow.models.baseoperator import BaseOperator
-from airflow.providers.google.cloud.hooks.bigquery import BigQueryJob
+from airflow.providers.google.cloud.hooks.bigquery import BigQueryHook, BigQueryJob
 from airflow.providers.google.cloud.operators.bigquery import (
     BigQueryCheckOperator,
     BigQueryGetDataOperator,
     BigQueryInsertJobOperator,
     BigQueryIntervalCheckOperator,
     BigQueryValueCheckOperator,
 )
 from airflow.utils.context import Context
 from google.api_core.exceptions import Conflict
 
-from astronomer.providers.google.cloud.hooks.bigquery import _BigQueryHook
 from astronomer.providers.google.cloud.triggers.bigquery import (
     BigQueryCheckTrigger,
     BigQueryGetDataTrigger,
     BigQueryInsertJobTrigger,
     BigQueryIntervalCheckTrigger,
     BigQueryValueCheckTrigger,
 )
@@ -68,26 +67,16 @@
         the Service Account Token Creator IAM role.
         If set as a sequence, the identities from the list must grant
         Service Account Token Creator IAM role to the directly preceding identity, with first
         account from the list granting this role to the originating account (templated).
     :param cancel_on_kill: Flag which indicates whether cancel the hook's job or not, when on_kill is called
     """
 
-    def _submit_job(self, hook: _BigQueryHook, job_id: str) -> BigQueryJob:  # type: ignore[override]
-        """Submit a new job and get the job id for polling the status using Triggerer."""
-        return hook.insert_job(
-            configuration=self.configuration,
-            project_id=self.project_id,
-            location=self.location,
-            job_id=job_id,
-            nowait=True,
-        )
-
     def execute(self, context: Context) -> None:  # noqa: D102
-        hook = _BigQueryHook(gcp_conn_id=self.gcp_conn_id)
+        hook = BigQueryHook(gcp_conn_id=self.gcp_conn_id)
 
         self.hook = hook
         job_id = self.hook.generate_job_id(
             job_id=self.job_id,
             dag_id=self.dag_id,
             task_id=self.task_id,
             logical_date=context["logical_date"],
@@ -148,30 +137,30 @@
     """
     BigQueryCheckOperatorAsync is asynchronous operator, submit the job and check
     for the status in async mode by using the job id
     """
 
     def _submit_job(
         self,
-        hook: _BigQueryHook,
+        hook: BigQueryHook,
         job_id: str,
     ) -> BigQueryJob:
         """Submit a new job and get the job id for polling the status using Trigger."""
         configuration = {"query": {"query": self.sql}}
 
         return hook.insert_job(
             configuration=configuration,
             project_id=hook.project_id,
             location=self.location,
             job_id=job_id,
             nowait=True,
         )
 
     def execute(self, context: Context) -> None:  # noqa: D102
-        hook = _BigQueryHook(
+        hook = BigQueryHook(
             gcp_conn_id=self.gcp_conn_id,
         )
         job = self._submit_job(hook, job_id="")
         context["ti"].xcom_push(key="job_id", value=job.job_id)
         self.defer(
             timeout=self.execution_timeout,
             trigger=BigQueryCheckTrigger(
@@ -246,15 +235,15 @@
         If set as a sequence, the identities from the list must grant
         Service Account Token Creator IAM role to the directly preceding identity, with first
         account from the list granting this role to the originating account (templated).
     """
 
     def _submit_job(
         self,
-        hook: _BigQueryHook,
+        hook: BigQueryHook,
         job_id: str,
         configuration: Dict[str, Any],
     ) -> BigQueryJob:
         """Submit a new job and get the job id for polling the status using Triggerer."""
         return hook.insert_job(
             configuration=configuration,
             location=self.location,
@@ -276,15 +265,15 @@
         query += " from " + self.dataset_id + "." + self.table_id + " limit " + str(self.max_results)
         return query
 
     def execute(self, context: Context) -> None:  # type: ignore[override]  # noqa: D102
         get_query = self.generate_query()
         configuration = {"query": {"query": get_query}}
 
-        hook = _BigQueryHook(
+        hook = BigQueryHook(
             gcp_conn_id=self.gcp_conn_id,
             delegate_to=self.delegate_to,
             location=self.location,
             impersonation_chain=self.impersonation_chain,
         )
 
         self.hook = hook
@@ -345,15 +334,15 @@
         Service Account Token Creator IAM role to the directly preceding identity, with first
         account from the list granting this role to the originating account (templated).
     :param labels: a dictionary containing labels for the table, passed to BigQuery
     """
 
     def _submit_job(
         self,
-        hook: _BigQueryHook,
+        hook: BigQueryHook,
         sql: str,
         job_id: str,
     ) -> BigQueryJob:
         """Submit a new job and get the job id for polling the status using Triggerer."""
         configuration = {"query": {"query": sql}}
         return hook.insert_job(
             configuration=configuration,
@@ -361,15 +350,15 @@
             location=self.location,
             job_id=job_id,
             nowait=True,
         )
 
     def execute(self, context: Context) -> None:
         """Execute the job in sync mode and defers the trigger with job id to poll for the status"""
-        hook = _BigQueryHook(gcp_conn_id=self.gcp_conn_id)
+        hook = BigQueryHook(gcp_conn_id=self.gcp_conn_id)
         self.log.info("Using ratio formula: %s", self.ratio_formula)
 
         self.log.info("Executing SQL check: %s", self.sql1)
         job_1 = self._submit_job(hook, sql=self.sql1, job_id="")
         context["ti"].xcom_push(key="job_id", value=job_1.job_id)
 
         self.log.info("Executing SQL check: %s", self.sql2)
@@ -406,15 +395,15 @@
             event["status"],
         )
 
 
 class BigQueryValueCheckOperatorAsync(BigQueryValueCheckOperator):  # noqa: D101
     def _submit_job(
         self,
-        hook: _BigQueryHook,
+        hook: BigQueryHook,
         job_id: str,
     ) -> BigQueryJob:
         """Submit a new job and get the job id for polling the status using Triggerer."""
         configuration = {
             "query": {
                 "query": self.sql,
                 "useLegacySql": False,
@@ -428,15 +417,15 @@
             project_id=hook.project_id,
             location=self.location,
             job_id=job_id,
             nowait=True,
         )
 
     def execute(self, context: Context) -> None:  # noqa: D102
-        hook = _BigQueryHook(gcp_conn_id=self.gcp_conn_id)
+        hook = BigQueryHook(gcp_conn_id=self.gcp_conn_id)
 
         job = self._submit_job(hook, job_id="")
         context["ti"].xcom_push(key="job_id", value=job.job_id)
         self.defer(
             timeout=self.execution_timeout,
             trigger=BigQueryValueCheckTrigger(
                 conn_id=self.gcp_conn_id,
```

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/operators/dataproc.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/operators/dataproc.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/operators/kubernetes_engine.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/operators/kubernetes_engine.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/sensors/bigquery.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/sensors/bigquery.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/sensors/gcs.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/sensors/gcs.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/triggers/bigquery.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/triggers/bigquery.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/triggers/dataproc.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/triggers/dataproc.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/triggers/gcs.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/triggers/gcs.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/cloud/triggers/kubernetes_engine.py` & `astronomer-providers-1.9.0/astronomer/providers/google/cloud/triggers/kubernetes_engine.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/google/common/hooks/base_google.py` & `astronomer-providers-1.9.0/astronomer/providers/google/common/hooks/base_google.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/http/example_dags/example_http.py` & `astronomer-providers-1.9.0/astronomer/providers/http/example_dags/example_http.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/http/hooks/http.py` & `astronomer-providers-1.9.0/astronomer/providers/http/hooks/http.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/http/sensors/http.py` & `astronomer-providers-1.9.0/astronomer/providers/http/sensors/http.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/http/triggers/http.py` & `astronomer-providers-1.9.0/astronomer/providers/http/triggers/http.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/example_dags/example_adf_run_pipeline.py` & `astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/example_dags/example_adf_run_pipeline.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/example_dags/example_wasb_sensors.py` & `astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/example_dags/example_wasb_sensors.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/hooks/data_factory.py` & `astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/hooks/data_factory.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/hooks/wasb.py` & `astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/hooks/wasb.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/operators/data_factory.py` & `astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/operators/data_factory.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/sensors/data_factory.py` & `astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/sensors/data_factory.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/sensors/wasb.py` & `astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/sensors/wasb.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/triggers/data_factory.py` & `astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/triggers/data_factory.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/microsoft/azure/triggers/wasb.py` & `astronomer-providers-1.9.0/astronomer/providers/microsoft/azure/triggers/wasb.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/snowflake/example_dags/example_snowflake.py` & `astronomer-providers-1.9.0/astronomer/providers/snowflake/example_dags/example_snowflake.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/snowflake/example_dags/example_snowflake_sql_api.py` & `astronomer-providers-1.9.0/astronomer/providers/snowflake/example_dags/example_snowflake_sql_api.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/snowflake/extractors/snowflake.py` & `astronomer-providers-1.9.0/astronomer/providers/snowflake/extractors/snowflake.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/snowflake/hooks/snowflake.py` & `astronomer-providers-1.9.0/astronomer/providers/snowflake/hooks/snowflake.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/snowflake/hooks/snowflake_sql_api.py` & `astronomer-providers-1.9.0/astronomer/providers/snowflake/hooks/snowflake_sql_api.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/snowflake/hooks/sql_api_generate_jwt.py` & `astronomer-providers-1.9.0/astronomer/providers/snowflake/hooks/sql_api_generate_jwt.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/snowflake/operators/snowflake.py` & `astronomer-providers-1.9.0/astronomer/providers/snowflake/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer/providers/snowflake/triggers/snowflake_trigger.py` & `astronomer-providers-1.9.0/astronomer/providers/snowflake/triggers/snowflake_trigger.py`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/astronomer_providers.egg-info/PKG-INFO` & `astronomer-providers-1.9.0/astronomer_providers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-providers
-Version: 1.8.1
+Version: 1.9.0
 Summary: Apache Airflow Providers containing Deferrable Operators & Sensors from Astronomer
 Home-page: https://github.com/astronomer/astronomer-providers/
 Author: Astronomer
 Author-email: humans@astronomer.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/astronomer/astronomer-providers/
 Project-URL: Homepage, https://astronomer.io/
@@ -25,14 +25,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Provides-Extra: amazon
 Provides-Extra: apache.hive
 Provides-Extra: apache.livy
 Provides-Extra: cncf.kubernetes
 Provides-Extra: databricks
+Provides-Extra: dbt.cloud
 Provides-Extra: google
 Provides-Extra: http
 Provides-Extra: microsoft.azure
 Provides-Extra: snowflake
 Provides-Extra: openlineage
 Provides-Extra: docs
 Provides-Extra: tests
@@ -120,14 +121,18 @@
      - ``pip install 'astronomer-providers[cncf.kubernetes]'``
      - Cncf Kubernetes
 
    * - ``databricks``
      - ``pip install 'astronomer-providers[databricks]'``
      - Databricks
 
+   * - ``dbt.cloud``
+     - ``pip install 'astronomer-providers[dbt.cloud]'``
+     - Dbt Cloud
+
    * - ``google``
      - ``pip install 'astronomer-providers[google]'``
      - Google
 
    * - ``http``
      - ``pip install 'astronomer-providers[http]'``
      - Http
```

### Comparing `astronomer-providers-1.8.1/astronomer_providers.egg-info/SOURCES.txt` & `astronomer-providers-1.9.0/astronomer_providers.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 README.rst
 pyproject.toml
 setup.cfg
+astronomer/providers/package.py
 astronomer/providers/amazon/__init__.py
 astronomer/providers/amazon/aws/__init__.py
 astronomer/providers/amazon/aws/example_dags/__init__.py
 astronomer/providers/amazon/aws/example_dags/example_aws_nuke.py
 astronomer/providers/amazon/aws/example_dags/example_batch.py
 astronomer/providers/amazon/aws/example_dags/example_emr_eks_containers_job.py
 astronomer/providers/amazon/aws/example_dags/example_emr_sensor.py
 astronomer/providers/amazon/aws/example_dags/example_redshift_cluster_management.py
 astronomer/providers/amazon/aws/example_dags/example_redshift_data.py
 astronomer/providers/amazon/aws/example_dags/example_redshift_sql.py
 astronomer/providers/amazon/aws/example_dags/example_s3.py
+astronomer/providers/amazon/aws/extractors/__init__.py
+astronomer/providers/amazon/aws/extractors/redshift.py
 astronomer/providers/amazon/aws/hooks/__init__.py
 astronomer/providers/amazon/aws/hooks/base_aws.py
 astronomer/providers/amazon/aws/hooks/base_aws_async.py
 astronomer/providers/amazon/aws/hooks/batch_client.py
 astronomer/providers/amazon/aws/hooks/emr.py
 astronomer/providers/amazon/aws/hooks/redshift_cluster.py
 astronomer/providers/amazon/aws/hooks/redshift_data.py
@@ -87,14 +90,26 @@
 astronomer/providers/databricks/example_dags/example_databricks.py
 astronomer/providers/databricks/hooks/__init__.py
 astronomer/providers/databricks/hooks/databricks.py
 astronomer/providers/databricks/operators/__init__.py
 astronomer/providers/databricks/operators/databricks.py
 astronomer/providers/databricks/triggers/__init__.py
 astronomer/providers/databricks/triggers/databricks.py
+astronomer/providers/dbt/__init__.py
+astronomer/providers/dbt/cloud/__init__.py
+astronomer/providers/dbt/cloud/example_dags/__init__.py
+astronomer/providers/dbt/cloud/example_dags/example_dbt_cloud.py
+astronomer/providers/dbt/cloud/hooks/__init__.py
+astronomer/providers/dbt/cloud/hooks/dbt.py
+astronomer/providers/dbt/cloud/operators/__init__.py
+astronomer/providers/dbt/cloud/operators/dbt.py
+astronomer/providers/dbt/cloud/sensors/__init__.py
+astronomer/providers/dbt/cloud/sensors/dbt.py
+astronomer/providers/dbt/cloud/triggers/__init__.py
+astronomer/providers/dbt/cloud/triggers/dbt.py
 astronomer/providers/google/__init__.py
 astronomer/providers/google/cloud/__init__.py
 astronomer/providers/google/cloud/example_dags/__init__.py
 astronomer/providers/google/cloud/example_dags/example_bigquery_queries.py
 astronomer/providers/google/cloud/example_dags/example_bigquery_sensors.py
 astronomer/providers/google/cloud/example_dags/example_dataproc.py
 astronomer/providers/google/cloud/example_dags/example_gcp_nuke.py
@@ -159,11 +174,12 @@
 astronomer/providers/snowflake/operators/__init__.py
 astronomer/providers/snowflake/operators/snowflake.py
 astronomer/providers/snowflake/triggers/__init__.py
 astronomer/providers/snowflake/triggers/snowflake_trigger.py
 astronomer_providers.egg-info/PKG-INFO
 astronomer_providers.egg-info/SOURCES.txt
 astronomer_providers.egg-info/dependency_links.txt
+astronomer_providers.egg-info/entry_points.txt
 astronomer_providers.egg-info/namespace_packages.txt
 astronomer_providers.egg-info/not-zip-safe
 astronomer_providers.egg-info/requires.txt
 astronomer_providers.egg-info/top_level.txt
```

### Comparing `astronomer-providers-1.8.1/astronomer_providers.egg-info/requires.txt` & `astronomer-providers-1.9.0/astronomer_providers.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 apache-airflow-providers-apache-livy
 apache-airflow-providers-cncf-kubernetes>=4
 apache-airflow-providers-databricks>=2.2.0
 apache-airflow-providers-google>=8.1.0
 apache-airflow-providers-http
 apache-airflow-providers-snowflake
 apache-airflow-providers-microsoft-azure
+apache-airflow-providers-dbt-cloud>=2.1.0
 gcloud-aio-bigquery
 gcloud-aio-storage
 kubernetes_asyncio
 impyla
-openlineage-airflow>=0.9.0
+openlineage-airflow>=0.12.0
 paramiko
 protobuf<=3.20.0
 
 [all:python_version >= "3.10"]
 databricks-sql-connector>=2.0.4
 
 [amazon]
@@ -47,14 +48,17 @@
 
 [databricks]
 apache-airflow-providers-databricks>=2.2.0
 
 [databricks:python_version >= "3.10"]
 databricks-sql-connector>=2.0.4
 
+[dbt.cloud]
+apache-airflow-providers-dbt-cloud>=2.1.0
+
 [docs]
 sphinx
 sphinx-autoapi
 sphinx-copybutton
 
 [google]
 apache-airflow-providers-google>=8.1.0
@@ -89,15 +93,15 @@
 types-tabulate
 types-toml
 types-Markdown
 types-PyMySQL
 types-PyYAML
 
 [openlineage]
-openlineage-airflow>=0.9.0
+openlineage-airflow>=0.12.0
 
 [snowflake]
 apache-airflow-providers-snowflake
 
 [tests]
 aioresponses
 asynctest
```

### Comparing `astronomer-providers-1.8.1/pyproject.toml` & `astronomer-providers-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astronomer-providers-1.8.1/setup.cfg` & `astronomer-providers-1.9.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = astronomer-providers
-version = 1.8.1
+version = 1.9.0
 url = https://github.com/astronomer/astronomer-providers/
 author = Astronomer
 author_email = humans@astronomer.io
 description = Apache Airflow Providers containing Deferrable Operators & Sensors from Astronomer
 long_description = file: README.rst
 license = Apache License 2.0
 license_files = LICENSE.txt
@@ -54,27 +54,29 @@
 	paramiko
 cncf.kubernetes = 
 	apache-airflow-providers-cncf-kubernetes>=4
 	kubernetes_asyncio
 databricks = 
 	apache-airflow-providers-databricks>=2.2.0
 	databricks-sql-connector>=2.0.4;python_version>='3.10'
+dbt.cloud = 
+	apache-airflow-providers-dbt-cloud>=2.1.0
 google = 
 	apache-airflow-providers-google>=8.1.0
 	gcloud-aio-storage
 	gcloud-aio-bigquery
 	protobuf<=3.20.0  # Bigquery provider isn't compatible with it. Details in https://github.com/apache/airflow/commit/25a9ae3b2eec85dfd500b0a921045fc95ab8ffd6
 http = 
 	apache-airflow-providers-http
 microsoft.azure = 
 	apache-airflow-providers-microsoft-azure
 snowflake = 
 	apache-airflow-providers-snowflake
 openlineage = 
-	openlineage-airflow>=0.9.0
+	openlineage-airflow>=0.12.0
 docs = 
 	sphinx
 	sphinx-autoapi
 	sphinx-copybutton
 tests = 
 	aioresponses
 	asynctest
@@ -114,26 +116,31 @@
 	apache-airflow-providers-cncf-kubernetes>=4
 	apache-airflow-providers-databricks>=2.2.0
 	apache-airflow-providers-google>=8.1.0
 	apache-airflow-providers-http
 	apache-airflow-providers-snowflake
 	apache-airflow-providers-microsoft-azure
 	databricks-sql-connector>=2.0.4;python_version>='3.10'
+	apache-airflow-providers-dbt-cloud>=2.1.0
 	gcloud-aio-bigquery
 	gcloud-aio-storage
 	kubernetes_asyncio
 	impyla
-	openlineage-airflow>=0.9.0
+	openlineage-airflow>=0.12.0
 	paramiko
 	protobuf<=3.20.0  # Bigquery provider isn't compatible with it. Details in https://github.com/apache/airflow/commit/25a9ae3b2eec85dfd500b0a921045fc95ab8ffd6
 
 [options.packages.find]
 include = 
 	astronomer.*
 
+[options.entry_points]
+apache_airflow_provider = 
+	provider_info=astronomer.providers.package:get_provider_info
+
 [flake8]
 enable-extensions = G
 exclude = venv/*,tox/*,specs/*
 ignore = E123,E128,E266,RST303,E402,W503,E731,W601
 max-line-length = 119
 rst-roles = 
 	class,
```

