# Comparing `tmp/blaster-server-0.0.425.tar.gz` & `tmp/blaster-server-0.0.425b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaster-server-0.0.425.tar", last modified: Sun Apr 16 18:16:05 2023, max compression
+gzip compressed data, was "blaster-server-0.0.425b0.tar", last modified: Sun Apr 16 21:13:49 2023, max compression
```

## Comparing `blaster-server-0.0.425.tar` & `blaster-server-0.0.425b0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.846692 blaster-server-0.0.425/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1061 2019-07-03 19:03:00.000000 blaster-server-0.0.425/LICENSE.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2022-11-07 18:47:07.000000 blaster-server-0.0.425/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-04-16 18:16:05.846692 blaster-server-0.0.425/PKG-INFO
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2620 2022-11-14 12:45:11.000000 blaster-server-0.0.425/README.md
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2021-10-05 11:27:02.000000 blaster-server-0.0.425/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/blaster/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      875 2023-01-09 13:10:46.000000 blaster-server-0.0.425/blaster/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/blaster/cloud/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2022-11-09 17:29:08.000000 blaster-server-0.0.425/blaster/cloud/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3257 2022-12-03 12:42:35.000000 blaster-server-0.0.425/blaster/cloud/analytics.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/blaster/cloud/aws/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       78 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/cloud/aws/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2022-12-01 11:30:06.000000 blaster-server-0.0.425/blaster/cloud/aws/ses_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5230 2023-01-28 12:53:32.000000 blaster-server-0.0.425/blaster/cloud/push_tasks.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3729 2023-03-23 02:32:10.000000 blaster-server-0.0.425/blaster/cloud/storage.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3796 2023-03-06 12:38:58.000000 blaster-server-0.0.425/blaster/config.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-01-28 12:57:17.000000 blaster-server-0.0.425/blaster/connection_pool.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       99 2020-11-22 14:37:38.000000 blaster-server-0.0.425/blaster/constants.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5290 2023-03-30 07:56:48.000000 blaster-server-0.0.425/blaster/logging.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62615 2023-04-15 22:13:28.000000 blaster-server-0.0.425/blaster/mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    14954 2023-03-22 22:32:18.000000 blaster-server-0.0.425/blaster/schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    36521 2023-04-03 11:05:37.000000 blaster-server-0.0.425/blaster/server.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46829 2023-04-03 00:57:53.000000 blaster-server-0.0.425/blaster/tools.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/blaster/utils/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/utils/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/blaster/utils/data/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2022-11-08 15:22:07.000000 blaster-server-0.0.425/blaster/utils/data/countries.json
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2022-12-01 10:20:50.000000 blaster-server-0.0.425/blaster/utils/data/mime_types.json
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7087 2023-04-16 18:10:42.000000 blaster-server-0.0.425/blaster/utils/data_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-01-07 12:42:21.000000 blaster-server-0.0.425/blaster/utils/events.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-03-30 16:36:26.000000 blaster-server-0.0.425/blaster/utils/fork.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1076 2023-02-21 07:52:48.000000 blaster-server-0.0.425/blaster/utils/lat_long_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5552 2023-02-01 17:01:50.000000 blaster-server-0.0.425/blaster/utils/phone_number_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     6773 2020-12-14 07:56:42.000000 blaster-server-0.0.425/blaster/utils/xss_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/blaster/websocket/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1022 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/__init__.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12874 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_abnf.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2022-01-06 11:42:20.000000 blaster-server-0.0.425/blaster/websocket/_app.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    16360 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_core.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2141 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_exceptions.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     4793 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_handshake.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7288 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_http.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1870 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_logging.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3623 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_socket.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1550 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_ssl_compat.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3670 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_url.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3632 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12758 2021-10-03 12:23:56.000000 blaster-server-0.0.425/blaster/websocket/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/blaster/websocket/tests/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/tests/__init__.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    26115 2019-07-03 19:03:00.000000 blaster-server-0.0.425/blaster/websocket/tests/test_websocket.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/blaster_server.egg-info/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      849 2023-04-16 18:16:05.000000 blaster-server-0.0.425/blaster_server.egg-info/PKG-INFO
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1682 2023-04-16 18:16:05.000000 blaster-server-0.0.425/blaster_server.egg-info/SOURCES.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        1 2023-04-16 18:16:05.000000 blaster-server-0.0.425/blaster_server.egg-info/dependency_links.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      221 2023-04-16 18:16:05.000000 blaster-server-0.0.425/blaster_server.egg-info/requires.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       41 2023-04-16 18:16:05.000000 blaster-server-0.0.425/blaster_server.egg-info/top_level.txt
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.842692 blaster-server-0.0.425/examples/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.425/examples/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2022-01-06 11:42:20.000000 blaster-server-0.0.425/examples/fast_api_test.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      636 2019-07-03 19:03:00.000000 blaster-server-0.0.425/examples/gevent_wsgi_test.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      233 2021-10-04 14:48:01.000000 blaster-server-0.0.425/examples/meinheld_flask.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1743 2022-06-17 17:10:40.000000 blaster-server-0.0.425/examples/mongo_ormexample.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2022-11-14 12:13:43.000000 blaster-server-0.0.425/examples/simple_examples.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1088 2019-07-03 19:03:00.000000 blaster-server-0.0.425/examples/test_chat_room.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      614 2021-02-24 01:34:32.000000 blaster-server-0.0.425/examples/tornado_hello_world.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      791 2021-02-24 01:20:44.000000 blaster-server-0.0.425/examples/wheezy_hello.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       79 2023-04-16 18:16:05.846692 blaster-server-0.0.425/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1559 2023-04-16 17:58:45.000000 blaster-server-0.0.425/setup.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 18:16:05.846692 blaster-server-0.0.425/test/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2022-07-26 21:35:40.000000 blaster-server-0.0.425/test/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-01-07 00:03:08.000000 blaster-server-0.0.425/test/test_mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      503 2022-11-07 18:31:41.000000 blaster-server-0.0.425/test/test_schema.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5457 2022-12-09 21:19:51.000000 blaster-server-0.0.425/test/test_tools.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-16 18:15:30.000000 blaster-server-0.0.425/test/test_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      615 2021-02-24 11:15:27.000000 blaster-server-0.0.425/test/timeit_snippets.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 21:13:49.616373 blaster-server-0.0.425b0/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1061 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/LICENSE.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2022-11-07 18:47:07.000000 blaster-server-0.0.425b0/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-04-16 21:13:49.616373 blaster-server-0.0.425b0/PKG-INFO
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2620 2022-11-14 12:45:11.000000 blaster-server-0.0.425b0/README.md
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2021-10-05 11:27:02.000000 blaster-server-0.0.425b0/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 21:13:49.612373 blaster-server-0.0.425b0/blaster/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      875 2023-01-09 13:10:46.000000 blaster-server-0.0.425b0/blaster/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 21:13:49.616373 blaster-server-0.0.425b0/blaster/cloud/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2022-11-09 17:29:08.000000 blaster-server-0.0.425b0/blaster/cloud/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3257 2022-12-03 12:42:35.000000 blaster-server-0.0.425b0/blaster/cloud/analytics.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 21:13:49.616373 blaster-server-0.0.425b0/blaster/cloud/aws/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       78 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/blaster/cloud/aws/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2022-12-01 11:30:06.000000 blaster-server-0.0.425b0/blaster/cloud/aws/ses_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5230 2023-01-28 12:53:32.000000 blaster-server-0.0.425b0/blaster/cloud/push_tasks.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3729 2023-03-23 02:32:10.000000 blaster-server-0.0.425b0/blaster/cloud/storage.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3796 2023-03-06 12:38:58.000000 blaster-server-0.0.425b0/blaster/config.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-01-28 12:57:17.000000 blaster-server-0.0.425b0/blaster/connection_pool.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       99 2020-11-22 14:37:38.000000 blaster-server-0.0.425b0/blaster/constants.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5290 2023-03-30 07:56:48.000000 blaster-server-0.0.425b0/blaster/logging.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62680 2023-04-16 21:10:06.000000 blaster-server-0.0.425b0/blaster/mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    14954 2023-03-22 22:32:18.000000 blaster-server-0.0.425b0/blaster/schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    36589 2023-04-16 18:28:33.000000 blaster-server-0.0.425b0/blaster/server.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    47003 2023-04-16 21:09:40.000000 blaster-server-0.0.425b0/blaster/tools.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 21:13:49.616373 blaster-server-0.0.425b0/blaster/utils/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/blaster/utils/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 21:13:49.616373 blaster-server-0.0.425b0/blaster/utils/data/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2022-11-08 15:22:07.000000 blaster-server-0.0.425b0/blaster/utils/data/countries.json
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2022-12-01 10:20:50.000000 blaster-server-0.0.425b0/blaster/utils/data/mime_types.json
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7086 2023-04-16 20:57:56.000000 blaster-server-0.0.425b0/blaster/utils/data_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-01-07 12:42:21.000000 blaster-server-0.0.425b0/blaster/utils/events.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-03-30 16:36:26.000000 blaster-server-0.0.425b0/blaster/utils/fork.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1076 2023-02-21 07:52:48.000000 blaster-server-0.0.425b0/blaster/utils/lat_long_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5552 2023-02-01 17:01:50.000000 blaster-server-0.0.425b0/blaster/utils/phone_number_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     6773 2020-12-14 07:56:42.000000 blaster-server-0.0.425b0/blaster/utils/xss_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 21:13:49.616373 blaster-server-0.0.425b0/blaster/websocket/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1022 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/blaster/websocket/__init__.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12874 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/blaster/websocket/_abnf.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2022-01-06 11:42:20.000000 blaster-server-0.0.425b0/blaster/websocket/_app.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    16360 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/blaster/websocket/_core.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2141 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/blaster/websocket/_exceptions.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     4793 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/blaster/websocket/_handshake.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7288 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/blaster/websocket/_http.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1870 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/blaster/websocket/_logging.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3623 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/blaster/websocket/_socket.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1550 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/blaster/websocket/_ssl_compat.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3670 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/blaster/websocket/_url.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3632 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/blaster/websocket/_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12758 2021-10-03 12:23:56.000000 blaster-server-0.0.425b0/blaster/websocket/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 21:13:49.616373 blaster-server-0.0.425b0/blaster/websocket/tests/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/blaster/websocket/tests/__init__.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    26115 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/blaster/websocket/tests/test_websocket.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 21:13:49.616373 blaster-server-0.0.425b0/blaster_server.egg-info/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      851 2023-04-16 21:13:49.000000 blaster-server-0.0.425b0/blaster_server.egg-info/PKG-INFO
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1682 2023-04-16 21:13:49.000000 blaster-server-0.0.425b0/blaster_server.egg-info/SOURCES.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        1 2023-04-16 21:13:49.000000 blaster-server-0.0.425b0/blaster_server.egg-info/dependency_links.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      221 2023-04-16 21:13:49.000000 blaster-server-0.0.425b0/blaster_server.egg-info/requires.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       41 2023-04-16 21:13:49.000000 blaster-server-0.0.425b0/blaster_server.egg-info/top_level.txt
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 21:13:49.616373 blaster-server-0.0.425b0/examples/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/examples/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2022-01-06 11:42:20.000000 blaster-server-0.0.425b0/examples/fast_api_test.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      636 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/examples/gevent_wsgi_test.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      233 2021-10-04 14:48:01.000000 blaster-server-0.0.425b0/examples/meinheld_flask.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1743 2022-06-17 17:10:40.000000 blaster-server-0.0.425b0/examples/mongo_ormexample.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2022-11-14 12:13:43.000000 blaster-server-0.0.425b0/examples/simple_examples.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1088 2019-07-03 19:03:00.000000 blaster-server-0.0.425b0/examples/test_chat_room.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      614 2021-02-24 01:34:32.000000 blaster-server-0.0.425b0/examples/tornado_hello_world.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      791 2021-02-24 01:20:44.000000 blaster-server-0.0.425b0/examples/wheezy_hello.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       79 2023-04-16 21:13:49.616373 blaster-server-0.0.425b0/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1560 2023-04-16 21:10:32.000000 blaster-server-0.0.425b0/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-16 21:13:49.616373 blaster-server-0.0.425b0/test/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2022-07-26 21:35:40.000000 blaster-server-0.0.425b0/test/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-01-07 00:03:08.000000 blaster-server-0.0.425b0/test/test_mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      503 2022-11-07 18:31:41.000000 blaster-server-0.0.425b0/test/test_schema.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5457 2022-12-09 21:19:51.000000 blaster-server-0.0.425b0/test/test_tools.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-16 18:26:08.000000 blaster-server-0.0.425b0/test/test_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      615 2021-02-24 11:15:27.000000 blaster-server-0.0.425b0/test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.425/LICENSE.txt` & `blaster-server-0.0.425b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/PKG-INFO` & `blaster-server-0.0.425b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.425
+Version: 0.0.425b0
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.425/README.md` & `blaster-server-0.0.425b0/README.md`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/__init__.py` & `blaster-server-0.0.425b0/blaster/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/cloud/analytics.py` & `blaster-server-0.0.425b0/blaster/cloud/analytics.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/cloud/aws/ses_utils.py` & `blaster-server-0.0.425b0/blaster/cloud/aws/ses_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/cloud/push_tasks.py` & `blaster-server-0.0.425b0/blaster/cloud/push_tasks.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/cloud/storage.py` & `blaster-server-0.0.425b0/blaster/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/config.py` & `blaster-server-0.0.425b0/blaster/config.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/connection_pool.py` & `blaster-server-0.0.425b0/blaster/connection_pool.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/logging.py` & `blaster-server-0.0.425b0/blaster/logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/mongo_orm.py` & `blaster-server-0.0.425b0/blaster/mongo_orm.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from bson.objectid import ObjectId
 from itertools import chain
 from collections import OrderedDict
 from pymongo import MongoClient
 from pymongo.errors import DuplicateKeyError, OperationFailure
 from pymongo import ReturnDocument, ReadPreference
 from .tools import ExpiringCache, all_subclasses,\
-	cur_ms, list_diff2, batched_iter, _OBJ_END_
+	cur_ms, list_diff2, batched_iter, set_by_key_list,\
+	_OBJ_END_
 from .config import IS_DEV, MONGO_WARN_MAX_RESULTS_RATE,\
 	MONGO_MAX_RESULTS_AT_HIGH_SCAN_RATE,\
 	MONGO_WARN_MAX_QUERY_RESPONSE_TIME_SECONDS,\
 	DEBUG_PRINT_LEVEL
 from gevent.threading import Thread
 from gevent import time
 from .logging import LOG_WARN, LOG_SERVER, LOG_ERROR
@@ -203,15 +204,19 @@
 		self.path = path
 		if(initial_value):
 			self.update(initial_value)
 		self._initializing = False
 
 	def __setitem__(self, k, v):
 		if(not self._initializing):
-			self._model_obj._set_query_updates[self.path + "." + str(k)] = v
+			set_by_key_list(
+				self._model_obj._set_query_updates,
+				(self.path + "." + str(k)).split("."),
+				v
+			)
 		if(self._initializing):
 			# recursively create custom dicts/list when
 			# loading object from db
 			if(isinstance(v, dict)):
 				v = MongoDict(self._model_obj, self.path + "." + str(k), v)
 			elif(isinstance(v, list)):
 				v = MongoList(self._model_obj, self.path + "." + str(k), v)
```

### Comparing `blaster-server-0.0.425/blaster/schema.py` & `blaster-server-0.0.425b0/blaster/schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/server.py` & `blaster-server-0.0.425b0/blaster/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from . import req_ctx
 from .tools import SanitizedDict,\
 	set_socket_fast_close_options, BufferedSocket, ltrim,\
 	_OBJ_END_
 from .utils import events
 from .utils.data_utils import FILE_EXTENSION_TO_MIME_TYPE
-from .logging import LOG_ERROR, LOG_SERVER
+from .logging import LOG_ERROR, LOG_SERVER, LOG_WARN
 from .schema import Int, Object, Required, schema as schema_func
 from .websocket.server import WebSocketServerHandler
 from .config import IS_DEV, BLASTER_HTTP_TOOK_LONG_WARN_THRESHOLD
 
 if(IS_DEV):
 	# dev specific config
 	from .config import DEV_FORCE_ACCESS_CONTROL_ALLOW_ORIGIN
@@ -1052,18 +1052,20 @@
 		except Exception as ex:
 			stacktrace_string = traceback.format_exc()
 			status = None
 			resp_headers = []
 			body = None
 
 			# if given as error page handler
+			log_handler = LOG_ERROR
 			for exception_handler in self.server_exception_handlers:
 				if(resp := exception_handler(req, ex)):
 					status, _resp_headers, body = App.response_body_to_parts(resp)
 					_resp_headers and resp_headers.extend(_resp_headers)
+					log_handler = LOG_WARN
 					break
 			if(isinstance(body, (dict, list))):
 				body = json.dumps(body)
 				resp_headers.append("Content-Type: application/json")
 
 			status = str(status) if status else b'502 Server error'
 			body = body or b'Internal server error'
@@ -1078,15 +1080,15 @@
 
 			# err.2.3 send final headers(content related only) and body
 			buffered_socket.send(
 				b'Connection: close', b'\r\n',
 				b'Content-Length: ', str(len(body)), b'\r\n\r\n',
 				body
 			)
-			LOG_ERROR(
+			log_handler(
 				"http_error",
 				exception_str=str(ex),
 				stacktrace_string=stacktrace_string,
 				request_type=request_type,
 				request_line=request_line,
 				req_str=str(req.to_dict())
 			)
@@ -1227,15 +1229,15 @@
 
 	return url_path + "{*path}", file_handler
 
 
 def proxy_file_handler(url_path, proxy_url):
 	import requests
 
-	def file_handler(req:Request, path):
+	def file_handler(req: Request, path):
 		ret = requests.get(proxy_url + path, headers=dict(req._headers), verify=False)
 		return {"Content-Type": ret.headers["Content-Type"]}, ret.text
 	return url_path + "{*path}", file_handler
 
 
 # Get args hook
 def _get_web_socket_handler(req):
```

### Comparing `blaster-server-0.0.425/blaster/tools.py` & `blaster-server-0.0.425b0/blaster/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,28 +193,38 @@
 def from_kwargs(cls, **kwargs):
 	ret = cls()
 	for key in kwargs:
 		setattr(ret, key, kwargs[key])
 	return ret
 
 
-def get_by_key_list(d, keyList, default=None):
-	for key in keyList:
+def get_by_key_list(d, key_list, default=None):
+	for key in key_list:
 		if(not d):
 			return default
 		if(isinstance(d, list)):
 			key = int(key)
 			if(key >= len(d) or key < 0):
 				return default  # dead end
 			d = d[key]
 		else:
 			d = d.get(key, None)
 	return d
 
 
+def set_by_key_list(d, key_list, value):
+	if(not key_list):
+		return
+	for key in key_list[0:-1]:
+		if(key not in d):
+			d[key] = {}
+		d = d[key]
+	d[key_list[-1]] = value
+
+
 def date2string(date):
 	return date.isoformat()
 
 
 def date2timestamp(dt):
 	# datetime to timestamp
 	if not isinstance(dt, datetime):
```

### Comparing `blaster-server-0.0.425/blaster/utils/data/countries.json` & `blaster-server-0.0.425b0/blaster/utils/data/countries.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/utils/data/mime_types.json` & `blaster-server-0.0.425b0/blaster/utils/data/mime_types.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/utils/data_utils.py` & `blaster-server-0.0.425b0/blaster/utils/data_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,20 +43,21 @@
 	# update with aliases
 	for i,j in _currency_aliases.items():
 		INR_EXCHANGE_RATE[i] = INR_EXCHANGE_RATE[j]
 	
 # currencies END
 
 
-#### MIME_TYPES
+# MIME_TYPES
 __mime_types = json.loads(open(os.path.join(os.path.dirname(__file__), "data/mime_types.json")).read())
 FILE_EXTENSION_TO_MIME_TYPE = {k: v["mime_type"] for k, v in __mime_types.items()}
 MIME_TYPE_TO_EXTENSION = {v["mime_type"]: k for k, v in __mime_types.items()}
 
-#points  =
+
+# points  =
 def make_nearrest_currency(val, f):
 	val = int(val)
 	if val == 0:
 		return f
 	if(val%f == 0):
 		return val
 	return f * (val / f + 1)
```

### Comparing `blaster-server-0.0.425/blaster/utils/events.py` & `blaster-server-0.0.425b0/blaster/utils/events.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/utils/fork.py` & `blaster-server-0.0.425b0/blaster/utils/fork.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/utils/lat_long_utils.py` & `blaster-server-0.0.425b0/blaster/utils/lat_long_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/utils/phone_number_utils.py` & `blaster-server-0.0.425b0/blaster/utils/phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/utils/xss_html.py` & `blaster-server-0.0.425b0/blaster/utils/xss_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/websocket/__init__.py` & `blaster-server-0.0.425b0/blaster/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/websocket/_abnf.py` & `blaster-server-0.0.425b0/blaster/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/websocket/_app.py` & `blaster-server-0.0.425b0/blaster/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/websocket/_core.py` & `blaster-server-0.0.425b0/blaster/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/websocket/_exceptions.py` & `blaster-server-0.0.425b0/blaster/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/websocket/_handshake.py` & `blaster-server-0.0.425b0/blaster/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/websocket/_http.py` & `blaster-server-0.0.425b0/blaster/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/websocket/_logging.py` & `blaster-server-0.0.425b0/blaster/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/websocket/_socket.py` & `blaster-server-0.0.425b0/blaster/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/websocket/_ssl_compat.py` & `blaster-server-0.0.425b0/blaster/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/websocket/_url.py` & `blaster-server-0.0.425b0/blaster/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/websocket/_utils.py` & `blaster-server-0.0.425b0/blaster/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/websocket/server.py` & `blaster-server-0.0.425b0/blaster/websocket/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster/websocket/tests/test_websocket.py` & `blaster-server-0.0.425b0/blaster/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/blaster_server.egg-info/PKG-INFO` & `blaster-server-0.0.425b0/blaster_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.425
+Version: 0.0.425b0
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.425/blaster_server.egg-info/SOURCES.txt` & `blaster-server-0.0.425b0/blaster_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/examples/gevent_wsgi_test.py` & `blaster-server-0.0.425b0/examples/gevent_wsgi_test.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/examples/mongo_ormexample.py` & `blaster-server-0.0.425b0/examples/mongo_ormexample.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/examples/simple_examples.py` & `blaster-server-0.0.425b0/examples/simple_examples.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/examples/test_chat_room.py` & `blaster-server-0.0.425b0/examples/test_chat_room.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/examples/tornado_hello_world.py` & `blaster-server-0.0.425b0/examples/tornado_hello_world.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/examples/wheezy_hello.py` & `blaster-server-0.0.425b0/examples/wheezy_hello.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/setup.py` & `blaster-server-0.0.425b0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name='blaster-server',
 	packages=find_packages() + ["blaster/utils/data"],
-	version='0.0.425',
+	version='0.0.425b',
 	license='MIT',
 	description='Gevent based python server built from scratch for maximum performance',
 	author='Abhinav Reddy',                   # Type in your name
 	author_email='abhinavabcd@gmail.com',      # Type in your E-Mail
 	url='https://github.com/abhinavabcd/blaster',
 	download_url='https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz',
 	keywords=['server', 'superfast', 'Like FastApi or Flask but 10x faster'],
```

### Comparing `blaster-server-0.0.425/test/test_mongo_orm.py` & `blaster-server-0.0.425b0/test/test_mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/test/test_tools.py` & `blaster-server-0.0.425b0/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/test/test_utils.py` & `blaster-server-0.0.425b0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.425/test/timeit_snippets.py` & `blaster-server-0.0.425b0/test/timeit_snippets.py`

 * *Files identical despite different names*

