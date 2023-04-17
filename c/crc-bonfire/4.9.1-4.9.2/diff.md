# Comparing `tmp/crc-bonfire-4.9.1.tar.gz` & `tmp/crc-bonfire-4.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crc-bonfire-4.9.1.tar", last modified: Fri Oct 14 16:56:19 2022, max compression
+gzip compressed data, was "crc-bonfire-4.9.2.tar", last modified: Wed Oct 19 20:17:40 2022, max compression
```

## Comparing `crc-bonfire-4.9.1.tar` & `crc-bonfire-4.9.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 16:56:19.471640 crc-bonfire-4.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 16:56:19.459640 crc-bonfire-4.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 16:56:19.467640 crc-bonfire-4.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2051 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    16932 2022-10-14 16:56:19.471640 crc-bonfire-4.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16219 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 16:56:19.467640 crc-bonfire-4.9.1/bonfire/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/bonfire/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    38174 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/bonfire/bonfire.py
--rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/bonfire/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1840 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/bonfire/local.py
--rw-r--r--   0 runner    (1001) docker     (121)    12696 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/bonfire/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (121)    10843 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/bonfire/openshift.py
--rw-r--r--   0 runner    (1001) docker     (121)    24318 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/bonfire/processor.py
--rw-r--r--   0 runner    (1001) docker     (121)    11518 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/bonfire/qontract.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 16:56:19.467640 crc-bonfire-4.9.1/bonfire/resources/
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/bonfire/resources/default-iqe-cji.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/bonfire/resources/default_config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2028 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/bonfire/resources/local-cluster-clowdenvironment.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/bonfire/resources/reservation-template.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/bonfire/secrets.py
--rw-r--r--   0 runner    (1001) docker     (121)    17776 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/bonfire/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 16:56:19.467640 crc-bonfire-4.9.1/cicd/
--rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/_common_container_logic.sh
--rw-r--r--   0 runner    (1001) docker     (121)     4930 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/_common_deploy_logic.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 16:56:19.467640 crc-bonfire-4.9.1/cicd/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1044 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/bin/check_junit_files
--rwxr-xr-x   0 runner    (1001) docker     (121)      337 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/bin/oc_wrapper
--rw-r--r--   0 runner    (1001) docker     (121)     2474 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/build.sh
--rw-r--r--   0 runner    (1001) docker     (121)     4985 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/cji_smoke_test.sh
--rw-r--r--   0 runner    (1001) docker     (121)     2389 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/deploy_ephemeral_db.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/deploy_ephemeral_env.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 16:56:19.471640 crc-bonfire-4.9.1/cicd/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     3223 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/examples/pr_check_template.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/examples/unit_test_example.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/examples/unit_test_example_ephemeral_db.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 16:56:19.471640 crc-bonfire-4.9.1/cicd/iqe_pod/
--rw-r--r--   0 runner    (1001) docker     (121)     7874 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/iqe_pod/create_iqe_pod.py
--rw-r--r--   0 runner    (1001) docker     (121)     4775 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/iqe_pod/env_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/iqe_pod/iqe_runner.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/post_test_results.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/cicd/smoke_test.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 16:56:19.471640 crc-bonfire-4.9.1/crc_bonfire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16932 2022-10-14 16:56:18.000000 crc-bonfire-4.9.1/crc_bonfire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-10-14 16:56:19.000000 crc-bonfire-4.9.1/crc_bonfire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-14 16:56:18.000000 crc-bonfire-4.9.1/crc_bonfire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-10-14 16:56:19.000000 crc-bonfire-4.9.1/crc_bonfire.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-10-14 16:56:19.000000 crc-bonfire-4.9.1/crc_bonfire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-14 16:56:19.000000 crc-bonfire-4.9.1/crc_bonfire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)  2975380 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/demo.gif
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-10-14 16:56:19.471640 crc-bonfire-4.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 16:56:19.471640 crc-bonfire-4.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 16:56:19.471640 crc-bonfire-4.9.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)     2382 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/tests/data/namespace_data.json
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/tests/data/reservation_data.json
--rw-r--r--   0 runner    (1001) docker     (121)    13102 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/tests/test_bonfire.py
--rw-r--r--   0 runner    (1001) docker     (121)    10894 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-14 16:56:19.471640 crc-bonfire-4.9.1/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-10-14 16:56:00.000000 crc-bonfire-4.9.1/utils/search_replace.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:17:40.387358 crc-bonfire-4.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:17:40.379357 crc-bonfire-4.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:17:40.383357 crc-bonfire-4.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      848 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2051 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1503 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)    16932 2022-10-19 20:17:40.387358 crc-bonfire-4.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    16219 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:17:40.383357 crc-bonfire-4.9.2/bonfire/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/bonfire/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    38174 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/bonfire/bonfire.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/bonfire/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1840 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/bonfire/local.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12696 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/bonfire/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10843 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/bonfire/openshift.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24318 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/bonfire/processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11518 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/bonfire/qontract.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:17:40.383357 crc-bonfire-4.9.2/bonfire/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/bonfire/resources/default-iqe-cji.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/bonfire/resources/default_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2614 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2028 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/bonfire/resources/local-cluster-clowdenvironment.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/bonfire/resources/reservation-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/bonfire/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18067 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/bonfire/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:17:40.387358 crc-bonfire-4.9.2/cicd/
+-rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/_common_container_logic.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     4930 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/_common_deploy_logic.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:17:40.387358 crc-bonfire-4.9.2/cicd/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1044 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/bin/check_junit_files
+-rwxr-xr-x   0 runner    (1001) docker     (121)      337 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/bin/oc_wrapper
+-rw-r--r--   0 runner    (1001) docker     (121)     2474 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/build.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     4985 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/cji_smoke_test.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     2389 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/deploy_ephemeral_db.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/deploy_ephemeral_env.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:17:40.387358 crc-bonfire-4.9.2/cicd/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     3223 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/examples/pr_check_template.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/examples/unit_test_example.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/examples/unit_test_example_ephemeral_db.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:17:40.387358 crc-bonfire-4.9.2/cicd/iqe_pod/
+-rw-r--r--   0 runner    (1001) docker     (121)     7874 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/iqe_pod/create_iqe_pod.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4775 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/iqe_pod/env_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/iqe_pod/iqe_runner.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/post_test_results.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     1556 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/cicd/smoke_test.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:17:40.387358 crc-bonfire-4.9.2/crc_bonfire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    16932 2022-10-19 20:17:39.000000 crc-bonfire-4.9.2/crc_bonfire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1476 2022-10-19 20:17:40.000000 crc-bonfire-4.9.2/crc_bonfire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 20:17:39.000000 crc-bonfire-4.9.2/crc_bonfire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-10-19 20:17:40.000000 crc-bonfire-4.9.2/crc_bonfire.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-10-19 20:17:40.000000 crc-bonfire-4.9.2/crc_bonfire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-19 20:17:40.000000 crc-bonfire-4.9.2/crc_bonfire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)  2975380 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/demo.gif
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-10-19 20:17:40.387358 crc-bonfire-4.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:17:40.387358 crc-bonfire-4.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:17:40.387358 crc-bonfire-4.9.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)     2382 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/tests/data/namespace_data.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/tests/data/reservation_data.json
+-rw-r--r--   0 runner    (1001) docker     (121)    13102 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/tests/test_bonfire.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10894 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 20:17:40.387358 crc-bonfire-4.9.2/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     1954 2022-10-19 20:17:21.000000 crc-bonfire-4.9.2/utils/search_replace.py
```

### Comparing `crc-bonfire-4.9.1/.github/workflows/release.yml` & `crc-bonfire-4.9.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/.github/workflows/tests.yml` & `crc-bonfire-4.9.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/.gitignore` & `crc-bonfire-4.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/CONTRIBUTING.md` & `crc-bonfire-4.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/PKG-INFO` & `crc-bonfire-4.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crc-bonfire
-Version: 4.9.1
+Version: 4.9.2
 Summary: A CLI tool used to deploy ephemeral environments for testing cloud.redhat.com applications
 Home-page: https://www.github.com/RedHatInsights/bonfire
 Author: Brandon Squizzato
 Author-email: bsquizza@redhat.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
```

### Comparing `crc-bonfire-4.9.1/README.md` & `crc-bonfire-4.9.2/README.md`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/bonfire/bonfire.py` & `crc-bonfire-4.9.2/bonfire/bonfire.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/bonfire/config.py` & `crc-bonfire-4.9.2/bonfire/config.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/bonfire/local.py` & `crc-bonfire-4.9.2/bonfire/local.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/bonfire/namespaces.py` & `crc-bonfire-4.9.2/bonfire/namespaces.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/bonfire/openshift.py` & `crc-bonfire-4.9.2/bonfire/openshift.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/bonfire/processor.py` & `crc-bonfire-4.9.2/bonfire/processor.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/bonfire/qontract.py` & `crc-bonfire-4.9.2/bonfire/qontract.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/bonfire/resources/default-iqe-cji.yaml` & `crc-bonfire-4.9.2/bonfire/resources/default-iqe-cji.yaml`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml` & `crc-bonfire-4.9.2/bonfire/resources/ephemeral-cluster-clowdenvironment.yaml`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/bonfire/resources/local-cluster-clowdenvironment.yaml` & `crc-bonfire-4.9.2/bonfire/resources/local-cluster-clowdenvironment.yaml`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/bonfire/secrets.py` & `crc-bonfire-4.9.2/bonfire/secrets.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/bonfire/utils.py` & `crc-bonfire-4.9.2/bonfire/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -384,17 +384,24 @@
             except Exception as err:
                 log.error("failed to fetch template file for %s: %s", component_name, err)
 
             template = yaml.safe_load(template_content)
             items = template.get("objects", [])
 
             dependencies = get_dependencies(items)
-            dependencies = dependencies.union(get_dependencies(items, optional=True))
+            optional_dependencies = get_dependencies(items, optional=True)
 
-            for name, deps in dependencies.items():
+            all_dependencies = {}
+            all_keys = dependencies.keys() | optional_dependencies.keys()
+            for name in all_keys:
+                all_dependencies[name] = dependencies.get(name, set()).union(
+                    optional_dependencies.get(name, set())
+                )
+
+            for name, deps in all_dependencies.items():
                 # check if the name of the ClowdApp is set with a parameter
                 parameter_name = _PARAM_REGEX.findall(name)
                 if parameter_name:
                     # replace 'name' with parameter's default value if found
                     for p in template.get("parameters", {}):
                         if p["name"] == parameter_name[0]:
                             name = p.get("value", name)
```

### Comparing `crc-bonfire-4.9.1/cicd/README.md` & `crc-bonfire-4.9.2/cicd/README.md`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/cicd/_common_container_logic.sh` & `crc-bonfire-4.9.2/cicd/_common_container_logic.sh`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/cicd/_common_deploy_logic.sh` & `crc-bonfire-4.9.2/cicd/_common_deploy_logic.sh`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/cicd/bin/check_junit_files` & `crc-bonfire-4.9.2/cicd/bin/check_junit_files`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/cicd/bootstrap.sh` & `crc-bonfire-4.9.2/cicd/bootstrap.sh`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/cicd/build.sh` & `crc-bonfire-4.9.2/cicd/build.sh`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/cicd/cji_smoke_test.sh` & `crc-bonfire-4.9.2/cicd/cji_smoke_test.sh`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/cicd/deploy_ephemeral_db.sh` & `crc-bonfire-4.9.2/cicd/deploy_ephemeral_db.sh`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/cicd/deploy_ephemeral_env.sh` & `crc-bonfire-4.9.2/cicd/deploy_ephemeral_env.sh`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/cicd/examples/pr_check_template.sh` & `crc-bonfire-4.9.2/cicd/examples/pr_check_template.sh`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/cicd/examples/unit_test_example.sh` & `crc-bonfire-4.9.2/cicd/examples/unit_test_example.sh`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/cicd/examples/unit_test_example_ephemeral_db.sh` & `crc-bonfire-4.9.2/cicd/examples/unit_test_example_ephemeral_db.sh`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/cicd/iqe_pod/create_iqe_pod.py` & `crc-bonfire-4.9.2/cicd/iqe_pod/create_iqe_pod.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/cicd/iqe_pod/env_parser.py` & `crc-bonfire-4.9.2/cicd/iqe_pod/env_parser.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/cicd/iqe_pod/iqe_runner.sh` & `crc-bonfire-4.9.2/cicd/iqe_pod/iqe_runner.sh`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/cicd/post_test_results.sh` & `crc-bonfire-4.9.2/cicd/post_test_results.sh`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/cicd/smoke_test.sh` & `crc-bonfire-4.9.2/cicd/smoke_test.sh`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/crc_bonfire.egg-info/PKG-INFO` & `crc-bonfire-4.9.2/crc_bonfire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crc-bonfire
-Version: 4.9.1
+Version: 4.9.2
 Summary: A CLI tool used to deploy ephemeral environments for testing cloud.redhat.com applications
 Home-page: https://www.github.com/RedHatInsights/bonfire
 Author: Brandon Squizzato
 Author-email: bsquizza@redhat.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
```

### Comparing `crc-bonfire-4.9.1/crc_bonfire.egg-info/SOURCES.txt` & `crc-bonfire-4.9.2/crc_bonfire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/demo.gif` & `crc-bonfire-4.9.2/demo.gif`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/requirements.txt` & `crc-bonfire-4.9.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/setup.cfg` & `crc-bonfire-4.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/tests/data/namespace_data.json` & `crc-bonfire-4.9.2/tests/data/namespace_data.json`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/tests/data/reservation_data.json` & `crc-bonfire-4.9.2/tests/data/reservation_data.json`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/tests/test_bonfire.py` & `crc-bonfire-4.9.2/tests/test_bonfire.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/tests/test_processor.py` & `crc-bonfire-4.9.2/tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/tests/test_utils.py` & `crc-bonfire-4.9.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `crc-bonfire-4.9.1/utils/search_replace.py` & `crc-bonfire-4.9.2/utils/search_replace.py`

 * *Files identical despite different names*

