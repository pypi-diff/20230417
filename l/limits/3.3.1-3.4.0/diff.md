# Comparing `tmp/limits-3.3.1.tar.gz` & `tmp/limits-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limits-3.3.1.tar", last modified: Wed Mar 22 22:15:44 2023, max compression
+gzip compressed data, was "limits-3.4.0.tar", last modified: Mon Apr 17 13:05:59 2023, max compression
```

## Comparing `limits-3.3.1.tar` & `limits-3.4.0.tar`

### file list

```diff
@@ -1,98 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:15:44.027770 limits-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-22 22:15:34.000000 limits-3.3.1/CLASSIFIERS
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-22 22:15:34.000000 limits-3.3.1/CONTRIBUTIONS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-03-22 22:15:34.000000 limits-3.3.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-22 22:15:34.000000 limits-3.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-22 22:15:34.000000 limits-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-03-22 22:15:44.027770 limits-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-03-22 22:15:34.000000 limits-3.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:15:44.019770 limits-3.3.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-03-22 22:15:34.000000 limits-3.3.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:15:44.019770 limits-3.3.1/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:15:44.019770 limits-3.3.1/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-22 22:15:34.000000 limits-3.3.1/doc/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-03-22 22:15:34.000000 limits-3.3.1/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-03-22 22:15:34.000000 limits-3.3.1/doc/source/async.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-22 22:15:34.000000 limits-3.3.1/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-03-22 22:15:34.000000 limits-3.3.1/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-03-22 22:15:34.000000 limits-3.3.1/doc/source/custom-storage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-03-22 22:15:34.000000 limits-3.3.1/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-03-22 22:15:34.000000 limits-3.3.1/doc/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-03-22 22:15:34.000000 limits-3.3.1/doc/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-03-22 22:15:34.000000 limits-3.3.1/doc/source/storage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-22 22:15:34.000000 limits-3.3.1/doc/source/strategies.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-22 22:15:34.000000 limits-3.3.1/doc/source/theme_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:15:44.027770 limits-3.3.1/limits/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-22 22:15:34.000000 limits-3.3.1/limits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-22 22:15:44.027770 limits-3.3.1/limits/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:15:44.023770 limits-3.3.1/limits/aio/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-22 22:15:34.000000 limits-3.3.1/limits/aio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:15:44.023770 limits-3.3.1/limits/aio/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-22 22:15:34.000000 limits-3.3.1/limits/aio/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-03-22 22:15:34.000000 limits-3.3.1/limits/aio/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-03-22 22:15:34.000000 limits-3.3.1/limits/aio/storage/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-03-22 22:15:34.000000 limits-3.3.1/limits/aio/storage/memcached.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-03-22 22:15:34.000000 limits-3.3.1/limits/aio/storage/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-03-22 22:15:34.000000 limits-3.3.1/limits/aio/storage/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-03-22 22:15:34.000000 limits-3.3.1/limits/aio/storage/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-03-22 22:15:34.000000 limits-3.3.1/limits/aio/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-22 22:15:34.000000 limits-3.3.1/limits/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-03-22 22:15:34.000000 limits-3.3.1/limits/limits.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 22:15:34.000000 limits-3.3.1/limits/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:15:44.019770 limits-3.3.1/limits/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:15:44.019770 limits-3.3.1/limits/resources/redis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:15:44.023770 limits-3.3.1/limits/resources/redis/lua_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-22 22:15:34.000000 limits-3.3.1/limits/resources/redis/lua_scripts/acquire_moving_window.lua
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-22 22:15:34.000000 limits-3.3.1/limits/resources/redis/lua_scripts/clear_keys.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-03-22 22:15:34.000000 limits-3.3.1/limits/resources/redis/lua_scripts/gcra_consume.lua
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-22 22:15:34.000000 limits-3.3.1/limits/resources/redis/lua_scripts/incr_expire.lua
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-22 22:15:34.000000 limits-3.3.1/limits/resources/redis/lua_scripts/moving_window.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:15:44.023770 limits-3.3.1/limits/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-03-22 22:15:34.000000 limits-3.3.1/limits/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-03-22 22:15:34.000000 limits-3.3.1/limits/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-03-22 22:15:34.000000 limits-3.3.1/limits/storage/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-03-22 22:15:34.000000 limits-3.3.1/limits/storage/memcached.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-03-22 22:15:34.000000 limits-3.3.1/limits/storage/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-03-22 22:15:34.000000 limits-3.3.1/limits/storage/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-03-22 22:15:34.000000 limits-3.3.1/limits/storage/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-03-22 22:15:34.000000 limits-3.3.1/limits/storage/redis_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-03-22 22:15:34.000000 limits-3.3.1/limits/storage/redis_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-22 22:15:34.000000 limits-3.3.1/limits/storage/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-03-22 22:15:34.000000 limits-3.3.1/limits/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-03-22 22:15:34.000000 limits-3.3.1/limits/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-03-22 22:15:34.000000 limits-3.3.1/limits/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-22 22:15:34.000000 limits-3.3.1/limits/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:15:44.023770 limits-3.3.1/limits.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-03-22 22:15:44.000000 limits-3.3.1/limits.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-22 22:15:44.000000 limits-3.3.1/limits.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 22:15:44.000000 limits-3.3.1/limits.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 22:15:43.000000 limits-3.3.1/limits.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-22 22:15:44.000000 limits-3.3.1/limits.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-22 22:15:44.000000 limits-3.3.1/limits.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-22 22:15:34.000000 limits-3.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:15:44.027770 limits-3.3.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-22 22:15:34.000000 limits-3.3.1/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-22 22:15:34.000000 limits-3.3.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-22 22:15:34.000000 limits-3.3.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-22 22:15:34.000000 limits-3.3.1/requirements/main.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:15:44.027770 limits-3.3.1/requirements/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-22 22:15:34.000000 limits-3.3.1/requirements/storage/async-etcd.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-22 22:15:34.000000 limits-3.3.1/requirements/storage/async-memcached.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-22 22:15:34.000000 limits-3.3.1/requirements/storage/async-mongodb.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-22 22:15:34.000000 limits-3.3.1/requirements/storage/async-redis.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-22 22:15:34.000000 limits-3.3.1/requirements/storage/etcd.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-22 22:15:34.000000 limits-3.3.1/requirements/storage/memcached.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-22 22:15:34.000000 limits-3.3.1/requirements/storage/mongodb.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-22 22:15:34.000000 limits-3.3.1/requirements/storage/redis.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-22 22:15:34.000000 limits-3.3.1/requirements/storage/rediscluster.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-22 22:15:34.000000 limits-3.3.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-22 22:15:44.027770 limits-3.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1925 2023-03-22 22:15:34.000000 limits-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:15:44.027770 limits-3.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-03-22 22:15:34.000000 limits-3.3.1/tests/test_limit_granularities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-03-22 22:15:34.000000 limits-3.3.1/tests/test_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-03-22 22:15:34.000000 limits-3.3.1/tests/test_ratelimit_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-03-22 22:15:34.000000 limits-3.3.1/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-03-22 22:15:34.000000 limits-3.3.1/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-22 22:15:34.000000 limits-3.3.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-03-22 22:15:34.000000 limits-3.3.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.036538 limits-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-17 13:05:49.000000 limits-3.4.0/CLASSIFIERS
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-17 13:05:49.000000 limits-3.4.0/CONTRIBUTIONS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-04-17 13:05:49.000000 limits-3.4.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-17 13:05:49.000000 limits-3.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-17 13:05:49.000000 limits-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-04-17 13:05:59.036538 limits-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-04-17 13:05:49.000000 limits-3.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.024538 limits-3.4.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-04-17 13:05:49.000000 limits-3.4.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.028538 limits-3.4.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.028538 limits-3.4.0/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/async.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/custom-storage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/storage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/strategies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-17 13:05:49.000000 limits-3.4.0/doc/source/theme_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.040538 limits-3.4.0/limits/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-17 13:05:49.000000 limits-3.4.0/limits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-17 13:05:59.040538 limits-3.4.0/limits/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.028538 limits-3.4.0/limits/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.032538 limits-3.4.0/limits/aio/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/storage/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/storage/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/storage/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/storage/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/storage/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-17 13:05:49.000000 limits-3.4.0/limits/aio/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-17 13:05:49.000000 limits-3.4.0/limits/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-17 13:05:49.000000 limits-3.4.0/limits/limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:49.000000 limits-3.4.0/limits/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.024538 limits-3.4.0/limits/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.024538 limits-3.4.0/limits/resources/redis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.032538 limits-3.4.0/limits/resources/redis/lua_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-17 13:05:49.000000 limits-3.4.0/limits/resources/redis/lua_scripts/acquire_moving_window.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-17 13:05:49.000000 limits-3.4.0/limits/resources/redis/lua_scripts/clear_keys.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-17 13:05:49.000000 limits-3.4.0/limits/resources/redis/lua_scripts/incr_expire.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-17 13:05:49.000000 limits-3.4.0/limits/resources/redis/lua_scripts/moving_window.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.032538 limits-3.4.0/limits/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/redis_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/redis_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-17 13:05:49.000000 limits-3.4.0/limits/storage/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-17 13:05:49.000000 limits-3.4.0/limits/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-17 13:05:49.000000 limits-3.4.0/limits/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-17 13:05:49.000000 limits-3.4.0/limits/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-17 13:05:49.000000 limits-3.4.0/limits/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.028538 limits-3.4.0/limits.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-04-17 13:05:59.000000 limits-3.4.0/limits.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-17 13:05:59.000000 limits-3.4.0/limits.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:05:59.000000 limits-3.4.0/limits.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:05:58.000000 limits-3.4.0/limits.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-17 13:05:59.000000 limits-3.4.0/limits.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 13:05:59.000000 limits-3.4.0/limits.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 13:05:49.000000 limits-3.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.036538 limits-3.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/main.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.036538 limits-3.4.0/requirements/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/async-etcd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/async-memcached.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/async-mongodb.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/async-redis.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/etcd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/memcached.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/mongodb.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/redis.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/storage/rediscluster.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-17 13:05:49.000000 limits-3.4.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-17 13:05:59.040538 limits-3.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1925 2023-04-17 13:05:49.000000 limits-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:05:59.036538 limits-3.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-17 13:05:49.000000 limits-3.4.0/tests/test_limit_granularities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-17 13:05:49.000000 limits-3.4.0/tests/test_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-17 13:05:49.000000 limits-3.4.0/tests/test_ratelimit_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-04-17 13:05:49.000000 limits-3.4.0/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-17 13:05:49.000000 limits-3.4.0/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-17 13:05:49.000000 limits-3.4.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-17 13:05:49.000000 limits-3.4.0/versioneer.py
```

### Comparing `limits-3.3.1/CLASSIFIERS` & `limits-3.4.0/CLASSIFIERS`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/HISTORY.rst` & `limits-3.4.0/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 .. :changelog:
 
 Changelog
 =========
 
+v3.4.0
+------
+Release Date: 2023-04-17
+
+* Bug Fix
+
+  * Remove use of weakreferences to storages in strategy
+    classes as this was not documented or required and
+    led to usability issues.
+
+* Chores
+
+  * Update documentation dependencies
+  * Remove unused gcra lua script
+
 v3.3.1
 ------
 Release Date: 2023-03-22
 
 * Compatibility
 
   * Block incompatible versions of redis-py
@@ -530,14 +545,15 @@
 
 
 
 
 
 
 
+
```

### Comparing `limits-3.3.1/LICENSE.txt` & `limits-3.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/PKG-INFO` & `limits-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limits
-Version: 3.3.1
+Version: 3.4.0
 Summary: Rate limiting utilities
 Home-page: https://limits.readthedocs.org
 Author: Ali-Akber Saifee
 Author-email: ali@indydevs.org
 License: MIT
 Project-URL: Source, https://github.com/alisaifee/limits
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `limits-3.3.1/README.rst` & `limits-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/doc/Makefile` & `limits-3.4.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/doc/source/api.rst` & `limits-3.4.0/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/doc/source/async.rst` & `limits-3.4.0/doc/source/async.rst`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/doc/source/conf.py` & `limits-3.4.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/doc/source/custom-storage.rst` & `limits-3.4.0/doc/source/custom-storage.rst`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/doc/source/index.rst` & `limits-3.4.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/doc/source/installation.rst` & `limits-3.4.0/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/doc/source/quickstart.rst` & `limits-3.4.0/doc/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/doc/source/storage.rst` & `limits-3.4.0/doc/source/storage.rst`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/doc/source/strategies.rst` & `limits-3.4.0/doc/source/strategies.rst`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/doc/source/theme_config.py` & `limits-3.4.0/doc/source/theme_config.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/__init__.py` & `limits-3.4.0/limits/__init__.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/aio/storage/__init__.py` & `limits-3.4.0/limits/aio/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/aio/storage/base.py` & `limits-3.4.0/limits/aio/storage/base.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/aio/storage/etcd.py` & `limits-3.4.0/limits/aio/storage/etcd.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/aio/storage/memcached.py` & `limits-3.4.0/limits/aio/storage/memcached.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/aio/storage/memory.py` & `limits-3.4.0/limits/aio/storage/memory.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/aio/storage/mongodb.py` & `limits-3.4.0/limits/aio/storage/mongodb.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/aio/storage/redis.py` & `limits-3.4.0/limits/aio/storage/redis.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/aio/strategies.py` & `limits-3.4.0/limits/aio/strategies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
 Asynchronous rate limiting strategies
 """
 
-import weakref
 from abc import ABC, abstractmethod
 from typing import cast
 
 from ..limits import RateLimitItem
 from ..storage import StorageTypes
 from ..util import WindowStats
 from .storage import MovingWindowSupport, Storage
 
 
 class RateLimiter(ABC):
     def __init__(self, storage: StorageTypes):
         assert isinstance(storage, Storage)
-        self.storage: Storage = weakref.proxy(storage)
+        self.storage: Storage = storage
 
     @abstractmethod
     async def hit(self, item: RateLimitItem, *identifiers: str, cost: int = 1) -> bool:
         """
         Consume the rate limit
 
         :param item: the rate limit item
```

### Comparing `limits-3.3.1/limits/limits.py` & `limits-3.4.0/limits/limits.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/resources/redis/lua_scripts/acquire_moving_window.lua` & `limits-3.4.0/limits/resources/redis/lua_scripts/acquire_moving_window.lua`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/storage/__init__.py` & `limits-3.4.0/limits/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/storage/base.py` & `limits-3.4.0/limits/storage/base.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/storage/etcd.py` & `limits-3.4.0/limits/storage/etcd.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/storage/memcached.py` & `limits-3.4.0/limits/storage/memcached.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/storage/memory.py` & `limits-3.4.0/limits/storage/memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections import Counter
 
 import limits.typing
 from limits.storage.base import MovingWindowSupport, Storage
 from limits.typing import Dict, List, Optional, Tuple
 
 
-class LockableEntry(threading._RLock):
+class LockableEntry(threading._RLock):  # type: ignore
     def __init__(self, expiry: float) -> None:
         self.atime = time.time()
         self.expiry = self.atime + expiry
         super().__init__()
 
 
 class MemoryStorage(Storage, MovingWindowSupport):
```

### Comparing `limits-3.3.1/limits/storage/mongodb.py` & `limits-3.4.0/limits/storage/mongodb.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/storage/redis.py` & `limits-3.4.0/limits/storage/redis.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/storage/redis_cluster.py` & `limits-3.4.0/limits/storage/redis_cluster.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/storage/redis_sentinel.py` & `limits-3.4.0/limits/storage/redis_sentinel.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/storage/registry.py` & `limits-3.4.0/limits/storage/registry.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/strategies.py` & `limits-3.4.0/limits/strategies.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """
 Rate limiting strategies
 """
 
-import weakref
 from abc import ABCMeta, abstractmethod
 from typing import Dict, Type, Union, cast
 
 from .limits import RateLimitItem
 from .storage import MovingWindowSupport, Storage, StorageTypes
 from .util import WindowStats
 
 
 class RateLimiter(metaclass=ABCMeta):
     def __init__(self, storage: StorageTypes):
         assert isinstance(storage, Storage)
-        self.storage: Storage = weakref.proxy(storage)
+        self.storage: Storage = storage
 
     @abstractmethod
     def hit(self, item: RateLimitItem, *identifiers: str, cost: int = 1) -> bool:
         """
         Consume the rate limit
 
         :param item: The rate limit item
```

### Comparing `limits-3.3.1/limits/typing.py` & `limits-3.4.0/limits/typing.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits/util.py` & `limits-3.4.0/limits/util.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/limits.egg-info/PKG-INFO` & `limits-3.4.0/limits.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limits
-Version: 3.3.1
+Version: 3.4.0
 Summary: Rate limiting utilities
 Home-page: https://limits.readthedocs.org
 Author: Ali-Akber Saifee
 Author-email: ali@indydevs.org
 License: MIT
 Project-URL: Source, https://github.com/alisaifee/limits
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `limits-3.3.1/limits.egg-info/SOURCES.txt` & `limits-3.4.0/limits.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 limits/aio/storage/etcd.py
 limits/aio/storage/memcached.py
 limits/aio/storage/memory.py
 limits/aio/storage/mongodb.py
 limits/aio/storage/redis.py
 limits/resources/redis/lua_scripts/acquire_moving_window.lua
 limits/resources/redis/lua_scripts/clear_keys.lua
-limits/resources/redis/lua_scripts/gcra_consume.lua
 limits/resources/redis/lua_scripts/incr_expire.lua
 limits/resources/redis/lua_scripts/moving_window.lua
 limits/storage/__init__.py
 limits/storage/base.py
 limits/storage/etcd.py
 limits/storage/memcached.py
 limits/storage/memory.py
```

### Comparing `limits-3.3.1/limits.egg-info/requires.txt` & `limits-3.4.0/limits.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/setup.cfg` & `limits-3.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/setup.py` & `limits-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/tests/test_limit_granularities.py` & `limits-3.4.0/tests/test_limit_granularities.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/tests/test_limits.py` & `limits-3.4.0/tests/test_limits.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/tests/test_ratelimit_parser.py` & `limits-3.4.0/tests/test_ratelimit_parser.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/tests/test_storage.py` & `limits-3.4.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/tests/test_strategy.py` & `limits-3.4.0/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/tests/test_utils.py` & `limits-3.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `limits-3.3.1/versioneer.py` & `limits-3.4.0/versioneer.py`

 * *Files identical despite different names*

