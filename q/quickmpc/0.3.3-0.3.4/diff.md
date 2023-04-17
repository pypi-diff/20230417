# Comparing `tmp/quickmpc-0.3.3.tar.gz` & `tmp/quickmpc-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-46fhb54f/quickmpc-0.3.3.tar", last modified: Wed Apr 12 08:18:21 2023, max compression
+gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-yd53resg/quickmpc-0.3.4.tar", last modified: Mon Apr 17 01:18:10 2023, max compression
```

## Comparing `quickmpc-0.3.3.tar` & `quickmpc-0.3.4.tar`

### file list

```diff
@@ -1,105 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-12 08:17:59.000000 quickmpc-0.3.3/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-12 08:17:59.000000 quickmpc-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-12 08:17:59.000000 quickmpc-0.3.3/.isort.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-12 08:17:59.000000 quickmpc-0.3.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 08:17:59.000000 quickmpc-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-12 08:17:59.000000 quickmpc-0.3.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 08:18:21.000000 quickmpc-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-12 08:17:59.000000 quickmpc-0.3.3/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    38604 2023-04-12 08:17:59.000000 quickmpc-0.3.3/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-12 08:17:59.000000 quickmpc-0.3.3/README-ja.md
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-12 08:17:59.000000 quickmpc-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/demo/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/README-ja.md
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/demo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/data/data-meshcode.csv
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/data/data1-1.csv
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/data/data1-2.csv
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/data/data1-3.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/demo/integration_demo/
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/integration_demo/execute_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/integration_demo/progress_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/integration_demo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/demo/unit_demo/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/unit_demo/delete_share.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/unit_demo/demo_sharize.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/unit_demo/execute_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/unit_demo/get_computation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/unit_demo/get_data_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/unit_demo/get_elapsed_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/unit_demo/get_join_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-12 08:17:59.000000 quickmpc-0.3.3/demo/unit_demo/send_share.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-12 08:17:59.000000 quickmpc-0.3.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-12 08:17:59.000000 quickmpc-0.3.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc/
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc/proto/common_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/common_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/common_types/common_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/common_types/common_types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/libc_to_manage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/libc_to_manage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/libc_to_manage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/qmpc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/share.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/utils/if_present.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/utils/make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/utils/overload_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/utils/parse_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/utils/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-12 08:17:59.000000 quickmpc-0.3.3/quickmpc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 08:18:21.000000 quickmpc-0.3.3/quickmpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-12 08:18:21.000000 quickmpc-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 08:17:59.000000 quickmpc-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/tests/unit_tests/certificates/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/certificates/server1.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/certificates/server1.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/certificates/server2.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/certificates/server2.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/certificates/server3.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/certificates/server3.pem
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/local_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:18:21.000000 quickmpc-0.3.3/tests/unit_tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/bitvector.csv
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/diff_col.csv
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/edge_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/empty.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/none.csv
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/normal.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/not_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/over_number.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_files/string_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_over_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_share_recons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tests/unit_tests/test_share_sharize.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-12 08:17:59.000000 quickmpc-0.3.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-17 01:17:45.000000 quickmpc-0.3.4/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-17 01:17:45.000000 quickmpc-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-17 01:17:45.000000 quickmpc-0.3.4/.isort.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-17 01:17:45.000000 quickmpc-0.3.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 01:17:45.000000 quickmpc-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-17 01:17:45.000000 quickmpc-0.3.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-17 01:18:10.000000 quickmpc-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-17 01:17:45.000000 quickmpc-0.3.4/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    38604 2023-04-17 01:17:45.000000 quickmpc-0.3.4/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-17 01:17:45.000000 quickmpc-0.3.4/README-ja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-17 01:17:45.000000 quickmpc-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-17 01:17:45.000000 quickmpc-0.3.4/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-17 01:17:45.000000 quickmpc-0.3.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc/proto/common_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/common_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/common_types/common_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/common_types/common_types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/libc_to_manage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/libc_to_manage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/libc_to_manage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/qmpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18252 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/qmpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/share.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/utils/if_present.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/utils/make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/utils/overload_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/utils/parse_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/utils/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-17 01:17:45.000000 quickmpc-0.3.4/quickmpc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 01:18:10.000000 quickmpc-0.3.4/quickmpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-17 01:18:10.000000 quickmpc-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 01:17:45.000000 quickmpc-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/tests/unit_tests/certificates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/certificates/server1.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/certificates/server1.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/certificates/server2.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/certificates/server2.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/certificates/server3.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/certificates/server3.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/local_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 01:18:10.000000 quickmpc-0.3.4/tests/unit_tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/bitvector.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/diff_col.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/edge_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/empty.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/none.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/normal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/not_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/over_number.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_files/string_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_over_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_qmpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_share_recons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tests/unit_tests/test_share_sharize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-17 01:17:45.000000 quickmpc-0.3.4/tox.ini
```

### Comparing `quickmpc-0.3.3/.vscode/settings.json` & `quickmpc-0.3.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/LICENSE` & `quickmpc-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/Pipfile.lock` & `quickmpc-0.3.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/README.md` & `quickmpc-0.3.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ### Testing with Python 3.7
 ```console
 $ pipenv run tox -e py37
 ```
 
 ## Demo
-This demonstration is performed by pip installing this repository under the assumption of actual use. The operating procedure is described in [demo/README.md](./demo/README.md).
+This demonstration is performed by pip installing this repository under the assumption of actual use. The operating procedure is described in [../../../demo/client_demo/README.md](../../../demo/client_demo/README.md).
 
 ## Coding Style
 Complies with [pep8](https://peps.python.org/pep-0008/) and checked with [flake8](https://github.com/PyCQA/flake8).
 
 Format all files with the following command.
 ```console
 $ pipenv run make fmt
```

### Comparing `quickmpc-0.3.3/mypy.ini` & `quickmpc-0.3.4/mypy.ini`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [mypy]
 python_version = 3.7
 
 # 検査するファイル，ディレクトリ
 files =
   quickmpc,
   tests,
-  demo
+  ../../../demo/client_demo
 
 # 自動生成されたファイルを検査から除外
 [mypy-quickmpc.proto.*]
 ignore_errors = True
 
 # 型ヒントが導入されていないライブラリのerrorを除外
 [mypy-numpy.*]
```

### Comparing `quickmpc-0.3.3/quickmpc/README.md` & `quickmpc-0.3.4/quickmpc/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -7,53 +7,25 @@
 	- 読み込むファイル名
 
 ### Returns
 - parse_data: `Tuple[List[List[float]], List[str]]`
 	- parse_data[0]: schemaを除くテーブルデータ
 	- parse_data[1]: schema
 
-## QMPC.csv_file_to_bitvector
-csvファイルからテーブルデータを読み込んでbitvectorにパースする．
-### Parameters
-- file: `str`
-	- 読み込むファイル名
-- exclude: `List[int]`
-	- bitvector化する対象から除外する列
-
-### Returns
-- parse_data: `Tuple[List[List[float]], List[str]]`
-	- parse_data[0]: schemaを除くbitvector化したテーブルデータ
-	- parse_data[1]: bitvector化したschema
-	- 例えば"s"というschemaを持つ列を3つのbitvectorに分割すると，`["s0","s1","s2"]`となる
-
 ## QMPC.parse_csv_data
 テーブルデータをパースする．
 ### Parameters
 - data: `List[List[str]]`
 	- パースするテーブルデータ
 
 ### Returns
 - parse_data: `Tuple[List[List[float]], List[str]]`
 	- parse_data[0]: schemaを除くテーブルデータ
 	- parse_data[1]: schema
 
-## QMPC.parse_csv_data_to_bitvector
-テーブルデータをbitvectorにパースする．
-### Parameters
-- data: `List[List[str]]`
-	- パースするテーブルデータ
-- exclude: `List[int]`
-	- bitvector化する対象から除外する列
-
-### Returns
-- parse_data: `Tuple[List[List[float]], List[str]]`
-	- parse_data[0]: schemaを除くbitvector化したテーブルデータ
-	- parse_data[1]: bitvector化したschema
-	- 例えば"s"というschemaを持つ列を3つのbitvectorに分割すると，`["s0","s1","s2"]`となる
-
 ## QMPC.send_share
 エンジンにテーブルデータをShare化して送信する
 ### Parameters
 - secrets: `List[List[str]]`
 	- 送信するテーブルデータ
 - schema: `List[str]`
 	- テーブルデータのschema
```

### Comparing `quickmpc-0.3.3/quickmpc/proto/common_types/common_types_pb2.py` & `quickmpc-0.3.4/quickmpc/proto/common_types/common_types_pb2.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/quickmpc/proto/common_types/common_types_pb2.pyi` & `quickmpc-0.3.4/quickmpc/proto/common_types/common_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/quickmpc/proto/libc_to_manage_pb2.py` & `quickmpc-0.3.4/quickmpc/proto/libc_to_manage_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: libc_to_manage.proto
 """Generated protocol buffer code."""
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from common_types import common_types_pb2 as common__types_dot_common__types__pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14libc_to_manage.proto\x12\x0clibctomanage\x1a\x1f\x63ommon_types/common_types.proto\"\xa8\x01\n\x11SendSharesRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\t\x12\x0e\n\x06shares\x18\x02 \x01(\t\x12\'\n\x06schema\x18\x03 \x03(\x0b\x32\x17.pb_common_types.Schema\x12\x10\n\x08piece_id\x18\x04 \x01(\x05\x12\x0f\n\x07sent_at\x18\x05 \x01(\t\x12\x17\n\x0fmatching_column\x18\x06 \x01(\x05\x12\r\n\x05token\x18\x07 \x01(\t\"4\n\x12SendSharesResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\r\n\x05is_ok\x18\x02 \x01(\x08\"5\n\x13\x44\x65leteSharesRequest\x12\x0f\n\x07\x64\x61taIds\x18\x01 \x03(\t\x12\r\n\x05token\x18\x02 \x01(\t\"6\n\x14\x44\x65leteSharesResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\r\n\x05is_ok\x18\x02 \x01(\x08\"2\n\x10GetSchemaRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\"\\\n\x11GetSchemaResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\r\n\x05is_ok\x18\x02 \x01(\x08\x12\'\n\x06schema\x18\x03 \x03(\x0b\x32\x17.pb_common_types.Schema\"9\n\tJoinOrder\x12\x0f\n\x07\x64\x61taIds\x18\x01 \x03(\t\x12\x0c\n\x04join\x18\x02 \x03(\x05\x12\r\n\x05index\x18\x03 \x03(\x05\"$\n\x05Input\x12\x0b\n\x03src\x18\x01 \x03(\x05\x12\x0e\n\x06target\x18\x02 \x03(\x05\"\xab\x01\n\x19\x45xecuteComputationRequest\x12\x35\n\tmethod_id\x18\x01 \x01(\x0e\x32\".pb_common_types.ComputationMethod\x12\r\n\x05token\x18\x02 \x01(\t\x12&\n\x05table\x18\x03 \x01(\x0b\x32\x17.libctomanage.JoinOrder\x12 \n\x03\x61rg\x18\x04 \x01(\x0b\x32\x13.libctomanage.Input\"N\n\x1a\x45xecuteComputationResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\r\n\x05is_ok\x18\x02 \x01(\x08\x12\x10\n\x08job_uuid\x18\x03 \x01(\t\">\n\x1bGetComputationResultRequest\x12\x10\n\x08job_uuid\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\"\xaf\x02\n\x1cGetComputationResultResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\r\n\x05is_ok\x18\x02 \x01(\x08\x12\x0e\n\x06result\x18\x03 \x03(\t\x12\x15\n\rcolumn_number\x18\x04 \x01(\x05\x12*\n\x06status\x18\x05 \x01(\x0e\x32\x1a.pb_common_types.JobStatus\x12\x10\n\x08piece_id\x18\x06 \x01(\x05\x12\x33\n\x08progress\x18\x07 \x01(\x0b\x32\x1c.pb_common_types.JobProgressH\x01\x88\x01\x01\x12\x11\n\x07is_dim1\x18\x08 \x01(\x08H\x00\x12\x11\n\x07is_dim2\x18\t \x01(\x08H\x00\x12\x13\n\tis_schema\x18\n \x01(\x08H\x00\x42\r\n\x0bresult_typeB\x0b\n\t_progress\"#\n\x12GetDataListRequest\x12\r\n\x05token\x18\x01 \x01(\t\"4\n\x13GetDataListResponse\x12\x0e\n\x06result\x18\x01 \x01(\t\x12\r\n\x05is_ok\x18\x02 \x01(\x08\"8\n\x15GetElapsedTimeRequest\x12\x10\n\x08job_uuid\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\"=\n\x16GetElapsedTimeResponse\x12\r\n\x05is_ok\x18\x01 \x01(\x08\x12\x14\n\x0c\x65lapsed_time\x18\x02 \x01(\x01\"9\n\x16GetJobErrorInfoRequest\x12\x10\n\x08job_uuid\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\"w\n\x17GetJobErrorInfoResponse\x12:\n\x0ejob_error_info\x18\x01 \x01(\x0b\x32\x1d.pb_common_types.JobErrorInfoH\x00\x88\x01\x01\x12\r\n\x05is_ok\x18\x02 \x01(\x08\x42\x11\n\x0f_job_error_info2\xff\x05\n\x0cLibcToManage\x12Q\n\nSendShares\x12\x1f.libctomanage.SendSharesRequest\x1a .libctomanage.SendSharesResponse\"\x00\x12W\n\x0c\x44\x65leteShares\x12!.libctomanage.DeleteSharesRequest\x1a\".libctomanage.DeleteSharesResponse\"\x00\x12N\n\tGetSchema\x12\x1e.libctomanage.GetSchemaRequest\x1a\x1f.libctomanage.GetSchemaResponse\"\x00\x12i\n\x12\x45xecuteComputation\x12\'.libctomanage.ExecuteComputationRequest\x1a(.libctomanage.ExecuteComputationResponse\"\x00\x12q\n\x14GetComputationResult\x12).libctomanage.GetComputationResultRequest\x1a*.libctomanage.GetComputationResultResponse\"\x00\x30\x01\x12T\n\x0bGetDataList\x12 .libctomanage.GetDataListRequest\x1a!.libctomanage.GetDataListResponse\"\x00\x12]\n\x0eGetElapsedTime\x12#.libctomanage.GetElapsedTimeRequest\x1a$.libctomanage.GetElapsedTimeResponse\"\x00\x12`\n\x0fGetJobErrorInfo\x12$.libctomanage.GetJobErrorInfoRequest\x1a%.libctomanage.GetJobErrorInfoResponse\"\x00\x42\x45ZCgithub.com/acompany-develop/QuickMPC/proto/libc_to_manage_containerb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14libc_to_manage.proto\x12\x0clibctomanage\x1a\x1f\x63ommon_types/common_types.proto\x1a\x1bgoogle/protobuf/empty.proto\"\xa8\x01\n\x11SendSharesRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\t\x12\x0e\n\x06shares\x18\x02 \x01(\t\x12\'\n\x06schema\x18\x03 \x03(\x0b\x32\x17.pb_common_types.Schema\x12\x10\n\x08piece_id\x18\x04 \x01(\x05\x12\x0f\n\x07sent_at\x18\x05 \x01(\t\x12\x17\n\x0fmatching_column\x18\x06 \x01(\x05\x12\r\n\x05token\x18\x07 \x01(\t\"5\n\x13\x44\x65leteSharesRequest\x12\x0f\n\x07\x64\x61taIds\x18\x01 \x03(\t\x12\r\n\x05token\x18\x02 \x01(\t\"2\n\x10GetSchemaRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\"<\n\x11GetSchemaResponse\x12\'\n\x06schema\x18\x01 \x03(\x0b\x32\x17.pb_common_types.Schema\"9\n\tJoinOrder\x12\x0f\n\x07\x64\x61taIds\x18\x01 \x03(\t\x12\x0c\n\x04join\x18\x02 \x03(\x05\x12\r\n\x05index\x18\x03 \x03(\x05\"$\n\x05Input\x12\x0b\n\x03src\x18\x01 \x03(\x05\x12\x0e\n\x06target\x18\x02 \x03(\x05\"\xab\x01\n\x19\x45xecuteComputationRequest\x12\x35\n\tmethod_id\x18\x01 \x01(\x0e\x32\".pb_common_types.ComputationMethod\x12\r\n\x05token\x18\x02 \x01(\t\x12&\n\x05table\x18\x03 \x01(\x0b\x32\x17.libctomanage.JoinOrder\x12 \n\x03\x61rg\x18\x04 \x01(\x0b\x32\x13.libctomanage.Input\".\n\x1a\x45xecuteComputationResponse\x12\x10\n\x08job_uuid\x18\x03 \x01(\t\">\n\x1bGetComputationResultRequest\x12\x10\n\x08job_uuid\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\"\x8f\x02\n\x1cGetComputationResultResponse\x12\x0e\n\x06result\x18\x03 \x03(\t\x12\x15\n\rcolumn_number\x18\x04 \x01(\x05\x12*\n\x06status\x18\x05 \x01(\x0e\x32\x1a.pb_common_types.JobStatus\x12\x10\n\x08piece_id\x18\x06 \x01(\x05\x12\x33\n\x08progress\x18\x07 \x01(\x0b\x32\x1c.pb_common_types.JobProgressH\x01\x88\x01\x01\x12\x11\n\x07is_dim1\x18\x08 \x01(\x08H\x00\x12\x11\n\x07is_dim2\x18\t \x01(\x08H\x00\x12\x13\n\tis_schema\x18\n \x01(\x08H\x00\x42\r\n\x0bresult_typeB\x0b\n\t_progress\"#\n\x12GetDataListRequest\x12\r\n\x05token\x18\x01 \x01(\t\"%\n\x13GetDataListResponse\x12\x0e\n\x06result\x18\x01 \x01(\t\"8\n\x15GetElapsedTimeRequest\x12\x10\n\x08job_uuid\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\".\n\x16GetElapsedTimeResponse\x12\x14\n\x0c\x65lapsed_time\x18\x01 \x01(\x01\"9\n\x16GetJobErrorInfoRequest\x12\x10\n\x08job_uuid\x18\x01 \x01(\t\x12\r\n\x05token\x18\x02 \x01(\t\"h\n\x17GetJobErrorInfoResponse\x12:\n\x0ejob_error_info\x18\x01 \x01(\x0b\x32\x1d.pb_common_types.JobErrorInfoH\x00\x88\x01\x01\x42\x11\n\x0f_job_error_info2\xe9\x05\n\x0cLibcToManage\x12G\n\nSendShares\x12\x1f.libctomanage.SendSharesRequest\x1a\x16.google.protobuf.Empty\"\x00\x12K\n\x0c\x44\x65leteShares\x12!.libctomanage.DeleteSharesRequest\x1a\x16.google.protobuf.Empty\"\x00\x12N\n\tGetSchema\x12\x1e.libctomanage.GetSchemaRequest\x1a\x1f.libctomanage.GetSchemaResponse\"\x00\x12i\n\x12\x45xecuteComputation\x12\'.libctomanage.ExecuteComputationRequest\x1a(.libctomanage.ExecuteComputationResponse\"\x00\x12q\n\x14GetComputationResult\x12).libctomanage.GetComputationResultRequest\x1a*.libctomanage.GetComputationResultResponse\"\x00\x30\x01\x12T\n\x0bGetDataList\x12 .libctomanage.GetDataListRequest\x1a!.libctomanage.GetDataListResponse\"\x00\x12]\n\x0eGetElapsedTime\x12#.libctomanage.GetElapsedTimeRequest\x1a$.libctomanage.GetElapsedTimeResponse\"\x00\x12`\n\x0fGetJobErrorInfo\x12$.libctomanage.GetJobErrorInfoRequest\x1a%.libctomanage.GetJobErrorInfoResponse\"\x00\x42\x45ZCgithub.com/acompany-develop/QuickMPC/proto/libc_to_manage_containerb\x06proto3')
 
 
 _SENDSHARESREQUEST = DESCRIPTOR.message_types_by_name['SendSharesRequest']
-_SENDSHARESRESPONSE = DESCRIPTOR.message_types_by_name['SendSharesResponse']
 _DELETESHARESREQUEST = DESCRIPTOR.message_types_by_name['DeleteSharesRequest']
-_DELETESHARESRESPONSE = DESCRIPTOR.message_types_by_name['DeleteSharesResponse']
 _GETSCHEMAREQUEST = DESCRIPTOR.message_types_by_name['GetSchemaRequest']
 _GETSCHEMARESPONSE = DESCRIPTOR.message_types_by_name['GetSchemaResponse']
 _JOINORDER = DESCRIPTOR.message_types_by_name['JoinOrder']
 _INPUT = DESCRIPTOR.message_types_by_name['Input']
 _EXECUTECOMPUTATIONREQUEST = DESCRIPTOR.message_types_by_name['ExecuteComputationRequest']
 _EXECUTECOMPUTATIONRESPONSE = DESCRIPTOR.message_types_by_name['ExecuteComputationResponse']
 _GETCOMPUTATIONRESULTREQUEST = DESCRIPTOR.message_types_by_name['GetComputationResultRequest']
@@ -37,35 +36,21 @@
 SendSharesRequest = _reflection.GeneratedProtocolMessageType('SendSharesRequest', (_message.Message,), {
     'DESCRIPTOR': _SENDSHARESREQUEST,
     '__module__': 'libc_to_manage_pb2'
     # @@protoc_insertion_point(class_scope:libctomanage.SendSharesRequest)
 })
 _sym_db.RegisterMessage(SendSharesRequest)
 
-SendSharesResponse = _reflection.GeneratedProtocolMessageType('SendSharesResponse', (_message.Message,), {
-    'DESCRIPTOR': _SENDSHARESRESPONSE,
-    '__module__': 'libc_to_manage_pb2'
-    # @@protoc_insertion_point(class_scope:libctomanage.SendSharesResponse)
-})
-_sym_db.RegisterMessage(SendSharesResponse)
-
 DeleteSharesRequest = _reflection.GeneratedProtocolMessageType('DeleteSharesRequest', (_message.Message,), {
     'DESCRIPTOR': _DELETESHARESREQUEST,
     '__module__': 'libc_to_manage_pb2'
     # @@protoc_insertion_point(class_scope:libctomanage.DeleteSharesRequest)
 })
 _sym_db.RegisterMessage(DeleteSharesRequest)
 
-DeleteSharesResponse = _reflection.GeneratedProtocolMessageType('DeleteSharesResponse', (_message.Message,), {
-    'DESCRIPTOR': _DELETESHARESRESPONSE,
-    '__module__': 'libc_to_manage_pb2'
-    # @@protoc_insertion_point(class_scope:libctomanage.DeleteSharesResponse)
-})
-_sym_db.RegisterMessage(DeleteSharesResponse)
-
 GetSchemaRequest = _reflection.GeneratedProtocolMessageType('GetSchemaRequest', (_message.Message,), {
     'DESCRIPTOR': _GETSCHEMAREQUEST,
     '__module__': 'libc_to_manage_pb2'
     # @@protoc_insertion_point(class_scope:libctomanage.GetSchemaRequest)
 })
 _sym_db.RegisterMessage(GetSchemaRequest)
 
@@ -161,46 +146,42 @@
 _sym_db.RegisterMessage(GetJobErrorInfoResponse)
 
 _LIBCTOMANAGE = DESCRIPTOR.services_by_name['LibcToManage']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'ZCgithub.com/acompany-develop/QuickMPC/proto/libc_to_manage_container'
-    _SENDSHARESREQUEST._serialized_start = 72
-    _SENDSHARESREQUEST._serialized_end = 240
-    _SENDSHARESRESPONSE._serialized_start = 242
-    _SENDSHARESRESPONSE._serialized_end = 294
-    _DELETESHARESREQUEST._serialized_start = 296
-    _DELETESHARESREQUEST._serialized_end = 349
-    _DELETESHARESRESPONSE._serialized_start = 351
-    _DELETESHARESRESPONSE._serialized_end = 405
-    _GETSCHEMAREQUEST._serialized_start = 407
-    _GETSCHEMAREQUEST._serialized_end = 457
-    _GETSCHEMARESPONSE._serialized_start = 459
-    _GETSCHEMARESPONSE._serialized_end = 551
-    _JOINORDER._serialized_start = 553
-    _JOINORDER._serialized_end = 610
-    _INPUT._serialized_start = 612
-    _INPUT._serialized_end = 648
-    _EXECUTECOMPUTATIONREQUEST._serialized_start = 651
-    _EXECUTECOMPUTATIONREQUEST._serialized_end = 822
-    _EXECUTECOMPUTATIONRESPONSE._serialized_start = 824
-    _EXECUTECOMPUTATIONRESPONSE._serialized_end = 902
-    _GETCOMPUTATIONRESULTREQUEST._serialized_start = 904
-    _GETCOMPUTATIONRESULTREQUEST._serialized_end = 966
-    _GETCOMPUTATIONRESULTRESPONSE._serialized_start = 969
-    _GETCOMPUTATIONRESULTRESPONSE._serialized_end = 1272
-    _GETDATALISTREQUEST._serialized_start = 1274
-    _GETDATALISTREQUEST._serialized_end = 1309
-    _GETDATALISTRESPONSE._serialized_start = 1311
-    _GETDATALISTRESPONSE._serialized_end = 1363
-    _GETELAPSEDTIMEREQUEST._serialized_start = 1365
-    _GETELAPSEDTIMEREQUEST._serialized_end = 1421
-    _GETELAPSEDTIMERESPONSE._serialized_start = 1423
-    _GETELAPSEDTIMERESPONSE._serialized_end = 1484
-    _GETJOBERRORINFOREQUEST._serialized_start = 1486
-    _GETJOBERRORINFOREQUEST._serialized_end = 1543
-    _GETJOBERRORINFORESPONSE._serialized_start = 1545
-    _GETJOBERRORINFORESPONSE._serialized_end = 1664
-    _LIBCTOMANAGE._serialized_start = 1667
-    _LIBCTOMANAGE._serialized_end = 2434
+    _SENDSHARESREQUEST._serialized_start = 101
+    _SENDSHARESREQUEST._serialized_end = 269
+    _DELETESHARESREQUEST._serialized_start = 271
+    _DELETESHARESREQUEST._serialized_end = 324
+    _GETSCHEMAREQUEST._serialized_start = 326
+    _GETSCHEMAREQUEST._serialized_end = 376
+    _GETSCHEMARESPONSE._serialized_start = 378
+    _GETSCHEMARESPONSE._serialized_end = 438
+    _JOINORDER._serialized_start = 440
+    _JOINORDER._serialized_end = 497
+    _INPUT._serialized_start = 499
+    _INPUT._serialized_end = 535
+    _EXECUTECOMPUTATIONREQUEST._serialized_start = 538
+    _EXECUTECOMPUTATIONREQUEST._serialized_end = 709
+    _EXECUTECOMPUTATIONRESPONSE._serialized_start = 711
+    _EXECUTECOMPUTATIONRESPONSE._serialized_end = 757
+    _GETCOMPUTATIONRESULTREQUEST._serialized_start = 759
+    _GETCOMPUTATIONRESULTREQUEST._serialized_end = 821
+    _GETCOMPUTATIONRESULTRESPONSE._serialized_start = 824
+    _GETCOMPUTATIONRESULTRESPONSE._serialized_end = 1095
+    _GETDATALISTREQUEST._serialized_start = 1097
+    _GETDATALISTREQUEST._serialized_end = 1132
+    _GETDATALISTRESPONSE._serialized_start = 1134
+    _GETDATALISTRESPONSE._serialized_end = 1171
+    _GETELAPSEDTIMEREQUEST._serialized_start = 1173
+    _GETELAPSEDTIMEREQUEST._serialized_end = 1229
+    _GETELAPSEDTIMERESPONSE._serialized_start = 1231
+    _GETELAPSEDTIMERESPONSE._serialized_end = 1277
+    _GETJOBERRORINFOREQUEST._serialized_start = 1279
+    _GETJOBERRORINFOREQUEST._serialized_end = 1336
+    _GETJOBERRORINFORESPONSE._serialized_start = 1338
+    _GETJOBERRORINFORESPONSE._serialized_end = 1442
+    _LIBCTOMANAGE._serialized_start = 1445
+    _LIBCTOMANAGE._serialized_end = 2190
 # @@protoc_insertion_point(module_scope)
```

### Comparing `quickmpc-0.3.3/quickmpc/proto/libc_to_manage_pb2.pyi` & `quickmpc-0.3.4/quickmpc/proto/libc_to_manage_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -51,35 +51,14 @@
         matching_column: builtins.int = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["data_id", b"data_id", "matching_column", b"matching_column", "piece_id", b"piece_id", "schema", b"schema", "sent_at", b"sent_at", "shares", b"shares", "token", b"token"]) -> None: ...
 
 global___SendSharesRequest = SendSharesRequest
 
-class SendSharesResponse(google.protobuf.message.Message):
-    """*
-    the message of SendSharesResponse
-    """
-
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    MESSAGE_FIELD_NUMBER: builtins.int
-    IS_OK_FIELD_NUMBER: builtins.int
-    message: builtins.str
-    is_ok: builtins.bool
-    def __init__(
-        self,
-        *,
-        message: builtins.str = ...,
-        is_ok: builtins.bool = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["is_ok", b"is_ok", "message", b"message"]) -> None: ...
-
-global___SendSharesResponse = SendSharesResponse
-
 class DeleteSharesRequest(google.protobuf.message.Message):
     """*
     the message of DeleteSharesRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -94,35 +73,14 @@
         dataIds: collections.abc.Iterable[builtins.str] | None = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["dataIds", b"dataIds", "token", b"token"]) -> None: ...
 
 global___DeleteSharesRequest = DeleteSharesRequest
 
-class DeleteSharesResponse(google.protobuf.message.Message):
-    """*
-    the message of DeleteSharesResponse
-    """
-
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    MESSAGE_FIELD_NUMBER: builtins.int
-    IS_OK_FIELD_NUMBER: builtins.int
-    message: builtins.str
-    is_ok: builtins.bool
-    def __init__(
-        self,
-        *,
-        message: builtins.str = ...,
-        is_ok: builtins.bool = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["is_ok", b"is_ok", "message", b"message"]) -> None: ...
-
-global___DeleteSharesResponse = DeleteSharesResponse
-
 class GetSchemaRequest(google.protobuf.message.Message):
     """*
     the message of GetSchemaRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -143,29 +101,23 @@
 class GetSchemaResponse(google.protobuf.message.Message):
     """*
     the message of GetSchemaResponse
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    MESSAGE_FIELD_NUMBER: builtins.int
-    IS_OK_FIELD_NUMBER: builtins.int
     SCHEMA_FIELD_NUMBER: builtins.int
-    message: builtins.str
-    is_ok: builtins.bool
     @property
     def schema(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[common_types.common_types_pb2.Schema]: ...
     def __init__(
         self,
         *,
-        message: builtins.str = ...,
-        is_ok: builtins.bool = ...,
         schema: collections.abc.Iterable[common_types.common_types_pb2.Schema] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["is_ok", b"is_ok", "message", b"message", "schema", b"schema"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["schema", b"schema"]) -> None: ...
 
 global___GetSchemaResponse = GetSchemaResponse
 
 class JoinOrder(google.protobuf.message.Message):
     """*
     the message of ExecuteComputationRequest
     """
@@ -240,28 +192,22 @@
 class ExecuteComputationResponse(google.protobuf.message.Message):
     """
     the message of ExecuteComputationResponse
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    MESSAGE_FIELD_NUMBER: builtins.int
-    IS_OK_FIELD_NUMBER: builtins.int
     JOB_UUID_FIELD_NUMBER: builtins.int
-    message: builtins.str
-    is_ok: builtins.bool
     job_uuid: builtins.str
     def __init__(
         self,
         *,
-        message: builtins.str = ...,
-        is_ok: builtins.bool = ...,
         job_uuid: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["is_ok", b"is_ok", "job_uuid", b"job_uuid", "message", b"message"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["job_uuid", b"job_uuid"]) -> None: ...
 
 global___ExecuteComputationResponse = ExecuteComputationResponse
 
 class GetComputationResultRequest(google.protobuf.message.Message):
     """*
     the message of GetComputationResultRequest
     """
@@ -285,52 +231,46 @@
 class GetComputationResultResponse(google.protobuf.message.Message):
     """*
     the message of GetComputationResultResponse
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    MESSAGE_FIELD_NUMBER: builtins.int
-    IS_OK_FIELD_NUMBER: builtins.int
     RESULT_FIELD_NUMBER: builtins.int
     COLUMN_NUMBER_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     PIECE_ID_FIELD_NUMBER: builtins.int
     PROGRESS_FIELD_NUMBER: builtins.int
     IS_DIM1_FIELD_NUMBER: builtins.int
     IS_DIM2_FIELD_NUMBER: builtins.int
     IS_SCHEMA_FIELD_NUMBER: builtins.int
-    message: builtins.str
-    is_ok: builtins.bool
     @property
     def result(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     column_number: builtins.int
     status: common_types.common_types_pb2.JobStatus.ValueType
     piece_id: builtins.int
     @property
     def progress(self) -> common_types.common_types_pb2.JobProgress: ...
     is_dim1: builtins.bool
     is_dim2: builtins.bool
     is_schema: builtins.bool
     def __init__(
         self,
         *,
-        message: builtins.str = ...,
-        is_ok: builtins.bool = ...,
         result: collections.abc.Iterable[builtins.str] | None = ...,
         column_number: builtins.int = ...,
         status: common_types.common_types_pb2.JobStatus.ValueType = ...,
         piece_id: builtins.int = ...,
         progress: common_types.common_types_pb2.JobProgress | None = ...,
         is_dim1: builtins.bool = ...,
         is_dim2: builtins.bool = ...,
         is_schema: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["_progress", b"_progress", "is_dim1", b"is_dim1", "is_dim2", b"is_dim2", "is_schema", b"is_schema", "progress", b"progress", "result_type", b"result_type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_progress", b"_progress", "column_number", b"column_number", "is_dim1", b"is_dim1", "is_dim2", b"is_dim2", "is_ok", b"is_ok", "is_schema", b"is_schema", "message", b"message", "piece_id", b"piece_id", "progress", b"progress", "result", b"result", "result_type", b"result_type", "status", b"status"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_progress", b"_progress", "column_number", b"column_number", "is_dim1", b"is_dim1", "is_dim2", b"is_dim2", "is_schema", b"is_schema", "piece_id", b"piece_id", "progress", b"progress", "result", b"result", "result_type", b"result_type", "status", b"status"]) -> None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_progress", b"_progress"]) -> typing_extensions.Literal["progress"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["result_type", b"result_type"]) -> typing_extensions.Literal["is_dim1", "is_dim2", "is_schema"] | None: ...
 
 global___GetComputationResultResponse = GetComputationResultResponse
 
@@ -348,24 +288,21 @@
 
 global___GetDataListRequest = GetDataListRequest
 
 class GetDataListResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESULT_FIELD_NUMBER: builtins.int
-    IS_OK_FIELD_NUMBER: builtins.int
     result: builtins.str
-    is_ok: builtins.bool
     def __init__(
         self,
         *,
         result: builtins.str = ...,
-        is_ok: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["is_ok", b"is_ok", "result", b"result"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["result", b"result"]) -> None: ...
 
 global___GetDataListResponse = GetDataListResponse
 
 class GetElapsedTimeRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_UUID_FIELD_NUMBER: builtins.int
@@ -381,25 +318,22 @@
     def ClearField(self, field_name: typing_extensions.Literal["job_uuid", b"job_uuid", "token", b"token"]) -> None: ...
 
 global___GetElapsedTimeRequest = GetElapsedTimeRequest
 
 class GetElapsedTimeResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    IS_OK_FIELD_NUMBER: builtins.int
     ELAPSED_TIME_FIELD_NUMBER: builtins.int
-    is_ok: builtins.bool
     elapsed_time: builtins.float
     def __init__(
         self,
         *,
-        is_ok: builtins.bool = ...,
         elapsed_time: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["elapsed_time", b"elapsed_time", "is_ok", b"is_ok"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["elapsed_time", b"elapsed_time"]) -> None: ...
 
 global___GetElapsedTimeResponse = GetElapsedTimeResponse
 
 class GetJobErrorInfoRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_UUID_FIELD_NUMBER: builtins.int
@@ -416,22 +350,19 @@
 
 global___GetJobErrorInfoRequest = GetJobErrorInfoRequest
 
 class GetJobErrorInfoResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_ERROR_INFO_FIELD_NUMBER: builtins.int
-    IS_OK_FIELD_NUMBER: builtins.int
     @property
     def job_error_info(self) -> common_types.common_types_pb2.JobErrorInfo: ...
-    is_ok: builtins.bool
     def __init__(
         self,
         *,
         job_error_info: common_types.common_types_pb2.JobErrorInfo | None = ...,
-        is_ok: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["_job_error_info", b"_job_error_info", "job_error_info", b"job_error_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["_job_error_info", b"_job_error_info", "is_ok", b"is_ok", "job_error_info", b"job_error_info"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["_job_error_info", b"_job_error_info", "job_error_info", b"job_error_info"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_job_error_info", b"_job_error_info"]) -> typing_extensions.Literal["job_error_info"] | None: ...
 
 global___GetJobErrorInfoResponse = GetJobErrorInfoResponse
```

### Comparing `quickmpc-0.3.3/quickmpc/proto/libc_to_manage_pb2_grpc.py` & `quickmpc-0.3.4/quickmpc/proto/libc_to_manage_pb2_grpc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
+from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 import libc_to_manage_pb2 as libc__to__manage__pb2
 
 
 class LibcToManageStub(object):
     """*
     LibcToManage service
     """
@@ -15,20 +16,20 @@
 
         Args:
             channel: A grpc.Channel.
         """
         self.SendShares = channel.unary_unary(
             '/libctomanage.LibcToManage/SendShares',
             request_serializer=libc__to__manage__pb2.SendSharesRequest.SerializeToString,
-            response_deserializer=libc__to__manage__pb2.SendSharesResponse.FromString,
+            response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
         )
         self.DeleteShares = channel.unary_unary(
             '/libctomanage.LibcToManage/DeleteShares',
             request_serializer=libc__to__manage__pb2.DeleteSharesRequest.SerializeToString,
-            response_deserializer=libc__to__manage__pb2.DeleteSharesResponse.FromString,
+            response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
         )
         self.GetSchema = channel.unary_unary(
             '/libctomanage.LibcToManage/GetSchema',
             request_serializer=libc__to__manage__pb2.GetSchemaRequest.SerializeToString,
             response_deserializer=libc__to__manage__pb2.GetSchemaResponse.FromString,
         )
         self.ExecuteComputation = channel.unary_unary(
@@ -113,20 +114,20 @@
 
 
 def add_LibcToManageServicer_to_server(servicer, server):
     rpc_method_handlers = {
         'SendShares': grpc.unary_unary_rpc_method_handler(
             servicer.SendShares,
             request_deserializer=libc__to__manage__pb2.SendSharesRequest.FromString,
-            response_serializer=libc__to__manage__pb2.SendSharesResponse.SerializeToString,
+            response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
         ),
         'DeleteShares': grpc.unary_unary_rpc_method_handler(
             servicer.DeleteShares,
             request_deserializer=libc__to__manage__pb2.DeleteSharesRequest.FromString,
-            response_serializer=libc__to__manage__pb2.DeleteSharesResponse.SerializeToString,
+            response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
         ),
         'GetSchema': grpc.unary_unary_rpc_method_handler(
             servicer.GetSchema,
             request_deserializer=libc__to__manage__pb2.GetSchemaRequest.FromString,
             response_serializer=libc__to__manage__pb2.GetSchemaResponse.SerializeToString,
         ),
         'ExecuteComputation': grpc.unary_unary_rpc_method_handler(
@@ -176,15 +177,15 @@
                    insecure=False,
                    compression=None,
                    wait_for_ready=None,
                    timeout=None,
                    metadata=None):
         return grpc.experimental.unary_unary(request, target, '/libctomanage.LibcToManage/SendShares',
                                              libc__to__manage__pb2.SendSharesRequest.SerializeToString,
-                                             libc__to__manage__pb2.SendSharesResponse.FromString,
+                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def DeleteShares(request,
                      target,
                      options=(),
@@ -193,15 +194,15 @@
                      insecure=False,
                      compression=None,
                      wait_for_ready=None,
                      timeout=None,
                      metadata=None):
         return grpc.experimental.unary_unary(request, target, '/libctomanage.LibcToManage/DeleteShares',
                                              libc__to__manage__pb2.DeleteSharesRequest.SerializeToString,
-                                             libc__to__manage__pb2.DeleteSharesResponse.FromString,
+                                             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def GetSchema(request,
                   target,
                   options=(),
```

### Comparing `quickmpc-0.3.3/quickmpc/proto/libc_to_manage_pb2_grpc.pyi` & `quickmpc-0.3.4/quickmpc/proto/libc_to_manage_pb2_grpc.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import abc
 import collections.abc
+import google.protobuf.empty_pb2
 import grpc
 import libc_to_manage_pb2
 
 class LibcToManageStub:
     """*
     LibcToManage service
     """
 
     def __init__(self, channel: grpc.Channel) -> None: ...
     SendShares: grpc.UnaryUnaryMultiCallable[
         libc_to_manage_pb2.SendSharesRequest,
-        libc_to_manage_pb2.SendSharesResponse,
+        google.protobuf.empty_pb2.Empty,
     ]
     DeleteShares: grpc.UnaryUnaryMultiCallable[
         libc_to_manage_pb2.DeleteSharesRequest,
-        libc_to_manage_pb2.DeleteSharesResponse,
+        google.protobuf.empty_pb2.Empty,
     ]
     GetSchema: grpc.UnaryUnaryMultiCallable[
         libc_to_manage_pb2.GetSchemaRequest,
         libc_to_manage_pb2.GetSchemaResponse,
     ]
     ExecuteComputation: grpc.UnaryUnaryMultiCallable[
         libc_to_manage_pb2.ExecuteComputationRequest,
@@ -52,21 +53,21 @@
     """
 
     @abc.abstractmethod
     def SendShares(
         self,
         request: libc_to_manage_pb2.SendSharesRequest,
         context: grpc.ServicerContext,
-    ) -> libc_to_manage_pb2.SendSharesResponse: ...
+    ) -> google.protobuf.empty_pb2.Empty: ...
     @abc.abstractmethod
     def DeleteShares(
         self,
         request: libc_to_manage_pb2.DeleteSharesRequest,
         context: grpc.ServicerContext,
-    ) -> libc_to_manage_pb2.DeleteSharesResponse: ...
+    ) -> google.protobuf.empty_pb2.Empty: ...
     @abc.abstractmethod
     def GetSchema(
         self,
         request: libc_to_manage_pb2.GetSchemaRequest,
         context: grpc.ServicerContext,
     ) -> libc_to_manage_pb2.GetSchemaResponse: ...
     @abc.abstractmethod
```

### Comparing `quickmpc-0.3.3/quickmpc/qmpc.py` & `quickmpc-0.3.4/quickmpc/qmpc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import logging
 from dataclasses import dataclass, field, InitVar
 from typing import Dict, List, Optional, Tuple
 
 from .proto.common_types import common_types_pb2
 from .qmpc_server import QMPCServer
 from .share import Share
-from .utils.parse_csv import (parse, parse_csv, parse_csv_to_bitvector,
-                              parse_to_bitvector, ShareValueType)
+from .utils.parse_csv import (parse, parse_csv, ShareValueType)
 from .utils.restore import restore
 
 logger = logging.getLogger(__name__)
 # qmpc.JobStatus でアクセスできるようにエイリアスを設定する
 JobStatus \
     = common_types_pb2.JobStatus
 ComputationMethod \
@@ -40,40 +39,22 @@
                        filename: str,
                        matching_column: Optional[int] = 1) \
             -> Tuple[List[List[ShareValueType]], List[Schema]]:
         logger.info("parse_csv_file. "
                     f"[filename]='{filename}'")
         return parse_csv(filename, matching_column)
 
-    def parse_csv_file_to_bitvector(self, filename: str,
-                                    exclude: List[int] = [],
-                                    matching_column: Optional[int] = 1) \
-            -> Tuple[List[List[ShareValueType]], List[Schema]]:
-        logger.info("parse_csv_file_to_bitvector. "
-                    f"[filename]='{filename}' "
-                    f"[not bitvector columns]={exclude}")
-        return parse_csv_to_bitvector(filename, exclude, matching_column)
-
     def parse_csv_data(self,
                        data: List[List[str]],
                        matching_column: Optional[int] = 1) \
             -> Tuple[List[List[ShareValueType]], List[Schema]]:
         logger.info("parse_csv_data. "
                     f"[data size]={len(data)}x{len(data[0])}")
         return parse(data, matching_column)
 
-    def parse_csv_data_to_bitvector(self, data: List[List[str]],
-                                    exclude: List[int] = [],
-                                    matching_column: Optional[int] = 1) \
-            -> Tuple[List[List[ShareValueType]], List[Schema]]:
-        logger.info("parse_csv_file_to_bitvector. "
-                    f"[data size]={len(data)}x{len(data[0])} "
-                    f"[not bitvector columns]={exclude}")
-        return parse_to_bitvector(data, exclude, matching_column)
-
     def send_share(self, secrets: List, schema: List[Schema],
                    matching_column: int = 1,
                    piece_size: int = 1_000_000) -> Dict:
         logger.info("send_share request. "
                     f"[secrets size]={len(secrets)}x{len(secrets[0])} "
                     f"[matching ID name]={schema[matching_column-1]}")
         return self.__qmpc_server.send_share(
@@ -124,61 +105,25 @@
                     f"[matching ID columns]={join_order[2]} "
                     f"[src columns]={inp[0]}"
                     f"[target columns]={inp[1]}")
         return self.__qmpc_server.execute_computation(
             ComputationMethod.Value("COMPUTATION_METHOD_CORREL"),
             join_order, inp)
 
-    def linear_regression(self, join_order: Tuple[List, List, List],
-                          inp: Tuple[List, List]) -> Dict:
-        logger.info("linear_regression request. "
-                    f"[data_id list]={join_order[0]} "
-                    f"[join method]={join_order[1]} "
-                    f"[matching ID columns]={join_order[2]} "
-                    f"[design variable columns]={inp[0]}"
-                    f"[objective variable columns]={inp[1]}")
-        return self.__qmpc_server.execute_computation(
-            ComputationMethod.Value("COMPUTATION_METHOD_LINEAR_REGRESSION"),
-            join_order, inp)
-
-    def logistic_regression(self, join_order: Tuple[List, List, List],
-                            inp: Tuple[List, List]) -> Dict:
-        logger.info("logistic_regression request. "
-                    f"[data_id list]={join_order[0]} "
-                    f"[join method]={join_order[1]} "
-                    f"[matching ID columns]={join_order[2]} "
-                    f"[design variable columns]={inp[0]}"
-                    f"[objective variable columns]={inp[1]}")
-        return self.__qmpc_server.execute_computation(
-            ComputationMethod.Value("COMPUTATION_METHOD_LOGISTIC_REGRESSION"),
-            join_order, inp)
-
     def meshcode(self, join_order: Tuple[List, List, List],
                  src: List) -> Dict:
         logger.info("meshcode request. "
                     f"[data_id list]={join_order[0]} "
                     f"[join method]={join_order[1]} "
                     f"[matching ID columns]={join_order[2]} "
                     f"[src columns]={src}")
         return self.__qmpc_server.execute_computation(
             ComputationMethod.Value("COMPUTATION_METHOD_MESH_CODE"),
             join_order, (src, []))
 
-    def decision_tree(self, join_order: Tuple[List, List, List],
-                      inp: Tuple[List, List]) -> Dict:
-        logger.info("decision_tree request. "
-                    f"[data_id list]={join_order[0]} "
-                    f"[join method]={join_order[1]} "
-                    f"[matching ID columns]={join_order[2]} "
-                    f"[design variable columns]={inp[0]}"
-                    f"[objective variable columns]={inp[1]}")
-        return self.__qmpc_server.execute_computation(
-            ComputationMethod.Value("COMPUTATION_METHOD_DECISION_TREE"),
-            join_order, inp)
-
     def get_join_table(self, join_order: Tuple[List, List, List]) -> Dict:
         logger.info("get_join_table request. "
                     f"[data_id list]={join_order[0]} "
                     f"[join method]={join_order[1]} "
                     f"[matching ID columns]={join_order[2]}")
         return self.__qmpc_server.execute_computation(
             ComputationMethod.Value("COMPUTATION_METHOD_JOIN_TABLE"),
```

### Comparing `quickmpc-0.3.3/quickmpc/qmpc_server.py` & `quickmpc-0.3.4/quickmpc/qmpc_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,23 +89,28 @@
         # TODO joinをenumにする
         if not all([0 <= join <= 2 for join in join_order[1]]):
             logger.error('join value must be in the range of 0 to 2')
             return False
         return True
 
     def __retry(self, f: Callable, *request: Any) -> Any:
-        for _ in range(self.retry_num):
+        for ch in self.__client_channels:
             # channelの接続チェック
-            try:
-                for ch in self.__client_channels:
-                    grpc.channel_ready_future(ch).result(timeout=5)
-            except grpc.FutureTimeoutError as e:
-                logger.error(e)
-                continue
+            is_channel_ready = False
+            for _ in range(self.retry_num):
+                try:
+                    grpc.channel_ready_future(ch).result(self.retry_wait_time)
+                    is_channel_ready = True
+                    break
+                except grpc.FutureTimeoutError as e:
+                    logger.error(e)
+            if not is_channel_ready:
+                raise RuntimeError("channel の準備が出来ません")
 
+        for _ in range(self.retry_num):
             # requestを送る
             try:
                 return f(*request)
             except grpc.RpcError as e:
                 logger.error(f'{e.details()} ({e.code()})')
 
                 # エラーが詳細な情報を持っているか確認
@@ -144,29 +149,23 @@
             response = [f.result() for f in futures]
         except (QMPCJobError, QMPCServerError):
             raise
         except Exception as e:
             is_ok = False
             logger.error(e)
 
-        for b in response:
-            if hasattr(b, "is_ok"):
-                is_ok &= b.is_ok
-            else:
-                is_ok &= b["is_ok"]
         return is_ok, response
 
     @staticmethod
     def __stream_result(stream: Iterable, job_uuid: str, party: int,
                         path: Optional[str]) -> Dict:
         """ エラーチェックしてstreamのresultを得る """
         is_ok: bool = True
         res_list = []
         for res in stream:
-            is_ok &= res.is_ok
             if path is not None:
                 file_title = "dim1"
                 if res.HasField("is_dim2"):
                     file_title = "dim2"
                 elif res.HasField("is_schema"):
                     file_title = "schema"
 
@@ -175,16 +174,14 @@
 
                 with open(file_path, 'w') as f:
                     writer = csv.writer(f)
                     writer.writerow([res.column_number])
                     writer.writerow(res.result)
                 progress = res.progress if res.HasField('progress') else None
                 res = GetComputationResultResponse(
-                    message=res.message,
-                    is_ok=res.is_ok,
                     column_number=res.column_number,
                     status=res.status,
                     piece_id=res.piece_id,
                     progress=progress,
                 )
             res_list.append(res)
         res_dict: Dict = {"is_ok": is_ok, "responses": res_list}
```

### Comparing `quickmpc-0.3.3/quickmpc/share.py` & `quickmpc-0.3.4/quickmpc/share.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/quickmpc/utils/make_pieces.py` & `quickmpc-0.3.4/quickmpc/utils/make_pieces.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/quickmpc/utils/overload_tools.py` & `quickmpc-0.3.4/quickmpc/utils/overload_tools.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/quickmpc/utils/parse_csv.py` & `quickmpc-0.3.4/quickmpc/utils/parse_csv.py`

 * *Files 24% similar despite different names*

```diff
@@ -157,63 +157,14 @@
 
     if not format_check(secrets, schema):
         raise RuntimeError("規定されたフォーマットでないデータです．")
 
     return secrets, schema
 
 
-def parse_to_bitvector(data: List[List[str]],
-                       exclude: List[int] = [],
-                       matching_column: Optional[int] = None) \
-        -> Tuple[List[List[ShareValueType]], List[Schema]]:
-    secrets, schema = parse(data, matching_column)
-
-    secrets_bitbevtor: List[List[float]] = []
-    schema_bitvector: List[Schema] = []
-    for col, (sec, sch) in enumerate(zip(np.transpose(secrets), schema)):
-        # 列が除外リストに含まれていたらそのままappend
-        if col in exclude:
-            secrets_bitbevtor.append(sec)
-            schema_bitvector.append(
-                Schema(
-                    name=sch.name + "#0",
-                    type=sch.type))
-            continue
-
-        # 座標圧縮
-        position: dict = {}
-        it: int = 0
-        for key in sec:
-            if key not in position:
-                position[key] = it
-                it += 1
-
-        # bitvector化
-        for key, val in position.items():
-            bitvector: list = [1 if (key == k) else 0 for k in sec]
-            sch_val: str = sch.name + "#" + str(val)
-            secrets_bitbevtor.append(bitvector)
-            schema_bitvector.append(
-                Schema(
-                    name=sch_val,
-                    type=ShareValueTypeEnum.SHARE_VALUE_TYPE_FIXED_POINT))
-
-    return np.transpose(secrets_bitbevtor).tolist(), schema_bitvector
-
-
 def parse_csv(
     filename: str, matching_column: Optional[int] = None) \
         -> Tuple[List[List[ShareValueType]], List[Schema]]:
     with open(filename) as f:
         reader = csv.reader(f)
         text: List[List[str]] = [row for row in reader]
         return parse(text, matching_column)
-
-
-def parse_csv_to_bitvector(filename: str,
-                           exclude: List[int] = [],
-                           matching_column: Optional[int] = None) ->  \
-        Tuple[List[List[ShareValueType]], List[Schema]]:
-    with open(filename) as f:
-        reader = csv.reader(f)
-        text: List[List[str]] = [row for row in reader]
-        return parse_to_bitvector(text, exclude, matching_column)
```

### Comparing `quickmpc-0.3.3/quickmpc/utils/random.py` & `quickmpc-0.3.4/quickmpc/utils/random.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/quickmpc/utils/restore.py` & `quickmpc-0.3.4/quickmpc/utils/restore.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/quickmpc.egg-info/SOURCES.txt` & `quickmpc-0.3.4/quickmpc.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -9,32 +9,14 @@
 README.md
 mypy.ini
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 .vscode/settings.json
-demo/Pipfile
-demo/README-ja.md
-demo/README.md
-demo/data/data-meshcode.csv
-demo/data/data1-1.csv
-demo/data/data1-2.csv
-demo/data/data1-3.csv
-demo/integration_demo/execute_demo.py
-demo/integration_demo/progress_demo.py
-demo/integration_demo/utils.py
-demo/unit_demo/delete_share.py
-demo/unit_demo/demo_sharize.py
-demo/unit_demo/execute_computation.py
-demo/unit_demo/get_computation_result.py
-demo/unit_demo/get_data_list.py
-demo/unit_demo/get_elapsed_time.py
-demo/unit_demo/get_join_table.py
-demo/unit_demo/send_share.py
 quickmpc/README.md
 quickmpc/__init__.py
 quickmpc/_version.py
 quickmpc/exception.py
 quickmpc/qmpc.py
 quickmpc/qmpc_server.py
 quickmpc/share.py
```

### Comparing `quickmpc-0.3.3/tests/unit_tests/certificates/server1.key` & `quickmpc-0.3.4/tests/unit_tests/certificates/server1.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/tests/unit_tests/certificates/server1.pem` & `quickmpc-0.3.4/tests/unit_tests/certificates/server1.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/tests/unit_tests/certificates/server2.key` & `quickmpc-0.3.4/tests/unit_tests/certificates/server2.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/tests/unit_tests/certificates/server2.pem` & `quickmpc-0.3.4/tests/unit_tests/certificates/server2.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/tests/unit_tests/certificates/server3.key` & `quickmpc-0.3.4/tests/unit_tests/certificates/server3.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/tests/unit_tests/certificates/server3.pem` & `quickmpc-0.3.4/tests/unit_tests/certificates/server3.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/tests/unit_tests/conftest.py` & `quickmpc-0.3.4/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/tests/unit_tests/local_server.py` & `quickmpc-0.3.4/tests/unit_tests/local_server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,30 @@
 """ テスト用のgrpc server """
 from concurrent import futures
 
 import grpc
-from google.protobuf import any_pb2
+from google.protobuf import any_pb2, empty_pb2
 from google.rpc import code_pb2, status_pb2
 from grpc_status import rpc_status
 
 from quickmpc.proto import libc_to_manage_pb2, libc_to_manage_pb2_grpc
 from quickmpc.proto.common_types import common_types_pb2
 from quickmpc.proto.common_types.common_types_pb2 import (JobErrorInfo,
                                                           Stacktrace)
 
 
 class LibToManageServiceServicer(libc_to_manage_pb2_grpc.LibcToManageServicer):
 
     def __init__(self): ...
 
     def SendShares(self, request, context):
-        res = libc_to_manage_pb2.SendSharesResponse(
-            message="ok",
-            is_ok=True
-        )
-        return res
+        return empty_pb2.Empty()
 
     def DeleteShares(self, request, context):
-        res = libc_to_manage_pb2.DeleteSharesResponse(
-            message="ok",
-            is_ok=True
-        )
-        return res
+        return empty_pb2.Empty()
 
     def ExecuteComputation(self, request, context):
         if len(request.arg.src) > 0 \
                 and request.arg.src[0] == 1000000000:
             # QMPCJobError
             # CC で Job 実行時にエラーが発生していた場合を再現
             detail = any_pb2.Any()
@@ -52,58 +44,50 @@
                 and request.table.dataIds[0] == "UnregisteredDataId":
             # QMPCServerError
             # MC で Internal Server Error が発生している場合を再現
             context.set_code(grpc.StatusCode.UNKNOWN)
             return libc_to_manage_pb2.ExecuteComputationResponse()
 
         res = libc_to_manage_pb2.ExecuteComputationResponse(
-            message="ok",
-            is_ok=True,
             job_uuid="jobjobjob"
         )
         return res
 
     def GetComputationResult(self, request, context):
         yield libc_to_manage_pb2.GetComputationResultResponse(
-            message="ok",
-            is_ok=True,
             result=["1"],
             status=common_types_pb2.COMPLETED,
             piece_id=1,
             column_number=2,
             is_dim1=True,
         )
         yield libc_to_manage_pb2.GetComputationResultResponse(
-            message="ok",
-            is_ok=True,
             result=["2"],
             status=common_types_pb2.COMPLETED,
             piece_id=2,
             column_number=2,
             is_dim1=True,
         )
 
     def GetDataList(self, request, context):
         res = libc_to_manage_pb2.GetDataListResponse(
-            is_ok=True,
             result="[]"
         )
         return res
 
     def GetJoinTable(self, request, context):
         res = libc_to_manage_pb2.GetJoinTableResponse(
             is_ok=True,
             result="['1']",
             schema=["s"]
         )
         return res
 
     def GetJobErrorInfo(self, request, context):
         res = libc_to_manage_pb2.GetJobErrorInfoResponse(
-            is_ok=True,
             job_error_info=JobErrorInfo(
                 what="QMPCJobError",
                 stacktrace=Stacktrace()
             )
         )
         return res
```

### Comparing `quickmpc-0.3.3/tests/unit_tests/test_files/edge_data.csv` & `quickmpc-0.3.4/tests/unit_tests/test_files/edge_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/tests/unit_tests/test_files/string_data.csv` & `quickmpc-0.3.4/tests/unit_tests/test_files/string_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/tests/unit_tests/test_make_pieces.py` & `quickmpc-0.3.4/tests/unit_tests/test_make_pieces.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/tests/unit_tests/test_over_load.py` & `quickmpc-0.3.4/tests/unit_tests/test_over_load.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/tests/unit_tests/test_parse.py` & `quickmpc-0.3.4/tests/unit_tests/test_parse.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import os
 from typing import List
 
 import numpy as np
 import pytest
 
 from quickmpc import Schema, ShareValueTypeEnum
-from quickmpc.utils.parse_csv import (parse, parse_csv, parse_csv_to_bitvector,
-                                      parse_to_bitvector)
+from quickmpc.utils.parse_csv import parse, parse_csv
 
 
 def schema_fp(name: str):
     return Schema(name=name,
                   type=ShareValueTypeEnum.SHARE_VALUE_TYPE_FIXED_POINT)
 
 
@@ -26,21 +25,14 @@
     "id,attr1,attr2,attr3,attr4,attr5,attr6",
     "hoge,0,0.77,0.63,0.35,0.39,0.35",
     "huga,0,0.37,0.36,0.43,0.41,0.39",
     "piyo,1,0.34,0.34,0.44,0.50,0.32",
     "moge,1,0.47,0.43,0.34,0.29,0.34",
     "moga,0,0.67,0.41,0.25,0.49,0.25",
 ]]
-bitvector_data: List[List[str]] = [s.split(",") for s in [
-    "id,attr1,attr2,attr3",
-    "hoge,0,1,3",
-    "huga,0,2,1",
-    "moge,1,0,4",
-    "moga,0,1,2",
-]]
 data3: List[List[str]] = [s.split(",") for s in [
     "id,id:id",
     "hoge,hoge",
     "huga,huga",
     "moge,moge",
     "moga,moga",
 ]]
@@ -80,22 +72,14 @@
 def test_parse():
     """ 正しくパースできるかTest """
     secrets, schema = parse(normal_data, matching_column=1)
     assert (np.allclose(secrets, d1_secrets))
     assert (schema == d1_schema)
 
 
-def test_parse_to_bitvector():
-    """ 正しくパースできるかTest """
-    secrets, schema = parse_to_bitvector(
-        bitvector_data, [0], matching_column=1)
-    assert (np.allclose(secrets, d2_secrets))
-    assert (schema == d2_schema)
-
-
 def test_parse_str():
     secrets, schema = parse(data3)
     assert (np.allclose(secrets, d3_secrets))
     assert (schema == d3_schema)
 
 
 def test_parse_errorhandring():
@@ -225,23 +209,14 @@
             if type(x) == int:
                 assert x == y
             else:
                 assert math.isclose(x, y)
     assert (schema == expected_schema)
 
 
-def test_parse_csv_to_bitvector():
-    """ csvを正しくパースできるかTest """
-    secrets, schema = parse_csv_to_bitvector(
-        f"{os.path.dirname(__file__)}/test_files/bitvector.csv",
-        [0], matching_column=1)
-    assert (np.allclose(secrets, d2_secrets))
-    assert (schema == d2_schema)
-
-
 @pytest.mark.parametrize(
     ("csv_file", "expected_exception"),
     [
         # ファイルが存在しない
         ("hoge", Exception),
 
         # 列数が異なる
```

### Comparing `quickmpc-0.3.3/tests/unit_tests/test_qmpc.py` & `quickmpc-0.3.4/tests/unit_tests/test_qmpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,8 +164,8 @@
             (qmpc_failed.get_job_error_info, ["uuid"]),
         ]
     )
     def test_retry(self, function, argument, caplog,
                    run_server1, run_server2, run_server3):
         # 10回の retry に失敗したら "All 10 times it was an error" が log に出るかをテスト
         _ = function(*argument)
-        assert "All 10 times it was an error" in caplog.text
+        assert "channel の準備が出来ません" in caplog.text
```

### Comparing `quickmpc-0.3.3/tests/unit_tests/test_random.py` & `quickmpc-0.3.4/tests/unit_tests/test_random.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/tests/unit_tests/test_restore.py` & `quickmpc-0.3.4/tests/unit_tests/test_restore.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/tests/unit_tests/test_share_recons.py` & `quickmpc-0.3.4/tests/unit_tests/test_share_recons.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.3.3/tests/unit_tests/test_share_sharize.py` & `quickmpc-0.3.4/tests/unit_tests/test_share_sharize.py`

 * *Files identical despite different names*

