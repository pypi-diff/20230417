# Comparing `tmp/mgo_serializer-0.1.4.tar.gz` & `tmp/mgo_serializer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgo_serializer-0.1.4.tar", last modified: Mon Apr 17 09:32:05 2023, max compression
+gzip compressed data, was "mgo_serializer-0.1.5.tar", last modified: Mon Apr 17 10:04:38 2023, max compression
```

## Comparing `mgo_serializer-0.1.4.tar` & `mgo_serializer-0.1.5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.951492 mgo_serializer-0.1.4/
--rw-r--r--   0 hydra     (1000) hydra     (1000)      392 2023-04-17 09:32:05.951492 mgo_serializer-0.1.4/PKG-INFO
--rwxrwxrwx   0 hydra     (1000) hydra     (1000)      146 2022-04-06 08:39:36.000000 mgo_serializer-0.1.4/README.md
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.948159 mgo_serializer-0.1.4/common/
--rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:10:32.000000 mgo_serializer-0.1.4/common/__init__.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.948159 mgo_serializer-0.1.4/common/api/
--rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/__init__.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.948159 mgo_serializer-0.1.4/common/api/services/
--rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/__init__.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.948159 mgo_serializer-0.1.4/common/api/services/account/
--rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/account/__init__.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)    32911 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/account/account_pb2.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)   114804 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/account/account_pb2_grpc.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.948159 mgo_serializer-0.1.4/common/api/services/common/
--rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/common/__init__.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     9632 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/common/common_pb2.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)      159 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/common/common_pb2_grpc.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.948159 mgo_serializer-0.1.4/common/api/services/discussion/
--rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/discussion/__init__.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     5389 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/discussion/discussion_pb2.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)    19113 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/discussion/discussion_pb2_grpc.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.948159 mgo_serializer-0.1.4/common/api/services/explore/
--rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/explore/__init__.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     3100 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/explore/explore_pb2.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     6027 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/explore/explore_pb2_grpc.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.948159 mgo_serializer-0.1.4/common/api/services/hashtag/
--rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/hashtag/__init__.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     6160 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/hashtag/hashtag_pb2.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)    14342 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/hashtag/hashtag_pb2_grpc.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.948159 mgo_serializer-0.1.4/common/api/services/history/
--rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/history/__init__.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     4696 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/history/history_pb2.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     5873 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/history/history_pb2_grpc.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.951492 mgo_serializer-0.1.4/common/api/services/mention/
--rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/mention/__init__.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     2302 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/mention/mention_pb2.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     6322 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/mention/mention_pb2_grpc.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.951492 mgo_serializer-0.1.4/common/api/services/post/
--rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/post/__init__.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)    11421 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/post/post_pb2.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)    39890 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/post/post_pb2_grpc.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.951492 mgo_serializer-0.1.4/common/api/services/product/
--rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/product/__init__.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)    32899 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/product/product_pb2.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)    86544 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/product/product_pb2_grpc.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.951492 mgo_serializer-0.1.4/common/api/services/shop/
--rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/shop/__init__.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)    45403 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/shop/shop_pb2.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)    74160 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/shop/shop_pb2_grpc.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.951492 mgo_serializer-0.1.4/common/api/services/stats/
--rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/stats/__init__.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     4291 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/stats/stats_pb2.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     9050 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/stats/stats_pb2_grpc.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.951492 mgo_serializer-0.1.4/common/api/services/story/
--rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/story/__init__.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     7304 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/story/story_pb2.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)    15700 2022-04-10 11:11:53.000000 mgo_serializer-0.1.4/common/api/services/story/story_pb2_grpc.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.951492 mgo_serializer-0.1.4/mgo_serializer/
--rwxrwxrwx   0 hydra     (1000) hydra     (1000)      104 2022-04-06 08:10:46.000000 mgo_serializer-0.1.4/mgo_serializer/__init__.py
--rwxrwxrwx   0 hydra     (1000) hydra     (1000)      671 2023-04-17 09:31:45.000000 mgo_serializer-0.1.4/mgo_serializer/exceptions.py
--rwxrwxrwx   0 hydra     (1000) hydra     (1000)    16480 2023-04-17 09:31:45.000000 mgo_serializer-0.1.4/mgo_serializer/fields.py
--rwxrwxrwx   0 hydra     (1000) hydra     (1000)     4894 2022-05-11 09:53:09.000000 mgo_serializer-0.1.4/mgo_serializer/helpers.py
--rwxrwxrwx   0 hydra     (1000) hydra     (1000)     1498 2022-04-06 08:02:56.000000 mgo_serializer-0.1.4/mgo_serializer/meta.py
--rwxrwxrwx   0 hydra     (1000) hydra     (1000)    14687 2023-04-16 10:02:43.000000 mgo_serializer-0.1.4/mgo_serializer/serializer.py
--rwxrwxrwx   0 hydra     (1000) hydra     (1000)      837 2022-04-06 08:02:56.000000 mgo_serializer-0.1.4/mgo_serializer/utils.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 09:32:05.951492 mgo_serializer-0.1.4/mgo_serializer.egg-info/
--rw-r--r--   0 hydra     (1000) hydra     (1000)      392 2023-04-17 09:32:05.000000 mgo_serializer-0.1.4/mgo_serializer.egg-info/PKG-INFO
--rw-r--r--   0 hydra     (1000) hydra     (1000)     1969 2023-04-17 09:32:05.000000 mgo_serializer-0.1.4/mgo_serializer.egg-info/SOURCES.txt
--rw-r--r--   0 hydra     (1000) hydra     (1000)        1 2023-04-17 09:32:05.000000 mgo_serializer-0.1.4/mgo_serializer.egg-info/dependency_links.txt
--rw-r--r--   0 hydra     (1000) hydra     (1000)       22 2023-04-17 09:32:05.000000 mgo_serializer-0.1.4/mgo_serializer.egg-info/top_level.txt
--rwxrwxrwx   0 hydra     (1000) hydra     (1000)       79 2023-04-17 09:32:05.951492 mgo_serializer-0.1.4/setup.cfg
--rwxrwxrwx   0 hydra     (1000) hydra     (1000)      528 2023-04-17 09:31:45.000000 mgo_serializer-0.1.4/setup.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.835198 mgo_serializer-0.1.5/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)      392 2023-04-17 10:04:38.835198 mgo_serializer-0.1.5/PKG-INFO
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)      146 2022-04-06 08:39:36.000000 mgo_serializer-0.1.5/README.md
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.831864 mgo_serializer-0.1.5/common/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:10:32.000000 mgo_serializer-0.1.5/common/__init__.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.831864 mgo_serializer-0.1.5/common/api/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/__init__.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.831864 mgo_serializer-0.1.5/common/api/services/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/__init__.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.831864 mgo_serializer-0.1.5/common/api/services/account/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/account/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    32911 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/account/account_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)   114804 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/account/account_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.831864 mgo_serializer-0.1.5/common/api/services/common/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/common/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     9632 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/common/common_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)      159 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/common/common_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.831864 mgo_serializer-0.1.5/common/api/services/discussion/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/discussion/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     5389 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/discussion/discussion_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    19113 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/discussion/discussion_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.831864 mgo_serializer-0.1.5/common/api/services/explore/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/explore/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     3100 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/explore/explore_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     6027 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/explore/explore_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.831864 mgo_serializer-0.1.5/common/api/services/hashtag/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/hashtag/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     6160 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/hashtag/hashtag_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    14342 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/hashtag/hashtag_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.831864 mgo_serializer-0.1.5/common/api/services/history/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/history/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     4696 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/history/history_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     5873 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/history/history_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.831864 mgo_serializer-0.1.5/common/api/services/mention/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/mention/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     2302 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/mention/mention_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     6322 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/mention/mention_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.831864 mgo_serializer-0.1.5/common/api/services/post/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/post/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    11421 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/post/post_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    39890 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/post/post_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.831864 mgo_serializer-0.1.5/common/api/services/product/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/product/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    32899 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/product/product_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    86544 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/product/product_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.831864 mgo_serializer-0.1.5/common/api/services/shop/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/shop/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    45403 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/shop/shop_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    74160 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/shop/shop_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.831864 mgo_serializer-0.1.5/common/api/services/stats/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/stats/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     4291 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/stats/stats_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     9050 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/stats/stats_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.831864 mgo_serializer-0.1.5/common/api/services/story/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/story/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     7304 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/story/story_pb2.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)    15700 2022-04-10 11:11:53.000000 mgo_serializer-0.1.5/common/api/services/story/story_pb2_grpc.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.835198 mgo_serializer-0.1.5/mgo_serializer/
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)      104 2022-04-06 08:10:46.000000 mgo_serializer-0.1.5/mgo_serializer/__init__.py
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)      671 2023-04-17 09:31:45.000000 mgo_serializer-0.1.5/mgo_serializer/exceptions.py
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)    16480 2023-04-17 09:31:45.000000 mgo_serializer-0.1.5/mgo_serializer/fields.py
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)     4894 2022-05-11 09:53:09.000000 mgo_serializer-0.1.5/mgo_serializer/helpers.py
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)     1498 2022-04-06 08:02:56.000000 mgo_serializer-0.1.5/mgo_serializer/meta.py
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)    14792 2023-04-17 10:03:46.000000 mgo_serializer-0.1.5/mgo_serializer/serializer.py
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)      837 2022-04-06 08:02:56.000000 mgo_serializer-0.1.5/mgo_serializer/utils.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-17 10:04:38.835198 mgo_serializer-0.1.5/mgo_serializer.egg-info/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)      392 2023-04-17 10:04:38.000000 mgo_serializer-0.1.5/mgo_serializer.egg-info/PKG-INFO
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     1969 2023-04-17 10:04:38.000000 mgo_serializer-0.1.5/mgo_serializer.egg-info/SOURCES.txt
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        1 2023-04-17 10:04:38.000000 mgo_serializer-0.1.5/mgo_serializer.egg-info/dependency_links.txt
+-rw-r--r--   0 hydra     (1000) hydra     (1000)       22 2023-04-17 10:04:38.000000 mgo_serializer-0.1.5/mgo_serializer.egg-info/top_level.txt
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)       79 2023-04-17 10:04:38.835198 mgo_serializer-0.1.5/setup.cfg
+-rwxrwxrwx   0 hydra     (1000) hydra     (1000)      528 2023-04-17 10:04:31.000000 mgo_serializer-0.1.5/setup.py
```

### Comparing `mgo_serializer-0.1.4/common/api/services/account/account_pb2.py` & `mgo_serializer-0.1.5/common/api/services/account/account_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/account/account_pb2_grpc.py` & `mgo_serializer-0.1.5/common/api/services/account/account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/common/common_pb2.py` & `mgo_serializer-0.1.5/common/api/services/common/common_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/discussion/discussion_pb2.py` & `mgo_serializer-0.1.5/common/api/services/discussion/discussion_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/discussion/discussion_pb2_grpc.py` & `mgo_serializer-0.1.5/common/api/services/discussion/discussion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/explore/explore_pb2.py` & `mgo_serializer-0.1.5/common/api/services/explore/explore_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/explore/explore_pb2_grpc.py` & `mgo_serializer-0.1.5/common/api/services/explore/explore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/hashtag/hashtag_pb2.py` & `mgo_serializer-0.1.5/common/api/services/hashtag/hashtag_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/hashtag/hashtag_pb2_grpc.py` & `mgo_serializer-0.1.5/common/api/services/hashtag/hashtag_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/history/history_pb2.py` & `mgo_serializer-0.1.5/common/api/services/history/history_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/history/history_pb2_grpc.py` & `mgo_serializer-0.1.5/common/api/services/history/history_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/mention/mention_pb2.py` & `mgo_serializer-0.1.5/common/api/services/mention/mention_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/mention/mention_pb2_grpc.py` & `mgo_serializer-0.1.5/common/api/services/mention/mention_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/post/post_pb2.py` & `mgo_serializer-0.1.5/common/api/services/post/post_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/post/post_pb2_grpc.py` & `mgo_serializer-0.1.5/common/api/services/post/post_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/product/product_pb2.py` & `mgo_serializer-0.1.5/common/api/services/product/product_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/product/product_pb2_grpc.py` & `mgo_serializer-0.1.5/common/api/services/product/product_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/shop/shop_pb2.py` & `mgo_serializer-0.1.5/common/api/services/shop/shop_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/shop/shop_pb2_grpc.py` & `mgo_serializer-0.1.5/common/api/services/shop/shop_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/stats/stats_pb2.py` & `mgo_serializer-0.1.5/common/api/services/stats/stats_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/stats/stats_pb2_grpc.py` & `mgo_serializer-0.1.5/common/api/services/stats/stats_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/story/story_pb2.py` & `mgo_serializer-0.1.5/common/api/services/story/story_pb2.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/common/api/services/story/story_pb2_grpc.py` & `mgo_serializer-0.1.5/common/api/services/story/story_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/mgo_serializer/exceptions.py` & `mgo_serializer-0.1.5/mgo_serializer/exceptions.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/mgo_serializer/fields.py` & `mgo_serializer-0.1.5/mgo_serializer/fields.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/mgo_serializer/helpers.py` & `mgo_serializer-0.1.5/mgo_serializer/helpers.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/mgo_serializer/meta.py` & `mgo_serializer-0.1.5/mgo_serializer/meta.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/mgo_serializer/serializer.py` & `mgo_serializer-0.1.5/mgo_serializer/serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 import re
+from abc import ABC
 from functools import cached_property
 
 from google.protobuf.json_format import ParseDict, MessageToDict  # noqa
 from google.protobuf.message import Message  # noqa
 
 from mgo_serializer.exceptions import ValidationError
 from mgo_serializer.fields import BaseField, Empty, set_value
@@ -219,18 +220,18 @@
         return self._errors
 
     @property
     def validated_data(self):
         if hasattr(self, 'initial_data') and not hasattr(self, '_validated_data'):
             msg = 'You must call `.is_valid()` before accessing `.validated_data`.'
             raise AssertionError(msg)
-        return self._validated_data
+        return self._validated_data if hasattr(self, '_validated_data') else self.parent.instance[self.field_name]
 
 
-class ListSerializer(BaseSerializer):
+class ListSerializer(BaseSerializer, ABC):
     """
     Serializer for list of objects.
     """
 
     child = None
     many = True
```

### Comparing `mgo_serializer-0.1.4/mgo_serializer/utils.py` & `mgo_serializer-0.1.5/mgo_serializer/utils.py`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/mgo_serializer.egg-info/SOURCES.txt` & `mgo_serializer-0.1.5/mgo_serializer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mgo_serializer-0.1.4/setup.py` & `mgo_serializer-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="mgo_serializer",
-    version="0.1.4",
+    version="0.1.5",
     author='MosyDev',
     author_email='mostafa.uwsgi@gmail.com',
     description='A MongoEngine Serializer to serialize objects from JSON/BSON to JSON and gRPC',
     url='https://github.com/its0x4d/mgo_serializer',
     packages=setuptools.find_packages(),
     license='GPLv3',
     classifiers=[
```

