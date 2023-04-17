# Comparing `tmp/irc3-1.1.8.tar.gz` & `tmp/irc3-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irc3-1.1.8.tar", last modified: Sun Jul 17 21:57:12 2022, max compression
+gzip compressed data, was "irc3-1.1.9.tar", last modified: Mon Feb 27 10:50:57 2023, max compression
```

## Comparing `irc3-1.1.8.tar` & `irc3-1.1.9.tar`

### file list

```diff
@@ -1,185 +1,184 @@
-drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2022-07-17 21:57:12.337466 irc3-1.1.8/
--rw-r--r--   0 gawel     (1000) gawel     (1000)     8148 2022-07-17 21:57:12.000000 irc3-1.1.8/CHANGES.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1237 2022-07-17 21:57:12.000000 irc3-1.1.8/CONTRIBUTING.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1082 2022-07-17 21:57:12.000000 irc3-1.1.8/LICENSE
--rw-r--r--   0 gawel     (1000) gawel     (1000)      391 2022-07-17 21:57:12.000000 irc3-1.1.8/MANIFEST.in
--rw-r--r--   0 gawel     (1000) gawel     (1000)      448 2022-07-17 21:57:12.000000 irc3-1.1.8/Makefile
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2198 2022-07-17 21:57:12.337466 irc3-1.1.8/PKG-INFO
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1484 2022-07-17 21:57:12.000000 irc3-1.1.8/README.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1092 2022-07-17 21:57:12.000000 irc3-1.1.8/conftest.py
-drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2022-07-17 21:57:12.329466 irc3-1.1.8/docs/
--rw-r--r--   0 gawel     (1000) gawel     (1000)     5563 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/Makefile
-drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2022-07-17 21:57:12.329466 irc3-1.1.8/docs/_static/
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1034 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/_static/logo.png
--rwxr-xr-x   0 gawel     (1000) gawel     (1000)     7837 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/conf.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      446 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/dcc.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)      244 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/dec.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       33 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/hack.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1499 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/index.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)      280 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/irc3.rst
-drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2022-07-17 21:57:12.333466 irc3-1.1.8/docs/plugins/
--rw-r--r--   0 gawel     (1000) gawel     (1000)       44 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/asynchronious.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       42 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/autocommand.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       40 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/autojoins.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       39 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/casefold.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       38 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/command.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       35 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/core.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       35 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/cron.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       35 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/ctcp.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       34 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/dcc.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       36 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/feeds.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       35 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/fifo.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       36 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/human.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       34 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/log.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       37 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/logger.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       36 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/pager.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       39 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/quakenet.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       35 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/sasl.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       37 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/search.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       44 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/shell_command.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       36 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/slack.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       37 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/social.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       38 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/storage.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       37 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/uptime.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       39 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/userlist.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)       34 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/plugins/web.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1249 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/reloadable.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)    45232 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/rfc.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)      386 2022-07-17 21:57:12.000000 irc3-1.1.8/docs/utils.rst
-drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2022-07-17 21:57:12.333466 irc3-1.1.8/examples/
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1018 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/async_command.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      299 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/benches.ini
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1361 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/benches.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1394 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/bot.ini
--rw-r--r--   0 gawel     (1000) gawel     (1000)      847 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/commands.rst
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1295 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/config.ini
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2542 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/dcc_chat.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      734 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/dcc_send.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2232 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/dcc_send_and_get.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1286 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/dev.ini
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2912 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/freenode_irc3.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      783 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/humans.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2488 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/mybot.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      617 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/mybot_plugin.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      598 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/mycommands.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      249 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/mycrons.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      336 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/myextends.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      390 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/nickserv.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      885 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/paginate.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      342 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/proxy.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      338 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/slack.ini
--rw-r--r--   0 gawel     (1000) gawel     (1000)      187 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/spy.ini
--rw-r--r--   0 gawel     (1000) gawel     (1000)      876 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/spy.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1253 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/topic.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      726 2022-07-17 21:57:12.000000 irc3-1.1.8/examples/wsgiapp.py
-drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2022-07-17 21:57:12.333466 irc3-1.1.8/irc3/
--rw-r--r--   0 gawel     (1000) gawel     (1000)    14481 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/__init__.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)       59 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/__main__.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2996 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/_gen_doc.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     5552 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/_parse_rfc.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)    39532 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/_rfc.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     3520 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/asynchronous.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)    17007 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/base.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1377 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/compat.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2983 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/config.py
-drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2022-07-17 21:57:12.333466 irc3-1.1.8/irc3/dcc/
--rw-r--r--   0 gawel     (1000) gawel     (1000)      174 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/dcc/__init__.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     6660 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/dcc/client.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     5638 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/dcc/manager.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      427 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/dcc/optim.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     4402 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/dec.py
-drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2022-07-17 21:57:12.333466 irc3-1.1.8/irc3/plugins/
--rw-r--r--   0 gawel     (1000) gawel     (1000)       24 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/__init__.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)    13254 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/asynchronious.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     3305 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/autocommand.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     4191 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/autojoins.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2105 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/casefold.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)    17660 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/command.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     3837 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/core.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2461 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/cron.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2248 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/ctcp.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1960 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/dcc.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     8778 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/feeds.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     4299 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/fifo.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     3011 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/human.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1645 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/log.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     3847 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/logger.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2869 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/pager.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     3924 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/quakenet.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1758 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/sasl.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1527 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/search.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     3987 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/shell_command.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)    11213 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/slack.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     6822 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/social.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)    12211 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/storage.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1529 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/uptime.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     6805 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/userlist.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2629 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/plugins/web.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     4399 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/rfc.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)   138964 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/rfc1459.txt
--rw-r--r--   0 gawel     (1000) gawel     (1000)   122637 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/rfc2812.txt
--rw-r--r--   0 gawel     (1000) gawel     (1000)     3560 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/tags.py
-drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2022-07-17 21:57:12.333466 irc3-1.1.8/irc3/template/
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1008 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/template/__init__.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)       95 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/template/__main__.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1305 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/template/config.ini
--rw-r--r--   0 gawel     (1000) gawel     (1000)      617 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/template/plugin.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     6727 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/testing.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)    10707 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3/utils.py
-drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2022-07-17 21:57:12.333466 irc3-1.1.8/irc3.egg-info/
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2198 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3.egg-info/PKG-INFO
--rw-r--r--   0 gawel     (1000) gawel     (1000)     3522 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3.egg-info/SOURCES.txt
--rw-r--r--   0 gawel     (1000) gawel     (1000)        1 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3.egg-info/dependency_links.txt
--rw-r--r--   0 gawel     (1000) gawel     (1000)       69 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3.egg-info/entry_points.txt
--rw-r--r--   0 gawel     (1000) gawel     (1000)        1 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3.egg-info/not-zip-safe
--rw-r--r--   0 gawel     (1000) gawel     (1000)      149 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3.egg-info/requires.txt
--rw-r--r--   0 gawel     (1000) gawel     (1000)       11 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3.egg-info/top_level.txt
-drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2022-07-17 21:57:12.337466 irc3-1.1.8/irc3d/
--rw-r--r--   0 gawel     (1000) gawel     (1000)     5860 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3d/__init__.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      774 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3d/__main__.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1192 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3d/dec.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      384 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3d/motd.txt
-drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2022-07-17 21:57:12.337466 irc3-1.1.8/irc3d/plugins/
--rw-r--r--   0 gawel     (1000) gawel     (1000)       24 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3d/plugins/__init__.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     4694 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3d/plugins/command.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     3728 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3d/plugins/core.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)    11724 2022-07-17 21:57:12.000000 irc3-1.1.8/irc3d/plugins/userlist.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      436 2022-07-17 21:57:12.337466 irc3-1.1.8/setup.cfg
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1689 2022-07-17 21:57:12.000000 irc3-1.1.8/setup.py
-drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2022-07-17 21:57:12.337466 irc3-1.1.8/tests/
--rw-r--r--   0 gawel     (1000) gawel     (1000)        0 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/__init__.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)    14955 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/feed.atom
--rw-r--r--   0 gawel     (1000) gawel     (1000)      486 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test.ini
--rw-r--r--   0 gawel     (1000) gawel     (1000)     7497 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_async.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1997 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_autocommand.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2840 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_autojoins.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     5309 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_bot.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      988 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_casefold.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)    10243 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_commands.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2000 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_cron.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1186 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_ctcp.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     6741 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_dcc.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      584 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_dec.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1837 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_events.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2915 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_feeds.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1406 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_fifo.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     3786 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_irc3d.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1978 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_irc3d_commands.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     5285 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_irc3d_userlist.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1705 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_logger.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      855 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_paginate.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1144 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_protocol.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2532 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_quakenet.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1079 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_reconn.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2109 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_reload.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     1671 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_run.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      849 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_sasl.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      877 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_search.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2123 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_slack.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2636 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_social.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      955 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_template.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      729 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_uptime.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2865 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_userlist.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2973 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_utils.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)     2286 2022-07-17 21:57:12.000000 irc3-1.1.8/tests/test_web.py
--rw-r--r--   0 gawel     (1000) gawel     (1000)      792 2022-07-17 21:57:12.000000 irc3-1.1.8/tox.ini
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2023-02-27 10:50:57.833097 irc3-1.1.9/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     8241 2023-02-27 10:50:57.000000 irc3-1.1.9/CHANGES.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1248 2023-02-27 10:50:57.000000 irc3-1.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1082 2023-02-27 10:50:57.000000 irc3-1.1.9/LICENSE
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      391 2023-02-27 10:50:57.000000 irc3-1.1.9/MANIFEST.in
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      448 2023-02-27 10:50:57.000000 irc3-1.1.9/Makefile
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2250 2023-02-27 10:50:57.833097 irc3-1.1.9/PKG-INFO
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1484 2023-02-27 10:50:57.000000 irc3-1.1.9/README.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1092 2023-02-27 10:50:57.000000 irc3-1.1.9/conftest.py
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2023-02-27 10:50:57.825096 irc3-1.1.9/docs/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     5563 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/Makefile
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2023-02-27 10:50:57.825096 irc3-1.1.9/docs/_static/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1034 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/_static/logo.png
+-rwxr-xr-x   0 gawel     (1000) gawel     (1000)     7829 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/conf.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      446 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/dcc.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      244 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/dec.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       33 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/hack.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1499 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/index.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      280 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/irc3.rst
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2023-02-27 10:50:57.829096 irc3-1.1.9/docs/plugins/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       44 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/asynchronious.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       42 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/autocommand.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       40 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/autojoins.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       39 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/casefold.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       38 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/command.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       35 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/core.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       35 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/cron.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       35 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/ctcp.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       34 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/dcc.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       36 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/feeds.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       35 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/fifo.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       36 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/human.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       34 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/log.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       37 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/logger.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       36 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/pager.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       39 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/quakenet.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       35 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/sasl.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       37 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/search.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       44 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/shell_command.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       36 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/slack.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       37 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/social.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       38 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/storage.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       37 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/uptime.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       39 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/userlist.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       34 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/plugins/web.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1249 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/reloadable.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)    45232 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/rfc.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      386 2023-02-27 10:50:57.000000 irc3-1.1.9/docs/utils.rst
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2023-02-27 10:50:57.829096 irc3-1.1.9/examples/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1018 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/async_command.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      299 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/benches.ini
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1361 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/benches.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1394 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/bot.ini
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      847 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/commands.rst
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1295 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/config.ini
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2542 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/dcc_chat.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      734 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/dcc_send.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2232 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/dcc_send_and_get.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1286 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/dev.ini
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2912 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/freenode_irc3.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      783 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/humans.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2488 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/mybot.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      617 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/mybot_plugin.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      598 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/mycommands.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      249 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/mycrons.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      336 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/myextends.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      390 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/nickserv.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      885 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/paginate.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      342 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/proxy.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      338 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/slack.ini
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      187 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/spy.ini
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      876 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/spy.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1253 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/topic.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      726 2023-02-27 10:50:57.000000 irc3-1.1.9/examples/wsgiapp.py
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2023-02-27 10:50:57.829096 irc3-1.1.9/irc3/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)    14524 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/__init__.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       59 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/__main__.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2996 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/_gen_doc.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     5552 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/_parse_rfc.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)    39532 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/_rfc.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     3554 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/asynchronous.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)    16765 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/base.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      956 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/compat.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2983 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/config.py
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2023-02-27 10:50:57.829096 irc3-1.1.9/irc3/dcc/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      174 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/dcc/__init__.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     6560 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/dcc/client.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     5449 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/dcc/manager.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     4472 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/dec.py
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2023-02-27 10:50:57.829096 irc3-1.1.9/irc3/plugins/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       24 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/__init__.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)    13250 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/asynchronious.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     3305 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/autocommand.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     4191 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/autojoins.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2105 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/casefold.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)    17660 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/command.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     3837 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/core.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2461 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/cron.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2248 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/ctcp.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1960 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/dcc.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     8658 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/feeds.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     4299 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/fifo.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     3008 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/human.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1645 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/log.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     3847 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/logger.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2869 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/pager.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     3924 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/quakenet.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1758 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/sasl.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1527 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/search.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     3989 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/shell_command.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)    11213 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/slack.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     6822 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/social.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)    12211 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/storage.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1529 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/uptime.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     6805 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/userlist.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2629 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/plugins/web.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     4399 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/rfc.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)   138964 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/rfc1459.txt
+-rw-r--r--   0 gawel     (1000) gawel     (1000)   122637 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/rfc2812.txt
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     3560 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/tags.py
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2023-02-27 10:50:57.829096 irc3-1.1.9/irc3/template/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1008 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/template/__init__.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       95 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/template/__main__.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1305 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/template/config.ini
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      617 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/template/plugin.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     6727 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/testing.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)    10776 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3/utils.py
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2023-02-27 10:50:57.829096 irc3-1.1.9/irc3.egg-info/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2250 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3.egg-info/PKG-INFO
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     3504 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3.egg-info/SOURCES.txt
+-rw-r--r--   0 gawel     (1000) gawel     (1000)        1 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3.egg-info/dependency_links.txt
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       69 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3.egg-info/entry_points.txt
+-rw-r--r--   0 gawel     (1000) gawel     (1000)        1 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3.egg-info/not-zip-safe
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      149 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3.egg-info/requires.txt
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       11 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3.egg-info/top_level.txt
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2023-02-27 10:50:57.829096 irc3-1.1.9/irc3d/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     5860 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3d/__init__.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      774 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3d/__main__.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1192 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3d/dec.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      384 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3d/motd.txt
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2023-02-27 10:50:57.833097 irc3-1.1.9/irc3d/plugins/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)       24 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3d/plugins/__init__.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     4694 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3d/plugins/command.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     3728 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3d/plugins/core.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)    11724 2023-02-27 10:50:57.000000 irc3-1.1.9/irc3d/plugins/userlist.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      463 2023-02-27 10:50:57.833097 irc3-1.1.9/setup.cfg
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1740 2023-02-27 10:50:57.000000 irc3-1.1.9/setup.py
+drwxr-xr-x   0 gawel     (1000) gawel     (1000)        0 2023-02-27 10:50:57.833097 irc3-1.1.9/tests/
+-rw-r--r--   0 gawel     (1000) gawel     (1000)        0 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/__init__.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)    14955 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/feed.atom
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      486 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test.ini
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     7497 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_async.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1997 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_autocommand.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2840 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_autojoins.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     5309 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_bot.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      984 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_casefold.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)    10243 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_commands.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1987 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_cron.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1186 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_ctcp.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     6476 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_dcc.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      584 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_dec.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1816 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_events.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2915 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_feeds.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1406 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_fifo.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     3786 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_irc3d.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1978 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_irc3d_commands.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     5285 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_irc3d_userlist.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1704 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_logger.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      855 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_paginate.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1144 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_protocol.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2532 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_quakenet.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1079 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_reconn.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2109 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_reload.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     1671 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_run.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      849 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_sasl.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      877 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_search.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2123 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_slack.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2624 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_social.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      955 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_template.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      729 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_uptime.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2865 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_userlist.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2973 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_utils.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)     2286 2023-02-27 10:50:57.000000 irc3-1.1.9/tests/test_web.py
+-rw-r--r--   0 gawel     (1000) gawel     (1000)      789 2023-02-27 10:50:57.000000 irc3-1.1.9/tox.ini
```

### Comparing `irc3-1.1.8/CHANGES.rst` & `irc3-1.1.9/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+1.1.9 (2023-02-27)
+==================
+
+- drop support for python 3.5
+
+- python 3.11 compat
+
+
 1.1.8 (2022-07-17)
 ==================
 
 - Allow comma-separated chans in server userlist JOIN
 
 - python 3.10 compat
```

### Comparing `irc3-1.1.8/CONTRIBUTING.rst` & `irc3-1.1.9/CONTRIBUTING.rst`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 First, if you want to add a cool plugin, consider submit a pull request to the
 `irc3_plugins <https://github.com/gawel/irc3_plugins>`_ instead of irc3 itself.
 
 
 Feel free to clone the project on `GitHub <https://github.com/gawel/irc3>`_.
 
+To test your change you can run irc3 in debug mode using::
+
+    $ irc3 --debug path-to-your-conf.ini
+
 Once you made a change, try to add a test for your feature/fix. At least assume
 that you have'nt broke anything by running tox::
 
     $ tox
     ...
     py27: commands succeeded
     py32: commands succeeded
@@ -36,13 +40,11 @@
 
     $ tox -e docs
 
 And check the result::
 
     $ firefox .tox/docs/tmp/html/index.html
 
-The project is `buildout <https://github.com/buildout/buildout>`_ ready. You
-can generate binaries using it instead of virtualenv::
+The project uses ``setuptools``, you can test-install it using `pip`:
 
-    $ python bootstrap.py
-    $ bin/buildout
-    $ bin/irc3 -h
+    $ pip install .
+    $ irc3 -h
```

### Comparing `irc3-1.1.8/LICENSE` & `irc3-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/PKG-INFO` & `irc3-1.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: irc3
-Version: 1.1.8
+Version: 1.1.9
 Summary: plugable irc client library based on asyncio with DCC and SASL support
 Home-page: https://github.com/gawel/irc3/
 Author: Gael Pasgrimaud
 Author-email: gael@gawel.org
 License: MIT
 Keywords: irc dcc asyncio
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Communications :: Chat :: Internet Relay Chat
 Classifier: Development Status :: 5 - Production/Stable
 Provides-Extra: test
 Provides-Extra: web
 License-File: LICENSE
```

### Comparing `irc3-1.1.8/README.rst` & `irc3-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/conftest.py` & `irc3-1.1.9/conftest.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/docs/Makefile` & `irc3-1.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/docs/_static/logo.png` & `irc3-1.1.9/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/docs/conf.py` & `irc3-1.1.9/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 # The encoding of source files.
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = u'irc3'
-copyright = u'2013, Gael Pasgrimaud'
+project = 'irc3'
+copyright = '2013, Gael Pasgrimaud'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = ''
@@ -179,16 +179,16 @@
 # Additional stuff for the LaTeX preamble.
 #'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-  ('index', 'irc3.tex', u'irc3 Documentation',
-   u'Gael Pasgrimaud', 'manual'),
+  ('index', 'irc3.tex', 'irc3 Documentation',
+   'Gael Pasgrimaud', 'manual'),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 #latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -209,30 +209,30 @@
 
 
 # -- Options for manual page output --------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    ('index', 'irc3', u'irc3 Documentation',
-     [u'Gael Pasgrimaud'], 1)
+    ('index', 'irc3', 'irc3 Documentation',
+     ['Gael Pasgrimaud'], 1)
 ]
 
 # If true, show URL addresses after external links.
 #man_show_urls = False
 
 
 # -- Options for Texinfo output ------------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-  ('index', 'irc3', u'irc3 Documentation',
-   u'Gael Pasgrimaud', 'irc3', 'One line description of project.',
+  ('index', 'irc3', 'irc3 Documentation',
+   'Gael Pasgrimaud', 'irc3', 'One line description of project.',
    'Miscellaneous'),
 ]
 
 # Documents to append as an appendix to all manuals.
 #texinfo_appendices = []
 
 # If false, no module index is generated.
```

### Comparing `irc3-1.1.8/docs/index.rst` & `irc3-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/docs/reloadable.rst` & `irc3-1.1.9/docs/reloadable.rst`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/docs/rfc.rst` & `irc3-1.1.9/docs/rfc.rst`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/async_command.py` & `irc3-1.1.9/examples/async_command.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/benches.py` & `irc3-1.1.9/examples/benches.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/bot.ini` & `irc3-1.1.9/examples/bot.ini`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/commands.rst` & `irc3-1.1.9/examples/commands.rst`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/config.ini` & `irc3-1.1.9/examples/config.ini`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/dcc_chat.py` & `irc3-1.1.9/examples/dcc_chat.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/dcc_send.py` & `irc3-1.1.9/examples/dcc_send.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/dcc_send_and_get.py` & `irc3-1.1.9/examples/dcc_send_and_get.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/dev.ini` & `irc3-1.1.9/examples/dev.ini`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/freenode_irc3.py` & `irc3-1.1.9/examples/freenode_irc3.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/humans.py` & `irc3-1.1.9/examples/humans.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/mybot.py` & `irc3-1.1.9/examples/mybot.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/mybot_plugin.py` & `irc3-1.1.9/examples/mybot_plugin.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/mycommands.py` & `irc3-1.1.9/examples/mycommands.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/paginate.py` & `irc3-1.1.9/examples/paginate.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/spy.py` & `irc3-1.1.9/examples/spy.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/topic.py` & `irc3-1.1.9/examples/topic.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/examples/wsgiapp.py` & `irc3-1.1.9/examples/wsgiapp.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/__init__.py` & `irc3-1.1.9/irc3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,15 @@
                 'NICK {nick}\r\n'
             ).format(**self.config))
             self.notify('connection_made')
 
     def send_line(self, data, nowait=False):
         """send a line to the server. replace CR by spaces"""
         data = data.replace('\n', ' ').replace('\r', ' ')
-        f = asyncio.Future(loop=self.loop)
+        f = self.loop.create_future()
         if self.queue is not None and nowait is False:
             self.queue.put_nowait((f, data))
         else:
             self.send(data.replace('\n', ' ').replace('\r', ' '))
             f.set_result(True)
         return f
 
@@ -203,15 +203,15 @@
                 for i in range(flood_burst):
                     future, data = await self.queue.get()
                     future.set_result(True)
                     lines.append(data)
                     if self.queue.empty():
                         break
                 if lines:
-                    self.send(u'\r\n'.join(lines))
+                    self.send('\r\n'.join(lines))
                 while not self.queue.empty():
                     await asyncio.sleep(flood_rate, loop=self.loop)
                     future, data = await self.queue.get()
                     future.set_result(True)
                     self.send(data)
 
     def send(self, data):
@@ -369,37 +369,39 @@
     @property
     def dcc(self):
         """return the :class:`~irc3.dcc.DCCManager`"""
         if self._dcc is None:
             self._dcc = DCCManager(self)
         return self._dcc
 
-    @asyncio.coroutine
-    def dcc_chat(self, mask, host=None, port=None):
+    async def dcc_chat(self, mask, host=None, port=None):
         """Open a DCC CHAT whith mask. If host/port are specified then connect
         to a server. Else create a server"""
-        return self.dcc.create(
-            'chat', mask, host=host, port=port).ready
+        conn = self.dcc.create(
+            'chat', mask, host=host, port=port)
+        await conn.ready
+        return conn
 
-    @asyncio.coroutine
-    def dcc_get(self, mask, host, port, filepath, filesize=None):
+    async def dcc_get(self, mask, host, port, filepath, filesize=None):
         """DCC GET a file from mask. filepath must be an absolute path with an
         existing directory. filesize is the expected file size."""
-        return self.dcc.create(
+        conn = self.dcc.create(
             'get', mask, filepath=filepath, filesize=filesize,
-            host=host, port=port).ready
+            host=host, port=port)
+        await conn.ready
+        return conn
 
-    @asyncio.coroutine
-    def dcc_send(self, mask, filepath):
+    async def dcc_send(self, mask, filepath):
         """DCC SEND a file to mask. filepath must be an absolute path to
         existing file"""
-        return self.dcc.create('send', mask, filepath=filepath).ready
+        conn = self.dcc.create('send', mask, filepath=filepath)
+        await conn.ready
+        return conn
 
-    @asyncio.coroutine
-    def dcc_accept(self, mask, filepath, port, pos):
+    async def dcc_accept(self, mask, filepath, port, pos):
         """accept a DCC RESUME for an axisting DCC SEND. filepath is the
         filename to sent.  port is the port opened on the server.
         pos is the expected offset"""
         return self.dcc.resume(mask, filepath, port, pos)
 
     def SIGHUP(self):
         self.reload()
```

### Comparing `irc3-1.1.8/irc3/_gen_doc.py` & `irc3-1.1.9/irc3/_gen_doc.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/_parse_rfc.py` & `irc3-1.1.9/irc3/_parse_rfc.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/_rfc.py` & `irc3-1.1.9/irc3/_rfc.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/asynchronous.py` & `irc3-1.1.9/irc3/asynchronous.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 from .compat import asyncio
-import functools
 import re
 
 
 class event:
 
     iotype = 'in'
     iscoroutine = True
@@ -27,15 +26,17 @@
 
     def __repr__(self):
         s = getattr(self.regexp, 'name', self.regexp)
         name = self.__class__.__name__
         return '<temp_event {0} {1}>'.format(name, s)
 
     def __call__(self, callback):
-        self.callback = asyncio.coroutine(functools.partial(callback, self))
+        async def wrapper(*args, **kwargs):
+            return await callback(self, *args, **kwargs)
+        self.callback = wrapper
         return self
 
 
 def default_result_processor(self, results=None, **value):  # pragma: no cover
     value['results'] = results
     if len(results) == 1:
         value.update(results[0])
@@ -43,15 +44,15 @@
 
 
 def async_events(context, events, send_line=None,
                  process_results=default_result_processor,
                  timeout=30, **params):
 
     loop = context.loop
-    task = asyncio.Future(loop=loop)  # async result
+    task = loop.create_future()  # async result
     results = []  # store events results
     events_ = []  # reference registered events
 
     # async timeout
     timeout = asyncio.ensure_future(
         asyncio.sleep(timeout, loop=loop), loop=loop)
```

### Comparing `irc3-1.1.8/irc3/base.py` & `irc3-1.1.9/irc3/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,25 +103,20 @@
         if self.loop is None:
             try:
                 self.loop = asyncio.get_event_loop()
             except RuntimeError:
                 self.loop = asyncio.new_event_loop()
                 asyncio.set_event_loop(self.loop)
 
-        # python 3.4.1 do not have a create_task method. check for it
-        self.create_task = getattr(self.loop, 'create_task', self.create_task)
+        self.create_task = self.loop.create_task
 
         self.registry = Registry()
 
         self.include(*self.config.get('includes', []))
 
-    def create_task(self, coro):  # pragma: no cover
-        # python 3.4.1 fallback
-        return asyncio.ensure_future(coro, loop=self.loop)
-
     def get_plugin(self, ob):
         plugins = self.registry.plugins
         includes = self.registry.includes
         reloading = self.registry.reloading
 
         if isinstance(ob, str):
             ob_name = ob
@@ -195,15 +190,15 @@
     def include(self, *modules, **kwargs):
         reg = self.registry
         categories = kwargs.get('venusian_categories',
                                 self.venusian_categories)
         scanner = self.venusian.Scanner(context=self)
         for module in modules:
             if module in reg.includes:
-                self.log.warn('%s included twice', module)
+                self.log.warning('%s included twice', module)
             else:
                 reg.includes.add(module)
                 try:
                     module = utils.maybedotted(module)
                 except LookupError as exc:
                     if HAS_PKG_RESOURCES:
                         entry_points = iter_entry_points(
```

### Comparing `irc3-1.1.8/irc3/config.py` & `irc3-1.1.9/irc3/config.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/dcc/client.py` & `irc3-1.1.9/irc3/dcc/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: utf-8 -*-
+import os
 import struct
 from collections import deque
 from functools import partial
 from irc3.compat import asyncio
 
 
 class DCCBase(asyncio.Protocol):
@@ -10,17 +11,17 @@
     idle_handle = None
     idle_timeout = None
     fd = None
 
     def __init__(self, **kwargs):
         for k, v in kwargs.items():
             setattr(self, k, v)
-        self.ready = asyncio.Future(loop=self.loop)
-        self.started = asyncio.Future(loop=self.loop)
-        self.closed = asyncio.Future(loop=self.loop)
+        self.ready = self.loop.create_future()
+        self.started = self.loop.create_future()
+        self.closed = self.loop.create_future()
         self.timeout_handle = None
 
     def factory(self):
         return self
 
     def connection_made(self, transport):
         self.transport = transport
@@ -169,19 +170,16 @@
         self.loop.remove_writer(socket)
         self.loop.add_writer(socket, self.next_chunk)
 
     def write(self, *args):  # pragma: no cover
         raise NotImplementedError('write is not available during DCCSend')
 
     def send_chunk(self):
-        if self.sendfile:
-            sent = self.sendfile(self.fd, self.offset, self.block_size)
-        else:
-            self.fd.seek(self.offset)
-            sent = self.socket.send(self.fd.read(self.block_size))
+        sent = os.sendfile(self.socket.fileno(), self.fd_fileno,
+                           self.offset, self.block_size)
         return sent
 
     def next_chunk(self):
         try:
             sent = self.send_chunk()
         except Exception as e:  # pragma: no cover
             self.bot.log.exception(e)
```

### Comparing `irc3-1.1.8/irc3/dcc/manager.py` & `irc3-1.1.9/irc3/dcc/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 # -*- coding: utf-8 -*-
 import os
 from functools import partial
 from collections import defaultdict
-from irc3.compat import PY35
 from irc3.utils import slugify
 from irc3.utils import maybedotted
 from irc3.dcc.client import DCCChat
 from irc3.dcc.client import DCCGet
-
-if PY35:
-    from irc3.dcc.client import DCCSend
-else:
-    try:
-        from irc3.dcc.optim import DCCSend
-    except ImportError:  # pragma: no cover
-        from irc3.dcc.client import DCCSend
+from irc3.dcc.client import DCCSend
 
 DCC_TYPES = ('chat', 'get', 'send')
 
 
 class DCCManager:
     """Manage DCC connections"""
```

### Comparing `irc3-1.1.8/irc3/dec.py` & `irc3-1.1.9/irc3/dec.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     setattr(wrapped, '__irc3d_plugin__', False)
     return wrapped
 
 
 class event:
     r"""register a method or function an irc event callback::
 
-        >>> @event('^:\S+ 353 [^&#]+(?P<channel>\S+) :(?P<nicknames>.*)')
+        >>> @event(r'^:\S+ 353 [^&#]+(?P<channel>\S+) :(?P<nicknames>.*)')
         ... def on_names(bot, channel=None, nicknames=None):
         ...     '''this will catch nickname when you enter a channel'''
         ...     print(channel, nicknames.split(':'))
 
     The callback can be either a function or a plugin method
 
     If you specify the `iotype` parameter to `"out"` then the event will be
@@ -114,13 +114,15 @@
         >>> print(bot.my_usefull_method(2))
         my_usefull_method(*(2,))
 
     """
     def callback(context, name, ob):
         obj = context.context
         if info.scope == 'class':
-            f = getattr(obj.get_plugin(ob), func.__name__)
+            instance = obj.get_plugin(ob)
+            f = getattr(instance, func.__name__)
         else:
+            instance = obj
             f = func
-        setattr(obj, f.__name__, f.__get__(obj, obj.__class__))
+        setattr(obj, f.__name__, f.__get__(instance, instance.__class__))
     info = venusian.attach(func, callback, category='irc3.extend')
     return func
```

### Comparing `irc3-1.1.8/irc3/plugins/asynchronious.py` & `irc3-1.1.9/irc3/plugins/asynchronious.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     send_line = 'WHOIS {nick} {nick}'
 
     # when those events occurs, we can add them to the result list
     events = (
         # (?i) is for IGNORECASE. This will match either NicK or nick
         {'match': r"(?i)^:\S+ 301 \S+ {nick} :(?P<away>.*)"},
         {'match': r"(?i)^:\S+ 311 \S+ {nick} (?P<username>\S+) "
-                  r"(?P<host>\S+) . :(?P<realname>.*)(?i)"},
+                  r"(?P<host>\S+) . :(?P<realname>.*)"},
         {'match': r"(?i)^:\S+ 312 \S+ {nick} (?P<server>\S+) "
                   r":(?P<server_desc>.*)"},
         {'match': r"(?i)^:\S+ 317 \S+ {nick} (?P<idle>[0-9]+).*"},
         {'match': r"(?i)^:\S+ 319 \S+ {nick} :(?P<channels>.*)",
          'multi': True},
         {'match': r"(?i)^:\S+ 330 \S+ {nick} (?P<account>\S+) "
                   r":(?P<account_desc>.*)"},
```

### Comparing `irc3-1.1.8/irc3/plugins/autocommand.py` & `irc3-1.1.9/irc3/plugins/autocommand.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/autojoins.py` & `irc3-1.1.9/irc3/plugins/autojoins.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/casefold.py` & `irc3-1.1.9/irc3/plugins/casefold.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/command.py` & `irc3-1.1.9/irc3/plugins/command.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/core.py` & `irc3-1.1.9/irc3/plugins/core.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/cron.py` & `irc3-1.1.9/irc3/plugins/cron.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/ctcp.py` & `irc3-1.1.9/irc3/plugins/ctcp.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/dcc.py` & `irc3-1.1.9/irc3/plugins/dcc.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/feeds.py` & `irc3-1.1.9/irc3/plugins/feeds.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,20 @@
 Here is a more complete hook used on freenode#irc3:
 
 .. literalinclude:: ../../examples/freenode_irc3.py
    :pyobject: FeedsHook
 
 '''
 
+HEADERS = {
+    'User-Agent': 'python-requests/irc3/feeds',
+    'Cache-Control': 'max-age=0',
+    'Pragma': 'no-cache',
+}
+
 
 def default_hook(entries):
     """Default hook called for each entry"""
     return entries
 
 
 def default_dispatcher(bot):  # pragma: no cover
@@ -74,18 +80,18 @@
     def dispatcher(messages):
         bot.call_many('privmsg', messages)
     return dispatcher
 
 
 def fetch(args):
     """fetch a feed"""
-    session = args['session']
+    requests = args['requests']
     for feed, filename in zip(args['feeds'], args['filenames']):
         try:
-            resp = session.get(feed, timeout=5)
+            resp = requests.get(feed, timeout=5, headers=HEADERS)
             content = resp.content
         except Exception:  # pragma: no cover
             pass
         else:
             with open(filename, 'wb') as fd:
                 fd.write(content)
     return args['name']
@@ -138,20 +144,14 @@
 
 @irc3.plugin
 class Feeds:
     """Feeds plugin"""
 
     PoolExecutor = ThreadPoolExecutor
 
-    headers = {
-        'User-Agent': 'python-requests/irc3/feeds',
-        'Cache-Control': 'max-age=0',
-        'Pragma': 'no-cache',
-    }
-
     def __init__(self, bot):
         bot.feeds = self
         self.bot = bot
 
         config = bot.config.get(__name__, {})
 
         self.directory = os.path.expanduser(
@@ -173,15 +173,14 @@
         delay = int(config.get('delay', 5))
         self.delay = delay * 60
 
         feed_config = dict(
             fmt=config.get('fmt', '[{feed.name}] {entry.title} {entry.link}'),
             delay=delay,
             channels=config.get('channels', ''),
-            headers=self.headers,
             time=0,
         )
 
         self.feeds = {}
         for name, feed in config.items():
             if str(feed).startswith('http'):
                 feeds = []
@@ -218,18 +217,17 @@
         except ImportError:  # pragma: no cover
             self.bot.log.critical('feedparser is not installed')
             self.feedparser = None
         try:
             import requests
         except ImportError:  # pragma: no cover
             self.bot.log.critical('requests is not installed')
-            self.session = None
+            self.requests = None
         else:
-            self.session = requests.Session()
-            self.session.headers.update(self.headers)
+            self.requests = requests
 
     def parse(self, *args):
         """parse pre-fetched feeds and notify new entries"""
         entries = []
         for feed in self.feeds.values():
             self.bot.log.debug('Parsing feed %s', feed['name'])
             entries.extend(parse(self.feedparser, feed))
@@ -252,16 +250,15 @@
 
     def update(self):
         """update feeds"""
         loop = self.bot.loop
         loop.call_later(self.delay, self.update)
 
         now = time.time()
-        session = self.session
-        feeds = [dict(f, session=session) for f in self.feeds.values()
+        feeds = [dict(f, requests=self.requests) for f in self.feeds.values()
                  if f['time'] < now - f['delay']]
         if feeds:
             self.bot.log.info('Fetching feeds %s',
                               ', '.join([f['name'] for f in feeds]))
             tasks = []
             for feed in feeds:
                 task = loop.run_in_executor(None, fetch, feed)
```

### Comparing `irc3-1.1.8/irc3/plugins/fifo.py` & `irc3-1.1.9/irc3/plugins/fifo.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/human.py` & `irc3-1.1.9/irc3/plugins/human.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,19 +63,19 @@
             data = page.read()
             if isinstance(data, bytes):
                 data = data.decode('utf8')
             quotes = json.loads(data)
             quotes = [v['joke'] for v in quotes['value']]
         except Exception:
             self.bot.log.error('Failed to get quotes from api.icndb.com')
-            quotes = [u'Hi!', u'lol']
+            quotes = ['Hi!', 'lol']
         self.bot.log.info('Initialise %s with %s quotes',
                           self.db, len(quotes))
         with codecs.open(self.db, 'w', 'utf8') as fd:
-            fd.write(u'\n'.join(quotes))
+            fd.write('\n'.join(quotes))
 
     @irc3.event(irc3.rfc.MY_PRIVMSG)
     def on_message(self, mask=None, event=None, target=None, data=None, **kw):
         with codecs.open(self.db, 'ab+', encoding=self.bot.encoding) as fd:
             fd.write(data + '\n')
 
         pos = random.randint(0, os.stat(self.db)[stat.ST_SIZE])
```

### Comparing `irc3-1.1.8/irc3/plugins/log.py` & `irc3-1.1.9/irc3/plugins/log.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/logger.py` & `irc3-1.1.9/irc3/plugins/logger.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/pager.py` & `irc3-1.1.9/irc3/plugins/pager.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/quakenet.py` & `irc3-1.1.9/irc3/plugins/quakenet.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/sasl.py` & `irc3-1.1.9/irc3/plugins/sasl.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/search.py` & `irc3-1.1.9/irc3/plugins/search.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/shell_command.py` & `irc3-1.1.9/irc3/plugins/shell_command.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 import os
 import irc3
 from irc3 import asyncio
-from functools import partial
 from irc3.plugins.command import Commands
 __doc__ = '''
 =================================================
 :mod:`irc3.plugins.shell_command` Shell commands
 =================================================
 
 Allow to quickly add commands map to a shell command.
@@ -87,33 +86,34 @@
                         if os.access(binary, os.X_OK):
                             name = os.path.splitext(filename)[0]
                             self.register_command(name, binary, skey=k)
             else:
                 self.register_command(k, v)
 
     def register_command(self, k, v, skey=None):
-        meth = partial(self.shell_command, v)
+        async def meth(*args, **kwargs):
+            await self.shell_command(v, *args, **kwargs)
         meth.__name__ = k
         meth.__doc__ = '''Run $ %s
         %%%%%s [<args>...]
         ''' % (v, k)
         p = {'permission': 'admin'}
         for opt in ('permission', 'public'):
             opt_key = '%s.%s' % (skey or k, opt)
             if opt_key in self.config:
                 p[opt] = self.config[opt_key]
         self.log.debug('Register command %s: $ %s', k, v)
         commands = self.context.get_plugin(Commands)
-        commands[k] = (p, asyncio.coroutine(meth))
+        commands[k] = (p, meth)
 
     async def shell_command(self, command, mask, target, args, **kwargs):
         env = os.environ.copy()
         env['IRC3_COMMAND_ARGS'] = ' '.join(args['<args>'])
         proc = await asyncio.create_subprocess_shell(
             command, shell=True, env=env,
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.STDOUT)
         await proc.wait()
         lines = await proc.stdout.read()
         if not isinstance(lines, str):
             lines = lines.decode('utf8')
-        return lines.split(u'\n')
+        return lines.split('\n')
```

### Comparing `irc3-1.1.8/irc3/plugins/slack.py` & `irc3-1.1.9/irc3/plugins/slack.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/social.py` & `irc3-1.1.9/irc3/plugins/social.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/storage.py` & `irc3-1.1.9/irc3/plugins/storage.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/uptime.py` & `irc3-1.1.9/irc3/plugins/uptime.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/userlist.py` & `irc3-1.1.9/irc3/plugins/userlist.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/plugins/web.py` & `irc3-1.1.9/irc3/plugins/web.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/rfc.py` & `irc3-1.1.9/irc3/rfc.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/rfc1459.txt` & `irc3-1.1.9/irc3/rfc1459.txt`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/rfc2812.txt` & `irc3-1.1.9/irc3/rfc2812.txt`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/tags.py` & `irc3-1.1.9/irc3/tags.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/template/__init__.py` & `irc3-1.1.9/irc3/template/__init__.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/template/config.ini` & `irc3-1.1.9/irc3/template/config.ini`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/template/plugin.py` & `irc3-1.1.9/irc3/template/plugin.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/testing.py` & `irc3-1.1.9/irc3/testing.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3/utils.py` & `irc3-1.1.9/irc3/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,18 +317,20 @@
         target = targets.pop(0) if mode not in noargs else None
         cleaned.append((char, mode, target))
     return cleaned
 
 
 def wraps_with_context(func, context):
     """Return a wrapped partial(func, context)"""
-    wrapped = functools.partial(func, context)
-    wrapped = functools.wraps(func)(wrapped)
     if asyncio.iscoroutinefunction(func):
-        wrapped = asyncio.coroutine(wrapped)
+        async def wrapped(*args, **kwargs):
+            return await func(context, *args, **kwargs)
+    else:
+        wrapped = functools.partial(func, context)
+    wrapped = functools.wraps(func)(wrapped)
     return wrapped
 
 
 def maybedotted(name):
     """Resolve dotted names:
 
     .. code-block:: python
```

### Comparing `irc3-1.1.8/irc3.egg-info/PKG-INFO` & `irc3-1.1.9/irc3.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: irc3
-Version: 1.1.8
+Version: 1.1.9
 Summary: plugable irc client library based on asyncio with DCC and SASL support
 Home-page: https://github.com/gawel/irc3/
 Author: Gael Pasgrimaud
 Author-email: gael@gawel.org
 License: MIT
 Keywords: irc dcc asyncio
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Communications :: Chat :: Internet Relay Chat
 Classifier: Development Status :: 5 - Production/Stable
 Provides-Extra: test
 Provides-Extra: web
 License-File: LICENSE
```

### Comparing `irc3-1.1.8/irc3.egg-info/SOURCES.txt` & `irc3-1.1.9/irc3.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,14 @@
 irc3.egg-info/entry_points.txt
 irc3.egg-info/not-zip-safe
 irc3.egg-info/requires.txt
 irc3.egg-info/top_level.txt
 irc3/dcc/__init__.py
 irc3/dcc/client.py
 irc3/dcc/manager.py
-irc3/dcc/optim.py
 irc3/plugins/__init__.py
 irc3/plugins/asynchronious.py
 irc3/plugins/autocommand.py
 irc3/plugins/autojoins.py
 irc3/plugins/casefold.py
 irc3/plugins/command.py
 irc3/plugins/core.py
```

### Comparing `irc3-1.1.8/irc3d/__init__.py` & `irc3-1.1.9/irc3d/__init__.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3d/__main__.py` & `irc3-1.1.9/irc3d/__main__.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3d/dec.py` & `irc3-1.1.9/irc3d/dec.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3d/plugins/command.py` & `irc3-1.1.9/irc3d/plugins/command.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3d/plugins/core.py` & `irc3-1.1.9/irc3d/plugins/core.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/irc3d/plugins/userlist.py` & `irc3-1.1.9/irc3d/plugins/userlist.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/setup.py` & `irc3-1.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import os
 import codecs
 from setuptools import setup
 from setuptools import find_packages
 
-version = '1.1.8'
+version = '1.1.9'
 
 install_requires = ['venusian>=3.0', 'docopt']
 test_requires = [
     'pytest-asyncio',
     'pytest-aiohttp',
     'feedparser',
     'requests',
@@ -33,17 +33,18 @@
     description=(
         "plugable irc client library based on asyncio "
         "with DCC and SASL support"
     ),
     long_description=read('README.rst'),
     classifiers=[
         'Intended Audience :: Developers',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
         'Topic :: Communications :: Chat :: Internet Relay Chat',
         'Development Status :: 5 - Production/Stable',
     ],
     keywords='irc dcc asyncio',
     author='Gael Pasgrimaud',
     author_email='gael@gawel.org',
```

### Comparing `irc3-1.1.8/tests/feed.atom` & `irc3-1.1.9/tests/feed.atom`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_async.py` & `irc3-1.1.9/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_autocommand.py` & `irc3-1.1.9/tests/test_autocommand.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_autojoins.py` & `irc3-1.1.9/tests/test_autojoins.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_bot.py` & `irc3-1.1.9/tests/test_bot.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_casefold.py` & `irc3-1.1.9/tests/test_casefold.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,18 @@
         bot = self.callFTU(server_config={'CASEMAPPING': 'ascii'})
 
         self.assertEquals(bot.casefold('#testchan\\123[]56'),
                           '#testchan\\123[]56')
         self.assertEquals(bot.casefold('#tESt[]chAn'), '#test[]chan')
         self.assertEquals(bot.casefold('#TEsT\\CHaN'), '#test\\chan')
 
-        self.assertEquals(bot.casefold(u'#TEsT\\CHaN'), u'#test\\chan')
+        self.assertEquals(bot.casefold('#TEsT\\CHaN'), '#test\\chan')
 
     def test_rfc1459(self):
         bot = self.callFTU(server_config={'CASEMAPPING': 'rfc1459'})
 
         self.assertEquals(bot.casefold('#testchan\\123[]56'),
                           '#testchan|123{}56')
         self.assertEquals(bot.casefold('#tESt[]chAn'), '#test{}chan')
         self.assertEquals(bot.casefold('#TEsT\\CHaN'), '#test|chan')
 
-        self.assertEquals(bot.casefold(u'#TEsT\\CHaN'), u'#test|chan')
+        self.assertEquals(bot.casefold('#TEsT\\CHaN'), '#test|chan')
```

### Comparing `irc3-1.1.8/tests/test_commands.py` & `irc3-1.1.9/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_cron.py` & `irc3-1.1.9/tests/test_cron.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
     @cron.cron('* * * * * *')
     def method(self):
         return self.bot
 
 
 @cron.cron('* * * * * *')
-@asyncio.coroutine
-def function(bot):
+async def function(bot):
     return bot
 
 
 class TestCron(BotTestCase):
 
     config = dict(includes=['irc3.plugins.cron'])
```

### Comparing `irc3-1.1.8/tests/test_ctcp.py` & `irc3-1.1.9/tests/test_ctcp.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_dcc.py` & `irc3-1.1.9/tests/test_dcc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 from irc3.testing import BotTestCase
 from irc3.compat import asyncio
 from irc3.dcc.client import DCCSend
-from irc3.dcc.optim import DCCSend as DCCSendOptim
 from irc3.plugins.dcc import dcc_command
 from irc3 import dcc_event
 from irc3 import utils
 import tempfile
 import pytest
 import shutil
 import os
@@ -141,19 +140,14 @@
         info = self.manager.connections['get']['masks'][self.dmask]
         assert proto not in info.values()
         assert proto.started.result() is proto
         assert proto.closed.done()
         self.assertFileSent()
 
 
-class TestSendOptim(TestSend):
-
-    send_class = DCCSendOptim
-
-
 class TestResume(DCCTestCase):
 
     send_class = DCCSend
 
     def created(self, f):
         with open(self.dst, 'wb') as fd:
             with open(self.src, 'rb') as fdd:
@@ -176,19 +170,14 @@
         info = self.manager.connections['get']['masks'][self.dmask]
         assert proto not in info.values()
         assert proto.started.result() is proto
         assert proto.closed.done()
         self.assertFileSent()
 
 
-class TestResumeOptim(TestResume):
-
-    send_class = DCCSendOptim
-
-
 class TestSendWithLimit(DCCTestCase):
 
     send_class = DCCSend
 
     def created(self, f):
         self.client = self.manager.create(
             'get', self.dmask,
@@ -204,12 +193,7 @@
         proto = self.client
         assert proto.transport is not None
         info = self.manager.connections['get']['masks'][self.dmask]
         assert proto not in info.values()
         assert proto.started.result() is proto
         assert proto.closed.done()
         self.assertFileSent()
-
-
-class TestSendWithLimitOptim(TestSendWithLimit):
-
-    send_class = DCCSendOptim
```

### Comparing `irc3-1.1.8/tests/test_dec.py` & `irc3-1.1.9/tests/test_dec.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_events.py` & `irc3-1.1.9/tests/test_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,16 +47,15 @@
             'PRIVMSG #irc3 :<nono> foo: Hi!',
         ])
 
     def test_async_event(self):
         loop = asyncio.new_event_loop()
         future = asyncio.Future(loop=loop)
 
-        @asyncio.coroutine
-        def e(ctx, **kwargs):
+        async def e(ctx, **kwargs):
             ctx.privmsg('#irc3', 'async')
             future.set_result(ctx)
 
         bot = self.callFTU(loop=loop)
 
         e = irc3.utils.wraps_with_context(e, bot)
         bot.attach_events(irc3.event(irc3.rfc.PRIVMSG, e))
```

### Comparing `irc3-1.1.8/tests/test_feeds.py` & `irc3-1.1.9/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_fifo.py` & `irc3-1.1.9/tests/test_fifo.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_irc3d.py` & `irc3-1.1.9/tests/test_irc3d.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_irc3d_commands.py` & `irc3-1.1.9/tests/test_irc3d_commands.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_irc3d_userlist.py` & `irc3-1.1.9/tests/test_irc3d_userlist.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_logger.py` & `irc3-1.1.9/tests/test_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                     self.logdir,
                     '{host}-{channel}-{date:%Y-%m-%d}.log')
             )}
         )
         filenames = os.listdir(self.logdir)
         self.assertEqual(len(filenames), 0, filenames)
 
-        bot.dispatch(u':server 332 foo #foo :topîc')
+        bot.dispatch(':server 332 foo #foo :topîc')
         filenames = glob.glob(os.path.join(self.logdir, '*.log'))
         self.assertEqual(len(filenames), 1, filenames)
 
         with open(filenames[0]) as fd:
             self.assertIn('server has set topic to: topîc', fd.read())
 
         bot.dispatch(':bar!user@host JOIN #foo')
```

### Comparing `irc3-1.1.8/tests/test_paginate.py` & `irc3-1.1.9/tests/test_paginate.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_protocol.py` & `irc3-1.1.9/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_quakenet.py` & `irc3-1.1.9/tests/test_quakenet.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_reconn.py` & `irc3-1.1.9/tests/test_reconn.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_reload.py` & `irc3-1.1.9/tests/test_reload.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_run.py` & `irc3-1.1.9/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_sasl.py` & `irc3-1.1.9/tests/test_sasl.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_search.py` & `irc3-1.1.9/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_slack.py` & `irc3-1.1.9/tests/test_slack.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_social.py` & `irc3-1.1.9/tests/test_social.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     config = dict(
         includes=['irc3.plugins.social'],
         twitter=dict(key='', secret='', token='', token_secret=''),
     )
 
     def test_get_conn(self):
         bot = self.callFTU()
-        conn = bot.get_social_connection(id='twitter')
+        conn = bot.get_social_connection()
         self.assertTrue(hasattr(conn, 'conn'))
 
     def test_conns(self):
         bot = self.callFTU()
         plugin = bot.get_plugin('irc3.plugins.social.Social')
         self.assertIn('twitter', plugin.conns)
```

### Comparing `irc3-1.1.8/tests/test_template.py` & `irc3-1.1.9/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_uptime.py` & `irc3-1.1.9/tests/test_uptime.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_userlist.py` & `irc3-1.1.9/tests/test_userlist.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_utils.py` & `irc3-1.1.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tests/test_web.py` & `irc3-1.1.9/tests/test_web.py`

 * *Files identical despite different names*

### Comparing `irc3-1.1.8/tox.ini` & `irc3-1.1.9/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tox]
-envlist = py35,py36,py37,py38,py39,py310,flake8,docs
+envlist = py37,py38,py39,py310,py311,flake8,docs
 
 [testenv]
 skipsdist=true
 skip_install=true
-whitelist_externals=
+allowlist_externals =
     rm
 commands =
     rm -f .coverage
     coverage run {envbindir}/py.test -xv []
     coverage report -m
 deps =
     -e .[test,web]
```

