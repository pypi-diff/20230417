# Comparing `tmp/tbats-1.1.2.tar.gz` & `tmp/tbats-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tbats-1.1.2.tar", last modified: Fri Dec  9 07:31:30 2022, max compression
+gzip compressed data, was "tbats-1.1.3.tar", last modified: Mon Apr 17 10:19:05 2023, max compression
```

## Comparing `tbats-1.1.2.tar` & `tbats-1.1.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 grzegorzskorupa   (502) staff       (20)        0 2022-12-09 07:31:30.708150 tbats-1.1.2/
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)       46 2020-01-08 08:35:13.000000 tbats-1.1.2/AUTHORS.txt
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     1075 2020-01-08 08:35:13.000000 tbats-1.1.2/LICENSE
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     3613 2022-12-09 07:31:30.707958 tbats-1.1.2/PKG-INFO
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     3105 2022-10-05 07:44:59.000000 tbats-1.1.2/README.md
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)       38 2022-12-09 07:31:30.708207 tbats-1.1.2/setup.cfg
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     2199 2022-12-09 07:25:45.000000 tbats-1.1.2/setup.py
-drwxr-xr-x   0 grzegorzskorupa   (502) staff       (20)        0 2022-12-09 07:31:30.657065 tbats-1.1.2/tbats/
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      239 2022-12-09 07:29:58.000000 tbats-1.1.2/tbats/__init__.py
-drwxr-xr-x   0 grzegorzskorupa   (502) staff       (20)        0 2022-12-09 07:31:30.679869 tbats-1.1.2/tbats/abstract/
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      799 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/abstract/ArrayHelper.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     2983 2020-02-03 13:47:24.000000 tbats-1.1.2/tbats/abstract/Case.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     2178 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/abstract/ComponentMatrix.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     6200 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/abstract/Components.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      795 2020-07-27 13:43:11.000000 tbats-1.1.2/tbats/abstract/Context.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     1360 2020-07-27 14:06:09.000000 tbats-1.1.2/tbats/abstract/ContextInterface.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)    10794 2020-07-27 13:36:01.000000 tbats-1.1.2/tbats/abstract/Estimator.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     4140 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/abstract/MatrixBuilder.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      971 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/abstract/MatrixBuilderCache.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      307 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/abstract/MatrixBuilderInterface.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)    12493 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/abstract/Model.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)    10935 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/abstract/ModelParams.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     6693 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/abstract/ParamsOptimizer.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      845 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/abstract/SeedFinder.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      798 2020-07-27 14:05:13.000000 tbats-1.1.2/tbats/abstract/__init__.py
-drwxr-xr-x   0 grzegorzskorupa   (502) staff       (20)        0 2022-12-09 07:31:30.689160 tbats-1.1.2/tbats/bats/
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     3919 2020-07-27 14:05:13.000000 tbats-1.1.2/tbats/bats/BATS.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      781 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/bats/Case.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     1376 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/bats/Components.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     1303 2020-07-27 13:39:03.000000 tbats-1.1.2/tbats/bats/Context.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     1857 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/bats/MatrixBuilder.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      136 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/bats/Model.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     2781 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/bats/ModelParams.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      170 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/bats/ParamsOptimizer.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     4181 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/bats/SeedFinder.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      431 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/bats/__init__.py
-drwxr-xr-x   0 grzegorzskorupa   (502) staff       (20)        0 2022-12-09 07:31:30.694842 tbats-1.1.2/tbats/error/
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)       41 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/error/BatsException.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)       41 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/error/BatsWarning.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      569 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/error/ExceptionHandler.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)       80 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/error/InputArgsException.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)       74 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/error/InputArgsWarning.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)       70 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/error/ModelWarning.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      384 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/error/__init__.py
-drwxr-xr-x   0 grzegorzskorupa   (502) staff       (20)        0 2022-12-09 07:31:30.703915 tbats-1.1.2/tbats/tbats/
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      568 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/tbats/Case.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     4314 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/tbats/Components.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     1429 2020-07-27 14:02:49.000000 tbats-1.1.2/tbats/tbats/Context.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)    10462 2020-07-27 14:00:21.000000 tbats-1.1.2/tbats/tbats/HarmonicsChoosingStrategy.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     2560 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/tbats/MatrixBuilder.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      136 2022-12-09 07:24:51.000000 tbats-1.1.2/tbats/tbats/Model.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     3197 2020-08-18 07:09:32.000000 tbats-1.1.2/tbats/tbats/ModelParams.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      170 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/tbats/ParamsOptimizer.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      832 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/tbats/SeedFinder.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     4966 2020-07-27 13:41:06.000000 tbats-1.1.2/tbats/tbats/TBATS.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      528 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/tbats/__init__.py
-drwxr-xr-x   0 grzegorzskorupa   (502) staff       (20)        0 2022-12-09 07:31:30.707489 tbats-1.1.2/tbats/transformation/
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     1601 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/transformation/BoxCox.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     2277 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/transformation/Guerrero.py
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      162 2020-01-08 08:35:13.000000 tbats-1.1.2/tbats/transformation/__init__.py
-drwxr-xr-x   0 grzegorzskorupa   (502) staff       (20)        0 2022-12-09 07:31:30.659262 tbats-1.1.2/tbats.egg-info/
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     3613 2022-12-09 07:31:30.000000 tbats-1.1.2/tbats.egg-info/PKG-INFO
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     1488 2022-12-09 07:31:30.000000 tbats-1.1.2/tbats.egg-info/SOURCES.txt
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)        1 2022-12-09 07:31:30.000000 tbats-1.1.2/tbats.egg-info/dependency_links.txt
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)       63 2022-12-09 07:31:30.000000 tbats-1.1.2/tbats.egg-info/requires.txt
--rw-r--r--   0 grzegorzskorupa   (502) staff       (20)        6 2022-12-09 07:31:30.000000 tbats-1.1.2/tbats.egg-info/top_level.txt
+drwxr-xr-x   0 grzegorzskorupa   (502) staff       (20)        0 2023-04-17 10:19:05.137339 tbats-1.1.3/
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)       46 2023-04-17 06:58:23.000000 tbats-1.1.3/AUTHORS.txt
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     1075 2023-04-17 06:58:23.000000 tbats-1.1.3/LICENSE
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     3613 2023-04-17 10:19:05.136987 tbats-1.1.3/PKG-INFO
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     3105 2023-04-17 06:58:23.000000 tbats-1.1.3/README.md
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)       38 2023-04-17 10:19:05.137391 tbats-1.1.3/setup.cfg
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     2199 2023-04-17 06:58:23.000000 tbats-1.1.3/setup.py
+drwxr-xr-x   0 grzegorzskorupa   (502) staff       (20)        0 2023-04-17 10:19:05.083524 tbats-1.1.3/tbats/
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      239 2023-04-17 10:03:47.000000 tbats-1.1.3/tbats/__init__.py
+drwxr-xr-x   0 grzegorzskorupa   (502) staff       (20)        0 2023-04-17 10:19:05.103259 tbats-1.1.3/tbats/abstract/
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      799 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/abstract/ArrayHelper.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     2983 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/abstract/Case.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     2178 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/abstract/ComponentMatrix.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     6200 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/abstract/Components.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      795 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/abstract/Context.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     1360 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/abstract/ContextInterface.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)    10794 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/abstract/Estimator.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     4140 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/abstract/MatrixBuilder.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      971 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/abstract/MatrixBuilderCache.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      307 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/abstract/MatrixBuilderInterface.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)    12493 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/abstract/Model.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)    10935 2023-04-17 09:56:51.000000 tbats-1.1.3/tbats/abstract/ModelParams.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     6693 2023-04-17 09:56:05.000000 tbats-1.1.3/tbats/abstract/ParamsOptimizer.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     1150 2023-04-17 09:59:31.000000 tbats-1.1.3/tbats/abstract/SeedFinder.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      798 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/abstract/__init__.py
+drwxr-xr-x   0 grzegorzskorupa   (502) staff       (20)        0 2023-04-17 10:19:05.112402 tbats-1.1.3/tbats/bats/
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     3919 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/bats/BATS.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      781 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/bats/Case.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     1376 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/bats/Components.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     1303 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/bats/Context.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     1857 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/bats/MatrixBuilder.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      136 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/bats/Model.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     2781 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/bats/ModelParams.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      170 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/bats/ParamsOptimizer.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     4181 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/bats/SeedFinder.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      431 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/bats/__init__.py
+drwxr-xr-x   0 grzegorzskorupa   (502) staff       (20)        0 2023-04-17 10:19:05.118045 tbats-1.1.3/tbats/error/
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)       41 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/error/BatsException.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)       41 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/error/BatsWarning.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      569 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/error/ExceptionHandler.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)       80 2023-04-17 10:00:13.000000 tbats-1.1.3/tbats/error/InputArgsException.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)       74 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/error/InputArgsWarning.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)       70 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/error/ModelWarning.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      384 2023-04-17 09:59:49.000000 tbats-1.1.3/tbats/error/__init__.py
+drwxr-xr-x   0 grzegorzskorupa   (502) staff       (20)        0 2023-04-17 10:19:05.130092 tbats-1.1.3/tbats/tbats/
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      568 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/tbats/Case.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     4314 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/tbats/Components.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     1429 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/tbats/Context.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)    10462 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/tbats/HarmonicsChoosingStrategy.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     2560 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/tbats/MatrixBuilder.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      136 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/tbats/Model.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     3197 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/tbats/ModelParams.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      170 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/tbats/ParamsOptimizer.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      832 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/tbats/SeedFinder.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     4966 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/tbats/TBATS.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      528 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/tbats/__init__.py
+drwxr-xr-x   0 grzegorzskorupa   (502) staff       (20)        0 2023-04-17 10:19:05.136723 tbats-1.1.3/tbats/transformation/
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     1625 2023-04-17 07:23:07.000000 tbats-1.1.3/tbats/transformation/BoxCox.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     2277 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/transformation/Guerrero.py
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)      162 2023-04-17 06:58:23.000000 tbats-1.1.3/tbats/transformation/__init__.py
+drwxr-xr-x   0 grzegorzskorupa   (502) staff       (20)        0 2023-04-17 10:19:05.086245 tbats-1.1.3/tbats.egg-info/
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     3613 2023-04-17 10:19:04.000000 tbats-1.1.3/tbats.egg-info/PKG-INFO
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)     1488 2023-04-17 10:19:04.000000 tbats-1.1.3/tbats.egg-info/SOURCES.txt
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)        1 2023-04-17 10:19:04.000000 tbats-1.1.3/tbats.egg-info/dependency_links.txt
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)       63 2023-04-17 10:19:04.000000 tbats-1.1.3/tbats.egg-info/requires.txt
+-rw-r--r--   0 grzegorzskorupa   (502) staff       (20)        6 2023-04-17 10:19:04.000000 tbats-1.1.3/tbats.egg-info/top_level.txt
```

### Comparing `tbats-1.1.2/LICENSE` & `tbats-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/PKG-INFO` & `tbats-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tbats
-Version: 1.1.2
+Version: 1.1.3
 Summary: BATS and TBATS for time series forecasting
 Home-page: https://github.com/intive-DataScience/tbats
 Author: Grzegorz Skorupa (intive)
 Author-email: grzegorz.skorupa@intive.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tbats-1.1.2/README.md` & `tbats-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/setup.py` & `tbats-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/abstract/ArrayHelper.py` & `tbats-1.1.3/tbats/abstract/ArrayHelper.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/abstract/Case.py` & `tbats-1.1.3/tbats/abstract/Case.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/abstract/ComponentMatrix.py` & `tbats-1.1.3/tbats/abstract/ComponentMatrix.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/abstract/Components.py` & `tbats-1.1.3/tbats/abstract/Components.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/abstract/Context.py` & `tbats-1.1.3/tbats/abstract/Context.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/abstract/ContextInterface.py` & `tbats-1.1.3/tbats/abstract/ContextInterface.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/abstract/Estimator.py` & `tbats-1.1.3/tbats/abstract/Estimator.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/abstract/MatrixBuilder.py` & `tbats-1.1.3/tbats/abstract/MatrixBuilder.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/abstract/MatrixBuilderCache.py` & `tbats-1.1.3/tbats/abstract/MatrixBuilderCache.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/abstract/Model.py` & `tbats-1.1.3/tbats/abstract/Model.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/abstract/ModelParams.py` & `tbats-1.1.3/tbats/abstract/ModelParams.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/abstract/ParamsOptimizer.py` & `tbats-1.1.3/tbats/abstract/ParamsOptimizer.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/abstract/__init__.py` & `tbats-1.1.3/tbats/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/bats/BATS.py` & `tbats-1.1.3/tbats/bats/BATS.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/bats/Case.py` & `tbats-1.1.3/tbats/bats/Case.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/bats/Components.py` & `tbats-1.1.3/tbats/bats/Components.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/bats/Context.py` & `tbats-1.1.3/tbats/bats/Context.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/bats/MatrixBuilder.py` & `tbats-1.1.3/tbats/bats/MatrixBuilder.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/bats/ModelParams.py` & `tbats-1.1.3/tbats/bats/ModelParams.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/bats/SeedFinder.py` & `tbats-1.1.3/tbats/bats/SeedFinder.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/error/ExceptionHandler.py` & `tbats-1.1.3/tbats/error/ExceptionHandler.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/tbats/Case.py` & `tbats-1.1.3/tbats/tbats/Case.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/tbats/Components.py` & `tbats-1.1.3/tbats/tbats/Components.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/tbats/Context.py` & `tbats-1.1.3/tbats/tbats/Context.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/tbats/HarmonicsChoosingStrategy.py` & `tbats-1.1.3/tbats/tbats/HarmonicsChoosingStrategy.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/tbats/MatrixBuilder.py` & `tbats-1.1.3/tbats/tbats/MatrixBuilder.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/tbats/ModelParams.py` & `tbats-1.1.3/tbats/tbats/ModelParams.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/tbats/SeedFinder.py` & `tbats-1.1.3/tbats/tbats/SeedFinder.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/tbats/TBATS.py` & `tbats-1.1.3/tbats/tbats/TBATS.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/tbats/__init__.py` & `tbats-1.1.3/tbats/tbats/__init__.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats/transformation/BoxCox.py` & `tbats-1.1.3/tbats/transformation/BoxCox.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 
 
 def boxcox(y, lam=None, seasonal_periods=None, bounds=(-1, 2)):
     y = c1d(check_array(y, ensure_2d=False, force_all_finite=True, ensure_min_samples=1,
                         copy=False, dtype=np.float64))  # type: np.ndarray
     if lam is None:
         lam = find_box_cox_lambda(y, seasonal_periods=seasonal_periods, bounds=bounds)
-    if lam <= 0 and np.any(y <= 0):
+    if (lam <= 0 or np.isclose(lam, 0)) and np.any(y <= 0):
         raise error.InputArgsException('y must have only positive values for box-cox transformation.')
     if np.isclose(0.0, lam):
         return np.log(y)
     return (np.sign(y) * (np.abs(y) ** lam) - 1) / lam
 
 
 def inv_boxcox(y, lam, force_valid=False):
     y = c1d(check_array(y, ensure_2d=False, force_all_finite=True, ensure_min_samples=1,
                         copy=False, dtype=np.float64))  # type: np.ndarray
+    if np.isclose(0.0, lam):
+        return np.exp(y)
     if lam < 0 and force_valid:
         y[y > -1 / lam] = -1 / lam
     if lam < 0 and np.any(y > -1 / lam):
         raise error.InputArgsException('Not possible to transform back such y values.')
-    if np.isclose(0.0, lam):
-        return np.exp(y)
     yy = y * lam + 1
     return np.sign(yy) * (np.abs(yy) ** (1 / lam))
```

### Comparing `tbats-1.1.2/tbats/transformation/Guerrero.py` & `tbats-1.1.3/tbats/transformation/Guerrero.py`

 * *Files identical despite different names*

### Comparing `tbats-1.1.2/tbats.egg-info/PKG-INFO` & `tbats-1.1.3/tbats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tbats
-Version: 1.1.2
+Version: 1.1.3
 Summary: BATS and TBATS for time series forecasting
 Home-page: https://github.com/intive-DataScience/tbats
 Author: Grzegorz Skorupa (intive)
 Author-email: grzegorz.skorupa@intive.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tbats-1.1.2/tbats.egg-info/SOURCES.txt` & `tbats-1.1.3/tbats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

